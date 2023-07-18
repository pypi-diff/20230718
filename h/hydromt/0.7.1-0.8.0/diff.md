# Comparing `tmp/hydromt-0.7.1.tar.gz` & `tmp/hydromt-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydromt-0.7.1.tar", last modified: Fri Apr 14 06:43:26 2023, max compression
+gzip compressed data, was "hydromt-0.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `hydromt-0.7.1.tar` & `hydromt-0.8.0.tar`

### file list

```diff
@@ -1,54 +1,65 @@
--rw-r--r--   0        0        0     1419 2023-04-14 06:43:16.410205 hydromt-0.7.1/.gitignore
--rw-r--r--   0        0        0     1833 2023-04-14 06:43:16.410205 hydromt-0.7.1/.zenodo.json
--rw-r--r--   0        0        0     1075 2023-04-14 06:43:16.410205 hydromt-0.7.1/LICENSE
--rw-r--r--   0        0        0     5933 2023-04-14 06:43:16.410205 hydromt-0.7.1/README.rst
--rw-r--r--   0        0        0     2679 2023-04-14 06:43:16.410205 hydromt-0.7.1/data/catalogs/README.rst
--rw-r--r--   0        0        0      449 2023-04-14 06:43:16.410205 hydromt-0.7.1/data/catalogs/aws_data.yml
--rw-r--r--   0        0        0     1543 2023-04-14 06:43:16.410205 hydromt-0.7.1/data/catalogs/changelog.rst
--rw-r--r--   0        0        0    48760 2023-04-14 06:43:16.410205 hydromt-0.7.1/data/catalogs/deltares_data.yml
--rw-r--r--   0        0        0    11367 2023-04-14 06:43:16.414205 hydromt-0.7.1/data/catalogs/gcs_cmip6_data.yml
--rw-r--r--   0        0        0     1464 2023-04-14 06:43:16.414205 hydromt-0.7.1/data/predefined_catalogs.yml
--rw-r--r--   0        0        0     4272 2023-04-14 06:43:16.414205 hydromt-0.7.1/data/src/chirps_download_convert.py
--rw-r--r--   0        0        0    23908 2023-04-14 06:43:16.414205 hydromt-0.7.1/data/src/era5_download_resample_convert.py
--rw-r--r--   0        0        0      243 2023-04-14 06:43:16.426206 hydromt-0.7.1/environment.yml
--rw-r--r--   0        0        0      526 2023-04-14 06:43:16.430206 hydromt-0.7.1/hydromt/__init__.py
--rw-r--r--   0        0        0      931 2023-04-14 06:43:16.430206 hydromt-0.7.1/hydromt/_compat.py
--rw-r--r--   0        0        0       71 2023-04-14 06:43:16.430206 hydromt-0.7.1/hydromt/cli/__init__.py
--rw-r--r--   0        0        0     6142 2023-04-14 06:43:16.430206 hydromt-0.7.1/hydromt/cli/api.py
--rw-r--r--   0        0        0     3300 2023-04-14 06:43:16.430206 hydromt-0.7.1/hydromt/cli/cli_utils.py
--rw-r--r--   0        0        0    10754 2023-04-14 06:43:16.430206 hydromt-0.7.1/hydromt/cli/main.py
--rw-r--r--   0        0        0     8266 2023-04-14 06:43:16.430206 hydromt-0.7.1/hydromt/config.py
--rw-r--r--   0        0        0      188 2023-04-14 06:43:16.430206 hydromt-0.7.1/hydromt/data_adapter/__init__.py
--rw-r--r--   0        0        0     3562 2023-04-14 06:43:16.430206 hydromt-0.7.1/hydromt/data_adapter/caching.py
--rw-r--r--   0        0        0    12724 2023-04-14 06:43:16.430206 hydromt-0.7.1/hydromt/data_adapter/data_adapter.py
--rw-r--r--   0        0        0     8108 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/data_adapter/dataframe.py
--rw-r--r--   0        0        0    10099 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/data_adapter/geodataframe.py
--rw-r--r--   0        0        0    14008 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/data_adapter/geodataset.py
--rw-r--r--   0        0        0    16847 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/data_adapter/rasterdataset.py
--rw-r--r--   0        0        0    38472 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/data_catalog.py
--rw-r--r--   0        0        0      290 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/error.py
--rw-r--r--   0        0        0    28915 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/flw.py
--rw-r--r--   0        0        0    21224 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/gis_utils.py
--rw-r--r--   0        0        0    21768 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/io.py
--rw-r--r--   0        0        0     2815 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/log.py
--rw-r--r--   0        0        0     8262 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/merge.py
--rw-r--r--   0        0        0      548 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/models/__init__.py
--rw-r--r--   0        0        0    58390 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/models/model_api.py
--rw-r--r--   0        0        0     7123 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/models/model_grid.py
--rw-r--r--   0        0        0     7814 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/models/model_lumped.py
--rw-r--r--   0        0        0    19085 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/models/model_mesh.py
--rw-r--r--   0        0        0     2454 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/models/model_network.py
--rw-r--r--   0        0        0     4744 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/models/model_plugins.py
--rw-r--r--   0        0        0    94702 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/raster.py
--rw-r--r--   0        0        0       72 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/stats/__init__.py
--rw-r--r--   0        0        0    13667 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/stats/skills.py
--rw-r--r--   0        0        0    32517 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/vector.py
--rw-r--r--   0        0        0      120 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/workflows/__init__.py
--rw-r--r--   0        0        0    18494 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/workflows/basin_mask.py
--rw-r--r--   0        0        0    26008 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/workflows/forcing.py
--rw-r--r--   0        0        0     6568 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/workflows/rivers.py
--rw-r--r--   0        0        0      592 2023-04-14 06:43:16.434206 hydromt-0.7.1/joss_paper/citation.bib
--rw-r--r--   0        0        0    15298 2023-04-14 06:43:16.438206 hydromt-0.7.1/joss_paper/paper.bib
--rw-r--r--   0        0        0    12874 2023-04-14 06:43:16.438206 hydromt-0.7.1/joss_paper/paper.md
--rw-r--r--   0        0        0     2319 2023-04-14 06:43:16.438206 hydromt-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     7916 1970-01-01 00:00:00.000000 hydromt-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0       18 2023-07-18 14:01:13.143138 hydromt-0.8.0/.act_event.json
+-rw-r--r--   0        0        0      164 2023-07-18 14:01:13.143138 hydromt-0.8.0/.actrc
+-rw-r--r--   0        0        0      625 2023-07-18 14:01:13.143138 hydromt-0.8.0/.binder/Dockerfile
+-rw-r--r--   0        0        0       12 2023-07-18 14:01:13.143138 hydromt-0.8.0/.dockerignore
+-rw-r--r--   0        0        0     1464 2023-07-18 14:01:13.143138 hydromt-0.8.0/.gitignore
+-rw-r--r--   0        0        0      591 2023-07-18 14:01:13.143138 hydromt-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1833 2023-07-18 14:01:13.143138 hydromt-0.8.0/.zenodo.json
+-rw-r--r--   0        0        0      190 2023-07-18 14:01:13.143138 hydromt-0.8.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     2987 2023-07-18 14:01:13.143138 hydromt-0.8.0/Dockerfile
+-rw-r--r--   0        0        0     1075 2023-07-18 14:01:13.143138 hydromt-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1937 2023-07-18 14:01:13.143138 hydromt-0.8.0/Makefile
+-rw-r--r--   0        0        0     5916 2023-07-18 14:01:13.143138 hydromt-0.8.0/README.rst
+-rw-r--r--   0        0        0     2642 2023-07-18 14:01:13.143138 hydromt-0.8.0/data/catalogs/README.rst
+-rw-r--r--   0        0        0      454 2023-07-18 14:01:13.143138 hydromt-0.8.0/data/catalogs/aws_data.yml
+-rw-r--r--   0        0        0     1541 2023-07-18 14:01:13.143138 hydromt-0.8.0/data/catalogs/changelog.rst
+-rw-r--r--   0        0        0    49044 2023-07-18 14:01:13.143138 hydromt-0.8.0/data/catalogs/deltares_data.yml
+-rw-r--r--   0        0        0    11277 2023-07-18 14:01:13.143138 hydromt-0.8.0/data/catalogs/gcs_cmip6_data.yml
+-rw-r--r--   0        0        0     1440 2023-07-18 14:01:13.143138 hydromt-0.8.0/data/predefined_catalogs.yml
+-rw-r--r--   0        0        0     5220 2023-07-18 14:01:13.143138 hydromt-0.8.0/data/src/chirps_download_convert.py
+-rw-r--r--   0        0        0    24831 2023-07-18 14:01:13.143138 hydromt-0.8.0/data/src/era5_download_resample_convert.py
+-rw-r--r--   0        0        0      699 2023-07-18 14:01:13.159138 hydromt-0.8.0/hydromt/__init__.py
+-rw-r--r--   0        0        0      913 2023-07-18 14:01:13.159138 hydromt-0.8.0/hydromt/_compat.py
+-rw-r--r--   0        0        0       71 2023-07-18 14:01:13.159138 hydromt-0.8.0/hydromt/cli/__init__.py
+-rw-r--r--   0        0        0     6028 2023-07-18 14:01:13.159138 hydromt-0.8.0/hydromt/cli/api.py
+-rw-r--r--   0        0        0     3540 2023-07-18 14:01:13.159138 hydromt-0.8.0/hydromt/cli/cli_utils.py
+-rw-r--r--   0        0        0    10841 2023-07-18 14:01:13.159138 hydromt-0.8.0/hydromt/cli/main.py
+-rw-r--r--   0        0        0     8431 2023-07-18 14:01:13.159138 hydromt-0.8.0/hydromt/config.py
+-rw-r--r--   0        0        0      405 2023-07-18 14:01:13.159138 hydromt-0.8.0/hydromt/data_adapter/__init__.py
+-rw-r--r--   0        0        0     3804 2023-07-18 14:01:13.159138 hydromt-0.8.0/hydromt/data_adapter/caching.py
+-rw-r--r--   0        0        0    15510 2023-07-18 14:01:13.159138 hydromt-0.8.0/hydromt/data_adapter/data_adapter.py
+-rw-r--r--   0        0        0    10001 2023-07-18 14:01:13.159138 hydromt-0.8.0/hydromt/data_adapter/dataframe.py
+-rw-r--r--   0        0        0    11769 2023-07-18 14:01:13.159138 hydromt-0.8.0/hydromt/data_adapter/geodataframe.py
+-rw-r--r--   0        0        0    16237 2023-07-18 14:01:13.163138 hydromt-0.8.0/hydromt/data_adapter/geodataset.py
+-rw-r--r--   0        0        0    18245 2023-07-18 14:01:13.163138 hydromt-0.8.0/hydromt/data_adapter/rasterdataset.py
+-rw-r--r--   0        0        0    42042 2023-07-18 14:01:13.163138 hydromt-0.8.0/hydromt/data_catalog.py
+-rw-r--r--   0        0        0      375 2023-07-18 14:01:13.163138 hydromt-0.8.0/hydromt/error.py
+-rw-r--r--   0        0        0    29978 2023-07-18 14:01:13.163138 hydromt-0.8.0/hydromt/flw.py
+-rw-r--r--   0        0        0    21450 2023-07-18 14:01:13.163138 hydromt-0.8.0/hydromt/gis_utils.py
+-rw-r--r--   0        0        0    22598 2023-07-18 14:01:13.163138 hydromt-0.8.0/hydromt/io.py
+-rw-r--r--   0        0        0     3131 2023-07-18 14:01:13.163138 hydromt-0.8.0/hydromt/log.py
+-rw-r--r--   0        0        0     8282 2023-07-18 14:01:13.163138 hydromt-0.8.0/hydromt/merge.py
+-rw-r--r--   0        0        0      410 2023-07-18 14:01:13.163138 hydromt-0.8.0/hydromt/models/__init__.py
+-rw-r--r--   0        0        0    62405 2023-07-18 14:01:13.163138 hydromt-0.8.0/hydromt/models/model_api.py
+-rw-r--r--   0        0        0    28701 2023-07-18 14:01:13.163138 hydromt-0.8.0/hydromt/models/model_grid.py
+-rw-r--r--   0        0        0     8223 2023-07-18 14:01:13.163138 hydromt-0.8.0/hydromt/models/model_lumped.py
+-rw-r--r--   0        0        0    21089 2023-07-18 14:01:13.163138 hydromt-0.8.0/hydromt/models/model_mesh.py
+-rw-r--r--   0        0        0     2588 2023-07-18 14:01:13.163138 hydromt-0.8.0/hydromt/models/model_network.py
+-rw-r--r--   0        0        0     5511 2023-07-18 14:01:13.163138 hydromt-0.8.0/hydromt/models/model_plugins.py
+-rw-r--r--   0        0        0   103066 2023-07-18 14:01:13.163138 hydromt-0.8.0/hydromt/raster.py
+-rw-r--r--   0        0        0      126 2023-07-18 14:01:13.163138 hydromt-0.8.0/hydromt/stats/__init__.py
+-rw-r--r--   0        0        0     3974 2023-07-18 14:01:13.163138 hydromt-0.8.0/hydromt/stats/design_events.py
+-rw-r--r--   0        0        0    29251 2023-07-18 14:01:13.163138 hydromt-0.8.0/hydromt/stats/extremes.py
+-rw-r--r--   0        0        0    13701 2023-07-18 14:01:13.163138 hydromt-0.8.0/hydromt/stats/skills.py
+-rw-r--r--   0        0        0    36302 2023-07-18 14:01:13.163138 hydromt-0.8.0/hydromt/vector.py
+-rw-r--r--   0        0        0      141 2023-07-18 14:01:13.163138 hydromt-0.8.0/hydromt/workflows/__init__.py
+-rw-r--r--   0        0        0    18795 2023-07-18 14:01:13.163138 hydromt-0.8.0/hydromt/workflows/basin_mask.py
+-rw-r--r--   0        0        0    26872 2023-07-18 14:01:13.163138 hydromt-0.8.0/hydromt/workflows/forcing.py
+-rw-r--r--   0        0        0    13821 2023-07-18 14:01:13.163138 hydromt-0.8.0/hydromt/workflows/grid.py
+-rw-r--r--   0        0        0     6708 2023-07-18 14:01:13.163138 hydromt-0.8.0/hydromt/workflows/rivers.py
+-rw-r--r--   0        0        0      582 2023-07-18 14:01:13.163138 hydromt-0.8.0/joss_paper/citation.bib
+-rw-r--r--   0        0        0    15299 2023-07-18 14:01:13.163138 hydromt-0.8.0/joss_paper/paper.bib
+-rw-r--r--   0        0        0    12867 2023-07-18 14:01:13.163138 hydromt-0.8.0/joss_paper/paper.md
+-rw-r--r--   0        0        0     3403 2023-07-18 14:01:13.167138 hydromt-0.8.0/make_env.py
+-rw-r--r--   0        0        0     5571 2023-07-18 14:01:13.167138 hydromt-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     8811 1970-01-01 00:00:00.000000 hydromt-0.8.0/PKG-INFO
```

### Comparing `hydromt-0.7.1/.gitignore` & `hydromt-0.8.0/.gitignore`

 * *Files 16% similar despite different names*

```diff
@@ -97,14 +97,15 @@
 .env
 .venv
 env/
 venv/
 ENV/
 env.bak/
 venv.bak/
+*environment.yml
 
 # Spyder project settings
 .spyderproject
 .spyproject
 
 # VScode
 .vscode
@@ -118,8 +119,11 @@
 # mkdocs documentation
 /site
 
 # mypy
 .mypy_cache/
 
 # dask
-dask-worker-space/
+dask-worker-space/
+
+#ruff linting
+.ruff_cache
```

### Comparing `hydromt-0.7.1/.zenodo.json` & `hydromt-0.8.0/.zenodo.json`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.1/LICENSE` & `hydromt-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.1/README.rst` & `hydromt-0.8.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -5,48 +5,48 @@
 ===============================================================
 
 |pypi| |conda forge| |docs_latest| |docs_stable| |binder| |codecov| |license| |doi| |joss_paper|
 
 
 What is HydroMT?
 ----------------
-**HydroMT** (Hydro Model Tools) is an open-source Python package that facilitates the process of 
-building and analyzing spatial geoscientific models with a focus on water system models. 
-It does so by automating the workflow to go from raw data to a complete model instance which 
-is ready to run and to analyse model results once the simulation has finished. 
-HydroMT builds on the latest packages in the scientific and geospatial python eco-system including 
+**HydroMT** (Hydro Model Tools) is an open-source Python package that facilitates the process of
+building and analyzing spatial geoscientific models with a focus on water system models.
+It does so by automating the workflow to go from raw data to a complete model instance which
+is ready to run and to analyse model results once the simulation has finished.
+HydroMT builds on the latest packages in the scientific and geospatial python eco-system including
 xarray_, rasterio_, rioxarray_, geopandas_, scipy_ and pyflwdir_.
 
 
 Why HydroMT?
 ------------
-Setting up spatial geoscientific models typically requires many (manual) steps 
-to process input data and might therefore be time consuming and hard to reproduce. 
-Especially improving models based on global geospatial datasets, which are 
-rapidly becoming available at increasingly high resolutions, might be challenging. 
-Furthermore, analyzing model schematization and results from different models, 
+Setting up spatial geoscientific models typically requires many (manual) steps
+to process input data and might therefore be time consuming and hard to reproduce.
+Especially improving models based on global geospatial datasets, which are
+rapidly becoming available at increasingly high resolutions, might be challenging.
+Furthermore, analyzing model schematization and results from different models,
 which often use model-specific peculiar data formats, can be time consuming.
-This package aims to make the model building process **fast**, **modular** and **reproducible** 
+This package aims to make the model building process **fast**, **modular** and **reproducible**
 by configuring the model building process from a single *ini* configuration file
-and **model- and data-agnostic** through a common model and data interface. 
+and **model- and data-agnostic** through a common model and data interface.
 
 
 How to use HydroMT?
 -------------------
 HydroMT can be used as a **command line** application (CLI) which provides commands to *build*,
 *update* and *clip* models with a single line, or **from Python** to exploit its rich interface.
 You can learn more about how to use HydroMT in its `online documentation. <https://deltares.github.io/hydromt/latest/>`_
-For a smooth installing experience, we recommend installing HydroMT and its dependencies 
+For a smooth installing experience, we recommend installing HydroMT and its dependencies
 from conda-forge in a clean environment, see `installation guide. <https://deltares.github.io/hydromt/latest/getting_started/installation>`_
 
 
 HydroMT model plugins
 ---------------------
-HydroMT is commonly used in combination with a **model plugin** which 
-provides a HydroMT implementation for specific model software. Using the plugins allows to prepare a ready-to-run set of input files from raw geoscientific datasets and analyse model results in a fast and reproducible way. 
+HydroMT is commonly used in combination with a **model plugin** which
+provides a HydroMT implementation for specific model software. Using the plugins allows to prepare a ready-to-run set of input files from raw geoscientific datasets and analyse model results in a fast and reproducible way.
 Known model plugins include:
 
 * hydromt_wflow_: A framework for distributed rainfall-runoff (wflow_sbm) and sediment transport (wflow_sediment) modelling.
 * hydromt_delwaq_: A framework for water quality (D-Water Quality) and emissions (D-Emissions) modelling.
 * hydromt_sfincs_: A fast 2D hydrodynamic flood model (SFINCS).
 * hydromt_fiat_: A flood impact model (FIAT).
 
@@ -62,17 +62,17 @@
 
 
 How to contribute?
 -------------------
 If you find any issues in the code or documentation feel free to leave an issue on the `github issue tracker. <https://github.com/Deltares/hydromt/issues>`_
 You can find information about how to contribute to the HydroMT project at our `contributing page. <https://deltares.github.io/hydromt/latest/dev/contributing>`_
 
-HydroMT seeks active contribution from the (hydro) geoscientific community. 
-So far, it has been developed and tested with a range of `Deltares <https://www.deltares.nl/en/>`_ models, but 
-we believe it is applicable to a much wider set of geoscientific models and are 
+HydroMT seeks active contribution from the (hydro) geoscientific community.
+So far, it has been developed and tested with a range of `Deltares <https://www.deltares.nl/en/>`_ models, but
+we believe it is applicable to a much wider set of geoscientific models and are
 happy to discuss how it can be implemented for your model.
 
 
 .. _scipy: https://scipy.org/
 .. _xarray: https://xarray.pydata.org
 .. _geopandas: https://geopandas.org
 .. _rioxarray: https://corteva.github.io/rioxarray/stable/
@@ -112,8 +112,8 @@
     :target: https://zenodo.org/badge/latestdoi/348020332
 
 .. |license| image:: https://img.shields.io/github/license/Deltares/hydromt?style=flat
     :alt: License
     :target: https://github.com/Deltares/hydromt/blob/main/LICENSE
 
 .. |joss_paper| image:: https://joss.theoj.org/papers/10.21105/joss.04897/status.svg
-   :target: https://doi.org/10.21105/joss.04897
+   :target: https://doi.org/10.21105/joss.04897
```

### Comparing `hydromt-0.7.1/data/catalogs/README.rst` & `hydromt-0.8.0/data/catalogs/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,103 +1,100 @@
 ========================
 Predefined Data Catalogs
 ========================
 
-This readme file contains information about the predefined data catalogs which be accessed through HydroMT. 
+This readme file contains information about the predefined data catalogs which be accessed through HydroMT.
 The data can be browsed through in the (predefined data catalogs of the HydroMT docs)[https://deltares.github.io/hydromt/latest/user_guide/data_existing_cat.html]
 For more information regarding working with data catalogs we refer the user to the (HydroMT user guide)[https://deltares.github.io/hydromt/latest/user_guide/data_main.html]
 
 deltares_data
 =============
 
-The HydroMT Deltares Data is managed by the HydroMT team. 
+The HydroMT Deltares Data is managed by the HydroMT team.
 For adding new data to the deltares_data.yml please follow the conventions given hereinafter.
 The data is currently only stored on the deltares server: p:/wflow_global/hydromt
 
 preferred data formats to download
 -----------------------------------
 vector data: flatgeobuf (because they contain a spatial index and are therefore much faster)
 raster data (2D): cloud optimized geotiff
 raster data (3D): zarr
 
 data storage (p:/wflow_global/hydromt)
 --------------------------------------
 
 data used by the geoserver:
 DO NOT CHAGE WITHOUT CONSULTATION
-- alosdem 
-- copdem 
+- alosdem
+- copdem
 
 writing convention:
-- lower case 
+- lower case
 - with underscores
 
-folder structure: 
+folder structure:
 - no subcategories
 
- 1. data type (category) 
+ 1. data type (category)
  	bathymetry
  	geography
  	hydro
  	hydrography
  	infrastructure
  	landuse
  	meteo
  	ocean
  	sociao_economic
  	soil
- 	topography 
- 2. data name 
+ 	topography
+ 2. data name
  	e.g.:
  	era5
  	eobs
  	grdc
  	osm
  	...
 (3. parameter)
 	e.g.:
 	t2m
 	msl
 	...
-       
+
 deltares_data.yml
 ------------------
 writing convention:
 - lower case
 - with underscore
 - the key "data_type" follows this convention but the data type itself is written in cam case (RasterDataset/GeoDataFrame/GeoDataset)
 - two spaces for indentation
 
-data versioning: 	
+data versioning:
 - data always refers to a specific version
-- version is indicated within the name of the alias 
-- short name refers to that version 
+- version is indicated within the name of the alias
+- short name refers to that version
 - convention: [data_name]_v[version_number]
 - e.g. eobs_v22.0e
 
-structure per data set: 
-- use placeholders where possible 
+structure per data set:
+- use placeholders where possible
 - order the data sets alphabetically
 - order the components of each data set alphabetically
-- for adding meta data use the following optional keys: 
-	
+- for adding meta data use the following optional keys:
+
 category:
 notes:
-paper_doi: 
-paper_ref: 
+paper_doi:
+paper_ref:
 source_author: (if different from paper_ref)
-source_license: 
-source_url: 
-source_version: 
+source_license:
+source_url:
+source_version:
 unit:
-	
-updates 
+
+updates
 -------
 
 - create new branch on github
 - make changes and bump the version in the global meta section using `calendar versioning <https://calver.org/>`
 - test your yml file (Can the added/changed data sources be read through HydroMT?)
 - create pull request
-- add new version to hydromt\data\predefined_catalogs.yml 
-
-	
-	
+- add new version to hydromt\data\predefined_catalogs.yml
```

### Comparing `hydromt-0.7.1/data/catalogs/changelog.rst` & `hydromt-0.8.0/data/catalogs/changelog.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ==============================
 Change log predefined datasets
 ==============================
 
-deltares_data 
+deltares_data
 =============
 
 version: 2023.2
 ----------------
 
 changed
 ^^^^^^^
@@ -39,18 +39,18 @@
 	- eobs_orography_v24.0e
 	- eobs_orography_v25.0e
 	- SM2RAIN_ASCAT_monthly_025_v1.4
 	- SM2RAIN_ASCAT_monthly_05_v1.4
 
 changed
 ^^^^^^^
-- Apply convention specified in the README 
+- Apply convention specified in the README
 	- check reasonable alphabetical order in data sets and components
 	- implement right versioning convention _v where possible
-	- apply consistent meta information 
+	- apply consistent meta information
 
 fixed
 ^^^^^
 - enable versioning of yml.files
 
 cmip6_data
 ==========
@@ -66,8 +66,8 @@
 ========
 
 version: 2023.2
 ---------------
 
 added
 ^^^^^
-- ESA Worldcover v100 2020.
+- ESA Worldcover v100 2020.
```

### Comparing `hydromt-0.7.1/data/catalogs/deltares_data.yml` & `hydromt-0.8.0/data/catalogs/deltares_data.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,63 +1,65 @@
+---
 meta:
   root: p:/wflow_global/hydromt
-  version: 2023.2
+  version: 2023.3
 
-basin_atlas_level12_v10: 
+
+basin_atlas_level12_v10:
   crs: 4326
   data_type: GeoDataFrame
   driver: vector
   kwargs:
     layer: BasinATLAS_v10_lev12
   meta:
     category: hydrography
-    notes: renaming and units might require some revision 
+    notes: renaming and units might require some revision
     paper_doi: 10.1038/s41597-019-0300-6
     paper_ref: Linke et al. (2019)
     source_license: CC BY 4.0
     source_url: https://www.hydrosheds.org/hydroatlas
     source_version: 10
   path: hydrography/hydro_atlas/basin_atlas_v10.gpkg
-  
-river_atlas_v10: 
+
+river_atlas_v10:
   crs: 4326
   data_type: GeoDataFrame
   driver: vector
   meta:
     category: hydrography
-    notes: renaming and units might require some revision 
+    notes: renaming and units might require some revision
     paper_doi: 10.1038/s41597-019-0300-6
     paper_ref: Linke et al. (2019)
     source_license: CC BY 4.0
     source_url: https://www.hydrosheds.org/hydroatlas
     source_version: 10
   path: hydrography/hydro_atlas/river_atlas_v10.gpkg
-  rename:    
+  rename:
     dis_m3_pyr: Dis_avg
 
-lake_atlas_pol_v10: 
+lake_atlas_pol_v10:
   crs: 4326
   data_type: GeoDataFrame
   driver: vector
   kwargs:
     layer: LakeATLAS_v10_pol
   meta:
     category: hydrography
-    notes: renaming and units might require some revision 
+    notes: renaming and units might require some revision
     paper_doi: 10.1038/s41597-022-01425-z
     paper_ref: Lehner et al. (2022)
     source_license: CC BY 4.0
     source_url: https://www.hydrosheds.org/hydroatlas
     source_version: 10
   path: hydrography/hydro_atlas/lake_atlas_v10.gpkg
-  rename:  
+  rename:
     dis_m3_pyr: Dis_avg
- 
+
 chelsa:
-  alias: chelsa_v1.2 
+  alias: chelsa_v1.2
 chelsa_v1.2:
   crs: 4326
   data_type: RasterDataset
   driver: raster
   kwargs:
     chunks:
       x: 3600
@@ -134,53 +136,53 @@
     chunks:
       x: 3600
       y: 3600
   meta:
     category: topography
     source_license: https://spacedata.copernicus.eu/documents/20126/0/CSCDA_ESA_Mission-specific+Annex+%281%29.pdf/83b44c0a-244a-7ba3-b00c-b578a34e88a7?t=1604070311399
     source_url: https://spacedata.copernicus.eu/web/cscda/dataset-details?articleId=394198#D4
-    source_version: 2021_1
-  nodata: -9999  # copdem has no actual nodata, this is to suppress a missing nodata warning 
+    source_version: '2021_1'
+  nodata: -9999 # copdem has no actual nodata, this is to suppress a missing nodata warning
   path: topography/copdem/copdem.vrt
   rename:
     copdem: elevtn
 
 copdem30_mask:
   alias: copdem30_mask_v2021.1
 copdem30_mask_v2021.1:
   data_type: RasterDataset
-  driver: raster  
+  driver: raster
   kwargs:
     chunks:
       x: 3600
       y: 3600
   meta:
     category: topography
     source_license: https://spacedata.copernicus.eu/documents/20126/0/CSCDA_ESA_Mission-specific+Annex+%281%29.pdf/83b44c0a-244a-7ba3-b00c-b578a34e88a7?t=1604070311399
     source_url: https://spacedata.copernicus.eu/web/cscda/dataset-details?articleId=394198#D4
-    source_version: 2021_1
-  nodata: -1  # copdem has no actual nodata, this is to suppress a missing nodata warning 
+    source_version: '2021_1'
+  nodata: -1 # copdem has no actual nodata, this is to suppress a missing nodata warning
   path: topography/copdem/copdem_mask.vrt
   rename:
     copdem_mask: mask
 
 copdem30_masked:
   alias: copdem30_masked_v2021.1
 copdem30_masked_v2021.1:
   data_type: RasterDataset
-  driver: raster 
+  driver: raster
   kwargs:
     chunks:
       x: 3600
       y: 3600
   meta:
     category: topography
     source_license: https://spacedata.copernicus.eu/documents/20126/0/CSCDA_ESA_Mission-specific+Annex+%281%29.pdf/83b44c0a-244a-7ba3-b00c-b578a34e88a7?t=1604070311399
     source_url: https://spacedata.copernicus.eu/web/cscda/dataset-details?articleId=394198#D4
-    source_version: 2021_1
+    source_version: '2021_1'
   path: topography/copdem/copdem_masked.vrt
   rename:
     copdem_masked: elevtn
 
 corine:
   alias: corine_2018_v2020_u1
 corine_2018_v2020_u1:
@@ -228,15 +230,15 @@
     paper_doi: 10.1029/2008JC005179
     paper_ref: Andersen and Knudsen (2009)
     source_url: https://www.space.dtu.dk/english/research/scientific_data_and_models/global_mean_dynamic_topography
     source_version: 2010
     unit: m+EGM96
   path: topography/dtu10mdt/DTU10MDT_1min_egm96.tif
 
-eobs: 
+eobs:
   alias: eobs_v22.0e
 eobs_v22.0e:
   crs: 4326
   data_type: RasterDataset
   driver: netcdf
   kwargs:
     chunks:
@@ -455,16 +457,15 @@
       longitude: 240
       time: 30
     combine: by_coords
     decode_times: true
     parallel: true
   meta:
     category: meteo
-    notes: Extracted from Copernicus Climate Data Store; resampled by Deltares to
-      daily frequency
+    notes: Extracted from Copernicus Climate Data Store; resampled by Deltares to daily frequency
     paper_doi: 10.1002/qj.3803
     paper_ref: Hersbach et al. (2019)
     source_license: https://cds.climate.copernicus.eu/cdsapp/#!/terms/licence-to-use-copernicus-products
     source_url: https://doi.org/10.24381/cds.bd0915c6
     source_version: ERA5 daily data on pressure levels
   path: meteo/era5_daily/nc_merged/era5_{year}*_daily.nc
   rename:
@@ -512,16 +513,16 @@
     parallel: true
   meta:
     category: meteo
     notes: Extracted from Copernicus Climate Data Store
     paper_doi: 10.1002/qj.3803
     paper_ref: Hersbach et al. (2019)
     source_license: https://cds.climate.copernicus.eu/cdsapp/#!/terms/licence-to-use-copernicus-products
-    source_url: https://doi.org/10.24381/cds.bd0915c6
-    source_version: ERA5 hourly data on pressure levels
+    source_url: https://doi.org/10.24381/cds.adbb2d47
+    source_version: ERA5 hourly data on single levels from 1940 to present
   path: meteo/era5/{variable}/era5_{variable}_{year}*_hourly.nc
   rename:
     d2m: temp_dew
     msl: press_msl
     ssrd: kin
     t2m: temp
     tisr: kout
@@ -533,15 +534,15 @@
     temp_dew: -273.15
   unit_mult:
     kin: 0.000277778
     kout: 0.000277778
     ssr: 0.000277778
     precip: 1000
     press_msl: 0.01
-    
+
 era5_hourly_zarr:
   alias: era5_hourly
   crs: 4326
   data_type: RasterDataset
   driver: zarr
   kwargs:
     chunks: auto
@@ -578,15 +579,15 @@
       longitude: 125
   meta:
     category: meteo
     notes: Extracted from Copernicus Climate Data Store
     paper_doi: 10.1002/qj.3803
     paper_ref: Hersbach et al. (2019)
     source_license: https://cds.climate.copernicus.eu/cdsapp/#!/terms/licence-to-use-copernicus-products
-    source_url: https://doi.org/10.24381/cds.bd0915c6
+    source_url: https://apps.ecmwf.int/codes/grib/param-db?id=129
   path: meteo/era5/meta/era5_orography_2018.nc
   rename:
     z: elevtn
   unit_mult:
     elevtn: 0.10197162129779283
 
 esa_worldcover:
@@ -671,15 +672,15 @@
     source_author: gadm
     source_license: https://gadm.org/license.html
     source_url: https://gadm.org/download_world.html
     source_version: 3.6
   path: geography/gadm/gadm36_levels.gpkg
   rename:
     fid: gadm_level3
-    
+
 gcn250:
   alias: gcn250_v1
 gcn250_v1:
   data_type: RasterDataset
   driver: raster
   kwargs:
     chunks:
@@ -703,16 +704,15 @@
   alias: gdp_world_v1
 gdp_world_v1:
   crs: 4326
   data_type: GeoDataFrame
   driver: vector
   meta:
     category: socio-economic
-    notes: data combined from World Bank (https://data.worldbank.org/indicator/NY.GDP.MKTP.CD)
-      and CIA World Factbook (https://www.cia.gov/the-world-factbook/field/real-gdp-per-capita/country-comparison)
+    notes: data combined from World Bank (https://data.worldbank.org/indicator/NY.GDP.MKTP.CD) and CIA World Factbook (https://www.cia.gov/the-world-factbook/field/real-gdp-per-capita/country-comparison)
     source_author: Wilfred Altena
     source_license: CC BY-4.0
     source_version: 1.0
   path: socio_economic/gdp_world/World_countries_GDPpcPPP.fgb
   rename:
     GDP: gdp
   unit_mult:
@@ -827,15 +827,15 @@
     category: landuse
     paper_doi: 10.1594/PANGAEA.787668
     paper_ref: Arino et al (2012)
     source_license: CC-BY-3.0
     source_url: http://due.esrin.esa.int/page_globcover.php
     source_version: v2.3
   path: landuse/globcover/GLOBCOVER_L4_200901_200912_V2.3.tif
-  
+
 glofas_era5_v31:
   crs: 4326
   data_type: RasterDataset
   driver: netcdf
   kwargs:
     chunks:
       time: 180
@@ -1244,15 +1244,15 @@
 merit:
   alias: merit_v1.0.3
 merit_v1.0.3:
   crs: 4326
   data_type: RasterDataset
   driver: netcdf
   kwargs:
-    drop_variables: 'projection'
+    drop_variables: projection
     chunks:
       lat: 6000
       lon: 6000
   meta:
     category: topography
     paper_doi: 10.1002/2017GL072874
     paper_ref: Yamazaki et al. (2018)
@@ -1299,39 +1299,52 @@
   driver: raster
   kwargs:
     chunks:
       x: 6000
       y: 6000
   meta:
     category: topography
-    paper_doi: 10.5281/zenodo.5166932
-    paper_ref: Eilander et al. (2020)
+    paper_doi: 10.5194/hess-2020-582
+    paper_ref: Eilander et al. (2021)
     source_license: ODC-By 1.0
     source_url: https://zenodo.org/record/5166932#.YVbxJ5pByUk
+    source_doi: 10.5281/zenodo.5166932
     source_version: 1.0
   path: topography/merit_hydro_ihu/30sec/*.tif
   rename:
     30sec_basids: basins
     30sec_flwdir: flwdir
     30sec_elevtn: elevtn
     30sec_strord: strord
     30sec_uparea: uparea
     30sec_rivlen: rivlen
     30sec_rivslp: rivslp
 
+merit_hydro_ihu_index:
+  crs: 4326
+  data_type: GeoDataFrame
+  driver: vector
+  meta:
+    category: topography
+    paper_doi: 10.5194/hess-25-5287-2021
+    paper_ref: Eilander et al. (2021)
+    source_license: CC-BY-NC 4.0
+    source_url: https://zenodo.org/record/5166932#.YVbxJ5pByUk
+  path: topography/merit_hydro_ihu/30sec/basins.gpkg
+
 merit_hydro_index:
   alias: merit_hydro_index_v1.0
 merit_hydro_index_v1.0:
   crs: 4326
   data_type: GeoDataFrame
   driver: vector
   meta:
     category: topography
-    paper_doi: 10.5194/hess-2020-582
-    paper_ref: Eilander et al. (in review)
+    paper_doi: 10.5194/hess-25-5287-2021
+    paper_ref: Eilander et al. (2021)
     source_license: CC-BY-NC 4.0
   path: topography/merit_hydro/basin_index.fgb
 
 merit_hydro_patch:
   alias: merit_hydro_patch_v1.0
 merit_hydro_patch_v1.0:
   crs: 4326
@@ -1368,16 +1381,15 @@
   kwargs:
     chunks:
       x: 3600
       y: 3600
     concat: true
   meta:
     category: landuse
-    notes: this dataset has been extracted from GEE ('MODIS/006/MCD15A3H') for the
-      period '2003-01-01', '2017-12-31'
+    notes: this dataset has been extracted from GEE ('MODIS/006/MCD15A3H') for the period '2003-01-01', '2017-12-31'
     paper_doi: 10.5067/MODIS/MCD15A3H.006
     paper_ref: Myneni et al (2015)
     source_license: https://lpdaac.usgs.gov/data/data-citation-and-policies/
     source_url: https://lpdaac.usgs.gov/products/mcd15a3hv006/
     source_version: MCD15A3H V006
   path: landuse/modis/MODIS_MCD15A3H_LAI/*.tif
   unit_mult:
@@ -1479,19 +1491,19 @@
       latitude: 360
       longitude: 720
       time: 84
   meta:
     category: meteo
     notes: crs guessed as it is neither mentioned in the data nor in the literature, 0.25-degree resolution
     paper_doi: 10.5194/essd-11-1583-2019
-    paper_ref: Brocca et al. (2019) 
+    paper_ref: Brocca et al. (2019)
     source_license: https://creativecommons.org/licenses/by/4.0/legalcode
     source_url: https://zenodo.org/record/4570192#.YueKJWNByUl
   path: meteo/sm2rain_ascat/SM2RAIN_ASCAT_monthly_025_2007_2020.nc
-  rename: 
+  rename:
     rainfall: precip
 
 SM2RAIN_ASCAT_monthly_05_v1.4:
   crs: 4326
   data_type: RasterDataset
   driver: netcdf
   kwargs:
@@ -1499,41 +1511,37 @@
       latitude: 180
       longitude: 360
       time: 84
   meta:
     category: meteo
     notes: crs guessed as it is neither mentioned in the data nor in the literature, 0.5-degree resolution
     paper_doi: 10.5194/essd-11-1583-2019
-    paper_ref: Brocca et al. (2019) 
+    paper_ref: Brocca et al. (2019)
     source_license: https://creativecommons.org/licenses/by/4.0/legalcode
     source_url: https://zenodo.org/record/4570192#.YueKJWNByUl
   path: meteo/sm2rain_ascat/SM2RAIN_ASCAT_monthly_05_2007_2020.nc
-  rename: 
-    rainfall: precip    
-  
+  rename:
+    rainfall: precip
+
 soilgrids:
   alias: soilgrids_v1.0
 soilgrids_v1.0:
   crs: 4326
   data_type: RasterDataset
   driver: raster
   kwargs:
     chunks:
       x: 2400
       y: 2400
   meta:
     category: soil
-    notes: "soilthickness is based on 1) soilgrids (global) and 2) dataset for Eurasia\
-      \ (ESDAC, 2004; Panagos et al., 2012): ESDAC, 2004. The european soil database\
-      \ distribution version 2.0, european commission and the European soil bureau\
-
-      \ network.  esdac.jrc.ec.europa.eu, accessed: 2017-11-17.  Panagos, P., Van\
-      \ Liedekerke, M., Jones, A., Montanarella, L., 2012. European soil data centre:\
-      \ Response to european policy support  and public data requirements. Land Use\
-      \ Policy 29 (2), 329\xE2\u20AC\u201C338. \n"
+    notes: "soilthickness is based on 1) soilgrids (global) and 2) dataset for Eurasia (ESDAC, 2004; Panagos et al., 2012): ESDAC, 2004. The european soil
+      database distribution version 2.0, european commission and the European soil bureau\n network.  esdac.jrc.ec.europa.eu, accessed: 2017-11-17.  Panagos,
+      P., Van Liedekerke, M., Jones, A., Montanarella, L., 2012. European soil data centre: Response to european policy support  and public data requirements.
+      Land Use Policy 29 (2), 329â€“338. \n"
     paper_doi: 10.1371/journal.pone.0169748
     paper_ref: Hengl et al. (2017)
     source_license: ODbL
     source_url: https://www.isric.org/explore/soilgrids/faq-soilgrids-2017
     source_version: 2017
   path: soil/soilgrids_v1.0/*_250m_ll.tif
   rename:
@@ -1611,21 +1619,18 @@
   driver: raster
   kwargs:
     chunks:
       x: 2400
       y: 2400
   meta:
     category: soil
-    notes: "soilthickness is based on 1) soilgrids (global) and 2) dataset for Eurasia\
-      \ (ESDAC, 2004; Panagos et al., 2012): ESDAC, 2004. The european soil database\
-      \ distribution version 2.0, european commission and the European soil bureau\
-      \ network.  esdac.jrc.ec.europa.eu, accessed: 2017-11-17.  Panagos, P., Van\
-      \ Liedekerke, M., Jones, A., Montanarella, L., 2012. European soil data centre:\
-      \ Response to european policy support  and public data requirements. Land Use\
-      \ Policy 29 (2), 329\xE2\u20AC\u201C338. \n"
+    notes: "soilthickness is based on 1) soilgrids (global) and 2) dataset for Eurasia (ESDAC, 2004; Panagos et al., 2012): ESDAC, 2004. The european soil
+      database distribution version 2.0, european commission and the European soil bureau network.  esdac.jrc.ec.europa.eu, accessed: 2017-11-17.  Panagos,
+      P., Van Liedekerke, M., Jones, A., Montanarella, L., 2012. European soil data centre: Response to european policy support  and public data requirements.
+      Land Use Policy 29 (2), 329â€“338. \n"
     paper_doi: https://doi.org/10.5194/soil-2020-65
     paper_ref: de Sousa et al. (2020)
     source_license: CC BY 4.0
     source_url: https://www.isric.org/explore/soilgrids/faq-soilgrids
     source_version: 2020
   path: soil/soilgrids_v2.0/*/*_mean.vrt
   rename:
@@ -1827,14 +1832,15 @@
       lon: 3600
   meta:
     category: meteo
     paper_doi: 10.1002/joc.5086
     paper_ref: Fick and Hijmans (2017)
     source_url: https://www.worldclim.org/data/worldclim21.html
     source_version: 2
+    nodata: -999.0
   path: meteo/worldclim_v2.0/wc2.0_30s_prec.nc
   rename:
     prec: precip
 
 worldpop_2020_constrained:
   data_type: RasterDataset
   driver: raster
@@ -1846,15 +1852,15 @@
     paper_ref: Stevens et al. (2015)
     source_license: CC BY 4.0
     source_url: https://www.worldpop.org/doi/10.5258/SOTON/WP00684
   nodata: -99999
   path: socio_economic/worldpop/ppp_2020_constrained.vrt
   rename:
     ppp_2020_constrained: population
-    
+
 worldpop_2020_UNadj_constrained:
   alias: worldpop_2020_constrained
   path: socio_economic/worldpop/ppp_2020_UNadj_constrained.vrt
   rename:
     ppp_2020_UNadj_constrained: population
 
 wsf_bld_2015:
@@ -1869,8 +1875,8 @@
       y: 1000
   meta:
     category: socio-economic
     paper_doi: 10.1038/s41597-020-00580-5
     paper_ref: Marconcini at al (2020)
     source_license: CC0 1.0
     source_url: https://un-spider.org/links-and-resources/data-sources/world-settlement-footprint-2015-wsf-dlr-eoc
-  path: infrastructure/wsf/WSF2015_v1_EPSG4326.vrt
+  path: infrastructure/wsf/WSF2015_v1_EPSG4326.vrt
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hydromt-0.7.1/data/catalogs/gcs_cmip6_data.yml` & `hydromt-0.8.0/data/catalogs/gcs_cmip6_data.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,75 +1,74 @@
+---
 meta:
   version: 2023.2
 cmip6_{model}_historical_{member}_{timestep}:
   crs: 4326
   data_type: RasterDataset
   driver: zarr
   filesystem: gcs
   kwargs:
-    drop_variables: ['time_bnds', 'lat_bnds', 'lon_bnds', 'bnds']
+    drop_variables: [time_bnds, lat_bnds, lon_bnds, bnds]
     decode_times: true
     preprocess: harmonise_dims
     consolidated: true
   meta:
     category: climate
     paper_doi: 10.1175/BAMS-D-11-00094.1
     paper_ref: Taylor et al. 2012
     source_license: CC BY 4.0
     source_url: https://console.cloud.google.com/marketplace/details/noaa-public/cmip6?_ga=2.136097265.-1784288694.1541379221&pli=1
     source_version: 1.3.1
   placeholders:
-    model: ['IPSL/IPSL-CM6A-LR','SNU/SAM0-UNICON','NCAR/CESM2','NCAR/CESM2-WACCM','INM/INM-CM4-8','INM/INM-CM5-0',
-    'NOAA-GFDL/GFDL-ESM4','NCC/NorESM2-LM','NIMS-KMA/KACE-1-0-G','CAS/FGOALS-f3-L','CSIRO-ARCCSS/ACCESS-CM2',
-    'NCC/NorESM2-MM','CSIRO/ACCESS-ESM1-5','NCAR/CESM2-WACCM-FV2','NCAR/CESM2-FV2','CMCC/CMCC-CM2-SR5',
-    'AS-RCEC/TaiESM1','NCC/NorCPM1','IPSL/IPSL-CM5A2-INCA','CMCC/CMCC-CM2-HR4','CMCC/CMCC-ESM2','IPSL/IPSL-CM6A-LR-INCA',
-    'E3SM-Project/E3SM-1-0']
-#    model: ['NOAA-GFDL/GFDL-CM4','BCC/BCC-CSM2-MR', 'BCC/BCC-ESM1', 'CCCma/CanESM5', 'MRI/MRI-ESM2-0', 
-#    'HAMMOZ-Consortium/MPI-ESM-1-2-HAM', 'MPI-M/MPI-ESM1-2-LR', 'MPI-M/MPI-ESM1-2-HR', 'NUIST/NESM3',
-#    'CAS/FGOALS-g3', 'MIROC/MIROC6', 'KIOST/KIOST-ESM', 'CCCR-IITM/IITM-ESM', 'AWI/AWI-ESM-1-1-LR',
-#    'EC-Earth-Consortium/EC-Earth3-Veg-LR', 'EC-Earth-Consortium/EC-Earth3-Veg', 
-#    'EC-Earth-Consortium/EC-Earth3', 'EC-Earth-Consortium/EC-Earth3-AerChem',
-#    'EC-Earth-Consortium/EC-Earth3-CC', 'MPI-M/ICON-ESM-LR'] # other models but were regridded to irregular grid for lat
-    member: ['r1i1p1f1']
-    timestep: ['day', 'Amon']
+    model: [IPSL/IPSL-CM6A-LR, SNU/SAM0-UNICON, NCAR/CESM2, NCAR/CESM2-WACCM, INM/INM-CM4-8, INM/INM-CM5-0, NOAA-GFDL/GFDL-ESM4, NCC/NorESM2-LM, NIMS-KMA/KACE-1-0-G,
+      CAS/FGOALS-f3-L, CSIRO-ARCCSS/ACCESS-CM2, NCC/NorESM2-MM, CSIRO/ACCESS-ESM1-5, NCAR/CESM2-WACCM-FV2, NCAR/CESM2-FV2, CMCC/CMCC-CM2-SR5, AS-RCEC/TaiESM1,
+      NCC/NorCPM1, IPSL/IPSL-CM5A2-INCA, CMCC/CMCC-CM2-HR4, CMCC/CMCC-ESM2, IPSL/IPSL-CM6A-LR-INCA, E3SM-Project/E3SM-1-0]
+    #    model: ['NOAA-GFDL/GFDL-CM4','BCC/BCC-CSM2-MR', 'BCC/BCC-ESM1', 'CCCma/CanESM5', 'MRI/MRI-ESM2-0',
+    #    'HAMMOZ-Consortium/MPI-ESM-1-2-HAM', 'MPI-M/MPI-ESM1-2-LR', 'MPI-M/MPI-ESM1-2-HR', 'NUIST/NESM3',
+    #    'CAS/FGOALS-g3', 'MIROC/MIROC6', 'KIOST/KIOST-ESM', 'CCCR-IITM/IITM-ESM', 'AWI/AWI-ESM-1-1-LR',
+    #    'EC-Earth-Consortium/EC-Earth3-Veg-LR', 'EC-Earth-Consortium/EC-Earth3-Veg',
+    #    'EC-Earth-Consortium/EC-Earth3', 'EC-Earth-Consortium/EC-Earth3-AerChem',
+    #    'EC-Earth-Consortium/EC-Earth3-CC', 'MPI-M/ICON-ESM-LR'] # other models but were regridded to irregular grid for lat
+    member: [r1i1p1f1]
+    timestep: [day, Amon]
   path: gs://cmip6/CMIP6/CMIP/{model}/historical/{member}/{timestep}/{variable}/*/*
   rename:
     pr: precip
     tas: temp
     rsds: kin
     psl: press_msl
   unit_add:
     temp: -273.15
   unit_mult:
     precip: 86400
     press_msl: 0.01
-    
+
 cmip6_{model}_ssp119_{member}_{timestep}:
   crs: 4326
   data_type: RasterDataset
   driver: zarr
   filesystem: gcs
   kwargs:
-    drop_variables: ['time_bnds', 'lat_bnds', 'lon_bnds', 'bnds']
+    drop_variables: [time_bnds, lat_bnds, lon_bnds, bnds]
     decode_times: true
     preprocess: harmonise_dims
     consolidated: true
   meta:
     category: climate
     paper_doi: 10.1175/BAMS-D-11-00094.1
     paper_ref: Taylor et al. 2012
     source_license: CC BY 4.0
     source_url: https://console.cloud.google.com/marketplace/details/noaa-public/cmip6?_ga=2.136097265.-1784288694.1541379221&pli=1
     source_version: 1.3.1
   placeholders:
-    model: ['NOAA-GFDL/GFDL-ESM4', 'IPSL/IPSL-CM6A-LR']
-#    model: ['CCCma/CanESM5', 'MRI/MRI-ESM2-0','EC-Earth-Consortium/EC-Earth3-Veg',
-#    'EC-Earth-Consortium/EC-Earth3-Veg-LR'] # other models but were regridded to irregular grid for lat
-    member: ['r1i1p1f1']
-    timestep: ['day','Amon']
+    model: [NOAA-GFDL/GFDL-ESM4, IPSL/IPSL-CM6A-LR]
+    #    model: ['CCCma/CanESM5', 'MRI/MRI-ESM2-0','EC-Earth-Consortium/EC-Earth3-Veg',
+    #    'EC-Earth-Consortium/EC-Earth3-Veg-LR'] # other models but were regridded to irregular grid for lat
+    member: [r1i1p1f1]
+    timestep: [day, Amon]
   path: gs://cmip6/CMIP6/ScenarioMIP/{model}/ssp119/{member}/{timestep}/{variable}/*/*
   rename:
     pr: precip
     tas: temp
     rsds: kin
     psl: press_msl
   unit_add:
@@ -80,34 +79,34 @@
 
 cmip6_{model}_ssp126_{member}_{timestep}:
   crs: 4326
   data_type: RasterDataset
   driver: zarr
   filesystem: gcs
   kwargs:
-    drop_variables: ['time_bnds', 'lat_bnds', 'lon_bnds', 'bnds']
+    drop_variables: [time_bnds, lat_bnds, lon_bnds, bnds]
     decode_times: true
     preprocess: harmonise_dims
     consolidated: true
   meta:
     category: climate
     paper_doi: 10.1175/BAMS-D-11-00094.1
     paper_ref: Taylor et al. 2012
     source_license: CC BY 4.0
     source_url: https://console.cloud.google.com/marketplace/details/noaa-public/cmip6?_ga=2.136097265.-1784288694.1541379221&pli=1
     source_version: 1.3.1
   placeholders:
-    model: ['NOAA-GFDL/GFDL-ESM4','INM/INM-CM4-8','INM/INM-CM5-0','IPSL/IPSL-CM6A-LR','NIMS-KMA/KACE-1-0-G',
-    'NCC/NorESM2-MM','CMCC/CMCC-CM2-SR5','IPSL/IPSL-CM5A2-INCA','CMCC/CMCC-ESM2']
-#    model: ['BCC/BCC-CSM2-MR','CCCma/CanESM5','AWI/AWI-CM-1-1-MR','DKRZ/MPI-ESM1-2-HR','MPI-M/MPI-ESM1-2-LR',
-#    'NUIST/NESM3', 'MIROC/MIROC6','MRI/MRI-ESM2-0','KIOST/KIOST-ESM','EC-Earth-Consortium/EC-Earth3-Veg',
-#    'EC-Earth-Consortium/EC-Earth3','CCCR-IITM/IITM-ESM','EC-Earth-Consortium/EC-Earth3-Veg-LR',
-#    'NCAR/CESM2-WACCM','CSIRO-ARCCSS/ACCESS-CM2'] # other models but were regridded to irregular grid for lat or time outofbounds
-    member: ['r1i1p1f1']
-    timestep: ['day','Amon']
+    model: [NOAA-GFDL/GFDL-ESM4, INM/INM-CM4-8, INM/INM-CM5-0, IPSL/IPSL-CM6A-LR, NIMS-KMA/KACE-1-0-G, NCC/NorESM2-MM, CMCC/CMCC-CM2-SR5, IPSL/IPSL-CM5A2-INCA,
+      CMCC/CMCC-ESM2]
+    #    model: ['BCC/BCC-CSM2-MR','CCCma/CanESM5','AWI/AWI-CM-1-1-MR','DKRZ/MPI-ESM1-2-HR','MPI-M/MPI-ESM1-2-LR',
+    #    'NUIST/NESM3', 'MIROC/MIROC6','MRI/MRI-ESM2-0','KIOST/KIOST-ESM','EC-Earth-Consortium/EC-Earth3-Veg',
+    #    'EC-Earth-Consortium/EC-Earth3','CCCR-IITM/IITM-ESM','EC-Earth-Consortium/EC-Earth3-Veg-LR',
+    #    'NCAR/CESM2-WACCM','CSIRO-ARCCSS/ACCESS-CM2'] # other models but were regridded to irregular grid for lat or time outofbounds
+    member: [r1i1p1f1]
+    timestep: [day, Amon]
   path: gs://cmip6/CMIP6/ScenarioMIP/{model}/ssp126/{member}/{timestep}/{variable}/*/*
   rename:
     pr: precip
     tas: temp
     rsds: kin
     psl: press_msl
   unit_add:
@@ -118,35 +117,34 @@
 
 cmip6_{model}_ssp245_{member}_{timestep}:
   crs: 4326
   data_type: RasterDataset
   driver: zarr
   filesystem: gcs
   kwargs:
-    drop_variables: ['time_bnds', 'lat_bnds', 'lon_bnds', 'bnds']
+    drop_variables: [time_bnds, lat_bnds, lon_bnds, bnds]
     decode_times: true
     preprocess: harmonise_dims
     consolidated: true
   meta:
     category: climate
     paper_doi: 10.1175/BAMS-D-11-00094.1
     paper_ref: Taylor et al. 2012
     source_license: CC BY 4.0
     source_url: https://console.cloud.google.com/marketplace/details/noaa-public/cmip6?_ga=2.136097265.-1784288694.1541379221&pli=1
     source_version: 1.3.1
   placeholders:
-    model: ['NOAA-GFDL/GFDL-ESM4','IPSL/IPSL-CM6A-LR','INM/INM-CM4-8','INM/INM-CM5-0','NCAR/CESM2-WACCM',
-    'NCC/NorESM2-LM','CSIRO-ARCCSS/ACCESS-CM2','NCC/NorESM2-MM','NIMS-KMA/KACE-1-0-G','CMCC/CMCC-CM2-SR5',
-    'CMCC/CMCC-ESM2','AS-RCEC/TaiESM1']
-#    model: ['NOAA-GFDL/GFDL-CM4','BCC/BCC-CSM2-MR','CCCma/CanESM5','EC-Earth-Consortium/EC-Earth3-Veg',
-#    'EC-Earth-Consortium/EC-Earth3','EC-Earth-Consortium/EC-Earth3-Veg-LR','EC-Earth-Consortium/EC-Earth3-CC',
-#    'AWI/AWI-CM-1-1-MR','MRI/MRI-ESM2-0','MPI-M/MPI-ESM1-2-LR','DKRZ/MPI-ESM1-2-HR','NUIST/NESM3',
-#    'CAS/FGOALS-g3','MIROC/MIROC6','KIOST/KIOST-ESM','CCCR-IITM/IITM-ESM'] # other models but were regridded to irregular grid for lat
-    member: ['r1i1p1f1']
-    timestep: ['day','Amon']
+    model: [NOAA-GFDL/GFDL-ESM4, IPSL/IPSL-CM6A-LR, INM/INM-CM4-8, INM/INM-CM5-0, NCAR/CESM2-WACCM, NCC/NorESM2-LM, CSIRO-ARCCSS/ACCESS-CM2, NCC/NorESM2-MM,
+      NIMS-KMA/KACE-1-0-G, CMCC/CMCC-CM2-SR5, CMCC/CMCC-ESM2, AS-RCEC/TaiESM1]
+    #    model: ['NOAA-GFDL/GFDL-CM4','BCC/BCC-CSM2-MR','CCCma/CanESM5','EC-Earth-Consortium/EC-Earth3-Veg',
+    #    'EC-Earth-Consortium/EC-Earth3','EC-Earth-Consortium/EC-Earth3-Veg-LR','EC-Earth-Consortium/EC-Earth3-CC',
+    #    'AWI/AWI-CM-1-1-MR','MRI/MRI-ESM2-0','MPI-M/MPI-ESM1-2-LR','DKRZ/MPI-ESM1-2-HR','NUIST/NESM3',
+    #    'CAS/FGOALS-g3','MIROC/MIROC6','KIOST/KIOST-ESM','CCCR-IITM/IITM-ESM'] # other models but were regridded to irregular grid for lat
+    member: [r1i1p1f1]
+    timestep: [day, Amon]
   path: gs://cmip6/CMIP6/ScenarioMIP/{model}/ssp245/{member}/{timestep}/{variable}/*/*
   rename:
     pr: precip
     tas: temp
     rsds: kin
     psl: press_msl
   unit_add:
@@ -157,35 +155,34 @@
 
 cmip6_{model}_ssp370_{member}_{timestep}:
   crs: 4326
   data_type: RasterDataset
   driver: zarr
   filesystem: gcs
   kwargs:
-    drop_variables: ['time_bnds', 'lat_bnds', 'lon_bnds', 'bnds']
+    drop_variables: [time_bnds, lat_bnds, lon_bnds, bnds]
     decode_times: true
     preprocess: harmonise_dims
     consolidated: true
   meta:
     category: climate
     paper_doi: 10.1175/BAMS-D-11-00094.1
     paper_ref: Taylor et al. 2012
     source_license: CC BY 4.0
     source_url: https://console.cloud.google.com/marketplace/details/noaa-public/cmip6?_ga=2.136097265.-1784288694.1541379221&pli=1
     source_version: 1.3.1
   placeholders:
-    model: ['NOAA-GFDL/GFDL-ESM4','IPSL/IPSL-CM6A-LR','INM/INM-CM4-8','INM/INM-CM5-0','NCAR/CESM2-WACCM',
-    'CSIRO-ARCCSS/ACCESS-CM2','NCC/NorESM2-MM','NCC/NorESM2-LM','NIMS-KMA/KACE-1-0-G','CMCC/CMCC-CM2-SR5',
-    'IPSL/IPSL-CM5A2-INCA','CMCC/CMCC-ESM2']
-#    model: ['BCC/BCC-CSM2-MR','CCCma/CanESM5','AWI/AWI-CM-1-1-MR','BCC/BCC-ESM1','DKRZ/MPI-ESM1-2-HR',
-#    EC-Earth-Consortium/EC-Earth3-Veg','EC-Earth-Consortium/EC-Earth3','EC-Earth-Consortium/EC-Earth3-AerChem',
-#    'EC-Earth-Consortium/EC-Earth3-Veg-LR','MRI/MRI-ESM2-0','MPI-M/MPI-ESM1-2-LR','HAMMOZ-Consortium/MPI-ESM-1-2-HAM',
-#    'CAS/FGOALS-g3','MIROC/MIROC6','CCCR-IITM/IITM-ESM'] # other models but were regridded to irregular grid for lat
-    member: ['r1i1p1f1']
-    timestep: ['day','Amon']
+    model: [NOAA-GFDL/GFDL-ESM4, IPSL/IPSL-CM6A-LR, INM/INM-CM4-8, INM/INM-CM5-0, NCAR/CESM2-WACCM, CSIRO-ARCCSS/ACCESS-CM2, NCC/NorESM2-MM, NCC/NorESM2-LM,
+      NIMS-KMA/KACE-1-0-G, CMCC/CMCC-CM2-SR5, IPSL/IPSL-CM5A2-INCA, CMCC/CMCC-ESM2]
+    #    model: ['BCC/BCC-CSM2-MR','CCCma/CanESM5','AWI/AWI-CM-1-1-MR','BCC/BCC-ESM1','DKRZ/MPI-ESM1-2-HR',
+    #    EC-Earth-Consortium/EC-Earth3-Veg','EC-Earth-Consortium/EC-Earth3','EC-Earth-Consortium/EC-Earth3-AerChem',
+    #    'EC-Earth-Consortium/EC-Earth3-Veg-LR','MRI/MRI-ESM2-0','MPI-M/MPI-ESM1-2-LR','HAMMOZ-Consortium/MPI-ESM-1-2-HAM',
+    #    'CAS/FGOALS-g3','MIROC/MIROC6','CCCR-IITM/IITM-ESM'] # other models but were regridded to irregular grid for lat
+    member: [r1i1p1f1]
+    timestep: [day, Amon]
   path: gs://cmip6/CMIP6/ScenarioMIP/{model}/ssp370/{member}/{timestep}/{variable}/*/*
   rename:
     pr: precip
     tas: temp
     rsds: kin
     psl: press_msl
   unit_add:
@@ -196,30 +193,30 @@
 
 cmip6_{model}_ssp434_{member}_{timestep}:
   crs: 4326
   data_type: RasterDataset
   driver: zarr
   filesystem: gcs
   kwargs:
-    drop_variables: ['time_bnds', 'lat_bnds', 'lon_bnds', 'bnds']
+    drop_variables: [time_bnds, lat_bnds, lon_bnds, bnds]
     decode_times: true
     preprocess: harmonise_dims
     consolidated: true
   meta:
     category: climate
     paper_doi: 10.1175/BAMS-D-11-00094.1
     paper_ref: Taylor et al. 2012
     source_license: CC BY 4.0
     source_url: https://console.cloud.google.com/marketplace/details/noaa-public/cmip6?_ga=2.136097265.-1784288694.1541379221&pli=1
     source_version: 1.3.1
   placeholders:
-    model: ['IPSL/IPSL-CM6A-LR']
-#    model: ['CCCma/CanESM5'] # other models but were regridded to irregular grid for lat
-    member: ['r1i1p1f1']
-    timestep: ['day','Amon']
+    model: [IPSL/IPSL-CM6A-LR]
+    #    model: ['CCCma/CanESM5'] # other models but were regridded to irregular grid for lat
+    member: [r1i1p1f1]
+    timestep: [day, Amon]
   path: gs://cmip6/CMIP6/ScenarioMIP/{model}/ssp434/{member}/{timestep}/{variable}/*/*
   rename:
     pr: precip
     tas: temp
     rsds: kin
     psl: press_msl
   unit_add:
@@ -230,30 +227,30 @@
 
 cmip6_{model}_ssp460_{member}_{timestep}:
   crs: 4326
   data_type: RasterDataset
   driver: zarr
   filesystem: gcs
   kwargs:
-    drop_variables: ['time_bnds', 'lat_bnds', 'lon_bnds', 'bnds']
+    drop_variables: [time_bnds, lat_bnds, lon_bnds, bnds]
     decode_times: true
     preprocess: harmonise_dims
     consolidated: true
   meta:
     category: climate
     paper_doi: 10.1175/BAMS-D-11-00094.1
     paper_ref: Taylor et al. 2012
     source_license: CC BY 4.0
     source_url: https://console.cloud.google.com/marketplace/details/noaa-public/cmip6?_ga=2.136097265.-1784288694.1541379221&pli=1
     source_version: 1.3.1
   placeholders:
-    model: ['IPSL/IPSL-CM6A-LR']
-#    model: ['CCCma/CanESM5'] # other models but were regridded to irregular grid for lat
-    member: ['r1i1p1f1']
-    timestep: ['day','Amon']
+    model: [IPSL/IPSL-CM6A-LR]
+    #    model: ['CCCma/CanESM5'] # other models but were regridded to irregular grid for lat
+    member: [r1i1p1f1]
+    timestep: [day, Amon]
   path: gs://cmip6/CMIP6/ScenarioMIP/{model}/ssp460/{member}/{timestep}/{variable}/*/*
   rename:
     pr: precip
     tas: temp
     rsds: kin
     psl: press_msl
   unit_add:
@@ -264,39 +261,39 @@
 
 cmip6_{model}_ssp585_{member}_{timestep}:
   crs: 4326
   data_type: RasterDataset
   driver: zarr
   filesystem: gcs
   kwargs:
-    drop_variables: ['time_bnds', 'lat_bnds', 'lon_bnds', 'bnds']
+    drop_variables: [time_bnds, lat_bnds, lon_bnds, bnds]
     decode_times: true
     preprocess: harmonise_dims
     consolidated: true
   meta:
     category: climate
     paper_doi: 10.1175/BAMS-D-11-00094.1
     paper_ref: Taylor et al. 2012
     source_license: CC BY 4.0
     source_url: https://console.cloud.google.com/marketplace/details/noaa-public/cmip6?_ga=2.136097265.-1784288694.1541379221&pli=1
     source_version: 1.3.1
   placeholders:
-    model: ['NOAA-GFDL/GFDL-ESM4','INM/INM-CM4-8','INM/INM-CM5-0','NIMS-KMA/KACE-1-0-G','NCC/NorESM2-MM','NCC/NorESM2-LM',
-    'CMCC/CMCC-CM2-SR5','AS-RCEC/TaiESM1','CMCC/CMCC-ESM2']
-#    model: ['NOAA-GFDL/GFDL-CM4','BCC/BCC-CSM2-MR','CCCma/CanESM5','AWI/AWI-CM-1-1-MR','MPI-M/MPI-ESM1-2-LR',
-#    'DKRZ/MPI-ESM1-2-HR','MIROC/MIROC6','MRI/MRI-ESM2-0','EC-Earth-Consortium/EC-Earth3-Veg',
-#    'EC-Earth-Consortium/EC-Earth3','EC-Earth-Consortium/EC-Earth3-Veg-LR','EC-Earth-Consortium/EC-Earth3-CC',
-#    'NUIST/NESM3','CAS/FGOALS-g3','IPSL/IPSL-CM6A-LR','KIOST/KIOST-ESM', 'NCAR/CESM2-WACCM','CCCR-IITM/IITM-ESM',
-#    'CSIRO-ARCCSS/ACCESS-CM2','CSIRO/ACCESS-ESM1-5'] # other models but were regridded to irregular grid for lat or time outofbounds
-    member: ['r1i1p1f1']
-    timestep: ['day','Amon']
+    model: [NOAA-GFDL/GFDL-ESM4, INM/INM-CM4-8, INM/INM-CM5-0, NIMS-KMA/KACE-1-0-G, NCC/NorESM2-MM, NCC/NorESM2-LM, CMCC/CMCC-CM2-SR5, AS-RCEC/TaiESM1,
+      CMCC/CMCC-ESM2]
+    #    model: ['NOAA-GFDL/GFDL-CM4','BCC/BCC-CSM2-MR','CCCma/CanESM5','AWI/AWI-CM-1-1-MR','MPI-M/MPI-ESM1-2-LR',
+    #    'DKRZ/MPI-ESM1-2-HR','MIROC/MIROC6','MRI/MRI-ESM2-0','EC-Earth-Consortium/EC-Earth3-Veg',
+    #    'EC-Earth-Consortium/EC-Earth3','EC-Earth-Consortium/EC-Earth3-Veg-LR','EC-Earth-Consortium/EC-Earth3-CC',
+    #    'NUIST/NESM3','CAS/FGOALS-g3','IPSL/IPSL-CM6A-LR','KIOST/KIOST-ESM', 'NCAR/CESM2-WACCM','CCCR-IITM/IITM-ESM',
+    #    'CSIRO-ARCCSS/ACCESS-CM2','CSIRO/ACCESS-ESM1-5'] # other models but were regridded to irregular grid for lat or time outofbounds
+    member: [r1i1p1f1]
+    timestep: [day, Amon]
   path: gs://cmip6/CMIP6/ScenarioMIP/{model}/ssp585/{member}/{timestep}/{variable}/*/*
   rename:
     pr: precip
     tas: temp
     rsds: kin
     psl: press_msl
   unit_add:
     temp: -273.15
   unit_mult:
     precip: 86400
-    press_msl: 0.01
+    press_msl: 0.01
```

### Comparing `hydromt-0.7.1/data/predefined_catalogs.yml` & `hydromt-0.8.0/data/predefined_catalogs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,33 @@
+---
 # list of predefined data catalogs
 #
 # <name>:
 #    urlpath: <path or url to yml file or data archive containing a data_catalog.yml file>
 #    versions:
 #       <calendar_version>: <git hash / tag>
-#    notes: <notes used in > 
-# if new versions of the data_catalogs are created, the current file predefined_catalogs.yml should be edited in main (not in the branch). 
+#    notes: <notes used in >
+# if new versions of the data_catalogs are created, the current file predefined_catalogs.yml should be edited in main (not in the branch).
 deltares_data:
-   urlpath: https://raw.githubusercontent.com/Deltares/hydromt/{version}/data/catalogs/deltares_data.yml
-   versions:
-     v2023.2: main
-     v2022.7: e082da339f22cb1fc3571eec5a901a21d1c8a7bd 
-     v2022.5: d88cc47bd4ecc83de38c00aa554a7d48ad23ec23
-   notes: This data is only accessible when connected to the Deltares network.
+  urlpath: https://raw.githubusercontent.com/Deltares/hydromt/{version}/data/catalogs/deltares_data.yml
+  versions:
+    v2023.2: main
+    v2022.7: e082da339f22cb1fc3571eec5a901a21d1c8a7bd
+    v2022.5: d88cc47bd4ecc83de38c00aa554a7d48ad23ec23
+  notes: This data is only accessible when connected to the Deltares network.
 gcs_cmip6_data:
-   urlpath: https://raw.githubusercontent.com/Deltares/hydromt/{version}/data/catalogs/gcs_cmip6_data.yml
-   versions:
-     v2023.2: main 
-   notes: This data uses CMIP6 data stored in Google Cloud Service.
+  urlpath: https://raw.githubusercontent.com/Deltares/hydromt/{version}/data/catalogs/gcs_cmip6_data.yml
+  versions:
+    v2023.2: main
+  notes: This data uses CMIP6 data stored in Google Cloud Service.
 aws_data:
-   urlpath: https://raw.githubusercontent.com/Deltares/hydromt/{version}/data/catalogs/aws_data.yml
-   versions:
-     v2023.2: main 
-   notes: This data are stored in public Amazon Web Services.
+  urlpath: https://raw.githubusercontent.com/Deltares/hydromt/{version}/data/catalogs/aws_data.yml
+  versions:
+    v2023.2: main
+  notes: This data are stored in public Amazon Web Services.
 artifact_data:
-   urlpath: https://github.com/DirkEilander/hydromt-artifacts/releases/download/{version}/data.tar.gz
-   versions:
-      v0.0.8: v0.0.8
-      v0.0.7: v0.0.7
-      v0.0.6: v0.0.6
-   notes: This data archive contains a sample dataset for the Piave basin (North Italy) to be used for tests and docs/demo purposes.
+  urlpath: https://github.com/DirkEilander/hydromt-artifacts/releases/download/{version}/data.tar.gz
+  versions:
+    v0.0.8: v0.0.8
+    v0.0.7: v0.0.7
+    v0.0.6: v0.0.6
+  notes: This data archive contains a sample dataset for the Piave basin (North Italy) to be used for tests and docs/demo purposes.
```

### Comparing `hydromt-0.7.1/data/src/era5_download_resample_convert.py` & `hydromt-0.8.0/data/src/era5_download_resample_convert.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# -*- coding: utf-8 -*-
-from os.path import join, isfile, basename
+"""Implementaions for downloading and resampling ERA5 data."""
+import glob
 import os
-import pdb
+import shutil
+import time
+from os.path import basename, isfile, join
+
 import dask
+import numpy as np
+import pandas as pd
 import xarray as xr
 from dask.diagnostics import ProgressBar
-import shutil
-import pandas as pd
-import numpy as np
-import glob
-import time
 
 # global vars
 dt_era5t = pd.to_timedelta(95, unit="d")
 era5_variables = {
     "ssrd": "surface_solar_radiation_downwards",
     "t2m": "2m_temperature",
     "tisr": "toa_incident_solar_radiation",
@@ -73,26 +73,31 @@
         "units": "-",
         "long_name": "Total cloud cover",
         "standard_name": "cloud_area_fraction",
     },
 }
 
 
-# donwload single year!
 def download_era5_year(
     fn_out: str, variable: str, year: int, months: list = None, days: list = None
 ) -> None:
-    """Download single ERA5 variable for single year from CDS.
+    """Download a ERA5 variable for a single year from Copernicus Climate Data Store.
 
-    Parameters
-    ----------
-    fn_out : str
-        output path
-    variable : str
-        CDS variable name
+    Arguments
+    ---------
+    fn_out: (str)
+        The output path to save the downloaded file.
+    variable: (str)
+        The CDS variable name to download.
+    year: (int)
+        The year to download the data for.
+    months: (list)
+        List of months to download data for. Use None to download data for all months.
+    days: (list)
+        List of days to download data for. Use None to downloads data for all days.
     """
     import cdsapi
 
     if not isfile(fn_out):
         # Set default months, days and hours options
         _months = [f"{m:02d}" for m in range(1, 13)]
         _days = [f"{d:02d}" for d in range(1, 32)]
@@ -101,15 +106,14 @@
         if months is None:
             months = _months
         if days is None:
             days = _days
 
         dataset = "reanalysis-era5-single-levels"
         if int(year) < 1979:
-            # raise ValueError("Years before 1979 not supported, please start download at 1979")
             dataset = f"{dataset}-complete-preliminary-back-extension"
 
         # Download ERA5 data
         c = cdsapi.Client()
         c.retrieve(
             dataset,
             {
@@ -168,41 +172,42 @@
     var: str,
     decimals: int = None,
     nodata=-9999,
     chunks: dict = {"time": 30, "latitude": 250, "longitude": 480},
     dask_kwargs: dict = {},
 ) -> None:
     """Resample hourly variables to daily timestep.
+
     The data is saved with the time labels at the end of the timestep.
     By default the data is aggregated using the mean.
 
     Exceptions:
     - the unit of tp is changed from m/hr to mm/day
     - from t2m, the mean, min and max daily values are saved
 
     Parameters
     ----------
     year : int
         year
     ddir : str
-        Root of hourly nc files with path format {ddir}/{var}/era5_{var}_{year}_hourly.nc
+        Root of hourly nc files with path format
+        {ddir}/{var}/era5_{var}_{year}_hourly.nc
     outdir : str
         Temporary output folder
     var : str
         input variable
     decimals : int, optional
         _description_, by default None
     nodata : int, optional
         _description_, by default -9999
     chunks : _type_, optional
         _description_, by default {'time':30, 'latitude':250, 'longitude':480}
     dask_kwargs : dict, optional
         _description_, by default {}
     """
-
     # nc out settings
     chunksizes = tuple([s for s in chunks.values()])
     e0 = {
         "zlib": True,
         "dtype": "float32",
         "_FillValue": nodata,
         "chunksizes": chunksizes,
@@ -246,15 +251,14 @@
         if var in dvars:
             continue
         dvars[var] = ds[var].resample(**kwargs).mean("time")
         dvars[var].attrs.update(daily_attrs.get(var, {}))
     ds_out = xr.merge(dvars.values()).chunk(chunks).fillna(nodata)
     if decimals:
         ds_out = ds_out.round(decimals=decimals)
-    # assert np.all(ds_out['time'].dt.year == year)
 
     # write
     fns = []
     for var in ds_out.data_vars.keys():
         print(f"{var}: {year} - {ds_out.time.size} days")
         fn_out = join(outdir, f"era5_{var:s}_{year:d}_daily.nc")
         fns.append(fn_out)
@@ -266,31 +270,48 @@
         with ProgressBar():
             obj.compute(**dask_kwargs)
 
     return fns
 
 
 def move_replace(src: str, dst: str, timeout: int = 300) -> None:
-    """try replacing old file which might be locked"""
+    """Try replacing old file which might be locked."""
     if not isfile(src):
         return
     if not os.path.isdir(os.path.dirname(dst)):
         os.makedirs(os.path.dirname(dst))
     while isfile(dst):
         try:
             os.unlink(dst)
-        except:
+        except PermissionError:
             print(f"FAILED deleting {dst} (retry in {timeout} sec)")
             time.sleep(timeout)
     os.rename(src, dst)
 
 
 def get_last_timestep_nc(fns: list) -> pd.Timedelta:
+    """Get the last timestep from a list of NetCDF files.
+
+    Parameters
+    ----------
+    fns : list
+        List of file paths or a glob pattern to match the files.
+
+    Returns
+    -------
+    pd.Timedelta
+        The time duration from the reference time to the last timestep.
+
+    Raises
+    ------
+    ValueError
+        If no files are found matching the provided file paths or glob pattern.
+    """
     if len(glob.glob(fns)) == 0:
-        raise ValueError(f"Files not found {fns}")
+        raise ValueError(f"Files not found: {fns}")
     with xr.open_mfdataset(fns, chunks="auto") as ds:
         t0 = pd.to_datetime(ds["time"][-1].values)
     return t0
 
 
 def append_zarr(
     store: str,
@@ -415,32 +436,36 @@
     variables: list,
     start_year: int = None,
     end_year: int = None,
     dt_era5t: pd.Timedelta = dt_era5t,
     move_to_ddir: bool = False,
     dask_kwargs: dict = {},
 ) -> None:
-    """Update the hourly by downloading the latest data from the CDS
+    """Update the hourly by downloading the latest data from the CDS.
 
     Parameters
     ----------
     outdir : str
         temporary output folder
     ddir : str
-        Root of hourly nc files with path format {ddir}/{var}/era5_{var}_{year}_hourly.nc
+        Root of hourly nc files with path format
+        {ddir}/{var}/era5_{var}_{year}_hourly.nc
     variables : list
         list of variable names to update
     start_year : int, optional
-        start year, by default None and read from last timestep of hourly nc files minus dt_era5t
+        start year, by default None and read from last timestep of hourly nc files
+        minus dt_era5t
     end_year : int, optional
         end year, by default None and based on todays' date
     dt_era5t : pd.Timedelta, optional
         time period of ERA5T data which is overwritten by new data, by default dt_era5t
     move_to_ddir : bool, optional
         Move files to root of hourly nc, by default False
+    dask_kwargs
+            Additional key-word arguments are passed to dask
     """
     t1 = pd.to_datetime("today").to_numpy()
     if end_year:
         t1 = pd.to_datetime(f"{end_year}0101")
     if start_year:
         t0 = pd.to_datetime(f"{start_year}0101")
 
@@ -486,34 +511,38 @@
     variables: list,
     start_year: int = None,
     end_year: int = None,
     dt_era5t: pd.Timedelta = dt_era5t,
     move_to_ddir: bool = False,
     dask_kwargs: dict = {},
 ) -> None:
-    """Update the daily nc files based on hourly files
+    """Update the daily nc files based on hourly files.
 
     Parameters
     ----------
     outdir : str
         temporary output folder
     ddir_hour : str
-        Root of hourly nc files with path format {ddir}/{var}/era5_{var}_{year}_hourly.nc
+        Root of hourly nc files with path format
+        {ddir}/{var}/era5_{var}_{year}_hourly.nc
     ddir_day : str
         Root of daily nc files with path format {ddir}/{var}/era5_{var}_{year}_daily.nc
     variables : list
         list of variable names to update
     start_year : int, optional
-        start year, by default None and read from last timestep of daily nc files minus dt_era5t
+        start year, by default None and read from last timestep of daily nc
+        files minus dt_era5t
     end_year : int, optional
         end year, by default None and read from last timestep of hourly nc files
     dt_era5t : pd.Timedelta, optional
         time period of ERA5T data which is overwritten by new data, by default dt_era5t
     move_to_ddir : bool, optional
         Move files to root of daily nc, by default False
+    dask_kwargs
+            Additional key-word arguments are passed to dask
     """
     if end_year:
         t1 = pd.to_datetime(f"{end_year}0101")
     if start_year:
         t0 = pd.to_datetime(f"{start_year}0101")
 
     fn_lst = []
@@ -563,21 +592,26 @@
     fn_zarr : str
         Zarr store path
     ddir : str
         Root of nc files with path format {ddir}/{var}/eray_{var}_*.nc
     variables : list
         list of variable names to update
     start_date : str, optional
-        start date in YYYYMMDD format, by default None and read from last timestep of zarr files minus dt_era5t
+        start date in YYYYMMDD format, by default None and read from last timestep of
+        zarr files minus dt_era5t
     end_date : str, optional
-        end date in YYYYMMDD format, by default None and read from last timestep of the nc files
+        end date in YYYYMMDD format, by default None and read from last timestep of
+        the nc files
+    chunks: tuple of int
+        size of the chunks to store to disk in.
+    **kwargs:
+        Key-word arguments passed to the zarr driver.
     dt_era5t : pd.Timedelta, optional
         time period of ERA5T data which is overwritten by new data, by default dt_era5t
     """
-
     print(f"writing to {fn_zarr}")
     for var in variables:
         # get start & end dates from files
         fns = join(ddir, var, f"era5_{var}_*.nc")
         if len(glob.glob(fns)) == 0:
             print(f'no nc files found for "{var}" - skipping')
         with xr.open_mfdataset(fns, chunks="auto", mode="r", autoclose=True) as ds_nc:
@@ -587,15 +621,16 @@
                 t1 = pd.to_datetime(end_date)
             if start_date:
                 t0 = pd.to_datetime(start_date)
             elif os.path.exists(fn_zarr):
                 with xr.open_zarr(fn_zarr, consolidated=False) as ds_zarr:
                     if var in ds_zarr:
                         # check last date with valid values at single location
-                        # TODO: this takes long, find alternative way with zarr library to find last date
+                        # TODO: this takes long, find alternative way with zarr library
+                        # to find last date
                         da_zarr = (
                             ds_zarr[var].isel(latitude=0, longitude=0).dropna("time")
                         )
                         t1_zr = pd.to_datetime(da_zarr["time"][-1].values)
                         if t1 > t1_zr:
                             t0 = t1_zr - dt_era5t
                         else:  # already up to date: skip var
@@ -660,22 +695,22 @@
         "u10",
         "v10",
         "d2m",
         "ssr",
         "tcc",
         "cape",
     ]
-    # NOTE: CAPE excluded from daily values, not sure how it is used and thus how to aggregate
+    # NOTE: CAPE excluded from daily values, not sure how it is used and
+    # thus how to aggregate
     variables_day = variables_hour[:-1] + ["tmin", "tmax"]
 
     # hydro / ocean
     # NOTE these are kept in different ddir
-    # variables_hour, ddir_hour = ["shww"], r"p:\wflow_global\hydromt\ocean\era5"
 
-    print(f"downloading ..")
+    print("downloading ..")
     update_hourly_nc(
         outdir,
         ddir=ddir_hour,
         variables=variables_hour,
         dask_kwargs=dask_kwargs,
         move_to_ddir=True,
     )
```

### Comparing `hydromt-0.7.1/hydromt/cli/api.py` & `hydromt-0.8.0/hydromt/cli/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
-"""This file describes an API for HydroMT, used by e.g. HydroMT-Dash to dynamically generate the inputs.
-"""
-from typing import List, Dict, Union
-import typing
+"""Defines the CLI-API."""
 import inspect
 import logging
+import typing
+from typing import Dict, List, Union
 
-from ..models import MODELS
-from ..data_catalog import DataCatalog
-from .. import workflows, log
 from hydromt.gis_utils import utm_crs
 
+from .. import workflows
+from ..data_catalog import DataCatalog
+from ..models import MODELS
+
 logger = logging.getLogger(__name__)
 
 
 def get_model_components(
     model: str, component_types=["read", "write", "setup"]
 ) -> Dict:
-    """Get all model components, each described with the following keys
+    """Get all model components, each described with the following keys.
 
         {
             <component_name> dict: {
                 "doc" str: doc string
                 "required" List: tuples of argument name and dtype,
                 "optional" List: tuples of argument name, dtype and default value,
                 "kwargs" bool: whether the component accepts key-word arguments,
@@ -44,19 +44,18 @@
         "RasterDatasetSource",
         "GeoDatasetSource",
         "GeoDataframeSource",
     ]
     model_class = MODELS.load(model)
     members = inspect.getmembers(model_class)
     components = {}
-    docs = []
     for name, member in members:
         if (
             name.startswith("_")
-            or not name.split("_")[0] in component_types
+            or name.split("_")[0] not in component_types
             or not callable(member)
         ):
             continue
         signature = inspect.signature(member)
         components[name] = {
             "doc": inspect.getdoc(member),
             "required": [],
@@ -80,28 +79,29 @@
                 # TODO convert default value to string ?
                 components[name]["optional"].append((k, type, v.default))
 
     return components
 
 
 def get_datasets(data_libs: Union[List, str]) -> Dict:
-    """Get all names of datasets sorted by data type
+    """Get all names of datasets sorted by data type.
 
         {
             "RasterDatasetSource": [],
             "GeoDatasetSource": [],
             "GeoDataframeSource": [],
         }
 
     Parameters
     ----------
     data_libs: (list of) str, Path, optional
-        One or more paths to data catalog yaml files or names of predefined data catalogs.
-        By default the data catalog is initiated without data entries.
-        See :py:func:`~hydromt.data_adapter.DataCatalog.from_yml` for accepted yaml format.
+        One or more paths to data catalog yaml files or names of predefined
+        data catalogs. By default the data catalog is initiated without data entries.
+        See :py:func:`~hydromt.data_adapter.DataCatalog.from_yml`
+        for accepted yaml format.
     """
     data_catalog = DataCatalog(data_libs)
     datasets = data_catalog.sources
     dataset_sources = {
         "RasterDatasetSource": [],
         "GeoDatasetSource": [],
         "GeoDataframeSource": [],
@@ -113,15 +113,15 @@
             dataset_sources["GeoDataframeSource"].append(k)
         elif v.data_type == "GeoDataset":
             dataset_sources["GeoDatasetSource"].append(k)
     return dataset_sources
 
 
 def get_predifined_catalogs() -> Dict:
-    """Get predefined catalogs
+    """Get predefined catalogs.
 
     {
         <catalog_name> Dict: {}
     }
 
     """
     return DataCatalog().predefined_catalogs
@@ -129,24 +129,25 @@
 
 def get_region(
     region: dict,
     data_libs: Union[List, str] = None,
     hydrography_fn: str = "merit_hydro",
     basin_index_fn: str = "merit_hydro_index",
 ) -> str:
-    """Get jsonified basin/subbasin/interbasin geometry that includes area as a property
+    """Get jsonified basin/subbasin/interbasin geometry including area as a property.
 
     Parameters
     ----------
     region : dict
         dictionary containing region definition
     data_libs : (list of) str, Path, optional
-        One or more paths to data catalog yaml files or names of predefined data catalogs.
-        By default the data catalog is initiated without data entries.
-        See :py:func:`~hydromt.data_adapter.DataCatalog.from_yml` for accepted yaml format.
+        One or more paths to data catalog yaml files or names of predefined
+        data catalogs. By default the data catalog is initiated without data entries.
+        See :py:func:`~hydromt.data_adapter.DataCatalog.from_yml`
+        for accepted yaml format.
     hydrography_fn : str
         Name of data source for hydrography data.
     basin_index_fn : str
         Name of data source with basin (bounding box) geometries associated with
             the 'basins' layer of `hydrography_fn`. Only required if the `region` is
             based on a (sub)(inter)basins without a 'bounds' argument.
 
@@ -170,15 +171,15 @@
         # get basin geometry
         geom, xy = workflows.get_basin_geometry(
             ds=ds_org,
             kind=kind,
             logger=logger,
             **region,
         )
-        # region.update(xy=xy)
+
         geom_bbox = geom.geometry.total_bounds
         projected_crs = utm_crs(geom_bbox)
         geom_projected = geom.to_crs(crs=projected_crs)
         geom["area"] = geom_projected["geometry"].area
 
         return geom.to_json()
     else:
```

### Comparing `hydromt-0.7.1/hydromt/cli/cli_utils.py` & `hydromt-0.8.0/hydromt/cli/cli_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 # -*- coding: utf-8 -*-
-"""Utils for parsing cli options and arguments 
-"""
+"""Utils for parsing cli options and arguments."""
 
-from os.path import isfile
 import json
 import logging
-import click
 from ast import literal_eval
-from typing import Union, Dict
+from os.path import isfile
 from pathlib import Path
+from typing import Any, Dict, Union
 from warnings import warn
 
+import click
+
 from .. import config
 from ..error import DeprecatedError
 
 logger = logging.getLogger(__name__)
 
 __all__ = ["parse_json", "parse_config", "parse_opt"]
 
 ### CLI callback methods ###
 
 
 def parse_opt(ctx, param, value):
-    """
-    click callback to validate `--opt KEY1=VAL1 --opt SECT.KEY2=VAL2` and collect
+    """Parse extra cli options.
+
+    Parse options like `--opt KEY1=VAL1 --opt SECT.KEY2=VAL2` and collect
     in a dictionary like the one below, which is what the CLI function receives.
     If no value or `None` is received then an empty dictionary is returned.
         {
             'KEY1': 'VAL1',
             'SECT': {
                 'KEY2': 'VAL2'
                 }
@@ -55,18 +56,24 @@
                     out[s] = dict()
                 out[s].update({k: v})
             else:
                 out.update({k: v})
     return out
 
 
-def parse_json(ctx, param, value):
+def parse_json(ctx, param, value: str) -> Dict[str, Any]:
+    """Parse json from object or file.
+
+    If the object passed is a path pointing to a file, load it's contents and parse it.
+    Otherwise attempt to parse the object as JSON itself.
+    """
     if isfile(value):
         with open(value, "r") as f:
             kwargs = json.load(f)
+
     # Catch old keyword for resulution "-r"
     elif type(literal_eval(value)) in (float, int):
         raise DeprecatedError("'-r' is used for region, resolution is deprecated")
     else:
         if value.strip("{").startswith("'"):
             value = value.replace("'", '"')
         try:
@@ -76,15 +83,15 @@
     return kwargs
 
 
 ### general parsing methods ##
 
 
 def parse_config(path: Union[Path, str] = None, opt_cli: Dict = None) -> Dict:
-    """Parse config from ini `path` and combine with command line options `opt_cli`"""
+    """Parse config from ini `path` and combine with command line options `opt_cli`."""
     opt = {}
     if path is not None and isfile(path):
         if str(path).endswith(".ini"):
             warn(
                 "Support for .ini configuration files will be deprecated",
                 PendingDeprecationWarning,
             )
@@ -93,15 +100,15 @@
         )
     elif path is not None:
         raise IOError(f"Config not found at {path}")
     if opt_cli is not None:
         for section in opt_cli:
             if not isinstance(opt_cli[section], dict):
                 raise ValueError(
-                    f"No section found in --opt values: "
+                    "No section found in --opt values: "
                     "use <section>.<option>=<value> notation."
                 )
             if section not in opt:
                 opt[section] = opt_cli[section]
                 continue
             for option, value in opt_cli[section].items():
                 opt[section].update({option: value})
```

### Comparing `hydromt-0.7.1/hydromt/cli/main.py` & `hydromt-0.8.0/hydromt/cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,45 @@
 # -*- coding: utf-8 -*-
-"""command line interface for hydromt models"""
+"""command line interface for hydromt models."""
 
-import click
-from os.path import join
 import logging
-import warnings
-import numpy as np
+from os.path import join
 
-### Uncomment the following lines for building exe
-# import sys
-# exepath = sys.prefix
-# import pyproj
-# pyproj_datadir = join(exepath, "proj-data")
-# pyproj.datadir.set_data_dir(pyproj_datadir)
-###
+import click
+import numpy as np
 
-from . import cli_utils
-from .. import log
+from .. import __version__, log
 from ..models import MODELS
-from .. import __version__
+from . import cli_utils
+
+BUILDING_EXE = False
+if BUILDING_EXE:
+    import sys
+
+    exepath = sys.prefix
+    import pyproj
+
+    pyproj_datadir = join(exepath, "proj-data")
+    pyproj.datadir.set_data_dir(pyproj_datadir)
 
 logger = logging.getLogger(__name__)
 
 
 def print_models(ctx, param, value):
+    """Print the available models and exit.
+
+    Parameters
+    ----------
+    ctx : click.Context
+        The Click context object.
+    param : click.Parameter
+        The Click parameter object.
+    value : bool
+        The value of the parameter.
+    """
     if not value:
         return {}
     click.echo(f"{MODELS}")
     ctx.exit()
 
 
 ## common arguments / options
@@ -113,17 +125,14 @@
 )
 @click.pass_context
 def main(ctx, models):  # , quiet, verbose):
     """Command line interface for hydromt models."""
     if ctx.obj is None:
         ctx.obj = {}
 
-    # ctx.obj["log_level"] = max(10, 30 - 10 * (verbose - quiet))
-    # logging.basicConfig(stream=sys.stderr, level=ctx.obj["log_level"])
-
 
 ## BUILD
 
 
 @main.command(short_help="Build models")
 @click.argument(
     "MODEL",
@@ -152,33 +161,31 @@
     fo,
     cache,
     verbose,
     quiet,
 ):
     """Build models from scratch.
 
-    \b
     Example usage:
     --------------
 
-    \b
-    To build a wflow model for a subbasin using and point coordinates snapped to cells with stream order >= 4
-    hydromt build wflow /path/to/model_root -i /path/to/wflow_config.ini -r "{'subbasin': [-7.24, 62.09], 'strord': 4}" -d deltares_data -d /path/to/data_catalog.yml -v
+    To build a wflow model for a subbasin using a point coordinates snapped to cells
+    with upstream area >= 50 km2
+    hydromt build wflow /path/to/model_root -i /path/to/wflow_config.ini  -r "{'subbasin': [-7.24, 62.09], 'uparea': 50}" -d deltares_data -d /path/to/data_catalog.yml -v
 
-    \b
     To build a sfincs model based on a bbox
-    hydromt build sfincs /path/to/model_root  -i /path/to/sfincs_config.ini -r "{'bbox': [4.6891,52.9750,4.9576,53.1994]}" -d /path/to/data_catalog.yml -v
+    hydromt build sfincs /path/to/model_root  -i /path/to/sfincs_config.ini  -r "{'bbox': [4.6891,52.9750,4.9576,53.1994]}"  -d /path/to/data_catalog.yml -v
 
-    """
+    """  # noqa: E501
     log_level = max(10, 30 - 10 * (verbose - quiet))
     logger = log.setuplog(
         "build", join(model_root, "hydromt.log"), log_level=log_level, append=False
     )
     logger.info(f"Building instance of {model} model at {model_root}.")
-    logger.info(f"User settings:")
+    logger.info("User settings:")
     opt = cli_utils.parse_config(config, opt_cli=opt)
     kwargs = opt.pop("global", {})
     # Set region to None if empty string json
     if len(region) == 0:
         region = None
     # parse data catalog options from global section in config and cli options
     data_libs = np.atleast_1d(kwargs.pop("data_libs", [])).tolist()  # from global
@@ -249,39 +256,38 @@
     data,
     dd,
     cache,
     verbose,
     quiet,
 ):
     """Update a specific component of a model.
+
     Set an output directory to copy the edited model to a new folder, otherwise maps
     are overwritten.
 
-    \b
     Example usage:
     --------------
 
-    \b
-    Update (overwrite!) landuse-landcover based maps in a Wflow model
+    Update (overwrite!) landuse-landcover based maps in a Wflow model:
     hydromt update wflow /path/to/model_root -c setup_lulcmaps --opt lulc_fn=vito -d /path/to/data_catalog.yml -v
 
-    \b
-    Update Wflow model components outlined in an .ini configuration file and write the model to a directory
-    hydromt update wflow /path/to/model_root -o /path/to/model_out -i /path/to/wflow_config.ini -d /path/to/data_catalog.yml -v
-    """
+    Update Wflow model components outlined in an .ini configuration file and
+    write the model to a directory:
+    hydromt update wflow /path/to/model_root  -o /path/to/model_out  -i /path/to/wflow_config.ini  -d /path/to/data_catalog.yml -v
+    """  # noqa: E501
     # logger
     mode = "r+" if model_root == model_out else "r"
     log_level = max(10, 30 - 10 * (verbose - quiet))
     logger = log.setuplog("update", join(model_out, "hydromt.log"), log_level=log_level)
     logger.info(f"Updating {model} model at {model_root} ({mode}).")
     logger.info(f"Output dir: {model_out}")
     # parse settings
     if len(components) == 1 and not isinstance(opt.get(components[0]), dict):
         opt = {components[0]: opt}
-    logger.info(f"User settings:")
+    logger.info("User settings:")
     opt = cli_utils.parse_config(config, opt_cli=opt)
     kwargs = opt.pop("global", {})
     # parse data catalog options from global section in config and cli options
     data_libs = np.atleast_1d(kwargs.pop("data_libs", [])).tolist()  # from global
     data_libs += list(data)  # add data catalogs from cli
     if dd and "deltares_data" not in data_libs:  # deltares_data from cli
         data_libs = ["deltares_data"] + data_libs  # prepend!
@@ -329,34 +335,32 @@
     callback=cli_utils.parse_json,
 )
 @quiet_opt
 @verbose_opt
 @click.pass_context
 def clip(ctx, model, model_root, model_destination, region, quiet, verbose):
     """Create a new model based on clipped region of an existing model.
+
     If the existing model contains forcing, they will also be clipped to the new model.
 
     For options to build wflow models see:
 
-    \b
     Example usage to clip a wflow model for a subbasin derived from point coordinates
-    snapped to cells with stream order >= 4
-    hydromt clip wflow /path/to/model_root /path/to/model_destination "{'subbasin': [-7.24, 62.09], 'wflow_streamorder': 4}"
+    snapped to cells with upstream area >= 50 km2
+    hydromt clip wflow /path/to/model_root /path/to/model_destination "{'subbasin': [-7.24, 62.09], 'wflow_uparea': 50}"
 
-    \b
     Example usage basin based on ID from model_root basins map
     hydromt clip wflow /path/to/model_root /path/to/model_destination "{'basin': 1}"
 
-    \b
     Example usage basins whose outlets are inside a geometry
     hydromt clip wflow /path/to/model_root /path/to/model_destination "{'outlet': 'geometry.geojson'}"
 
     All available option in the clip_staticmaps function help.
 
-    """
+    """  # noqa: E501
     log_level = max(10, 30 - 10 * (verbose - quiet))
     logger = log.setuplog(
         "clip", join(model_destination, "hydromt-clip.log"), log_level=log_level
     )
     logger.info(f"Clipping instance of {model} model.")
     logger.info(f"Region: {region}")
```

### Comparing `hydromt-0.7.1/hydromt/config.py` & `hydromt-0.8.0/hydromt/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-"""config I/O functions"""
+"""config I/O functions."""
 
 import abc
-from ast import literal_eval
 import codecs
+from ast import literal_eval
 from configparser import ConfigParser
-from os.path import dirname, join, abspath, exists, splitext
+from os.path import abspath, dirname, exists, join, splitext
 from pathlib import Path
-from typing import Union, Dict, List
+from typing import Dict, List, Union
+
 import yaml
 
 __all__ = [
     "configread",
     "configwrite",
 ]
 
@@ -27,19 +28,23 @@
     Parameters
     ----------
     config_fn : Union[Path, str]
         Path to configuration file
     defaults : dict, optional
         Nested dictionary with default options, by default dict()
     abs_path : bool, optional
-        If True, parse string values to an absolute path if the a file or folder with that
-        name (string value) relative to the config file exist, by default False
+        If True, parse string values to an absolute path if the a file or folder
+        with that name (string value) relative to the config file exist,
+        by default False
     skip_abspath_sections: list, optional
         These sections are not evaluated for absolute paths if abs_path=True,
         by default ['update_config']
+    **kwargs
+        Additional keyword arguments that are passed to the read_ini`
+        function.
 
     Returns
     -------
     cfdict : dict
         Configuration dictionary.
     """
     # read
@@ -65,21 +70,26 @@
 
     Parameters
     ----------
     config_fn : Union[Path, str]
         Path to configuration file
     cfdict : dict
         Configuration dictionary. If the configuration contains headers,
-        the first level keys are the section headers, the second level option-value pairs.
+        the first level keys are the section headers, the second level
+        option-value pairs.
     encoding : str, optional
         File encoding, by default "utf-8"
     cf : ConfigParser, optional
         Alternative configuration parser, by default None
     noheader : bool, optional
-        Set true for a single-level configuration dictionary with no headers, by default False
+        Set true for a single-level configuration dictionary with no headers,
+        by default False
+    **kwargs
+        Additional keyword arguments that are passed to the `write_ini_config`
+        function.
     """
     root = Path(dirname(config_fn))
     _cfdict = parse_relpath(cfdict.copy(), root)
     if splitext(config_fn)[-1] in [".yaml", ".yml"]:
         with open(config_fn, "w") as f:
             yaml.dump(_cfdict, f, sort_keys=False)
     else:
@@ -149,15 +159,16 @@
     cfdict : dict
         Configuration dictionary.
     encoding : str, optional
         File encoding, by default "utf-8"
     cf : ConfigParser, optional
         Alternative configuration parser, by default None
     noheader : bool, optional
-        Set true for a single-level configuration dictionary with no headers, by default False
+        Set true for a single-level configuration dictionary with no headers,
+        by default False
     """
     if cf is None:
         cf = ConfigParser(allow_no_value=True, inline_comment_prefixes=[";", "#"])
     elif isinstance(cf, abc.ABCMeta):  # not yet instantiated
         cf = cf()
     cf.optionxform = str  # preserve capital letter
     if noheader:  # add dummy header
@@ -189,17 +200,15 @@
             cfdict[key] = _relpath(val, root)
     return cfdict
 
 
 def parse_abspath(
     cfdict: dict, root: Path, skip_abspath_sections: List = ["setup_config"]
 ) -> dict:
-    """Parse string value to absolute path if the a file or folder with that
-    name (string value) relative to the config file exist.
-    """
+    """Parse string value to absolute path from config file."""
 
     def _abspath(value, root):
         if exists(join(root, value)):
             value = Path(abspath(join(root, value)))
         return value
 
     # loop through n-level of dict
```

### Comparing `hydromt-0.7.1/hydromt/data_adapter/caching.py` & `hydromt-0.8.0/hydromt/data_adapter/caching.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,51 @@
-from affine import Affine
+"""Caching mechanisms used in HydroMT."""
+import logging
+import os
+import shutil
 from ast import literal_eval
-import geopandas as gpd
+from os.path import basename, dirname, isdir, isfile, join
 from pathlib import Path
-from pyproj import CRS
+from typing import Union
+from urllib.parse import urlparse
+
+import geopandas as gpd
 import numpy as np
-import os
-from os.path import isfile, dirname, isdir, join, basename
 import requests
-import shutil
-from urllib.parse import urlparse
-import logging
+from affine import Affine
+from pyproj import CRS
 
 logger = logging.getLogger(__name__)
 
 
 HYDROMT_DATADIR = join(Path.home(), ".hydromt_data")
 
 
-def _uri_validator(uri: str) -> bool:
-    """Check if uri is valid"""
+def _uri_validator(uri: Union[str, Path]) -> bool:
+    """Check if uri is valid."""
     try:
-        result = urlparse(uri)
+        result = urlparse(str(uri))
         return all([result.scheme, result.netloc])
-    except:
+    except ValueError | AttributeError:
         return False
 
 
-def _copyfile(src, dst):
+def _copyfile(src, dst, chunk_size=1024):
     """Copy src file to dst. This method supports both online and local files."""
     if not isdir(dirname(dst)):
         os.makedirs(dirname(dst))
     if _uri_validator(str(src)):
         with requests.get(src, stream=True) as r:
             if r.status_code != 200:
                 raise ConnectionError(
                     f"Data download failed with status code {r.status_code}"
                 )
             with open(dst, "wb") as f:
-                shutil.copyfileobj(r.raw, f)
+                for chunk in r.iter_content(chunk_size=chunk_size):
+                    f.write(chunk)
     else:
         shutil.copyfile(src, dst)
 
 
 def cache_vrt_tiles(
     vrt_fn: str,
     geom: gpd.GeoSeries = None,
@@ -56,14 +60,16 @@
     ----------
     vrt_fn: str, Path
         path to source vrt
     geom: geopandas.GeoSeries, optional
         geometry to intersect tiles with
     cache_dir: str, Path
         path of the root folder where
+    logger: Logger
+        Logger to write logs to
 
     Returns
     -------
     dst_vrt_fn: str
         path to cached vrt
     """
     import xmltodict as xd
@@ -75,15 +81,15 @@
         _copyfile(vrt_fn, dst_vrt_fn)
     # read vrt file
     # TODO check if this is the optimal xml parser
     with open(dst_vrt_fn, "r") as f:
         ds = xd.parse(f.read())["VRTDataset"]
 
     def intersects(source: dict, affine, bbox):
-        """Check whether source interesects with bbox"""
+        """Check whether source interesects with bbox."""
         names = ["@xOff", "@yOff", "@xSize", "@ySize"]
         x0, y0, dx, dy = [float(source["DstRect"][k]) for k in names]
         xs, ys = affine * (np.array([x0, x0 + dx]), np.array([y0, y0 + dy]))
         return (
             max(xs) < bbox[0]
             or max(ys) < bbox[1]
             or min(xs) > bbox[2]
```

### Comparing `hydromt-0.7.1/hydromt/data_adapter/data_adapter.py` & `hydromt-0.8.0/hydromt/data_adapter/data_adapter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-# -*- coding: utf-8 -*-
+"""DataAdapter class."""
 from __future__ import annotations
+
+import logging
 from abc import ABCMeta, abstractmethod
+from itertools import product
+from string import Formatter
+
+import geopandas as gpd
 import numpy as np
 import pandas as pd
 import xarray as xr
-import geopandas as gpd
 import yaml
-from upath import UPath
 from fsspec.implementations import local
-from string import Formatter
-from typing import Tuple
-from itertools import product
 from pyproj import CRS
-import logging
+from upath import UPath
 
 from .. import _compat, gis_utils
 
 logger = logging.getLogger(__name__)
 
 
 __all__ = [
@@ -50,20 +51,20 @@
 
 
 def remove_duplicates(ds):
     return ds.sel(time=~ds.get_index("time").duplicated())
 
 
 def harmonise_dims(ds):
-    """
-    Function to harmonise lon-lat-time dimensions
+    """Harmonise lon-lat-time dimensions.
+
     Where needed:
         - lon: Convert longitude coordinates from 0-360 to -180-180
         - lat: Do N->S orientation instead of S->N
-        - time: Convert to datetimeindex
+        - time: Convert to datetimeindex.
 
     Parameters
     ----------
     ds: xr.DataSet
         DataSet with dims to harmonise
 
     Returns
@@ -79,16 +80,19 @@
         ds = ds.sortby(x_dim)
     # Latitude
     y_dim = ds.raster.y_dim
     if np.diff(ds[y_dim].values)[0] > 0:
         ds = ds.reindex({y_dim: ds[y_dim][::-1]})
     # Final check for lat-lon
     assert (
-        np.diff(ds[y_dim].values)[0] < 0 and np.diff(ds[x_dim].values)[0] > 0
-    ), "orientation not N->S & W->E after get_data preprocess set_lon_lat_axis"
+        np.diff(ds[y_dim].values)[0] < 0
+    ), "orientation not N->S after get_data preprocess set_lon_lat_axis"
+    assert (
+        np.diff(ds[x_dim].values)[0] > 0
+    ), "orientation not W->E after get_data preprocess set_lon_lat_axis"
     # Time
     if ds.indexes["time"].dtype == "O":
         ds = to_datetimeindex(ds)
 
     return ds
 
 
@@ -97,100 +101,151 @@
     "to_datetimeindex": to_datetimeindex,
     "remove_duplicates": remove_duplicates,
     "harmonise_dims": harmonise_dims,
 }
 
 
 class DataAdapter(object, metaclass=ABCMeta):
-    """General Interface to data source for HydroMT"""
+
+    """General Interface to data source for HydroMT."""
 
     _DEFAULT_DRIVER = None  # placeholder
     _DRIVERS = {}
 
     def __init__(
         self,
         path,
-        driver,
-        name="",  # optional for now
-        catalog_name="",  # optional for now
+        driver=None,
         filesystem="local",
-        crs=None,
         nodata=None,
         rename={},
         unit_mult={},
         unit_add={},
         meta={},
-        zoom_levels={},
-        **kwargs,
+        attrs={},
+        driver_kwargs={},
+        name="",  # optional for now
+        catalog_name="",  # optional for now
     ):
+        """General Interface to data source for HydroMT.
+
+        Parameters
+        ----------
+        path: str, Path
+            Path to data source. If the dataset consists of multiple files, the path may
+            contain {variable}, {year}, {month} placeholders as well as path
+            search pattern using a '*' wildcard.
+        driver: {'vector', 'netcdf', 'zarr'}, optional
+            Driver to read files with,
+            for 'vector' :py:func:`~hydromt.io.open_geodataset`,
+            for 'netcdf' :py:func:`xarray.open_mfdataset`.
+            By default the driver is inferred from the file extension and falls back to
+            'vector' if unknown.
+        filesystem: {'local', 'gcs', 's3'}, optional
+            Filesystem where the data is stored (local, cloud, http etc.).
+            By default, local.
+        nodata: float, int, optional
+            Missing value number. Only used if the data has no native missing value.
+            Nodata values can be differentiated between variables using a dictionary.
+        rename: dict, optional
+            Mapping of native data source variable to output source variable name as
+            required by hydroMT.
+        unit_mult, unit_add: dict, optional
+            Scaling multiplication and addition to change to map from the native
+            data unit to the output data unit as required by hydroMT.
+        meta: dict, optional
+            Metadata information of dataset, prefably containing the following keys:
+            {'source_version', 'source_url', 'source_license',
+            'paper_ref', 'paper_doi', 'category'}
+        placeholders: dict, optional
+            Placeholders to expand yaml entry to multiple entries (name and path)
+            based on placeholder values
+        attrs: dict, optional
+            Additional attributes relating to data variables. For instance unit
+            or long name of the variable.
+        driver_kwargs, dict, optional
+            Additional key-word arguments passed to the driver.
+        name, catalog_name: str, optional
+            Name of the dataset and catalog, optional for now.
+
+        """
         self.name = name
         self.catalog_name = catalog_name
         # general arguments
         self.path = path
         # driver and driver keyword-arguments
         # check for non default driver based on extension
         if driver is None:
             driver = self._DRIVERS.get(
                 str(path).split(".")[-1].lower(), self._DEFAULT_DRIVER
             )
         self.driver = driver
         self.filesystem = filesystem
-        self.kwargs = kwargs
+        self.driver_kwargs = driver_kwargs
+
         # data adapter arguments
-        self.crs = crs
         self.nodata = nodata
         self.rename = rename
         self.unit_mult = unit_mult
         self.unit_add = unit_add
-        self.zoom_levels = zoom_levels
         # meta data
         self.meta = {k: v for k, v in meta.items() if v is not None}
+        # variable attributes
+        self.attrs = {k: v for k, v in attrs.items() if v is not None}
 
     @property
     def data_type(self):
+        """Return the datatype of the addapter."""
         return type(self).__name__.replace("Adapter", "")
 
     def summary(self):
-        """Returns a dictionary summary of the data adapter."""
+        """Return a dictionary summary of the data adapter."""
         return dict(
             path=self.path,
             data_type=self.data_type,
             driver=self.driver,
             **self.meta,
         )
 
     def to_dict(self):
-        """Returns a dictionary view of the data source. Can be used to initialize
-        the data adapter."""
+        """Return a dictionary view of the data source.
+
+        Can be used to initialize the data adapter.
+        """
         source = dict(data_type=self.data_type)
         for k, v in vars(self).items():
             if k in ["name", "catalog_name"]:
                 continue  # do not add these identifiers
             if v is not None and (not isinstance(v, dict) or len(v) > 0):
                 source.update({k: v})
         return source
 
     def __str__(self):
+        """Return string representation of self in yaml."""
         return yaml.dump(self.to_dict())
 
     def __repr__(self):
+        """Pretty print string representation of self."""
         return self.__str__()
 
     def _parse_zoom_level(
         self,
         zoom_level: int | tuple = None,
         geom: gpd.GeoSeries = None,
         bbox: list = None,
         logger=logger,
     ) -> int:
-        """Return nearest smaller zoom level based on zoom resolutions defined in data catalog"""
+        """Return nearest smaller zoom level.
+
+        Based on zoom resolutions defined in data catalog.
+        """
         # common pyproj crs axis units
         known_units = ["degree", "metre", "US survey foot"]
         if self.zoom_levels is None or len(self.zoom_levels) == 0:
-            logger.warning(f"No zoom levels available, default to zero")
+            logger.warning("No zoom levels available, default to zero")
             return 0
         zls = list(self.zoom_levels.keys())
         if zoom_level is None:  # return first zoomlevel (assume these are ordered)
             return next(iter(zls))
         # parse zoom_level argument
         if (
             isinstance(zoom_level, tuple)
@@ -199,15 +254,16 @@
             and len(zoom_level) == 2
         ):
             res, unit = zoom_level
             # covert 'meter' and foot to official pyproj units
             unit = {"meter": "metre", "foot": "US survey foot"}.get(unit, unit)
             if unit not in known_units:
                 raise TypeError(
-                    f"zoom_level unit {unit} not understood; should be one of {known_units}"
+                    f"zoom_level unit {unit} not understood;"
+                    f" should be one of {known_units}"
                 )
         elif not isinstance(zoom_level, int):
             raise TypeError(
                 f"zoom_level argument not understood: {zoom_level}; should be a float"
             )
         else:
             return zoom_level
@@ -243,27 +299,37 @@
         variables: list = None,
         zoom_level: int | tuple = None,
         geom: gpd.GeoSeries = None,
         bbox: list = None,
         logger=logger,
         **kwargs,
     ):
-        """Resolve {year}, {month} and {variable} keywords
-        in self.path based on 'time_tuple' and 'variables' arguments
+        """Resolve {year}, {month} and {variable} keywords in self.path.
+
+          Keywords are based on 'time_tuple' and 'variables'.
 
         Parameters
         ----------
         time_tuple : tuple of str, optional
-            Start and end data in string format understood by :py:func:`pandas.to_timedelta`, by default None
+            Start and end date in string format understood by
+            :py:func:`pandas.to_timedelta`, by default None
         variables : list of str, optional
             List of variable names, by default None
         zoom_level : int | tuple, optional
-            zoom level of dataset, can be provided as tuple of (<zoom resolution>, <unit>)
+            zoom level of dataset, can be provided as tuple of
+            (<zoom resolution>, <unit>)
         **kwargs
-            key-word arguments are passed to fsspec FileSystem objects. Arguments depend on protocal (local, gcs, s3...).
+            key-word arguments are passed to fsspec FileSystem objects. Arguments
+            depend on protocal (local, gcs, s3...).
+        geom:
+            A geoSeries describing the geometries.
+        bbox:
+            A list of bounding boxes.
+        logger:
+            The logger to use. If none is provided, the devault logger will be used.
 
         Returns
         -------
         List:
             list of filenames matching the path pattern given date range and variables
         """
         known_keys = ["year", "month", "zoom_level", "variable"]
@@ -319,44 +385,51 @@
                 fmt.update(year=date.year, month=date.month)
             if var is not None:
                 fmt.update(variable=var)
             fns.extend(fs.glob(path.format(**fmt)))
         if len(fns) == 0:
             raise FileNotFoundError(f"No such file found: {path}{postfix}")
 
-        # With some fs like gcfs or s3fs, the first part of the past is not returned properly with glob
+        # With some fs like gcfs or s3fs, the first part of the path is not returned
+        # properly with glob
         if not str(UPath(fns[0])).startswith(str(UPath(path))[0:2]):
-            # Assumes it's the first part of the path that is not correctly parsed with gcsfs, s3fs etc.
+            # Assumes it's the first part of the path that is not
+            # correctly parsed with gcsfs, s3fs etc.
             last_parent = UPath(path).parents[-1]
             # add the rest of the path
             fns = [last_parent.joinpath(*UPath(fn).parts[1:]) for fn in fns]
         return list(set(fns))  # return unique paths
 
     def get_filesystem(self, **kwargs):
-        """Return an initialised filesystem object based on self.filesystem and **kwargs"""
+        """Return an initialised filesystem object."""
         if self.filesystem == "local":
             fs = local.LocalFileSystem(**kwargs)
         elif self.filesystem == "gcs":
             if _compat.HAS_GCSFS:
                 fs = gcsfs.GCSFileSystem(**kwargs)
             else:
                 raise ModuleNotFoundError(
-                    "The gcsfs library is required to read data from gcs (Google Cloud Storage). Please install."
+                    "The gcsfs library is required to read data from gcs"
+                    + "(Google Cloud Storage). Please install."
                 )
         elif self.filesystem == "s3":
             if _compat.HAS_S3FS:
                 fs = s3fs.S3FileSystem(**kwargs)
             else:
                 raise ModuleNotFoundError(
-                    "The s3fs library is required to read data from s3 (Amazon Web Storage). Please install."
+                    "The s3fs library is required to read data from s3"
+                    + " (Amazon Web Storage). Please install."
                 )
         else:
             raise ValueError(
-                f"Unknown or unsupported filesystem {self.filesystem}. Use one of {FILESYSTEMS}"
+                f"Unknown or unsupported filesystem {self.filesystem}."
+                + f" Use one of {FILESYSTEMS}"
             )
 
         return fs
 
     @abstractmethod
     def get_data(self, bbox, geom, buffer):
         """Return a view (lazy if possible) of the data with standardized field names.
-        If bbox of mask are given, clip data to that extent"""
+
+        If bbox of mask are given, clip data to that extent.
+        """
```

### Comparing `hydromt-0.7.1/hydromt/data_adapter/dataframe.py` & `hydromt-0.8.0/hydromt/data_adapter/dataframe.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,168 +1,207 @@
-# -*- coding: utf-8 -*-
+"""Implementation for the Pandas Dataframe adapter."""
+import logging
 import os
+import warnings
 from os.path import join
+from typing import Union
+
 import numpy as np
 import pandas as pd
-from .data_adapter import DataAdapter
 
-import logging
+from .data_adapter import DataAdapter
 
 logger = logging.getLogger(__name__)
 
 __all__ = [
     "DataFrameAdapter",
 ]
 
 
 class DataFrameAdapter(DataAdapter):
+
+    """DataAdapter implementation for Pandas Dataframes."""
+
     _DEFAULT_DRIVER = "csv"
     _DRIVERS = {"xlsx": "excel", "xls": "excel"}
 
     def __init__(
         self,
-        path,
-        driver=None,
-        filesystem="local",
-        nodata=None,
-        rename={},
-        unit_mult={},
-        unit_add={},
-        meta={},
+        path: str,
+        driver: str = None,
+        filesystem: str = "local",
+        nodata: Union[dict, float, int] = None,
+        rename: dict = {},
+        unit_mult: dict = {},
+        unit_add: dict = {},
+        meta: dict = {},
+        attrs: dict = {},
+        driver_kwargs: dict = {},
+        name: str = "",  # optional for now
+        catalog_name: str = "",  # optional for now
         **kwargs,
     ):
-        """Initiates data adapter for 2D tabular data.
+        """Initiate data adapter for 2D tabular data.
 
         This object contains all properties required to read supported files into
         a :py:func:`pandas.DataFrame`.
         In addition it keeps meta data to be able to reproduce which data is used.
 
         Parameters
         ----------
         path: str, Path
-            Path to data source.
+            Path to data source. If the dataset consists of multiple files, the path may
+            contain {variable}, {year}, {month} placeholders as well as path
+            search pattern using a '*' wildcard.
         driver: {'csv', 'xlsx', 'xls', 'fwf'}, optional
             Driver to read files with, for 'csv' :py:func:`~pandas.read_csv`,
             for {'xlsx', 'xls'} :py:func:`~pandas.read_excel`, and for 'fwf'
             :py:func:`~pandas.read_fwf`.
             By default the driver is inferred from the file extension and falls back to
             'csv' if unknown.
         filesystem: {'local', 'gcs', 's3'}, optional
             Filesystem where the data is stored (local, cloud, http etc.).
             By default, local.
-        nodata: (dictionary) float, int, optional
+        nodata: dict, float, int, optional
             Missing value number. Only used if the data has no native missing value.
-            Multiple nodata values can be provided in a list and differentiated between
-            dataframe columns using a dictionary with variable (column) keys. The nodata
-            values are only applied to columns with numeric data.
+            Nodata values can be differentiated between variables using a dictionary.
         rename: dict, optional
-            Mapping of native column names to output column names as
+            Mapping of native data source variable to output source variable name as
             required by hydroMT.
         unit_mult, unit_add: dict, optional
-            Scaling multiplication and addition to change to map from the native data unit
-            to the output data unit as required by hydroMT.
+            Scaling multiplication and addition to change to map from the native
+            data unit to the output data unit as required by hydroMT.
         meta: dict, optional
-            Metadata information of dataframe, prefably containing the following keys:
-            {'source_version', 'source_url', 'source_license', 'paper_ref', 'paper_doi', 'category'}
-        **kwargs
+            Metadata information of dataset, prefably containing the following keys:
+            {'source_version', 'source_url', 'source_license',
+            'paper_ref', 'paper_doi', 'category'}
+        placeholders: dict, optional
+            Placeholders to expand yaml entry to multiple entries (name and path)
+            based on placeholder values
+        attrs: dict, optional
+            Additional attributes relating to data variables. For instance unit
+            or long name of the variable.
+        driver_kwargs, dict, optional
             Additional key-word arguments passed to the driver.
+        name, catalog_name: str, optional
+            Name of the dataset and catalog, optional for now.
         """
+        if kwargs:
+            warnings.warn(
+                "Passing additional keyword arguments to be used by the "
+                "DataFrameAdapter driver is deprecated and will be removed "
+                "in a future version. Please use 'driver_kwargs' instead.",
+                DeprecationWarning,
+            )
+            driver_kwargs.update(kwargs)
         super().__init__(
             path=path,
             driver=driver,
             filesystem=filesystem,
             nodata=nodata,
             rename=rename,
             unit_mult=unit_mult,
             unit_add=unit_add,
             meta=meta,
-            **kwargs,
+            attrs=attrs,
+            driver_kwargs=driver_kwargs,
+            name=name,
+            catalog_name=catalog_name,
         )
 
     def to_file(
         self,
         data_root,
         data_name,
         driver=None,
         variables=None,
         time_tuple=None,
         logger=logger,
         **kwargs,
     ):
-        """Save dataframe slice to file.
+        """Save a dataframe slice to a file.
 
         Parameters
         ----------
-        data_root : str, Path
-            Path to output folder
+        data_root : str or Path
+            Path to the output folder.
         data_name : str
-            Name of output file without extension.
+            Name of the output file without extension.
         driver : str, optional
-            Driver to write file, e.g.: 'csv', 'excel', by default None
+            Driver to write the file, e.g., 'csv', 'excel'. If None,
+            the default behavior is used.
         variables : list of str, optional
-            Names of DataFrame columns to return. By default all columns
-            are returned.
-        time_tuple : tuple of str, datetime, optional
-            Start and end date of period of interest. By default the entire time period
-            of the DataFrame is returned.
+            Names of DataFrame columns to include in the output. By default,
+            all columns are included.
+        time_tuple : tuple of str or datetime, optional
+            Start and end date of the period of interest. By default, the entire time
+            period of the DataFrame is included.
+        logger : Logger, optional
+            Logger object to log warnings or messages. By default, the module
+            logger is used.
+        **kwargs : dict
+            Additional keyword arguments to be passed to the file writing method.
 
         Returns
         -------
-        fn_out: str
-            Absolute path to output file
-        driver: str
-            Name of driver to read data with, see :py:func:`~hydromt.data_catalog.DataCatalog.get_geodataset`
+        fn_out : str
+            Absolute path to the output file.
+        driver : str
+            Name of the driver used to read the data.
+            See :py:func:`~hydromt.data_catalog.DataCatalog.get_geodataset`.
+
+
         """
         kwargs.pop("bbox", None)
         try:
             obj = self.get_data(
                 time_tuple=time_tuple, variables=variables, logger=logger
             )
         except IndexError as err:  # out of bounds for time
             logger.warning(str(err))
             return None, None
 
         if driver is None or driver == "csv":
-            # always write netcdf
+            # always write as CSV
             driver = "csv"
             fn_out = join(data_root, f"{data_name}.csv")
-
             obj.to_csv(fn_out, **kwargs)
         elif driver == "excel":
             fn_out = join(data_root, f"{data_name}.xlsx")
             obj.to_excel(fn_out, **kwargs)
         else:
-            raise ValueError(f"DataFrame: Driver {driver} unknown.")
+            raise ValueError(f"DataFrame: Driver {driver} is unknown.")
 
         return fn_out, driver
 
     def get_data(
         self,
         variables=None,
         time_tuple=None,
         logger=logger,
-        **kwargs,
     ):
-        """Returns a DataFrame, optionally sliced by time and variables, based on the properties of this DataFrameAdapter.
+        """Return a DataFrame.
 
-        For a detailed description see: :py:func:`~hydromt.data_catalog.DataCatalog.get_dataframe`
+        Returned data is optionally sliced by time and variables,
+        based on the properties of this DataFrameAdapter. For a detailed
+        description see: :py:func:`~hydromt.data_catalog.DataCatalog.get_dataframe`
         """
-
         # Extract storage_options from kwargs to instantiate fsspec object correctly
-        if "storage_options" in self.kwargs:
-            kwargs = self.kwargs["storage_options"]
-            # For s3, anonymous connection still requires --no-sign-request profile to read the data
-            # setting environment variable works
-            if "anon" in kwargs:
+        so_kwargs = {}
+        if "storage_options" in self.driver_kwargs:
+            so_kwargs = self.driver_kwargs["storage_options"]
+            # For s3, anonymous connection still requires --no-sign-request profile
+            # to read the data setting environment variable works
+            if "anon" in so_kwargs:
                 os.environ["AWS_NO_SIGN_REQUEST"] = "YES"
             else:
                 os.environ["AWS_NO_SIGN_REQUEST"] = "NO"
-        _ = self.resolve_paths(**kwargs)  # throw nice error if data not found
+        _ = self.resolve_paths(**so_kwargs)  # throw nice error if data not found
 
-        kwargs = self.kwargs.copy()
+        kwargs = self.driver_kwargs.copy()
 
         # read and clip
         logger.info(f"DataFrame: Read {self.driver} data.")
 
         if self.driver in ["csv"]:
             df = pd.read_csv(self.path, **kwargs)
         elif self.driver in ["xls", "xlsx", "excel"]:
@@ -209,13 +248,18 @@
                 df[name] = df[name] * m + a
 
         # clip time slice
         if time_tuple is not None and np.dtype(df.index).type == np.datetime64:
             logger.debug(f"DataFrame: Slicing time dime {time_tuple}")
             df = df[df.index.slice_indexer(*time_tuple)]
             if df.size == 0:
-                raise IndexError(f"DataFrame: Time slice out of range.")
+                raise IndexError("DataFrame: Time slice out of range.")
 
         # set meta data
         df.attrs.update(self.meta)
 
+        # set column attributes
+        for col in self.attrs:
+            if col in df.columns:
+                df[col].attrs.update(**self.attrs[col])
+
         return df
```

### Comparing `hydromt-0.7.1/hydromt/data_adapter/geodataframe.py` & `hydromt-0.8.0/hydromt/data_adapter/geodataframe.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,100 +1,127 @@
-# -*- coding: utf-8 -*-
+"""The Geodataframe adapter implementation."""
+import logging
+import warnings
 from os.path import join
-import numpy as np
+from pathlib import Path
+from typing import NewType, Union
+
 import geopandas as gpd
+import numpy as np
 from shapely.geometry import box
-import logging
-from typing import Union, NewType
-from pathlib import Path
 
-from .data_adapter import DataAdapter
 from .. import io
-
+from .data_adapter import DataAdapter
 
 logger = logging.getLogger(__name__)
 
 __all__ = ["GeoDataFrameAdapter", "GeoDataframeSource"]
 
 GeoDataframeSource = NewType("GeoDataframeSource", Union[str, Path])
 
 
 class GeoDataFrameAdapter(DataAdapter):
+
+    """The Geodataframe adapter implementation."""
+
     _DEFAULT_DRIVER = "vector"
     _DRIVERS = {
         "xy": "xy",
         "csv": "csv",
         "xls": "xls",
         "xlsx": "xlsx",
     }
 
     def __init__(
         self,
-        path,
-        driver=None,
-        filesystem="local",
-        crs=None,
-        nodata=None,
-        rename={},
-        unit_mult={},
-        unit_add={},
-        units={},
-        meta={},
+        path: str,
+        driver: str = None,
+        filesystem: str = "local",
+        crs: Union[int, str, dict] = None,
+        nodata: Union[dict, float, int] = None,
+        rename: dict = {},
+        unit_mult: dict = {},
+        unit_add: dict = {},
+        meta: dict = {},
+        attrs: dict = {},
+        driver_kwargs: dict = {},
+        name: str = "",  # optional for now
+        catalog_name: str = "",  # optional for now
         **kwargs,
     ):
-        """Initiates data adapter for geospatial vector data.
+        """Initiate data adapter for geospatial vector data.
 
         This object contains all properties required to read supported files into
         a single unified :py:func:`geopandas.GeoDataFrame`.
         In addition it keeps meta data to be able to reproduce which data is used.
 
         Parameters
         ----------
         path: str, Path
-            Path to data source.
+            Path to data source. If the dataset consists of multiple files, the path may
+            contain {variable} placeholders as well as path
+            search pattern using a '*' wildcard.
         driver: {'vector', 'vector_table'}, optional
             Driver to read files with, for 'vector' :py:func:`~geopandas.read_file`,
             for {'vector_table'} :py:func:`hydromt.io.open_vector_from_table`
             By default the driver is inferred from the file extension and falls back to
             'vector' if unknown.
         filesystem: {'local', 'gcs', 's3'}, optional
             Filesystem where the data is stored (local, cloud, http etc.).
             By default, local.
         crs: int, dict, or str, optional
-            Coordinate Reference System. Accepts EPSG codes (int or str); proj (str or dict)
-            or wkt (str). Only used if the data has no native CRS.
-        nodata: (dictionary) float, int, optional
+            Coordinate Reference System. Accepts EPSG codes (int or str);
+            proj (str or dict) or wkt (str). Only used if the data has no native CRS.
+        nodata: dictionary, float, int, optional
             Missing value number. Only used if the data has no native missing value.
-            Multiple nodata values can be provided in a list and differentiated between
-            dataframe columns using a dictionary with variable (column) keys. The nodata
-            values are only applied to columns with numeric data.
+            Nodata values can be differentiated between variables using a dictionary.
         rename: dict, optional
             Mapping of native data source variable to output source variable name as
             required by hydroMT.
         unit_mult, unit_add: dict, optional
-            Scaling multiplication and addition to change to map from the native data unit
-            to the output data unit as required by hydroMT.
+            Scaling multiplication and addition to change to map from the native
+            data unit to the output data unit as required by hydroMT.
         meta: dict, optional
             Metadata information of dataset, prefably containing the following keys:
-            {'source_version', 'source_url', 'source_license', 'paper_ref', 'paper_doi', 'category'}
-        **kwargs
+            {'source_version', 'source_url', 'source_license',
+            'paper_ref', 'paper_doi', 'category'}
+        placeholders: dict, optional
+            Placeholders to expand yaml entry to multiple entries (name and path)
+            based on placeholder values
+        attrs: dict, optional
+            Additional attributes relating to data variables. For instance unit
+            or long name of the variable.
+        driver_kwargs, dict, optional
             Additional key-word arguments passed to the driver.
+        name, catalog_name: str, optional
+            Name of the dataset and catalog, optional for now.
         """
+        if kwargs:
+            warnings.warn(
+                "Passing additional keyword arguments to be used by the "
+                "GeoDataFrameAdapter driver is deprecated and will be removed "
+                "in a future version. Please use 'driver_kwargs' instead.",
+                DeprecationWarning,
+            )
+            driver_kwargs.update(kwargs)
         super().__init__(
             path=path,
             driver=driver,
             filesystem=filesystem,
-            crs=crs,
             nodata=nodata,
             rename=rename,
             unit_mult=unit_mult,
             unit_add=unit_add,
             meta=meta,
-            **kwargs,
+            attrs=attrs,
+            driver_kwargs=driver_kwargs,
+            name=name,
+            catalog_name=catalog_name,
         )
+        self.crs = crs
 
     def to_file(
         self,
         data_root,
         data_name,
         bbox=None,
         driver=None,
@@ -109,25 +136,32 @@
         data_root : str, Path
             Path to output folder
         data_name : str
             Name of output file without extension.
         bbox : array-like of floats
             (xmin, ymin, xmax, ymax) bounding box of area of interest.
         driver : str, optional
-            Driver to write file, e.g.: 'GPKG', 'ESRI Shapefile' or any fiona data type, by default None
+            Driver to write file, e.g.: 'GPKG', 'ESRI Shapefile' or any fiona data type,
+            by default None
         variables : list of str, optional
             Names of GeoDataset variables to return. By default all dataset variables
             are returned.
+        logger : logger object, optional
+            The logger object used for logging messages. If not provided, the default
+            logger will be used.
+        **kwargs
+            Additional keyword arguments that are passed to the geopandas driver.
 
         Returns
         -------
         fn_out: str
             Absolute path to output file
         driver: str
-            Name of driver to read data with, see :py:func:`~hydromt.data_catalog.DataCatalog.get_geodataframe`
+            Name of driver to read data with, see
+            :py:func:`~hydromt.data_catalog.DataCatalog.get_geodataframe`
         """
         kwargs.pop("time_tuple", None)
         gdf = self.get_data(bbox=bbox, variables=variables, logger=logger)
         if gdf.index.size == 0:
             return None, None
 
         if driver is None:
@@ -158,34 +192,34 @@
         self,
         bbox=None,
         geom=None,
         predicate="intersects",
         buffer=0,
         logger=logger,
         variables=None,
-        **kwargs,  # this is not used, for testing only
+        # **kwargs,  # this is not used, for testing only
     ):
-        """Returns a clipped and unified GeoDataFrame (vector) based on the properties
-        of this GeoDataFrameAdapter.
+        """Return a clipped and unified GeoDataFrame (vector).
 
-        For a detailed description see: :py:func:`~hydromt.data_catalog.DataCatalog.get_geodataframe`
+        For a detailed description see:
+        :py:func:`~hydromt.data_catalog.DataCatalog.get_geodataframe`
         """
         # If variable is string, convert to list
         if variables:
             variables = np.atleast_1d(variables).tolist()
 
-        kwargs = self.kwargs.copy()
-        if "storage_options" in kwargs:
+        if "storage_options" in self.driver_kwargs:
             # not sure if storage options can be passed to fiona.open()
             # for now throw NotImplemented Error
             raise NotImplementedError(
                 "Remote file storage_options not implemented for GeoDataFrame"
             )
         _ = self.resolve_paths()  # throw nice error if data not found
 
+        kwargs = self.driver_kwargs.copy()
         # parse geom, bbox and buffer arguments
         clip_str = ""
         if geom is None and bbox is not None:
             # convert bbox to geom with crs EPGS:4326 to apply buffer later
             geom = gpd.GeoDataFrame(geometry=[box(*bbox)], crs=4326)
             clip_str = " and clip to bbox (epsg:4326)"
         elif geom is not None:
@@ -252,8 +286,13 @@
             for name in list(set(unit_names)):  # unique
                 m = self.unit_mult.get(name, 1)
                 a = self.unit_add.get(name, 0)
                 gdf[name] = gdf[name] * m + a
 
         # set meta data
         gdf.attrs.update(self.meta)
+
+        # set column attributes
+        for col in self.attrs:
+            if col in gdf.columns:
+                gdf[col].attrs.update(**self.attrs[col])
         return gdf
```

### Comparing `hydromt-0.7.1/hydromt/data_adapter/geodataset.py` & `hydromt-0.8.0/hydromt/data_adapter/geodataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,102 +1,134 @@
-# -*- coding: utf-8 -*-
+"""Implementation for the geodataset DataAdapter."""
+import logging
 import os
+import warnings
 from os.path import join
+from pathlib import Path
+from typing import NewType, Union
+
+import geopandas as gpd
 import numpy as np
 import pandas as pd
 import xarray as xr
-import geopandas as gpd
 from shapely.geometry import box
-import logging
-from typing import Union, NewType
-from pathlib import Path
 
 from .. import gis_utils, io
-from .data_adapter import DataAdapter
 from ..raster import GEO_MAP_COORD
-
+from .data_adapter import DataAdapter
 
 logger = logging.getLogger(__name__)
 
 __all__ = ["GeoDatasetAdapter", "GeoDatasetSource"]
 
 GeoDatasetSource = NewType("GeoDatasetSource", Union[str, Path])
 
 
 class GeoDatasetAdapter(DataAdapter):
+
+    """DatasetAdapter for GeoDatasets."""
+
     _DEFAULT_DRIVER = "vector"
     _DRIVERS = {
         "nc": "netcdf",
     }
 
     def __init__(
         self,
-        path,
-        driver=None,
-        filesystem="local",
-        crs=None,
-        nodata=None,
-        rename={},
-        unit_mult={},
-        unit_add={},
-        meta={},
+        path: str,
+        driver: str = None,
+        filesystem: str = "local",
+        crs: Union[int, str, dict] = None,
+        nodata: Union[dict, float, int] = None,
+        rename: dict = {},
+        unit_mult: dict = {},
+        unit_add: dict = {},
+        meta: dict = {},
+        attrs: dict = {},
+        driver_kwargs: dict = {},
+        name: str = "",  # optional for now
+        catalog_name: str = "",  # optional for now
         **kwargs,
     ):
-        """Initiates data adapter for geospatial timeseries data.
+        """Initiate data adapter for geospatial timeseries data.
 
         This object contains all properties required to read supported files into
-        a single unified GeoDataset, i.e. :py:class:`xarray.Dataset` with geospatial point
-        geometries. In addition it keeps meta data to be able to reproduce which data is used.
+        a single unified GeoDataset, i.e. :py:class:`xarray.Dataset` with geospatial
+        point geometries. In addition it keeps meta data to be able to reproduce which
+        data is used.
 
         Parameters
         ----------
         path: str, Path
             Path to data source. If the dataset consists of multiple files, the path may
-            contain {variable}, {year}, {month} placeholders as well as path search pattern
-            using a '*' wildcard.
+            contain {variable}, {year}, {month} placeholders as well as path
+            search pattern using a '*' wildcard.
         driver: {'vector', 'netcdf', 'zarr'}, optional
-            Driver to read files with, for 'vector' :py:func:`~hydromt.io.open_geodataset`,
+            Driver to read files with,
+            for 'vector' :py:func:`~hydromt.io.open_geodataset`,
             for 'netcdf' :py:func:`xarray.open_mfdataset`.
             By default the driver is inferred from the file extension and falls back to
             'vector' if unknown.
         filesystem: {'local', 'gcs', 's3'}, optional
             Filesystem where the data is stored (local, cloud, http etc.).
             By default, local.
         crs: int, dict, or str, optional
-            Coordinate Reference System. Accepts EPSG codes (int or str); proj (str or dict)
-            or wkt (str). Only used if the data has no native CRS.
+            Coordinate Reference System. Accepts EPSG codes (int or str);
+            proj (str or dict) or wkt (str). Only used if the data has no native CRS.
         nodata: float, int, optional
             Missing value number. Only used if the data has no native missing value.
             Nodata values can be differentiated between variables using a dictionary.
         rename: dict, optional
             Mapping of native data source variable to output source variable name as
             required by hydroMT.
         unit_mult, unit_add: dict, optional
-            Scaling multiplication and addition to change to map from the native data unit
-            to the output data unit as required by hydroMT.
+            Scaling multiplication and addition to change to map from the native
+            data unit to the output data unit as required by hydroMT.
         meta: dict, optional
             Metadata information of dataset, prefably containing the following keys:
-            {'source_version', 'source_url', 'source_license', 'paper_ref', 'paper_doi', 'category'}
+            - 'source_version'
+            - 'source_url'
+            - 'source_license'
+            - 'paper_ref'
+            - 'paper_doi'
+            - 'category'
         placeholders: dict, optional
-            Placeholders to expand yaml entry to multiple entries (name and path) based on placeholder values
-        **kwargs
+            Placeholders to expand yaml entry to multiple entries (name and path)
+            based on placeholder values
+        attrs: dict, optional
+            Additional attributes relating to data variables. For instance unit
+            or long name of the variable.
+        driver_kwargs, dict, optional
             Additional key-word arguments passed to the driver.
+        name, catalog_name: str, optional
+            Name of the dataset and catalog, optional for now.
         """
+        if kwargs:
+            warnings.warn(
+                "Passing additional keyword arguments to be used by the "
+                "GeoDatasetAdapter driver is deprecated and will be removed "
+                "in a future version. Please use 'driver_kwargs' instead.",
+                DeprecationWarning,
+            )
+            driver_kwargs.update(kwargs)
         super().__init__(
             path=path,
             driver=driver,
             filesystem=filesystem,
-            crs=crs,
             nodata=nodata,
             rename=rename,
             unit_mult=unit_mult,
             unit_add=unit_add,
             meta=meta,
-            **kwargs,
+            attrs=attrs,
+            driver_kwargs=driver_kwargs,
+            name=name,
+            catalog_name=catalog_name,
         )
+        self.crs = crs
 
     def to_file(
         self,
         data_root,
         data_name,
         bbox=None,
         time_tuple=None,
@@ -119,32 +151,50 @@
             Start and end date of period of interest. By default the entire time period
             of the dataset is returned.
         driver : str, optional
             Driver to write file, e.g.: 'netcdf', 'zarr', by default None
         variables : list of str, optional
             Names of GeoDataset variables to return. By default all dataset variables
             are returned.
+        logger : logger object, optional
+            The logger object used for logging messages. If not provided, the default
+            logger will be used.
+        **kwargs
+            Additional keyword arguments that are passed to the `to_zarr`
+            function.
 
         Returns
         -------
         fn_out: str
             Absolute path to output file
         driver: str
-            Name of driver to read data with, see :py:func:`~hydromt.data_catalog.DataCatalog.get_geodataset`
+            Name of driver to read data with, see
+            :py:func:`~hydromt.data_catalog.DataCatalog.get_geodataset`
         """
         obj = self.get_data(
             bbox=bbox,
             time_tuple=time_tuple,
             variables=variables,
             logger=logger,
             single_var_as_array=variables is None,
         )
         if obj.vector.index.size == 0 or ("time" in obj.coords and obj.time.size == 0):
             return None, None
 
+        # much better for mem/storage/processing if dtypes are set correctly
+        for name, coord in obj.coords.items():
+            if coord.values.dtype != object:
+                continue
+
+            # not sure if coordinates values of different dtypes
+            # are possible, but let's just hope users aren't
+            # that mean for now.
+            if isinstance(coord.values[0], str):
+                obj[name] = obj[name].astype(str)
+
         if driver is None or driver == "netcdf":
             # always write netcdf
             driver = "netcdf"
             dvars = [obj.name] if isinstance(obj, xr.DataArray) else obj.vector.vars
             if variables is None:
                 encoding = {k: {"zlib": True} for k in dvars}
                 fn_out = join(data_root, f"{data_name}.nc")
@@ -172,41 +222,43 @@
         geom=None,
         buffer=0,
         variables=None,
         time_tuple=None,
         single_var_as_array=True,
         logger=logger,
     ):
-        """Returns a clipped, sliced and unified GeoDataset based on the properties
-        of this GeoDatasetAdapter.
+        """Return a clipped, sliced and unified GeoDataset.
 
-        For a detailed description see: :py:func:`~hydromt.data_catalog.DataCatalog.get_geodataset`
+        For a detailed description see:
+        :py:func:`~hydromt.data_catalog.DataCatalog.get_geodataset`
         """
         # If variable is string, convert to list
         if variables:
             variables = np.atleast_1d(variables).tolist()
 
         # Extract storage_options from kwargs to instantiate fsspec object correctly
-        if "storage_options" in self.kwargs and self.driver == "zarr":
-            kwargs = self.kwargs["storage_options"]
-            # For s3, anonymous connection still requires --no-sign-request profile to read the data
+        so_kwargs = dict()
+        if "storage_options" in self.driver_kwargs and self.driver == "zarr":
+            so_kwargs = self.driver_kwargs["storage_options"]
+            # For s3, anonymous connection still requires --no-sign-request profile to
+            # read the data
             # setting environment variable works
-            if "anon" in kwargs:
+            if "anon" in so_kwargs:
                 os.environ["AWS_NO_SIGN_REQUEST"] = "YES"
             else:
                 os.environ["AWS_NO_SIGN_REQUEST"] = "NO"
-        elif "storage_options" in self.kwargs:
+        elif "storage_options" in self.driver_kwargs:
             raise NotImplementedError(
                 "Remote (cloud) GeoDataset only supported with driver zarr."
             )
-        else:
-            kwargs = dict()
-        fns = self.resolve_paths(time_tuple=time_tuple, variables=variables, **kwargs)
+        fns = self.resolve_paths(
+            time_tuple=time_tuple, variables=variables, **so_kwargs
+        )
 
-        kwargs = self.kwargs.copy()
+        kwargs = self.driver_kwargs.copy()
 
         # parse geom, bbox and buffer arguments
         clip_str = ""
         if geom is None and bbox is not None:
             # convert bbox to geom with crs EPGS:4326 to apply buffer later
             geom = gpd.GeoDataFrame(geometry=[box(*bbox)], crs=4326)
             clip_str = " and clip to bbox (epsg:4326)"
@@ -262,15 +314,15 @@
             raise ValueError(f"GeoDataset: No spatial coords found in data {self.path}")
         if variables is not None:
             if np.any([var not in ds_out.data_vars for var in variables]):
                 raise ValueError(f"GeoDataset: Not all variables found: {variables}")
             ds_out = ds_out[variables]
 
         # set crs
-        if ds_out.vector.crs is None and self.crs != None:
+        if ds_out.vector.crs is None and self.crs is not None:
             ds_out.vector.set_crs(self.crs)
         if ds_out.vector.crs is None:
             raise ValueError(
                 "GeoDataset: The data has no CRS, set in GeoDatasetAdapter."
             )
 
         # clip
@@ -298,15 +350,15 @@
             if dt != 0:
                 logger.debug(f"GeoDataset: Shifting time labels with {dt} sec.")
                 ds_out["time"] = ds_out["time"] + pd.to_timedelta(dt, unit="s")
             if time_tuple is not None:
                 logger.debug(f"GeoDataset: Slicing time dim {time_tuple}")
                 ds_out = ds_out.sel(time=slice(*time_tuple))
             if ds_out.time.size == 0:
-                logger.warning(f"GeoDataset: Time slice out of range.")
+                logger.warning("GeoDataset: Time slice out of range.")
                 drop_vars = [v for v in ds_out.data_vars if "time" in ds_out[v].dims]
                 ds_out = ds_out.drop_vars(drop_vars)
 
         # set nodata value
         if self.nodata is not None:
             if not isinstance(self.nodata, dict):
                 nodata = {k: self.nodata for k in ds_out.data_vars.keys()}
@@ -334,11 +386,19 @@
             ds_out[name] = xr.where(data_bool, da * m + a, nodata)
             ds_out[name].attrs.update(attrs)  # set original attributes
 
         # return data array if single var
         if single_var_as_array and len(ds_out.vector.vars) == 1:
             ds_out = ds_out[ds_out.vector.vars[0]]
 
+        # Set variable attribute data
+        if self.attrs:
+            if isinstance(ds_out, xr.DataArray):
+                ds_out.attrs.update(self.attrs[ds_out.name])
+            else:
+                for k in self.attrs:
+                    ds_out[k].attrs.update(self.attrs[k])
+
         # set meta data
         ds_out.attrs.update(self.meta)
 
         return ds_out
```

### Comparing `hydromt-0.7.1/hydromt/data_adapter/rasterdataset.py` & `hydromt-0.8.0/hydromt/data_adapter/rasterdataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,107 +1,139 @@
-# -*- coding: utf-8 -*-
+"""Implementation for the RasterDatasetAdapter."""
+import logging
 import os
+import warnings
+from os import PathLike
 from os.path import join
-from fsspec.implementations import local
+from typing import NewType, Union
+
 import numpy as np
 import pandas as pd
+import pyproj
+import rasterio
 import xarray as xr
-import geopandas as gpd
-from shapely.geometry import box
-import warnings
-import logging
-from typing import Union, NewType
-from pathlib import Path
 
 from .. import gis_utils, io
-from .data_adapter import DataAdapter, PREPROCESSORS
-from .caching import cache_vrt_tiles
 from ..raster import GEO_MAP_COORD
-
+from .caching import cache_vrt_tiles
+from .data_adapter import PREPROCESSORS, DataAdapter
 
 logger = logging.getLogger(__name__)
 
 __all__ = ["RasterDatasetAdapter", "RasterDatasetSource"]
 
-RasterDatasetSource = NewType("RasterDatasetSource", Union[str, Path])
+RasterDatasetSource = NewType("RasterDatasetSource", Union[str, PathLike])
 
 
 class RasterDatasetAdapter(DataAdapter):
+
+    """Implementation for the RasterDatasetAdapter."""
+
     _DEFAULT_DRIVER = "raster"
     _DRIVERS = {
         "nc": "netcdf",
         "zarr": "zarr",
     }
 
     def __init__(
         self,
-        path,
-        driver=None,
-        filesystem="local",
-        crs=None,
-        nodata=None,
-        rename={},
-        unit_mult={},
-        unit_add={},
-        units={},
-        meta={},
+        path: str,
+        driver: str = None,
+        filesystem: str = "local",
+        crs: Union[int, str, dict] = None,
+        nodata: Union[dict, float, int] = None,
+        rename: dict = {},
+        unit_mult: dict = {},
+        unit_add: dict = {},
+        meta: dict = {},
+        attrs: dict = {},
+        driver_kwargs: dict = {},
+        zoom_levels: dict = {},
+        name: str = "",  # optional for now
+        catalog_name: str = "",  # optional for now
         **kwargs,
     ):
-        """Initiates data adapter for geospatial raster data.
+        """Initiate data adapter for geospatial raster data.
 
         This object contains all properties required to read supported raster files into
-        a single unified RasterDataset, i.e. :py:class:`xarray.Dataset` with geospatial attributes.
-        In addition it keeps meta data to be able to reproduce which data is used.
+        a single unified RasterDataset, i.e. :py:class:`xarray.Dataset` with geospatial
+        attributes. In addition it keeps meta data to be able to reproduce
+        which data is used.
 
         Parameters
         ----------
         path: str, Path
             Path to data source. If the dataset consists of multiple files, the path may
-            contain {variable}, {year}, {month} placeholders as well as path search pattern
-            using a '*' wildcard.
+            contain {variable}, {year}, {month} placeholders as well as path
+            search pattern using a '*' wildcard.
         driver: {'raster', 'netcdf', 'zarr', 'raster_tindex'}, optional
-            Driver to read files with, for 'raster' :py:func:`~hydromt.io.open_mfraster`,
-            for 'netcdf' :py:func:`xarray.open_mfdataset`, and for 'zarr' :py:func:`xarray.open_zarr`
+            Driver to read files with,
+            for 'raster' :py:func:`~hydromt.io.open_mfraster`,
+            for 'netcdf' :py:func:`xarray.open_mfdataset`,
+            and for 'zarr' :py:func:`xarray.open_zarr`
             By default the driver is inferred from the file extension and falls back to
             'raster' if unknown.
         filesystem: {'local', 'gcs', 's3'}, optional
             Filesystem where the data is stored (local, cloud, http etc.).
             By default, local.
         crs: int, dict, or str, optional
-            Coordinate Reference System. Accepts EPSG codes (int or str); proj (str or dict)
-            or wkt (str). Only used if the data has no native CRS.
+            Coordinate Reference System. Accepts EPSG codes (int or str);
+            proj (str or dict) or wkt (str). Only used if the data has no native CRS.
         nodata: float, int, optional
             Missing value number. Only used if the data has no native missing value.
             Nodata values can be differentiated between variables using a dictionary.
         rename: dict, optional
             Mapping of native data source variable to output source variable name as
             required by hydroMT.
         unit_mult, unit_add: dict, optional
-            Scaling multiplication and addition to change to map from the native data unit
-            to the output data unit as required by hydroMT.
+            Scaling multiplication and addition to change to map from the native
+            data unit to the output data unit as required by hydroMT.
         meta: dict, optional
-            Metadata information of dataset, preferably containing the following keys:
-            {'source_version', 'source_url', 'source_license', 'paper_ref', 'paper_doi', 'category'}
-        **kwargs
+            Metadata information of dataset, prefably containing the following keys:
+            {'source_version', 'source_url', 'source_license',
+            'paper_ref', 'paper_doi', 'category'}
+        placeholders: dict, optional
+            Placeholders to expand yaml entry to multiple entries (name and path)
+            based on placeholder values
+        attrs: dict, optional
+            Additional attributes relating to data variables. For instance unit
+            or long name of the variable.
+        driver_kwargs, dict, optional
             Additional key-word arguments passed to the driver.
+        name, catalog_name: str, optional
+            Name of the dataset and catalog, optional for now.
+        zoomlevels: dict, optional
+            Dictionary with zoom levels and associated resolution in the unit of the
+            data CRS.
+
         """
+        if kwargs:
+            warnings.warn(
+                "Passing additional keyword arguments to be used by the "
+                "RasterDatasetAdapter driver is deprecated and will be removed "
+                "in a future version. Please use 'driver_kwargs' instead.",
+                DeprecationWarning,
+            )
+            driver_kwargs.update(kwargs)
         super().__init__(
             path=path,
             driver=driver,
             filesystem=filesystem,
-            crs=crs,
             nodata=nodata,
             rename=rename,
             unit_mult=unit_mult,
             unit_add=unit_add,
             meta=meta,
-            **kwargs,
+            attrs=attrs,
+            driver_kwargs=driver_kwargs,
+            name=name,
+            catalog_name=catalog_name,
         )
-        # TODO: see if the units argument can be solved with unit_mult/unit_add
-        self.units = units
+        self.crs = crs
+        self.zoom_levels = zoom_levels
 
     def to_file(
         self,
         data_root,
         data_name,
         bbox=None,
         time_tuple=None,
@@ -120,27 +152,34 @@
             Name of output file without extension.
         bbox : array-like of floats
             (xmin, ymin, xmax, ymax) bounding box of area of interest.
         time_tuple : tuple of str, datetime, optional
             Start and end date of period of interest. By default the entire time period
             of the dataset is returned.
         driver : str, optional
-            Driver to write file, e.g.: 'netcdf', 'zarr' or any gdal data type, by default None
+            Driver to write file, e.g.: 'netcdf', 'zarr' or any gdal data type,
+            by default None
         variables : list of str, optional
             Names of GeoDataset variables to return. By default all dataset variables
             are returned.
+        logger : logger object, optional
+            The logger object used for logging messages. If not provided, the default
+            logger will be used.
+        **kwargs
+            Additional keyword arguments that are passed to the `to_netcdf`
+            function.
 
         Returns
         -------
         fn_out: str
             Absolute path to output file
         driver: str
-            Name of driver to read data with, see :py:func:`~hydromt.data_catalog.DataCatalog.get_rasterdataset`
+            Name of driver to read data with, see
+            :py:func:`~hydromt.data_catalog.DataCatalog.get_rasterdataset`
         """
-
         try:
             obj = self.get_data(
                 bbox=bbox,
                 time_tuple=time_tuple,
                 variables=variables,
                 logger=logger,
                 single_var_as_array=variables is None,
@@ -196,48 +235,48 @@
         align=None,
         variables=None,
         time_tuple=None,
         single_var_as_array=True,
         cache_root=None,
         logger=logger,
     ):
-        """Returns a clipped, sliced and unified RasterDataset based on the properties
-        of this RasterDatasetAdapter.
+        """Return a clipped, sliced and unified RasterDataset.
 
-        For a detailed description see: :py:func:`~hydromt.data_catalog.DataCatalog.get_rasterdataset`
+        For a detailed description see:
+        :py:func:`~hydromt.data_catalog.DataCatalog.get_rasterdataset`
         """
         # If variable is string, convert to list
         if variables:
             variables = np.atleast_1d(variables).tolist()
 
         # Extract storage_options from kwargs to instantiate fsspec object correctly
-        if "storage_options" in self.kwargs:
-            so_kwargs = self.kwargs["storage_options"]
-            # For s3, anonymous connection still requires --no-sign-request profile to read the data
-            # setting environment variable works
+        so_kwargs = dict()
+        if "storage_options" in self.driver_kwargs:
+            so_kwargs = self.driver_kwargs["storage_options"]
+            # For s3, anonymous connection still requires --no-sign-request profile to
+            # read the data setting environment variable works
             if "anon" in so_kwargs:
                 os.environ["AWS_NO_SIGN_REQUEST"] = "YES"
             else:
                 os.environ["AWS_NO_SIGN_REQUEST"] = "NO"
-        else:
-            so_kwargs = dict()
 
         # resolve path based on time, zoom level and/or variables
         fns = self.resolve_paths(
             time_tuple=time_tuple,
             variables=variables,
             zoom_level=zoom_level,
             geom=geom,
             bbox=bbox,
             logger=logger,
             **so_kwargs,
         )
 
-        kwargs = self.kwargs.copy()
-        # zarr can use storage options directly, the rest should be converted to file-like objects
+        kwargs = self.driver_kwargs.copy()
+        # zarr can use storage options directly, the rest should be converted to
+        # file-like objects
         if "storage_options" in kwargs and self.driver == "raster":
             storage_options = kwargs.pop("storage_options")
             fs = self.get_filesystem(**storage_options)
             fns = [fs.open(f) for f in fns]
 
         # read using various readers
         if self.driver in ["netcdf"]:  # TODO complete list
@@ -268,15 +307,16 @@
                 if np.issubdtype(type(self.nodata), np.number):
                     kwargs.update(nodata=self.nodata)
                 ds_out = io.open_raster_from_tindex(
                     fns[0], bbox=bbox, geom=geom, **kwargs
                 )
             else:
                 raise NotImplementedError(
-                    "Remote (cloud) RasterDataset not supported with driver raster_tindex."
+                    "Remote (cloud) RasterDataset not supported "
+                    "with driver raster_tindex."
                 )
         elif self.driver == "raster":  # rasterio files
             if cache_root is not None and all([str(fn).endswith(".vrt") for fn in fns]):
                 cache_dir = join(cache_root, self.catalog_name, self.name)
                 fns_cached = []
                 for fn in fns:
                     fn1 = cache_vrt_tiles(
@@ -288,84 +328,84 @@
                 kwargs.update(nodata=self.nodata)
             ds_out = io.open_mfraster(fns, logger=logger, **kwargs)
         else:
             raise ValueError(f"RasterDataset: Driver {self.driver} unknown")
         if GEO_MAP_COORD in ds_out.data_vars:
             ds_out = ds_out.set_coords(GEO_MAP_COORD)
 
-        # transpose dims to get y and x dim last
-        x_dim = ds_out.raster.x_dim
-        y_dim = ds_out.raster.y_dim
-        ds_out = ds_out.transpose(..., y_dim, x_dim)
-
         # rename and select vars
         if variables and len(ds_out.raster.vars) == 1 and len(self.rename) == 0:
             rm = {ds_out.raster.vars[0]: variables[0]}
-            if rm.keys() != rm.values():
+            if set(rm.keys()) != set(rm.values()):
                 warnings.warn(
-                    f"Automatic renaming of single var array will be deprecated, rename {rm} in the data catalog instead.",
+                    "Automatic renaming of single var array will be deprecated, rename"
+                    f" {rm} in the data catalog instead.",
                     DeprecationWarning,
                 )
         else:
             rm = {k: v for k, v in self.rename.items() if k in ds_out}
         ds_out = ds_out.rename(rm)
         if variables is not None:
             if np.any([var not in ds_out.data_vars for var in variables]):
                 raise ValueError(f"RasterDataset: Not all variables found: {variables}")
             ds_out = ds_out[variables]
 
+        # transpose dims to get y and x dim last
+        x_dim = ds_out.raster.x_dim
+        y_dim = ds_out.raster.y_dim
+        ds_out = ds_out.transpose(..., y_dim, x_dim)
+
         # clip tslice
         if (
             "time" in ds_out.dims
             and ds_out["time"].size > 1
             and np.issubdtype(ds_out["time"].dtype, np.datetime64)
         ):
             dt = self.unit_add.get("time", 0)
             if dt != 0:
                 logger.debug(f"RasterDataset: Shifting time labels with {dt} sec.")
                 ds_out["time"] = ds_out["time"] + pd.to_timedelta(dt, unit="s")
             if time_tuple is not None:
                 logger.debug(f"RasterDataset: Slicing time dim {time_tuple}")
                 ds_out = ds_out.sel({"time": slice(*time_tuple)})
             if ds_out.time.size == 0:
-                raise IndexError(f"RasterDataset: Time slice out of range.")
+                raise IndexError("RasterDataset: Time slice out of range.")
 
         # set crs
-        if ds_out.raster.crs is None and self.crs != None:
+        if ds_out.raster.crs is None and self.crs is not None:
             ds_out.raster.set_crs(self.crs)
         elif ds_out.raster.crs is None:
             raise ValueError(
                 "RasterDataset: The data has no CRS, set in RasterDatasetAdapter."
             )
 
         # clip
-        epsg = ds_out.raster.crs.to_epsg()
+        # make sure bbox is in data crs
+        crs = ds_out.raster.crs
+        epsg = crs.to_epsg()  # this could return None
         if geom is not None:
-            bbox = geom.to_crs(4326).total_bounds
-        if epsg != 4326 and bbox is not None and geom is None:
-            geom = gpd.GeoDataFrame(geometry=[box(*bbox)], crs=4326)
-        elif epsg == 4326:
-            w, e = np.asarray(ds_out.raster.bounds)[[0, 2]]
+            bbox = geom.to_crs(crs).total_bounds
+        elif epsg != 4326 and bbox is not None:
+            crs4326 = pyproj.CRS.from_epsg(4326)
+            bbox = rasterio.warp.transform_bounds(crs4326, crs, *bbox)
+        # work with 4326 data that is defined at 0-360 degrees longtitude
+        if epsg == 4326:
+            e = ds_out.raster.bounds[2]
             if e > 180 or (bbox is not None and (bbox[0] < -180 or bbox[2] > 180)):
                 x_dim = ds_out.raster.x_dim
                 ds_out = gis_utils.meridian_offset(ds_out, x_dim, bbox).sortby(x_dim)
+        # clip with bbox
         if bbox is not None:
-            err = f"RasterDataset: No data within spatial domain for {self.path}."
-            try:
-                bbox_str = ", ".join([f"{c:.3f}" for c in bbox])
-                if geom is not None:
-                    logger.debug(f"RasterDataset: Clip with geom - [{bbox_str}]")
-                    ds_out = ds_out.raster.clip_geom(geom, buffer=buffer, align=align)
-                elif bbox is not None:
-                    logger.debug(f"RasterDataset: Clip with bbox - [{bbox_str}]")
-                    ds_out = ds_out.raster.clip_bbox(bbox, buffer=buffer, align=align)
-            except IndexError:
-                raise IndexError(err)
-            if ds_out.raster.xcoords.size == 0 or ds_out.raster.ycoords.size == 0:
-                raise IndexError(err)
+            bbox_str = ", ".join([f"{c:.3f}" for c in bbox])
+            logger.debug(f"RasterDataset: Clip with bbox - [{bbox_str}] (epsg:{epsg}))")
+            ds_out = ds_out.raster.clip_bbox(bbox, buffer=buffer, align=align)
+            if np.any(np.array(ds_out.raster.shape) < 2):
+                raise IndexError(
+                    f"RasterDataset: No data within spatial domain for {self.path}."
+                )
 
         # set nodata value
         if self.nodata is not None:
             if not isinstance(self.nodata, dict):
                 nodata = {k: self.nodata for k in ds_out.data_vars.keys()}
             else:
                 nodata = self.nodata
@@ -391,17 +431,16 @@
             nodata = np.nan if nodata_isnan else da.raster.nodata
             data_bool = ~np.isnan(da) if nodata_isnan else da != nodata
             ds_out[name] = xr.where(data_bool, da * m + a, nodata)
             ds_out[name].attrs.update(attrs)  # set original attributes
             ds_out[name].raster.set_nodata(nodata)  # reset nodata in case of change
 
         # unit attributes
-        # TODO: can we solve this with unit conversion or otherwise generalize meta
-        for k in self.units:
-            ds_out[k].attrs.update(units=self.units[k])
+        for k in self.attrs:
+            ds_out[k].attrs.update(self.attrs[k])
 
         # return data array if single var
         if single_var_as_array and len(ds_out.raster.vars) == 1:
             ds_out = ds_out[ds_out.raster.vars[0]]
 
         # set meta data
         ds_out.attrs.update(self.meta)
```

### Comparing `hydromt-0.7.1/hydromt/data_catalog.py` & `hydromt-0.8.0/hydromt/data_catalog.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,78 +1,92 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-"""DataCatalog module for HydroMT"""
+"""DataCatalog module for HydroMT."""
 from __future__ import annotations
-import os
-from os.path import join, isdir, dirname, basename, isfile, abspath, exists
+
 import copy
-from pathlib import Path
-from typing import Dict, List, Tuple, Union, Optional
+import inspect
+import itertools
+import logging
+import os
+import shutil
 import warnings
+from os.path import abspath, basename, exists, isdir, isfile, join
+from pathlib import Path
+from typing import Dict, List, Optional, Tuple, Union
+
+import geopandas as gpd
 import numpy as np
 import pandas as pd
-import geopandas as gpd
+import requests
 import xarray as xr
 import yaml
-import logging
-import requests
-import shutil
 from packaging.version import Version
-import itertools
 
+from . import __version__
 from .data_adapter import (
     DataAdapter,
-    RasterDatasetAdapter,
-    GeoDatasetAdapter,
-    GeoDataFrameAdapter,
     DataFrameAdapter,
+    GeoDataFrameAdapter,
+    GeoDatasetAdapter,
+    RasterDatasetAdapter,
 )
-from .data_adapter.caching import _uri_validator, _copyfile, HYDROMT_DATADIR
+from .data_adapter.caching import HYDROMT_DATADIR, _copyfile, _uri_validator
 
 logger = logging.getLogger(__name__)
 
 __all__ = [
     "DataCatalog",
 ]
 
 
 class DataCatalog(object):
+
+    """Base class for the data catalog object."""
+
     # root URL with data_catalog file
     _url = r"https://raw.githubusercontent.com/Deltares/hydromt/main/data/predefined_catalogs.yml"
     _cache_dir = HYDROMT_DATADIR
 
     def __init__(
         self,
         data_libs: Union[List, str] = [],
         fallback_lib: Optional[str] = "artifact_data",
         logger=logger,
         cache: bool = False,
         cache_dir: str = None,
         **artifact_keys,
     ) -> None:
-        """Catalog of DataAdapter sources to easily read from different files
-        and keep track of files which have been accessed.
+        """Catalog of DataAdapter sources.
+
+        Helps to easily read from different files and keep track of
+        files which have been accessed.
 
         Arguments
         ---------
         data_libs: (list of) str, Path, optional
-            One or more paths to data catalog yaml files or names of predefined data catalogs.
-            By default the data catalog is initiated without data entries.
-            See :py:func:`~hydromt.data_adapter.DataCatalog.from_yml` for accepted yaml format.
+            One or more paths to data catalog yaml files or names of predefined data
+            catalogs. By default the data catalog is initiated without data entries.
+            See :py:func:`~hydromt.data_adapter.DataCatalog.from_yml` for
+            accepted yaml format.
         fallback_lib:
-            Name of pre-defined data catalog to read if no data_libs are provided, by default 'artifact_data'.
+            Name of pre-defined data catalog to read if no data_libs are provided,
+            by default 'artifact_data'.
             If None, no default data catalog is used.
         cache: bool, optional
             Set to true to cache data locally before reading.
             Currently only implemented for tiled rasterdatasets, by default False.
         cache_dir: str, Path, optional
             Folder root path to cach data to, by default ~/.hydromt_data
         artifact_keys:
             Deprecated from version v0.5
+        logger : logger object, optional
+            The logger object used for logging messages. If not provided, the default
+            logger will be used.
         """
         if data_libs is None:  # legacy code. to be removed
             data_libs = []
         elif not isinstance(data_libs, list):  # make sure data_libs is a list
             data_libs = np.atleast_1d(data_libs).tolist()
         self._sources = {}  # dictionary of DataAdapter
         self._catalogs = {}  # dictionary of predefined Catalogs
@@ -116,71 +130,96 @@
     @property
     def keys(self) -> List:
         """Returns list of data source names."""
         return list(self._sources.keys())
 
     @property
     def predefined_catalogs(self) -> Dict:
+        """Return all predefined catalogs."""
         if not self._catalogs:
             self.set_predefined_catalogs()
         return self._catalogs
 
     def __getitem__(self, key: str) -> DataAdapter:
+        """Get the source."""
         return self._sources[key]
 
     def __setitem__(self, key: str, value: DataAdapter) -> None:
+        """Set or update adaptors."""
         if not isinstance(value, DataAdapter):
             raise ValueError(f"Value must be DataAdapter, not {type(key).__name__}.")
         if key in self._sources:
             self.logger.warning(f"Overwriting data source {key}.")
         return self._sources.__setitem__(key, value)
 
     def __iter__(self):
+        """Iterate over sources."""
         return self._sources.__iter__()
 
     def __len__(self):
+        """Return number of sources."""
         return self._sources.__len__()
 
     def __repr__(self):
+        """Prettyprint the sources."""
         return self.to_dataframe().__repr__()
 
     def _repr_html_(self):
         return self.to_dataframe()._repr_html_()
 
     def update(self, **kwargs) -> None:
         """Add data sources to library."""
         for k, v in kwargs.items():
             self[k] = v
 
     def set_predefined_catalogs(self, urlpath: Union[Path, str] = None) -> Dict:
+        """Initialise the predefined catalogs."""
         # get predefined_catalogs
         urlpath = self._url if urlpath is None else urlpath
-        # TODO cache predefined catalogs
-        self._catalogs = _yml_from_uri_or_path(urlpath)
+        cache_path = join(self._cache_dir, basename(urlpath))
+        try:
+            # download file locally; overwrite existing file
+            _copyfile(urlpath, cache_path)
+        except Exception:  # if offline
+            self.logger.warning(
+                "Downloading the predefined catalogs failed;"
+                "check your internet connection"
+            )
+            pass
+        if isfile(cache_path):
+            self._catalogs = _yml_from_uri_or_path(cache_path)
+        if self._catalogs is None:
+            raise ConnectionError(
+                "Predefined catalogs not found; check your internet connection."
+            )
         return self._catalogs
 
     def from_artifacts(
         self, name: str = "artifact_data", version: str = "latest"
     ) -> None:
-        """Deprecated method. Use :py:func:`hydromt.data_catalog.DataCatalog.from_predefined_catalogs` instead
+        """Parse artifacts.
+
+        Deprecated method. Use
+        :py:func:`hydromt.data_catalog.DataCatalog.from_predefined_catalogs` instead.
 
         Parameters
         ----------
         name : str, optional
             Catalog name. If None (default) sample data is downloaded.
         version : str, optional
             Release version. By default it takes the latest known release.
         """
         warnings.warn(
-            f'"from_artifacts" is deprecated. Use "from_predefined_catalogs instead".',
+            '"from_artifacts" is deprecated. Use "from_predefined_catalogs instead".',
             DeprecationWarning,
         )
         self.from_predefined_catalogs(name, version)
 
     def from_predefined_catalogs(self, name: str, version: str = "latest") -> None:
+        """Generate a catalogue from one of the predefined ones."""
         if "=" in name:
             name, version = name.split("=")[0], name.split("=")[-1]
         if name not in self.predefined_catalogs:
             raise ValueError(
                 f'Catalog with name "{name}" not found in predefined catalogs'
             )
         urlpath = self.predefined_catalogs[name].get("urlpath")
@@ -198,15 +237,15 @@
         else:
             self.logger.info(f"Reading data catalog {name} {version}")
             self.from_yml(urlpath)
 
     def from_archive(
         self, urlpath: Union[Path, str], version: str = None, name: str = None
     ) -> None:
-        """Read a data archive including a data_catalog.yml file"""
+        """Read a data archive including a data_catalog.yml file."""
         name = basename(urlpath).split(".")[0] if name is None else name
         root = join(self._cache_dir, name)
         if version is not None:
             root = join(root, version)
         archive_fn = join(root, basename(urlpath))
         yml_fn = join(root, "data_catalog.yml")
         if not isdir(root):
@@ -286,15 +325,26 @@
         # legacy code with root/category at highest yml level
         if "root" in yml:
             meta.update(root=yml.pop("root"))
         if "category" in yml:
             meta.update(category=yml.pop("category"))
         # read meta data
         meta = yml.pop("meta", meta)
+        self_version = Version(__version__)
+        hydromt_version = meta.get("hydromt_version", __version__)
+        yml_version = Version(hydromt_version)
+
+        if yml_version > self_version:
+            self.logger.warning(
+                f"Specified HydroMT version ({hydromt_version}) \
+                  more recent than installed version ({__version__}).",
+            )
+
         catalog_name = meta.get("name", "".join(basename(urlpath).split(".")[:-1]))
+
         # TODO keep meta data!! Note only possible if yml files are not merged
         if root is None:
             root = meta.get("root", os.path.dirname(urlpath))
         self.from_dict(
             yml,
             catalog_name=catalog_name,
             root=root,
@@ -323,16 +373,16 @@
         category: str, optional
             Global category for all sources in `data_dict`.
         mark_used: bool
             If True, append to used_data list.
 
         Examples
         --------
-        A data dictionary with two entries is provided below, where all the text between <>
-        should be filled by the user. See the specific data adapters
+        A data dictionary with two entries is provided below, where all the text between
+        <> should be filled by the user. See the specific data adapters
         for more information about the required and optional arguments.
 
         .. code-block:: text
 
             {
                 <name1>: {
                     "path": <path>,
@@ -377,22 +427,24 @@
 
         Parameters
         ----------
         path: str, Path
             yaml output path.
         root: str, Path, optional
             Global root for all relative paths in yaml file.
-            If "auto" (default) the data source paths are relative to the yaml output ``path``.
+            If "auto" (default) the data source paths are relative to the yaml
+            output ``path``.
         source_names: list, optional
-            List of source names to export, by default None in which case all sources are exported.
-            This argument is ignored if `used_only=True`.
+            List of source names to export, by default None in which case all sources
+            are exported. This argument is ignored if `used_only=True`.
         used_only: bool, optional
             If True, export only data entries kept in used_data list, by default False.
         meta: dict, optional
-            key-value pairs to add to the data catalog meta section, such as 'version', by default empty.
+            key-value pairs to add to the data catalog meta section, such as 'version',
+            by default empty.
         """
         source_names = self._used_data if used_only else source_names
         yml_dir = os.path.dirname(abspath(path))
         if root == "auto":
             root = yml_dir
         data_dict = self.to_dict(root=root, source_names=source_names, meta=meta)
         if str(root) == yml_dir:
@@ -410,19 +462,21 @@
         meta: dict = {},
     ) -> Dict:
         """Export the data catalog to a dictionary.
 
         Parameters
         ----------
         source_names : list, optional
-            List of source names to export, by default None in which case all sources are exported.
+            List of source names to export, by default None in which case all sources
+            are exported.
         root : str, Path, optional
             Global root for all relative paths in yml file.
         meta: dict, optional
-            key-value pairs to add to the data catalog meta section, such as 'version', by default empty.
+            key-value pairs to add to the data catalog meta section, such as 'version',
+            by default empty.
 
         Returns
         -------
         dict
             data catalog dictionary
         """
         sources_out = dict()
@@ -448,15 +502,15 @@
             source_dict = _process_dict(source_dict, logger=self.logger)  # TODO TEST
             sources_out.update({name: source_dict})
         if meta:
             sources_out = {"meta": meta, **sources_out}
         return sources_out
 
     def to_dataframe(self, source_names: List = []) -> pd.DataFrame:
-        """Return data catalog summary as DataFrame"""
+        """Return data catalog summary as DataFrame."""
         d = dict()
         for name, source in self._sources.items():
             if len(source_names) > 0 and name not in source_names:
                 continue
             d[name] = source.summary()
         return pd.DataFrame.from_dict(d, orient="index")
 
@@ -478,22 +532,24 @@
             Path to output folder
         bbox : array-like of floats
             (xmin, ymin, xmax, ymax) bounding box of area of interest.
         time_tuple : tuple of str, datetime, optional
             Start and end date of period of interest. By default the entire time period
             of the dataset is returned.
         source_names: list, optional
-            List of source names to export, by default None in which case all sources are exported.
-            Specific variables can be selected by appending them to the source name in square brackets.
-            For example, to export all variables of 'source_name1' and only 'var1' and 'var2' of 'source_name'
+            List of source names to export, by default None in which case all sources
+            are exported. Specific variables can be selected by appending them to the
+            source name in square brackets. For example, to export all variables of
+            'source_name1' and only 'var1' and 'var2' of 'source_name'
             use source_names=['source_name1', 'source_name2[var1,var2]']
         unit_conversion: boolean, optional
             If False skip unit conversion when parsing data from file, by default True.
         meta: dict, optional
-            key-value pairs to add to the data catalog meta section, such as 'version', by default empty.
+            key-value pairs to add to the data catalog meta section, such as 'version',
+            by default empty.
         append: bool, optional
             If True, append to existing data catalog, by default False.
         """
         data_root = abspath(data_root)
         if not os.path.isdir(data_root):
             os.makedirs(data_root)
 
@@ -546,15 +602,15 @@
                     source.unit_add = {}
                 else:
                     source.unit_mult = unit_mult
                     source.unit_add = unit_add
                 source.path = fn_out
                 source.driver = driver
                 source.filesystem = "local"
-                source.kwargs = {}
+                source.driver_kwargs = {}
                 source.rename = {}
                 if key in sources_out:
                     self.logger.warning(
                         f"{key} already exists in data catalog and is overwritten."
                     )
                 sources_out[key] = source
             except FileNotFoundError:
@@ -574,77 +630,85 @@
         buffer: Union[float, int] = 0,
         align: bool = None,
         variables: Union[List, str] = None,
         time_tuple: Tuple = None,
         single_var_as_array: bool = True,
         **kwargs,
     ) -> xr.Dataset:
-        """Returns a clipped, sliced and unified RasterDataset.
+        """Return a clipped, sliced and unified RasterDataset.
 
         To clip the data to the area of interest, provide a `bbox` or `geom`,
         with optional additional `buffer` and `align` arguments.
-        To slice the data to the time period of interest, provide the `time_tuple` argument.
-        To return only the dataset variables of interest provide the `variables` argument.
+        To slice the data to the time period of interest, provide the `time_tuple`
+        argument. To return only the dataset variables of interest provide the
+        `variables` argument.
 
         NOTE: Unless `single_var_as_array` is set to False a single-variable data source
-        will be returned as :py:class:`xarray.DataArray` rather than :py:class:`xarray.Dataset`.
+        will be returned as :py:class:`xarray.DataArray` rather than
+        :py:class:`xarray.Dataset`.
 
         Arguments
         ---------
         data_like: str, Path, xr.Dataset, xr.Datarray
             Data catalog key, path to raster file or raster xarray data object.
             If a path to a raster file is provided it will be added
             to the data_catalog with its based on the file basename without extension.
         bbox : array-like of floats
-            (xmin, ymin, xmax, ymax) bounding box of area of interest (in WGS84 coordinates).
+            (xmin, ymin, xmax, ymax) bounding box of area of interest
+            (in WGS84 coordinates).
         geom : geopandas.GeoDataFrame/Series,
             A geometry defining the area of interest.
         zoom_level : int, tuple, optional
             Zoom level of the xyz tile dataset (0 is base level)
-            Using a tuple the zoom level can be specified as (<zoom_resolution>, <unit>),
-            e.g., (1000, 'meter')
+            Using a tuple the zoom level can be specified as
+            (<zoom_resolution>, <unit>), e.g., (1000, 'meter')
         buffer : int, optional
             Buffer around the `bbox` or `geom` area of interest in pixels. By default 0.
         align : float, optional
             Resolution to align the bounding box, by default None
         variables : str or list of str, optional.
             Names of RasterDataset variables to return. By default all dataset variables
             are returned.
         time_tuple : tuple of str, datetime, optional
             Start and end date of period of interest. By default the entire time period
             of the dataset is returned.
         single_var_as_array: bool, optional
             If True, return a DataArray if the dataset consists of a single variable.
             If False, always return a Dataset. By default True.
+        **kwargs:
+            Additional keyword arguments that are passed to the `RasterDatasetAdapter`
+            function. Only used if `data_like` is a path to a raster file.
 
         Returns
         -------
         obj: xarray.Dataset or xarray.DataArray
             RasterDataset
         """
         if isinstance(data_like, (xr.DataArray, xr.Dataset)):
             return data_like
         elif not isinstance(data_like, (str, Path)):
             raise ValueError(f'Unknown raster data type "{type(data_like).__name__}"')
 
         if data_like not in self.sources and exists(abspath(data_like)):
             path = str(abspath(data_like))
             name = basename(data_like).split(".")[0]
-            self.update(**{name: RasterDatasetAdapter(path=path, **kwargs)})
+            source = RasterDatasetAdapter(path=path, **kwargs)
+            self.update(**{name: source})
         elif data_like in self.sources:
             name = data_like
+            source = self.sources[name]
         else:
             raise FileNotFoundError(f"No such file or catalog key: {data_like}")
 
         self._used_data.append(name)
-        source = self.sources[name]
         self.logger.info(
-            f"DataCatalog: Getting {name} RasterDataset {source.driver} data from {source.path}"
+            f"DataCatalog: Getting {name} RasterDataset {source.driver} data from"
+            f" {source.path}"
         )
-        obj = self.sources[name].get_data(
+        obj = source.get_data(
             bbox=bbox,
             geom=geom,
             buffer=buffer,
             zoom_level=zoom_level,
             align=align,
             variables=variables,
             time_tuple=time_tuple,
@@ -660,64 +724,72 @@
         bbox: List = None,
         geom: gpd.GeoDataFrame = None,
         buffer: Union[float, int] = 0,
         variables: Union[List, str] = None,
         predicate: str = "intersects",
         **kwargs,
     ):
-        """Returns a clipped and unified GeoDataFrame (vector).
+        """Return a clipped and unified GeoDataFrame (vector).
 
         To clip the data to the area of interest, provide a `bbox` or `geom`,
         with optional additional `buffer` and `align` arguments.
-        To return only the dataframe columns of interest provide the `variables` argument.
+        To return only the dataframe columns of interest provide the
+        `variables` argument.
 
         Arguments
         ---------
         data_like: str, Path, gpd.GeoDataFrame
             Data catalog key, path to vector file or a vector geopandas object.
             If a path to a vector file is provided it will be added
             to the data_catalog with its based on the file basename without extension.
         bbox : array-like of floats
-            (xmin, ymin, xmax, ymax) bounding box of area of interest (in WGS84 coordinates).
+            (xmin, ymin, xmax, ymax) bounding box of area of interest
+            (in WGS84 coordinates).
         geom : geopandas.GeoDataFrame/Series,
             A geometry defining the area of interest.
         buffer : float, optional
             Buffer around the `bbox` or `geom` area of interest in meters. By default 0.
-        predicate : {'intersects', 'within', 'contains', 'overlaps', 'crosses', 'touches'}, optional
-            If predicate is provided, the GeoDataFrame is filtered by testing
-            the predicate function against each item. Requires bbox or mask.
-            By default 'intersects'
+        predicate : {'intersects', 'within', 'contains', 'overlaps',
+            'crosses', 'touches'}, optional If predicate is provided,
+            the GeoDataFrame is filtered by testing the predicate function
+            against each item. Requires bbox or mask. By default 'intersects'
         align : float, optional
             Resolution to align the bounding box, by default None
         variables : str or list of str, optional.
-            Names of GeoDataFrame columns to return. By default all columns are returned.
+            Names of GeoDataFrame columns to return. By default all columns are
+            returned.
+        **kwargs:
+            Additional keyword arguments that are passed to the `GeoDataFrameAdapter`
+            function. Only used if `data_like` is a path to a vector file.
 
         Returns
         -------
         gdf: geopandas.GeoDataFrame
             GeoDataFrame
         """
         if isinstance(data_like, gpd.GeoDataFrame):
             return data_like
         elif not isinstance(data_like, (str, Path)):
             raise ValueError(f'Unknown vector data type "{type(data_like).__name__}"')
 
         if data_like not in self.sources and exists(abspath(data_like)):
             path = str(abspath(data_like))
             name = basename(data_like).split(".")[0]
-            self.update(**{name: GeoDataFrameAdapter(path=path, **kwargs)})
+            source = GeoDataFrameAdapter(path=path, **kwargs)
+            self.update(**{name: source})
         elif data_like in self.sources:
             name = data_like
+            source = self.sources[name]
         else:
             raise FileNotFoundError(f"No such file or catalog key: {data_like}")
 
         self._used_data.append(name)
-        source = self.sources[name]
         self.logger.info(
-            f"DataCatalog: Getting {name} GeoDataFrame {source.driver} data from {source.path}"
+            f"DataCatalog: Getting {name} GeoDataFrame {source.driver} data"
+            f" from {source.path}"
         )
         gdf = source.get_data(
             bbox=bbox,
             geom=geom,
             buffer=buffer,
             predicate=predicate,
             variables=variables,
@@ -732,32 +804,34 @@
         geom: gpd.GeoDataFrame = None,
         buffer: Union[float, int] = 0,
         variables: List = None,
         time_tuple: Tuple = None,
         single_var_as_array: bool = True,
         **kwargs,
     ) -> xr.Dataset:
-        """Returns a clipped, sliced and unified GeoDataset.
+        """Return a clipped, sliced and unified GeoDataset.
 
         To clip the data to the area of interest, provide a `bbox` or `geom`,
         with optional additional `buffer` and `align` arguments.
-        To slice the data to the time period of interest, provide the `time_tuple` argument.
-        To return only the dataset variables of interest provide the `variables` argument.
+        To slice the data to the time period of interest, provide the
+        `time_tuple` argument. To return only the dataset variables
+        of interest provide the `variables` argument.
 
         NOTE: Unless `single_var_as_array` is set to False a single-variable data source
         will be returned as xarray.DataArray rather than Dataset.
 
         Arguments
         ---------
         data_like: str, Path, xr.Dataset, xr.DataArray
             Data catalog key, path to geodataset file or geodataset xarray object.
             If a path to a file is provided it will be added
             to the data_catalog with its based on the file basename without extension.
         bbox : array-like of floats
-            (xmin, ymin, xmax, ymax) bounding box of area of interest (in WGS84 coordinates).
+            (xmin, ymin, xmax, ymax) bounding box of area of interest
+            (in WGS84 coordinates).
         geom : geopandas.GeoDataFrame/Series,
             A geometry defining the area of interest.
         buffer : float, optional
             Buffer around the `bbox` or `geom` area of interest in meters. By default 0.
         align : float, optional
             Resolution to align the bounding box, by default None
         variables : str or list of str, optional.
@@ -765,38 +839,43 @@
             are returned.
         time_tuple : tuple of str, datetime, optional
             Start and end date of period of interest. By default the entire time period
             of the dataset is returned.
         single_var_as_array: bool, optional
             If True, return a DataArray if the dataset consists of a single variable.
             If False, always return a Dataset. By default True.
+        **kwargs:
+            Additional keyword arguments that are passed to the `GeoDatasetAdapter`
+            function. Only used if `data_like` is a path to a geodataset file.
 
         Returns
         -------
         obj: xarray.Dataset or xarray.DataArray
             GeoDataset
         """
         if isinstance(data_like, (xr.DataArray, xr.Dataset)):
             return data_like
         elif not isinstance(data_like, (str, Path)):
             raise ValueError(f'Unknown geo data type "{type(data_like).__name__}"')
 
         if data_like not in self.sources and exists(abspath(data_like)):
             path = str(abspath(data_like))
             name = basename(data_like).split(".")[0]
-            self.update(**{name: GeoDatasetAdapter(path=path, **kwargs)})
+            source = GeoDatasetAdapter(path=path, **kwargs)
+            self.update(**{name: source})
         elif data_like in self.sources:
             name = data_like
+            source = self.sources[name]
         else:
             raise FileNotFoundError(f"No such file or catalog key: {data_like}")
 
         self._used_data.append(name)
-        source = self.sources[name]
         self.logger.info(
-            f"DataCatalog: Getting {name} GeoDataset {source.driver} data from {source.path}"
+            f"DataCatalog: Getting {name} GeoDataset {source.driver} data"
+            f" from {source.path}"
         )
         obj = source.get_data(
             bbox=bbox,
             geom=geom,
             buffer=buffer,
             variables=variables,
             time_tuple=time_tuple,
@@ -808,52 +887,57 @@
     def get_dataframe(
         self,
         data_like: Union[str, Path, pd.DataFrame],
         variables: list = None,
         time_tuple: tuple = None,
         **kwargs,
     ):
-        """Returns a unified and sliced DataFrame.
+        """Return a unified and sliced DataFrame.
 
         Parameters
         ----------
         data_like : str, Path, pd.DataFrame
-            Data catalog key, path to tabular data file or tabular pandas dataframe object.
-            If a path to a tabular data file is provided it will be added
+            Data catalog key, path to tabular data file or tabular pandas dataframe
+            object. If a path to a tabular data file is provided it will be added
             to the data_catalog with its based on the file basename without extension.
         variables : str or list of str, optional.
             Names of GeoDataset variables to return. By default all dataset variables
             are returned.
         time_tuple : tuple of str, datetime, optional
             Start and end date of period of interest. By default the entire time period
             of the dataset is returned.
+        **kwargs:
+            Additional keyword arguments that are passed to the `DataframeAdapter`
+            function. Only used if `data_like` is a path to a tabular data file.
 
         Returns
         -------
         pd.DataFrame
             Tabular data
         """
         if isinstance(data_like, pd.DataFrame):
             return data_like
         elif not isinstance(data_like, (str, Path)):
             raise ValueError(f'Unknown tabular data type "{type(data_like).__name__}"')
 
         if data_like not in self.sources and exists(abspath(data_like)):
             path = str(abspath(data_like))
             name = basename(data_like).split(".")[0]
-            self.update(**{name: DataFrameAdapter(path=path, **kwargs)})
+            source = DataFrameAdapter(path=path, **kwargs)
+            self.update(**{name: source})
         elif data_like in self.sources:
             name = data_like
+            source = self.sources[name]
         else:
             raise FileNotFoundError(f"No such file or catalog key: {data_like}")
 
         self._used_data.append(name)
-        source = self.sources[name]
         self.logger.info(
-            f"DataCatalog: Getting {name} DataFrame {source.driver} data from {source.path}"
+            f"DataCatalog: Getting {name} DataFrame {source.driver} data"
+            f" from {source.path}"
         )
         obj = source.get_data(
             variables=variables,
             time_tuple=time_tuple,
             logger=self.logger,
         )
         return obj
@@ -877,14 +961,15 @@
     if root is None:
         root = data_dict.pop("root", None)
 
     # parse data
     data = dict()
     for name, source in data_dict.items():
         source = source.copy()  # important as we modify with pop
+
         if "alias" in source:
             alias = source.pop("alias")
             if alias not in data_dict:
                 raise ValueError(f"alias {alias} not found in data_dict.")
             # use alias source but overwrite any attributes with original source
             source_org = source.copy()
             source = data_dict[alias].copy()
@@ -896,51 +981,70 @@
             raise ValueError(f"{name}: Data type missing.")
         elif data_type not in ADAPTERS:
             raise ValueError(f"{name}: Data type {data_type} unknown")
         adapter = ADAPTERS.get(data_type)
         # Only for local files
         path = source.pop("path")
         # if remote path, keep as is else call abs_path method to solve local files
-        if not _uri_validator(path):
+        if not _uri_validator(str(path)):
             path = abs_path(root, path)
         meta = source.pop("meta", {})
         if "category" not in meta and category is not None:
             meta.update(category=category)
+        # Get unit attrs if given from source
+        attrs = source.pop("attrs", {})
         # lower kwargs for backwards compatability
-        # FIXME this could be problamatic if driver kwargs conflict DataAdapter arguments
-        source.update(**source.pop("kwargs", {}))
+        # FIXME this could be problamatic if driver kwargs conflict DataAdapter
+        #  arguments
+        driver_kwargs = source.pop("driver_kwargs", source.pop("kwargs", {}))
+        for driver_kwarg in driver_kwargs:
+            # required for geodataset where driver_kwargs can be a path
+            if "fn" in driver_kwarg:
+                driver_kwargs.update(
+                    {driver_kwarg: abs_path(root, driver_kwargs[driver_kwarg])}
+                )
         for opt in source:
             if "fn" in opt:  # get absolute paths for file names
                 source.update({opt: abs_path(root, source[opt])})
         if "placeholders" in source:
             # pop avoid placeholders being passed to adapter
             options = source.pop("placeholders")
             for combination in itertools.product(*options.values()):
                 path_n = path
                 name_n = name
                 for k, v in zip(options.keys(), combination):
                     path_n = path_n.replace("{" + k + "}", v)
                     name_n = name_n.replace("{" + k + "}", v)
+
                 data[name_n] = adapter(
                     path=path_n,
                     name=name_n,
                     catalog_name=catalog_name,
                     meta=meta,
-                    **source,
+                    attrs=attrs,
+                    driver_kwargs=driver_kwargs,
+                    **source,  # key word arguments specific to certain adaptors
                 )
+
         else:
             data[name] = adapter(
-                path=path, name=name, catalog_name=catalog_name, meta=meta, **source
+                path=path,
+                name=name,
+                catalog_name=catalog_name,
+                meta=meta,
+                attrs=attrs,
+                driver_kwargs=driver_kwargs,
+                **source,
             )
 
     return data
 
 
 def _yml_from_uri_or_path(uri_or_path: Union[Path, str]) -> Dict:
-    if _uri_validator(uri_or_path):
+    if _uri_validator(str(uri_or_path)):
         with requests.get(uri_or_path, stream=True) as r:
             if r.status_code != 200:
                 raise IOError(f"URL {r.content}: {uri_or_path}")
             yml = yaml.load(r.text, Loader=yaml.FullLoader)
     else:
         with open(uri_or_path, "r") as stream:
             yml = yaml.load(stream, Loader=yaml.FullLoader)
@@ -951,20 +1055,29 @@
     """Recursively change dict values to keep only python literal structures."""
     for k, v in d.items():
         _check_key = isinstance(k, str)
         if _check_key and isinstance(v, dict):
             d[k] = _process_dict(v)
         elif _check_key and isinstance(v, Path):
             d[k] = str(v)  # path to string
-        # elif not _check_key or not isinstance(v, (list, str, int, float, bool)):
-        #     d.pop(k)  # remove this entry
-        #     logger.debug(f'Removing non-serializable entry "{k}"')
     return d
 
 
 def abs_path(root: Union[Path, str], rel_path: Union[Path, str]) -> str:
     path = Path(str(rel_path))
     if not path.is_absolute():
         if root is not None:
             rel_path = join(root, rel_path)
         path = Path(abspath(rel_path))
     return str(path)
+
+
+def _seperate_driver_kwargs_from_kwargs(
+    kwargs: dict, data_adapter: DataAdapter
+) -> Tuple[dict]:
+    driver_kwargs = kwargs
+    driver_kwargs_copy = driver_kwargs.copy()
+    kwargs = {}
+    for k, v in driver_kwargs_copy.items():
+        if k in inspect.signature(data_adapter.__init__).parameters.keys():
+            kwargs.update({k: driver_kwargs.pop(k)})
+    return kwargs, driver_kwargs
```

### Comparing `hydromt-0.7.1/hydromt/flw.py` & `hydromt-0.8.0/hydromt/flw.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
+"""Hydrological flow direction methods powered by pyFlwDir."""
 
-"""hydrological methods powered by pyFlwDir"""
-
-import warnings
 import logging
-import numpy as np
-import xarray as xr
+import warnings
+from typing import Optional, Tuple, Union
+
 import geopandas as gpd
+import numpy as np
 import pyflwdir
-from typing import Tuple, Union, Optional
+import xarray as xr
+
 from . import gis_utils
 
 logger = logging.getLogger(__name__)
 
 __all__ = [
     "flwdir_from_da",
     "d8_from_dem",
@@ -32,28 +31,33 @@
 def flwdir_from_da(
     da: xr.DataArray,
     ftype: str = "infer",
     check_ftype: bool = True,
     mask: Union[xr.DataArray, bool, None] = None,
     logger=logger,
 ):
-    """Parse dataarray to flow direction raster object. If a mask coordinate is present
-    this will be passed on the the pyflwdir.from_array method.
+    """Parse dataarray to flow direction raster object.
+
+    If a mask coordinate is present this will be passed
+    on the the pyflwdir.from_array method.
 
     Parameters
     ----------
     da : xarray.DataArray
         DataArray containing flow direction raster
     ftype : {'d8', 'ldd', 'nextxy', 'nextidx', 'infer'}, optional
         name of flow direction type, infer from data if 'infer', by default is 'infer'
     check_ftype : bool, optional
         check if valid flow direction raster if ftype is not 'infer', by default True
     mask : xr.DataArray, bool, optional
         Mask for gridded flow direction data, by default None.
         If True, use the mask coordinate of `da`.
+    logger : logger object, optional
+        The logger object used for logging messages. If not provided, the default
+        logger will be used.
 
     Returns
     -------
     flwdir : pyflwdir.FlwdirRaster
         Flow direction raster object
     """
     if not isinstance(da, xr.DataArray):
@@ -89,17 +93,18 @@
     max_depth: float = -1.0,
     outlets: str = "edge",
     idxs_pit: Optional[np.ndarray] = None,
     **kwargs,
 ) -> xr.DataArray:
     """Derive D8 flow directions grid from an elevation grid.
 
-    Outlets occur at the edge of valid data or at user defined cells (if `idxs_pit` is provided).
-    A local depressions is filled based on its lowest pour point level if the pour point
-    depth is smaller than the maximum pour point depth `max_depth`, otherwise the lowest
+    Outlets occur at the edge of valid data or at user defined cells
+    (if `idxs_pit` is provided). A local depressions is filled based on its
+    lowest pour point level if the pour point depth is smaller than the
+    maximum pour point depth `max_depth`, otherwise the lowest
     elevation in the depression becomes a pit.
 
     Parameters
     ----------
     da_elv: 2D xarray.DataArray
         elevation raster
     gdf_stream: geopandas.GeoDataArray, optional
@@ -110,28 +115,32 @@
         depth are set as pit. A negative value (default) equals an infinitely
         large pour point depth causing all depressions to be filled.
     outlets: {'edge', 'min'}
         Position for basin outlet(s) at the all valid elevation edge cell ('edge')
         or only the minimum elevation edge cell ('min')
     idxs_pit: 1D array of int
         Linear indices of outlet cells.
+    **kwargs:
+        Additional keyword arguments that are passed to the `fill_depressions`
+        function.
 
     Returns
     -------
     da_flw: xarray.DataArray
         D8 flow direction grid
 
     See Also
     --------
     pyflwdir.dem.fill_depressions
     """
     nodata = da_elv.raster.nodata
     crs = da_elv.raster.crs
     assert da_elv.raster.res[1] < 0
-    assert nodata is not None and ~np.isnan(nodata)
+    assert nodata is not None
+    assert ~np.isnan(nodata)
     # burn in river if
     if gdf_stream is not None and "uparea" in gdf_stream.columns:
         gdf_stream = gdf_stream.sort_values(by="uparea")
         dst_rivupa = da_elv.raster.rasterize(gdf_stream, col_name="uparea", nodata=0)
         # make sure the rivers have a slope and are below all other elevation cells.
         # river elevation = min(elv) - log10(uparea[m2]) from rasterized river uparea.
         elvmin = da_elv.where(da_elv != nodata).min()
@@ -183,14 +192,20 @@
         Size of upscaled (coarse) grid cells.
     uparea_name : str, optional
         Name of upstream area DataArray, by default None and derived on the fly.
     flwdir_name : str, optional
         Name of upscaled flow direction raster DataArray, by default "flwdir"
     method : {'com2', 'com', 'eam', 'dmm'}
         Upscaling method for flow direction data, by default 'com2'.
+    logger : logger object, optional
+        The logger object used for logging messages. If not provided, the default
+        logger will be used.
+    **kwargs:
+        Additional keyword arguments that are passed to the `flwdir.upscale`
+        function.
 
     Returns
     -------
     da_flwdir = xarray.DataArray
         Upscaled D8 flow direction grid.
     flwdir_out : pyflwdir.FlwdirRaster
         Upscaled pyflwdir flow direction raster object.
@@ -256,16 +271,17 @@
     flwdir_name: str = "flwdir",
     logger=logger,
     **kwargs,
 ) -> xr.Dataset:
     """Reproject flow direction and upstream area data to the `da_elv` crs and grid.
 
     Flow directions are derived from a reprojected grid of synthetic elevation,
-    based on the log10 upstream area [m2]. For regions without upstream area, the original
-    elevation is used assuming these elevation values are <= 0 (i.e. offshore bathymetry).
+    based on the log10 upstream area [m2]. For regions without upstream area,
+    the original elevation is used assuming these elevation values are <= 0
+    (i.e. offshore bathymetry).
 
     The upstream area on the reprojected grid is based on the new flow directions and
     rivers entering the domain, defined by the minimum upstream area `river_upa` [km2]
     and a distance from river outlets `river_len` [m]. The latter is to avoid setting
     boundary conditions at the downstream end / outflow of a river.
 
     NOTE: the resolution of `ds_hydro` should be similar or smaller than the resolution
@@ -278,20 +294,24 @@
         Dataset with gridded flow directions named `flwdir_name` and upstream area
         named `uparea_name` [km2].
     da_elv: xarray.DataArray
         DataArray with elevation on destination grid.
     river_upa: float, optional
         Minimum upstream area threshold [km2] for inflowing rivers, by default 5 km2
     river_len: float, optional
-        Mimimum distance from river outlet for inflowing river location, by default 1000 m.
+        Mimimum distance from river outlet for inflowing river location,
+        by default 1000 m.
     uparea_name, flwdir_name : str, optional
         Name of upstream area (default "uparea") and flow direction ("flwdir") variables
         in `ds_hydro`.
     kwargs: key-word arguments
         key-word arguments are passed to `d8_from_dem`
+    logger : logger object, optional
+        The logger object used for logging messages. If not provided, the default
+        logger will be used.
 
     Returns
     -------
     xarray.Dataset
         Reprojected gridded dataset with flow direction and upstream area variables.
 
     See Also
@@ -315,45 +335,48 @@
     # take minimum with rank to ensure pits of main rivers have zero syn. elevation
     if np.any(rivmask):
         flwdir_src = flwdir_from_da(ds_hydro[flwdir_name], mask=rivmask)
         elvsyn = np.minimum(flwdir_src.rank, elvsyn).where(flwdir_src.rank == 0, elvsyn)
     # reproject with 'min' to preserve rivers
     elv_mask = da_elv != da_elv.raster.nodata
     elvsyn_reproj = elvsyn.raster.reproject_like(da_elv, method="min")
-    # in regions without uparea use elevation, assuming the elevation < 0 (i.e. offshore bathymetry)
+    # in regions without uparea use elevation, assuming the elevation < 0
+    # (i.e. offshore bathymetry)
     elvsyn_reproj = elvsyn_reproj.where(
         np.logical_or(elvsyn_reproj != nodata, ~elv_mask),
         da_elv - da_elv.where(elvsyn_reproj == nodata).max() - 0.1,  # make sure < 0
     )
     elvsyn_reproj = elvsyn_reproj.where(da_elv != da_elv.raster.nodata, nodata)
     elvsyn_reproj.raster.set_crs(crs)
     elvsyn_reproj.raster.set_nodata(nodata)
     # get flow directions based on reprojected synthetic elevation
-    logger.info(f"Deriving flow direction from reprojected synthethic elevation.")
+    logger.info("Deriving flow direction from reprojected synthethic elevation.")
     da_flw1 = d8_from_dem(elvsyn_reproj, **kwargs)
     flwdir = flwdir_from_da(da_flw1, ftype="d8", mask=elv_mask)
     # find source river cells outside destination grid bbox
     outside_dst = da_upa.raster.geometry_mask(da_elv.raster.box, invert=True)
     area = flwdir.area / 1e6  # area [km2]
-    # If any river cell outside the destination grid, vectorize and reproject river segments(!) uparea
+    # If any river cell outside the destination grid, vectorize and reproject river
+    # segments(!) uparea
     # to set as boundary condition to the upstream area map.
     nriv = 0
     if np.any(np.logical_and(rivmask, outside_dst)):
         feats = flwdir_src.streams(uparea=da_upa.values, mask=rivmask)
         gdf_stream = gpd.GeoDataFrame.from_features(feats, crs=ds_hydro.raster.crs)
         gdf_stream = gdf_stream.sort_values(by="uparea")
         # calculate upstream area with uparea from inflowing rivers at edge
         # get edge river cells indices
         rivupa = da_flw1.raster.rasterize(gdf_stream, col_name="uparea", nodata=0)
         rivmsk = np.logical_and(flwdir.distnc > river_len, rivupa > 0).values
         _edge = pyflwdir.gis_utils.get_edge(elv_mask.values)
         inflow_idxs = np.where(np.logical_and(rivmsk, _edge).ravel())[0]
         if inflow_idxs.size > 0:
             # map nearest segment to each river edge cell;
-            # keep cell which longest distance to outlet per river segment to avoid duplicating uparea
+            # keep cell which longest distance to outlet per river segment to
+            # avoid duplicating uparea
             gdf0 = gpd.GeoDataFrame(
                 index=inflow_idxs,
                 geometry=gpd.points_from_xy(*flwdir.xy(inflow_idxs)),
                 crs=crs,
             )
             gdf0["distnc"] = flwdir.distnc.flat[inflow_idxs]
             gdf0["idx2"], gdf0["dst2"] = gis_utils.nearest(gdf0, gdf_stream)
@@ -387,15 +410,18 @@
     idxs: Optional[np.ndarray] = None,
     xy: Optional[Tuple] = None,
     ids: Optional[np.ndarray] = None,
     mask: Optional[xr.DataArray] = None,
     flwdir: Optional[pyflwdir.FlwdirRaster] = None,
     logger=logger,
 ) -> xr.DataArray:
-    """This method is deprecated. See :py:meth:`~hydromt.flw.gauge_map`"""
+    """Return map with unique gauge IDs.
+
+    This method is deprecated. See :py:meth:`~hydromt.flw.gauge_map`.
+    """
     warnings.warn(
         'The "gaugemap" method is deprecated, use  "hydromt.flw.gauge_map" instead.',
         DeprecationWarning,
     )
     return gauge_map(
         ds=ds,
         idxs=idxs,
@@ -441,14 +467,17 @@
     flwdir : pyflwdir.FlwdirRaster, optional
         Flow direction raster object, by default None.
     stream: 2D array of bool, optional
         Mask of stream cells used to snap gauges to, by default None
     max_dist: float, optional
         Maximum distance between original and snapped point location.
         A warning is logged if exceeded. By default 10 km.
+    logger : logger object, optional
+        The logger object used for logging messages. If not provided, the default
+        logger will be used.
 
     Returns
     -------
     da_gauges: xarray.DataArray
         Map with unique gauge IDs
     idxs: 1D array or int
         linear indices of gauges
@@ -480,15 +509,15 @@
         data=gauges,
         attrs=dict(_FillValue=0),
     )
     return da_gauges, idxs, ids
 
 
 def outlet_map(da_flw: xr.DataArray, ftype: str = "infer") -> xr.DataArray:
-    """Returns a mask of basin outlets/pits from a flow direction raster.
+    """Return a mask of basin outlets/pits from a flow direction raster.
 
     Parameters
     ----------
     da_flw: xr.DataArray
         Flow direction data array
     ftype : {'d8', 'ldd', 'nextxy', 'nextidx', 'infer'}, optional
         name of flow direction type, infer from data if 'infer', by default is 'infer'
@@ -504,15 +533,15 @@
         raise ValueError(f"Unknown pyflwdir ftype: {ftype}")
     pit_values = pyflwdir.pyflwdir.FTYPES[ftype]._pv
     mask = np.isin(da_flw.values, pit_values)
     return xr.DataArray(mask, dims=da_flw.raster.dims, coords=da_flw.raster.coords)
 
 
 def stream_map(ds, stream=None, **stream_kwargs):
-    """Return a stream mask DataArray
+    """Return a stream mask DataArray.
 
     Parameters
     ----------
     ds : xarray.Dataset
         dataset containing all maps for stream criteria
     stream: 2D array of bool, optional
         Initial mask of stream cells. If a stream if provided, it is combined with the
@@ -551,15 +580,16 @@
     **stream_kwargs,
 ) -> Union[xr.DataArray, Tuple]:
     """Return a (sub)basin map, with unique non-zero IDs for each subbasin.
 
     Parameters
     ----------
     ds : xarray.Dataset
-        Dataset used for output grid definition and containing `stream_kwargs` variables.
+        Dataset used for output grid definition and containing `stream_kwargs`
+        variables.
     flwdir : pyflwdir.FlwdirRaster
         Flow direction raster object
     idxs : 1D array or int, optional
         linear indices of sub(basin) outlets, by default is None.
     xy : tuple of 1D array of float, optional
         x, y coordinates of sub(basin) outlets, by default is None.
     outlets : bool, optional
@@ -617,15 +647,17 @@
 def basin_shape(
     ds: xr.Dataset,
     flwdir: pyflwdir.FlwdirRaster,
     basin_name: str = "basins",
     mask: bool = True,
     **kwargs,
 ) -> gpd.GeoDataFrame:
-    """This method is be deprecated. Use :py:meth:`~hydromt.flw.basin_map` in combination
+    """Generate basins from a given dataset and flow direction raster.
+
+    This method is be deprecated. Use :py:meth:`~hydromt.flw.basin_map` in combination
     with :py:meth:`~hydromt.raster.RasterDataArray.vectorize` instead.
     """
     warnings.warn(
         "basin_shape is deprecated, use a combination of hydromt.flw.basin_map"
         " and hydromt.raster.RasterDataArray.vectorize instead.",
         DeprecationWarning,
     )
@@ -695,15 +727,15 @@
     da_flwdir: xr.DataArray,
     da_rivmsk: Optional[xr.DataArray] = None,
     flwdir: Optional[pyflwdir.FlwdirRaster] = None,
     connectivity: int = 4,
     river_d8: bool = False,
     logger=logger,
 ) -> xr.DataArray:
-    """Returns hydrologically conditioned elevation.
+    """Return hydrologically conditioned elevation.
 
     The elevation is conditioned to D4 (`connectivity=4`) or D8 (`connectivity=8`)
     flow directions based on the algorithm described in Yamazaki et al. [1]_
 
     The method assumes the original flow directions are in D8. Therefore, if
     `connectivity=4`, an intermediate D4 conditioned elevation raster is derived
     first, based on which new D4 flow directions are obtained used to condition the
@@ -712,29 +744,35 @@
     Parameters
     ----------
     da_elevtn, da_flwdir, da_rivmsk : xr.DataArray
         elevation [m+REF]
         D8 flow directions [-]
         binary river mask [-], optional
     flwdir : pyflwdir.FlwdirRaster, optional
-        D8 flow direction raster object. If None it is derived on the fly from `da_flwdir`.
+        D8 flow direction raster object. If None it is derived on the fly
+        from `da_flwdir`.
     connectivity: {4, 8}
         D4 or D8 flow connectivity.
     river_d8 : bool
         If True and `connectivity==4`, additionally condition river cells to D8.
         Requires `da_rivmsk`.
+    logger : logger object, optional
+        The logger object used for logging messages. If not provided, the default
+        logger will be used.
 
     Returns
     -------
     xr.Dataset
         Dataset with hydrologically adjusted elevation ('elevtn') [m+REF]
 
     References
     ----------
-    .. [1] Yamazaki et al. (2012). Adjustment of a spaceborne DEM for use in floodplain hydrodynamic modeling. Journal of Hydrology, 436-437, 81–91. https://doi.org/10.1016/j.jhydrol.2012.02.045
+    .. [1] Yamazaki et al. (2012). Adjustment of a spaceborne DEM for use in floodplain
+        hydrodynamic modeling. Journal of Hydrology, 436-437, 81-91.
+        https://doi.org/10.1016/j.jhydrol.2012.02.045
 
 
     See Also
     --------
     pyflwdir.FlwdirRaster.dem_adjust
     pyflwdir.FlwdirRaster.dem_dig_d4
     """
@@ -764,15 +802,14 @@
             d4, ftype="d8", transform=flwdir.transform, latlon=flwdir.latlon
         )
         elevtn = flwdir_d4.dem_adjust(elevtn)
         # condition river cells to D8
         if river_d8:
             flwdir_river = flwdir_from_da(da_flwdir, mask=rivmsk)
             elevtn = flwdir_river.dem_adjust(elevtn)
-        # assert np.all((elv2 - flwdir_d4.downstream(elv2))>=0)
 
     # save to dataarray
     da_out = xr.DataArray(
         data=elevtn,
         coords=da_elevtn.raster.coords,
         dims=da_elevtn.raster.dims,
     )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hydromt-0.7.1/hydromt/gis_utils.py` & `hydromt-0.8.0/hydromt/gis_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-"""gis related convience functions. More in pyflwdir.gis_utils"""
-from os.path import dirname, join, isfile
-import os
+"""GIS related convenience functions."""
 import glob
-import sys
+import logging
+import os
 import subprocess
+from os.path import dirname, isfile, join
+from typing import Optional, Tuple
+
+import geopandas as gpd
 import numpy as np
-import xarray as xr
 import rasterio
+import xarray as xr
+from pyflwdir import core_conversion, core_d8, core_ldd
+from pyflwdir import gis_utils as gis
 from pyproj import CRS
 from rasterio.transform import Affine
-import geopandas as gpd
-from shapely.geometry.base import BaseGeometry
 from shapely.geometry import box
-import logging
-from pyflwdir import core_conversion, core_d8, core_ldd
-from pyflwdir import gis_utils as gis
-from typing import Optional, Tuple
-from . import _compat
+from shapely.geometry.base import BaseGeometry
 
+from . import _compat
 
 __all__ = ["spread2d", "nearest", "nearest_merge"]
 
 logger = logging.getLogger(__name__)
 
 _R = 6371e3  # Radius of earth in m. Use 3956e3 for miles
 XATTRS = {
@@ -105,29 +105,35 @@
     gdf2: gpd.GeoDataFrame,
     columns: Optional[list] = None,
     max_dist: Optional[float] = None,
     overwrite: bool = False,
     inplace: bool = False,
     logger=logger,
 ) -> gpd.GeoDataFrame:
-    """Merge attributes of gdf2 with the nearest feature of gdf1, optionally bounded by
-    a maximumum distance `max_dist`. Unless `overwrite = True`, gdf2 values are only
+    """Merge attributes of gdf2 with the nearest feature of gdf1.
+
+    Output is optionally bounded by a maximumum distance `max_dist`.
+    Unless `overwrite = True`, gdf2 values are only
     merged where gdf1 has missing values.
 
     Parameters
     ----------
     gdf1, gdf2: geopandas.GeoDataFrame
         Source `gdf1` and destination `gdf2` geometries.
     columns : list of str, optional
         Names of columns in `gdf2` to merge, by default None
     max_dist : float, optional
         Maximum distance threshold for merge, by default None, i.e.: no threshold.
     overwrite : bool, optional
         If False (default) gdf2 values are only merged where gdf1 has missing values,
         i.e. NaN values for existing columns or missing columns.
+    inplace : bool,
+        If True, apply the merge to gdf1, otherwise return a new object.
+    logger:
+        The logger to use.
 
     Returns
     -------
     gpd.GeoDataFrame
         Merged GeoDataFrames
     """
     idx_nn, dst = nearest(gdf1, gdf2)
@@ -152,18 +158,19 @@
         gdf1.loc[valid, col] = new_vals
     return gdf1
 
 
 def nearest(
     gdf1: gpd.GeoDataFrame, gdf2: gpd.GeoDataFrame
 ) -> Tuple[np.ndarray, np.ndarray]:
-    """Return the index of and distance [m] to the nearest geometry
-    in `gdf2` for each geometry of `gdf1`. For Line geometries in `gdf1` the nearest
-    geometry is based line center point and for polygons on its representative point.
-    Mixed geometry types are not yet supported.
+    """Return the index of and distance [m] to the nearest geometry.
+
+    For Line geometries in `gdf1` the nearest geometry is based line center point
+    and for polygons on its representative point. Mixed geometry types are not
+    yet supported.
 
     Note: Since geopandas v0.10.0 it contains a sjoin_nearest method which is very
     similar and should.
 
 
     Parameters
     ----------
@@ -224,15 +231,15 @@
         geom = geom.unary_union
     idx = gdf.sindex.query(geom, predicate=predicate)
     return idx
 
 
 # REPROJ
 def utm_crs(bbox):
-    """Returns wkt string of nearest UTM projects
+    """Return wkt string of nearest UTM projects.
 
     Parameters
     ----------
     bbox : array-like of floats
         (xmin, ymin, xmax, ymax) bounding box in latlon WGS84 (EPSG:4326) coordinates
 
     Returns
@@ -260,16 +267,15 @@
             raise ValueError('CRS "utm" requires bbox')
     else:
         crs = CRS.from_user_input(crs)
     return crs
 
 
 def axes_attrs(crs):
-    """
-    Provide CF-compliant variable names and metadata for axes
+    """Provide CF-compliant variable names and metadata for axes.
 
     Parameters
     ----------
     crs: pyproj.CRS
         coordinate reference system
 
     Returns
@@ -285,15 +291,15 @@
     x_dim = XATTRS[crs_type]["short_name"]
     y_attrs = YATTRS[crs_type]
     x_attrs = XATTRS[crs_type]
     return x_dim, y_dim, x_attrs, y_attrs
 
 
 def meridian_offset(ds, x_name="x", bbox=None):
-    """re-arange data along x dim"""
+    """re-arrange data along x dim."""
     if ds.raster.crs is None or ds.raster.crs.is_projected:
         raise ValueError("The method is only applicable to geographic CRS")
     lons = np.copy(ds[x_name].values)
     w, e = lons.min(), lons.max()
     if bbox is not None and bbox[0] < w and bbox[0] < -180:  # 180W - 180E > 360W - 0W
         lons = np.where(lons > 0, lons - 360, lons)
     elif bbox is not None and bbox[2] > e and bbox[2] > 180:  # 180W - 180E > 0E-360E
@@ -307,15 +313,15 @@
     return ds.sortby(x_name)
 
 
 # TRANSFORM
 
 
 def affine_to_coords(transform, shape, x_dim="x", y_dim="y"):
-    """Returns a raster axis with pixel center coordinates based on the transform.
+    """Return a raster axis with pixel center coordinates based on the transform.
 
     Parameters
     ----------
     transform : affine transform
         Two dimensional affine transform for 2D linear mapping
     shape : tuple of int
         The height, width  of the raster.
@@ -346,15 +352,15 @@
             "yc": ((y_dim, x_dim), y_coords),
             "xc": ((y_dim, x_dim), x_coords),
         }
     return coords
 
 
 def affine_to_meshgrid(transform, shape):
-    """Returns a mesgrid of pixel center coordinates based on the transform.
+    """Return a meshgrid of pixel center coordinates based on the transform.
 
     Parameters
     ----------
     transform : affine transform
         Two dimensional affine transform for 2D linear mapping
     shape : tuple of int
         The height, width  of the raster.
@@ -373,34 +379,37 @@
         * np.meshgrid(np.arange(width), np.arange(height))
     )
     return x_coords, y_coords
 
 
 ## CELLAREAS
 def reggrid_area(lats, lons):
-    """Returns the cell area [m2] for a regular grid based on its cell centres
-    lat, lon coordinates."""
+    """Return the cell area [m2] for a regular grid based on its cell centres lat, lon."""  # noqa: E501
     xres = np.abs(np.mean(np.diff(lons)))
     yres = np.abs(np.mean(np.diff(lats)))
     area = np.ones((lats.size, lons.size), dtype=lats.dtype)
     return cellarea(lats, xres, yres)[:, None] * area
 
 
 def cellarea(lat, xres=1.0, yres=1.0):
-    """Return the area [m2] of cell based on the cell center latitude and its resolution
-    in measured in degrees."""
+    """Return the area [m2] of cell based on its center latitude and resolution in degrees.
+
+    Resolution is in measured degrees.
+    """  # noqa: E501
     l1 = np.radians(lat - np.abs(yres) / 2.0)
     l2 = np.radians(lat + np.abs(yres) / 2.0)
     dx = np.radians(np.abs(xres))
     return _R**2 * dx * (np.sin(l2) - np.sin(l1))
 
 
 def cellres(lat, xres=1.0, yres=1.0):
-    """Return the cell (x, y) resolution [m] based on cell center latitude and its
-    resolution measured in degrees."""
+    """Return the cell (x, y) resolution [m].
+
+    Based on cell center latitude and its resolution measured in degrees.
+    """
     m1 = 111132.92  # latitude calculation term 1
     m2 = -559.82  # latitude calculation term 2
     m3 = 1.175  # latitude calculation term 3
     m4 = -0.0023  # latitude calculation term 4
     p1 = 111412.84  # longitude calculation term 1
     p2 = -93.5  # longitude calculation term 2
     p3 = 0.118  # longitude calculation term 3
@@ -427,16 +436,17 @@
 
 def spread2d(
     da_obs: xr.DataArray,
     da_mask: Optional[xr.DataArray] = None,
     da_friction: Optional[xr.DataArray] = None,
     nodata: Optional[float] = None,
 ) -> xr.Dataset:
-    """Returns values of `da_obs` spreaded to cells with `nodata` value within `da_mask`,
-    powered by :py:meth:`pyflwdir.gis_utils.spread2d`
+    """Return values of `da_obs` spreaded to cells with `nodata` value within `da_mask`.
+
+    powered by :py:meth:`pyflwdir.gis_utils.spread2d`.
 
     Parameters
     ----------
     da_obs : xarray.DataArray
         Input raster with observation values and background/nodata values which are
         filled by the spreading algorithm.
     da_mask :  xarray.DataArray, optional
@@ -447,16 +457,16 @@
     nodata : float, optional
         Nodata or background value. Must be finite numeric value. If not given the
         raster nodata value is used.
 
     Returns
     -------
     ds_out: xarray.Dataset
-        Dataset with spreaded source values, linear index of the source cell "source_idx"
-        and friction distance to the source cell "source_dst".
+        Dataset with spreaded source values, linear index of the source cell
+        "source_idx" and friction distance to the source cell "source_dst".
     """
     nodata = da_obs.raster.nodata if nodata is None else nodata
     if nodata is None or np.isnan(nodata):
         raise ValueError(f'"nodata" must be a finite value, not {nodata}')
     msk, frc = None, None
     if da_mask is not None:
         assert da_obs.raster.identical_grid(da_mask)
@@ -488,33 +498,32 @@
     return ds_out
 
 
 ## PCRASTER
 
 
 def write_clone(tmpdir, gdal_transform, wkt_projection, shape):
-    """write pcraster clone file to a tmpdir using gdal"""
+    """Write pcraster clone file to a tmpdir using gdal."""
     from osgeo import gdal
 
     gdal.AllRegister()
     driver1 = gdal.GetDriverByName("GTiff")
     driver2 = gdal.GetDriverByName("PCRaster")
     fn = join(tmpdir, "clone.map")
     # create temp tif file
     fn_temp = join(tmpdir, "clone.tif")
     TempDataset = driver1.Create(fn_temp, shape[1], shape[0], 1, gdal.GDT_Float32)
     TempDataset.SetGeoTransform(gdal_transform)
     if wkt_projection is not None:
         TempDataset.SetProjection(wkt_projection)
     # TODO set csr
     # copy to pcraster format
-    outDataset = driver2.CreateCopy(fn, TempDataset, 0)
+    driver2.CreateCopy(fn, TempDataset, 0)
     # close and cleanup
     TempDataset = None
-    outDataset = None
     return fn
 
 
 def write_map(
     data,
     raster_path,
     nodata,
@@ -539,25 +548,31 @@
         no data value
     transform : affine transform
         Two dimensional affine transform for 2D linear mapping
     clone_path : str, optional
         Path to PCRaster clone map, by default None
     pcr_vs : str, optional
         pcraster type, by default "scalar"
+    **kwargs:
+        not used in this function, mainly here for compatability reasons.
+    crs:
+        The coordinate reference system of the data.
+
 
     Raises
     ------
     ImportError
         pcraster package is required
     ValueError
         if invalid ldd
     """
     if not _compat.HAS_PCRASTER:
         raise ImportError("The pcraster package is required to write map files")
     import tempfile
+
     import pcraster as pcr
 
     with tempfile.TemporaryDirectory() as tmpdir:
         # deal with pcr clone map
         if clone_path is None:
             clone_path = write_clone(
                 tmpdir,
@@ -580,15 +595,15 @@
                 raise ValueError("LDD data not understood")
             mv = int(core_ldd._mv)
             ldd = pcr.numpy2pcr(pcr.Ldd, data.astype(int), mv)
             # make sure it is pcr sound
             # NOTE this should not be necessary
             pcrmap = pcr.lddrepair(ldd)
         elif pcr_vs == "bool":
-            pcrmap = pcr.numpy2pcr(pcr.Boolean, data.astype(np.bool), np.bool(nodata))
+            pcrmap = pcr.numpy2pcr(pcr.Boolean, data.astype(bool), np.bool_(nodata))
         elif pcr_vs == "scalar":
             pcrmap = pcr.numpy2pcr(pcr.Scalar, data.astype(float), float(nodata))
         elif pcr_vs == "ordinal":
             pcrmap = pcr.numpy2pcr(pcr.Ordinal, data.astype(int), int(nodata))
         elif pcr_vs == "nominal":
             pcrmap = pcr.numpy2pcr(pcr.Nominal, data.astype(int), int(nodata))
         pcr.report(pcrmap, raster_path)
@@ -599,18 +614,19 @@
 
 
 def create_vrt(
     vrt_path: str,
     file_list_path: str = None,
     files_path: str = None,
 ):
-    """Creates a .vrt file from a list op raster datasets by either
-    passing the list directly (file_list_path) or by inferring it by passing
+    r"""Create a .vrt file from a list op raster datasets.
+
+    Either passing the list directly (file_list_path) or by inferring it by passing
     a path containing wildcards (files_path) of the location(s) of the
-    raster datasets
+    raster datasets.
 
     Parameters
     ----------
     vrt_path : str
         Path of the output vrt
     file_list_path : str, optional
         Path to the text file containing the paths to the raster files
@@ -620,15 +636,14 @@
         e.g. c:\\temp\\*\\*.tif for all tif files in subfolders of 'c:\temp'
 
     Raises
     ------
     ValueError
         A Path is needed, either file_list_path or files_path
     """
-
     if file_list_path is None and files_path is None:
         raise ValueError(
             "Either 'file_list_path' or 'files_path' is required -> None was given"
         )
 
     outdir = dirname(vrt_path)
     if not os.path.isdir(outdir):
```

### Comparing `hydromt-0.7.1/hydromt/io.py` & `hydromt-0.8.0/hydromt/io.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from os.path import isfile, basename, abspath, join, dirname
+"""Implementations for all of the necessary IO for HydroMT."""
+import glob
 import io
+import logging
+from os.path import abspath, basename, dirname, isfile, join
 from pathlib import Path
-import glob
-from fsspec.implementations import local
-import pandas as pd
-import numpy as np
+
+import dask
 import geopandas as gpd
+import numpy as np
+import pandas as pd
+import pyproj
 import xarray as xr
-import dask
-from shapely.geometry.base import GEOMETRY_TYPES
 from shapely.geometry import box
-import pyproj
-import logging
+from shapely.geometry.base import GEOMETRY_TYPES
 
-from . import raster, vector, gis_utils, merge
+from . import gis_utils, merge, raster, vector
 
 logger = logging.getLogger(__name__)
 
 __all__ = [
     "open_raster",
     "open_mfraster",
     "open_raster_from_tindex",
@@ -28,32 +29,36 @@
     "write_xy",
 ]
 
 
 def open_raster(
     filename, mask_nodata=False, chunks={}, nodata=None, logger=logger, **kwargs
 ):
-    """Open a gdal-readable file with rasterio based on
+    """Open a gdal-readable file with rasterio based on.
+
     :py:meth:`rioxarray.open_rasterio`, but return squeezed DataArray.
 
     Arguments
-    ----------
+    ---------
     filename : str, path, file-like, rasterio.DatasetReader, or rasterio.WarpedVRT
         Path to the file to open. Or already open rasterio dataset.
     mask_nodata : bool, optional
         set nodata values to np.nan (xarray default nodata value)
     nodata: int, float, optional
         Set nodata value if missing
     chunks : int, tuple or dict, optional
         Chunk sizes along each dimension, e.g., ``5``, ``(5, 5)`` or
         ``{'x': 5, 'y': 5}``. If chunks is provided, it used to load the new
         DataArray into a dask array.
-    **kwargs
+    **kwargs:
         key-word arguments are passed to :py:meth:`xarray.open_dataset` with
         "rasterio" engine.
+    logger : logger object, optional
+        The logger object used for logging messages. If not provided, the default
+        logger will be used.
 
     Returns
     -------
     data : DataArray
         DataArray
     """
     kwargs.update(
@@ -87,29 +92,28 @@
 def open_mfraster(
     paths,
     chunks={},
     concat=False,
     concat_dim="dim0",
     mosaic=False,
     mosaic_kwargs={},
-    logger=logger,
     **kwargs,
 ):
     """Open multiple gdal-readable files as single Dataset with geospatial attributes.
 
     Each raster is turned into a DataArray with its name inferred from the filename.
     By default all DataArray are assumed to be on an identical grid and the output
     dataset is a merge of the rasters.
     If ``concat`` the DataArrays are concatenated along ``concat_dim`` returning a
     Dataset with a single 3D DataArray.
     If ``mosaic`` the DataArrays are concatenated along the the spatial dimensions
     using :py:meth:`~hydromt.raster.merge`.
 
     Arguments
-    ----------
+    ---------
     paths: str, list of str/Path/file-like
         Paths to the rasterio/gdal files.
         Paths can be provided as list of paths or a path pattern string which is
         interpreted according to the rules used by the Unix shell. The variable name
         is derived from the basename minus extension in case a list of paths:
         ``<name>.<extension>`` and based on the file basename minus pre-, postfix and
         extension in a path pattern: ``<prefix><*name><postfix>.<extension>``
@@ -128,15 +132,15 @@
         Dimension name of concatenate index, by default 'dim0'
     mosaic: bool, optional
         If True create mosaic of several rasters. The variable is named based on
         variable name infered from the first raster.
     mosaic_kwargs: dict, optional
         Mosaic key_word arguments to unify raster crs and/or resolution. See
         :py:meth:`hydromt.merge.merge` for options.
-    **kwargs
+    **kwargs:
         key-word arguments are passed to :py:meth:`hydromt.raster.open_raster`
 
     Returns
     -------
     data : DataSet
         The newly created DataSet.
     """
@@ -185,15 +189,15 @@
         fn_attrs.append(bname)
         da.name = vname
 
         if i > 0:
             if not mosaic:
                 # check if transform, shape and crs are close
                 if not da_lst[0].raster.identical_grid(da):
-                    raise xr.MergeError(f"Geotransform and/or shape do not match")
+                    raise xr.MergeError("Geotransform and/or shape do not match")
                 # copy coordinates from first raster
                 da[da.raster.x_dim] = da_lst[0][da.raster.x_dim]
                 da[da.raster.y_dim] = da_lst[0][da.raster.y_dim]
             if concat or mosaic:
                 # copy name from first raster
                 da.name = da_lst[0].name
         da_lst.append(da)
@@ -208,46 +212,48 @@
         else:
             da = merge.merge(da_lst, **mosaic_kwargs)  # spatial merge
             da.attrs.update({"source_file": "; ".join(fn_attrs)})
         ds = da.to_dataset()  # dataset for consistency
     else:
         ds = xr.merge(
             da_lst
-        )  # , combine_attrs="drop") seems that with rioxarray drops all datarrays atrributes not just ds
+        )  # seems that with rioxarray drops all datarrays atrributes not just ds
         ds.attrs = {}
 
     # update spatial attributes
     if da_lst[0].rio.crs is not None:
         ds.rio.write_crs(da_lst[0].rio.crs, inplace=True)
     ds.rio.write_transform(inplace=True)
     return ds
 
 
 def open_raster_from_tindex(
     fn_tindex, bbox=None, geom=None, tileindex="location", mosaic_kwargs={}, **kwargs
 ):
-    """Reads and merges raster tiles (potentially in different CRS) based on a
+    """Read and merge raster tiles.
+
+    Raster tiles can potentially be in different CRS. Based on a
     tile index file as generated with `gdaltindex`. A bbox or geom describing the
     output area of interest is required.
 
     Arguments
     ---------
-    fn: path, str
+    fn_tindex: path, str
         Path to tile index file.
     bbox : tuple of floats, optional
         (xmin, ymin, xmax, ymax) bounding box in EPGS:4326, by default None.
     geom : geopandas.GeoDataFrame/Series, optional
         A geometry defining the area of interest, by default None. The geom.crs
         defaults to EPSG:4326 if not set.
     tileindex: str
         Field name to hold the file path/location to the indexed rasters
     mosaic_kwargs: dict, optional
         Mosaic key_word arguments to unify raster crs and/or resolution. See
         :py:meth:`~hydromt.merge.merge()` for options.
-    **kwargs
+    **kwargs:
         key-word arguments are passed to :py:meth:`hydromt.io.open_mfraster()`
 
 
     Returns
     -------
     data : Dataset
         A single-variable Dataset of merged raster tiles.
@@ -309,20 +315,27 @@
         Name of the variable in case of a csv fn_data file. By default, None and
         infered from basename.
     crs: str, `pyproj.CRS`, or dict
         Source coordinate reference system, ignored for files with a native crs.
     bbox : array of float, default None
         Filter features by given bounding box described by [xmin, ymin, xmax, ymax]
         Cannot be used with geom.
+    index_dim:
+        The dimention to index on.
+    chunks:
+        The dimentions of the chunks to store the underlying data in.
     geom : GeoDataFrame or GeoSeries | shapely Geometry, default None
         Filter for features that intersect with the geom.
         CRS mis-matches are resolved if given a GeoSeries or GeoDataFrame.
         Cannot be used with bbox.
-    **kwargs
-        Key-word arguments passed to :py:func:`geopandas.read_file` to read the point geometry file.
+    **kwargs:
+        Key-word argume
+    logger : logger object, optional
+        The logger object used for logging messages. If not provided, the default
+        logger will be used.
 
     Returns
     -------
     ds: xarray.Dataset
         Dataset with geospatial coordinates.
     """
     if not isfile(fn_locs):
@@ -345,25 +358,32 @@
     return ds.chunk(chunks)
 
 
 def open_timeseries_from_table(
     fn, name=None, index_dim="index", logger=logger, **kwargs
 ):
     """Open timeseries csv file and parse to xarray.DataArray.
-    Accepts files with time index on one dimension and numeric location index on the other dimension.
-    In case of string location indices, non-numeric parts are filtered from the location index.
+
+    Accepts files with time index on one dimension and numeric location index on the
+    other dimension. In case of string location indices, non-numeric parts are
+    filtered from the location index.
 
     Arguments
     ---------
     fn: path, str
         Path to time series file
     name: str
         variable name, derived from basename of fn if None.
+    index_dim:
+        the dimention to index on.
     **kwargs:
         key-word arguments are passed to the reader method
+    logger:
+        The logger to be used. If none probided, the default will be used.
+
 
 
     Returns
     -------
     da: xarray.DataArray
         DataArray
     """
@@ -398,51 +418,54 @@
     geom=None,
     assert_gtype=None,
     predicate="intersects",
     mode="r",
     logger=logger,
     **kwargs,
 ):
-    """Open fiona-compatible geometry, csv, excel or xy file and
-    parse to :py:meth:`geopandas.GeoDataFrame`.
+    """Open fiona-compatible geometry, csv, excel or xy file and parse it.
 
-    CSV or XLS file are converted to point geometries based on default columns names
+    Construct a :py:meth:`geopandas.GeoDataFrame` CSV or XLS file are
+    converted to point geometries based on default columns names
     for the x- and y-coordinates, or if given, the x_dim and y_dim arguments.
 
     Parameters
     ----------
     fn : str
         path to geometry file
     driver: {'csv', 'xls', 'xy', 'vector'}, optional
-        driver used to read the file: :py:meth:`geopandas.open_file` for gdal vector files,
-        :py:meth:`hydromt.io.open_vector_from_table` for csv, xls(x) and xy files.
-        By default None, and infered from file extention.
+        driver used to read the file: :py:meth:`geopandas.open_file` for gdal vector
+        files, :py:meth:`hydromt.io.open_vector_from_table`
+        for csv, xls(x) and xy files. By default None, and infered from file extention.
     crs: str, `pyproj.CRS`, or dict
         Source coordinate reference system, ignored for files with a native crs.
     dst_crs: str, `pyproj.CRS`, or dict
         Destination coordinate reference system.
     bbox : array of float, default None
         Filter features by given bounding box described by [xmin, ymin, xmax, ymax]
         Cannot be used with mask.
     geom : GeoDataFrame or GeoSeries | shapely Geometry, default None
         Filter for features that intersect with the mask.
         CRS mis-matches are resolved if given a GeoSeries or GeoDataFrame.
         Cannot be used with bbox.
-    predicate : {'intersects', 'within', 'contains', 'overlaps', 'crosses', 'touches'}, optional
-        If predicate is provided, the GeoDataFrame is filtered by testing
+    predicate : {'intersects', 'within', 'contains', 'overlaps', 'crosses', 'touches'},
+        optional. If predicate is provided, the GeoDataFrame is filtered by testing
         the predicate function against each item. Requires bbox or mask.
         By default 'intersects'
     x_dim, y_dim : str
         Name of x, y-coordinate columns, only applicable for csv or xls tables
     assert_gtype : {Point, LineString, Polygon}, optional
         If given, assert geometry type
     mode: {'r', 'a', 'w'}
         file opening mode (fiona files only), by default 'r'
     **kwargs:
         Keyword args to be passed to the driver method when opening the file
+    logger : logger object, optional
+        The logger object used for logging messages. If not provided, the default
+        logger will be used.
 
     Returns
     -------
     gdf : geopandas.GeoDataFrame
         Parsed geometry file
     """
     filtered = False
@@ -489,22 +512,28 @@
     """Read point geometry files from csv, xy or excel table files.
 
     Parameters
     ----------
     driver: {'csv', 'xls', 'xlsx', 'xy'}
         If 'csv' use :py:meth:`pandas.read_csv` to read the data;
         If 'xls' or 'xlsx' use :py:meth:`pandas.read_excel` with `engine=openpyxl`
-        If 'xy' use :py:meth:`pandas.read_csv` with `index_col=False`, `header=None`, `delim_whitespace=True`.
+        If 'xy' use :py:meth:`pandas.read_csv` with `index_col=False`, `header=None`,
+        `delim_whitespace=True`.
     x_dim, y_dim: str
         Name of x, y column. By default the x-column header should be one of
-        ['x', 'longitude', 'lon', 'long'], and y-column header one of ['y', 'latitude', 'lat'].
-        For xy files, which don't have a header, the first column is interpreted as x
-        and the second as y column.
+        ['x', 'longitude', 'lon', 'long'], and y-column header one of
+        ['y', 'latitude', 'lat']. For xy files, which don't have a header,
+        the first column is interpreted as x and the second as y column.
     crs: int, dict, or str, optional
-        Coordinate reference system, accepts EPSG codes (int or str), proj (str or dict) or wkt (str)
+        Coordinate reference system, accepts EPSG codes (int or str), proj (str or dict)
+        or wkt (str)
+    fn:
+        The filename to read the table from.
+    **kwargs
+        Additional keyword arguments that are passed to the underlying drivers.
 
     Returns
     -------
     gdf: geopandas.GeoDataFrame
         Parsed and filtered point geometries
     """
     driver = driver.lower() if driver is not None else str(fn).split(".")[-1].lower()
```

### Comparing `hydromt-0.7.1/hydromt/log.py` & `hydromt-0.8.0/hydromt/log.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
+"""Implementations related to logging."""
 
-from functools import wraps
 import logging
 import logging.handlers
-import sys
 import os
-import logging
+import sys
+from functools import wraps
 
-FMT = "%(asctime)s - %(name)s - %(module)s - %(levelname)s - %(message)s"
 from . import __version__
 
+FMT = "%(asctime)s - %(name)s - %(module)s - %(levelname)s - %(message)s"
+
 
 def setuplog(
     name: str = "hydromt",
     path: str = None,
     log_level: int = 20,
     fmt: str = FMT,
     append: bool = True,
 ) -> logging.Logger:
-    f"""Set-up the logging on sys.stdout and file if path is given.
+    """Set up the logging on sys.stdout and file if path is given.
 
     Parameters
     ----------
     name : str, optional
         logger name, by default "hydromt"
     path : str, optional
         path to logfile, by default None
     log_level : int, optional
         Log level [0-50], by default 20 (info)
     fmt : str, optional
-        log message formatter, by default {FMT}
+        log message formatter
     append : bool, optional
-        Wether to append (True) or overwrite (False) to a logfile at path, by default True
+        Whether to append (True) or overwrite (False) to a logfile at path,
+        by default True
 
     Returns
     -------
     logging.Logger
         _description_
     """
     logger = logging.getLogger(name)
@@ -69,20 +69,34 @@
     if isfile:
         logger.debug(f"Appending log messages to file {path}.")
     else:
         logger.debug(f"Writing log messages to new file {path}.")
 
 
 def logged(logger):
+    """Define a decorator that logs the execution of a function.
+
+    This decorator logs the input arguments, output, and any raised exceptions of
+    the decorated function using the provided logger.
+
+    Parameters
+    ----------
+    logger : Logger
+        The logger object used to log the function execution.
+
+    Returns
+    -------
+    wrap : callable
+        The decorator function that wraps the decorated function.
+    """
+
     def wrap(function):
         @wraps(function)
         def wrapper(*args, **kwargs):
-            # logger = logging.getLogger(log)
             f = function.__name__
-            # logger.debug(f"Calling '{f}'")
             logger.debug(f"{f} - args={args} kwargs={kwargs}")
             try:
                 response = function(*args, **kwargs)
             except Exception as error:
                 e = error.__class__.__name__
                 emsg = str(error)
                 logger.error(f"{f} - raised {e} with error '{emsg}'")
```

### Comparing `hydromt-0.7.1/hydromt/merge.py` & `hydromt-0.8.0/hydromt/merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,35 @@
+"""Implementations relating to merging of datasets and arrays."""
 import numpy as np
-import geopandas as gpd
 import rasterio
 from pyproj import CRS
-from shapely.geometry import box
 
 from .raster import full_from_transform
 
 
 def merge(
     data_arrays,
     dst_crs=None,
     dst_bounds=None,
     dst_res=None,
     align=True,
     mask=None,
     merge_method="first",
     **kwargs,
 ):
-    """Merge multiple tiles to a single DataArray, if mismatching grid CRS or resolution,
-    tiles are reprojected to match the output DataArray grid. If no destination
+    """Merge multiple tiles to a single DataArray.
+
+    If mismatching grid CRS or resolution, tiles are reprojected
+    to match the output DataArray grid. If no destination
     grid is defined it is based on the first DataArray in the list.
 
     Based on :py:meth:`rasterio.merge.merge`.
 
     Arguments
-    ----------
+    ---------
     data_arrays: list of xarray.DataArray
         Tiles to merge
     dst_crs: pyproj.CRS, int
         CRS (or EPSG code) of destination grid
     dst_bounds: list of float
         Bounding box [xmin, ymin, xmax, ymax] of destination grid
     dst_res: float
@@ -43,22 +44,22 @@
 
         * first: reverse painting
         * last: paint valid new on top of existing
         * min: pixel-wise min of existing and new
         * max: pixel-wise max of existing and new
         * new: assert no pixel overlap
     **kwargs:
-        Key-word arguments passed to :py:meth:`~hydromt.raster.RasterDataArray.reproject`
+        Key-word arguments passed to
+        :py:meth:`~hydromt.raster.RasterDataArray.reproject`
 
     Returns
     -------
     da_out: xarray.DataArray
         Merged tiles.
     """
-
     # define merge method
     if merge_method == "first":
 
         def copyto(old_data, new_data, old_nodata, new_nodata):
             dmask = np.logical_and(old_nodata, ~new_nodata)
             old_data[dmask] = new_data[dmask]
```

### Comparing `hydromt-0.7.1/hydromt/models/model_api.py` & `hydromt-0.8.0/hydromt/models/model_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 # -*- coding: utf-8 -*-
-"""General and basic API for models in HydroMT"""
+"""General and basic API for models in HydroMT."""
 
-from abc import ABCMeta
-import os
 import glob
-from os.path import join, isdir, isfile, abspath, dirname, basename, isabs
-import xarray as xr
-import numpy as np
-import geopandas as gpd
-from geopandas.testing import assert_geodataframe_equal
-from shapely.geometry import box
-import logging
-from pathlib import Path
 import inspect
+import logging
+import os
+import typing
 import warnings
+from abc import ABCMeta
+from os.path import abspath, basename, dirname, isabs, isdir, isfile, join
+from pathlib import Path
+from typing import Any, Dict, List, Optional, Tuple, Union
+
+import geopandas as gpd
+import numpy as np
+import pandas as pd
+import xarray as xr
+from geopandas.testing import assert_geodataframe_equal
 from pyproj import CRS
-import typing
-from typing import Any, Dict, List, Tuple, Union, Optional
+from shapely.geometry import box
 
-from ..data_catalog import DataCatalog
 from .. import config, log, workflows
+from ..data_catalog import DataCatalog
 from ..raster import GEO_MAP_COORD
 
 __all__ = ["Model"]
 
 logger = logging.getLogger(__name__)
 
 
 class Model(object, metaclass=ABCMeta):
-    """General and basic API for models in HydroMT"""
+
+    """General and basic API for models in HydroMT."""
 
     # FIXME
     _DATADIR = ""  # path to the model data folder
     _NAME = "modelname"
     _CONF = "model.ini"
     _CF = dict()  # configreader kwargs
     _GEOMS = {"<general_hydromt_name>": "<model_name>"}
@@ -58,27 +61,31 @@
         root: Optional[str] = None,
         mode: Optional[str] = "w",
         config_fn: Optional[str] = None,
         data_libs: Union[List, str] = [],
         logger=logger,
         **artifact_keys,
     ):
-        """Initialize a model
+        """Initialize a model.
 
         Parameters
         ----------
         root : str, optional
             Model root, by default None
         mode : {'r','r+','w'}, optional
             read/append/write mode, by default "w"
         config_fn : str, optional
             Model simulation configuration file, by default None.
             Note that this is not the HydroMT model setup configuration file!
         data_libs : List[str], optional
             List of data catalog yaml files, by default None
+        **artifact_keys:
+            Additional keyword arguments to be passed down.
+        logger:
+            The logger to be used.
         """
         from . import MODELS  # avoid circular import
 
         self.logger = logger
         dist, version = "unknown", "NA"
         if self._NAME in MODELS:
             ep = MODELS[self._NAME]
@@ -86,17 +93,19 @@
 
         # link to data
         self.data_catalog = DataCatalog(
             data_libs=data_libs, logger=self.logger, **artifact_keys
         )
 
         # placeholders
-        # metadata maps that can be at different resolutions #TODO> do we want read/write maps?
+        # metadata maps that can be at different resolutions
+        # TODO do we want read/write maps?
         self._config = dict()  # nested dictionary
         self._maps = dict()  # dictionary of xr.DataArray and/or xr.Dataset
+
         # NOTE was staticgeoms in <=v0.5
         self._geoms = dict()  # dictionary of gdp.GeoDataFrame
         self._forcing = dict()  # dictionary of xr.DataArray and/or xr.Dataset
         self._states = dict()  # dictionary of xr.DataArray and/or xr.Dataset
         self._results = dict()  # dictionary of xr.DataArray and/or xr.Dataset
         # To be deprecated in future versions!
         self._staticmaps = xr.Dataset()
@@ -110,15 +119,15 @@
         # model paths
         self._config_fn = self._CONF if config_fn is None else config_fn
         self.set_root(root, mode)  # also creates hydromt.log file
         self.logger.info(f"Initializing {self._NAME} model from {dist} (v{version}).")
 
     @property
     def api(self) -> Dict:
-        """Return all model components and their data types"""
+        """Return all model components and their data types."""
         _api = self._API.copy()
         # loop over parent and mixin classes and update API
         for base_cls in self.__class__.__bases__:
             _api.update(getattr(base_cls, "_API", {}))
         return _api
 
     def _check_get_opt(self, opt):
@@ -126,15 +135,15 @@
         for method in opt.keys():
             m = method.strip("0123456789")
             if not callable(getattr(self, m, None)):
                 raise ValueError(f'Model {self._NAME} has no method "{method}"')
         return opt
 
     def _run_log_method(self, method, *args, **kwargs):
-        """Log method parameters before running a method"""
+        """Log method parameters before running a method."""
         method = method.strip("0123456789")
         func = getattr(self, method)
         signature = inspect.signature(func)
         # combine user and default options
         params = {}
         for i, (k, v) in enumerate(signature.parameters.items()):
             if k in ["args", "kwargs"]:
@@ -157,32 +166,34 @@
         self,
         region: Optional[dict] = None,
         write: Optional[bool] = True,
         opt: Optional[dict] = {},
     ):
         """Single method to build a model from scratch based on settings in `opt`.
 
-        Methods will be run one by one based on the order of appearance in `opt` (.ini configuration file).
-        All model methods are supported including setup_*, read_* and write_* methods.
+        Methods will be run one by one based on the order of appearance in `opt`
+        (.ini configuration file). All model methods are supported including
+        setup_*, read_* and write_* methods.
 
-        If a write_* option is listed in `opt` (ini file) the full writing of the model at the end
-        of the update process is skipped.
+        If a write_* option is listed in `opt` (ini file) the full writing of the
+        model at the end of the update process is skipped.
 
         Parameters
         ----------
         region: dict
             Description of model region. See :py:meth:`~hydromt.workflows.parse_region`
             for all options.
         write: bool, optional
-            Write the complete model after executing all methods in opt, by default True.
+            Write complete model after executing all methods in opt, by default True.
         opt: dict, optional
             Model build configuration. The configuration can be parsed from a
             .ini file using :py:meth:`~hydromt.config.configread`.
-            This is a nested dictionary where the first-level keys are the names of model
-            specific (setup) methods and the second-level contain argument-value pairs of the method.
+            This is a nested dictionary where the first-level keys are the names
+            of model specific (setup) methods and the second-level contain
+            argument-value pairs of the method.
 
             .. code-block:: text
 
                 {
                     <name of method1>: {
                         <argument1>: <value1>, <argument2>: <value2>
                     },
@@ -198,15 +209,15 @@
         if region is not None:
             if self._CLI_ARGS["region"] not in opt:
                 opt = {self._CLI_ARGS["region"]: {}, **opt}
             opt[self._CLI_ARGS["region"]].update(region=region)
 
         # then loop over other methods
         for method in opt:
-            # if any write_* functions are present in opt, skip the final self.write() call
+            # if any write_* functions are present in opt, skip the final self.write()
             if method.startswith("write_"):
                 write = False
             kwargs = {} if opt[method] is None else opt[method]
             self._run_log_method(method, **kwargs)
 
         # write
         if write:
@@ -216,33 +227,35 @@
         self,
         model_out: Optional[Union[str, Path]] = None,
         write: Optional[bool] = True,
         opt: Dict = {},
     ):
         """Single method to update a model based the settings in `opt`.
 
-        Methods will be run one by one based on the order of appearance in `opt` (ini configuration file).
+        Methods will be run one by one based on the order of appearance in `opt`
+        (ini configuration file).
 
         All model methods are supported including setup_*, read_* and write_* methods.
-        If a write_* option is listed in `opt` (ini file) the full writing of the model at the end
-        of the update process is skipped.
+        If a write_* option is listed in `opt` (ini file) the full writing of the model
+        at the end of the update process is skipped.
 
         Parameters
         ----------
         model_out: str, path, optional
             Destination folder to write the model schematization after updating
             the model. If None the updated model components are overwritten in the
             current model schematization if these exist. By default None.
         write: bool, optional
             Write the updated model schematization to disk. By default True.
         opt: dict, optional
             Model build configuration. The configuration can be parsed from a
             .ini file using :py:meth:`~hydromt.config.configread`.
-            This is a nested dictionary where the first-level keys are the names of model
-            specific (setup) methods and the second-level contain argument-value pairs of the method.
+            This is a nested dictionary where the first-level keys
+            are the names of model specific (setup) methods and
+            the second-level contain argument-value pairs of the method.
 
             .. code-block:: text
 
                 {
                     <name of method1>: {
                         <argument1>: <value1>, <argument2>: <value2>
                     },
@@ -270,15 +283,15 @@
         method = self._CLI_ARGS["region"]
         if method in opt:
             opt.pop(method)  # remove from opt
             self.logger.warning(f'"{method}" can only be called when building a model.')
 
         # loop over other methods from ini file
         for method in opt:
-            # if any write_* functions are present in opt, skip the final self.write() call
+            # if any write_* functions are present in opt, skip the final self.write()
             if method.startswith("write_"):
                 write = False
             kwargs = {} if opt[method] is None else opt[method]
             self._run_log_method(method, **kwargs)
 
         # write
         if write:
@@ -288,16 +301,15 @@
 
     def setup_region(
         self,
         region: dict,
         hydrography_fn: str = "merit_hydro",
         basin_index_fn: str = "merit_hydro_index",
     ) -> dict:
-        """
-        This component sets the `region` of interest of the model.
+        """Set the `region` of interest of the model.
 
         Adds model layer:
 
         * **region** geom: region boundary vector
 
         Parameters
         ----------
@@ -358,21 +370,21 @@
         elif "model" in region:
             geom = region["model"].region
         else:
             raise ValueError(f"model region argument not understood: {region}")
 
         self.set_geoms(geom, name="region")
 
-        # This setup method returns region so that it can be wrapped for models which require
-        # more information, e.g. grid RasterDataArray or xy coordinates.
+        # This setup method returns region so that it can be wrapped for models which
+        # require more information, e.g. grid RasterDataArray or xy coordinates.
         return region
 
-    # TODO remove
-    # placeholder to make make sure build with the current _CLI_ARGS does not raise an error
-    def setup_basemaps(self, *args, **kwargs):
+    # TODO remove placeholder to make make sure
+    # build with the current _CLI_ARGS does not raise an error
+    def setup_basemaps(self, *args, **kwargs):  # noqa: D102
         warnings.warn(
             "The setup_basemaps method is not implemented.",
             UserWarning,
         )
 
     ## file system
 
@@ -407,15 +419,14 @@
             read/append/write mode for model files
         """
         ignore_ext = set([".log", ".yml"])
         if mode not in ["r", "r+", "w", "w+"]:
             raise ValueError(
                 f'mode "{mode}" unknown, select from "r", "r+", "w" or "w+"'
             )
-        # old_root = getattr(self, "_root", None)
         self._root = root if root is None else abspath(root)
         self._read = mode.startswith("r")
         self._write = mode != "r"
         self._overwrite = mode == "w+"
         if root is not None:
             if self._write:
                 for name in self._FOLDERS:
@@ -431,23 +442,25 @@
                         if mode.endswith("+"):
                             self.logger.warning(
                                 "Model dir already exists and "
                                 f"files might be overwritten: {path}."
                             )
                         else:
                             msg = (
-                                f"Model dir already exists and cannot be overwritten: {path}."
-                                "Use 'mode=w+' to force overwrite existing files."
+                                "Model dir already exists and cannot be "
+                                + f"overwritten: {path}. Use 'mode=w+' to force "
+                                + "overwrite existing files."
                             )
                             self.logger.error(msg)
                             raise IOError(msg)
             # check directory
             elif not isdir(self._root):
                 raise IOError(f'model root not found at "{self._root}"')
-            # remove old logging file handler and add new filehandler in root if it does not exist
+            # remove old logging file handler and add new filehandler
+            # in root if it does not exist
             has_log_file = False
             log_level = 20  # default, but overwritten by the level of active loggers
             for i, h in enumerate(self.logger.handlers):
                 log_level = h.level
                 if hasattr(h, "baseFilename"):
                     if dirname(h.baseFilename) != self._root:
                         self.logger.handlers.pop(
@@ -474,16 +487,17 @@
         ],
     ) -> None:
         """Read the complete model schematization and configuration from model files.
 
         Parameters
         ----------
         components : List, optional
-            List of model components to read, each should have an associated read_<component> method.
-            By default ['config', 'maps', 'staticmaps', 'geoms', 'forcing', 'states', 'results']
+            List of model components to read, each should have an associated
+            read_<component> method. By default ['config', 'maps', 'staticmaps',
+            'geoms', 'forcing', 'states', 'results']
         """
         self.logger.info(f"Reading model data from {self.root}")
         for component in components:
             if not hasattr(self, f"read_{component}"):
                 raise AttributeError(
                     f"{type(self).__name__} does not have read_{component}"
                 )
@@ -501,16 +515,17 @@
         ],
     ) -> None:
         """Write the complete model schematization and configuration to model files.
 
         Parameters
         ----------
         components : List, optional
-            List of model components to write, each should have an associated write_<component> method.
-            By default ['config', 'maps', 'staticmaps', 'geoms', 'forcing', 'states']
+            List of model components to write, each should have an
+            associated write_<component> method. By default ['config', 'maps',
+            'staticmaps', 'geoms', 'forcing', 'states']
         """
         self.logger.info(f"Writing model data to {self.root}")
         for component in components:
             if not hasattr(self, f"write_{component}"):
                 raise AttributeError(
                     f"{type(self).__name__} does not have write_{component}"
                 )
@@ -519,23 +534,24 @@
     def write_data_catalog(
         self,
         root: Optional[Union[str, Path]] = None,
         data_lib_fn: Union[str, Path] = "hydromt_data.yml",
         used_only: bool = True,
         append: bool = True,
     ):
-        """Write the data catalog to data_lib_fn
+        """Write the data catalog to data_lib_fn.
 
         Parameters
         ----------
         root: str, Path, optional
             Global root for all relative paths in yaml file.
             If "auto" the data source paths are relative to the yaml output ``path``.
         data_lib_fn: str, Path, optional
-            Path of output yml file, absolute or relative to the model root, by default "hydromt_data.yml".
+            Path of output yml file, absolute or relative to the model root,
+            by default "hydromt_data.yml".
         used_only: bool, optional
             If True, export only data entries kept in used_data list. By default True
         append: bool, optional
             If True, append to an existing
         """
         path = data_lib_fn if isabs(data_lib_fn) else join(self.root, data_lib_fn)
         cat = DataCatalog(logger=self.logger, fallback_lib=None)
@@ -553,15 +569,15 @@
         if cat.sources:
             self._assert_write_mode
             cat.to_yml(path, root=root)
 
     # model configuration
     @property
     def config(self) -> Dict[str, Union[Dict, str]]:
-        """Model configuration. Returns a (nested) dictionary"""
+        """Model configuration. Returns a (nested) dictionary."""
         # initialize default config if in write-mode
         if not self._config:
             self.read_config()
         return self._config
 
     def set_config(self, *args):
         """Update the config dictionary at key(s) with values.
@@ -586,42 +602,44 @@
             raise TypeError("set_config() requires a least one key and one value.")
         args = list(args)
         value = args.pop(-1)
         if len(args) == 1 and "." in args[0]:
             args = args[0].split(".") + args[1:]
         branch = self.config  # reads config at first call
         for key in args[:-1]:
-            if not key in branch or not isinstance(branch[key], dict):
+            if key not in branch or not isinstance(branch[key], dict):
                 branch[key] = {}
             branch = branch[key]
         branch[args[-1]] = value
 
     def setup_config(self, **cfdict):
-        """Update config with a dictionary"""
+        """Update config with a dictionary."""
         # TODO rename to update_config
         if len(cfdict) > 0:
-            self.logger.debug(f"Setting model config options.")
+            self.logger.debug("Setting model config options.")
         for key, value in cfdict.items():
             self.set_config(key, value)
 
     def get_config(self, *args, fallback=None, abs_path: Optional[bool] = False):
         """Get a config value at key(s).
 
         Parameters
         ----------
         args : tuple or string
             keys can given by multiple args: ('key1', 'key2')
             or a string with '.' indicating a new level: ('key1.key2')
         fallback: any, optional
             fallback value if key(s) not found in config, by default None.
         abs_path: bool, optional
-            If True return the absolute path relative to the model root, by deafult False.
+            If True return the absolute path relative to the model root,
+            by deafult False.
             NOTE: this assumes the config is located in model root!
 
         Returns
+        -------
         value : any type
             dictionary value
 
         Examples
         --------
         >> # self.config = {'a': 1, 'b': {'c': {'d': 2}}}
 
@@ -653,83 +671,100 @@
     def _configread(self, fn: str):
         return config.configread(fn, abs_path=False)
 
     def _configwrite(self, fn: str):
         return config.configwrite(fn, self.config)
 
     def read_config(self, config_fn: Optional[str] = None):
-        """Parse config from file. If no config file found a default config file is
-        read in writing mode."""
+        """Parse config from file.
+
+        If no config file found a default config file is read in writing mode.
+        """
         prefix = "User defined"
         if config_fn is None:  # prioritize user defined config path (new v0.4.1)
             if not self._read:  # write-only mode > read default config
                 config_fn = join(self._DATADIR, self._NAME, self._CONF)
                 prefix = "Default"
             elif self.root is not None:  # append or write mode > read model config
                 config_fn = join(self.root, self._config_fn)
                 prefix = "Model"
         cfdict = dict()
         if config_fn is not None:
             if isfile(config_fn):
                 cfdict = self._configread(config_fn)
                 self.logger.debug(f"{prefix} config read from {config_fn}")
-            elif not self._read and prefix != "Default":  # skip for missing default
+            elif (
+                self._root is not None
+                and not isabs(config_fn)
+                and isfile(join(self._root, config_fn))
+            ):
+                cfdict = self._configread(join(self.root, config_fn))
+                self.logger.debug(
+                    f"{prefix} config read from {join(self.root,config_fn)}"
+                )
+            elif isfile(abspath(config_fn)):
+                cfdict = self._configread(abspath(config_fn))
+                self.logger.debug(f"{prefix} config read from {abspath(config_fn)}")
+            else:  # skip for missing default
                 self.logger.error(f"{prefix} config file not found at {config_fn}")
+
         self._config = cfdict
 
     def write_config(
         self, config_name: Optional[str] = None, config_root: Optional[str] = None
     ):
-        """Write config to <root/config_fn>"""
+        """Write config to <root/config_fn>."""
         self._assert_write_mode
         if config_name is not None:
             self._config_fn = config_name
         elif self._config_fn is None:
             self._config_fn = self._CONF
         if config_root is None:
             config_root = self.root
         fn = join(config_root, self._config_fn)
         self.logger.info(f"Writing model config to {fn}")
         self._configwrite(fn)
 
     # model static maps
     @property
     def staticmaps(self):
-        """Model static maps. Returns xarray.Dataset,
-        ..NOTE: will be deprecated in future versions and replaced by `grid`
+        """Model static maps.
+
+        Returns xarray.Dataset,
+        ..NOTE: will be deprecated in future versions and replaced by `grid`.
         """
         warnings.warn(
-            "The staticmaps property of the Model class will be deprecated in future versions, "
-            "use the grid property of the GridModel class instead.",
+            "The staticmaps property of the Model class will be deprecated in future"
+            "versions. Use the grid property of the GridModel class instead.",
             DeprecationWarning,
         )
         if len(self._staticmaps) == 0 and self._read:
             self.read_staticmaps()
         return self._staticmaps
 
     def set_staticmaps(
         self, data: Union[xr.DataArray, xr.Dataset], name: Optional[str] = None
     ):
-        """
-        This method will be deprecated in future versions. See :py:meth:`~hydromt.models.GridModel.set_grid`
-
-        Add data to staticmaps.
+        """Add data to staticmaps.
 
         All layers of staticmaps must have identical spatial coordinates.
+        This method will be deprecated in future versions. See
+        :py:meth:`~hydromt.models.GridModel.set_grid`.
 
         Parameters
         ----------
         data: xarray.DataArray or xarray.Dataset
             new map layer to add to staticmaps
         name: str, optional
             Name of new map layer, this is used to overwrite the name of a DataArray
             or to select a variable from a Dataset.
         """
         warnings.warn(
-            "The set_staticmaps method will be deprecated in future versions, use set_grid instead.",
+            "The set_staticmaps method will be deprecated in future versions, "
+            + "use set_grid instead.",
             DeprecationWarning,
         )
         if name is None:
             if isinstance(data, xr.DataArray) and data.name is not None:
                 name = data.name
             elif not isinstance(data, xr.Dataset):
                 raise ValueError("Setting a map requires a name")
@@ -753,83 +788,97 @@
                 data = xr.DataArray(dims=self.dims, data=data, name=name).to_dataset()
             for dvar in data.data_vars.keys():
                 if dvar in self._staticmaps:
                     self.logger.warning(f"Replacing staticmap: {dvar}")
                 self._staticmaps[dvar] = data[dvar]
 
     def read_staticmaps(self, fn: str = "staticmaps/staticmaps.nc", **kwargs) -> None:
-        """Read static model maps at <root>/<fn> and add to staticmaps property
+        """Read static model maps at <root>/<fn> and add to staticmaps property.
 
         key-word arguments are passed to :py:func:`xarray.open_dataset`
 
-        .. NOTE: this method is deprecated. Use the grid property of the GridMixin instead.
+        .. NOTE: this method is deprecated.
+        Use the grid property of the GridMixin instead.
 
         Parameters
         ----------
         fn : str, optional
             filename relative to model root, by default "staticmaps/staticmaps.nc"
+        **kwargs:
+            Additional keyword arguments that are passed to the
+            `_read_nc` function.
         """
         self._assert_read_mode
         for ds in self._read_nc(fn, **kwargs).values():
             self.set_staticmaps(ds)
 
     def write_staticmaps(self, fn: str = "staticmaps/staticmaps.nc", **kwargs) -> None:
-        """Write static model maps to netcdf file at <root>/<fn>
+        """Write static model maps to netcdf file at <root>/<fn>.
 
         key-word arguments are passed to :py:meth:`xarray.Dataset.to_netcdf`
 
-        .. NOTE: this method is deprecated. Use the grid property of the GridMixin instead.
+        .. NOTE: this method is deprecated.
+        Use the grid property of the GridMixin instead.
 
         Parameters
         ----------
         fn : str, optional
             filename relative to model root, by default 'staticmaps/staticmaps.nc'
+        **kwargs:
+            Additional keyword arguments that are passed to the
+            `_write_nc` function.
         """
         if len(self._staticmaps) == 0:
             self.logger.debug("No staticmaps data found, skip writing.")
         else:
             self._assert_write_mode
             # _write_nc requires dict - use dummy 'staticmaps' key
             nc_dict = {"staticmaps": self._staticmaps}
             self._write_nc(nc_dict, fn, **kwargs)
 
     # map files setup methods
-    def setup_maps_from_raster(
+    def setup_maps_from_rasterdataset(
         self,
-        raster_fn: str,
+        raster_fn: Union[str, Path, xr.Dataset],
         variables: Optional[List] = None,
         fill_method: Optional[str] = None,
         name: Optional[str] = None,
         reproject_method: Optional[str] = None,
         split_dataset: Optional[bool] = True,
+        rename: Optional[Dict] = dict(),
     ) -> List[str]:
-        """
-        This component adds data variable(s) from ``raster_fn`` to maps object.
+        """HYDROMT CORE METHOD: Add data variable(s) from ``raster_fn`` to maps object.
 
-        If raster is a dataset, all variables will be added unless ``variables`` list is specified.
+        If raster is a dataset, all variables will be added unless ``variables``
+        list is specified.
 
         Adds model layers:
 
         * **raster.name** maps: data from raster_fn
 
         Parameters
         ----------
-        raster_fn: str
-            Source name of raster data in data_catalog.
+        raster_fn: str, Path, xr.Dataset
+            Data catalog key, path to raster file or raster xarray data object.
         variables: list, optional
             List of variables to add to maps from raster_fn. By default all.
         fill_method : str, optional
             If specified, fills nodata values using fill_nodata method.
             Available methods are {'linear', 'nearest', 'cubic', 'rio_idw'}.
         name: str, optional
-            Name of new maps variable, only in case split_dataset=False.
+            Name of new dataset in self.maps dictionnary,
+            only in case split_dataset=False.
         reproject_method: str, optional
-            See rasterio.warp.reproject for existing methods, by default the data is not reprojected (None).
+            See rasterio.warp.reproject for existing methods, by default the data is
+            not reprojected (None).
         split_dataset: bool, optional
-            If data is a xarray.Dataset split it into several xarray.DataArrays (default).
+            If data is a xarray.Dataset split it into several xarray.DataArrays.
+        rename: dict, optional
+            Dictionary to rename variable names in raster_fn before adding to maps
+            {'name_in_raster_fn': 'name_in_maps'}. By default empty.
 
         Returns
         -------
         list
             Names of added model map layers
         """
         self.logger.info(f"Preparing maps data from raster source {raster_fn}")
@@ -843,97 +892,111 @@
         )
         # Fill nodata
         if fill_method is not None:
             ds = ds.raster.interpolate_na(method=fill_method)
         # Reprojection
         if ds.rio.crs != self.crs and reproject_method is not None:
             ds = ds.raster.reproject(dst_crs=self.crs, method=reproject_method)
-        # Add to maps
-        self.set_maps(ds, name=name, split_dataset=split_dataset)
+        # Rename and add to maps
+        self.set_maps(ds.rename(rename), name=name, split_dataset=split_dataset)
 
         return list(ds.data_vars.keys())
 
     def setup_maps_from_raster_reclass(
         self,
-        raster_fn: str,
-        reclass_table_fn: str,
+        raster_fn: Union[str, Path, xr.DataArray],
+        reclass_table_fn: Union[str, Path, pd.DataFrame],
         reclass_variables: List,
         variable: Optional[str] = None,
         fill_method: Optional[str] = None,
         reproject_method: Optional[str] = None,
         name: Optional[str] = None,
         split_dataset: Optional[bool] = True,
+        rename: Optional[Dict] = dict(),
         **kwargs,
     ) -> List[str]:
-        """
-        This component adds data variable(s) to maps object by reclassifying the data in ``raster_fn`` based on ``reclass_table_fn``.
+        """HYDROMT CORE METHOD: Add data variable(s) to maps object by reclassifying the data in ``raster_fn`` based on ``reclass_table_fn``.
+
+        This is done by reclassifying the data in
+        ``raster_fn`` based on ``reclass_table_fn``.
 
         Adds model layers:
 
         * **reclass_variables** maps: reclassified raster data
 
         Parameters
         ----------
-        raster_fn: str
-            Source name of raster data in data_catalog. Should be a DataArray. Else use **kwargs to select variables/time_tuple in
-            :py:meth:`hydromt.data_catalog.get_rasterdataset` method.
-        reclass_table_fn: str
-            Source name of reclassification table of `raster_fn` in data_catalog.
+        raster_fn: str, Path, xr.DataArray
+            Data catalog key, path to raster file or raster xarray data object.
+            Should be a DataArray. Else use `variable` argument for selection.
+        reclass_table_fn: str, Path, pd.DataFrame
+            Data catalog key, path to tabular data file or tabular pandas dataframe
+            object for the reclassification table of `raster_fn`.
         reclass_variables: list
-            List of reclass_variables from reclass_table_fn table to add to maps. Index column should match values in `raster_fn`.
+            List of reclass_variables from reclass_table_fn table to add to maps. Index
+            column should match values in `raster_fn`.
         variable: str, optional
-            Name of raster dataset variable to use. This is only required when reading datasets with multiple variables.
-            By default None.
+            Name of raster dataset variable to use. This is only required when reading
+            datasets with multiple variables. By default None.
         fill_method : str, optional
-            If specified, fills nodata values in `raster_fn` using fill_nodata method before reclassifying.
-            Available methods are {'linear', 'nearest', 'cubic', 'rio_idw'}.
+            If specified, fills nodata values in `raster_fn` using fill_nodata method
+            before reclassifying. Available methods are {'linear', 'nearest',
+            'cubic', 'rio_idw'}.
         reproject_method: str, optional
-            See rasterio.warp.reproject for existing methods, by default the data is not reprojected (None).
+            See rasterio.warp.reproject for existing methods, by default the data is
+            not reprojected (None).
         name: str, optional
             Name of new maps variable, only in case split_dataset=False.
         split_dataset: bool, optional
-            If data is a xarray.Dataset split it into several xarray.DataArrays (default).
+            If data is a xarray.Dataset split it into several xarray.DataArrays.
+        rename: dict, optional
+            Dictionary to rename variable names in reclass_variables before adding to
+            grid {'name_in_reclass_table': 'name_in_grid'}. By default empty.
+        **kwargs:
+            Additional keyword arguments that are passed to the
+            `data_catalog.get_rasterdataset` function.
 
         Returns
         -------
         list
             Names of added model map layers
-        """
+        """  # noqa: E501
         self.logger.info(
-            f"Preparing map data by reclassifying the data in {raster_fn} based on {reclass_table_fn}"
+            f"Preparing map data by reclassifying the data in {raster_fn} based"
+            f" on {reclass_table_fn}"
         )
         # Read raster data and remapping table
         da = self.data_catalog.get_rasterdataset(
-            raster_fn, geom=self.region, buffer=2, **kwargs
+            raster_fn, geom=self.region, buffer=2, variables=variable, **kwargs
         )
         if not isinstance(da, xr.DataArray):
             raise ValueError(
                 f"raster_fn {raster_fn} should be a single variable. "
                 "Please select one using the 'variable' argument"
             )
         df_vars = self.data_catalog.get_dataframe(
             reclass_table_fn, variables=reclass_variables
         )
         # Fill nodata
         if fill_method is not None:
-            ds = ds.raster.interpolate_na(method=fill_method)
+            da = da.raster.interpolate_na(method=fill_method)
         # Mapping function
         ds_vars = da.raster.reclassify(reclass_table=df_vars, method="exact")
         # Reprojection
         if ds_vars.rio.crs != self.crs and reproject_method is not None:
             ds_vars = ds_vars.raster.reproject(dst_crs=self.crs)
         # Add to maps
-        self.set_maps(ds_vars, name=name, split_dataset=split_dataset)
+        self.set_maps(ds_vars.rename(rename), name=name, split_dataset=split_dataset)
 
         return list(ds_vars.data_vars.keys())
 
     # model map
     @property
     def maps(self) -> Dict[str, Union[xr.Dataset, xr.DataArray]]:
-        """Model maps. Returns dict of xarray.DataArray or xarray.Dataset"""
+        """Model maps. Returns dict of xarray.DataArray or xarray.Dataset."""
         if len(self._maps) == 0 and self._read:
             self.read_maps()
         return self._maps
 
     def set_maps(
         self,
         data: Union[xr.DataArray, xr.Dataset],
@@ -946,111 +1009,128 @@
         DataArrays using the split_dataset argument.
 
         Arguments
         ---------
         data: xarray.Dataset or xarray.DataArray
             New forcing data to add
         name: str, optional
-            Variable name, only in case data is of type DataArray or if a Dataset is added as is (split_dataset=False).
+            Variable name, only in case data is of type DataArray or if a Dataset is
+            added as is (split_dataset=False).
         split_dataset: bool, optional
-            If data is a xarray.Dataset split it into several xarray.DataArrays (default).
+            If data is a xarray.Dataset split it into several xarray.DataArrays.
         """
         data_dict = _check_data(data, name, split_dataset)
         for name in data_dict:
             if name in self._maps:
                 self.logger.warning(f"Replacing result: {name}")
             self._maps[name] = data_dict[name]
 
     def read_maps(self, fn: str = "maps/*.nc", **kwargs) -> None:
-        """Read model map at <root>/<fn> and add to maps component
+        """Read model map at <root>/<fn> and add to maps component.
 
         key-word arguments are passed to :py:func:`xarray.open_dataset`
 
         Parameters
         ----------
         fn : str, optional
             filename relative to model root, may wildcards, by default "maps/*.nc"
+        **kwargs:
+            Additional keyword arguments that are passed to the
+            `_read_nc` function.
         """
         self._assert_read_mode
         ncs = self._read_nc(fn, **kwargs)
         for name, ds in ncs.items():
             self.set_maps(ds, name=name)
 
     def write_maps(self, fn="maps/{name}.nc", **kwargs) -> None:
-        """Write maps to netcdf file at <root>/<fn>
+        """Write maps to netcdf file at <root>/<fn>.
 
         key-word arguments are passed to :py:meth:`xarray.Dataset.to_netcdf`
 
         Parameters
         ----------
         fn : str, optional
             filename relative to model root and should contain a {name} placeholder,
             by default 'maps/{name}.nc'
+        **kwargs:
+            Additional keyword arguments that are passed to the
+            `_write_nc` function.
         """
         if len(self._maps) == 0:
             self.logger.debug("No maps data found, skip writing.")
         else:
             self._assert_write_mode
             self._write_nc(self._maps, fn, **kwargs)
 
     # model geometry files
     @property
     def geoms(self) -> Dict[str, Union[gpd.GeoDataFrame, gpd.GeoSeries]]:
-        """Model geometries. Returns dict of geopandas.GeoDataFrame or geopandas.GeoDataSeries
-        ..NOTE: previously call staticgeoms."""
+        """Model geometries.
+
+        Return dict of geopandas.GeoDataFrame or geopandas.GeoDataSeries
+        ..NOTE: previously call staticgeoms.
+        """
         if not self._geoms and self._read:
             self.read_geoms()
         return self._geoms
 
     def set_geoms(self, geom: Union[gpd.GeoDataFrame, gpd.GeoSeries], name: str):
         """Add data to the geoms attribute.
 
         Arguments
         ---------
-        geoms: geopandas.GeoDataFrame or geopandas.GeoSeries
+        geom: geopandas.GeoDataFrame or geopandas.GeoSeries
             New geometry data to add
         name: str
             Geometry name.
         """
         gtypes = [gpd.GeoDataFrame, gpd.GeoSeries]
         if not np.any([isinstance(geom, t) for t in gtypes]):
             raise ValueError(
-                "First parameter map(s) should be geopandas.GeoDataFrame or geopandas.GeoSeries"
+                "First parameter map(s) should be geopandas.GeoDataFrame"
+                " or geopandas.GeoSeries"
             )
         if name in self._geoms:
             self.logger.warning(f"Replacing geom: {name}")
         self._geoms[name] = geom
 
     def read_geoms(self, fn: str = "geoms/*.geojson", **kwargs) -> None:
-        """Read model geometries files at <root>/<fn> and add to geoms property
+        """Read model geometries files at <root>/<fn> and add to geoms property.
 
         key-word arguments are passed to :py:func:`geopandas.read_file`
 
         Parameters
         ----------
         fn : str, optional
             filename relative to model root, may wildcards, by default "geoms/*.nc"
+        **kwargs:
+            Additional keyword arguments that are passed to the
+            `geopandas.read_file` function.
         """
         self._assert_read_mode
         fns = glob.glob(join(self.root, fn))
         for fn in fns:
             name = basename(fn).split(".")[0]
             self.logger.debug(f"Reading model file {name}.")
             self.set_geoms(gpd.read_file(fn, **kwargs), name=name)
 
     def write_geoms(self, fn: str = "geoms/{name}.geojson", **kwargs) -> None:
-        """Write model geometries to a vector file (by default GeoJSON) at <root>/<fn>
+        """Write model geometries to a vector file (by default GeoJSON) at <root>/<fn>.
 
         key-word arguments are passed to :py:meth:`geopandas.GeoDataFrame.to_file`
 
         Parameters
         ----------
         fn : str, optional
             filename relative to model root and should contain a {name} placeholder,
             by default 'geoms/{name}.geojson'
+        **kwargs:
+            Additional keyword arguments that are passed to the
+            `geopandas.to_file` function.
         """
         if len(self._geoms) == 0:
             self.logger.debug("No geoms data found, skip writing.")
             return
         self._assert_write_mode
         if "driver" not in kwargs:
             kwargs.update(driver="GeoJSON")  # default
@@ -1062,56 +1142,74 @@
                 continue
             self.logger.debug(f"Writing file {fn.format(name=name)}")
             _fn = join(self.root, fn.format(name=name))
             if not isdir(dirname(_fn)):
                 os.makedirs(dirname(_fn))
             gdf.to_file(_fn, **kwargs)
 
-    # OLD model geometry files; TODO remove
-
     @property
     def staticgeoms(self):
-        """This property will be deprecated in future versions, use :py:meth:`~hydromt.Model.geom`"""
+        """Access the geometryes.
+
+        This property will be deprecated in future versions,
+        use :py:meth:`~hydromt.Model.geom`.
+        """
         warnings.warn(
-            "The staticgeoms method will be deprecated in future versions, use geoms instead.",
+            "The staticgeoms method will be deprecated in future versions,"
+            " use geoms instead.",
             DeprecationWarning,
         )
         if not self._geoms and self._read:
             self.read_staticgeoms()
         self._staticgeoms = self._geoms
         return self._staticgeoms
 
     def set_staticgeoms(self, geom: Union[gpd.GeoDataFrame, gpd.GeoSeries], name: str):
-        """This method will be deprecated in future versions, use :py:meth:`~hydromt.Model.set_geoms`"""
+        """Set the geometries.
+
+        This method will be deprecated in future versions,
+        use :py:meth:`~hydromt.Model.set_geoms`.
+        """
         warnings.warn(
-            "The set_staticgeoms method will be deprecated in future versions, use set_geoms instead.",
+            "The set_staticgeoms method will be deprecated in future versions,"
+            " use set_geoms instead.",
             DeprecationWarning,
         )
         return self.set_geoms(geom, name)
 
     def read_staticgeoms(self):
-        """This method will be deprecated in future versions, use :py:meth:`~hydromt.Model.read_geoms`"""
+        """Read gemoetries from disk.
+
+        This method will be deprecated in future versions
+        use :py:meth:`~hydromt.Model.read_geoms`.
+        """
         warnings.warn(
-            'The read_staticgeoms" method will be deprecated in future versions, use read_geoms instead.',
+            'The read_staticgeoms" method will be deprecated in future versions," \
+            " use read_geoms instead.',
             DeprecationWarning,
         )
         return self.read_geoms(fn="staticgeoms/*.geojson")
 
     def write_staticgeoms(self):
-        """This method will be deprecated in future versions, use :py:meth:`~hydromt.Model.write_geoms`"""
+        """Write the geometries to disk.
+
+        This method will be deprecated in future versions,
+        use :py:meth:`~hydromt.Model.write_geoms`.
+        """
         warnings.warn(
-            'The "write_staticgeoms" method will be deprecated in future versions, use  "write_geoms" instead.',
+            'The "write_staticgeoms" method will be deprecated in future versions,"\
+             " use  "write_geoms" instead.',
             DeprecationWarning,
         )
         return self.write_geoms(fn="staticgeoms/{name}.geojson")
 
     # model forcing files
     @property
     def forcing(self) -> Dict[str, Union[xr.Dataset, xr.DataArray]]:
-        """Model forcing. Returns dict of xarray.DataArray or xarray.Dataset"""
+        """Model forcing. Returns dict of xarray.DataArray or xarray.Dataset."""
         if not self._forcing and self._read:
             self.read_forcing()
         return self._forcing
 
     def set_forcing(
         self,
         data: Union[xr.DataArray, xr.Dataset],
@@ -1132,49 +1230,55 @@
         data_dict = _check_data(data, name, split_dataset)
         for name in data_dict:
             if name in self._forcing:
                 self.logger.warning(f"Replacing forcing: {name}")
             self._forcing[name] = data_dict[name]
 
     def read_forcing(self, fn: str = "forcing/*.nc", **kwargs) -> None:
-        """Read forcing at <root>/<fn> and add to forcing property
+        """Read forcing at <root>/<fn> and add to forcing property.
 
         key-word arguments are passed to :py:func:`xarray.open_dataset`
 
         Parameters
         ----------
         fn : str, optional
             filename relative to model root, may wildcards, by default "forcing/*.nc"
+        **kwargs:
+            Additional keyword arguments that are passed to the `_read_nc`
+            function.
         """
         self._assert_read_mode
         ncs = self._read_nc(fn, **kwargs)
         for name, ds in ncs.items():
             self.set_forcing(ds, name=name)
 
     def write_forcing(self, fn="forcing/{name}.nc", **kwargs) -> None:
-        """Write forcing to netcdf file at <root>/<fn>
+        """Write forcing to netcdf file at <root>/<fn>.
 
         key-word arguments are passed to :py:meth:`xarray.Dataset.to_netcdf`
 
         Parameters
         ----------
         fn : str, optional
             filename relative to model root and should contain a {name} placeholder,
             by default 'forcing/{name}.nc'
+        **kwargs:
+            Additional keyword arguments that are passed to the `_write_nc`
+            function.
         """
         if len(self._forcing) == 0:
             self.logger.debug("No forcing data found, skip writing.")
         else:
             self._assert_write_mode
             self._write_nc(self._forcing, fn, **kwargs)
 
     # model state files
     @property
     def states(self) -> Dict[str, Union[xr.Dataset, xr.DataArray]]:
-        """Model states. Returns dict of xarray.DataArray or xarray.Dataset"""
+        """Model states. Returns dict of xarray.DataArray or xarray.Dataset."""
         if not self._states and self._read:
             self.read_states()
         return self._states
 
     def set_states(
         self,
         data: Union[xr.DataArray, xr.Dataset],
@@ -1195,49 +1299,56 @@
         data_dict = _check_data(data, name, split_dataset)
         for name in data_dict:
             if name in self._states:
                 self.logger.warning(f"Replacing state: {name}")
             self._states[name] = data_dict[name]
 
     def read_states(self, fn: str = "states/*.nc", **kwargs) -> None:
-        """Read states at <root>/<fn> and add to states property
+        """Read states at <root>/<fn> and add to states property.
 
         key-word arguments are passed to :py:func:`xarray.open_dataset`
 
         Parameters
         ----------
         fn : str, optional
             filename relative to model root, may wildcards, by default "states/*.nc"
+        **kwargs:
+            Additional keyword arguments that are passed to the `_read_nc`
+            function.
         """
         self._assert_read_mode
         ncs = self._read_nc(fn, **kwargs)
         for name, ds in ncs.items():
             self.set_states(ds, name=name)
 
     def write_states(self, fn="states/{name}.nc", **kwargs) -> None:
-        """Write states to netcdf file at <root>/<fn>
+        """Write states to netcdf file at <root>/<fn>.
 
         key-word arguments are passed to :py:meth:`xarray.Dataset.to_netcdf`
 
         Parameters
         ----------
         fn : str, optional
             filename relative to model root and should contain a {name} placeholder,
             by default 'states/{name}.nc'
+        **kwargs:
+            Additional keyword arguments that are passed to the `RasterDatasetAdapter`
+            function.
         """
         if len(self._states) == 0:
             self.logger.debug("No states data found, skip writing.")
         else:
             self._assert_write_mode
             self._write_nc(self._states, fn, **kwargs)
 
-    # model results files; NOTE we don't have a write_results method (that's up to the model kernel)
+    # model results files; NOTE we don't have a write_results method
+    # (that's up to the model kernel)
     @property
     def results(self) -> Dict[str, Union[xr.Dataset, xr.DataArray]]:
-        """Model results.  Returns dict of xarray.DataArray or xarray.Dataset"""
+        """Model results.  Returns dict of xarray.DataArray or xarray.Dataset."""
         if not self._results and self._read:
             self.read_results()
         return self._results
 
     def set_results(
         self,
         data: Union[xr.DataArray, xr.Dataset],
@@ -1252,50 +1363,64 @@
         Arguments
         ---------
         data: xarray.Dataset or xarray.DataArray
             New forcing data to add
         name: str, optional
             Results name, required if data is xarray.Dataset and split_dataset=False.
         split_dataset: bool, optional
-            If True (False by default), split a Dataset to store each variable as a DataArray.
+            If True (False by default), split a Dataset to store each variable
+            as a DataArray.
         """
         data_dict = _check_data(data, name, split_dataset)
         for name in data_dict:
             if name in self._results:
                 self.logger.warning(f"Replacing result: {name}")
             self._results[name] = data_dict[name]
 
     def read_results(self, fn: str = "results/*.nc", **kwargs) -> None:
-        """Read results at <root>/<fn> and add to results property
+        """Read results at <root>/<fn> and add to results property.
 
         key-word arguments are passed to :py:func:`xarray.open_dataset`
 
         Parameters
         ----------
         fn : str, optional
             filename relative to model root, may wildcards, by default "results/*.nc"
+        **kwargs:
+            Additional keyword arguments that are passed to the `_read_nc`
+            function.
         """
         self._assert_read_mode
         ncs = self._read_nc(fn, **kwargs)
         for name, ds in ncs.items():
             self.set_results(ds, name=name)
 
     def _write_nc(
-        self, nc_dict: Dict[str, Union[xr.DataArray, xr.Dataset]], fn, **kwargs
+        self,
+        nc_dict: Dict[str, Union[xr.DataArray, xr.Dataset]],
+        fn: str,
+        gdal_compliant: bool = False,
+        rename_dims: bool = False,
+        force_sn: bool = False,
+        **kwargs,
     ) -> None:
         for name, ds in nc_dict.items():
             if not isinstance(ds, (xr.Dataset, xr.DataArray)) or len(ds) == 0:
                 self.logger.error(
                     f"{name} object of type {type(ds).__name__} not recognized"
                 )
                 continue
             self.logger.debug(f"Writing file {fn.format(name=name)}")
             _fn = join(self.root, fn.format(name=name))
             if not isdir(dirname(_fn)):
                 os.makedirs(dirname(_fn))
+            if gdal_compliant:
+                ds = ds.raster.gdal_compliant(
+                    rename_dims=rename_dims, force_sn=force_sn
+                )
             ds.to_netcdf(_fn, **kwargs)
 
     # general reader & writer
     def _read_nc(
         self, fn: str, mask_and_scale=False, single_var_as_array=True, **kwargs
     ) -> Dict[str, xr.Dataset]:
         ncs = dict()
@@ -1321,67 +1446,83 @@
         """Returns coordinate reference system embedded in region."""
         if len(self._staticmaps) > 0:
             return self.staticmaps.raster.crs
         else:
             return self.region.crs
 
     def set_crs(self, crs) -> None:
+        """Set the coordinate reference system."""
         warnings.warn(
-            '"set_crs" is deprecated. Please set the crs of all model components instead.',
+            '"set_crs" is deprecated. Please set the crs of all model'
+            " components instead.",
             DeprecationWarning,
         )
         if len(self._staticmaps) > 0:
             return self.staticmaps.raster.set_crs(crs)
 
     @property
     def dims(self) -> Tuple:
         """Returns spatial dimension names of staticmaps.
-        ..NOTE: will be deprecated in future versions"""
+
+        ..NOTE: will be deprecated in future versions.
+        """
         if len(self._staticmaps) > 0:
             return self.staticmaps.raster.dims
 
     @property
     def coords(self) -> Dict:
         """Returns the coordinates of model staticmaps.
-        ..NOTE: will be deprecated in future versions"""
+
+        ..NOTE: will be deprecated in future versions.
+        """
         if len(self._staticmaps) > 0:
             return self.staticmaps.raster.coords
 
     @property
     def res(self) -> Tuple:
         """Returns the resolution of the model staticmaps.
-        ..NOTE: will be deprecated in future versions"""
+
+        ..NOTE: will be deprecated in future versions.
+        """
         if len(self._staticmaps) > 0:
             return self.staticmaps.raster.res
 
     @property
     def transform(self):
         """Returns the geospatial transform of the model staticmaps.
-        ..NOTE: will be deprecated in future versions"""
+
+        ..NOTE: will be deprecated in future versions.
+        """
         if len(self._staticmaps) > 0:
             return self.staticmaps.raster.transform
 
     @property
     def width(self):
         """Returns the width of the model staticmaps.
-        ..NOTE: will be deprecated in future versions"""
+
+        ..NOTE: will be deprecated in future versions.
+        """
         if len(self._staticmaps) > 0:
             return self.staticmaps.raster.width
 
     @property
     def height(self):
         """Returns the height of the model staticmaps.
-        ..NOTE: will be deprecated in future versions"""
+
+        ..NOTE: will be deprecated in future versions.
+        """
         if len(self._staticmaps) > 0:
             return self.staticmaps.raster.height
 
     @property
     def shape(self) -> Tuple:
         """Returns the shape of the model staticmaps.
-        ..NOTE: will be deprecated in future versions"""
+
+        ..NOTE: will be deprecated in future versions.
+        """
         if len(self._staticmaps) > 0:
             return self.staticmaps.raster.shape
 
     @property
     def bounds(self) -> Tuple:
         """Returns the bounding box of the model region."""
         if len(self._staticmaps) > 0:
@@ -1394,54 +1535,58 @@
         """Returns the geometry of the model area of interest."""
         region = gpd.GeoDataFrame()
         if "region" in self.geoms:
             region = self.geoms["region"]
         # TODO: For now stays here but move to grid in GridModel and delete
         elif len(self.staticmaps) > 0:
             warnings.warn(
-                'Defining "region" based on staticmaps will be deprecated. Either use use region from GridModel or define your own method.',
+                'Defining "region" based on staticmaps will be deprecated. Either use'
+                " region from GridModel or define your own method.",
                 DeprecationWarning,
             )
             crs = self.staticmaps.raster.crs
             if crs is None and hasattr(crs, "to_epsg"):
                 crs = crs.to_epsg()  # not all CRS have an EPSG code
             region = gpd.GeoDataFrame(
                 geometry=[box(*self.staticmaps.raster.bounds)], crs=crs
             )
         return region
 
     # test methods
     def test_model_api(self):
+        """Test compliance with HydroMT Model API."""
         warnings.warn(
-            '"test_model_api" is now part of the internal API, use "_test_model_api" instead.',
+            '"test_model_api" is now part of the internal API, use "_test_model_api"'
+            " instead.",
             DeprecationWarning,
         )
         return self._test_model_api()
 
     def _test_model_api(self) -> List:
         """Test compliance with HydroMT Model API.
 
         Returns
         -------
         non_compliant: list
-            List of model components that are non-compliant with the model API structure.
+            List of model components that are non-compliant with the model API
+            structure.
         """
         non_compliant = []
         for component, dtype in self.api.items():
             obj = getattr(self, component, None)
             try:
                 assert obj is not None, component
                 _assert_isinstance(obj, dtype, component)
             except AssertionError as err:
                 non_compliant.append(str(err))
 
         return non_compliant
 
     def _test_equal(self, other, skip_component=["root"]) -> Tuple[bool, Dict]:
-        """Test if two models including their data components are equal
+        """Test if two models including their data components are equal.
 
         Parameters
         ----------
         other : Model (or subclass)
             Model to compare against
         skip_component: list
             List of components to skip when testing equality. By default root.
@@ -1491,15 +1636,15 @@
             data = {name: data}
     else:
         raise ValueError(f'Data type "{type(data).__name__}" not recognized')
     return data
 
 
 def _assert_isinstance(obj: Any, dtype: Any, name: str = ""):
-    """Check if obj match typing or class (dtype)"""
+    """Check if obj match typing or class (dtype)."""
     args = typing.get_args(dtype)
     _cls = typing.get_origin(dtype)
     if len(args) == 0 and dtype != Any and dtype is not None:
         assert isinstance(obj, dtype), name
     elif _cls == Union:
         assert isinstance(obj, args), name
     elif _cls is not None:
@@ -1509,15 +1654,17 @@
         for key, val in obj.items():
             _assert_isinstance(key, args[0], f"{name}.{str(key)}")
             _assert_isinstance(val, args[1], f"{name}.{str(key)}")
 
 
 def _check_equal(a, b, name="") -> Dict[str, str]:
     """Recursive test of model components.
-    Returns dict with component name and associated error message."""
+
+    Returns dict with component name and associated error message.
+    """
     errors = {}
     try:
         assert isinstance(b, type(a)), "property types do not match"
         if isinstance(a, dict):
             for key in a:
                 assert key in b, f"{key} missing"
                 errors.update(**_check_equal(a[key], b[key], f"{name}.{key}"))
```

### Comparing `hydromt-0.7.1/hydromt/models/model_lumped.py` & `hydromt-0.8.0/hydromt/models/model_lumped.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # -*- coding: utf-8 -*-
-"""HydroMT LumpedModel class definition"""
+"""HydroMT LumpedModel class definition."""
 
-import xarray as xr
-import numpy as np
-import geopandas as gpd
-import os
-from os.path import join, isfile, isdir, dirname
-from typing import Union, Optional, List, Dict
 import logging
+import os
+from os.path import dirname, isdir, isfile, join
+from typing import List, Optional, Union
+
+import geopandas as gpd
+import numpy as np
+import xarray as xr
 from shapely.geometry import box
 
 from .model_api import Model
 
 __all__ = ["LumpedModel"]
 logger = logging.getLogger(__name__)
 
@@ -74,25 +75,31 @@
 
     def read_response_units(
         self,
         fn: str = "response_units/response_units.nc",
         fn_geom: str = "response_units/response_units.geojson",
         **kwargs,
     ) -> None:
-        """Read model response units from combined netcdf file at <root>/<fn> and geojson file at <root>/<fn_geom>.
-        The netcdf file contains the attribute data and the geojson file the geometry vector data.
+        """Read model response units from combined netcdf and geojson file.
 
-        key-word arguments are passed to :py:func:`xarray.open_dataset`
+        Files are read at <root>/<fn> and geojson file at <root>/<fn_geom>.
+        The netcdf file contains the attribute data and the geojson file the geometry
+        vector data. key-word arguments are passed to :py:func:`xarray.open_dataset`
 
         Parameters
         ----------
         fn : str, optional
-            netcdf filename relative to model root, by default 'response_units/response_units.nc'
+            netcdf filename relative to model root,
+            by default 'response_units/response_units.nc'
         fn_geom : str, optional
-            geojson filename relative to model root, by default 'response_units/response_units.geojson'
+            geojson filename relative to model root,
+            by default 'response_units/response_units.geojson'
+        **kwargs:
+            Additional keyword arguments that are passed to the `RasterDatasetAdapter`
+            function.
         """
         self._assert_read_mode
         ds = xr.merge(self._read_nc(fn, **kwargs).values())
         if isfile(join(self.root, fn_geom)):
             gdf = gpd.read_file(join(self.root, fn_geom))
             # TODO: index name is hard coded. Using GeoDataset.index property once ready
             ds = ds.assign_coords(geometry=(["index"], gdf["geometry"]))
@@ -102,25 +109,32 @@
 
     def write_response_units(
         self,
         fn: str = "response_units/response_units.nc",
         fn_geom: str = "response_units/response_units.geojson",
         **kwargs,
     ):
-        """Write model response units to combined netcdf file at <root>/<fn> and geojson file at <root>/<fn_geom>.
-        The netcdf file contains the attribute data and the geojson file the geometry vector data.
+        """Write model response units to combined netcdf and geojson files.
 
-        key-word arguments are passed to :py:meth:`xarray.Dataset.to_netcdf`
+        Files are written at <root>/<fn> and at <root>/<fn_geom> respectively.
+        The netcdf file contains the attribute data and the geojson file the geometry
+        vector data. Key-word arguments are passed to
+        :py:meth:`xarray.Dataset.to_netcdf`
 
         Parameters
         ----------
         fn : str, optional
-            netcdf filename relative to model root, by default 'response_units/response_units.nc'
+            netcdf filename relative to model root,
+            by default 'response_units/response_units.nc'
         fn_geom : str, optional
-            geojson filename relative to model root, by default 'response_units/response_units.geojson'
+            geojson filename relative to model root,
+            by default 'response_units/response_units.geojson'
+        **kwargs:
+            Additional keyword arguments that are passed to the `_write_nc`
+            function.
         """
         if len(self._response_units) == 0:
             self.logger.debug("No response_units data found, skip writing.")
             return
         self._assert_write_mode
         # write geometry
         ds = self._response_units
@@ -130,15 +144,16 @@
         gdf.to_file(join(self.root, fn_geom), driver="GeoJSON")
         # _write_nc requires dict - use dummy key
         nc_dict = {"response_units": ds.drop_vars("geometry")}
         self._write_nc(nc_dict, fn, **kwargs)
 
 
 class LumpedModel(LumpedMixin, Model):
-    """Model class Lumped Model for lumped models in HydroMT"""
+
+    """Model class Lumped Model for lumped models in HydroMT."""
 
     _CLI_ARGS = {"region": "setup_region"}
     _NAME = "lumped_model"
 
     def __init__(
         self,
         root: str = None,
@@ -168,16 +183,18 @@
         ],
     ) -> None:
         """Read the complete model schematization and configuration from model files.
 
         Parameters
         ----------
         components : List, optional
-            List of model components to read, each should have an associated read_<component> method.
-            By default ['config', 'maps', 'response_units', 'geoms', 'forcing', 'states', 'results']
+            List of model components to read, each should have an
+            associated read_<component> method.
+            By default ['config', 'maps', 'response_units', 'geoms',
+            'forcing', 'states', 'results']
         """
         super().read(components=components)
 
     def write(
         self,
         components: List = [
             "config",
@@ -188,16 +205,17 @@
         ],
     ) -> None:
         """Write the complete model schematization and configuration to model files.
 
         Parameters
         ----------
         components : List, optional
-            List of model components to write, each should have an associated write_<component> method.
-            By default ['config', 'maps', 'response_units', 'geoms', 'forcing', 'states']
+            List of model components to write, each should have an
+            associated write_<component> method. By default ['config',
+            'maps', 'response_units', 'geoms', 'forcing', 'states']
         """
         super().write(components=components)
 
     @property
     def region(self) -> gpd.GeoDataFrame:
         """Returns the geometry of the model area of interest."""
         region = gpd.GeoDataFrame()
```

### Comparing `hydromt-0.7.1/hydromt/models/model_mesh.py` & `hydromt-0.8.0/hydromt/models/model_mesh.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-from typing import Union, Optional, List, Tuple
+"""Implementations for model mesh workloads."""
 import logging
 import os
-from os.path import join, isdir, dirname, isfile
+from os.path import dirname, isdir, isfile, join
 from pathlib import Path
+from typing import Dict, List, Optional, Tuple, Union
+
+import geopandas as gpd
 import numpy as np
+import pandas as pd
 import xarray as xr
 import xugrid as xu
-import geopandas as gpd
-from shapely.geometry import box, Polygon
+from shapely.geometry import box
 
+from .. import workflows
 from ..raster import GEO_MAP_COORD
 from .model_api import Model
-from .. import workflows
 
 __all__ = ["MeshModel"]
 logger = logging.getLogger(__name__)
 
 
 class MeshMixin(object):
     # placeholders
@@ -25,48 +28,57 @@
     }
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self._mesh = None
 
     ## general setup methods
-    def setup_mesh_from_raster(
+    def setup_mesh_from_rasterdataset(
         self,
-        raster_fn: str,
+        raster_fn: Union[str, Path, xr.DataArray, xr.Dataset],
         variables: Optional[list] = None,
         fill_method: Optional[str] = None,
         resampling_method: Optional[str] = "mean",
         all_touched: Optional[bool] = True,
-    ) -> None:
-        """
-        This component adds data variable(s) from ``raster_fn`` to mesh object.
+        rename: Optional[Dict] = dict(),
+    ) -> List[str]:
+        """HYDROMT CORE METHOD: Add data variable(s) from ``raster_fn`` to mesh object.
 
         Raster data is interpolated to the mesh grid using the ``resampling_method``.
-        If raster is a dataset, all variables will be added unless ``variables`` list is specified.
+        If raster is a dataset, all variables will be added unless ``variables`` list
+        is specified.
 
         Adds model layers:
 
         * **raster.name** mesh: data from raster_fn
 
         Parameters
         ----------
-        raster_fn: str
-            Source name of raster data in data_catalog.
+        raster_fn: str, Path, xr.DataArray, xr.Dataset
+            Data catalog key, path to raster file or raster xarray data object.
         variables: list, optional
             List of variables to add to mesh from raster_fn. By default all.
         fill_method : str, optional
-            If specified, fills no data values using fill_nodata method. AVailable methods
-            are {'linear', 'nearest', 'cubic', 'rio_idw'}.
+            If specified, fills no data values using fill_nodata method.
+            Available methods are {'linear', 'nearest', 'cubic', 'rio_idw'}.
         resampling_method: str, optional
             Method to sample from raster data to mesh. By default mean. Options include
             {'count', 'min', 'max', 'sum', 'mean', 'std', 'median', 'q##'}.
         all_touched : bool, optional
             If True, all pixels touched by geometries will used to define the sample.
             If False, only pixels whose center is within the geometry or that are
             selected by Bresenham's line algorithm will be used. By default True.
+        rename: dict, optional
+            Dictionary to rename variable names in raster_fn before adding to mesh
+            {'name_in_raster_fn': 'name_in_mesh'}. By default empty.
+
+        Returns
+        -------
+        list
+            List of variables added to mesh.
         """
         self.logger.info(f"Preparing mesh data from raster source {raster_fn}")
         # Read raster data and select variables
         ds = self.data_catalog.get_rasterdataset(
             raster_fn, geom=self.region, buffer=2, variables=variables
         )
         if isinstance(ds, xr.DataArray):
@@ -78,66 +90,92 @@
         # Convert mesh grid as geodataframe for sampling
         # Reprojection happens to gdf inside of zonal_stats method
         ds_sample = ds.raster.zonal_stats(
             gdf=self.mesh_gdf, stats=resampling_method, all_touched=all_touched
         )
         # Rename variables
         rm_dict = {f"{var}_{resampling_method}": var for var in ds.data_vars}
-        ds_sample = ds_sample.rename(rm_dict)
+        ds_sample = ds_sample.rename(rm_dict).rename(rename)
         # Convert to UgridDataset
         uds_sample = xu.UgridDataset(ds_sample, grids=self.mesh.ugrid.grid)
 
         self.set_mesh(uds_sample)
 
+        return list(ds_sample.data_vars.keys())
+
     def setup_mesh_from_raster_reclass(
         self,
-        raster_fn: str,
-        reclass_table_fn: str,
+        raster_fn: Union[str, Path, xr.DataArray],
+        reclass_table_fn: Union[str, Path, pd.DataFrame],
         reclass_variables: list,
         variable: Optional[str] = None,
         fill_nodata: Optional[str] = None,
         resampling_method: Optional[Union[str, list]] = "mean",
         all_touched: Optional[bool] = True,
+        rename: Optional[Dict] = dict(),
         **kwargs,
-    ) -> None:
-        """
-        This component adds data variable(s) to mesh object by reclassifying the data in ``raster_fn`` based on ``reclass_table_fn``.
+    ) -> List[str]:
+        """HYDROMT CORE METHOD: Add data variable(s) to mesh object by reclassifying the data in ``raster_fn`` based on ``reclass_table_fn``.
 
-        The reclassified raster data are subsequently interpolated to the mesh using ``resampling_method``.
+        The reclassified raster data
+        are subsequently interpolated to the mesh using `resampling_method`.
 
         Adds model layers:
 
-        * **reclass_variables** mesh: reclassified raster data interpolated to the model mesh
+        * **reclass_variables** mesh: reclassified raster data interpolated to the
+            model mesh
 
         Parameters
         ----------
-        raster_fn: str
-            Source name of raster data in data_catalog. Should be a DataArray. Else use **kwargs to select variables/time_tuple in
-            :py:meth:`hydromt.data_catalog.get_rasterdataset` method
-        reclass_table_fn: str
-            Source name of reclassification table of raster_fn in data_catalog.
-        reclass_variables: list
-            List of reclass_variables from reclass_table_fn table to add to mesh. Index column should match values in raster_fn.
-        variable: str, optional
-            Name of raster dataset variable to use. This is only required when reading datasets with multiple variables.
-            By default None.
-        fill_method : str, optional
-            If specified, fills nodata values in `raster_fn` using fill_nodata method before reclassifying.
-            Available methods are {'linear', 'nearest', 'cubic', 'rio_idw'}.
-        resampling_method: str, list, optional
-            Method to sample from raster data to mesh. Can be a list per variable in ``reclass_variables`` or a
-            single method for all. By default mean for all reclass_variables.
-            Options include {'count', 'min', 'max', 'sum', 'mean', 'std', 'median', 'q##'}.
+        raster_fn : str, Path, xr.DataArray
+            Data catalog key, path to the raster file, or raster xarray data object.
+            Should be a DataArray. If not, use the `variable` argument for selection.
+        reclass_table_fn : str, Path, pd.DataFrame
+            Data catalog key, path to the tabular data file, or tabular pandas dataframe
+            object for the reclassification table of `raster_fn`.
+        reclass_variables : list
+            List of reclass_variables from the reclass_table_fn table to add to the
+            mesh. The index column should match values in raster_fn.
+        variable : str, optional
+            Name of the raster dataset variable to use. This is only required when
+            reading datasets with multiple variables. By default, None.
+        fill_nodata : str, optional
+            If specified, fills nodata values in `raster_fn` using the `fill_nodata`
+            method before reclassifying. Available methods are
+            {'linear', 'nearest', 'cubic', 'rio_idw'}.
+        resampling_method : str or list, optional
+            Method to sample from raster data to the mesh. Can be a list per variable
+            in `reclass_variables` or a single method for all. By default, 'mean' is
+            used for all `reclass_variables`. Options include {'count', 'min', 'max',
+            'sum', 'mean', 'std', 'median', 'q##'}.
         all_touched : bool, optional
-            If True, all pixels touched by geometries will used to define the sample.
+            If True, all pixels touched by geometries will be used to define the sample.
             If False, only pixels whose center is within the geometry or that are
-            selected by Bresenham's line algorithm will be used. By default True.
-        """
+            selected by Bresenham's line algorithm will be used. By default, True.
+        rename : dict, optional
+            Dictionary to rename variable names in `reclass_variables` before adding
+            them to the mesh. The dictionary should have the form
+            {'name_in_reclass_table': 'name_in_mesh'}. By default, an empty dictionary.
+        **kwargs : dict
+            Additional keyword arguments to be passed to the raster dataset
+            retrieval method.
+
+        Returns
+        -------
+        variable_names : List[str]
+            List of added variable names in the mesh.
+
+        Raises
+        ------
+        ValueError
+            If `raster_fn` is not a single variable raster.
+        """  # noqa: E501
         self.logger.info(
-            f"Preparing mesh data by reclassifying the data in {raster_fn} based on {reclass_table_fn}."
+            f"Preparing mesh data by reclassifying the data in {raster_fn} "
+            f"based on {reclass_table_fn}."
         )
         # Read raster data and mapping table
         da = self.data_catalog.get_rasterdataset(
             raster_fn, geom=self.region, buffer=2, variables=variable, **kwargs
         )
         if not isinstance(da, xr.DataArray):
             raise ValueError(
@@ -145,15 +183,15 @@
                 "Please select one using the 'variable' argument"
             )
         df_vars = self.data_catalog.get_dataframe(
             reclass_table_fn, variables=reclass_variables
         )
 
         if fill_nodata is not None:
-            ds = ds.raster.interpolate_na(method=fill_nodata)
+            da = da.raster.interpolate_na(method=fill_nodata)
 
         # Mapping function
         ds_vars = da.raster.reclassify(reclass_table=df_vars, method="exact")
 
         # Convert mesh grid as geodataframe for sampling
         # Reprojection happens to gdf inside of zonal_stats method
         ds_sample = ds_vars.raster.zonal_stats(
@@ -164,21 +202,23 @@
         # Rename variables
         if isinstance(resampling_method, str):
             resampling_method = np.repeat(resampling_method, len(reclass_variables))
         rm_dict = {
             f"{var}_{mtd}": var
             for var, mtd in zip(reclass_variables, resampling_method)
         }
-        ds_sample = ds_sample.rename(rm_dict)
+        ds_sample = ds_sample.rename(rm_dict).rename(rename)
         ds_sample = ds_sample[reclass_variables]
         # Convert to UgridDataset
         uds_sample = xu.UgridDataset(ds_sample, grids=self.mesh.ugrid.grid)
 
         self.set_mesh(uds_sample)
 
+        return list(ds_sample.data_vars.keys())
+
     @property
     def mesh(self) -> Union[xu.UgridDataArray, xu.UgridDataset]:
         """Model static mesh data. Returns a xarray.Dataset."""
         # XU grid data type Xarray dataset with xu sampling.
         if self._mesh is None and self._read:
             self.read_mesh()
         return self._mesh
@@ -193,19 +233,21 @@
         All layers of mesh have identical spatial coordinates in Ugrid conventions.
 
         Parameters
         ----------
         data: xugrid.UgridDataArray or xugrid.UgridDataset
             new layer to add to mesh
         name: str, optional
-            Name of new object layer, this is used to overwrite the name of a UgridDataArray.
+            Name of new object layer, this is used to overwrite the name of
+            a UgridDataArray.
         """
         if not isinstance(data, (xu.UgridDataArray, xu.UgridDataset)):
             raise ValueError(
-                "New mesh data in set_mesh should be of type xu.UgridDataArray or xu.UgridDataset"
+                "New mesh data in set_mesh should be of type xu.UgridDataArray"
+                " or xu.UgridDataset"
             )
         if isinstance(data, xu.UgridDataArray):
             if name is not None:
                 data = data.rename(name)
             elif data.name is None:
                 raise ValueError(
                     f"Cannot set mesh from {str(type(data).__name__)} without a name."
@@ -216,60 +258,65 @@
         else:
             for dvar in data.data_vars:
                 if dvar in self._mesh:
                     self.logger.warning(f"Replacing mesh parameter: {dvar}")
                 self._mesh[dvar] = data[dvar]
 
     def read_mesh(self, fn: str = "mesh/mesh.nc", **kwargs) -> None:
-        """Read model mesh data at <root>/<fn> and add to mesh property
+        """Read model mesh data at <root>/<fn> and add to mesh property.
 
         key-word arguments are passed to :py:func:`xr.open_dataset`
 
         Parameters
         ----------
         fn : str, optional
             filename relative to model root, by default 'mesh/mesh.nc'
+        **kwargs : dict
+            Additional keyword arguments to be passed to the `_read_nc` method.
         """
         self._assert_read_mode
         for ds in self._read_nc(fn, **kwargs).values():
             uds = xu.UgridDataset(ds)
             if ds.rio.crs is not None:  # parse crs
                 uds.ugrid.grid.set_crs(ds.raster.crs)
                 uds = uds.drop_vars(GEO_MAP_COORD, errors="ignore")
             self.set_mesh(uds)
 
     def write_mesh(self, fn: str = "mesh/mesh.nc", **kwargs) -> None:
-        """Write model grid data to netcdf file at <root>/<fn>
+        """Write model grid data to a netCDF file at <root>/<fn>.
 
-        key-word arguments are passed to :py:meth:`xarray.Dataset.ugrid.to_netcdf`
+        Keyword arguments are passed to :py:meth:`xarray.Dataset.ugrid.to_netcdf`.
 
         Parameters
         ----------
         fn : str, optional
-            filename relative to model root, by default 'grid/grid.nc'
+            Filename relative to the model root directory, by default 'grid/grid.nc'.
+        **kwargs : dict
+            Additional keyword arguments to be passed to the
+            `xarray.Dataset.ugrid.to_netcdf` method.
         """
         if self._mesh is None:
             self.logger.debug("No mesh data found, skip writing.")
             return
         self._assert_write_mode
         # filename
         _fn = join(self.root, fn)
         if not isdir(dirname(_fn)):
             os.makedirs(dirname(_fn))
         self.logger.debug(f"Writing file {fn}")
-        # ds_new = xu.UgridDataset(grid=ds_out.ugrid.grid) # bug in xugrid?
         ds_out = self.mesh.ugrid.to_dataset()
         if self.mesh.ugrid.grid.crs is not None:
             # save crs to spatial_ref coordinate
             ds_out = ds_out.rio.write_crs(self.mesh.ugrid.grid.crs)
         ds_out.to_netcdf(_fn, **kwargs)
 
 
 class MeshModel(MeshMixin, Model):
-    """Model class Mesh Model for mesh models in HydroMT"""
+
+    """Model class Mesh Model for mesh models in HydroMT."""
 
     _CLI_ARGS = {"region": "setup_mesh", "res": "setup_mesh"}
     _NAME = "mesh_model"
 
     def __init__(
         self,
         root: str = None,
@@ -290,17 +337,19 @@
     ## general setup methods
     def setup_mesh(
         self,
         region: dict,
         res: Optional[float] = None,
         crs: int = None,
     ) -> xu.UgridDataset:
-        """Creates an 2D unstructured mesh or reads an existing 2D mesh according UGRID conventions.
-        An 2D unstructured mesh will be created as 2D rectangular grid from a geometry (geom_fn) or bbox. If an existing
-        2D mesh is given, then no new mesh will be generated
+        """HYDROMT CORE METHOD: Create an 2D unstructured mesh or reads an existing 2D mesh according UGRID conventions.
+
+        Grids are read according to UGRID conventions. An 2D unstructured mesh
+        will be created as 2D rectangular grid from a geometry (geom_fn) or bbox.
+        If an existing 2D mesh is given, then no new mesh will be generated
 
         Note Only existing meshed with only 2D grid can be read.
         #FIXME: read existing 1D2D network file and extract 2D part.
 
         Adds/Updates model layers:
 
         * **mesh** mesh topology: add mesh topology to mesh object
@@ -312,40 +361,43 @@
 
             * {'bbox': [xmin, ymin, xmax, ymax]}
 
             * {'geom': 'path/to/polygon_geometry'}
 
             * {'mesh': 'path/to/2dmesh_file'}
         res: float
-            Resolution used to generate 2D mesh [unit of the CRS], required if region is not based on 'mesh'.
+            Resolution used to generate 2D mesh [unit of the CRS], required if region
+            is not based on 'mesh'.
         crs : EPSG code, int, optional
-            Optional EPSG code of the model. If None using the one from region, and else 4326.
+            Optional EPSG code of the model. If None using the one from region,
+            and else 4326.
 
         Returns
         -------
         mesh2d : xu.UgridDataset
             Generated mesh2d.
 
-        """
-        self.logger.info(f"Preparing 2D mesh.")
+        """  # noqa: E501
+        self.logger.info("Preparing 2D mesh.")
 
         if "mesh" not in region:
             if not isinstance(res, (int, float)):
                 raise ValueError("res argument required")
             kind, region = workflows.parse_region(region, logger=self.logger)
             if kind == "bbox":
                 bbox = region["bbox"]
                 geom = gpd.GeoDataFrame(geometry=[box(*bbox)], crs=4326)
             elif kind == "geom":
                 geom = region["geom"]
                 if geom.crs is None:
                     raise ValueError('Model region "geom" has no CRS')
             else:
                 raise ValueError(
-                    f"Region for mesh must of kind [bbox, geom, mesh], kind {kind} not understood."
+                    f"Region for mesh must of kind [bbox, geom, mesh], kind {kind} "
+                    "not understood."
                 )
             if crs is not None:
                 geom = geom.to_crs(crs)
             # Generate grid based on res for region bbox
             xmin, ymin, xmax, ymax = geom.total_bounds
             # note we flood the number of faces within bounds
             ncol = int((xmax - xmin) // res)
@@ -361,26 +413,26 @@
                     faces.append(box(left, bottom, right, top))
             grid = gpd.GeoDataFrame(geometry=faces, crs=geom.crs)
             # If needed clip to geom
             if kind != "bbox":
                 # TODO: grid.intersects(geom) does not seem to work ?
                 grid = grid.loc[
                     gpd.sjoin(
-                        grid, geom, how="left", op="intersects"
+                        grid, geom, how="left", predicate="intersects"
                     ).index_right.notna()
                 ].reset_index()
             # Create mesh from grid
             grid.index.name = "mesh2d_nFaces"
             mesh2d = xu.UgridDataset.from_geodataframe(grid)
             mesh2d.ugrid.grid.set_crs(grid.crs)
 
         else:
             mesh2d_fn = region["mesh"]
             if isinstance(mesh2d_fn, (str, Path)) and isfile(mesh2d_fn):
-                self.logger.info(f"An existing 2D grid is used to prepare 2D mesh.")
+                self.logger.info("An existing 2D grid is used to prepare 2D mesh.")
 
                 ds = xr.open_dataset(mesh2d_fn, mask_and_scale=False)
             elif isinstance(mesh2d_fn, xr.Dataset):
                 ds = mesh2d_fn
             else:
                 raise ValueError(
                     f"Region 'mesh' file {mesh2d_fn} not found, please check"
@@ -388,42 +440,44 @@
             topologies = [
                 k for k in ds.data_vars if ds[k].attrs.get("cf_role") == "mesh_topology"
             ]
             for topology in topologies:
                 topodim = ds[topology].attrs["topology_dimension"]
                 if topodim != 2:  # chek if 2d mesh file else throw error
                     raise NotImplementedError(
-                        f"{mesh2d_fn} cannot be opened. Please check if the existing grid is "
-                        f"an 2D mesh and not 1D2D mesh. This option is not yet available for 1D2D meshes."
+                        f"{mesh2d_fn} cannot be opened. Please check if the existing"
+                        " grid is an 2D mesh and not 1D2D mesh. "
+                        " This option is not yet available for 1D2D meshes."
                     )
 
             # Continues with a 2D grid
             mesh2d = xu.UgridDataset(ds)
             # Check crs and reproject to model crs
             if crs is None:
                 crs = 4326
             if ds.rio.crs is not None:  # parse crs
                 mesh2d.ugrid.grid.set_crs(ds.raster.crs)
             else:
                 # Assume model crs
                 self.logger.warning(
-                    f"Mesh data from {mesh2d_fn} doesn't have a CRS. Assuming crs option {crs}"
+                    f"Mesh data from {mesh2d_fn} doesn't have a CRS."
+                    f" Assuming crs option {crs}"
                 )
                 mesh2d.ugrid.grid.set_crs(crs)
             mesh2d = mesh2d.drop_vars(GEO_MAP_COORD, errors="ignore")
 
         # Reproject to user crs option if needed
         if mesh2d.ugrid.grid.crs != crs and crs is not None:
             self.logger.info(f"Reprojecting mesh to crs {crs}")
             mesh2d.ugrid.grid.to_crs(self.crs)
 
         self.set_mesh(mesh2d)
 
-        # This setup method returns region so that it can be wrapped for models which require
-        # more information
+        # This setup method returns region so that it can be wrapped for models
+        # which require more information
         return mesh2d
 
     ## I/O
     def read(
         self,
         components: List = [
             "config",
@@ -435,30 +489,32 @@
         ],
     ) -> None:
         """Read the complete model schematization and configuration from model files.
 
         Parameters
         ----------
         components : List, optional
-            List of model components to read, each should have an associated read_<component> method.
-            By default ['config', 'maps', 'mesh', 'geoms', 'forcing', 'states', 'results']
+            List of model components to read, each should have an associated
+            read_<component> method. By default ['config', 'maps', 'mesh',
+            'geoms', 'forcing', 'states', 'results']
         """
         super().read(components=components)
 
     def write(
         self,
         components: List = ["config", "mesh", "geoms", "forcing", "states"],
     ) -> None:
         """Write the complete model schematization and configuration to model files.
 
         Parameters
         ----------
         components : List, optional
-            List of model components to write, each should have an associated write_<component> method.
-            By default ['config', 'maps', 'mesh', 'geoms', 'forcing', 'states']
+            List of model components to write, each should have an
+            associated write_<component> method. By default ['config', 'maps',
+            'mesh', 'geoms', 'forcing', 'states']
         """
         super().write(components=components)
 
     # MeshModel specific methods
 
     # MeshModel properties
     @property
@@ -478,11 +534,11 @@
             if crs is None and hasattr(crs, "to_epsg"):
                 crs = crs.to_epsg()  # not all CRS have an EPSG code
             region = gpd.GeoDataFrame(geometry=[box(*self.bounds)], crs=crs)
         return region
 
     @property
     def mesh_gdf(self) -> gpd.GeoDataFrame:
-        """Returns geometry of mesh as a gpd.GeoDataFrame"""
+        """Returns geometry of mesh as a gpd.GeoDataFrame."""
         if self._mesh is not None:
             name = [n for n in self.mesh.data_vars][0]  # works better on a DataArray
             return self._mesh[name].ugrid.to_geodataframe()
```

### Comparing `hydromt-0.7.1/hydromt/models/model_network.py` & `hydromt-0.8.0/hydromt/models/model_network.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 # -*- coding: utf-8 -*-
-"""HydroMT NetworkModel class definition"""
+"""HydroMT NetworkModel class definition."""
 
-import xarray as xr
 import logging
 from typing import List
+
+import xarray as xr
+
 from .model_api import Model
 
 __all__ = ["NetworkModel"]
 logger = logging.getLogger(__name__)
 
 
 class NetworkModel(Model):
+
+    """Implementation for the network models."""
+
     _CLI_ARGS = {"region": "setup_region"}
     _NAME = "network_model"
 
     def __init__(
         self,
         root: str = None,
         mode: str = "w",
@@ -47,16 +52,17 @@
         ],
     ) -> None:
         """Read the complete model schematization and configuration from model files.
 
         Parameters
         ----------
         components : List, optional
-            List of model components to read, each should have an associated read_<component> method.
-            By default ['config', 'maps', 'network', 'geoms', 'forcing', 'states', 'results']
+            List of model components to read, each should have an associated
+            read_<component> method. By default ['config', 'maps',
+            'network', 'geoms', 'forcing', 'states', 'results']
         """
         super().read(components=components)
 
     def write(
         self,
         components: List = [
             "config",
@@ -67,25 +73,26 @@
         ],
     ) -> None:
         """Write the complete model schematization and configuration to model files.
 
         Parameters
         ----------
         components : List, optional
-            List of model components to write, each should have an associated write_<component> method.
-            By default ['config', 'maps', 'network', 'geoms', 'forcing', 'states']
+            List of model components to write, each should have an
+            associated write_<component> method. By default ['config', 'maps',
+            'network', 'geoms', 'forcing', 'states']
         """
         super().write(components=components)
 
     # TODO: make NetworkMixin class with following properties/methods
     @property
-    def network(self):
+    def network(self):  # noqa: D102
         raise NotImplementedError()
 
-    def set_network(self):
+    def set_network(self):  # noqa: D102
         raise NotImplementedError()
 
-    def read_network(self):
+    def read_network(self):  # noqa: D102
         raise NotImplementedError()
 
-    def write_network(self):
+    def write_network(self):  # noqa: D102
         raise NotImplementedError()
```

### Comparing `hydromt-0.7.1/hydromt/models/model_plugins.py` & `hydromt-0.8.0/hydromt/models/model_plugins.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from entrypoints import EntryPoint, Distribution, get_group_all
+"""Implementation of the mechanism to access the plugin entrypoints."""
 import logging
 from typing import Dict, Iterator, List
-from .. import __version__
+
+from entrypoints import Distribution, EntryPoint, get_group_all
+
+from .. import __version__, _compat
 from .model_api import Model
-from .. import _compat
 
 logger = logging.getLogger(__name__)
 
 __all__ = ["ModelCatalog"]
 
 # local generic models
 LOCAL_EPS = {
@@ -15,15 +17,15 @@
     "lumped_model": "hydromt.models.model_lumped:LumpedModel",
     "mesh_model": "hydromt.models.model_mesh:MeshModel",
     "network_model": "hydromt.models.model_network:NetworkModel",
 }
 
 
 def get_general_eps() -> Dict:
-    """Get local hydromt generic model class entrypoints
+    """Get local hydromt generic model class entrypoints.
 
     Returns
     -------
     eps : dict
         Entrypoints dict
     """
     eps = {}
@@ -32,52 +34,59 @@
         if name == "mesh_model" and not _compat.HAS_XUGRID:
             continue
         eps[name] = EntryPoint.from_string(epstr, name, distro)
     return eps
 
 
 def _discover(path=None) -> List:
-    """Discover drivers via entrypoints"""
+    """Discover drivers via entrypoints."""
     return get_group_all("hydromt.models", path=path)
 
 
 def get_plugin_eps(path=None, logger=logger) -> Dict:
-    """Discover hydromt model plugins based on 'hydromt.models' entrypoints
+    """Discover hydromt model plugins based on 'hydromt.models' entrypoints.
 
     Parameters
     ----------
     path : str or None
         Default is ``sys.path``.
+    logger : logger object, optional
+        The logger object used for logging messages. If not provided, the default
+        logger will be used.
 
     Returns
     -------
     eps : dict
         Entrypoints dict
     """
     eps = {}
     for ep in _discover():
         name = ep.name
         if name in eps or name in LOCAL_EPS:
             plugin = f"{ep.module_name}.{ep.object_name}"
             logger.warning(f"Duplicated model plugin '{name}'; skipping {plugin}")
             continue
         logger.debug(
-            f"Discovered model plugin '{name} = {ep.module_name}.{ep.object_name}' ({ep.distro.version})"
+            f"Discovered model plugin '{name} = {ep.module_name}.{ep.object_name}' "
+            f"({ep.distro.version})"
         )
         eps[ep.name] = ep
     return eps
 
 
 def load(ep, logger=logger) -> Model:
-    """Load entrypoint and return plugin model class
+    """Load entrypoint and return plugin model class.
 
     Parameters
     ----------
     ep : entrypoint
         discovered entrypoint
+    logger : logger object, optional
+        The logger object used for logging messages. If not provided, the default
+        logger will be used.
 
     Returns
     -------
     model_class : Model
         plugin model class
     """
     _str = f"{ep.name} = {ep.module_name}.{ep.object_name}"
@@ -88,71 +97,82 @@
         logger.debug(f"Loaded model plugin {_str}")
         return model_class
     except (ModuleNotFoundError, AttributeError) as err:
         raise ImportError(f"Error while loading model plugin '{_str}' ({err})")
 
 
 class ModelCatalog:
+
+    """The model catalogue provides access to plugins and their Model classes."""
+
     def __init__(self):
+        """Initiate the catalog object."""
         self._eps = {}  # entrypoints
         self._cls = {}  # classes
         self._plugins = []  # names of plugins
         self._general = []  # names of local model classes
 
     @property
     def eps(self) -> Dict:
-        """Returns dictionary with available model entrypoints."""
+        """Return dictionary with available model entrypoints."""
         if len(self._eps) == 0:
             self.plugins  # discover plugins
             self.generic  # get generic local model classes
         return self._eps
 
     @property
     def cls(self) -> Dict:
-        """Returns dictionary with available model classes."""
+        """Return dictionary with available model classes."""
         if len(self._cls) != len(self.eps):
             for name in self.eps:
                 if name not in self._cls:
                     self._cls[name] = load(self.eps[name])
         return self._cls
 
     @property
     def plugins(self) -> List:
-        """Returns list with names of model plugins"""
+        """Return list with names of model plugins."""
         if len(self._plugins) == 0:
             eps = get_plugin_eps()
             self._plugins = list(eps.keys())
             self._eps.update(**eps)
         return self._plugins
 
     @property
     def generic(self) -> List:
-        """Returns list with names of generic models"""
+        """Return list with names of generic models."""
         if len(self._general) == 0:
             eps = get_general_eps()
             self._general = list(eps.keys())
             self._eps.update(**eps)
         return self._general
 
     def load(self, name) -> Model:
-        """Returns model class"""
+        """Return model class."""
         if name not in self._cls:
             self._cls[name] = load(self[name])
         return self._cls[name]
 
     def __str__(self):
+        """Generate string representation containing the registered entrypoints."""
         plugins = "".join(
             [
-                f" - {name} ({self.eps[name].distro.name} {self.eps[name].distro.version})\n"
+                f" - {name} ({self.eps[name].distro.name}"
+                f" {self.eps[name].distro.version})\n"
                 for name in self.plugins
             ]
         )
         generic = "".join([f" - {name}\n" for name in self.generic])
-        return f"model plugins:\n{plugins}generic models (hydromt {__version__}):\n{generic}"
+        return (
+            f"model plugins:\n{plugins}generic models (hydromt {__version__})"
+            f":\n{generic}"
+        )
 
     def __getitem__(self, name) -> Model:
+        """Return the entrypoint with the provided name."""
         if name not in self.eps:
             raise ValueError(f"Unknown model {name}; select from {self.eps.keys()}")
         return self._eps[name]
 
     def __iter__(self) -> Iterator:
+        """Return an iterator over registered entrypoints."""
         return iter(self.eps)
```

### Comparing `hydromt-0.7.1/hydromt/raster.py` & `hydromt-0.8.0/hydromt/raster.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Credits: This script is based on the rioxarray package (Apache License, Version 2.0)
 # source file: https://github.com/corteva/rioxarray
 # license file: https://github.com/corteva/rioxarray/blob/master/LICENSE
 
-"""
-This module is an extension for xarray to provide rasterio capabilities
-to xarray datasets/dataarrays.
-"""
+"""Extension for xarray to provide rasterio capabilities to xarray datasets/arrays."""
 from __future__ import annotations
+
+import logging
+import math
 import os
-import sys
-from os.path import join, basename, dirname, isdir
-from typing import Any, Optional
+import tempfile
+from itertools import product
+from os.path import basename, dirname, isdir, join
+from typing import Any, Optional, Union
+
+import dask
+import geopandas as gpd
 import numpy as np
-from shapely.geometry import box, Polygon
 import pandas as pd
-import geopandas as gpd
+import pyproj
+import rasterio.fill
+import rasterio.warp
+import rioxarray  # noqa: F401
+import shapely
 import xarray as xr
-import dask
+import yaml
 from affine import Affine
 from pyproj import CRS
-from itertools import product
-import rasterio.warp
-import rasterio.fill
 from rasterio import features
-from rasterio.enums import Resampling
-from scipy.spatial import cKDTree
-from scipy.interpolate import griddata
+from rasterio.enums import MergeAlg, Resampling
 from scipy import ndimage
-import tempfile
-import pyproj
-import logging
-import yaml
-import rioxarray
-import math
-from . import gis_utils, _compat
+from scipy.interpolate import griddata
+from scipy.spatial import cKDTree
+from shapely.geometry import LineString, Polygon, box
+
+from . import _compat, gis_utils
 
 logger = logging.getLogger(__name__)
 XDIMS = ("x", "longitude", "lon", "long")
 YDIMS = ("y", "latitude", "lat")
 GEO_MAP_COORD = "spatial_ref"
 
 
@@ -146,26 +146,39 @@
     dtype=np.float32,
     name=None,
     attrs={},
     crs=None,
     lazy=False,
 ):
     """Return a full DataArray based on a geospatial transform and shape.
+
     See :py:meth:`~hydromt.raster.full` for all options.
 
-    Arguments
-    ---------
+    Parameters
+    ----------
     transform : affine transform
-        Two dimensional affine transform for 2D linear mapping
-    shape: tuple of int
+        Two dimensional affine transform for 2D linear mapping.
+    shape : tuple of int
         Length along (dim0, x, y) dimensions, of which the first is optional.
+    nodata : optional
+        The nodata value to assign to the DataArray. Defaults to np.nan.
+    dtype : optional
+        The data type to use for the DataArray. Defaults to np.float32.
+    name : optional
+        The name of the DataArray. Defaults to None.
+    attrs : optional
+        Additional attributes to assign to the DataArray. Empty by default.
+    crs : optional
+        The coordinate reference system (CRS) of the DataArray. Defaults to None.
+    lazy : bool, optional
+        Whether to create a lazy DataArray. Defaults to False.
 
     Returns
     -------
-    da: DataArray
+    da : DataArray
         Filled DataArray
     """
     if len(shape) not in [2, 3]:
         raise ValueError("Only 2D and 3D data arrays supported.")
     coords = gis_utils.affine_to_coords(transform, shape[-2:], x_dim="x", y_dim="y")
     dims = ("y", "x")
     if len(shape) == 3:
@@ -182,52 +195,59 @@
         shape=shape,
         dims=dims,
     )
     return da
 
 
 class XGeoBase(object):
-    """This is the base class for the GIS extensions for xarray"""
+
+    """Base class for the GIS extensions for xarray."""
 
     def __init__(self, xarray_obj: xr.DataArray | xr.Dataset) -> None:
+        """Initialize new object based on the xarray object provided."""
         self._obj = xarray_obj
         # create new coordinate with attributes in which to save x_dim, y_dim and crs.
-        # other spatial properties are always calculated on the fly to ensure consistency with data
+        # other spatial properties are always calculated on the fly to ensure
+        # consistency with data
         if GEO_MAP_COORD not in self._obj.coords:
             # zero is used by rioxarray
             self._obj.coords[GEO_MAP_COORD] = xr.Variable((), 0)
 
     @property
     def attrs(self) -> dict:
-        """Return dictionary of spatial attributes"""
+        """Return dictionary of spatial attributes."""
         return self._obj.coords[GEO_MAP_COORD].attrs
 
     def set_attrs(self, **kwargs) -> None:
         """Update spatial attributes. Usage raster.set_attr(key=value)."""
         self._obj.coords[GEO_MAP_COORD].attrs.update(**kwargs)
 
     def get_attrs(self, key, placeholder=None) -> Any:
         """Return single spatial attribute."""
         return self._obj.coords[GEO_MAP_COORD].attrs.get(key, placeholder)
 
     @property
     def crs(self) -> CRS:
-        """Return Coordinate Reference System as :py:meth:`pyproj.CRS` object."""
+        """Return horizontal Coordinate Reference System."""
+        # return horizontal crs by default to avoid errors downstream
+        # with reproject / rasterize etc.
         if "crs_wkt" not in self.attrs:
             self.set_crs()
         if "crs_wkt" in self.attrs:
-            return pyproj.CRS.from_user_input(self.attrs["crs_wkt"])
+            crs = pyproj.CRS.from_user_input(self.attrs["crs_wkt"])
+            return crs
 
     def set_crs(self, input_crs=None):
         """Set the Coordinate Reference System.
 
         Arguments
-        ----------
+        ---------
         input_crs: int, dict, or str, optional
-            Coordinate Reference System. Accepts EPSG codes (int or str); proj (str or dict)
+            Coordinate Reference System. Accepts EPSG codes (int or str)
+            and proj (str or dict)
         """
         crs_names = ["crs_wkt", "crs", "epsg"]
         names = list(self._obj.coords.keys())
         if isinstance(self._obj, xr.Dataset):
             names = names + list(self._obj.data_vars.keys())
         # user defined
         if input_crs is not None:
@@ -245,47 +265,49 @@
                         break
                 if crs is not None:
                     # avoid Warning 1: +init=epsg:XXXX syntax is deprecated
                     crs = crs.strip("+init=") if isinstance(crs, str) else crs
                     try:
                         input_crs = pyproj.CRS.from_user_input(crs)
                         break
-                    except:
+                    except RuntimeError:
                         pass
         if input_crs is not None:
             grid_map_attrs = input_crs.to_cf()
             crs_wkt = input_crs.to_wkt()
             grid_map_attrs["spatial_ref"] = crs_wkt
             grid_map_attrs["crs_wkt"] = crs_wkt
             self.set_attrs(**grid_map_attrs)
 
 
 class XRasterBase(XGeoBase):
-    """This is the base class for a Raster GIS extensions for xarray"""
+
+    """Base class for a Raster GIS extensions for xarray."""
 
     def __init__(self, xarray_obj):
+        """Initialize new object based on the xarray object provided."""
         super(XRasterBase, self).__init__(xarray_obj)
 
     @property
     def x_dim(self) -> str:
-        """Return the x dimension name"""
+        """Return the x dimension name."""
         if self.get_attrs("x_dim") not in self._obj.dims:
             self.set_spatial_dims()
         return self.attrs["x_dim"]
 
     @property
     def y_dim(self) -> str:
-        """Return the y dimension name"""
+        """Return the y dimension name."""
         if self.get_attrs("y_dim") not in self._obj.dims:
             self.set_spatial_dims()
         return self.attrs["y_dim"]
 
     @property
     def xcoords(self) -> xr.IndexVariable:
-        """Return the x coordinates"""
+        """Return the x coordinates."""
         xcoords = self._obj[self.x_dim]
         if self.x_dim not in self._obj.coords:
             for key in list(self._obj.coords.keys()):
                 if key.startswith(self.x_dim):
                     xcoords = self._obj.coords[key]
                     break
         if xcoords.ndim == 2 and list(xcoords.dims).index(self.x_dim) != 1:
@@ -295,15 +317,15 @@
             )
         if xcoords.size < 2 or (xcoords.ndim == 2 and xcoords.shape[1] < 2):
             raise ValueError(f"Invalid raster: less than 2 cells in x_dim {self.x_dim}")
         return xcoords
 
     @property
     def ycoords(self) -> xr.IndexVariable:
-        """Return the y coordinates"""
+        """Return the y coordinates."""
         ycoords = self._obj[self.y_dim]
         if self.y_dim not in self._obj.coords:
             for key in list(self._obj.coords.keys()):
                 if key.startswith(self.y_dim):
                     ycoords = self._obj.coords[key]
                     break
         if ycoords.ndim == 2 and list(ycoords.dims).index(self.y_dim) != 0:
@@ -315,38 +337,42 @@
             raise ValueError(f"Invalid raster: less than 2 cells in y_dim {self.y_dim}")
         return ycoords
 
     def set_spatial_dims(self, x_dim=None, y_dim=None) -> None:
         """Set the geospatial dimensions of the object.
 
         Arguments
-        ----------
+        ---------
         x_dim: str, optional
             The name of the x dimension.
         y_dim: str, optional
             The name of the y dimension.
         """
         _dims = list(self._obj.dims)
+        # Switch to lower case to compare to XDIMS and YDIMS
+        _dimslow = [d.lower() for d in _dims]
         if x_dim is None:
             for dim in XDIMS:
-                if dim in _dims:
-                    x_dim = dim
+                if dim in _dimslow:
+                    idim = _dimslow.index(dim)
+                    x_dim = _dims[idim]
                     break
         if x_dim and x_dim in _dims:
             self.set_attrs(x_dim=x_dim)
         else:
             raise ValueError(
                 "x dimension not found. Use 'set_spatial_dims'"
                 + " functions with correct x_dim argument provided."
             )
 
         if y_dim is None:
             for dim in YDIMS:
-                if dim in _dims:
-                    y_dim = dim
+                if dim in _dimslow:
+                    idim = _dimslow.index(dim)
+                    y_dim = _dims[idim]
                     break
         if y_dim and y_dim in _dims:
             self.set_attrs(y_dim=y_dim)
         else:
             raise ValueError(
                 "y dimension not found. Use 'set_spatial_dims'"
                 + " functions with correct y_dim argument provided."
@@ -354,16 +380,18 @@
 
         check_x = np.all(np.isclose(np.diff(np.diff(self._obj[x_dim])), 0, atol=1e-4))
         check_y = np.all(np.isclose(np.diff(np.diff(self._obj[y_dim])), 0, atol=1e-4))
         if check_x == False or check_y == False:
             raise ValueError("raster only applies to regular grids")
 
     def reset_spatial_dims_attrs(self):
-        """Reset spatial dimension names and attributes to make CF-compliant
-        Requires CRS attribute."""
+        """Reset spatial dimension names and attributes.
+
+        Needed to make CF-compliant and requires CRS attribute.
+        """
         if self.crs is None:
             raise ValueError("CRS is missing. Use set_crs function to resolve.")
         _da = self._obj
         x_dim, y_dim, x_attrs, y_attrs = gis_utils.axes_attrs(self.crs)
         if x_dim != self.x_dim or y_dim != self.y_dim:
             _da = _da.rename({self.x_dim: x_dim, self.y_dim: y_dim})
         _da[x_dim].attrs.update(x_attrs)
@@ -378,27 +406,24 @@
             self._check_dimensions()
         return self.get_attrs("dim0")
 
     @property
     def dims(self) -> tuple[str, str]:
         """Return tuple of geospatial dimensions names."""
         # if self.dim0 is not None:
-        #     return self.dim0, self.y_dim, self.x_dim
-        # else:
         return self.y_dim, self.x_dim
 
     @property
     def coords(self) -> dict[str, xr.IndexVariable]:
         """Return dict of geospatial dimensions coordinates."""
         return {self.ycoords.name: self.ycoords, self.xcoords.name: self.xcoords}
 
     @property
     def shape(self) -> tuple[int, int]:
         """Return shape of geospatial dimension (height, width)."""
-        # return tuple([self._obj.coords[d].size for d in list(self.dims)])
         return self.height, self.width
 
     @property
     def size(self) -> int:
         """Return size of geospatial grid."""
         return int(np.multiply(*self.shape))
 
@@ -446,28 +471,26 @@
             c3x, c3y = transform * (self.width, 0)
             xs = (c0x, c1x, c2x, c3x)
             ys = (c0y, c1y, c2y, c3y)
         return min(xs), min(ys), max(xs), max(ys)
 
     @property
     def box(self) -> gpd.GeoDataFrame:
-        """Return :py:meth:`~geopandas.GeoDataFrame` of bounding box"""
-        crs = self.crs
-        if crs is not None and crs.to_epsg() is not None:
-            crs = crs.to_epsg()  # not all CRS have an EPSG code
+        """Return :py:meth:`~geopandas.GeoDataFrame` of bounding box."""
         transform = self.transform
         rs = np.array([0, self.height, self.height, 0, 0])
         cs = np.array([0, 0, self.width, self.width, 0])
         xs, ys = transform * (cs, rs)
-        return gpd.GeoDataFrame(geometry=[Polygon([*zip(xs, ys)])], crs=crs)
+        return gpd.GeoDataFrame(geometry=[Polygon([*zip(xs, ys)])], crs=self.crs)
 
     @property
     def res(self) -> tuple[float, float]:
         """Return resolution (x, y) tuple.
-        NOTE: rotated rasters with a negative dx are not supported
+
+        NOTE: rotated rasters with a negative dx are not supported.
         """
         xs, ys = self.xcoords.data, self.ycoords.data
         dx, dy = 0, 0
         if xs.ndim == 1:
             dx = xs[1] - xs[0]
             dy = ys[1] - ys[0]
         elif xs.ndim == 2:
@@ -490,23 +513,27 @@
                 )
             ):
                 dy = -1 * dy
         return dx, dy
 
     @property
     def rotation(self) -> float:
-        """Return rotation of grid (degree)
-        NOTE: rotated rasters with a negative dx are not supported
+        """Return rotation of grid (degrees).
+
+        NOTE: rotated rasters with a negative dx are not supported.
         """
         xs, ys = self.xcoords.data, self.ycoords.data
         rot = 0
         if xs.ndim == 2:
             ddx1 = xs[0, -1] - xs[0, 0]
             ddy1 = ys[0, -1] - ys[0, 0]
-            rot = math.degrees(math.atan(ddy1 / ddx1))
+            if not np.isclose(ddx1, 0):
+                rot = math.degrees(math.atan(ddy1 / ddx1))
+            else:
+                rot = -90
             if ddx1 < 0:
                 rot = 180 + rot
             elif ddy1 < 0:
                 rot = 360 + rot
         return rot
 
     @property
@@ -524,15 +551,15 @@
             a = c * math.sin(beta - alpha)
             b = c * math.cos(beta - alpha)
             x0 = xs[0, 0] - np.sign(dy) * a
             y0 = ys[0, 0] - np.sign(dy) * b
         return x0, y0
 
     def _check_dimensions(self) -> None:
-        """Validates the dimensions number of dimensions and dimension order."""
+        """Validate the number and order of dimensions."""
         dims = (self.y_dim, self.x_dim)
         da = self._obj[self.vars[0]] if isinstance(self._obj, xr.Dataset) else self._obj
         extra_dims = [dim for dim in da.dims if dim not in dims]
         if len(extra_dims) == 1:
             dims = tuple(extra_dims) + dims
             self.set_attrs(dim0=extra_dims[0])
         elif len(extra_dims) == 0:
@@ -558,16 +585,18 @@
                 or self.crs == other.raster.crs
             )
             and np.allclose(self.transform, other.raster.transform, atol=1e-06)
             and np.allclose(self.shape, other.raster.shape)
         )
 
     def aligned_grid(self, other) -> bool:
-        """Return True if other grid aligns with object grid (crs, resolution, origin),
-        but with a smaller extent"""
+        """Check if other grid aligns with object grid (crs, resolution, origin).
+
+        Other can have a smaller extent.
+        """
         w, s, e, n = self.bounds
         w1, s1, e1, n1 = other.raster.bounds
         dx = (w - w1) % self.res[0]
         dy = (n - n1) % self.res[1]
         return (
             (
                 self.crs is None
@@ -579,18 +608,18 @@
             and (np.isclose(dy, 0) or np.isclose(dy, 1))
             and np.logical_and.reduce((w <= w1, s <= s1, e >= e1, n >= n1))
         )
 
     def gdal_compliant(
         self, rename_dims=True, force_sn=False
     ) -> xr.DataArray | xr.Dataset:
-        """Updates attributes to get GDAL compliant NetCDF files.
+        """Update attributes to get GDAL compliant NetCDF files.
 
         Arguments
-        ----------
+        ---------
         rename_dims: bool, optional
             If True, rename x_dim and y_dim to standard names depending on the CRS
             (x/y for projected and lat/lon for geographic).
         force_sn: bool, optional
             If True, forces the dataset to have South -> North orientation.
 
         Returns
@@ -628,15 +657,15 @@
 
         Optionally densifying the edges (to account for nonlinear transformations
         along these edges) and extracting the outermost bounds.
 
         Note: this does not account for the antimeridian.
 
         Arguments
-        ----------
+        ---------
         dst_crs: CRS, str, int, or dict
             Target coordinate reference system, input to
             :py:meth:`pyproj.CRS.from_user_input`
         densify_pts: uint, optional
             Number of points to add to each edge to account for nonlinear
             edges produced by the transform process.  Large numbers will produce
             worse performance.  Default: 21 (gdal default).
@@ -651,33 +680,35 @@
                 self.crs, dst_crs, *self.bounds, densify_pts=densify_pts
             )
         else:
             bounds = self.bounds
         return bounds
 
     def flipud(self) -> xr.DataArray | xr.Dataset:
-        """Returns raster flipped along y dimension"""
+        """Return raster flipped along y dimension."""
         y_dim = self.y_dim
         # NOTE don't use ycoords to work for rotated grids
         yrev = self._obj[y_dim].values[::-1]
         obj_filpud = self._obj.reindex({y_dim: yrev})
         # y_dim is typically a dimension without coords in rotated grids
         if y_dim not in self._obj.coords:
             obj_filpud = obj_filpud.drop_vars(y_dim)
         return obj_filpud
 
     def rowcol(
         self, xs, ys, mask=None, mask_outside=False, nodata=-1
     ) -> tuple[np.ndarray[int], np.ndarray[int]]:
-        """Return row, col indices of x, y coordinates
+        """Return row, col indices of x, y coordinates.
 
         Arguments
-        ----------
-        xs, ys: ndarray of float
-            x, y coordinates
+        ---------
+        xs: ndarray of float
+            x coordinates
+        ys: ndarray of float
+            y coordinates
         mask : ndarray of bool, optional
             data mask of valid values, by default None
         mask_outside : boolean, optional
             mask xy points outside domain (i.e. set nodata), by default False
         nodata : int, optional
             nodata value, used for output array, by default -1
 
@@ -706,20 +737,22 @@
         self,
         r: np.ndarray[int],
         c: np.ndarray[int],
         mask: np.ndarray[bool] = None,
         mask_outside: bool = False,
         nodata: float | int = np.nan,
     ) -> tuple[np.ndarray[float], np.ndarray[float]]:
-        """Return x,y coordinates at cell center of row, col indices
+        """Return x,y coordinates at cell center of row, col indices.
 
         Arguments
-        ----------
-        r, c : ndarray of int
-            index of row, column
+        ---------
+        r : ndarray of int
+            index of row
+        c : ndarray of int
+            index of column
         mask : ndarray of bool, optional
             data mask of valid values, by default None
         mask_outside : boolean, optional
             mask xy points outside domain (i.e. set nodata), by default False
         nodata : int, optional
             nodata value, used for output array, by default np.nan
 
@@ -740,18 +773,18 @@
             raise ValueError("Linear indices outside domain.")
         y = np.full(r.shape, nodata, dtype=np.float64)
         x = np.full(r.shape, nodata, dtype=np.float64)
         x[mask], y[mask] = self.transform * (c[mask], r[mask])
         return x, y
 
     def idx_to_xy(self, idx, mask=None, mask_outside=False, nodata=np.nan):
-        """Return x,y coordinates at linear index
+        """Return x,y coordinates at linear index.
 
         Arguments
-        ----------
+        ---------
         idx : ndarray of int
             linear index
         mask : ndarray of bool, optional
             data mask of valid values, by default None
         mask_outside : boolean, optional
             mask xy points outside domain (i.e. set nodata), by default False
         nodata : int, optional
@@ -764,20 +797,22 @@
         """
         idx = np.atleast_1d(idx)
         nrow, ncol = self.shape
         r, c = idx // ncol, idx % ncol
         return self.xy(r, c, mask=mask, mask_outside=mask_outside, nodata=nodata)
 
     def xy_to_idx(self, xs, ys, mask=None, mask_outside=False, nodata=-1):
-        """Return linear index of x, y coordinates
+        """Return linear index of x, y coordinates.
 
         Arguments
-        ----------
-        xs, ys: ndarray of float
-            x, y coordinates
+        ---------
+        xs: ndarray of float
+            x coordinates
+        ys: ndarray of float
+            y coordinates
         mask : ndarray of bool, optional
             data mask of valid values, by default None
         mask_outside : boolean, optional
             mask xy points outside domain (i.e. set nodata), by default False
         nodata : int, optional
             nodata value, used for output array, by default -1
 
@@ -856,17 +891,17 @@
         Arguments
         ---------
         gdf: geopandas.GeoDataFrame
             GeoDataFrame with geometries
         stats: list of str, callable
             Statistics to compute from raster values, options include
             {'count', 'min', 'max', 'sum', 'mean', 'std', 'median', 'q##'}.
-            Multiple percentiles can be calculated using comma-seperated values, e.g.: 'q10,50,90'
-            Statistics ignore the nodata value and are applied along the x and y dimension.
-            By default ['mean']
+            Multiple percentiles can be calculated using comma-seperated values,
+            e.g.: 'q10,50,90'. Statistics ignore the nodata value and are applied
+            along the x and y dimension. By default ['mean']
         all_touched : bool, optional
             If True, all pixels touched by geometries will used to define the sample.
             If False, only pixels whose center is within the geometry or that are
             selected by Bresenham's line algorithm will be used. By default False.
 
         Returns
         -------
@@ -935,23 +970,30 @@
 
         dss, idx = zip(*out)
         ds_out = xr.concat(dss, "index")
         ds_out["index"] = xr.IndexVariable("index", gdf.index.values[np.array(idx)])
 
         return ds_out
 
-    def reclassify(self, reclass_table: pd.DataFrame, method: str = "exact"):
+    def reclassify(
+        self, reclass_table: pd.DataFrame, method: str = "exact", logger=logger
+    ):
         """Reclass columns in df from raster map (DataArray).
 
         Arguments
         ---------
         reclass_table : pd.DataFrame
-            Tables with parameter names and values in columns and values in obj as index.
+            Tables with parameter names and values in columns
+            and values in obj as index.
         method : str, optional
-            Reclassification method. For now only 'exact' for one-on-one cell value mapping.
+            Reclassification method. For now only 'exact' for
+            one-on-one cell value mapping.
+        logger:
+            The logger to be used. If no logger is provided the
+            default one will beused.
 
         Returns
         -------
         ds_out: xr.Dataset
             Output dataset with a variable for each column in reclass_table.
         """
 
@@ -967,34 +1009,48 @@
         # limit dtypes to avoid gdal errors downstream
         ddict = {"float64": np.float32, "int64": np.int32}
         dtypes = {
             c: ddict.get(str(reclass_table[c].dtype), reclass_table[c].dtype)
             for c in reclass_table.columns
         }
         reclass_table = reclass_table.astype(dtypes)
+        # Get the nodata line
+        nodata_ref = da.raster.nodata
+        if nodata_ref is not None:
+            nodata_line = reclass_table[reclass_table.index == nodata_ref]
+            if nodata_line.empty:
+                # None will be used
+                nodata_ref = None
+                logger.warning(
+                    f"The nodata value {nodata_ref} is not in the reclass table."
+                    "None will be used for the params."
+                )
         # apply for each parameter
         for param in params:
             values = reclass_table[param].values
             d = dict(zip(keys, values))
             da_param = xr.apply_ufunc(
                 reclass_exact,
                 da,
                 dask="parallelized",
                 output_dtypes=[values.dtype],
                 kwargs={"ddict": d},
             )
-            da_param.attrs.update(_FillValue=np.nan)
+            nodata = (
+                nodata_line.at[nodata_ref, param] if nodata_ref is not None else None
+            )
+            da_param.attrs.update(_FillValue=nodata)
             ds_out[param] = da_param
         return ds_out
 
     def clip_bbox(self, bbox, align=None, buffer=0, crs=None):
         """Clip object based on a bounding box.
 
         Arguments
-        ----------
+        ---------
         bbox : array-like of floats
             (xmin, ymin, xmax, ymax) bounding box
         align : float, optional
             Resolution to align the bounding box, by default None
         buffer : int, optional
             Buffer around the bounding box expressed in resolution multiplicity,
             by default 0
@@ -1042,66 +1098,76 @@
             if buffer > 0:
                 y0 -= yres * buffer
                 y1 += yres * buffer
                 x0 -= xres * buffer
                 x1 += xres * buffer
             return self._obj.sel({self.x_dim: slice(x0, x1), self.y_dim: slice(y0, y1)})
 
-    # TODO make consistent with clip_geom
-    def clip_mask(self, mask):
+    def clip_mask(self, da_mask: xr.DataArray, mask: bool = False):
         """Clip object to region with mask values greater than zero.
+
         Arguments
         ---------
-        mask : xarray.DataArray
+        da_mask : xarray.DataArray
             Mask array.
+        mask: bool, optional
+            Mask values outside geometry with the raster nodata value
+            and add a "mask" coordinate with the boolean mask.
+
         Returns
         -------
         xarray.DataSet or DataArray
-            Data clipped to mask
+            Data clipped to mask.
         """
-        if not isinstance(mask, xr.DataArray):
+        if not isinstance(da_mask, xr.DataArray):
             raise ValueError("Mask should be xarray.DataArray type.")
-        if not mask.raster.shape == self.shape:
-            raise ValueError("Mask shape invalid.")
-        mask_bin = (mask.values != 0).astype(np.uint8)
-        if not np.any(mask_bin):
-            raise ValueError("Invalid mask.")
-        row_slice, col_slice = ndimage.find_objects(mask_bin)[0]
-        self._obj.coords["mask"] = xr.Variable(self.dims, mask_bin)
-        return self._obj.isel({self.x_dim: col_slice, self.y_dim: row_slice})
+        if not self.identical_grid(da_mask):
+            raise ValueError("Mask grid invalid.")
+        da_mask = da_mask != 0  # convert to boolean
+        if not np.any(da_mask):
+            raise ValueError("No valid values found in mask.")
+        # clip
+        row_slice, col_slice = ndimage.find_objects(da_mask.values.astype(np.uint8))[0]
+        obj_clip = self._obj.isel({self.x_dim: col_slice, self.y_dim: row_slice})
+        if mask:  # mask values and add mask coordinate
+            mask_bin = da_mask.isel({self.x_dim: col_slice, self.y_dim: row_slice})
+            obj_clip.coords["mask"] = xr.Variable(self.dims, mask_bin.values)
+            obj_clip = obj_clip.raster.mask(obj_clip.coords["mask"])
+        return obj_clip
 
     def clip_geom(self, geom, align=None, buffer=0, mask=False):
-        """Clip object to the bounding box of the geometry and add geometry 'mask' coordinate.
+        """Clip object to bounding box of the geometry.
 
         Arguments
         ---------
         geom : geopandas.GeoDataFrame/Series,
             A geometry defining the area of interest.
         align : float, optional
             Resolution to align the bounding box, by default None
         buffer : int, optional
             Buffer around the bounding box expressed in resolution multiplicity,
             by default 0
         mask: bool, optional
-            Mask values outside geometry with the raster nodata value
+            Mask values outside geometry with the raster nodata value,
+            and add a "mask" coordinate with the rasterize geometry mask.
 
         Returns
         -------
         xarray.DataSet or DataArray
             Data clipped to geometry
         """
         # TODO make common geom to gdf with correct crs parsing
         if not hasattr(geom, "crs"):
             raise ValueError("geom should be geopandas GeoDataFrame object.")
         bbox = geom.total_bounds
         if geom.crs is not None and self.crs is not None and geom.crs != self.crs:
             bbox = rasterio.warp.transform_bounds(geom.crs, self.crs, *bbox)
         obj_clip = self.clip_bbox(bbox, align=align, buffer=buffer)
-        obj_clip.coords["mask"] = obj_clip.raster.geometry_mask(geom)  # TODO remove!
-        if mask:
+        if mask:  # set nodata values outside geometry
+            obj_clip = obj_clip.assign_coords(mask=obj_clip.raster.geometry_mask(geom))
             obj_clip = obj_clip.raster.mask(obj_clip.coords["mask"])
         return obj_clip
 
     def rasterize(
         self,
         gdf,
         col_name="index",
@@ -1114,26 +1180,29 @@
         """Return an object with input geometry values burned in.
 
         Arguments
         ---------
         gdf : geopandas.GeoDataFrame
             GeoDataFrame of shapes and values to burn.
         col_name : str, optional
-            GeoDataFrame column name to use for burning, by default 'index'
+            GeoDataFrame column name to use for burning, by default 'index'.
         nodata : int or float, optional
-            Used as fill value for all areas not covered by input geometries, by default 0.
+            Used as fill value for all areas not covered by input geometries.
+            0 by default.
         all_touched : bool, optional
             If True, all pixels touched by geometries will be burned in. If false, only
             pixels whose center is within the polygon or that are selected by
             Bresenham's line algorithm will be burned in.
         dtype : numpy dtype, optional
             Used as data type for results, by default it is derived from values.
         sindex : bool, optional
             Create a spatial index to select overlapping geometries before rasterizing,
             by default False.
+        kwargs : optional
+            Additional keyword arguments to pass to `features.rasterize`.
 
         Returns
         -------
         xarray.DataArray
             DataArray with burned geometries
 
         Raises
@@ -1171,27 +1240,136 @@
         da_out = xr.DataArray(
             name=col_name, dims=self.dims, coords=self.coords, data=raster, attrs=attrs
         )
         da_out.raster.set_nodata(nodata)
         da_out.raster.set_attrs(**self.attrs)
         return da_out
 
+    def rasterize_geometry(
+        self,
+        gdf: gpd.GeoDataFrame,
+        method: Optional[str] = "fraction",
+        mask_name: Optional[str] = None,
+        name: Optional[str] = None,
+        nodata: Optional[Union[int, float]] = -1,
+        keep_geom_type: Optional[bool] = False,
+    ) -> xr.DataArray:
+        """Return an object with the fraction of the grid cells covered by geometry.
+
+        Arguments
+        ---------
+        gdf : geopandas.GeoDataFrame
+            GeoDataFrame of shapes to burn.
+        method : str, optional
+            Method to burn in the geometry, either 'fraction' (default) or 'area'.
+        mask_name : str, optional
+            Name of the mask variable in self to use for calculating the fraction of
+            area covered by the geometry. By default None for no masking.
+        name : str, optional
+            Name of the output DataArray. If None, the method name is used.
+        nodata : int or float, optional
+            Used as fill value for all areas not covered by input geometries.
+            By default -1.
+        keep_geom_type : bool
+            Only maintain geometries of the same type if true, otherwise
+            keep geometries, regardless of their remaining type.
+            False by default
+
+        Returns
+        -------
+        da_out: xarray.DataArray
+            DataArray with burned geometries
+        """
+        ds_like = self._obj.copy()
+        # Create vector grid (for calculating fraction and storage per grid cell)
+        logger.debug(
+            "Creating vector grid for calculating coverage fraction per grid cell"
+        )
+        gdf["geometry"] = gdf.geometry.buffer(0)  # fix potential geometry errors
+        gdf_grid_all = ds_like.raster.vector_grid()
+        if mask_name is None:
+            gdf_grid = gdf_grid_all
+        else:
+            msktn = ds_like[mask_name]
+            idx_valid = np.where(msktn.values.flatten() != msktn.raster.nodata)[0]
+            gdf_grid = gdf_grid_all.loc[idx_valid]
+
+        # intersect the gdf data with the grid
+        gdf = gdf.to_crs(gdf_grid.crs)
+        gdf_intersect = gdf.overlay(
+            gdf_grid, how="intersection", keep_geom_type=keep_geom_type
+        )
+
+        # find the best UTM CRS for area computation
+        if gdf_intersect.crs.is_geographic:
+            crs_utm = gis_utils.parse_crs(
+                "utm", gdf_intersect.to_crs(4326).total_bounds
+            )
+        else:
+            crs_utm = gdf_intersect.crs
+
+        # compute area using same crs for frac
+        gdf_intersect = gdf_intersect.to_crs(crs_utm)
+        gdf_intersect["area"] = gdf_intersect.area
+        # convert to point (easier for stats)
+        gdf_intersect["geometry"] = gdf_intersect.representative_point()
+
+        # Rasterize area column with sum
+        da_area = ds_like.raster.rasterize(
+            gdf_intersect,
+            col_name="area",
+            nodata=0,
+            all_touched=True,
+            merge_alg=MergeAlg.add,
+        )
+
+        if method == "area":
+            da_out = da_area
+        else:  # fraction
+            # Mask grid cells that actually do intersect with the geometry
+            idx_area = np.where(da_area.values.flatten() != da_area.raster.nodata)[0]
+            gdf_grid = gdf_grid_all.loc[idx_area]
+            # Convert to frac using gdf grid in same crs
+            # (area error when using ds_like.raster.area_grid)
+            gdf_grid = gdf_grid.to_crs(crs_utm)
+            gdf_grid["area"] = gdf_grid.area
+            da_gridarea = ds_like.raster.rasterize(
+                gdf_grid, col_name="area", nodata=0, all_touched=False
+            )
+
+            da_out = da_area / da_gridarea
+            # As not all da_gridarea were computed, cover with zeros
+            da_out = da_out.fillna(0)
+            da_out.name = "fraction"
+
+        da_out.raster.set_crs(ds_like.raster.crs)
+        da_out.raster.set_nodata(nodata)
+        # Rename da_area
+        if name is not None:
+            da_out.name = name
+
+        return da_out
+
     def geometry_mask(self, gdf, all_touched=False, invert=False, **kwargs):
         """Return a grid with True values where shapes overlap pixels.
 
         Arguments
         ---------
         gdf : geopandas.GeoDataFrame
             GeoDataFrame of shapes and values to burn.
         all_touched : bool, optional
             If True, all pixels touched by geometries will masked. If false, only
             pixels whose center is within the polygon or that are selected by
             Bresenham's line algorithm will be burned in. By default False.
         invert : bool, optional
-            If True, the mask will be False where shapes overlap pixels, by default False
+            If True, the mask will be False where shapes overlap pixels,
+            by default False
+        kwargs : optional
+            Additional keyword arguments to pass to `features.rasterize`.
+
 
         Returns
         -------
         xarray.DataArray
             Geometry mask
         """
         gdf1 = gdf.copy()
@@ -1203,29 +1381,68 @@
             nodata=np.uint8(invert),
             **kwargs,
         )
         # remove nodata value before converting to boolean
         da_out.attrs.pop("_FillValue", None)
         return da_out.astype(bool)
 
-    def vector_grid(self):
-        """Return a geopandas GeoDataFrame with a geometry for each grid cell."""
-        transform = self.transform
+    def vector_grid(self, geom_type: str = "polygon") -> gpd.GeoDataFrame:
+        """Return a vector representation of the grid.
+
+        Parameters
+        ----------
+        geom_type : str, optional
+            Type of geometry to return, by default 'polygon'
+            Available options are 'polygon', 'line', 'point'
+
+        Returns
+        -------
+        geopandas.GeoDataFrame
+            GeoDataFrame with grid geometries
+        """
+        if not hasattr(shapely, "from_ragged_array"):
+            raise ImportError("the vector_grid method requires shapely 2.0+")
         nrow, ncol = self.shape
-        cells = []
-        for i in range(nrow):
-            rs = np.array([i, i + 1, i + 1, i, i])
-            for j in range(ncol):
-                cs = np.array([j, j, j + 1, j + 1, j])
-                xs, ys = transform * (cs, rs)
-                cells.append(Polygon([*zip(xs, ys)]))
-        return gpd.GeoDataFrame(geometry=cells, crs=self.crs)
+        transform = self.transform
+        if geom_type.lower().startswith("polygon"):
+            # build a flattened list of coordinates for each cell
+            dr = np.array([0, 0, 1, 1, 0])
+            dc = np.array([0, 1, 1, 0, 0])
+            ii, jj = np.meshgrid(np.arange(0, nrow), np.arange(0, ncol))
+            coords = np.empty((nrow * ncol * 5, 2), dtype=np.float64)
+            # order of cells: first rows, then cols
+            coords[:, 0], coords[:, 1] = transform * (
+                (jj.T[:, :, None] + dr[None, None, :]).ravel(),
+                (ii.T[:, :, None] + dc[None, None, :]).ravel(),
+            )
+            # offsets of the first coordinate of each cell, index of cells
+            offsets = (
+                np.arange(0, nrow * ncol * 5 + 1, 5, dtype=np.int32),
+                np.arange(nrow * ncol + 1, dtype=np.int32),
+            )
+            # build the geometry array in a fast way
+            geoms = shapely.from_ragged_array(3, coords, offsets)  # type 3 is polygon
+        elif geom_type.lower().startswith("line"):  # line or linestring
+            geoms = []
+            # horizontal lines
+            for i in range(nrow + 1):
+                xs, ys = transform * (np.array([0, ncol]), np.array([i, i]))
+                geoms.append(LineString(zip(xs, ys)))
+            for i in range(ncol + 1):
+                xs, ys = transform * (np.array([i, i]), np.array([0, nrow]))
+                geoms.append(LineString(zip(xs, ys)))
+        elif geom_type.lower().startswith("point"):
+            x, y = gis_utils.affine_to_meshgrid(transform, (nrow, ncol))
+            geoms = gpd.points_from_xy(x.ravel(), y.ravel())
+        else:
+            raise ValueError(f"geom_type {geom_type} not recognized")
+        return gpd.GeoDataFrame(geometry=geoms, crs=self.crs)
 
     def area_grid(self, dtype=np.float32):
-        """Returns the grid cell area [m2].
+        """Return the grid cell area [m2].
 
         Returns
         -------
         da_area : xarray.DataArray
             Grid cell surface area [m2].
         """
         if self.rotation > 0:
@@ -1242,23 +1459,24 @@
         )
         da_area.raster.set_nodata(0)
         da_area.raster.set_crs(self.crs)
         da_area.attrs.update(unit="m2")
         return da_area.rename("area")
 
     def density_grid(self):
-        """Returns the density in [unit/m2] of raster(s). The cell areas are calculated
-        using :py:meth:`~hydromt.raster.XRasterBase.area_grid`.
+        """Return the density in [unit/m2] of raster(s).
+
+        The cell areas are calculated using
+        :py:meth:`~hydromt.raster.XRasterBase.area_grid`.
 
         Returns
         -------
         ds_out: xarray.DataArray or xarray.DataSet
             The density in [unit/m2] of the raster.
         """
-
         # Create a grid that contains the area in m2 per grid cell.
         if self.crs.is_geographic:
             area = self.area_grid()
 
         elif self.crs.is_projected:
             ucf = rasterio.crs.CRS.from_user_input(self.crs).linear_units_factor[1]
             area = abs(self.res[0] * self.res[0]) * ucf**2
@@ -1274,15 +1492,14 @@
         dst_crs=None,
         dst_res=None,
         dst_transform=None,
         dst_width=None,
         dst_height=None,
         align=False,
     ):
-        xres, yres = self.res
         # NOTE dst_tranform may get overwritten here?!
         if dst_transform is None or dst_width is None or dst_height is None:
             (
                 dst_transform,
                 dst_width,
                 dst_height,
             ) = rasterio.warp.calculate_default_transform(
@@ -1317,43 +1534,56 @@
         dst_crs=None,
         dst_res=None,
         dst_transform=None,
         dst_width=None,
         dst_height=None,
         align=False,
     ):
-        """Prepare nearest index mapping for the reprojection of a gridded timeseries
-        file, powered by pyproj and k-d tree lookup.
+        """Prepare nearest index mapping for reprojection of a gridded timeseries file.
 
-        Index mappings typically are used in reprojection workflows of time series,
-        or combinations of time series
+        Powered by pyproj and k-d tree lookup. Index mappings typically are used
+        in reprojection workflows of time series, or combinations of time series.
 
-        ... Note: Is used by :py:meth:`~hydromt.raster.RasterDataArray.reproject` if method equals 'nearest_index'
+        ... Note: Is used by :py:meth:`~hydromt.raster.RasterDataArray.reproject` if
+        method equals 'nearest_index'
 
         Arguments
-        ----------
+        ---------
         dst_crs: int, dict, or str, optional
-            Target CRS. Accepts EPSG codes (int or str); proj (str or dict) or wkt (str)
-            "utm" is accepted and will return the centroid utm zone CRS
+            Target CRS. Accepts EPSG codes (int or str);
+            proj (str or dict) or wkt (str).
+            "utm" is accepted and will return the centroid utm zone CRS.
         dst_res: tuple (x resolution, y resolution) or float, optional
-            Target resolution, in units of target CRS.
+            Target resolution, in units of the target CRS.
         dst_transform: affine.Affine(), optional
             Target affine transformation. Will be calculated if None.
-        dst_width, dst_height: int, optional
-            Output file size in pixels and lines. Cannot be used together with
-            resolution (dst_res).
-        align: boolean, optional
-            If True, align target transform to resolution
+        dst_width: int, optional
+            Output file width in pixels. Can't be used together with resolution dst_res.
+        dst_height: int, optional
+            Output file height in lines. Can't be used together with resolution dst_res.
+        align: bool, optional
+            If True, align the target transform to the resolution.
 
         Returns
         -------
         index: xarray.DataArray of intp
-            DataArray with flat indices of source DataArray
+            DataArray with flat indices of the source DataArray.
+
+        Raises
+        ------
+        ValueError
+            If the destination grid and CRS are not valid.
+
+        Notes
+        -----
+        - The method is powered by pyproj and k-d tree lookup.
+        - | The index mappings are typically used in reprojection workflows of
+          | time series or combinations of time series.
         """
-        # parse and check destination grid and crs
+        # parse and check destination grid and CRS
         dst_crs = self._dst_crs(dst_crs)
         dst_transform, dst_width, dst_height = self._dst_transform(
             dst_crs, dst_res, dst_transform, dst_width, dst_height, align
         )
         # Transform the destination grid points to the source CRS.
         reproj2src = pyproj.transformer.Transformer.from_crs(
             crs_from=dst_crs, crs_to=self.crs, always_xy=True
@@ -1368,21 +1598,21 @@
         # Create source coordinate pairs.
         src_yy, src_xx = self.ycoords.values, self.xcoords.values
         if src_yy.ndim == 1:
             src_yy, src_xx = np.meshgrid(src_yy, src_xx, indexing="ij")
         src_yy, src_xx = src_yy.ravel(), src_xx.ravel()
         src_coords = np.vstack([src_xx, src_yy]).transpose()
         # Build a KD-tree with the source grid cell center coordinate pairs.
-        # For each destination grid cell coordinate pairs, search for the nearest
+        # For each destination grid cell coordinate pair, search for the nearest
         # source grid cell in the KD-tree.
         # TODO: benchmark against RTree or S2Index https://github.com/benbovy/pys2index
         tree = cKDTree(src_coords)
         _, indices = tree.query(dst_coords_reproj)
         # filter destination cells with center outside source bbox
-        # TODO filter for rotated case
+        # TODO filter for the rotated case
         w, s, e, n = self.bounds
         valid = np.logical_and(
             np.logical_and(dst_xx_reproj > w, dst_xx_reproj < e),
             np.logical_and(dst_yy_reproj > s, dst_yy_reproj < n),
         )
         indices[~valid] = -1  # nodata value
         # create 2D remapping dataset
@@ -1399,37 +1629,41 @@
         index.raster.set_crs(dst_crs)
         index.raster.set_nodata(-1)
         return index
 
 
 @xr.register_dataarray_accessor("raster")
 class RasterDataArray(XRasterBase):
-    """This is the GIS extension for xarray.DataArray"""
+
+    """GIS extension for xarray.DataArray."""
 
     def __init__(self, xarray_obj):
+        """Initiallize the object based on the provided xarray object."""
         super(RasterDataArray, self).__init__(xarray_obj)
 
     @staticmethod
     def from_numpy(data, transform, nodata=None, attrs={}, crs=None):
         """Transform a 2D/3D numpy array into a DataArray with geospatial attributes.
-        The data dimensions should have the y and x on the second last and last dimensions.
+
+        The data dimensions should have the y and x on the second last
+        and last dimensions.
 
         Arguments
         ---------
         data : numpy.array, 2-dimensional
             values to parse into DataArray
         transform : affine transform
             Two dimensional affine transform for 2D linear mapping
         nodata : float or int, optional
             nodata value
         attrs : dict, optional
             additional attributes
         crs: int, dict, or str, optional
-            Coordinate Reference System. Accepts EPSG codes (int or str); proj (str or dict)
-            or wkt (str)
+            Coordinate Reference System. Accepts EPSG codes (int or str);
+            proj (str or dict) or wkt (str)
 
         Returns
         -------
         da : RasterDataArray
             xarray.DataArray with geospatial information
         """
         nrow, ncol = data.shape[-2:]
@@ -1462,46 +1696,60 @@
                 self.set_nodata(nodata)
         return nodata
 
     def set_nodata(self, nodata=None, logger=logger):
         """Set the nodata value as CF compliant attribute of the DataArray.
 
         Arguments
-        ----------
+        ---------
         nodata: float, integer
             Nodata value for the DataArray.
             If the nodata property and argument are both None, the _FillValue
             attribute will be removed.
+        logger:
+            The logger to use.
         """
         if nodata is None:
             nodata = self._obj.rio.nodata
             if nodata is None:
                 nodata = self._obj.rio.encoded_nodata
         # Only numerical nodata values are supported
         if np.issubdtype(type(nodata), np.number):
-            self._obj.rio.set_nodata(nodata, inplace=True)
-            self._obj.rio.write_nodata(nodata, inplace=True)
+            # python naitive types don't play very nice
+            if isinstance(nodata, float):
+                nodata_cast = np.float32(nodata)
+            elif isinstance(nodata, int):
+                nodata_cast = np.int32(nodata)
+            else:
+                nodata_cast = nodata
+
+            # cast to float since using int causes inconsistent casting
+            self._obj.rio.set_nodata(nodata_cast, inplace=True)
+            self._obj.rio.write_nodata(nodata_cast, inplace=True)
         else:
             logger.warning("No numerical nodata value found, skipping set_nodata")
             self._obj.attrs.pop("_FillValue", None)
 
     def mask_nodata(self, fill_value=np.nan):
         """Mask nodata values with fill_value (default np.nan).
+
         Note that masking with np.nan will change integer dtypes to float.
         """
         _da = self._obj
         if self.nodata is not None and self.nodata != fill_value:
             mask = _da.notnull() if np.isnan(self.nodata) else _da != self.nodata
             _da = _da.where(mask, fill_value)
             _da.raster.set_nodata(fill_value)
         return _da
 
     def mask(self, mask, logger=logger):
         """Mask cells where mask equals False with the data nodata value.
-        A warning is raised if no the data has no nodata value."""
+
+        A warning is raised if no the data has no nodata value.
+        """
         if self.nodata is not None:
             da_masked = self._obj.where(mask != 0, self.nodata)
         else:
             logger.warning("Nodata value missing, skipping mask")
             da_masked = self._obj
         return da_masked
 
@@ -1538,28 +1786,28 @@
             shape=(dst_height, dst_width)
             if self.dim0 is None
             else (self._obj.shape[0], dst_height, dst_width),
             dims=self.dims if self.dim0 is None else (self.dim0, *self.dims),
         )
         # apply rasterio warp reproject
         rasterio.warp.reproject(
-            source=self._obj.load().data,
+            source=self._obj.values,
             destination=da_reproject.data,
             src_transform=self.transform,
             src_crs=self.crs,
             src_nodata=self.nodata,
             dst_transform=dst_transform,
             dst_crs=dst_crs,
             dst_nodata=da_reproject.raster.nodata,
             resampling=resampling,
         )
         return da_reproject
 
     def _reindex2d(self, index, dst_nodata=np.nan):
-        """Return reindexed (reprojected) object"""
+        """Return reindexed (reprojected) object."""
         # create new DataArray for output
         dst_coords = {d: self._obj.coords[d] for d in self._obj.dims}
         ys, xs = index.raster.ycoords, index.raster.xcoords
         dst_coords.update({self.y_dim: ys, self.x_dim: xs})
         da_reproject = full(
             dst_coords,
             nodata=dst_nodata,
@@ -1590,29 +1838,31 @@
         dst_transform=None,
         dst_width=None,
         dst_height=None,
         dst_nodata=None,
         method="nearest",
         align=False,
     ):
-        """Reproject a DataArray with geospatial coordinates, powered
-        by :py:meth:`rasterio.warp.reproject`.
+        """Reproject a DataArray with geospatial coordinates.
+
+        Powered by :py:meth:`rasterio.warp.reproject`.
 
         Arguments
-        ----------
+        ---------
         dst_crs: int, dict, or str, optional
             Target CRS. Accepts EPSG codes (int or str); proj (str or dict) or wkt (str)
             "utm" is accepted and will return the centroid utm zone CRS
         dst_res: tuple (x resolution, y resolution) or float, optional
             Target resolution, in units of target CRS.
         dst_transform: affine.Affine(), optional
             Target affine transformation. Will be calculated if None.
-        dst_width, dst_height: int, optional
-            Output file size in pixels and lines. Cannot be used together with
-            resolution (dst_res).
+        dst_width: int, optional
+            Output file width in pixels. Can't be used together with resolution dst_res.
+        dst_height: int, optional
+            Output file height in lines. Can't be used together with resolution dst_res.
         dst_nodata: int or float, optional
             The nodata value used to initialize the destination; it will
             remain in all areas not covered by the reprojected source. If None, the
             source nodata value will be used.
         method: str, optional
             See rasterio.warp.reproject for existing methods, by default nearest.
             Additionally "nearest_index" can be used for KDTree based downsampling.
@@ -1673,51 +1923,59 @@
                 crs=dst_crs,
                 lazy=True,
                 shape=(dst_height, dst_width)
                 if self.dim0 is None
                 else (self._obj.shape[0], dst_height, dst_width),
                 dims=self.dims if self.dim0 is None else (self.dim0, *self.dims),
             )
-            # chunk time and set reset chunks on other dims
+            # no chunks on spatial dims
             chunksize = max(self._obj.chunks[0])
             chunks = {d: chunksize if d == self.dim0 else -1 for d in self._obj.dims}
             _da = self._obj.chunk(chunks)
             da_temp = da_temp.chunk(chunks)
             da_reproj = _da.map_blocks(_reproj, kwargs=reproj_kwargs, template=da_temp)
         da_reproj.raster.set_crs(dst_crs)
         return da_reproj.raster.reset_spatial_dims_attrs()
 
     def reproject_like(self, other, method="nearest"):
         """Reproject a object to match the grid of ``other``.
 
         Arguments
-        ----------
+        ---------
         other : xarray.DataArray or Dataset
             DataArray of the target resolution and projection.
         method : str, optional
-            See :py:meth:`~hydromt.raster.RasterDataArray.reproject` for existing methods,
-            by default 'nearest'.
+            See :py:meth:`~hydromt.raster.RasterDataArray.reproject` for existing
+            methods, by default 'nearest'.
 
         Returns
-        --------
+        -------
         da : xarray.DataArray
             Reprojected object.
         """
         # clip first; then reproject
         da = self._obj
         if self.aligned_grid(other):
             da = self.clip_bbox(other.raster.bounds)
         elif not self.identical_grid(other):
-            da = self.reproject(
-                dst_crs=other.raster.crs,
-                dst_transform=other.raster.transform,
-                dst_width=other.raster.width,
-                dst_height=other.raster.height,
-                method=method,
-            )
+            da_clip = self.clip_bbox(other.raster.transform_bounds(self.crs), buffer=2)
+            if np.any(np.array(da_clip.raster.shape) < 2):
+                # out of bounds -> return empty array
+                if isinstance(other, xr.Dataset):
+                    other = other[list(other.data_vars.keys())[0]]
+                da = full_like(other, nodata=self.nodata)
+                da.name = self._obj.name
+            else:
+                da = da_clip.raster.reproject(
+                    dst_crs=other.raster.crs,
+                    dst_transform=other.raster.transform,
+                    dst_width=other.raster.width,
+                    dst_height=other.raster.height,
+                    method=method,
+                )
         if (
             da.raster.x_dim != other.raster.x_dim
             or da.raster.y_dim != other.raster.y_dim
         ):
             # overwrite spatial dimension names which might have been changed
             rm = {
                 da.raster.x_dim: other.raster.x_dim,
@@ -1725,29 +1983,33 @@
             }
             da = da.rename(rm)
             da.raster.set_spatial_dims(
                 x_dim=other.raster.x_dim, y_dim=other.raster.y_dim
             )
         # make sure coordinates are identical!
         xcoords, ycoords = other.raster.xcoords, other.raster.ycoords
-        da[xcoords.name] = xcoords
-        da[ycoords.name] = ycoords
+        da = da.assign_coords({xcoords.name: xcoords, ycoords.name: ycoords})
         return da
 
     def reindex2d(self, index, dst_nodata=None):
-        """Return reprojected DataArray object based on simple reindexing using
-        linear indices in ``index``, which can be calculated with
+        """Return reprojected DataArray object based on simple reindexing.
+
+        Use linear indices in ``index``, which can be calculated with
         :py:meth:`~hydromt.raster.RasterDataArray.nearest_index`.
 
         This is typically used to downscale time series data.
 
         Arguments
-        ----------
+        ---------
         index: xarray.DataArray of intp
             DataArray with flat indices of source DataArray
+        dst_nodata: int or float, optional
+            The nodata value used to initialize the destination; it will
+            remain in all areas not covered by the reprojected source. If None, the
+            source nodata value will be used.
 
         Returns
         -------
         da_reproject : xarray.DataArray
             The reindexed DataArray.
         """
 
@@ -1773,93 +2035,112 @@
                 crs=index.raster.crs,
                 lazy=True,
                 shape=index.raster.shape
                 if self.dim0 is None
                 else (self._obj.shape[0], *index.raster.shape),
                 dims=self.dims if self.dim0 is None else (self.dim0, *self.dims),
             )
-            # chunk along first dim
+            # no chunks on spatial dims
             chunksize = max(self._obj.chunks[0])
             chunks = {d: chunksize if d == self.dim0 else -1 for d in self._obj.dims}
             _da = self._obj.chunk(chunks)
             da_temp = da_temp.chunk(chunks)
             # map blocks
             da_reproj = _da.map_blocks(_reindex2d, kwargs=kwargs, template=da_temp)
         da_reproj.raster.set_nodata(dst_nodata)
         return da_reproj.raster.reset_spatial_dims_attrs()
 
     def _interpolate_na(
-        self, src_data: np.ndarray, method: str = "nearest", **kwargs
+        self, src_data: np.ndarray, method: str = "nearest", extrapolate=False, **kwargs
     ) -> np.ndarray:
-        """Returns interpolated array"""
+        """Return interpolated array."""
         data_isnan = True if self.nodata is None else np.isnan(self.nodata)
         mask = ~np.isnan(src_data) if data_isnan else src_data != self.nodata
         if not mask.any() or mask.all():
             return src_data
-        if method == "rio_idw":  # NOTE: modifies src_data inplace
-            # NOTE this method might also extrapolate
-            interp_data = rasterio.fill.fillnodata(src_data.copy(), mask, **kwargs)
-        else:
+        if not (method == "rio_idw" and not extrapolate):
             # get valid cells D4-neighboring nodata cells to setup triangulation
             valid = np.logical_and(mask, ndimage.binary_dilation(~mask))
             xs, ys = self.xcoords.values, self.ycoords.values
             if xs.ndim == 1:
                 xs, ys = np.meshgrid(xs, ys)
+        if method == "rio_idw":
+            # NOTE: modifies src_data inplace
+            interp_data = rasterio.fill.fillnodata(src_data.copy(), mask, **kwargs)
+        else:
             # interpolate data at nodata cells only
             interp_data = src_data.copy()
             interp_data[~mask] = griddata(
                 points=(xs[valid], ys[valid]),
                 values=src_data[valid],
                 xi=(xs[~mask], ys[~mask]),
                 method=method,
                 fill_value=self.nodata,
             )
+        mask = ~np.isnan(interp_data) if data_isnan else src_data != self.nodata
+        if extrapolate and not np.all(mask):
+            # extrapolate data at remaining nodata cells based on nearest neighbor
+            interp_data[~mask] = griddata(
+                points=(xs[mask], ys[mask]),
+                values=interp_data[mask],
+                xi=(xs[~mask], ys[~mask]),
+                method="nearest",
+                fill_value=self.nodata,
+            )
         return interp_data
 
-    def interpolate_na(self, method: str = "nearest", **kwargs):
-        """Interpolate missing data
+    def interpolate_na(
+        self, method: str = "nearest", extrapolate: bool = False, **kwargs
+    ):
+        """Interpolate missing data.
 
         Arguments
-        ----------
+        ---------
         method: {'linear', 'nearest', 'cubic', 'rio_idw'}, optional
             {'linear', 'nearest', 'cubic'} use :py:meth:`scipy.interpolate.griddata`;
-            'rio_idw' applies inverse distance weighting based on :py:meth:`rasterio.fill.fillnodata`.
-        **kwargs
-            Additional key-word arguments are passed to :py:meth:`rasterio.fill.fillnodata`,
-            only used in combination with `method='rio_idw'`
+            'rio_idw' applies inverse distance weighting based on
+            :py:meth:`rasterio.fill.fillnodata`. Default is 'nearest'.
+        extrapolate: bool, optional
+            If True, extrapolate data at remaining nodata cells after interpolation
+            based on nearest neighbor.
+        **kwargs:
+            Additional key-word arguments are passed to
+            :py:meth:`rasterio.fill.fillnodata`, only used in
+            combination with `method='rio_idw'`
 
         Returns
         -------
         xarray.DataArray
             Filled object
         """
         dim0 = self.dim0
+        kwargs.update(dict(method=method, extrapolate=extrapolate))
         if dim0:
             interp_data = np.empty(self._obj.shape, dtype=self._obj.dtype)
             for i, (_, sub_xds) in enumerate(self._obj.groupby(dim0)):
                 interp_data[i, ...] = self._interpolate_na(
-                    sub_xds.load().data, method=method, **kwargs
+                    sub_xds.load().data, **kwargs
                 )
         else:
-            interp_data = self._interpolate_na(
-                self._obj.load().data, method=method, **kwargs
-            )
+            interp_data = self._interpolate_na(self._obj.load().data, **kwargs)
         interp_array = xr.DataArray(
             name=self._obj.name,
             dims=self._obj.dims,
             coords=self._obj.coords,
             data=interp_data,
             attrs=self._obj.attrs,
         )
+        interp_array.raster.set_nodata(self.nodata)
+        interp_array.raster.set_crs(self.crs)
         return interp_array
 
     def to_xyz_tiles(
         self, root: str, tile_size: int, zoom_levels: list, driver="GTiff", **kwargs
     ):
-        """Export rasterdataset to tiles in a xyz structure
+        """Export rasterdataset to tiles in a xyz structure.
 
         Parameters
         ----------
         root : str
             Path where the database will be saved
             Database yml will be put one directory above
         tile_size : int
@@ -1874,17 +2155,18 @@
         mName = os.path.normpath(os.path.basename(root))
 
         def create_folder(path):
             if not os.path.exists(path):
                 os.makedirs(path)
 
         def tile_window(shape, px):
-            """Yield (left, upper, width, height)"""
+            """Yield (left, upper, width, height)."""
             nr, nc = shape
             lu = product(range(0, nc, px), range(0, nr, px))
+
             ## create the window
             for l, u in lu:
                 h = min(px, nr - u)
                 w = min(px, nc - l)
                 yield (l, u, w, h)
 
         vrt_fn = None
@@ -1961,155 +2243,50 @@
             "driver": "raster",
             "path": f"{mName}_zl{{zoom_level}}.vrt",
             "zoom_levels": zls,
         }
         with open(join(root, f"{mName}.yml"), "w") as f:
             yaml.dump({mName: yml}, f, default_flow_style=False, sort_keys=False)
 
-    # def to_osm(
-    #     self,
-    #     root: str,
-    #     zl: int,
-    #     bbox: tuple = (),
-    # ):
-    #     """Generate tiles from raster according to the osm scheme
-
-    #     Parameters
-    #     ----------
-    #     root : str
-    #         Path to folder where the database will be created
-    #     zl : int
-    #         Maximum zoom level of the database
-    #         Everyting is generated incrementally up until this level
-    #         E.g. zl = 8, levels generated: 0 to 7
-    #     bbox : tuple, optional
-    #         Bounding Box in the objects crs
-
-    #     """
-
-    #     assert self._obj.ndim == 2, "Only 2d datasets are accepted..."
-    #     obj = self._obj.transpose(self.y_dim, self.x_dim)
-
-    #     mName = os.path.normpath(os.path.basename(root))
-
-    #     def create_folder(path):
-    #         if not os.path.exists(path):
-    #             os.makedirs(path)
-
-    #     def transform_res(dres, transformer):
-    #         return transformer.transform(0, dres)[0]
-
-    #     create_folder(root)
-
-    #     dres = abs(self._obj.raster.res[0])
-    #     if bbox:
-    #         minx, miny, maxx, maxy = bbox
-    #     else:
-    #         minx, miny, maxx, maxy = self._obj.raster.transform_bounds(
-    #             dst_crs=self._obj.raster.crs
-    #         )
-
-    #     transformer = pyproj.Transformer.from_crs(self._obj.raster.crs.to_epsg(), 3857)
-    #     minx, miny = map(
-    #         max, zip(transformer.transform(miny, minx), [-20037508.34] * 2)
-    #     )
-    #     maxx, maxy = map(min, zip(transformer.transform(maxy, maxx), [20037508.34] * 2))
-
-    #     dres = transform_res(dres, transformer)
-    #     nzl = int(np.ceil((np.log10((20037508.34 * 2) / (dres * 256)) / np.log10(2))))
-
-    #     if zl > nzl:
-    #         zl = nzl
-
-    #     def tile_window(zl, minx, miny, maxx, maxy):
-    #         # Basic stuff
-    #         dx = (20037508.34 * 2) / (2**zl)
-    #         # Origin displacement
-    #         odx = np.floor(abs(-20037508.34 - minx) / dx)
-    #         ody = np.floor(abs(20037508.34 - maxy) / dx)
-
-    #         # Set the new origin
-    #         minx = -20037508.34 + odx * dx
-    #         maxy = 20037508.34 - ody * dx
-
-    #         # Create window generator
-    #         lu = product(np.arange(minx, maxx, dx), np.arange(maxy, miny, -dx))
-    #         for l, u in lu:
-    #             col = int(odx + (l - minx) / dx)
-    #             row = int(ody + (maxy - u) / dx)
-    #             yield Affine(dx / 256, 0, l, 0, -dx / 256, u), col, row
-
-    #     for zlvl in range(zl):
-    #         sd = f"{root}\\{zlvl}"
-    #         create_folder(sd)
-    #         file = open(f"{sd}\\filelist.txt", "w")
-
-    #         for transform, col, row in tile_window(zlvl, minx, miny, maxx, maxy):
-    #             ssd = f"{sd}\\{col}"
-    #             create_folder(ssd)
-
-    #             temp = obj.load()
-    #             temp = temp.raster.reproject(
-    #                 dst_transform=transform,
-    #                 dst_crs=3857,
-    #                 dst_width=256,
-    #                 dst_height=256,
-    #             )
-
-    #             temp.raster.to_raster(f"{ssd}\\{row}.tif", driver="GTiff")
-
-    #             file.write(f"{ssd}\\{row}.tif\n")
-
-    #             del temp
-
-    #         file.close()
-
-    #         gis_utils.create_vrt(sd, mName)
-    #     # Write a quick yaml for the database
-    #     with open(f"{root}\\..\\{mName}.yml", "w") as w:
-    #         w.write(f"{mName}:\n")
-    #         crs = 3857
-    #         w.write(f"  crs: {crs}\n")
-    #         w.write("  data_type: RasterDataset\n")
-    #         w.write("  driver: raster\n")
-    #         w.write(f"  path: {mName}/{{zoom_level}}/{mName}.vrt\n")
-
     def to_raster(
         self,
         raster_path,
         driver="GTiff",
         dtype=None,
         tags=None,
         windowed=False,
         mask=False,
         logger=logger,
         **profile_kwargs,
     ):
         """Write DataArray object to a gdal-writable raster file.
 
         Arguments
-        ----------
+        ---------
         raster_path: str
             The path to output the raster to.
         driver: str, optional
             The name of the GDAL/rasterio driver to use to export the raster.
             Default is "GTiff".
         dtype: str, optional
             The data type to write the raster to. Default is the datasets dtype.
         tags: dict, optional
             A dictionary of tags to write to the raster.
         windowed: bool, optional
             If True, it will write using the windows of the output raster.
             Default is False.
         mask: bool, optional
             If True, set nodata values where 'mask' coordinate equals False.
-        **profile_kwargs
+        **profile_kwargs:
             Additional keyword arguments to pass into writing the raster. The
             nodata, transform, crs, count, width, and height attributes
             are ignored.
+        logger : logger object, optional
+            The logger object used for logging messages. If not provided, the default
+            logger will be used.
 
         """
         for k in ["height", "width", "count", "transform"]:
             if k in profile_kwargs:
                 msg = f"{k} will be set based on the DataArray, remove the argument"
                 raise ValueError(msg)
         da_out = self._obj
@@ -2184,15 +2361,16 @@
 
     def vectorize(self, connectivity=8):
         """Return geometry of grouped pixels with the same value in a DataArray object.
 
         Arguments
         ---------
         connectivity : int, optional
-            Use 4 or 8 pixel connectivity for grouping pixels into features, by default 8
+            Use 4 or 8 pixel connectivity for grouping pixels into features,
+            by default 8
 
         Returns
         -------
         gdf : geopandas.GeoDataFrame
             Geometry of grouped pixels.
         """
         data = self._obj.values
@@ -2206,51 +2384,53 @@
         )
         feats = [
             {"geometry": geom, "properties": {"value": idx}}
             for geom, idx in list(feats_gen)
         ]
         if len(feats) == 0:  # return empty GeoDataFrame
             return gpd.GeoDataFrame()
-        crs = self.crs
-        if crs is None and crs.to_epsg() is not None:
-            crs = crs.to_epsg()  # not all CRS have an EPSG code
-        gdf = gpd.GeoDataFrame.from_features(feats, crs=crs)
+        gdf = gpd.GeoDataFrame.from_features(feats, crs=self.crs)
         gdf.index = gdf.index.astype(self._obj.dtype)
         return gdf
 
 
 @xr.register_dataset_accessor("raster")
 class RasterDataset(XRasterBase):
-    """This is the GIS extension for :class:`xarray.Dataset`"""
+
+    """GIS extension for :class:`xarray.Dataset`."""
 
     @property
     def vars(self):
-        """list: Returns non-coordinate varibles"""
+        """list: Returns non-coordinate varibles."""
         return list(self._obj.data_vars.keys())
 
     def mask_nodata(self):
         """Mask nodata values with np.nan.
+
         Note this will change integer dtypes to float.
         """
         ds_out = self._obj
         for var in self.vars:
             ds_out[var] = ds_out[var].raster.mask_nodata()
         return ds_out
 
     def mask(self, mask):
         """Mask cells where mask equals False with the data nodata value.
-        A warning is raised if no the data has no nodata value."""
+
+        A warning is raised if no the data has no nodata value.
+        """
         ds_out = self._obj
         for var in self.vars:
             ds_out[var] = ds_out[var].raster.mask(mask)
         return ds_out
 
     @staticmethod
     def from_numpy(data_vars, transform, attrs=None, crs=None):
         """Transform multiple numpy arrays to a Dataset object.
+
         The arrays should have identical shape.
 
         Arguments
         ---------
         data_vars: - dict-like
             A mapping from variable names to numpy arrays. The following notations
             are accepted:
@@ -2259,30 +2439,31 @@
             * {var_name: (array-like, nodata)}
             * {var_name: (array-like, nodata, attrs)}
         transform : affine transform
             Two dimensional affine transform for 2D linear mapping
         attrs : dict, optional
             additional global attributes
         crs: int, dict, or str, optional
-            Coordinate Reference System. Accepts EPSG codes (int or str); proj (str or dict)
+            Coordinate Reference System. Accepts EPSG codes (int or str);
+            proj (str or dict)
 
         Returns
         -------
         ds : xr.Dataset
             Dataset of data_vars arrays
         """
         da_lst = list()
         for i, (name, data) in enumerate(data_vars.items()):
             args = ()
             if isinstance(data, tuple):
                 data, args = data[0], data[1:]
             da = RasterDataArray.from_numpy(data, transform, *args)
             da.name = name
             if i > 0 and da.shape[-2:] != da_lst[0].shape[-2:]:
-                raise xr.MergeError(f"Data shapes do not match.")
+                raise xr.MergeError("Data shapes do not match.")
             da_lst.append(da)
         ds = xr.merge(da_lst)
         if attrs is not None:
             ds.attrs.update(attrs)
         if crs is not None:
             ds.raster.set_crs(input_crs=crs)
             ds = ds.raster.reset_spatial_dims_attrs()
@@ -2297,33 +2478,37 @@
         dst_height=None,
         method="nearest",
         align=False,
     ):
         """Reproject a Dataset object, powered by :py:meth:`rasterio.warp.reproject`.
 
         Arguments
-        ----------
+        ---------
         dst_crs: int, dict, or str, optional
             Target CRS. Accepts EPSG codes (int or str); proj (str or dict) or wkt (str)
             "utm" is accepted and will return the centroid utm zone CRS
         dst_res: tuple (x resolution, y resolution) or float, optional
             Target resolution, in units of target CRS.
         dst_transform: affine.Affine(), optional
             Target affine transformation. Will be calculated if None.
-        dst_width, dst_height: int, optional
+        dst_height: int, optional
+            Output file size in pixels and lines. Cannot be used together with
+            resolution (dst_res).
+        dst_width: int, optional
             Output file size in pixels and lines. Cannot be used together with
             resolution (dst_res).
         method: str, optional
-            See :py:meth:`rasterio.warp.reproject` for existing methods, by default nearest.
-            Additionally "nearest_index" can be used for KDTree based downsampling.
+            See :py:meth:`rasterio.warp.reproject` for existing methods,
+            by default nearest. Additionally "nearest_index" can be used
+            for KDTree based downsampling.
         align: boolean, optional
             If True, align target transform to resolution
 
         Returns
-        --------
+        -------
         ds_out : xarray.Dataset
             A reprojected Dataset.
         """
         reproj_kwargs = dict(
             dst_crs=dst_crs,
             dst_res=dst_res,
             dst_transform=dst_transform,
@@ -2343,95 +2528,106 @@
             for var in method:
                 ds[var] = self._obj[var].raster.reproject(
                     method=method[var], **reproj_kwargs
                 )
         return ds
 
     def interpolate_na(self, method: str = "nearest", **kwargs):
-        """Interpolate missing data
+        """Interpolate missing data.
 
         Arguments
-        ----------
+        ---------
         method: {'linear', 'nearest', 'cubic', 'rio_idw'}, optional
             {'linear', 'nearest', 'cubic'} use :py:meth:`scipy.interpolate.griddata`;
-            'rio_idw' applies inverse distance weighting based on :py:meth:`rasterio.fill.fillnodata`.
-        **kwargs
-            Additional key-word arguments are passed to :py:meth:`rasterio.fill.fillnodata`,
-            only used in combination with `method='rio_idw'`
+            'rio_idw' applies inverse distance weighting based on
+            :py:meth:`rasterio.fill.fillnodata`.
+        **kwargs:
+            Additional key-word arguments are passed to
+            :py:meth:`rasterio.fill.fillnodata`, only used in combination
+            with `method='rio_idw'`
 
         Returns
         -------
         xarray.Dataset
             Filled object
         """
         ds_out = xr.Dataset(attrs=self._obj.attrs)
         for var in self.vars:
             ds_out[var] = self._obj[var].raster.interpolate_na(method=method, **kwargs)
         return ds_out
 
     def reproject_like(self, other, method="nearest"):
-        """Reproject a Dataset object to match the resolution, projection,
-        and region of ``other``.
+        """Reproject to match the resolution, projection, and region of ``other``.
 
         Arguments
-        ----------
+        ---------
         other: :xarray.DataArray of Dataset
             DataArray of the target resolution and projection.
         method: dict, optional
             Reproject method mapping. If a string is provided all variables are
             reprojecte with the same method. See
             :py:meth:`~hydromt.raster.RasterDataArray.reproject` for existing methods,
             by default nearest.
 
         Returns
-        --------
+        -------
         ds_out : xarray.Dataset
             Reprojected Dataset
         """
         ds = self._obj
         if self.aligned_grid(other):
             ds = self.clip_bbox(other.raster.bounds)
         elif not self.identical_grid(other):
-            ds = self.reproject(
-                dst_crs=other.raster.crs,
-                dst_transform=other.raster.transform,
-                dst_width=other.raster.width,
-                dst_height=other.raster.height,
-                method=method,
-            )
+            ds_clip = self.clip_bbox(other.raster.transform_bounds(self.crs), buffer=2)
+            if np.any(np.array(ds_clip.raster.shape) < 2):
+                # out of bounds -> return empty dataset
+                if isinstance(other, xr.Dataset):
+                    other = other[list(other.data_vars.keys())[0]]
+                ds = xr.Dataset(attrs=self._obj.attrs)
+                for var in self._obj.data_vars:
+                    ds[var] = full_like(other, nodata=np.nan)
+            else:
+                ds = ds_clip.raster.reproject(
+                    dst_crs=other.raster.crs,
+                    dst_transform=other.raster.transform,
+                    dst_width=other.raster.width,
+                    dst_height=other.raster.height,
+                    method=method,
+                )
         if (
             ds.raster.x_dim != other.raster.x_dim
             or ds.raster.y_dim != other.raster.y_dim
         ):
             # overwrite spatial dimension names which might have been changed
             rm = {
                 ds.raster.x_dim: other.raster.x_dim,
                 ds.raster.y_dim: other.raster.y_dim,
             }
             ds = ds.rename(rm)
             ds.raster.set_spatial_dims(
                 x_dim=other.raster.x_dim, y_dim=other.raster.y_dim
             )
         # make sure coordinates are identical!
-        ds[other.raster.x_dim] = other.raster.xcoords
-        ds[other.raster.y_dim] = other.raster.ycoords
+        xcoords, ycoords = other.raster.xcoords, other.raster.ycoords
+        ds = ds.assign_coords({xcoords.name: xcoords, ycoords.name: ycoords})
         return ds
 
     def reindex2d(self, index):
-        """Return reprojected Dataset object based on simple reindexing using
-        linear indices in ``index``, which can be calculated with
+        """Return reprojected Dataset based on simple reindexing.
+
+        Uses linear indices in ``index``, which can be calculated with
         :py:meth:`~hydromt.raster.RasterDataArray.nearest_index`.
 
         Arguments
-        ----------
+        ---------
         index: xarray.DataArray of intp
             DataArray with flat indices of source DataArray
 
         Returns
-        --------
+        -------
         ds_out : xarray.Dataset
             The reindexed dataset
         """
         ds_out = xr.Dataset(attrs=self._obj.attrs)
         for var in self.vars:
             ds_out[var] = self._obj[var].raster.reindex2d(index=index)
         return ds_out
@@ -2447,42 +2643,48 @@
         prefix="",
         postfix="",
         pcr_vs_map=gis_utils.PCR_VS_MAP,
         logger=logger,
         **profile_kwargs,
     ):
         """Write the Dataset object to one gdal-writable raster files per variable.
+
         The files are written to the ``root`` directory using the following filename
         ``<prefix><variable_name><postfix>.<ext>``.
 
         Arguments
-        ----------
+        ---------
         root : str
             The path to output the raster to. It is created if it does not yet exist.
         driver : str, optional
             The name of the GDAL/rasterio driver to use to export the raster.
             Default is "GTiff".
         dtype : str, optional
             The data type to write the raster to. Default is the datasets dtype.
         tags : dict, optional
             A dictionary of tags to write to the raster.
         windowed : bool, optional
             If True, it will write using the windows of the output raster.
             Default is False.
+        mask: bool
+            Whether to apply the mask to the tasterisation.
         prefix : str, optional
             Prefix to filenames in mapstack
         postfix : str, optional
             Postfix to filenames in mapstack
         pcr_vs_map : dict, optional
             Only for PCRaster driver: <variable name> : <PCRaster type> key-value pairs
             e.g.: {'dem': 'scalar'}, see https://www.gdal.org/frmt_various.html#PCRaster
-        **profile_kwargs
+        **profile_kwargs:
             Additional keyword arguments to pass into writing the raster. The
             nodata, transform, crs, count, width, and height attributes
             are ignored.
+        logger : logger object, optional
+            The logger object used for logging messages. If not provided, the default
+            logger will be used.
 
         """
         if driver not in gis_utils.GDAL_EXT_CODE_MAP:
             raise ValueError(f"Extension unknown for driver: {driver}")
         ext = gis_utils.GDAL_EXT_CODE_MAP.get(driver)
         if not isdir(root):
             os.makedirs(root)
```

### Comparing `hydromt-0.7.1/hydromt/stats/skills.py` & `hydromt-0.8.0/hydromt/stats/skills.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
+"""Implementation of necessary statistical methods."""
 
-import xarray as xr
-import numpy as np
-import pandas as pd
-import calendar
-from datetime import timedelta, datetime
-import bottleneck
 import warnings
 
+import bottleneck
+import numpy as np
+import xarray as xr
+
 warnings.filterwarnings("ignore")
 
 
 # PERFORMANCE METRICS
 def bias(sim, obs, dim="time"):
-    """Returns the bias between two time series.
+    r"""Return the bias between two time series.
 
         .. math::
          Bias=\\frac{1}{N}\\sum_{i=1}^{N}(obs_{i}-sim_{i})
 
     Parameters
     ----------
     sim : xarray DataArray
@@ -39,15 +36,15 @@
     )
     bias = xr.apply_ufunc(_bias, sim, obs, **kwargs)
     bias.name = "bias"
     return bias
 
 
 def percentual_bias(sim, obs, dim="time"):
-    """Returns the percentual bias between two time series.
+    r"""Return the percentual bias between two time series.
 
         .. math::
          PBias= 100 * \\frac{\\sum_{i=1}^{N}(sim_{i}-obs_{i})}{\\sum_{i=1}^{N}(obs_{i})}
 
     Parameters
     ----------
     sim : xarray DataArray
@@ -68,19 +65,21 @@
     )
     pbias = xr.apply_ufunc(_pbias, sim, obs, **kwargs)
     pbias.name = "pbias"
     return pbias
 
 
 def nashsutcliffe(sim, obs, dim="time"):
-    """Returns the Nash-Sutcliffe model efficiency based on a simulated
-    and observed time series.
+    r"""Return the Nash-Sutcliffe model efficiency.
+
+    Efficiency is based on a simulated and observed time series.
 
         .. math::
-         NSE = 1-\\frac{\\sum_{i=1}^{N}(sim_{i}-obs_{i})^2}{\\sum_{i=1}^{N}(obs_{i}-\\bar{obs})^2}
+         NSE = 1-\\frac{\\sum_{i=1}^{N}(sim_{i}-obs_{i})^2}
+         {\\sum_{i=1}^{N}(obs_{i}-\\bar{obs})^2}
 
     Parameters
     ----------
     sim : xarray DataArray
         simulations time series
     obs : xarray DataArray
         observations time series
@@ -98,19 +97,21 @@
     )
     nse = xr.apply_ufunc(_nse, sim, obs, **kwargs)
     nse.name = "nse"
     return nse
 
 
 def lognashsutcliffe(sim, obs, epsilon=1e-6, dim="time"):
-    """Returns the log Nash-Sutcliffe model efficiency based on simulated
-    and observed time series.
+    r"""Return the log Nash-Sutcliffe model efficiency.
+
+    Efficiency calculation is based on simulated and observed time series.
 
         .. math::
-         NSE = 1-\\frac{\\sum_{i=1}^{N}(log(sim_{i})-log(obs_{i}))^2}{\\sum_{i=1}^{N}(log(sim_{i})-log(\\bar{obs})^2}-1)*-1
+         NSE = 1-\\frac{\\sum_{i=1}^{N}(log(sim_{i})-log(obs_{i}))^2}
+         {\\sum_{i=1}^{N}(log(sim_{i})-log(\\bar{obs})^2}-1)*-1
 
     Parameters
     ----------
     sim : xarray DataArray
         simulations time series
     obs : xarray DataArray
         observations time series
@@ -132,15 +133,15 @@
     )
     log_nse = xr.apply_ufunc(_nse, sim, obs, **kwargs)
     log_nse.name = "log_nse"
     return log_nse
 
 
 def pearson_correlation(sim, obs, dim="time"):
-    """Returns the Pearson correlation coefficient of two time series.
+    """Return the Pearson correlation coefficient of two time series.
 
     Parameters
     ----------
     sim : xarray DataArray
         simulations time series
     obs : xarray DataArray
         observations time series
@@ -158,16 +159,15 @@
     )
     pearsonr = xr.apply_ufunc(_pearson_correlation, sim, obs, **kwargs)
     pearsonr.name = "pearson_coef"
     return pearsonr
 
 
 def spearman_rank_correlation(sim, obs, dim="time"):
-    """Returns the spearman rank correlation coefficient of
-    two time series.
+    """Return the spearman rank correlation coefficient of two time series.
 
     Parameters
     ----------
     sim : xarray DataArray
         simulations time series
     obs : xarray DataArray
         observations time series
@@ -185,20 +185,23 @@
     )
     spearmanr = xr.apply_ufunc(_spearman_correlation, sim, obs, **kwargs)
     spearmanr.name = "spearmanr_coef"
     return spearmanr
 
 
 def kge_non_parametric(sim, obs, dim="time"):
-    """Returns the Non Parametric Kling-Gupta Efficiency (KGE, 2018) of two time series with decomposed scores
+    """Return the Non Parametric Kling-Gupta Efficiency (KGE, 2018).
+
+    Calculation is based on the two time series with decomposed scores.
 
     .. ref:
 
         Pool, Vis, and Seibert, 2018 Evaluating model performance: towards
-        a non-parametric variant of the Kling-Gupta efficiency, Hydrological Sciences Journal.
+        a non-parametric variant of the Kling-Gupta efficiency,
+        Hydrological Sciences Journal.
 
     Parameters
     ----------
     sim : xarray DataArray
         simulations time series
     obs : xarray DataArray
         observations time series
@@ -222,20 +225,23 @@
     kge = 1 - np.sqrt((cc - 1) ** 2 + (alpha - 1) ** 2 + (beta - 1) ** 2)
     kge.name = "kge_np"
     ds_out = xr.merge([kge, cc, alpha, beta])
     return ds_out
 
 
 def kge_non_parametric_flood(sim, obs, dim="time"):
-    """Returns the Non Parametric Kling-Gupta Efficiency (KGE, 2018) of two time series optimized for flood peaks using Pearson (see Pool et al., 2018)
+    """Return the Non Parametric Kling-Gupta Efficiency (KGE, 2018) of two time series.
+
+    this KGE is optimized for flood peaks using Pearson (see Pool et al., 2018).
 
     .. ref:
 
         Pool, Vis, and Seibert, 2018 Evaluating model performance: towards
-        a non-parametric variant of the Kling-Gupta efficiency, Hydrological Sciences Journal.
+        a non-parametric variant of the Kling-Gupta efficiency,
+        Hydrological Sciences Journal.
 
     Parameters
     ----------
     sim : xarray DataArray
         simulations time series
     obs : xarray DataArray
         observations time series
@@ -244,15 +250,14 @@
 
     Returns
     -------
     xarray DataSet
         Non Parametric Kling-Gupta Efficiency (2018) optimize for flood peaks
         using pearson (see Pool et al., 2018) and with decomposed score
     """
-    # cc = spearman_rank_correlation(sim, obs)
     cc = pearson_correlation(sim, obs, dim=dim)
     cc.name = "kge_np_flood_pearson_coef"
     kwargs = dict(
         input_core_dims=[[dim], [dim]], dask="parallelized", output_dtypes=[float]
     )
     alpha = xr.apply_ufunc(_fdc_alpha, sim, obs, **kwargs)
     alpha.name = "kge_np_flood_rel_var"
@@ -261,18 +266,20 @@
     kge = 1 - np.sqrt((cc - 1) ** 2 + (alpha - 1) ** 2 + (beta - 1) ** 2)
     kge.name = "kge_np_flood"
     ds_out = xr.merge([kge, cc, alpha, beta])
     return ds_out
 
 
 def rsquared(sim, obs, dim="time"):
-    """Returns the coefficient of determination of two time series.
+    r"""Return the coefficient of determination of two time series.
 
         .. math::
-         r^2=(\\frac{\\sum ^n _{i=1}(e_i - \\bar{e})(s_i - \\bar{s})}{\\sqrt{\\sum ^n _{i=1}(e_i - \\bar{e})^2} \\sqrt{\\sum ^n _{i=1}(s_i - \\bar{s})^2}})^2
+         r^2=(\\frac{\\sum ^n _{i=1}(e_i - \\bar{e})(s_i - \\bar{s})}
+         {\\sqrt{\\sum ^n _{i=1}(e_i - \\bar{e})^2}
+         \\sqrt{\\sum ^n _{i=1}(s_i - \\bar{s})^2}})^2
 
     Parameters
     ----------
     sim : xarray DataArray
         simulations time series
     obs : xarray DataArray
         observations time series
@@ -287,15 +294,15 @@
     # R2 equals the square of the Pearson correlation coefficient between obs and sim
     rsquared = pearson_correlation(sim, obs, dim=dim) ** 2
     rsquared.name = "rsquared"
     return rsquared
 
 
 def mse(sim, obs, dim="time"):
-    """Returns the mean squared error (MSE) between two time series.
+    r"""Return the mean squared error (MSE) between two time series.
 
         .. math::
          MSE=\\frac{1}{N}\\sum_{i=1}^{N}(e_{i}-s_{i})^2
 
     Parameters
     ----------
     sim : xarray DataArray
@@ -316,15 +323,15 @@
     )
     mse = xr.apply_ufunc(_mse, sim, obs, **kwargs)
     mse.name = "mse"
     return mse
 
 
 def rmse(sim, obs, dim="time"):
-    """Returns the root mean squared error between two time series.
+    r"""Return the root mean squared error between two time series.
 
         .. math::
          RMSE=\\sqrt{\\frac{1}{N}\\sum_{i=1}^{N}(e_{i}-s_{i})^2}
 
     Parameters
     ----------
     sim : xarray DataArray
@@ -341,15 +348,15 @@
     """
     rmse = np.sqrt(mse(sim, obs, dim=dim))
     rmse.name = "rmse"
     return rmse
 
 
 def kge(sim, obs, dim="time"):
-    """Returns the Kling-Gupta Efficiency (KGE) of two time series
+    r"""Return the Kling-Gupta Efficiency (KGE) of two time series.
 
     .. ref:
 
         Gupta, Kling, Yilmaz, Martinez, 2009, Decomposition of the mean
         squared error and NSE performance criteria: Implications for improving
         hydrological modelling.
 
@@ -376,15 +383,15 @@
     kge = 1 - np.sqrt((cc - 1) ** 2 + (alpha - 1) ** 2 + (beta - 1) ** 2)
     kge.name = "kge"
     ds_out = xr.merge([kge, cc, alpha, beta])
     return ds_out
 
 
 def kge_2012(sim, obs, dim="time"):
-    """Returns the Kling-Gupta Efficiency (KGE, 2012) of two time series
+    r"""Return the Kling-Gupta Efficiency (KGE, 2012) of two time series.
 
     .. ref:
 
         Kling, H., Fuchs, M., & Paulin, M. (2012). Runoff conditions in the
         upper Danube basin under an ensemble of climate change scenarios.
         Journal of Hydrology, 424, 264-277, doi:10.1016/j.jhydrol.2012.01.011.
 
@@ -441,28 +448,28 @@
 def _fdc_alpha(sim, obs, axis=-1):
     fdc_s = np.sort(sim, axis=axis) / (np.nanmean(sim, axis=axis) * len(sim))
     fdc_o = np.sort(obs, axis=axis) / (np.nanmean(obs, axis=axis) * len(obs))
     return 1 - 0.5 * np.nansum(np.abs(fdc_s - fdc_o), axis=axis)
 
 
 def _bias(sim, obs, axis=-1):
-    """bias"""
+    """Bias."""
     return np.nansum(sim - obs, axis=axis) / np.nansum(np.isfinite(obs), axis=axis)
 
 
 def _pbias(sim, obs, axis=-1):
-    """percentual bias"""
+    """Percentual bias."""
     return np.nansum(sim - obs, axis=axis) / np.nansum(obs, axis=axis)
 
 
 def _mse(sim, obs, axis=-1):
-    """mean squared error"""
+    """Mean squared error."""
     mse = np.nansum((obs - sim) ** 2, axis=axis)
     return mse
 
 
 def _nse(sim, obs, axis=-1):
-    """nash-sutcliffe efficiency"""
+    """nash-sutcliffe efficiency."""
     obs_mean = np.nanmean(obs, axis=axis)
     a = np.nansum((sim - obs) ** 2, axis=axis)
     b = np.nansum((obs - obs_mean[..., None]) ** 2, axis=axis)
     return 1 - a / b
```

### Comparing `hydromt-0.7.1/hydromt/vector.py` & `hydromt-0.8.0/hydromt/vector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,50 @@
+"""Implementaion of the vector workloads."""
 from __future__ import annotations
-from typing import Union, Any
+
+import logging
+from typing import Any, Union
+
+import geopandas as gpd
 import numpy as np
+import pyproj
+import shapely
 import xarray as xr
-import geopandas as gpd
-from geopandas import GeoSeries, GeoDataFrame
+from geopandas import GeoDataFrame, GeoSeries
+
+# TODO try getting this version without importing osgeo to avoid
+# conflicts with geopandas/rasterio
+from osgeo import __version__ as GDAL_VERSION
 from shapely.geometry.base import BaseGeometry
-import shapely
-import pyproj
-import logging
 
 from hydromt import gis_utils, raster
 
-# TODO try getting this version without importing osgeo to avoid conflicts with geopandas/rasterio
-from osgeo import __version__ as GDAL_VERSION
-
 logger = logging.getLogger(__name__)
 
 
 class GeoBase(raster.XGeoBase):
+
+    """Base accessor class for geo data."""
+
     def __init__(self, xarray_obj):
+        """Initialize a new object based on the provided xarray_obj."""
         super(GeoBase, self).__init__(xarray_obj)
         self._geometry = None
 
     @property
     def _all_names(self):
-        """Return names of all variables and coordinates in the dataset/array"""
+        """Return names of all variables and coordinates in the dataset/array."""
         # TODO: move to geobase
         names = [n for n in self._obj.coords]
         if isinstance(self._obj, xr.Dataset):
             names = names + [n for n in self._obj.data_vars]
         return names
 
     def _get_geom_names_types(self, geom_name: str = None) -> tuple[list, list]:
-        """Discover coordinates with wkt/geom type data the dataset/array"""
+        """Discover coordinates with wkt/geom type data the dataset/array."""
         names, types = [], []
         dvars = self._all_names if geom_name is None else [geom_name]
         for name in dvars:
             if self._obj[name].ndim == 1 and isinstance(
                 self._obj[name][0].values.item(), BaseGeometry
             ):
                 names.append(name)
@@ -49,15 +57,15 @@
                     names.append(name)
                     types.append("wkt")
                 except Exception:
                     pass
         return names, types
 
     def _discover_xy(self, x_name=None, y_name=None, index_dim=None):
-        """Discover xy type geometries in the dataset/array"""
+        """Discover xy type geometries in the dataset/array."""
         # infer x dim
         if x_name is None:
             for name in raster.XDIMS:
                 if name in self._all_names:
                     dim0 = (
                         index_dim if index_dim is not None else self._obj[name].dims[0]
                     )
@@ -85,15 +93,15 @@
         else:
             self.attrs.pop("x_name", None)
             self.attrs.pop("y_name", None)
             self.attrs.pop("geom_format", None)
             self.attrs.pop("index_dim", None)
 
     def _discover_geom(self, geom_name=None, index_dim=None):
-        """Discover geom/wkt type geometries in the dataset/array"""
+        """Discover geom/wkt type geometries in the dataset/array."""
         # check /infer geom dim
         names, types = self._get_geom_names_types(geom_name=geom_name)
         if geom_name is None:
             if index_dim is not None:
                 names = [name for name in names if self._obj[name].dims[0] == index_dim]
             # priority for geometry named variable/coord
             if "geometry" in names:
@@ -123,17 +131,21 @@
         y_name: str = None,
         index_dim: str = None,
         geom_format: str = None,
     ) -> None:
         """Set the spatial and index dimensions of the object.
 
         Arguments
-        ----------
-        x_name, y_name, geom_name: str, optional
-            The name of the x, y and geometry coordinate.
+        ---------
+        x_name: str, optional
+            The name of the x coordinate.
+        y_name: str, optional
+            The name of the ycoordinate.
+        geom_name: str, optional
+            The name of the geometry coordinate.
         index_dim: str optional
             The name of the geometry index dimension
         geom_format: {'xy', 'wkt', 'geom'}
             Geometry format
         """
         if geom_format != "xy":
             self._discover_geom(geom_name=geom_name, index_dim=index_dim)
@@ -159,15 +171,15 @@
         if self.get_attrs("geom_name") not in self._obj.dims:
             self.set_spatial_dims()
         if "geom_name" in self.attrs:
             return self.attrs["geom_name"]
 
     @property
     def geom_type(self) -> str:
-        """Return geometry type"""
+        """Return geometry type."""
         geom_types = self.geometry.type.values
         if len(set(geom_types)) > 1:
             # TODO: can we safely assume there is multi geom?
             i = ["MULTI" in g.upper() for g in geom_types].index(True)
             geom_type = geom_types[i]
         else:
             geom_type = geom_types[0]
@@ -216,30 +228,30 @@
                     tdims.append(dim)
             if len(tdims) == 1:
                 self.set_attrs(time_dim=tdims[0])
         return self.get_attrs("time_dim")
 
     @property
     def index(self):
-        """Return the index values"""
+        """Return the index values."""
         return self._obj[self.index_dim]
 
     @property
     def size(self):
-        """Return the length of the index array"""
+        """Return the length of the index array."""
         return self._obj[self.index_dim].size
 
     @property
     def bounds(self):
         """Return the bounds (xmin, ymin, xmax, ymax) of the object."""
         return self.geometry.total_bounds
 
     @property
     def geometry(self) -> GeoSeries:
-        """Return the geometry of the dataset or array as GeoSeries
+        """Return the geometry of the dataset or array as GeoSeries.
 
         Returns
         -------
         GeoSeries
             A Series object with shapely geometries
         """
         if self._geometry is not None and self._geometry.index.size == self.size:
@@ -275,16 +287,18 @@
         geometry: GeoSeries = None,
         geom_format: str = None,
         x_name: str = None,
         y_name: str = None,
         geom_name: str = None,
         replace: bool = True,
     ):
-        """Update the geometry in the Dataset/Array with a new geometry (if provided)
-        or update the current geometry to a new geometry format.
+        """Update the geometry in the Dataset/Array with a new geometry.
+
+        if provided or use that, otherwise update the current
+        geometry to a new geometry format.
 
 
         Parameters
         ----------
         geometry : GeoSeries, optional
             New geometry, by default None
         geom_format: {'xy', 'wkt', 'geom'}
@@ -300,15 +314,15 @@
             Update GeoDataset/Array
         """
         if geom_format is None:
             geom_format = self.geom_format
         if geometry is None:
             geometry = self.geometry
         elif not isinstance(geometry, GeoSeries):
-            raise ValueError(f"geometry should be a GeoSeries object")
+            raise ValueError("geometry should be a GeoSeries object")
         elif geometry.size != self.size:
             raise ValueError(
                 f'The sizes of geometry and index dim "{self.index_dim}" do not match'
             )
 
         # update geometry and drop old
         drop_vars = []
@@ -360,15 +374,15 @@
         )
         obj.vector.set_crs(geometry.crs)
         return obj
 
     # Internal conversion and selection methods
     # i.e. produces xarray.Dataset/ xarray.DataArray
     def ogr_compliant(self, reducer=None) -> xr.Dataset:
-        """Creates a Dataset/Array which is understood by OGR.
+        """Create a Dataset/Array which is understood by OGR.
 
         Variables with more than one dimension are not understood and will
         removed if no reducer is provided.
 
         Parameters
         ----------
         reducer : callable, optional
@@ -397,15 +411,15 @@
 
         if reducer is not None:
             rdims = [dim for dim in obj.dims if dim != index_dim]
             obj = obj.reduce(reducer, dim=rdims)
 
         dtypes = {"i": "Integer64", "f": "Real", "U": "String"}
         for name, da in obj.data_vars.items():
-            if not index_dim in da.dims:
+            if index_dim not in da.dims:
                 continue
             if reducer is not None:
                 rdims = [dim for dim in obj.dims if dim != index_dim]
                 obj[name] = obj[name].reduce(reducer, rdims)
             # set ogr meta data
             dtype = dtypes.get(obj[name].dtype.kind, None)
             if dtype is not None:
@@ -430,15 +444,15 @@
                 "ogr_geometry_field": "ogc_wkt",
                 "ogr_layer_type": f"{self.geom_type}",
             }
         )
         return obj
 
     def to_geom(self, geom_name: str = None) -> Union[xr.DataArray, xr.Dataset]:
-        """Converts Dataset/ DataArray with xy or wkt geometries to shapely Geometries.
+        """Convert Dataset/ DataArray with xy or wkt geometries to shapely Geometries.
 
         Parameters
         ----------
         geom_name: str, optional
             The name of the geometry coordinate.
             If None (default), derived from current object or default to 'geometry'.
 
@@ -446,15 +460,15 @@
         -------
         xr.Dataset
             Dataset with new geometry coordinates
         """
         return self.update_geometry(geom_format="geom", geom_name=geom_name)
 
     def to_xy(self, x_name="x", y_name="y") -> Union[xr.DataArray, xr.Dataset]:
-        """Converts Dataset/ DataArray with Point geometries to x,y structure.
+        """Convert Dataset/ DataArray with Point geometries to x,y structure.
 
         Parameters
         ----------
         x_name, y_name: str, optional
             The name of the x and y coordinates.
 
         Returns
@@ -465,15 +479,15 @@
         return self.update_geometry(geom_format="xy", x_name=x_name, y_name=y_name)
 
     def to_wkt(
         self,
         ogr_compliant=False,
         reducer=None,
     ) -> Union[xr.DataArray, xr.Dataset]:
-        """Converts geometries in Dataset/DataArray to wkt strings.
+        """Convert geometries in Dataset/DataArray to wkt strings.
 
         Parameters
         ----------
         ogr_compliant: bool, optional
             Whether to create a OGR compliant Dataset/Array
             see :py:meth:`~hydromt.vector.GeoBase.ogr_compliant` for more details.
         reducer : callable, optional
@@ -502,32 +516,34 @@
             A geometry defining the area of interest.
         predicate : {None, 'intersects', 'within', 'contains', \
                      'overlaps', 'crosses', 'touches'}, optional
             If predicate is provided, the input geometry is tested
             using the predicate function against each item in the
             index whose extent intersects the envelope of the input geometry:
             predicate(input_geometry, tree_geometry).
-        
+
         Returns
         -------
         da: xarray.DataArray
             Clipped DataArray
         """
         idx = gis_utils.filter_gdf(self.geometry, geom=geom, predicate=predicate)
         return self._obj.isel({self.index_dim: idx})
 
     def clip_bbox(self, bbox, crs=None, buffer=None):
         """Select point locations to bounding box.
 
         Arguments
-        ----------
+        ---------
         bbox: tuple of floats
             (xmin, ymin, xmax, ymax) bounding box
         buffer: float, optional
             buffer around bbox in crs units, None by default.
+        crs : int, optional
+            EPSG of the data. If not given, it will be inferred.
 
         Returns
         -------
         da: xarray.DataArray
             Clipped DataArray
         """
         if buffer is not None:
@@ -543,15 +559,15 @@
     # TODO write general wrapper
     def to_crs(self, dst_crs):
         """Transform spatial coordinates to a new coordinate reference system.
 
         The ``crs`` attribute on the current GeoDataArray must be set.
 
         Arguments
-        ----------
+        ---------
         dst_crs: int, dict, or str, optional
             Accepts EPSG codes (int or str); proj (str or dict) or wkt (str)
 
         Returns
         -------
         xr.DataArray
             DataArray with transformed geospatial coordinates
@@ -563,17 +579,19 @@
 
     # Constructers
     # i.e. from other datatypes or files
 
     ## Output methods
     ## Either writes to files or other data types
     def to_gdf(self, reducer=None):
-        """Return geopandas GeoDataFrame with Point geometry based on Dataset
-        coordinates. If a reducer is passed the Dataset variables are reduced along
-        the all non-index dimensions and to a GeoDataFrame column.
+        """Return geopandas GeoDataFrame with Point geometry.
+
+        Geometry is based on Dataset coordinates. If a reducer is
+        passed the Dataset variables are reduced along the all
+        non-index dimensions and to a GeoDataFrame column.
 
         Arguments
         ---------
         reducer : callable, optional
             method by which multidimensional data is reduced to 1 dimensional
             e.g. numpy.mean
 
@@ -612,57 +630,87 @@
     def to_netcdf(
         self,
         path: str,
         ogr_compliant: bool = False,
         reducer=None,
         **kwargs,
     ) -> None:
-        """Export geodataset vectordata to an ogr compliant netCDF4 file
+        """Export geodataset vectordata to an ogr compliant netCDF4 file.
 
         Parameters
         ----------
         path : str
             Output path for netcdf file.
         ogr_compliant : bool
             write the netCDF4 file in an ogr compliant format
             This makes it readable as a vector file in e.g. QGIS
             see :py:meth:`~hydromt.vector.GeoBase.ogr_compliant` for more details.
         reducer : callable, optional
             Method by which multidimensional data is reduced to 1 dimensional
             e.g. numpy.mean
+        kwargs:
+            Any additional arguments to be passed down to the driver.
         """
         if ogr_compliant:
             self.ogr_compliant(reducer=reducer).to_netcdf(
                 path, engine="netcdf4", **kwargs
             )
         else:
             obj = self.update_geometry(geom_format="wkt", geom_name="ogc_wkt")
             obj.to_netcdf(path, engine="netcdf4", **kwargs)
             del obj
 
 
 @xr.register_dataarray_accessor("vector")
 class GeoDataArray(GeoBase):
+
+    """Accessor class for vector based geo data arrays."""
+
     def __init__(self, xarray_obj):
+        """Initialise the object."""
         super(GeoDataArray, self).__init__(xarray_obj)
 
+    @property
+    def nodata(self):
+        """Nodata value of the DataArray."""
+        return self._obj.attrs.get("_FillValue", None)
+
+    def set_nodata(self, nodata=None):
+        """Set the nodata value of the DataArray.
+
+        Parameters
+        ----------
+        nodata : float, int, opional
+            nodata value
+        """
+        # Only numerical nodata values are supported
+        if np.issubdtype(type(nodata), np.number):
+            if not np.issubdtype(type(nodata), self._obj.dtype):
+                nodata = self._obj.dtype.type(nodata)
+            self._obj.attrs["_FillValue"] = nodata
+        else:
+            logger.warning("No numerical nodata value found, skipping set_nodata")
+            self._obj.attrs.pop("_FillValue", None)
+
     # Constructers
     # i.e. from other datatypes or files
     @staticmethod
     def from_gdf(
         gdf: gpd.GeoDataFrame,
         data: Any,
         coords: dict = None,
         dims: tuple = None,
         name: str = None,
         index_dim: str = None,
         keep_cols: bool = True,
+        merge_index: str = "gdf",
     ) -> xr.DataArray:
-        """Parse GeoDataFrame object with point geometries to DataArray with
-        geospatial attributes and merge with array_like data.
+        """Parse GeoDataFrame object with point geometries to DataArray.
+
+        DataArray will have geospatial attributes and be merged with array_like data.
 
         Arguments
         ---------
         gdf: geopandas GeoDataFrame
             Spatial coordinates. The index should match the array_like index_dim and the
             geometry column may only contain Point geometries.
         data: array_like
@@ -674,49 +722,73 @@
         coords: sequence or dict of array_like, optional
             Coordinates (tick labels) to use for indexing along each dimension.
         dims: hashable or sequence of hashable, optional
             Name(s) of the data dimension(s). Must be either a hashable (only
             for 1D data) or a sequence of hashables with length equal to the
             number of dimensions. If this argument is omitted, dimension names
             default to ``['dim_0', ... 'dim_n']``.
+        name: str, optional
+            The name of the data set for metadata purposes.
         index_dim: str, optional
             Name of index dimension of data
         keep_cols: bool, optional
             If True, keep gdf columns as extra coordinates in dataset
+        merge_index: {'gdf', 'inner'}, default 'gdf'
+            Type of merge to be performed between gdf and data.
+
+            * gdf: use only keys from gdf index. Missing values will be filled with NaNs
+            * inner: use intersection of gdf and data index.
 
         Returns
         -------
         da: xarray.DataArray
             DataArray with geospatial coordinates
         """
+        # parse gdf to dataset
+        if isinstance(gdf, GeoSeries):
+            if gdf.name is None:
+                gdf.name = "geometry"
+            gdf = gdf.to_frame()
+        if not isinstance(gdf, GeoDataFrame):
+            raise ValueError(f"gdf data type not understood {type(gdf)}")
+        # check index_dim
         if index_dim is None:
             index_dim = gdf.index.name if gdf.index.name is not None else "index"
         geom_name = gdf.geometry.name
         # create DataArray from array_like data
         da = xr.DataArray(data=data, coords=coords, dims=dims, name=name)
         # check dims -> assume index dim is first dim if not provided
-        if dims is None and index_dim not in da.dims:
+        if dims is None and index_dim not in da.dims and len(da.dims) > 0:
             da = da.rename({list(da.dims)[0]: index_dim})
         # check if all data array contain index_dim
         if index_dim not in da.dims:
             raise ValueError(f"Index dimension {index_dim} not found on DataArray.")
         if np.dtype(da[index_dim]).type != np.dtype(gdf.index).type:
             try:
                 da[index_dim] = da[index_dim].astype(np.dtype(gdf.index).type)
             except TypeError:
                 raise TypeError(
                     "DataArray and GeoDataFrame index datatypes do not match."
                 )
-        # set gdf geometry and optional other columns
-        if keep_cols:
-            hdrs = gdf.columns
+        # Which indices to use
+        gdf_index = gdf.index.values
+        ds_index = da[index_dim].values
+        intersect_index = np.intersect1d(gdf_index, ds_index)
+        if merge_index == "gdf":
+            _index = gdf_index
+        elif merge_index == "inner":
+            _index = intersect_index
         else:
-            hdrs = [geom_name]
-        da = da.assign_coords({hdr: (index_dim, gdf[hdr]) for hdr in hdrs})
-        da = da.transpose(index_dim, ...).reindex({index_dim: gdf.index})
+            raise ValueError(f"{merge_index} is not a valid value for 'merge_index'")
+        if len(intersect_index) == 0:
+            raise ValueError("No common indices found between gdf and data.")
+        da = da.reindex({index_dim: _index}).transpose(index_dim, ...)
+        # set gdf geometry and optional other columns
+        hdrs = gdf.columns if keep_cols else [geom_name]
+        da = da.assign_coords({hdr: (index_dim, gdf.loc[_index, hdr]) for hdr in hdrs})
         # set geospatial attributes
         da.vector.set_spatial_dims(geom_name=geom_name, geom_format="geom")
         da.vector.set_crs(gdf.crs)
         return da
 
     @staticmethod
     def from_netcdf(
@@ -724,22 +796,23 @@
         parse_geom: bool = True,
         geom_name: str = None,
         x_name: str = None,
         y_name: str = None,
         crs: int = None,
         **kwargs,
     ) -> xr.DataArray:
-        """Read netcdf file as GeoDataArray
+        """Read netcdf file as GeoDataArray.
 
         Parameters
         ----------
         path : str
             path to file
         parse_geom : bool, optional
-            Create geometry objects in place of existing x, y or wkt geometry coordinates.
+            Create geometry objects in place of existing x, y or wkt geometry
+            coordinates.
         x_name, y_name, geom_name: str, optional
             The name of the x, y and geometry coordinate.
         crs : int, optional
             EPSG of the data. If not given, it will be inferred.
         **kwargs
             passed to :py:func:`xarray.open_dataarray`
 
@@ -755,120 +828,148 @@
             da = da.vector.update_geometry(geom_format="geom", replace=True)
         da.vector.set_crs(input_crs=crs)  # try to parse from netcdf if None
         return da
 
 
 @xr.register_dataset_accessor("vector")
 class GeoDataset(GeoBase):
+
+    """Implementation for a vectorased geo dataset."""
+
     def __init__(self, xarray_obj):
+        """Initialise the object."""
         super(GeoDataset, self).__init__(xarray_obj)
 
     # Properties
     # Will probably be deleted in the future but now needed for compatibility
     @property
     def vars(self):
-        """list: Returns non-coordinate varibles"""
+        """list: Returns non-coordinate varibles."""
         return list(self._obj.data_vars.keys())
 
     # Internal conversion and selection methods
     # i.e. produces xarray.Dataset/ xarray.DataArray
 
     # Constructers
     # i.e. from other datatypes or filess
     @staticmethod
     def from_gdf(
         gdf: gpd.GeoDataFrame,
-        data_vars: dict = {},
+        data_vars: dict = None,
         coords: dict = None,
         index_dim: str = None,
         keep_cols: bool = True,
+        merge_index: str = "gdf",
     ) -> xr.Dataset:
-        """Creates Dataset with geospatial coordinates. The Dataset values are
-        reindexed to the gdf index.
+        """Create Dataset with geospatial coordinates.
 
         Arguments
         ---------
         gdf: geopandas GeoDataFrame
             Spatial coordinates. The index should match the df index and the geometry
             columun may only contain Point geometries. Additional columns are also
             parsed to the xarray DataArray coordinates.
         data_vars: dict-like, DataArray or Dataset
             A mapping from variable names to `xarray.DataArray` objects.
             See `xarray.Dataset` for all options.
-            Aditionally it accepts `xarray.DataArray` with name property and `xarray.Dataset`.
+            Aditionally it accepts `xarray.DataArray` with name property and
+            `xarray.Dataset`.
         coords: sequence or dict of array_like, optional
             Coordinates (tick labels) to use for indexing along each dimension.
         index_dim: str, optional
             Name of index dimension in data_vars
         keep_cols: bool, optional
             If True, keep gdf columns as extra coordinates in dataset
+        merge_index: {'gdf', 'inner'}, default 'gdf'
+            Type of merge to be performed between gdf and data.
+
+            * gdf: use only keys from gdf index. Missing values will be filled with NaNs
+            * inner: use intersection of gdf and data index.
 
         Returns
         -------
         da: xarray.Dataset
             Dataset with geospatial coordinates
         """
         # parse gdf to dataset
         if isinstance(gdf, GeoSeries):
             if gdf.name is None:
                 gdf.name = "geometry"
             gdf = gdf.to_frame()
         if not isinstance(gdf, GeoDataFrame):
             raise ValueError(f"gdf data type not understood {type(gdf)}")
+        # check index_dim
         if index_dim is None:
             index_dim = gdf.index.name if gdf.index.name is not None else "index"
         geom_name = gdf.geometry.name
-        if not keep_cols:
-            gdf = gdf[[geom_name]]
-        ds = gdf.to_xarray().set_coords(gdf.columns)
         # parse data_vars to dataset
-        if data_vars is not None and len(data_vars) > 0:
+        if data_vars is not None:
             if isinstance(data_vars, xr.DataArray):
-                data_vars = data_vars.to_dataset()
+                ds = data_vars.to_dataset()
             elif isinstance(data_vars, xr.Dataset):
-                pass
+                ds = data_vars
             else:
-                data_vars = xr.Dataset(data_vars, coords=coords)
-            # check if any data array contain index_dim
-            if index_dim not in data_vars.dims:
-                raise ValueError(f"Index dimension {index_dim} not found in dataset.")
-            if np.dtype(data_vars[index_dim]).type != np.dtype(gdf.index).type:
                 try:
-                    data_vars[index_dim] = data_vars[index_dim].astype(
-                        np.dtype(gdf.index).type
+                    ds = xr.Dataset(data_vars, coords=coords)
+                except TypeError:
+                    raise TypeError(
+                        "data_vars should be a dict-like, DataArray or Dataset"
                     )
+            # check if any data array contain index_dim
+            if index_dim not in ds.dims:
+                raise ValueError(f"Index dimension {index_dim} not found in data_vars.")
+            if np.dtype(ds[index_dim]).type != np.dtype(gdf.index).type:
+                try:
+                    ds[index_dim] = ds[index_dim].astype(np.dtype(gdf.index).type)
                 except TypeError:
                     raise TypeError(
                         "Dataset and GeoDataFrame index datatypes do not match."
                     )
-        # combine both, transpose and reindex
-        ds = ds.assign(data_vars)
-        ds = ds.transpose(index_dim, ...).reindex({index_dim: gdf.index})
+        else:  # create empty dataset
+            ds = xr.Dataset(coords={index_dim: gdf.index.values})
+        # Which indices to use
+        gdf_index = gdf.index.values
+        ds_index = ds[index_dim].values
+        intersect_index = np.intersect1d(gdf_index, ds_index)
+        if merge_index == "gdf":
+            _index = gdf_index
+        elif merge_index == "inner":
+            _index = intersect_index
+        else:
+            raise ValueError(f"{merge_index} is not a valid value for 'merge_index'")
+        if len(intersect_index) == 0:
+            raise ValueError("No common indices found between gdf and data_vars.")
+        ds = ds.reindex({index_dim: _index}).transpose(index_dim, ...)
+        # set gdf geometry and optional other columns
+        hdrs = gdf.columns if keep_cols else [geom_name]
+        ds = ds.assign_coords({hdr: (index_dim, gdf.loc[_index, hdr]) for hdr in hdrs})
+        # set geospatial attributes
         ds.vector.set_spatial_dims(geom_name=geom_name, geom_format="geom")
         ds.vector.set_crs(gdf.crs)
         return ds
 
     @staticmethod
     def from_netcdf(
         path: str,
         parse_geom=True,
         geom_name=None,
         x_name=None,
         y_name=None,
         crs=None,
         **kwargs,
     ) -> xr.Dataset:
-        """Create GeoDataset from ogr compliant netCDF4 file
+        """Create GeoDataset from ogr compliant netCDF4 file.
 
         Parameters
         ----------
         path : str
             Path to the netCDF4 file
         parse_geom : bool, optional
-            Create geometry objects in place of existing x, y or wkt geometry coordinates.
+            Create geometry objects in place of existing x, y or
+            wkt geometry coordinates.
         x_name, y_name, geom_name: str, optional
             The name of the x, y and geometry coordinate.
         crs : int, optional
             EPSG of the data. If not given, it will be inferred.
         **kwargs
             passed to :py:func:`xarray.open_dataset`
```

### Comparing `hydromt-0.7.1/hydromt/workflows/basin_mask.py` & `hydromt-0.8.0/hydromt/workflows/basin_mask.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 # -*- coding: utf-8 -*-
-"""Scripts to derive (sub)basin geometries from pre-cooked basin index files, 
-basin maps or flow direction maps.
+"""Scripts to derive (sub)basin geometries.
+
+Based on pre-cooked basin index files, basin maps or flow direction maps.
 """
 
+import logging
+import warnings
 from os.path import isdir, isfile
 from pathlib import Path
-import numpy as np
+
 import geopandas as gpd
-from shapely.geometry import box
+import numpy as np
 import xarray as xr
-import logging
-import warnings
+from shapely.geometry import box
+
+from ..data_adapter import GeoDataFrameAdapter
+from ..flw import basin_map, flwdir_from_da, outlet_map, stream_map
 
 # local
 from ..io import open_raster
-from ..flw import flwdir_from_da, basin_map, stream_map, outlet_map
-from ..data_adapter import GeoDataFrameAdapter
 from ..models import MODELS
 
 logger = logging.getLogger(__name__)
 
 __all__ = ["get_basin_geometry", "parse_region"]
 
 
 def parse_region(region, logger=logger):
-    """Checks and returns parsed region arguments.
+    """Check and return parsed region arguments.
 
     Parameters
     ----------
     region : dict
         Dictionary describing region of interest.
 
         For an exact clip of the region:
@@ -41,19 +44,21 @@
 
         * {'<model_name>': root}
 
         For a region based of the grid of a raster file:
 
         * {'grid': /path/to/raster}
 
-        Entire basin can be defined based on an ID, one or multiple point location (x, y),
-        or a region of interest (bounding box or geometry) for which the basin IDs are
-        looked up. The basins withint the area of interest can be further filtered to
-        only include basins with their outlet within the area of interest ('outlets': true)
-        of stream threshold arguments (e.g.: 'uparea': 1000). Common use-cases include:
+        Entire basin can be defined based on an ID, one or multiple point location
+        (x, y), or a region of interest (bounding box or geometry) for which the
+        basin IDs are looked up. The basins withint the area of interest can be further
+        filtered to only include basins with their outlet within the area of interest
+        ('outlets': true) of stream threshold arguments (e.g.: 'uparea': 1000).
+
+        Common use-cases include:
 
         * {'basin': ID}
 
         * {'basin': [ID1, ID2, ..]}
 
         * {'basin': [x, y]}
 
@@ -66,38 +71,44 @@
         * {'basin': [xmin, ymin, xmax, ymax], 'outlets': true}
 
         * {'basin': [xmin, ymin, xmax, ymax], '<variable>': threshold}
 
         Subbasins are defined by its outlet locations and include all area upstream
         from these points. The outlet locations can be passed as xy coordinate pairs,
         but also derived from the most downstream cell(s) within a area of interest
-        defined by a bounding box or geometry, optionally refined by stream threshold arguments.
+        defined by a bounding box or geometry, optionally refined by stream threshold
+        arguments.
 
         The method can be speed up by providing an additional ``bounds`` argument which
         should contain all upstream cell. If cells upstream of the subbasin are not
         within the provide bounds a warning will be raised. Common use-cases include:
 
         * {'subbasin': [x, y], '<variable>': threshold}
 
-        * {'subbasin': [[x1, x2, ..], [y1, y2, ..]], '<variable>': threshold, 'bounds': [xmin, ymin, xmax, ymax]}
+        * {
+            'subbasin': [[x1, x2, ..], [y1, y2, ..]],
+            '<variable>': threshold, 'bounds': [xmin, ymin, xmax, ymax]
+            }
 
         * {'subbasin': /path/to/point_geometry, '<variable>': threshold}
 
         * {'subbasin': [xmin, ymin, xmax, ymax], '<variable>': threshold}
 
         * {'subbasin': /path/to/polygon_geometry, '<variable>': threshold}
 
-        Interbasins are similar to subbasins but are bounded by a bounding box or geometry
-        and do not include all upstream area. Common use-cases include:
+        Interbasins are similar to subbasins but are bounded by a bounding box or
+        geometry and do not include all upstream area. Common use-cases include:
 
         * {'interbasin': [xmin, ymin, xmax, ymax], '<variable>': threshold}
 
         * {'interbasin': [xmin, ymin, xmax, ymax], 'xy': [x, y]}
 
         * {'interbasin': /path/to/polygon_geometry, 'outlets': true}
+    logger:
+        The logger to use.
 
     Returns
     -------
     kind : {'basin', 'subbasin', 'interbasin', 'geom', 'bbox', 'grid'}
         region kind
     kwargs : dict
         parsed region json
@@ -201,15 +212,15 @@
     basins_name="basins",
     flwdir_name="flwdir",
     ftype="infer",
     logger=logger,
     buffer=10,
     **stream_kwargs,
 ):
-    """Returns a geometry of the (sub)(inter)basin(s).
+    """Return a geometry of the (sub)(inter)basin(s).
 
     This method derives a geometry of sub-, inter- or full basin based on an input
     dataset with flow-direction and optional basins ID raster data in combination
     with a matching basin geometry file containing the bounding boxes of each basin.
 
     Either ``bbox``, ``geom``, ``xy`` (or ``basid`` in case of ``kind='basin'``) must
     be provided.
@@ -240,14 +251,18 @@
         Name of flow direction variable in source, by default "flwdir"
     basins_name : str, optional
         Name of flow direction variable in source, by default "basins"
     ftype : {'d8', 'ldd', 'nextxy'}, optional
         name of flow direction type, by default None; use input ftype.
     stream_kwargs : key-word arguments
         name of variable in ds and threshold value
+    buffer:
+        The buffer to apply.
+    logger:
+        The logger to use.
 
     Returns
     -------
     basin_geom : geopandas.geoDataFrame
         geometry the (sub)basin(s)
     outlet_geom : geopandas.geoDataFrame
         geometry the outlet point location
@@ -318,15 +333,16 @@
     ## BASINS
     if kind == "basin" or bounds is None:
         dvars = dvars + [basins_name]
         if basins_name not in ds:
             if gdf_bas is not None:
                 gdf_bas = None
                 logger.warning(
-                    "Basin geometries ignored as no corresponding basin map is provided."
+                    "Basin geometries ignored as no corresponding"
+                    + " basin map is provided."
                 )
             _check_size(ds, logger)
             logger.info(f'basin map "{basins_name}" missing, calculating on the fly.')
             flwdir = flwdir_from_da(ds[flwdir_name], ftype=ftype)
             ds[basins_name] = xr.Variable(ds.raster.dims, flwdir.basins())
         elif (
             ds[basins_name].raster.nodata != 0
@@ -336,15 +352,15 @@
         ds[basins_name].raster.set_nodata(0)
         # clip
         ds_clip = ds[dvars]
         if geom is not None:
             ds_clip = ds[dvars].raster.clip_geom(geom, buffer=buffer, mask=True)
         # get basin IDs
         if xy is not None:
-            logger.debug(f"Getting basin IDs at point locations.")
+            logger.debug("Getting basin IDs at point locations.")
             sel = {
                 ds.raster.x_dim: xr.IndexVariable("xy", np.atleast_1d(xy[0])),
                 ds.raster.y_dim: xr.IndexVariable("xy", np.atleast_1d(xy[1])),
             }
             basid = np.unique(ds_clip[basins_name].sel(**sel, method="nearest").values)
         elif basid is None:
             if stream_kwargs or outlets:
@@ -353,28 +369,29 @@
                 if outlets:
                     outmap = outlet_map(ds_clip[flwdir_name], ftype=ftype)
                     if stream_kwargs:
                         stream = stream.where(outmap, 0)
                     else:
                         stream = outmap
                 ds_clip[basins_name] = ds_clip[basins_name].where(stream, 0)
-            logger.debug(f"Getting IDs of intersecting basins.")
+            logger.debug("Getting IDs of intersecting basins.")
             basid = np.unique(ds_clip[basins_name].values)
         basid = np.atleast_1d(basid)
         basid = basid[basid > 0]
         if basid.size == 0:
-            raise ValueError(f"No basins found with given criteria.")
+            raise ValueError("No basins found with given criteria.")
         # clip ds to total basin
         if gdf_bas is not None:
             gdf_match = np.isin(gdf_bas["basid"], basid)
             gdf_bas = gdf_bas.loc[gdf_match]
             if gdf_bas.index.size > 0:
                 if geom is not None:
                     xminbas, yminbas, xmaxbas, ymaxbas = gdf_bas.total_bounds
-                    # Check that total_bounds is at least bigger than original geom bounds
+                    # Check that total_bounds is at least bigger
+                    # than original geom bounds
                     xmingeom, ymingeom, xmaxgeom, ymaxgeom = geom.total_bounds
                     total_bounds = [
                         min(xminbas, xmingeom),
                         min(yminbas, ymingeom),
                         max(xmaxbas, xmaxgeom),
                         max(ymaxbas, ymaxgeom),
                     ]
@@ -402,22 +419,25 @@
             mask = ds.raster.geometry_mask(geom)
         elif basins_name in ds:  # set flwdir mask based on basin map
             mask = ds[basins_name] > 0
         flwdir = flwdir_from_da(ds[flwdir_name], ftype=ftype, mask=mask)
         # get area of interest (aoi) mask
         if geom is not None:
             aoi = ds.raster.geometry_mask(geom)
-            # stream = stream.where(aoi, False)
         else:
             aoi = xr.DataArray(
                 coords=ds.raster.coords,
                 dims=ds.raster.dims,
                 data=np.full(ds.raster.shape, True, dtype=bool),
             )  # all True
-        # get stream mask (always over entire domain to include cells downstream of aoi!)
+        # Convert xy to tuple
+        if xy is not None:
+            xy = (np.atleast_1d(xy[0]), np.atleast_1d(xy[1]))
+        # get stream mask. Always over entire domain
+        # to include cells downstream of aoi!
         kwargs = dict()
         if stream_kwargs:
             stream = stream_map(ds, **stream_kwargs)
             if not np.any(stream):
                 raise ValueError(f"No streams found with: {stream_kwargs}.")
             if not outlets and xy is None:  # get aoi outflow cells if none provided
                 xy = flwdir.xy(flwdir.outflow_idxs(np.logical_and(stream, aoi).values))
@@ -425,15 +445,15 @@
                 kwargs.update(stream=stream.values)
         if outlets:
             outmap = aoi.where(outlet_map(ds[flwdir_name], ftype=flwdir.ftype), False)
             if stream_kwargs:
                 outmap = outmap.where(stream_kwargs, False)
             idxs_out = np.where(outmap.values.ravel())[0]
             if not np.any(outmap):
-                raise ValueError(f"No outlets found with with given criteria.")
+                raise ValueError("No outlets found with with given criteria.")
             xy = outmap.raster.idx_to_xy(idxs_out)
         # get subbasin map
         bas_mask, xy_out = basin_map(ds, flwdir, xy, **kwargs)
         # is subbasin with bounds check if all upstream cells are included
         if kind == "subbasin" and bounds is not None:
             geom = gpd.GeoDataFrame(geometry=[box(*bounds)], crs=ds.raster.crs)
             mask = ds.raster.geometry_mask(geom)
```

### Comparing `hydromt-0.7.1/hydromt/workflows/forcing.py` & `hydromt-0.8.0/hydromt/workflows/forcing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+"""Implementaion of forcing workflows."""
+import logging
+import re
+from typing import Union
+
+import numpy as np
 import pandas as pd
 import xarray as xr
 import xarray.core.resample
-import numpy as np
-import re
-import logging
-from typing import Union
 
 from .._compat import HAS_PYET
 
 if HAS_PYET:
     import pyet
 
 logger = logging.getLogger(__name__)
@@ -19,15 +21,17 @@
     da_like,
     clim=None,
     freq=None,
     reproj_method="nearest_index",
     resample_kwargs={},
     logger=logger,
 ):
-    """Lazy reprojection of precipitation to model grid and resampling of time dimension to frequency.
+    """Return the lazy reprojection of precipitation to model.
+
+      Applies the projection to the grid and resampling of time dimension to frequency.
 
     Parameters
     ----------
     precip: xarray.DataArray
         DataArray of precipitation forcing [mm]
     da_like: xarray.DataArray or Dataset
         DataArray of the target resolution and projection.
@@ -36,17 +40,21 @@
         to correct the precip downscaling.
     freq: str, Timedelta
         output frequency of time dimension
     reproj_method: str, optional
         Method for spatital reprojection of precip, by default 'nearest_index'
     resample_kwargs:
         Additional key-word arguments (e.g. label, closed) for time resampling method
+    kwargs:
+        Additional arguments to pass through to underlying methods.
+    logger:
+        The logger to use
 
     Returns
-    --------
+    -------
     p_out: xarray.DataArray (lazy)
         processed precipitation forcing
     """
     if precip.raster.dim0 != "time":
         raise ValueError(f'First precip dim should be "time", not {precip.raster.dim0}')
     # downscale precip (lazy); global min of zero
     p_out = np.fmax(precip.raster.reproject_like(da_like, method=reproj_method), 0)
@@ -84,16 +92,18 @@
     lapse_correction=True,
     freq=None,
     reproj_method="nearest_index",
     lapse_rate=-0.0065,
     resample_kwargs={},
     logger=logger,
 ):
-    """Lazy reprojection of temperature to model grid using lapse_rate for downscaling,
-    and resampling of time dimension to frequency.
+    """Return lazy reprojection of temperature to model grid.
+
+    Use lapse_rate for downscaling, and resampling of time
+    dimension to frequency.
 
     Parameters
     ----------
     temp: xarray.DataArray
         DataArray of temperature forcing [°C]
     dem_model: xarray.DataArray
         DataArray of the target resolution and projection, contains elevation
@@ -107,17 +117,19 @@
         output frequency of timedimension
     reproj_method: str, optional
         Method for spatital reprojection of precip, by default 'nearest_index'
     lapse_rate: float, optional
         lapse rate of temperature [C m-1] (default: -0.0065)
     resample_kwargs:
         Additional key-word arguments (e.g. label, closed) for time resampling method
+    logger:
+        The logger to use.
 
     Returns
-    --------
+    -------
     t_out: xarray.DataArray (lazy)
         processed temperature forcing
     """
     if temp.raster.dim0 != "time":
         raise ValueError(f'First temp dim should be "time", not {temp.raster.dim0}')
     # apply lapse rate
     if lapse_correction:
@@ -159,15 +171,17 @@
     lapse_correction=True,
     freq=None,
     reproj_method="nearest_index",
     lapse_rate=-0.0065,
     resample_kwargs={},
     logger=logger,
 ):
-    """Lazy reprojection of pressure to model grid and resampling of time dimension to frequency.
+    """Return lazy reprojection of pressure to model grid.
+
+    Resample time dimension to frequency.
 
     Parameters
     ----------
     press: xarray.DataArray
         DataArray of pressure forcing [hPa]
     dem_model: xarray.DataArray
         DataArray of the target resolution and projection, contains elevation
@@ -178,17 +192,19 @@
         output frequency of timedimension
     reproj_method: str, optional
         Method for spatital reprojection of precip, by default 'nearest_index'
     lapse_rate: float, optional
         lapse rate of temperature [C m-1] (default: -0.0065)
     resample_kwargs:
         Additional key-word arguments (e.g. label, closed) for time resampling method
+    logger:
+        The logger to use.
 
     Returns
-    --------
+    -------
     press_out: xarray.DataArray (lazy)
         processed pressure forcing
     """
     if press.raster.dim0 != "time":
         raise ValueError(f'First press dim should be "time", not {press.raster.dim0}')
     # downscale pressure (lazy)
     press_out = press.raster.reproject_like(dem_model, method=reproj_method)
@@ -216,41 +232,45 @@
     altitude: float = 10,
     altitude_correction: bool = False,
     freq: pd.Timedelta = None,
     reproj_method: str = "nearest_index",
     resample_kwargs: dict = {},
     logger=logger,
 ):
-    """Lazy reprojection of wind speed to model grid and resampling of time dimension to frequency.
+    """Return lazy reprojection of wind speed to model grid.
 
-    Either provide wind speed directly or both wind_u and wind_v components.
+    Resample time dimension to frequency. Either provides wind speed directly
+    or both wind_u and wind_v components.
 
     Parameters
     ----------
     wind: xarray.DataArray
         DataArray of wind speed forcing [m s-1]
     wind_u: xarray.DataArray
         DataArray of U component of wind speed forcing [m s-1]
     wind_v: xarray.DataArray
         DataArray of V component of wind speed forcing [m s-1]
     da_model: xarray.DataArray
         DataArray of the target resolution and projection
     altitude: float, optional
         ALtitude of wind speed data. By default 10m.
     altitude_correction: str, optional
-       If True wind speed is re-calculated to wind speed at 2 meters using original `altitude`.
+       If True wind speed is re-calculated to wind speed at 2 meters using
+       original `altitude`.
     freq: str, Timedelta
         output frequency of timedimension
     reproj_method: str, optional
         Method for spatital reprojection of precip, by default 'nearest_index'
     resample_kwargs:
         Additional key-word arguments (e.g. label, closed) for time resampling method
+    logger:
+        The logger to use.
 
     Returns
-    --------
+    -------
     wind_out: xarray.DataArray (lazy)
         processed wind forcing
     """
     if wind_u is not None and wind_v is not None:
         wind = np.sqrt(np.power(wind_u, 2) + np.power(wind_v, 2))
     elif wind is None:
         raise ValueError("Either wind or wind_u and wind_v varibales must be supplied.")
@@ -277,57 +297,66 @@
     temp: xarray.DataArray,
     dem_model: xarray.DataArray,
     method: str = "debruin",
     press_correction: bool = False,
     wind_correction: bool = True,
     wind_altitude: float = 10,
     reproj_method: str = "nearest_index",
-    # lapse_rate: float=-0.0065,
     freq: str = None,
     resample_kwargs: dict = {},
     logger=logger,
 ) -> xarray.DataArray:
-    """Determines reference evapotranspiration (lazy reprojection on model grid and resampling of time dimension to frequency).
+    """Determine reference evapotranspiration.
+
+    (lazy reprojection on model grid and resampling of time dimension to frequency).
 
     Parameters
     ----------
     ds : xarray.Dataset
-        Dataset with climate variables: pressure [hPa], global radiation [W m-2], TOA incident solar radiation [W m-2], wind [m s-1]
+        Dataset with climate variables: pressure [hPa], global radiation [W m-2],
+        TOA incident solar radiation [W m-2], wind [m s-1]
 
         * Required variables: {"temp", "press" or "press_msl", "kin"}
         * additional variables for debruin: {"kout"}
-        * additional variables for penman-monteith_rh_simple: {"temp_min", "temp_max", "wind" or "wind_u"+"wind_v", "rh"}
-        * additional variables for penman-monteith_tdew: {"temp_min", "temp_max", "wind" or "wind_u"+"wind_v", "temp_dew"}
+        * additional variables for penman-monteith_rh_simple:
+            {"temp_min", "temp_max", "wind" or "wind_u"+"wind_v", "rh"}
+        * additional variables for penman-monteith_tdew:
+            {"temp_min", "temp_max", "wind" or "wind_u"+"wind_v", "temp_dew"}
     temp : xarray.DataArray
         DataArray with temperature on model grid resolution [°C]
     dem_model : xarray.DataArray
         DataArray of the target resolution and projection, contains elevation
         data
     method : {'debruin', 'makkink', "penman-monteith_rh_simple", "penman-monteith_tdew"}
         Potential evapotranspiration method.
         if penman-monteith is used, requires the installation of the pyet package.
+    reproj_method: str, optional
+        Method for spatital reprojection of precip, by default 'nearest_index'
     press_correction : bool, default False
         If True pressure is corrected, based on elevation data of `dem_model`
     wind_altitude: float, optional
         ALtitude of wind speed data. By default 10m.
     wind_correction: str, optional
-       If True wind speed is re-calculated to wind speed at 2 meters using original `wind_altitude`.
-    freq : str, Timedelta, default None
+        If True wind speed is re-calculated to wind speed at 2 meters using
+        original `wind_altitude`.
+    freq: str, Timedelta, default None
         output frequency of timedimension
     resample_kwargs:
         Additional key-word arguments (e.g. label, closed) for time resampling method
+    logger:
+        The logger to use.
 
     Returns
-    --------
+    -------
     pet_out : xarray.DataArray (lazy)
         reference evapotranspiration
     """
     # # resample in time
     if temp.raster.dim0 != "time" or ds.raster.dim0 != "time":
-        raise ValueError(f'First dimension of input variables should be "time"')
+        raise ValueError('First dimension of input variables should be "time"')
     # make sure temp and ds align both temporally and spatially
     if not np.all(temp["time"].values == ds["time"].values):
         raise ValueError("All input variables have same time index.")
     if not temp.raster.identical_grid(dem_model):
         raise ValueError("Temp variable should be on model grid.")
 
     # resample input to model grid
@@ -348,15 +377,16 @@
         elif HAS_PYET:
             # calculate pressure from elevation [kPa]
             ds["press"] = pyet.calc_press(dem_model)
             # convert to hPa to be consistent with press function calculation:
             ds["press"] = ds["press"] * 10
         else:
             raise ModuleNotFoundError(
-                "If 'press' is supplied and 'press_correction' is not used, the pyet package must be installed."
+                "If 'press' is supplied and 'press_correction' is not used,"
+                + " the pyet package must be installed."
             )
 
     timestep = to_timedelta(ds).total_seconds()
     if method == "debruin":
         pet_out = pet_debruin(
             temp,
             ds["press"],
@@ -437,16 +467,16 @@
     dem_model : xarray.DataArray
         DataArray with high res lat/lon axis and elevation data
     g : float, default 9.80665
         gravitational constant [m s-2]
     R_air : float, default 8.3144621
         specific gas constant for dry air [J mol-1 K-1]
     Mo : float, default 0.0289644
-        molecular weight of gas [g / mol]
-    LapseRate : float, deafult -0.0065
+        molecular weight of gas [kg / mol]
+    lapse_rate : float, deafult -0.0065
         lapse rate of temperature [C m-1]
 
     Returns
     -------
     press_fact : xarray.DataArray
         pressure correction factor
     """
@@ -467,34 +497,33 @@
         lapse rate of temperature [°C m-1]
 
     Returns
     -------
     temp_add : xarray.DataArray
         temperature addition
     """
-
     temp_add = (dem * lapse_rate).fillna(0)
 
     return temp_add
 
 
 def pet_debruin(
     temp, press, k_in, k_ext, timestep=86400, cp=1005.0, beta=20.0, Cs=110.0
 ):
-    """Determines De Bruin (2016) reference evapotranspiration.
+    """Determine De Bruin (2016) reference evapotranspiration.
 
     Parameters
     ----------
     temp : xarray.DataArray
         DataArray with temperature [°C]
     press : xarray.DataArray
         pressure at surface [hPa]
     k_in : xarray.DataArray
         global (=short wave incoming) radiation [W m-2]
-    k_ext : xarray.DataArray}
+    k_ext : xarray.DataArray
         TOA incident solar radiation [W m-2]
     timestep : int, default 86400
         seconds per timestep
     cp : float, default 1005.0
         standard cp [J kg-1 K-1]
     beta : float, default 20.0
         correction constant [W m-2]
@@ -502,20 +531,21 @@
         emperical constant [W m-2]
 
     Returns
     -------
     pet : xarray.DataArray
         reference evapotranspiration
     """
-    # saturation and actual vapour pressure at given temperature [Pa]
+    # saturation and actual vapour pressure at given temperature [hPa °C-1]
     esat = 6.112 * np.exp((17.67 * temp) / (temp + 243.5))
-    # slope of vapour pressure curve
+    # slope of vapour pressure curve [hPa °C-1]
     slope = esat * (17.269 / (temp + 243.5)) * (1.0 - (temp / (temp + 243.5)))
     # compute latent heat of vapourization [J kg-1]
     lam = (2.502 * 10**6) - (2250.0 * temp)
+    # psychometric constant [hPa °C-1]
     gamma = (cp * press) / (0.622 * lam)
     # compute ref. evaporation (with global radiation, therefore calling it potential)
     # in J m-2 over whole period
     ep_joule = (
         (slope / (slope + gamma))
         * (((1.0 - 0.23) * k_in) - (Cs * (k_in / (k_ext + 0.00001))))
     ) + beta
@@ -538,24 +568,25 @@
         DataArray with global radiation [W m-2]
     timestep : int, default 86400
         seconds per timestep
     cp : float, default 1005.0
         standard cp [J kg-1 K-1]
 
     Returns
-    --------
+    -------
     pet : xarray.DataArray (lazy)
         reference evapotranspiration
     """
-    # saturation and actual vapour pressure at given temperature [Pa]
+    # saturation and actual vapour pressure at given temperature [hPa °C-1]
     esat = 6.112 * np.exp((17.67 * temp) / (temp + 243.5))
-    # slope of vapour pressure curve
+    # slope of vapour pressure curve [hPa °C-1]
     slope = esat * (17.269 / (temp + 243.5)) * (1.0 - (temp / (temp + 243.5)))
     # compute latent heat of vapourization [J kg-1]
     lam = (2.502 * 10**6) - (2250.0 * temp)
+    # psychometric constant [hPa °C-1]
     gamma = (cp * press) / (0.622 * lam)
 
     ep_joule = 0.65 * slope / (slope + gamma) * k_in
     pet = ((ep_joule / lam) * timestep).astype(np.float32)
     pet = xr.where(pet > 0.0, pet, 0.0)
     return pet
 
@@ -567,21 +598,21 @@
     press: xarray.DataArray,
     kin: xarray.DataArray,
     wind: xarray.DataArray,
     temp_dew: xarray.DataArray,
     dem: xarray.DataArray,
     var: str = "temp_dew",
 ) -> xarray.DataArray:
-    """
-    Estimate daily reference evapotranspiration (ETo) from a hypothetical
-    short grass reference surface using the FAO-56 Penman-Monteith equation.
-
-    Actual vapor pressure is derived either from relative humidity or dewpoint temperature (depending on var_for_avp_name).
+    """Estimate daily reference evapotranspiration (ETo).
 
-    Based on equation 6 in Allen et al (1998) and using the functions provided by the pyet package ()
+    Based on a hypothetical short grass reference surface using the
+    FAO-56 Penman-Monteith equation. Actual vapor pressure is derived either
+    from relative humidity or dewpoint temperature (depending on var_for_avp_name).
+    Based on equation 6 in Allen et al (1998) and using the functions provided
+    by the pyet package ()
 
     Parameters
     ----------
     temp : xarray.DataArray
         DataArray with daily temperature [°C]
     temp_max : xarray.DataArray
         DataArray with maximum daily temperature [°C]
@@ -590,19 +621,21 @@
     press : xarray.DataArray
         DataArray with pressure [hPa]
     kin : xarray.DataArray
         DataArray with global radiation [W m-2]
     wind : xarray.DataArray
         DataArray with wind speed at 2m above the surface [m s-1]
     temp_dew : xarray.DataArray
-        DataArray with either temp_dew (dewpoint temperature at 2m above surface [°C]) or rh (relative humidity [%]) to estimate actual vapor pressure
+        DataArray with either temp_dew (dewpoint temperature at 2m above surface [°C])
+        or rh (relative humidity [%]) to estimate actual vapor pressure
     dem : xarray.DataArray
         DataArray with elevation at model resolution [m]
     var : str, optional
-        String with variable name used to estimate actual vapor pressure (chose from ["temp_dew", "rh"])
+        String with variable name used to estimate actual vapor pressure
+        (chose from ["temp_dew", "rh"])
 
     Returns
     -------
     xarray.DataArray
         DataArray with the estimated daily reference evapotranspiration pet [mm d-1]
 
     Raises
@@ -666,14 +699,15 @@
     closed="right",
     upsampling="bfill",
     downsampling="mean",
     conserve_mass=True,
     logger=logger,
 ):
     """Resample data to destination frequency.
+
     Skip if input data already at output frequency.
 
     Parameters
     ----------
     da: xarray.DataArray
         Input data
     freq: str, pd.timedelta
@@ -683,17 +717,19 @@
     closed: {'left', 'right'}, optional
         Side of each interval to treat as closed. By default 'right'.
     upsampling, downsampling: str, optional
         Resampling method if output frequency is higher, lower (resp.) compared
         to input frequency.
     conserve_mass: bool, optional
         If True multiply output with relative change in frequency to conserve mass
+    logger:
+        The logger to use.
 
     Returns
-    --------
+    -------
     pet : xarray.DataArray
         Resampled data.
     """
     da_out = da
     dfreq = delta_freq(da, freq)
     if not np.isclose(dfreq, 1.0):
         resample = upsampling if dfreq < 1 else downsampling
@@ -708,34 +744,38 @@
         if conserve_mass:
             da_out = da_out * min(dfreq, 1)
 
     return da_out
 
 
 def delta_freq(da_or_freq, da_or_freq1):
-    """Returns the relative difference between the dataset mean timestep and destination freq
+    """Return relative difference between dataset mean timestep and destination freq.
+
     <1 : upsampling
     1 : same
-    >1 : downsampling
+    >1 : downsampling.
     """
     return to_timedelta(da_or_freq1) / to_timedelta(da_or_freq)
 
 
 def to_timedelta(da_or_freq):
+    """Convert time dimention or frequency to timedelta."""
     if isinstance(da_or_freq, (xr.DataArray, xr.Dataset)):
         freq = da_to_timedelta(da_or_freq)
     else:
         freq = freq_to_timedelta(da_or_freq)
     return freq
 
 
 def da_to_timedelta(da):
+    """Convert time dimenstion in dataset to timedelta."""
     return pd.to_timedelta(np.diff(da.time).mean())
 
 
 def freq_to_timedelta(freq):
+    """Convert frequency to timedelta."""
     # Add '1' to freq that doesn't have any digit
     if isinstance(freq, str) and not bool(re.search(r"\d", freq)):
         freq = "1{}".format(freq)
 
     # Convert str to datetime.timedelta
     return pd.to_timedelta(freq)
```

### Comparing `hydromt-0.7.1/hydromt/workflows/rivers.py` & `hydromt-0.8.0/hydromt/workflows/rivers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,32 @@
+"""Implementations for river workflows."""
+import logging
+from typing import Union
+
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import xarray as xr
-from scipy import ndimage
-from typing import Union
-import logging
 from pyflwdir import Flwdir, FlwdirRaster
+from scipy import ndimage
 
 from ..gis_utils import spread2d
 
 logger = logging.Logger(__name__)
 
 __all__ = ["river_width", "river_depth"]
 
 
 def river_width(
     gdf_stream: gpd.GeoDataFrame,
     da_rivmask: xr.DataArray,
     nmin=5,
 ) -> np.ndarray:
-    """Return segment average river width based on a river mask raster.
+    """Return average river width along a segment based on a river mask raster.
+
     For each segment in gdf_stream the associated area is calculated from stream mask
     and divided by the segment length to obtain the average width.
 
     Parameters
     ----------
     gdf_stream : gpd.GeoDataFrame
         River segments
@@ -81,46 +84,55 @@
     Parameters
     ----------
     data : xr.Dataset, pd.DataFrame, gpd.GeoDataFrame
         Dataset/DataFrame containing required variables
     method : {'powlaw', 'manning', 'gvf'}
         Method to estimate the river depth:
 
-        * powlaw [1]_ [2]_: power-law hc*Qbf**hp, requires bankfull discharge (Qbf) variable in `data`.
-          Optionally, `hc` (default = 0.27) and `hp` (default = 0.30) set through `kwargs`.
-        * manning [3]_: river depth for kinematic conditions, requires bankfull discharge,
-          river width, river slope in `data`; the river manning roughness either in data
-          or as constant and optionally `min_rivslp` (default = 1e-5) set through `kwargs`.
+        * powlaw [1]_ [2]_: power-law hc*Qbf**hp, requires bankfull discharge (Qbf).
+          Optionally, `hc` (default = 0.27) and `hp` (default = 0.30) set in `kwargs`.
+        * manning [3]_: river depth for kinematic conditions,
+          requires bankfull discharge, river width, river slope in `data`;
+          the river manning roughness either in data or as constant and
+          optionally `min_rivslp` (default = 1e-5) set in `kwargs`.
         * gvf [4]_: gradually varying flow, requires bankfull discharge,
-          river width, river surface elevation in `data`; the river manning roughness either in data
-          or as constant and optionally `min_rivslp` (default = 1e-5) set through `kwargs`.
+          river width, river surface elevation in `data`;
+          the river manning roughness either in data
+          or as constant and optionally `min_rivslp` (default = 1e-5) set in `kwargs`.
     flwdir : Flwdir, FlwdirRaster, optional
         Flow directions, required if method is not powlaw
     min_rivdph : float, optional
         Minimum river depth [m], by default 1.0
     manning : float, optional
         Constant manning roughness [s/m^{1/3}] used if `rivman_name` not in data,
         by default 0.03
-    qbankfull_name, rivwth_name, rivzs_name, rivdst_name, rivslp_name, rivman_name: str, optional
+    qbankfull_name, rivwth_name, rivzs_name, rivdst_name, rivslp_name, rivman_name:
         Name for variables in data: bankfull discharge [m3/s], river width [m],
         bankfull water surface elevation profile [m+REF], distance to river outlet [m],
         river slope [m/m] and river manning roughness [s/m^{1/3}]
+    kwargs:
+        additional arguments to be passed down
 
     Returns
     -------
     rivdph: xr.DataArray, np.ndarray
-        River depth [m]. A DataArray is returned if the input data is a Dataset, otherwise
-        a array with the shape of one input data variable is returned.
+        River depth [m]. A DataArray is returned if the input data is a Dataset,
+        otherwise a array with the shape of one input data variable is returned.
 
     References
     ----------
-    .. [1] Leopold & Maddock (1953). The hydraulic geometry of stream channels and some physiographic implications (No. 252; Professional Paper). U.S. Government Printing Office. https://doi.org/10.3133/pp252
-    .. [2] Andreadis et al. (2013). A simple global river bankfull width and depth database. Water Resources Research, 49(10), 7164–7168. https://doi.org/10.1002/wrcr.20440
-    .. [3] Sampson et al. (2015). A high-resolution global flood hazard model. Water Resources Research, 51(9), 7358–7381. https://doi.org/10.1002/2015WR016954
-    .. [4] Neal et al. (2021). Estimating river channel bathymetry in large scale flood inundation models. Water Resources Research, 57(5). https://doi.org/10.1029/2020wr028301
+    .. [1] Leopold & Maddock (1953). The hydraulic geometry of stream channels and some
+            physiographic implications (No. 252; Professional Paper).
+            U.S. Government Printing Office. https://doi.org/10.3133/pp252
+    .. [2] Andreadis et al. (2013). A simple global river bankfull width and depth
+            database. Water Resources Research, 49(10), 7164-7168. https://doi.org/10.1002/wrcr.20440
+    .. [3] Sampson et al. (2015). A high-resolution global flood hazard model.
+            Water Resources Research, 51(9), 7358-7381. https://doi.org/10.1002/2015WR016954
+    .. [4] Neal et al. (2021). Estimating river channel bathymetry in large scale
+            flood inundation models. Water Resources Research, 57(5). https://doi.org/10.1029/2020wr028301
 
     See Also
     --------
     pyflwdir.FlwdirRaster.river_depth
     """
     methods = ["powlaw", "manning", "gvf"]
     if method == "powlaw":
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hydromt-0.7.1/joss_paper/citation.bib` & `hydromt-0.8.0/joss_paper/citation.bib`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-@article{Eilander2023, 
-    doi = {10.21105/joss.04897}, 
-    url = {https://doi.org/10.21105/joss.04897}, 
-    year = {2023}, 
-    publisher = {The Open Journal}, 
-    volume = {8}, 
-    number = {83}, 
-    pages = {4897}, 
-    author = {Dirk Eilander and Hélène Boisgontier and Laurène J. E. Bouaziz and Joost Buitink and Anaïs Couasnon and Brendan Dalmijn and Mark Hegnauer and Tjalling de Jong and Sibren Loos and Indra Marth and Willem van Verseveld}, 
-    title = {HydroMT: Automated and reproducible model building and analysis}, 
-    journal = {Journal of Open Source Software} 
-}
+@article{Eilander2023,
+    doi = {10.21105/joss.04897},
+    url = {https://doi.org/10.21105/joss.04897},
+    year = {2023},
+    publisher = {The Open Journal},
+    volume = {8},
+    number = {83},
+    pages = {4897},
+    author = {Dirk Eilander and Hélène Boisgontier and Laurène J. E. Bouaziz and Joost Buitink and Anaïs Couasnon and Brendan Dalmijn and Mark Hegnauer and Tjalling de Jong and Sibren Loos and Indra Marth and Willem van Verseveld},
+    title = {HydroMT: Automated and reproducible model building and analysis},
+    journal = {Journal of Open Source Software}
+}
```

### Comparing `hydromt-0.7.1/joss_paper/paper.bib` & `hydromt-0.8.0/joss_paper/paper.bib`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -404,8 +404,8 @@
   month        = nov,
   year         = 2022,
   note         = {If you use this software, please cite it as below.},
   publisher    = {Zenodo},
   version      = {v1.5.2},
   doi          = {10.5281/zenodo.7344967},
   url          = {https://doi.org/10.5281/zenodo.7344967}
-}
+}
```

### Comparing `hydromt-0.7.1/joss_paper/paper.md` & `hydromt-0.8.0/joss_paper/paper.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   - Python
   - reproducible model building
   - model analysis
   - hydrology
   - hydrodynamics
   - gis
 authors:
-  - name: Dirk Eilander^[Corresponding author] 
+  - name: Dirk Eilander^[Corresponding author]
     orcid: 0000-0002-0951-8418
     affiliation: "1, 2" # (Multiple affiliations must be quoted)
   - name: Hélène Boisgontier
     affiliation: 1
   - name: Laurène J. E. Bouaziz
     affiliation: 1
     orcid: 0000-0003-0597-8051
@@ -49,42 +49,42 @@
 
 Many impact assessment studies rely on hydrological and hydrodynamic (hydro) models. These models typically require a large set of parameters derived from different datasets and hence manual setup can be time consuming and hard to reproduce. HydroMT (Hydro Model Tools) is an open-source Python package that aims to make the process of building model instances and analyzing model results automated and reproducible. The package provides a common interface to data and model instances, workflows to transform data into models based on (hydrological) GIS and statistical methods, and various methods to analyze model results. The user can describe a full model instance including its forcing in a single configuration file based on a sequence of workflows, making the process reproducible, fast, and modular. The package has been designed with an iterative, data-centered modeling process in mind. First-order model schematizations can be built for any location in the world by leveraging open global datasets. These can later be improved by updating the input datasets with detailed local datasets. This iterative process enables the user to quickly get an initial result to then make informed decisions about the most relevant improvements and/or required data collection and to kick-start discussions with stakeholders. Furthermore, model parameter maps or forcing data can easily be modified for sensitivity analysis or calibration to support these robust modeling practices. HydroMT is successfully being used for several model software through a plugin infrastructure that allow for model specific functionality, such as readers and writers of model data formats, and can easily be extended to new model software. Currently supported model software include the distributed rainfall-runoff model Wflow, the hydrodynamic flood model SFINCS, the water quality models D-Water Quality and D-Emissions and the flood impact model Delft-FIAT.
 
 # Statement of need
 
 Hydrological and hydrodynamic (hydro) models are crucial to understand water systems and perform impact assessment studies [e.g., @Undrr2022]. These models require different accurate input data. For instance, hydrodynamic models typically require bathymetric and/or topographic data, surface roughness data and boundary forcing data (e.g., water level time series). However, sufficiently accurate datasets are often not readily available and need to be converted into model-specific, sometimes idiosyncratic, file formats. For instance, many Digital Elevation Models (DEMs) require ample preprocessing as these typically represent the elevation of the top of buildings, trees or water surface, while in the model the terrain and riverbed elevation are required [@Hawker2022; @Neal2021]. Therefore, hydro models require various steps to process raw input data to model data which, if done manually, makes the process time consuming and hard to reproduce. Furthermore, it makes it hard to improve model instances based on new or updated (large) datasets, such as (global) DEMs and land use maps, potentially slowing down the uptake of such datasets for geoscientific modeling. Hence, there is a clear need for automated setup of model instances for increased transparency and reproducibility in hydro modeling [@White2020; @Hall2022].
 
-Several open-source packages have been proposed to facilitate automated and reproducible model building. For the Soil and Water Assessment Tool (SWAT) model [@Arnold2012], the SWAT+AW package provides scripted automated workflows (AW) that are compatible with the SWAT GUI to improve reproducibility [@Chawanda2020]. For groundwater modeling the FloPy [@Bakker2016] and iMOD-Python [@Van_Engelen2022] packages provide scripting interfaces to automatically setup instances of the groundwater model MODFLOW [@Harbaugh2005]. Similarly, LFPtools [@Sosa2020] provides scripts to setup instances of the hydrodynamic model LISFLOOD-FP [@Bates2010]. While these packages can provide automated and reproducible modeling, their functionally is model software specific and often requires scripting skills to be used. 
+Several open-source packages have been proposed to facilitate automated and reproducible model building. For the Soil and Water Assessment Tool (SWAT) model [@Arnold2012], the SWAT+AW package provides scripted automated workflows (AW) that are compatible with the SWAT GUI to improve reproducibility [@Chawanda2020]. For groundwater modeling the FloPy [@Bakker2016] and iMOD-Python [@Van_Engelen2022] packages provide scripting interfaces to automatically setup instances of the groundwater model MODFLOW [@Harbaugh2005]. Similarly, LFPtools [@Sosa2020] provides scripts to setup instances of the hydrodynamic model LISFLOOD-FP [@Bates2010]. While these packages can provide automated and reproducible modeling, their functionally is model software specific and often requires scripting skills to be used.
 
-HydroMT (Hydro Model Tools) is an open-source Python package that aims to make the process of building a model instance and analyzing model results automated and reproducible for any hydro software. As such it contributes towards the FAIR principles of research software (FAIR4RS) which aim to increase the transparency, reproducibility, and reusability of research [@Chue_Hong2021]. Compared to other packages for automated model building, it is data- and model-agnostic meaning that data sources can easily be interchanged without additional coding and the generic model interface can be used for different model software. This makes it possible to reuse workflows to prepare input for different model software that require the same parameter (e.g., Manning roughness derived from landuse maps) or workflows used for postprocessing of results (e.g., calculating model skill statistics), thereby providing an environment for controlled model experiments. Furthermore, it provides a high-level command line interface making it accessible to modelers without Python scripting experience. 
+HydroMT (Hydro Model Tools) is an open-source Python package that aims to make the process of building a model instance and analyzing model results automated and reproducible for any hydro software. As such it contributes towards the FAIR principles of research software (FAIR4RS) which aim to increase the transparency, reproducibility, and reusability of research [@Chue_Hong2021]. Compared to other packages for automated model building, it is data- and model-agnostic meaning that data sources can easily be interchanged without additional coding and the generic model interface can be used for different model software. This makes it possible to reuse workflows to prepare input for different model software that require the same parameter (e.g., Manning roughness derived from landuse maps) or workflows used for postprocessing of results (e.g., calculating model skill statistics), thereby providing an environment for controlled model experiments. Furthermore, it provides a high-level command line interface making it accessible to modelers without Python scripting experience.
+
+Several recent applications have already used HydroMT. It has been used to build instances of the hydrological Wflow model [@Van_Verseveld2022; @Imhoff2020] for climate change impact studies [@Sperna_Weiland2021]; for a large sample assessment of spatial scales in hydrological modeling [@Aerts2021]; to estimate water balance components based on global data in a data-scarce area [@Rusli2021]; and to build instances of the hydrodynamic SFINCS model [@Leijnse2021] to simulate compound flood hazard from (global) datasets in any coastal delta globally [@Eilander2022-nhess]. While the package is sufficiently general to support model software outside the domain of hydro models, the focus of many workflows is on typical hydrological data and parameters and hence hydro models benefit most from the tool.
 
-Several recent applications have already used HydroMT. It has been used to build instances of the hydrological Wflow model [@Van_Verseveld2022; @Imhoff2020] for climate change impact studies [@Sperna_Weiland2021]; for a large sample assessment of spatial scales in hydrological modeling [@Aerts2021]; to estimate water balance components based on global data in a data-scarce area [@Rusli2021]; and to build instances of the hydrodynamic SFINCS model [@Leijnse2021] to simulate compound flood hazard from (global) datasets in any coastal delta globally [@Eilander2022-nhess]. While the package is sufficiently general to support model software outside the domain of hydro models, the focus of many workflows is on typical hydrological data and parameters and hence hydro models benefit most from the tool. 
- 
 # Functionality
 
 The functionality of HydroMT can be broken down into three components, which are around input data, model instances, and methods and workflows. Users can interact with HydroMT through a high-level command line interface (CLI) to build model instances from scratch, update existing model instances or analyze model results (in progress). Furthermore, a Python interface is available that exposes all functionality for experienced users. A schematic overview of the package is provided in \autoref{fig:schematic} and each HydroMT component is discussed below.
 
-- **Input Data.** HydroMT is data-agnostic through the Data Adapter, which reads a wide range of data formats and unifies the input data (e.g., on-the-fly renaming and unit conversion). Datasets are listed and passed to HydroMT in a user defined data catalog yaml file. HydroMT also provides several predefined data catalogs with mostly global datasets that can be used as is, although not all datasets in these catalogs are openly accessible. Currently, four different types of input data are supported and represented by a specific Python data object: gridded datasets such as DEMs or gridded spatially distributed rainfall datasets (represented by RasterDataset objects, a raster-specific type of Xarray Datasets); tables that can be used to, for example, convert land classes to roughness values (represented by Pandas DataFrame objects); vector datasets such as administrative units or river centerlines (represented by Geopandas GeoDataFrame objects); and time series with associated geolocations such as observations of discharge (represented by GeoDataset objects, a geo-specific type of Xarray Datasets). 
-- **Models.** HydroMT defines any model instance through the model-agnostic Model API based on several components: maps, geometries, forcings, results, states, and the model simulation configuration. For different types of general model classes (i.e., gridded, lumped, mesh and network models) additional model components have been defined. Each component is represented with a specific Python data object to provide a common interface to different model software. Model instances can be built from scratch, and existing instances can be updated based on a pipeline of methods defined in a model configuration ini file. While HydroMT provides several general model classes that can readily be used, it can also be tailored to specific model software through a plugin infrastructure. These plugins have the same interface, but with model-specific file readers, writers and workflows. 
+- **Input Data.** HydroMT is data-agnostic through the Data Adapter, which reads a wide range of data formats and unifies the input data (e.g., on-the-fly renaming and unit conversion). Datasets are listed and passed to HydroMT in a user defined data catalog yaml file. HydroMT also provides several predefined data catalogs with mostly global datasets that can be used as is, although not all datasets in these catalogs are openly accessible. Currently, four different types of input data are supported and represented by a specific Python data object: gridded datasets such as DEMs or gridded spatially distributed rainfall datasets (represented by RasterDataset objects, a raster-specific type of Xarray Datasets); tables that can be used to, for example, convert land classes to roughness values (represented by Pandas DataFrame objects); vector datasets such as administrative units or river centerlines (represented by Geopandas GeoDataFrame objects); and time series with associated geolocations such as observations of discharge (represented by GeoDataset objects, a geo-specific type of Xarray Datasets).
+- **Models.** HydroMT defines any model instance through the model-agnostic Model API based on several components: maps, geometries, forcings, results, states, and the model simulation configuration. For different types of general model classes (i.e., gridded, lumped, mesh and network models) additional model components have been defined. Each component is represented with a specific Python data object to provide a common interface to different model software. Model instances can be built from scratch, and existing instances can be updated based on a pipeline of methods defined in a model configuration ini file. While HydroMT provides several general model classes that can readily be used, it can also be tailored to specific model software through a plugin infrastructure. These plugins have the same interface, but with model-specific file readers, writers and workflows.
 -	**Methods and workflows.** Most of the heavy work in HydroMT is done by methods and workflows, indicated by the gear wheels in \autoref{fig:schematic}. Methods provide the low-level functionality such as GIS rasterization, reprojection, or zonal statistics. Workflows combine several methods to transform data to a model layer or postprocess model results. Examples of workflows include the delineation of hydrological basins (watersheds), conversion of landuse-landcover data to model parameter maps, and calculation of model skill statistics. Workflows are implemented for the data types mentioned above to allow reusing common workflows between HydroMT plugins for different model software.
 
 ![Schematic overview of HydroMT design.\label{fig:schematic}](docs/_static/Architecture_model_data_input.png)
 
 # Example usage
 
 Here, a high-level example of how to build a model instance using HydroMT is provided. Building a model instance from scratch with HydroMT involves the following four generic steps, see \autoref{fig:hydromt_build}. First, the user defines the input data in a *yaml* data catalog file or selects available datasets from a pre-defined data catalog. Second, the user defines the region that describes the area of interest. The region can be based on a simple bounding box or geometry, but also a (sub)(inter)basin that is delineated on-the-fly based on available hydrography data. Third, the user configures the model instance in an *ini* configuration file. This file represents a model software specific recipe to build a model instance and this is where the modeler can make choices how to best setup the model instance. It lists the workflows and their arguments in order of execution and in combination with the data catalog file provides a reproducible recipe to build a model instance. Available workflows (i.e., model setup methods) and their arguments are described in the documentation. Finally, the user runs the HydroMT build method from either command line or Python.
 
 ![Workflow of building a model from scratch with HydroMT.\label{fig:hydromt_build}](docs/_static/getting_started.png)
 
-# Audience 
+# Audience
 
 HydroMT is intended for students, researchers and modelers who would like to automatically build reproducible hydro models, anywhere in the world and based on the input data of their choice. For users, no Python knowledge beyond installing the package is required as HydroMT provides a CLI for common high-level functionalities. However, with Python knowledge, experienced users can directly use methods and workflows of HydroMT and interact their with model instances.
 
 # Dependencies
 
 HydroMT builds on many open source (Python) packages including Xarray [@Hoyer2017], dask [@Dask_Development_Team2016], rasterio [@Gillies2013], rioxarray [@Snow2022], pandas [@pandas2022], geopandas [@Jordahl2021], pyflwdir [@Eilander2022], and GDAL [@GDALOGR_contributors2022].
 
 # Acknowledgements
 
 The developments have been sponsored by Deltares Strategic Research funding, the Deltares Hydrology Product Line, and the Netherlands Organization for Scientific Research (NWO) in the form of a VIDI grant (Grant No. 016.161.324).
 
-# References
+# References
```

### Comparing `hydromt-0.7.1/PKG-INFO` & `hydromt-0.8.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,109 +1,130 @@
 Metadata-Version: 2.1
 Name: hydromt
-Version: 0.7.1
-Summary: HydroMT: Automated and reproducible model building and analysis
-Author-email: Dirk Eilander <dirk.eilander@deltares.nl>, Hélène Boisgontier <helene.boisgontier@deltares.nl>
-Requires-Python: >=3.8
+Version: 0.8.0
+Summary: HydroMT: Automated and reproducible model building and analysis.
+Author-email: Dirk Eilander <dirk.eilander@deltares.nl>, Hélène Boisgontier <helene.boisgontier@deltares.nl>, Sam Vente <sam.vente@deltares.nl>
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: affine
 Requires-Dist: bottleneck
 Requires-Dist: click
 Requires-Dist: dask
 Requires-Dist: entrypoints
-Requires-Dist: fsspec
 Requires-Dist: geopandas>=0.10
 Requires-Dist: gdal>=3.1
-Requires-Dist: numpy
+Requires-Dist: fiona==1.8.22
+Requires-Dist: numba
+Requires-Dist: numpy>=1.20
 Requires-Dist: netcdf4
-Requires-Dist: openpyxl
 Requires-Dist: packaging
+Requires-Dist: rioxarray
 Requires-Dist: pandas
 Requires-Dist: pyflwdir>=0.5.4
 Requires-Dist: pyproj
 Requires-Dist: rasterio
-Requires-Dist: requests
-Requires-Dist: rioxarray
 Requires-Dist: shapely>=2.0.0
 Requires-Dist: scipy
-Requires-Dist: universal_pathlib
 Requires-Dist: xarray
+Requires-Dist: universal_pathlib
 Requires-Dist: xmltodict
 Requires-Dist: zarr
-Requires-Dist: pcraster ; extra == "all"
-Requires-Dist: xugrid ; extra == "all"
-Requires-Dist: pygeos ; extra == "all"
-Requires-Dist: pyet ; extra == "all"
+Requires-Dist: pcraster ; extra == "deprecated"
+Requires-Dist: pygeos ; extra == "deprecated"
+Requires-Dist: black ; extra == "dev"
+Requires-Dist: ruff ; extra == "dev"
+Requires-Dist: pre-commit ; extra == "dev"
+Requires-Dist: pip>=23.1.2 ; extra == "dev"
+Requires-Dist: flit ; extra == "dev"
+Requires-Dist: twine ; extra == "dev"
 Requires-Dist: nbsphinx ; extra == "doc"
 Requires-Dist: pydata-sphinx-theme ; extra == "doc"
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: sphinx_design ; extra == "doc"
 Requires-Dist: sphinx_autosummary_accessors ; extra == "doc"
-Requires-Dist: black ; extra == "test"
+Requires-Dist: hydromt[examples,extra] ; extra == "doc"
+Requires-Dist: jupyterlab ; extra == "examples"
+Requires-Dist: cartopy ; extra == "examples"
+Requires-Dist: matplotlib-base ; extra == "examples"
+Requires-Dist: notebook ; extra == "examples"
+Requires-Dist: xugrid ; extra == "extra"
+Requires-Dist: pyet ; extra == "extra"
+Requires-Dist: hydromt[io,extra,dev,test,doc,examples] ; extra == "full"
+Requires-Dist: s3fs ; extra == "io"
+Requires-Dist: gcsfs ; extra == "io"
+Requires-Dist: openpyxl ; extra == "io"
+Requires-Dist: requests ; extra == "io"
+Requires-Dist: fsspec==2023.5.0 ; extra == "io"
+Requires-Dist: hydromt[io,extra,examples] ; extra == "slim"
 Requires-Dist: pytest>=2.7.3 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-mock ; extra == "test"
-Requires-Dist: responses ; extra == "test"
 Project-URL: Documentation, https://deltares.github.io/hydromt
 Project-URL: Source, https://github.com/Deltares/hydromt
-Provides-Extra: all
+Provides-Extra: deprecated
+Provides-Extra: dev
 Provides-Extra: doc
+Provides-Extra: examples
+Provides-Extra: extra
+Provides-Extra: full
+Provides-Extra: io
+Provides-Extra: slim
 Provides-Extra: test
 
 .. _readme:
 
 ===============================================================
 HydroMT: Automated and reproducible model building and analysis
 ===============================================================
 
 |pypi| |conda forge| |docs_latest| |docs_stable| |binder| |codecov| |license| |doi| |joss_paper|
 
 
 What is HydroMT?
 ----------------
-**HydroMT** (Hydro Model Tools) is an open-source Python package that facilitates the process of 
-building and analyzing spatial geoscientific models with a focus on water system models. 
-It does so by automating the workflow to go from raw data to a complete model instance which 
-is ready to run and to analyse model results once the simulation has finished. 
-HydroMT builds on the latest packages in the scientific and geospatial python eco-system including 
+**HydroMT** (Hydro Model Tools) is an open-source Python package that facilitates the process of
+building and analyzing spatial geoscientific models with a focus on water system models.
+It does so by automating the workflow to go from raw data to a complete model instance which
+is ready to run and to analyse model results once the simulation has finished.
+HydroMT builds on the latest packages in the scientific and geospatial python eco-system including
 xarray_, rasterio_, rioxarray_, geopandas_, scipy_ and pyflwdir_.
 
 
 Why HydroMT?
 ------------
-Setting up spatial geoscientific models typically requires many (manual) steps 
-to process input data and might therefore be time consuming and hard to reproduce. 
-Especially improving models based on global geospatial datasets, which are 
-rapidly becoming available at increasingly high resolutions, might be challenging. 
-Furthermore, analyzing model schematization and results from different models, 
+Setting up spatial geoscientific models typically requires many (manual) steps
+to process input data and might therefore be time consuming and hard to reproduce.
+Especially improving models based on global geospatial datasets, which are
+rapidly becoming available at increasingly high resolutions, might be challenging.
+Furthermore, analyzing model schematization and results from different models,
 which often use model-specific peculiar data formats, can be time consuming.
-This package aims to make the model building process **fast**, **modular** and **reproducible** 
+This package aims to make the model building process **fast**, **modular** and **reproducible**
 by configuring the model building process from a single *ini* configuration file
-and **model- and data-agnostic** through a common model and data interface. 
+and **model- and data-agnostic** through a common model and data interface.
 
 
 How to use HydroMT?
 -------------------
 HydroMT can be used as a **command line** application (CLI) which provides commands to *build*,
 *update* and *clip* models with a single line, or **from Python** to exploit its rich interface.
 You can learn more about how to use HydroMT in its `online documentation. <https://deltares.github.io/hydromt/latest/>`_
-For a smooth installing experience, we recommend installing HydroMT and its dependencies 
+For a smooth installing experience, we recommend installing HydroMT and its dependencies
 from conda-forge in a clean environment, see `installation guide. <https://deltares.github.io/hydromt/latest/getting_started/installation>`_
 
 
 HydroMT model plugins
 ---------------------
-HydroMT is commonly used in combination with a **model plugin** which 
-provides a HydroMT implementation for specific model software. Using the plugins allows to prepare a ready-to-run set of input files from raw geoscientific datasets and analyse model results in a fast and reproducible way. 
+HydroMT is commonly used in combination with a **model plugin** which
+provides a HydroMT implementation for specific model software. Using the plugins allows to prepare a ready-to-run set of input files from raw geoscientific datasets and analyse model results in a fast and reproducible way.
 Known model plugins include:
 
 * hydromt_wflow_: A framework for distributed rainfall-runoff (wflow_sbm) and sediment transport (wflow_sediment) modelling.
 * hydromt_delwaq_: A framework for water quality (D-Water Quality) and emissions (D-Emissions) modelling.
 * hydromt_sfincs_: A fast 2D hydrodynamic flood model (SFINCS).
 * hydromt_fiat_: A flood impact model (FIAT).
 
@@ -119,17 +140,17 @@
 
 
 How to contribute?
 -------------------
 If you find any issues in the code or documentation feel free to leave an issue on the `github issue tracker. <https://github.com/Deltares/hydromt/issues>`_
 You can find information about how to contribute to the HydroMT project at our `contributing page. <https://deltares.github.io/hydromt/latest/dev/contributing>`_
 
-HydroMT seeks active contribution from the (hydro) geoscientific community. 
-So far, it has been developed and tested with a range of `Deltares <https://www.deltares.nl/en/>`_ models, but 
-we believe it is applicable to a much wider set of geoscientific models and are 
+HydroMT seeks active contribution from the (hydro) geoscientific community.
+So far, it has been developed and tested with a range of `Deltares <https://www.deltares.nl/en/>`_ models, but
+we believe it is applicable to a much wider set of geoscientific models and are
 happy to discuss how it can be implemented for your model.
 
 
 .. _scipy: https://scipy.org/
 .. _xarray: https://xarray.pydata.org
 .. _geopandas: https://geopandas.org
 .. _rioxarray: https://corteva.github.io/rioxarray/stable/
@@ -170,7 +191,8 @@
 
 .. |license| image:: https://img.shields.io/github/license/Deltares/hydromt?style=flat
     :alt: License
     :target: https://github.com/Deltares/hydromt/blob/main/LICENSE
 
 .. |joss_paper| image:: https://joss.theoj.org/papers/10.21105/joss.04897/status.svg
    :target: https://doi.org/10.21105/joss.04897
+
```

