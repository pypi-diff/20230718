# Comparing `tmp/windkit-0.6.2.tar.gz` & `tmp/windkit-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windkit-0.6.2.tar", last modified: Tue Jun 20 10:08:22 2023, max compression
+gzip compressed data, was "windkit-0.6.3.tar", last modified: Tue Jul 18 10:40:33 2023, max compression
```

## Comparing `windkit-0.6.2.tar` & `windkit-0.6.3.tar`

### file list

```diff
@@ -1,150 +1,149 @@
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:22.022385 windkit-0.6.2/
--rw-rw-r--   0 neil      (1000) neil      (1000)      461 2023-01-31 04:56:55.000000 windkit-0.6.2/.gitignore
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:21.986385 windkit-0.6.2/.gitlab/
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:21.998385 windkit-0.6.2/.gitlab/merge_request_templates/
--rw-rw-r--   0 neil      (1000) neil      (1000)      491 2023-01-31 04:56:55.000000 windkit-0.6.2/.gitlab/merge_request_templates/default.md
--rw-rw-r--   0 neil      (1000) neil      (1000)    12309 2023-03-14 11:45:01.000000 windkit-0.6.2/.gitlab-ci.yml
--rw-rw-r--   0 neil      (1000) neil      (1000)     1058 2023-03-14 11:45:01.000000 windkit-0.6.2/.pre-commit-config.yaml
--rw-rw-r--   0 neil      (1000) neil      (1000)     1261 2023-01-31 04:56:55.000000 windkit-0.6.2/.pylintrc
--rw-rw-r--   0 neil      (1000) neil      (1000)    14505 2023-06-20 10:07:06.000000 windkit-0.6.2/CHANGELOG.md
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:21.998385 windkit-0.6.2/CI_helper_scripts/
--rwxrwxr-x   0 neil      (1000) neil      (1000)      624 2023-01-31 04:56:55.000000 windkit-0.6.2/CI_helper_scripts/post_build_test_nix.sh
--rwxrwxr-x   0 neil      (1000) neil      (1000)      680 2023-01-31 04:56:55.000000 windkit-0.6.2/CI_helper_scripts/post_build_test_win.sh
--rw-rw-r--   0 neil      (1000) neil      (1000)     1523 2023-01-31 04:56:55.000000 windkit-0.6.2/LICENSE
--rw-rw-r--   0 neil      (1000) neil      (1000)      149 2023-02-14 09:38:21.000000 windkit-0.6.2/MANIFEST.in
--rw-rw-r--   0 neil      (1000) neil      (1000)     4045 2023-06-20 10:08:22.022385 windkit-0.6.2/PKG-INFO
--rw-rw-r--   0 neil      (1000) neil      (1000)     2634 2023-06-20 05:48:52.000000 windkit-0.6.2/README-Internal.md
--rw-rw-r--   0 neil      (1000) neil      (1000)     3537 2023-01-31 04:56:55.000000 windkit-0.6.2/README.md
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:21.998385 windkit-0.6.2/docs/
--rw-rw-r--   0 neil      (1000) neil      (1000)       82 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/.dockerignore
--rw-rw-r--   0 neil      (1000) neil      (1000)       11 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/.gitignore
--rw-rw-r--   0 neil      (1000) neil      (1000)      108 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/Dockerfile
--rw-rw-r--   0 neil      (1000) neil      (1000)     7042 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/Makefile
--rw-rw-r--   0 neil      (1000) neil      (1000)      559 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/docker-compose.yml
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:21.986385 windkit-0.6.2/docs/legacy/
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:21.998385 windkit-0.6.2/docs/legacy/dev/
--rw-rw-r--   0 neil      (1000) neil      (1000)     2228 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/legacy/dev/dev-git.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)     1759 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/legacy/dev/dev-intro.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)     2208 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/legacy/dev/dev-pytest.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)     1418 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/legacy/dev/dev-sphinx.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)      239 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/nginx.conf
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:22.002385 windkit-0.6.2/docs/source/
--rw-rw-r--   0 neil      (1000) neil      (1000)     9713 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/source/WAsP.bib
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:21.990385 windkit-0.6.2/docs/source/_templates/
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:22.002385 windkit-0.6.2/docs/source/_templates/autosummary/
--rw-rw-r--   0 neil      (1000) neil      (1000)      585 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/source/_templates/autosummary/class.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)      693 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/source/_templates/autosummary/module.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)     9885 2023-03-14 11:45:01.000000 windkit-0.6.2/docs/source/conf.py
--rw-rw-r--   0 neil      (1000) neil      (1000)      125 2023-03-14 11:45:01.000000 windkit-0.6.2/docs/source/development_roadmap.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)     1358 2023-03-14 11:45:01.000000 windkit-0.6.2/docs/source/index.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)     4567 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/source/installation.rst
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:22.002385 windkit-0.6.2/docs/source/io/
--rw-rw-r--   0 neil      (1000) neil      (1000)     4014 2023-03-14 11:45:01.000000 windkit-0.6.2/docs/source/io/io.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)      241 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/source/map_conversion.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)       66 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/source/map_conversion_examples_nb.nblink
--rw-rw-r--   0 neil      (1000) neil      (1000)      439 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/source/plotting.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)      301 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/source/plotting_examples.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)       53 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/source/plotting_examples_nb.nblink
--rw-rw-r--   0 neil      (1000) neil      (1000)    10214 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/source/plotting_user_guide.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)      127 2023-03-14 11:45:01.000000 windkit-0.6.2/docs/source/release_notes.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)     4794 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/source/topographic_data.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)     3232 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/source/wind_climate_objects.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)     5859 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/source/windkit.rst
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:22.006385 windkit-0.6.2/env/
--rw-rw-r--   0 neil      (1000) neil      (1000)      498 2023-01-31 04:56:55.000000 windkit-0.6.2/env/Dockerfile.api
--rw-rw-r--   0 neil      (1000) neil      (1000)     1209 2023-03-14 11:45:01.000000 windkit-0.6.2/env/Dockerfile.ci
--rw-rw-r--   0 neil      (1000) neil      (1000)      421 2023-01-31 04:56:55.000000 windkit-0.6.2/env/Dockerfile.miniconda
--rw-rw-r--   0 neil      (1000) neil      (1000)      187 2023-03-14 11:45:01.000000 windkit-0.6.2/env/Makefile
--rw-rw-r--   0 neil      (1000) neil      (1000)      891 2023-06-20 05:48:25.000000 windkit-0.6.2/env/conda-linux-64.lock
--rw-rw-r--   0 neil      (1000) neil      (1000)    35182 2023-01-31 04:56:55.000000 windkit-0.6.2/env/conda-osx-64.lock
--rw-rw-r--   0 neil      (1000) neil      (1000)    42058 2023-02-14 09:38:21.000000 windkit-0.6.2/env/conda-win-64.lock
--rw-rw-r--   0 neil      (1000) neil      (1000)     1692 2023-02-14 09:38:21.000000 windkit-0.6.2/env/create_locks.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     1066 2023-03-14 11:45:01.000000 windkit-0.6.2/env/dev_env.yaml
--rw-rw-r--   0 neil      (1000) neil      (1000)      186 2023-02-14 09:38:21.000000 windkit-0.6.2/env/pywasp.cfg
--rw-rw-r--   0 neil      (1000) neil      (1000)      653 2023-02-14 09:38:21.000000 windkit-0.6.2/env/pywasp_env.yml
--rw-rw-r--   0 neil      (1000) neil      (1000)      470 2023-02-14 09:38:21.000000 windkit-0.6.2/env/pywaspio_env.yml
--rw-rw-r--   0 neil      (1000) neil      (1000)       78 2023-02-14 09:38:21.000000 windkit-0.6.2/env/windkit.ini
--rw-rw-r--   0 neil      (1000) neil      (1000)      441 2023-02-07 11:47:48.000000 windkit-0.6.2/pyproject.toml
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:22.006385 windkit-0.6.2/recipe/
--rw-rw-r--   0 neil      (1000) neil      (1000)      667 2023-03-14 11:45:01.000000 windkit-0.6.2/recipe/meta.yaml
--rw-rw-r--   0 neil      (1000) neil      (1000)      962 2023-06-20 10:08:22.022385 windkit-0.6.2/setup.cfg
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:22.014385 windkit-0.6.2/windkit/
--rw-rw-r--   0 neil      (1000) neil      (1000)     1153 2023-06-20 05:48:25.000000 windkit-0.6.2/windkit/__init__.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     1726 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/_errors.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     8505 2023-03-14 11:45:01.000000 windkit-0.6.2/windkit/_rvea_xml.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     2179 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/_validate.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    11639 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/_vectormap_gml.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     5008 2023-03-14 11:45:01.000000 windkit-0.6.2/windkit/_vectormap_helpers.py
--rw-rw-r--   0 neil      (1000) neil      (1000)      160 2023-06-20 10:08:21.000000 windkit-0.6.2/windkit/_version.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    37804 2023-02-14 09:38:21.000000 windkit-0.6.2/windkit/all_vars.json
--rw-rw-r--   0 neil      (1000) neil      (1000)    32058 2023-02-14 09:38:21.000000 windkit-0.6.2/windkit/binned_wind_climate.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     4910 2023-06-20 05:48:25.000000 windkit-0.6.2/windkit/cfd.py
--rw-rw-r--   0 neil      (1000) neil      (1000)      155 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/config.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     1030 2023-06-20 05:48:25.000000 windkit-0.6.2/windkit/data_structures.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     1110 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/elevation_map.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    17220 2023-06-20 05:27:05.000000 windkit-0.6.2/windkit/empty.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    21529 2023-03-14 11:45:01.000000 windkit-0.6.2/windkit/generalized_wind_climate.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     1131 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/geospatial_imports.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     9775 2023-02-14 09:38:21.000000 windkit-0.6.2/windkit/get_map.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     8201 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/landcover.py
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:22.018385 windkit-0.6.2/windkit/landcovertables/
--rw-rw-r--   0 neil      (1000) neil      (1000)     1943 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/landcovertables/CGLS-LC100.json
--rw-rw-r--   0 neil      (1000) neil      (1000)     5736 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/landcovertables/CORINE.json
--rw-rw-r--   0 neil      (1000) neil      (1000)     2643 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/landcovertables/Globcover.json
--rw-rw-r--   0 neil      (1000) neil      (1000)     1315 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/landcovertables/MODIS.json
--rw-rw-r--   0 neil      (1000) neil      (1000)      883 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/landcovertables/WorldCover.json
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:22.018385 windkit-0.6.2/windkit/map_conversion/
--rw-rw-r--   0 neil      (1000) neil      (1000)        0 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/map_conversion/__init__.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     1757 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/map_conversion/helper_functions.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    24213 2023-03-14 11:45:01.000000 windkit-0.6.2/windkit/map_conversion/lines2poly.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    21612 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/map_conversion/poly2lines.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    12972 2023-03-14 11:45:01.000000 windkit-0.6.2/windkit/map_file_header_to_epsg.json
--rw-rw-r--   0 neil      (1000) neil      (1000)    16270 2023-06-20 05:48:25.000000 windkit-0.6.2/windkit/metadata.py
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:22.018385 windkit-0.6.2/windkit/plot/
--rw-rw-r--   0 neil      (1000) neil      (1000)      889 2023-02-14 09:38:21.000000 windkit-0.6.2/windkit/plot/__init__.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     1237 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/plot/_colormaps.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     3859 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/plot/_helpers.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     8517 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/plot/color.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    16579 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/plot/histogram.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     2605 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/plot/landcover_map.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    13441 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/plot/operational_curves.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     4040 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/plot/raster_plot.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     5476 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/plot/roughness_rose.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     5569 2023-06-20 05:48:25.000000 windkit-0.6.2/windkit/plot/vertical_profile.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     8993 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/plot/wind_rose.py
--rw-rw-r--   0 neil      (1000) neil      (1000)      981 2023-02-14 09:38:21.000000 windkit-0.6.2/windkit/plot/wind_turbine.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    12330 2023-02-14 09:38:21.000000 windkit-0.6.2/windkit/raster_map.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     1096 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/roughness_map.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     4708 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/sector.py
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:22.022385 windkit-0.6.2/windkit/spatial/
--rw-rw-r--   0 neil      (1000) neil      (1000)     1684 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/spatial/README.md
--rw-rw-r--   0 neil      (1000) neil      (1000)     1433 2023-03-14 11:45:01.000000 windkit-0.6.2/windkit/spatial/__init__.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     5989 2023-02-14 09:38:21.000000 windkit-0.6.2/windkit/spatial/_bbox.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     4003 2023-03-14 11:45:01.000000 windkit-0.6.2/windkit/spatial/_crs.py
--rw-rw-r--   0 neil      (1000) neil      (1000)      754 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/spatial/_cuboid.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     1432 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/spatial/_dimensions.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     4676 2023-02-14 09:38:21.000000 windkit-0.6.2/windkit/spatial/_interpolation.py
--rw-rw-r--   0 neil      (1000) neil      (1000)      775 2023-02-14 09:38:21.000000 windkit-0.6.2/windkit/spatial/_latitude.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     8724 2023-03-14 11:45:01.000000 windkit-0.6.2/windkit/spatial/_point.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    19130 2023-05-16 14:34:54.000000 windkit-0.6.2/windkit/spatial/_raster.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     7062 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/spatial/_struct.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     4062 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/spatial/_utm.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     2808 2023-02-14 09:38:21.000000 windkit-0.6.2/windkit/spatial/_vector.py
--rw-rw-r--   0 neil      (1000) neil      (1000)      300 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/spatial/_vertical.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     2530 2023-02-14 09:38:21.000000 windkit-0.6.2/windkit/spatial/decorators.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    25867 2023-06-20 05:48:25.000000 windkit-0.6.2/windkit/spatial/spatial.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    13485 2023-06-20 05:48:25.000000 windkit-0.6.2/windkit/time_series_wind_climate.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    18766 2023-06-20 05:48:25.000000 windkit-0.6.2/windkit/vector_map.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    11843 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/weibull.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    21666 2023-06-20 06:55:20.000000 windkit-0.6.2/windkit/weibull_wind_climate.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     3870 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/wind.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     3611 2023-02-14 09:38:21.000000 windkit-0.6.2/windkit/wind_climate.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    22640 2023-03-14 11:45:01.000000 windkit-0.6.2/windkit/wind_turbine.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    21523 2023-03-14 11:45:01.000000 windkit-0.6.2/windkit/workspace.py
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:22.014385 windkit-0.6.2/windkit.egg-info/
--rw-rw-r--   0 neil      (1000) neil      (1000)     4045 2023-06-20 10:08:21.000000 windkit-0.6.2/windkit.egg-info/PKG-INFO
--rw-rw-r--   0 neil      (1000) neil      (1000)     3383 2023-06-20 10:08:21.000000 windkit-0.6.2/windkit.egg-info/SOURCES.txt
--rw-rw-r--   0 neil      (1000) neil      (1000)        1 2023-06-20 10:08:21.000000 windkit-0.6.2/windkit.egg-info/dependency_links.txt
--rw-rw-r--   0 neil      (1000) neil      (1000)       63 2023-06-20 10:08:21.000000 windkit-0.6.2/windkit.egg-info/entry_points.txt
--rw-rw-r--   0 neil      (1000) neil      (1000)      244 2023-06-20 10:08:21.000000 windkit-0.6.2/windkit.egg-info/requires.txt
--rw-rw-r--   0 neil      (1000) neil      (1000)        8 2023-06-20 10:08:21.000000 windkit-0.6.2/windkit.egg-info/top_level.txt
+drwxr-xr-x   0 mambauser  (1000) mambauser  (1000)        0 2023-07-18 10:40:33.965649 windkit-0.6.3/
+drwxr-xr-x   0 mambauser  (1000) mambauser  (1000)        0 2023-07-18 10:40:33.809648 windkit-0.6.3/.conda_env/
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      750 2023-07-18 07:50:50.000000 windkit-0.6.3/.conda_env/dev_unix.yml
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      774 2023-07-18 07:50:50.000000 windkit-0.6.3/.conda_env/dev_win.yml
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      189 2023-06-21 08:13:25.000000 windkit-0.6.3/.conda_env/prod_unix.yml
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      461 2023-05-26 09:25:17.000000 windkit-0.6.3/.gitignore
+drwxr-xr-x   0 mambauser  (1000) mambauser  (1000)        0 2023-07-18 10:40:33.793647 windkit-0.6.3/.gitlab/
+drwxr-xr-x   0 mambauser  (1000) mambauser  (1000)        0 2023-07-18 10:40:33.809648 windkit-0.6.3/.gitlab/issue_templates/
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)       97 2023-07-18 09:05:19.000000 windkit-0.6.3/.gitlab/issue_templates/release.md
+drwxr-xr-x   0 mambauser  (1000) mambauser  (1000)        0 2023-07-18 10:40:33.813648 windkit-0.6.3/.gitlab/merge_request_templates/
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      491 2023-05-26 09:25:17.000000 windkit-0.6.3/.gitlab/merge_request_templates/default.md
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     2591 2023-06-21 08:13:25.000000 windkit-0.6.3/.gitlab-ci.yml
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     1113 2023-06-21 08:13:25.000000 windkit-0.6.3/.pre-commit-config.yaml
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     1261 2023-05-26 09:25:17.000000 windkit-0.6.3/.pylintrc
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)    17744 2023-07-18 09:05:19.000000 windkit-0.6.3/CHANGELOG.md
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     1523 2023-05-26 09:25:17.000000 windkit-0.6.3/LICENSE
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      202 2023-06-21 08:13:25.000000 windkit-0.6.3/MANIFEST.in
+-rw-r--r--   0 mambauser  (1000) mambauser  (1000)     4045 2023-07-18 10:40:33.965649 windkit-0.6.3/PKG-INFO
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     2634 2023-06-21 08:13:25.000000 windkit-0.6.3/README-Internal.md
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     3537 2023-06-22 09:36:17.000000 windkit-0.6.3/README.md
+drwxr-xr-x   0 mambauser  (1000) mambauser  (1000)        0 2023-07-18 10:40:33.817648 windkit-0.6.3/docs/
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)       82 2023-05-26 09:25:17.000000 windkit-0.6.3/docs/.dockerignore
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)       11 2023-05-26 09:25:17.000000 windkit-0.6.3/docs/.gitignore
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      108 2023-05-26 09:25:17.000000 windkit-0.6.3/docs/Dockerfile
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     7042 2023-05-26 09:25:17.000000 windkit-0.6.3/docs/Makefile
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      559 2023-05-26 09:25:17.000000 windkit-0.6.3/docs/docker-compose.yml
+drwxr-xr-x   0 mambauser  (1000) mambauser  (1000)        0 2023-07-18 10:40:33.793647 windkit-0.6.3/docs/legacy/
+drwxr-xr-x   0 mambauser  (1000) mambauser  (1000)        0 2023-07-18 10:40:33.821648 windkit-0.6.3/docs/legacy/dev/
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     2228 2023-05-26 09:25:17.000000 windkit-0.6.3/docs/legacy/dev/dev-git.rst
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     1759 2023-05-26 09:25:17.000000 windkit-0.6.3/docs/legacy/dev/dev-intro.rst
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     2208 2023-05-26 09:25:17.000000 windkit-0.6.3/docs/legacy/dev/dev-pytest.rst
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     1418 2023-05-26 09:25:17.000000 windkit-0.6.3/docs/legacy/dev/dev-sphinx.rst
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      239 2023-05-26 09:25:17.000000 windkit-0.6.3/docs/nginx.conf
+drwxr-xr-x   0 mambauser  (1000) mambauser  (1000)        0 2023-07-18 10:40:33.845648 windkit-0.6.3/docs/source/
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     9713 2023-05-26 09:25:17.000000 windkit-0.6.3/docs/source/WAsP.bib
+drwxr-xr-x   0 mambauser  (1000) mambauser  (1000)        0 2023-07-18 10:40:33.793647 windkit-0.6.3/docs/source/_templates/
+drwxr-xr-x   0 mambauser  (1000) mambauser  (1000)        0 2023-07-18 10:40:33.845648 windkit-0.6.3/docs/source/_templates/autosummary/
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      585 2023-05-26 09:25:17.000000 windkit-0.6.3/docs/source/_templates/autosummary/class.rst
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      693 2023-05-26 09:25:17.000000 windkit-0.6.3/docs/source/_templates/autosummary/module.rst
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     9942 2023-07-18 07:50:50.000000 windkit-0.6.3/docs/source/conf.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      125 2023-05-26 09:25:17.000000 windkit-0.6.3/docs/source/development_roadmap.rst
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      532 2023-07-18 07:50:50.000000 windkit-0.6.3/docs/source/getting_started.rst
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     1362 2023-07-18 07:50:50.000000 windkit-0.6.3/docs/source/index.rst
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     4567 2023-05-26 09:25:17.000000 windkit-0.6.3/docs/source/installation.rst
+drwxr-xr-x   0 mambauser  (1000) mambauser  (1000)        0 2023-07-18 10:40:33.849648 windkit-0.6.3/docs/source/io/
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     4014 2023-05-26 09:25:17.000000 windkit-0.6.3/docs/source/io/io.rst
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      241 2023-05-26 09:25:17.000000 windkit-0.6.3/docs/source/map_conversion.rst
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)       66 2023-05-26 09:25:17.000000 windkit-0.6.3/docs/source/map_conversion_examples_nb.nblink
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      439 2023-05-26 09:25:17.000000 windkit-0.6.3/docs/source/plotting.rst
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      301 2023-05-26 09:25:17.000000 windkit-0.6.3/docs/source/plotting_examples.rst
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)       53 2023-05-26 09:25:17.000000 windkit-0.6.3/docs/source/plotting_examples_nb.nblink
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)    10214 2023-05-26 09:25:17.000000 windkit-0.6.3/docs/source/plotting_user_guide.rst
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      127 2023-05-26 09:25:17.000000 windkit-0.6.3/docs/source/release_notes.rst
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     4794 2023-05-26 09:25:17.000000 windkit-0.6.3/docs/source/topographic_data.rst
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     3232 2023-05-26 09:25:17.000000 windkit-0.6.3/docs/source/wind_climate_objects.rst
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     5859 2023-05-26 09:25:17.000000 windkit-0.6.3/docs/source/windkit.rst
+drwxr-xr-x   0 mambauser  (1000) mambauser  (1000)        0 2023-07-18 10:40:33.865648 windkit-0.6.3/env/
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      498 2023-05-26 09:25:17.000000 windkit-0.6.3/env/Dockerfile.api
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     1209 2023-05-26 09:25:17.000000 windkit-0.6.3/env/Dockerfile.ci
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      421 2023-05-26 09:25:17.000000 windkit-0.6.3/env/Dockerfile.miniconda
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      187 2023-05-26 09:25:17.000000 windkit-0.6.3/env/Makefile
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      871 2023-07-18 07:50:50.000000 windkit-0.6.3/env/conda-linux-64.lock
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)    35182 2023-05-26 09:25:17.000000 windkit-0.6.3/env/conda-osx-64.lock
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)    42058 2023-05-26 09:25:17.000000 windkit-0.6.3/env/conda-win-64.lock
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     1692 2023-05-26 09:25:17.000000 windkit-0.6.3/env/create_locks.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     1046 2023-07-18 07:50:50.000000 windkit-0.6.3/env/dev_env.yaml
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      186 2023-05-26 09:25:17.000000 windkit-0.6.3/env/pywasp.cfg
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      653 2023-05-26 09:25:17.000000 windkit-0.6.3/env/pywasp_env.yml
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      470 2023-05-26 09:25:17.000000 windkit-0.6.3/env/pywaspio_env.yml
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)       78 2023-05-26 09:25:17.000000 windkit-0.6.3/env/windkit.ini
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      441 2023-05-26 09:25:17.000000 windkit-0.6.3/pyproject.toml
+drwxr-xr-x   0 mambauser  (1000) mambauser  (1000)        0 2023-07-18 10:40:33.865648 windkit-0.6.3/recipe/
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      757 2023-07-18 07:50:50.000000 windkit-0.6.3/recipe/meta.yaml
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     1033 2023-07-18 10:40:33.965649 windkit-0.6.3/setup.cfg
+drwxr-xr-x   0 mambauser  (1000) mambauser  (1000)        0 2023-07-18 10:40:33.913648 windkit-0.6.3/windkit/
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     1153 2023-07-17 09:23:52.000000 windkit-0.6.3/windkit/__init__.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     1726 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/_errors.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     8505 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/_rvea_xml.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     2179 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/_validate.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)    11639 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/_vectormap_gml.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     5206 2023-07-18 07:50:50.000000 windkit-0.6.3/windkit/_vectormap_helpers.py
+-rw-r--r--   0 mambauser  (1000) mambauser  (1000)      161 2023-07-18 10:40:32.000000 windkit-0.6.3/windkit/_version.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)    37966 2023-07-18 07:50:50.000000 windkit-0.6.3/windkit/all_vars.json
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)    32058 2023-06-26 12:43:40.000000 windkit-0.6.3/windkit/binned_wind_climate.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     4910 2023-06-01 12:03:20.000000 windkit-0.6.3/windkit/cfd.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      155 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/config.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     1030 2023-06-22 14:04:53.000000 windkit-0.6.3/windkit/data_structures.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     1110 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/elevation_map.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)    17283 2023-07-18 09:05:19.000000 windkit-0.6.3/windkit/empty.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)    21529 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/generalized_wind_climate.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     1131 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/geospatial_imports.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     9775 2023-07-17 09:23:52.000000 windkit-0.6.3/windkit/get_map.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     8201 2023-07-05 08:57:02.000000 windkit-0.6.3/windkit/landcover.py
+drwxr-xr-x   0 mambauser  (1000) mambauser  (1000)        0 2023-07-18 10:40:33.921649 windkit-0.6.3/windkit/landcovertables/
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     1943 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/landcovertables/CGLS-LC100.json
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     5736 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/landcovertables/CORINE.json
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     2643 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/landcovertables/Globcover.json
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     1315 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/landcovertables/MODIS.json
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      883 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/landcovertables/WorldCover.json
+drwxr-xr-x   0 mambauser  (1000) mambauser  (1000)        0 2023-07-18 10:40:33.925649 windkit-0.6.3/windkit/map_conversion/
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)        0 2023-07-18 10:38:09.000000 windkit-0.6.3/windkit/map_conversion/__init__.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     1757 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/map_conversion/helper_functions.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)    24213 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/map_conversion/lines2poly.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)    21758 2023-07-18 07:50:50.000000 windkit-0.6.3/windkit/map_conversion/poly2lines.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)    12972 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/map_file_header_to_epsg.json
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)    16474 2023-07-18 07:50:50.000000 windkit-0.6.3/windkit/metadata.py
+drwxr-xr-x   0 mambauser  (1000) mambauser  (1000)        0 2023-07-18 10:40:33.941649 windkit-0.6.3/windkit/plot/
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      889 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/plot/__init__.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     1237 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/plot/_colormaps.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     3859 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/plot/_helpers.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     8517 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/plot/color.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)    16579 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/plot/histogram.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     2605 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/plot/landcover_map.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)    13441 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/plot/operational_curves.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     4040 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/plot/raster_plot.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     5476 2023-06-12 13:22:01.000000 windkit-0.6.3/windkit/plot/roughness_rose.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     5569 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/plot/vertical_profile.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     8993 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/plot/wind_rose.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      981 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/plot/wind_turbine.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)    12330 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/raster_map.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     1096 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/roughness_map.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     5449 2023-07-03 08:57:53.000000 windkit-0.6.3/windkit/sector.py
+drwxr-xr-x   0 mambauser  (1000) mambauser  (1000)        0 2023-07-18 10:40:33.965649 windkit-0.6.3/windkit/spatial/
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     1684 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/spatial/README.md
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     1433 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/spatial/__init__.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)    10277 2023-07-18 07:50:50.000000 windkit-0.6.3/windkit/spatial/_bbox.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     4003 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/spatial/_crs.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      754 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/spatial/_cuboid.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     1432 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/spatial/_dimensions.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     4676 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/spatial/_interpolation.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      775 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/spatial/_latitude.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     8724 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/spatial/_point.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)    19130 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/spatial/_raster.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     7062 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/spatial/_struct.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     4062 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/spatial/_utm.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     2808 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/spatial/_vector.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)      300 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/spatial/_vertical.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     2530 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/spatial/decorators.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)    25867 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/spatial/spatial.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)    13512 2023-07-18 07:50:50.000000 windkit-0.6.3/windkit/time_series_wind_climate.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)    20474 2023-07-18 07:50:50.000000 windkit-0.6.3/windkit/vector_map.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)    11843 2023-06-22 14:04:53.000000 windkit-0.6.3/windkit/weibull.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)    27356 2023-07-03 08:57:53.000000 windkit-0.6.3/windkit/weibull_wind_climate.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     3870 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/wind.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)     3611 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/wind_climate.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)    26020 2023-07-18 07:50:50.000000 windkit-0.6.3/windkit/wind_turbine.py
+-rw-rw-rw-   0 mambauser  (1000) mambauser  (1000)    21523 2023-05-26 09:25:17.000000 windkit-0.6.3/windkit/workspace.py
+drwxr-xr-x   0 mambauser  (1000) mambauser  (1000)        0 2023-07-18 10:40:33.965649 windkit-0.6.3/windkit.egg-info/
+-rw-r--r--   0 mambauser  (1000) mambauser  (1000)     3252 2023-07-18 10:40:33.000000 windkit-0.6.3/windkit.egg-info/SOURCES.txt
```

### Comparing `windkit-0.6.2/.pre-commit-config.yaml` & `windkit-0.6.3/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v3.1.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-yaml
-        exclude: .gitlab-ci.yml|meta.yaml
+        exclude: .gitlab-ci.yml|meta.yaml|.ci-includes/run_pytest.yml|.ci-includes/py_deploy.yml
       - id: check-merge-conflict
       - id: fix-encoding-pragma
         args: [--remove]
       - id: mixed-line-ending
         args: [--fix=no]
         exclude: "test/test_old/data/|test/data/|test_old/data/"
       - id: check-json
```

### Comparing `windkit-0.6.2/.pylintrc` & `windkit-0.6.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/CHANGELOG.md` & `windkit-0.6.3/CHANGELOG.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,53 @@
 # Changelog
 
 All major changes are listed here.
 
+## 0.6.3 (2023-07-18)
+
+### New Features
+
+#### Enhanced bounding box object
+
+Several new methods were added to the BBox object to make it easier to work with.
+
+* Create BBox objects in more ways:
+    * `BBox.from_bounds` as alias to `BBox.from_cornerpts` and set default crs to `EPSG:4326`
+    * `BBox.from_point_and_buffer` to create a bbox from a x,y-point, a buffer size, and a crs
+    * `BBox.utm_bbox_from_geographic_coordinate` to create a bbox from a geographic coordinate (point) and a buffer in meters, projecting to the appropriate UTM coordinates.
+* Simplified reproject to geographic and UTM coordinates
+    * Added method `BBox.reproject_to_geographic()` to reproject a bbox to geographic coordinates
+    * Added method `BBox.reproject_to_utm()` to reproject a bbox to UTM coordinates
+* Return data in common GIS formats using:
+    * Added method `BBox.polygon` property to return a shapely polygon
+    * Added method `BBox.envelope()` to return an enveloped bbox in the current crs
+* Create a simple plot of your BBox using `BBox.plot()`
+
+#### Formatting improvements when writing .wrg/.rsf files
+
+* `windkit.to_rsffile` and `windkit.to_wrgfile` now attempts to match the WAsP formatting more closely and a new `formatters` argument allows the user to specify the formatting for each column. This allows for more control over the formatting of the output file. Additional formatting checks have also been added to ensure that the formatting is correct.
+
+#### Require regulation_type for wtg data structures
+
+* The WindTurbineGenerator now requires a regulation_type variable. When reading in a WTG using `windkit.read_wtg`, the default mode is pitch. You can set it to stall or have it autodetected using the new `windkit.wind_turbine.estimate_regulation_type` function.
+* Validation functions have been added to the WTG object type, so you can now ensure that your Dataset has the correct format before using the WTG.
+
+#### Allow use of Polygons for defining landcover data
+
+* `windkit.read_vector_map` Now can read polygon based landcover vector map files in `gpkg` format, which is commonly used in GIS tools. The function has a new parameter `background_lc_id` that is needed to setup the background for polygon based vector maps.
+
+### Changes
+* `windkit.read_vector_map`: For landcover data in `gpkg` format,`id` is now the default name used to identify landcover ID's in the landcover table. For old `gpkg` files where the name `index` is used, `windkit.read_vector_map` will print a `FutureWarning`.
+* Remove dependency on `cf-xarray`, as we have our own metadata vocabulary. This fixes an issue where Pooch was an optional dependency of `cf-xarray`, but required for the functionality used by WindKit.
+
+### BugFixes
+
+* Prevent exception when running in the python interpreter and calling `windkit.metadata.update_history`. Now a the generic message "Unknown python interpreter command." is added to the object history in this scenario. To get a correct history, it is recommended to use iPython for interactive sessions.
+* Fixed a bug in `BBox.buffer`, which would cause negative buffering to not preserve bbox shape
+
 ## 0.6.2 (2023-06-20)
 
 ### New Features
 
 #### New file reading functions
 
 * `windkit.read_timeseries_from_pandas` and `windkit.read_timeseries_from_csv` build a time-series wind climate `xarray.Dataset` from time-series data in tabular form, either a `pandas` Dataframe or a `csv` file. The functions attempt to auto-detect the wind speed and wind direction columns based on a standard list of names if they are not provided.
@@ -13,20 +55,21 @@
 
 #### Detection of CRS from WAsP .map files
 
 * `windkit.read_vector_map` and by extension `windkit.read_elevation_map` and `windkit.read_roughness_map` now try to detect CRS information from the header of WAsP `.map` files, which can be added using recent versions of the WAsP MapEditor. In case there is a problem (e.g. wrong format) it will raise an error.
 
 #### Updates to vertical profile plotting
 
-* `windkit.plot.vertical_profile` Function now works for data arrays without their attributes set. If the height coordinate does not have attributes, `Height [m]` will be used for the y-axis. If the data variable to plot does not have attributes, `DataArray.name` will be used for the x-axis. 
+* `windkit.plot.vertical_profile` Function now works for data arrays without their attributes set. If the height coordinate does not have attributes, `Height [m]` will be used for the y-axis. If the data variable to plot does not have attributes, `DataArray.name` will be used for the x-axis.
 * `windkit.plot.vertical_profile` no longer allows plotting of objects with a `time` coordinate. This is due to performance limitations when plotting potentially thousands of points when a time-series object is passed.
 
 ### Breaking changes
 
-* When creating a file using `windkit.to_rsffile` and `windkit.to_wrgfile` or reading a file using `wk.read_rsffile` and `wk.read_wrgfile`, the elevation variable has been renamed from `elevation` to `site_elev`. This now matches the variable name used in PyWAsP. 
+* When creating a file using `windkit.to_rsffile` and `windkit.to_wrgfile` or reading a file using `wk.read_rsffile` and `wk.read_wrgfile`, the elevation variable has been renamed from `elevation` to `site_elev`. This now matches the variable name used in PyWAsP.
+* class `windkit.WindTurbines` does not allow wind turbine `xarray.Dataset` with more than one mode.
 
 ### Changes
 
 * `windkit.spatial.nearest_points` will issue a warning instead of a `ValueError` when it is used on datasets with geographical coordinates.
 * `windkit.to_rsffile` and `windkit.to_wrgfile` calculate necessary parameters met_fields, "power_density", "combined_A", "combined_k", and "wspd", from a wwc if they aren't included.
 
 ### Bug Fixes
@@ -107,15 +150,15 @@
 * Requires `geopandas>=0.11`.
 * Requires `rioxarray` for reading raster GIS files.
 
 ### Deprecations
 
 ### Changes
 
-* To support `pyproj` 3.4.0, changed from `pyproj.crs.CRS.is_exact_same` to `pyproj.crs.CRS.equals`, and dropped deprecated `skip_equivalent` kwarg.
+* To support `pyproj` 3.4.0, changed from `pyproj.crs.CRS.is_exact_same` to `pyproj.crs.CRS.equals`, and dropped deprecated `skip_equivalent` kwargs.
 * Drop `south_north` and `west_east` coords before reassigning them as required in [future `xarray` version](https://github.com/pydata/xarray/issues/6505).
 * Added height dependent wind direction frequencies to GWC I/O routines
   - For the .lib-file reader frequencies are duplicated across all gen_heights
   - For the .lib-file writer a check is made to ensure all frequencies are these same across heights. If they are not, a gen_height is required to be set by the user.
 
 ### Improvements
  * Sped up creation of .lib strings for GWC objects. In testing 15 sites, went from 11s to <1.
```

### Comparing `windkit-0.6.2/LICENSE` & `windkit-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/PKG-INFO` & `windkit-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windkit
-Version: 0.6.2
+Version: 0.6.3
 Summary: WindKit provides core functionalities for working with wind resource data
 Home-page: https://docs-wasp.ramtt.xyz/windkit
 Author: DTU Wind Energy
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `windkit-0.6.2/README-Internal.md` & `windkit-0.6.3/README-Internal.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,16 @@
 
 # Build & deploy conda
 # This cannot be done from a submodule folder, windkit must be cloned in a different folder.
 rm -r conda_build
 export VERSION=<version>
 time conda mambabuild -c https://conda.windenergy.dtu.dk/channel/open --output-folder conda_build  ./recipe
 
-rsync -auPv conda_build/ VIND-pWASPInt01:~/.
-ssh VIND-pWASPInt01
+rsync -auPv conda_build/ VIND-pWASPint01:~/.
+ssh VIND-pWASPint01
   sudo rsync --ignore-existing -tprm --include=*/ --include=*.tar.bz2 --exclude=* conda_build/ /mnt/data/external/rw/conda-channel/basic_auth_node_server/conda/open/
   sudo chown -R 1000:1000 /mnt/data/external/rw/conda-channel/basic_auth_node_server/conda/
   # To check whether it worked correctly, go to  https://conda.windenergy.dtu.dk/channel/open/noarch/
 ```
 
 ### Build and deploy docs
```

### Comparing `windkit-0.6.2/README.md` & `windkit-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/docs/Makefile` & `windkit-0.6.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/docs/docker-compose.yml` & `windkit-0.6.3/docs/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/docs/legacy/dev/dev-git.rst` & `windkit-0.6.3/docs/legacy/dev/dev-git.rst`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/docs/legacy/dev/dev-intro.rst` & `windkit-0.6.3/docs/legacy/dev/dev-intro.rst`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/docs/legacy/dev/dev-pytest.rst` & `windkit-0.6.3/docs/legacy/dev/dev-pytest.rst`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/docs/legacy/dev/dev-sphinx.rst` & `windkit-0.6.3/docs/legacy/dev/dev-sphinx.rst`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/docs/source/WAsP.bib` & `windkit-0.6.3/docs/source/WAsP.bib`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/docs/source/_templates/autosummary/class.rst` & `windkit-0.6.3/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/docs/source/_templates/autosummary/module.rst` & `windkit-0.6.3/docs/source/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/docs/source/conf.py` & `windkit-0.6.3/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -305,8 +305,9 @@
         "https://docs-wasp.ramtt.xyz/pywasp/",
         ("../../../../docs/build/html/objects.inv", None),
     ),
     "rasterio": ("https://rasterio.readthedocs.io/en/latest/", None),
     "geopandas": ("https://geopandas.org/", None),
     "plotly": ("https://plotly.com/python-api-reference/", None),
     "pyproj": ("https://pyproj4.github.io/pyproj/stable/", None),
+    "pandas": ("https://pandas.pydata.org/docs/", None),
 }
```

### Comparing `windkit-0.6.2/docs/source/index.rst` & `windkit-0.6.3/docs/source/index.rst`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 WindKit
 =======
 
 WindKit provides a Pythonic interface to read, write, and analyse many of the file formats used in the WAsP wind resource assessment program. Over time the project will include additional file types, and work to standardize the structures that are used in Wind Resource Assessment.
 
 WindKit is built to include robust metadata for all objects, allowing for easier interoperability and reusability of different data sets.
 
-.. note:: WindKit does not provide an interface to calculate WAsP results. For that you will need PyWAsP, which will be launched later in 2022. PyWAsP will be a commercial tool, and require a license fee.
+.. note:: WindKit does not provide an interface to calculate WAsP results. For that you need PyWAsP, which can be purchased from the `WAsP Website <https://www.wasp.dk/products/pywasp>`_ .
 
 Tools Using WindKit
 -------------------
 
 - Wind-validation
 - New European Wind Atlas data APIs
 
@@ -21,14 +21,15 @@
 - Use the `WAsP Forum for Python Tools <https://www.wasptechnical.dk/forum/forum/19-wasp-python-tools/>`_.
 - Use our support email support at wasp.dk
 
 .. toctree::
     :caption: Setup
     :hidden:
 
+    getting_started
     installation
 
 .. toctree::
     :caption: Users Guide
     :hidden:
 
     windkit
```

### Comparing `windkit-0.6.2/docs/source/installation.rst` & `windkit-0.6.3/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/docs/source/io/io.rst` & `windkit-0.6.3/docs/source/io/io.rst`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/docs/source/plotting_user_guide.rst` & `windkit-0.6.3/docs/source/plotting_user_guide.rst`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/docs/source/topographic_data.rst` & `windkit-0.6.3/docs/source/topographic_data.rst`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/docs/source/wind_climate_objects.rst` & `windkit-0.6.3/docs/source/wind_climate_objects.rst`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/docs/source/windkit.rst` & `windkit-0.6.3/docs/source/windkit.rst`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/env/Dockerfile.ci` & `windkit-0.6.3/env/Dockerfile.ci`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/env/conda-linux-64.lock` & `windkit-0.6.3/env/conda-linux-64.lock`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 channels:
   - conda-forge
   - https://conda.windenergy.dtu.dk/channel/open
 dependencies:
   - python >=3.8
   # PyWAsP and WindKit
   - appdirs=1
-  - cf_xarray >=0.7
   - dtu_config
   - geopandas =0.11
   - lxml =4
   - matplotlib =3
   - netcdf4 =1.5
   - numpy =1.21.2
   - packaging =21.0
```

### Comparing `windkit-0.6.2/env/conda-osx-64.lock` & `windkit-0.6.3/env/conda-osx-64.lock`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/env/conda-win-64.lock` & `windkit-0.6.3/env/conda-win-64.lock`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/env/create_locks.py` & `windkit-0.6.3/env/create_locks.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/env/dev_env.yaml` & `windkit-0.6.3/env/dev_env.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 channels:
   - conda-forge
   - https://conda.windenergy.dtu.dk/channel/open
 dependencies:
   - python >=3.8
   # PyWAsP and WindKit
   - appdirs=1
-  - cf_xarray >=0.7
   - dtu_config
   - geopandas =0.11
   - lxml =4
   - matplotlib =3
   - netcdf4 =1.5
   - numpy =1.21.2
   - packaging =21.0
```

### Comparing `windkit-0.6.2/env/pywasp_env.yml` & `windkit-0.6.3/env/pywasp_env.yml`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/recipe/meta.yaml` & `windkit-0.6.3/.conda_env/dev_unix.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,44 @@
-{% set pkg_name = 'windkit' %}
-
-package:
-  name: {{ pkg_name }}
-  version: {{ environ.get('VERSION', '0.0.0') }}
-
-source:
-  path: ../
-
-build:
-  number: 0
-  script: pip install --no-deps .
-  skip: True # [py<38]
-  noarch: python
-
-requirements:
-  run:
-  - cf_xarray >=0.7
+name: base
+channels:
+  - conda-forge
+  - https://conda.windenergy.dtu.dk/channel/open
+dependencies:
   - dtu_config
   - geopandas =0.11
   - lxml =4
   - matplotlib =3
   - netcdf4 =1.5
-  - numpy =1.21
-  - packaging
+  - numpy =1.21.2
+  - packaging =21.0
   - pandas =1
   - plotly >=5.1.0
-  - pyproj >=3
+  - pyproj >=2.2.2
   - python >=3.8
   - python-kaleido >=0.2.1
   - rasterio =1
   - scipy =1
   - shapely =1
   - xarray >=2022
   - rioxarray >=0.12
-  host:
-    - python {{ python }}
-    - setuptools
-    - setuptools_scm
-test:
-  imports:
-    - {{ pkg_name }}
+  # Build dependencies all
+  - pip
+  - git
+  - setuptools
+  - setuptools_scm
+  # Developer dependencies
+  - conda-lock
+  - ipython
+  - jupyter
+  - jupyter-dash
+  - make
+  - nbsphinx
+  - nbsphinx-link
+  - pre-commit
+  - pytest
+  - pytest-cov
+  - recommonmark
+  - sphinx
+  - sphinx_rtd_theme
+  - sphinx-argparse
+  - sphinxcontrib-bibtex
+  - myst-parser
```

### Comparing `windkit-0.6.2/windkit/__init__.py` & `windkit-0.6.3/windkit/__init__.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/_errors.py` & `windkit-0.6.3/windkit/_errors.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/_rvea_xml.py` & `windkit-0.6.3/windkit/_rvea_xml.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/_validate.py` & `windkit-0.6.3/windkit/_validate.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/_vectormap_gml.py` & `windkit-0.6.3/windkit/_vectormap_gml.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/_vectormap_helpers.py` & `windkit-0.6.3/windkit/_vectormap_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 VECTORMAP_IDL_COL = "id_left"
 VECTORMAP_IDR_COL = "id_right"
 VECTORMAP_ID_COLS = (VECTORMAP_IDL_COL, VECTORMAP_IDR_COL)
 VECTORMAP_LMASKL_COL = "landmask_left"
 VECTORMAP_LMASKR_COL = "landmask_right"
 VECTORMAP_LMASK_COLS = (VECTORMAP_LMASKL_COL, VECTORMAP_LMASKR_COL)
 VECTORMAP_META_COLS = [VECTORMAP_ELEV_COL] + list(VECTORMAP_ROU_COLS)
+VECTORMAP_INLINE_LCTABLE_COLS = ("id", "d", "z0", "desc")
 _MAP_TYPE_CODES = {
     "elevation": 0,
     "roughness": 1,
     "speedup": 2,
     "turning": 3,
     "flow_inclination": 4,
     "turbulence_intensity": 5,
@@ -154,14 +155,20 @@
 
 def _is_elev(gdf):
     if VECTORMAP_ELEV_COL in gdf.columns:
         return True
     return False
 
 
+def _has_inline_lctable(gdf):
+    if all([i in gdf.columns for i in VECTORMAP_INLINE_LCTABLE_COLS]):
+        return True
+    return False
+
+
 def _get_map_type(gdf):  # pragma: no cover
     if _is_lc(gdf):
         return "landcover"
     elif _is_z0(gdf):
         return "roughness"
     elif _is_elev(gdf):
         return "elevation"
```

### Comparing `windkit-0.6.2/windkit/all_vars.json` & `windkit-0.6.3/windkit/all_vars.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9934640522875817%*

 * *Differences: {"'regulation_type'": "OrderedDict([('description', 'Regulation type used by the wind turbine.'), "*

 * *                      "('long_name', 'Regulation Type stall=1; pitch=2;'), ('units', '')])"}*

```diff
@@ -447,14 +447,19 @@
     },
     "rated_power": {
         "description": "Maximum amount of power by which the wind turbine can produce",
         "long_name": "Rated Power",
         "standard_name": "rated_power",
         "units": "W"
     },
+    "regulation_type": {
+        "description": "Regulation type used by the wind turbine.",
+        "long_name": "Regulation Type stall=1; pitch=2;",
+        "units": ""
+    },
     "rix": {
         "description": "One objective measure of the steepness or ruggedness of the terrain around a site is the so-called ruggedness index or RIX (Bowen and Mortensen, 1996), defined as the percentage fraction of the terrain within a certain distance from a specific site which is steeper than some critical slope, say 0.3 (Wood, 1995). ",
         "long_name": "Ruggedness Index",
         "units": "`1`"
     },
     "rms_temp_scale": {
         "cell_method": "time: conditional standard deviation (comment: sampled instantaneously from highest 50 percent of wind speed)",
```

### Comparing `windkit-0.6.2/windkit/binned_wind_climate.py` & `windkit-0.6.3/windkit/binned_wind_climate.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/cfd.py` & `windkit-0.6.3/windkit/cfd.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/data_structures.py` & `windkit-0.6.3/windkit/data_structures.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/elevation_map.py` & `windkit-0.6.3/windkit/elevation_map.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/empty.py` & `windkit-0.6.3/windkit/empty.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,46 +150,47 @@
     ustack_ds = spatial_unstack(ds)
 
     ds = update_var_attrs(_copy_chunks(output_locs, ustack_ds), _TOPO_EFFECTS_ATTRS)
 
     return update_history(ds)
 
 
-def empty_bwc(output_locs, nsec=12, not_empty=True, seed=9876538):
+def empty_bwc(output_locs, nsec=12, nbins=30, not_empty=True, seed=9876538):
     """
     Create empty binned wind climate dataset.
 
     If not_empty=True, the data variables are filled with meaninful random numbers,
     e.g. the sum of wdfreq is 1.
 
     Parameters
     ----------
     output_loc : xarray.Dataset
         Output geospatial information.
     nsec : int
         Number of sectors, defaults to 12.
+    nbins: int
+        Number of histogram bins, defaults to 30.
     not_empty : bool
         If true, the empty dataset is filled with random
         meaningful data.
     seed : int
         Seed for the random data, defaults to 9876538.
 
     Returns
     -------
     ds : xarray.Dataset
         Binned wind climate dataset either empty or filled with
         random numbers.
     """
 
-    nbins = 30
     da_dict, unstack_attrs = _define_std_arrays(output_locs, nsec)
     ds = xr.Dataset(
         {"wdfreq": da_dict["da_4d"], "wsfreq": da_dict["da_4d"]}, attrs=unstack_attrs
     )
-    wsbin_coords = create_ws_bin_coords(bin_width=1.0, nws=30)
+    wsbin_coords = create_ws_bin_coords(bin_width=1.0, nws=nbins)
 
     ds["wsfreq"] = ds["wsfreq"].expand_dims({"wsbin": wsbin_coords.values})
     ds = ds.assign_coords({**wsbin_coords.coords})
     n_pt = len(ds["point"])
 
     if not_empty:
         wsbin_n = np.linspace(1, nbins, nbins)
```

### Comparing `windkit-0.6.2/windkit/generalized_wind_climate.py` & `windkit-0.6.3/windkit/generalized_wind_climate.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/geospatial_imports.py` & `windkit-0.6.3/windkit/geospatial_imports.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/get_map.py` & `windkit-0.6.3/windkit/get_map.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/landcover.py` & `windkit-0.6.3/windkit/landcover.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/landcovertables/CGLS-LC100.json` & `windkit-0.6.3/windkit/landcovertables/CGLS-LC100.json`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/landcovertables/CORINE.json` & `windkit-0.6.3/windkit/landcovertables/CORINE.json`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/landcovertables/Globcover.json` & `windkit-0.6.3/windkit/landcovertables/Globcover.json`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/landcovertables/MODIS.json` & `windkit-0.6.3/windkit/landcovertables/MODIS.json`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/landcovertables/WorldCover.json` & `windkit-0.6.3/windkit/landcovertables/WorldCover.json`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/map_conversion/helper_functions.py` & `windkit-0.6.3/windkit/map_conversion/helper_functions.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/map_conversion/lines2poly.py` & `windkit-0.6.3/windkit/map_conversion/lines2poly.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/map_conversion/poly2lines.py` & `windkit-0.6.3/windkit/map_conversion/poly2lines.py`

 * *Files 2% similar despite different names*

```diff
@@ -506,14 +506,18 @@
         To define when the map is not entirely filled. It will be used when a
         line is defined by only one polygon.
     closed_map: bool or list of bool, optional. Default: False
         if close_map is True, all the lines will appear in the result. Otherwise
         the border lines will be removed. This parameter can be controlled border
         by border by providing a list of booleans (order: left, down, right, up).
     """
+    # Transform to polygon
+    if (np.array(poly_gdf.geom_type) == "MultiPolygon").any():
+        poly_gdf = poly_gdf.explode(index_parts=False)
+
     poly_map = PolygonMap(poly_gdf, background_lc_id=background_lc_id)
     line_map = poly_map.to_line_map(closed_map=closed_map)
     return line_map.line_gdf
 
 
 def sort_poly_gdf(gdf):
     """Return the dataframe "sorted".
```

### Comparing `windkit-0.6.2/windkit/map_file_header_to_epsg.json` & `windkit-0.6.3/windkit/map_file_header_to_epsg.json`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/metadata.py` & `windkit-0.6.3/windkit/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 """
 import inspect
 import json
 from datetime import datetime
 from logging import Logger
 from pathlib import Path
 
-import cf_xarray  # nopycln: import use as ds.cf
 import xarray as xr
 
 from ._version import version
 from .config import CONFIG
 from .data_structures import DataStructures
 from .spatial._struct import get_spatial_struct
 
@@ -419,15 +418,14 @@
 
     """
     _setup_user_global_attrs()
     CONFIG.create_config()
     var_dict_copy = var_dict.copy()
     object_type = var_dict_copy.pop("object_type", None)
     if isinstance(obj, xr.Dataset):
-        obj = obj.cf.add_canonical_attributes()
         for var in obj.data_vars:
             obj[var] = _update_local_attrs(obj[var], var_dict)
         obj.attrs["Conventions"] = "CF-1.8"
         obj.attrs["Package name"] = __name__.split(".")[0]
         obj.attrs["Package version"] = version
         obj.attrs["Creation date"] = (
             datetime.utcnow().replace(microsecond=0).isoformat()
@@ -435,15 +433,14 @@
         if object_type is not None:
             obj.attrs["Object type"] = object_type
         obj.attrs["author"] = CONFIG.get_option("user_data", "name")
         obj.attrs["author_email"] = CONFIG.get_option("user_data", "email")
         obj.attrs["institution"] = CONFIG.get_option("user_data", "institution")
 
     elif isinstance(obj, xr.DataArray):
-        obj = obj.cf.add_canonical_attributes()
         obj = _update_local_attrs(obj, var_dict)
     else:
         raise ValueError(
             "Can only add attributes to xarray.Dataset or xarray.DataArray objects."
         )
 
     return obj
@@ -464,15 +461,23 @@
     -------
     xarray.Dataset
         The same Dataset with updated attribute.
 
     """
     current_utc = datetime.utcnow().replace(microsecond=0).isoformat()
     package = __name__.split(".")[0]
-    function_call = inspect.stack()[2].code_context[0][:-1]
+
+    # Get the function call that was used before calling update_history.
+    # NOTE: If call is from the python interpreter, we can't determine the context, so
+    #       include a generic message.
+    function_context = inspect.stack()[2].code_context
+    if function_context is None:
+        function_call = "Unknown python interpreter command."
+    else:
+        function_call = function_context[0][:-1]
 
     if "=" in function_call:
         function_call = function_call[function_call.index("=") + 1 :]
         if " " in function_call:
             function_call = function_call[function_call.index(" ") + 1 :]
     history_to_add = (
         current_utc + ":" + "\t" + package + "==" + version + "\t" + function_call
```

### Comparing `windkit-0.6.2/windkit/plot/__init__.py` & `windkit-0.6.3/windkit/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/plot/_colormaps.py` & `windkit-0.6.3/windkit/plot/_colormaps.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/plot/_helpers.py` & `windkit-0.6.3/windkit/plot/_helpers.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/plot/color.py` & `windkit-0.6.3/windkit/plot/color.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/plot/histogram.py` & `windkit-0.6.3/windkit/plot/histogram.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/plot/landcover_map.py` & `windkit-0.6.3/windkit/plot/landcover_map.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/plot/operational_curves.py` & `windkit-0.6.3/windkit/plot/operational_curves.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/plot/raster_plot.py` & `windkit-0.6.3/windkit/plot/raster_plot.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/plot/roughness_rose.py` & `windkit-0.6.3/windkit/plot/roughness_rose.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/plot/vertical_profile.py` & `windkit-0.6.3/windkit/plot/vertical_profile.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/plot/wind_rose.py` & `windkit-0.6.3/windkit/plot/wind_rose.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/plot/wind_turbine.py` & `windkit-0.6.3/windkit/plot/wind_turbine.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/raster_map.py` & `windkit-0.6.3/windkit/raster_map.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/roughness_map.py` & `windkit-0.6.3/windkit/roughness_map.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/sector.py` & `windkit-0.6.3/windkit/sector.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,23 +13,30 @@
 
     Create a data array with the wind speed bins, ceiling and floor.
 
     Parameters
     ----------
     bin_width : float
         Wind speed bin width, defaults to 1.0
-    nws : float
+    nws : int
         Number of wind speed bins, defaults to 40.
 
     Returns
     -------
     cen_da : xarray.DataArray
         Data array with wind speed bins.
     """
 
+    if type(nws) is not int:
+        raise TypeError("'nws' argument must be integer")
+    if bin_width <= 0.0:
+        raise ValueError("'bin_width' argument must be positive")
+    if nws <= 0:
+        raise ValueError("'nws' argument must be positive")
+
     cen_vals = np.linspace(bin_width / 2, float(nws) * bin_width - bin_width / 2, nws)
     # Create data arrays of sector valuse
     cen_da = xr.DataArray(cen_vals, dims="wsbin")
     ceil_da = xr.DataArray(cen_vals + 0.5 * bin_width, dims="wsbin")
     floor_da = xr.DataArray(cen_vals - 0.5 * bin_width, dims="wsbin")
 
     cen_da = cen_da.assign_coords(
@@ -52,22 +59,32 @@
 def create_ws_bin_coords_from_values(wsbins):
     """Create wind speed bins coordinates from an array of bins.
 
     Create a data array with the wind speed bins, ceiling and floor.
 
     Parameters
     ----------
-    wsbins : numpy.ndarray
-        Array with wind speed bins.
+    wsbins : numpy.ndarray or array_like
+        1D array with wind speed bins.
     Returns
     -------
     cen_da : xarray.DataArray
         Data array with wind speed bins.
     """
 
+    try:
+        wsbins = np.asfarray(wsbins)
+    except:
+        raise TypeError(
+            "'wsbins' is not a numpy.ndarray or array_like of wind speed bins"
+        )
+
+    if wsbins.ndim != 1:
+        raise ValueError("'wsbins' has to be a 1D numpy.ndarray or array_like")
+
     cen_vals = 0.5 * (wsbins[:-1] + wsbins[1:])
     # Create data arrays of sector valuse
     cen_da = xr.DataArray(cen_vals, dims="wsbin")
     ceil_da = xr.DataArray(wsbins[1:], dims="wsbin")
     floor_da = xr.DataArray(wsbins[:-1], dims="wsbin")
 
     cen_da = cen_da.assign_coords(
@@ -96,14 +113,19 @@
         Number of sectors to create
 
     Returns
     -------
     cen_da : xarray.DataArray
         Data array with sector coordinates, ceiling and floor.
     """
+    if type(nsec) not in [np.int32, np.int64, int]:
+        raise TypeError("'nsec' must be of integer type")
+    if nsec <= 0:
+        raise ValueError("'nsec' must be a positive integer")
+
     sec_width = 360 / nsec
     cen_vals = np.linspace(0.0, 360.0 - sec_width, nsec)
 
     # Create data arrays of sector valuse
     cen_da = xr.DataArray(cen_vals, dims="sector")
     ceil_da = xr.DataArray((cen_vals + 0.5 * sec_width) % 360, dims="sector")
     floor_da = xr.DataArray((cen_vals - 0.5 * sec_width) % 360, dims="sector")
```

### Comparing `windkit-0.6.2/windkit/spatial/README.md` & `windkit-0.6.3/windkit/spatial/README.md`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/spatial/__init__.py` & `windkit-0.6.3/windkit/spatial/__init__.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/spatial/_crs.py` & `windkit-0.6.3/windkit/spatial/_crs.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/spatial/_cuboid.py` & `windkit-0.6.3/windkit/spatial/_cuboid.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/spatial/_dimensions.py` & `windkit-0.6.3/windkit/spatial/_dimensions.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/spatial/_interpolation.py` & `windkit-0.6.3/windkit/spatial/_interpolation.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/spatial/_latitude.py` & `windkit-0.6.3/windkit/spatial/_latitude.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/spatial/_point.py` & `windkit-0.6.3/windkit/spatial/_point.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/spatial/_raster.py` & `windkit-0.6.3/windkit/spatial/_raster.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/spatial/_struct.py` & `windkit-0.6.3/windkit/spatial/_struct.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/spatial/_utm.py` & `windkit-0.6.3/windkit/spatial/_utm.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/spatial/_vector.py` & `windkit-0.6.3/windkit/spatial/_vector.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/spatial/decorators.py` & `windkit-0.6.3/windkit/spatial/decorators.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/spatial/spatial.py` & `windkit-0.6.3/windkit/spatial/spatial.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/time_series_wind_climate.py` & `windkit-0.6.3/windkit/time_series_wind_climate.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,27 +157,29 @@
         west east locaton of the measurement
     south_north: float
         south north location of the measurement
     crs : int, dict, str or pyproj.crs.CRS
         Value to initialize `pyproj.crs.CRS`
     time_col: int, str
         column position (integer) or header (str) where the timestamp is located. it can be overriden by
-        using `pandas.read_csv` **kwargs. Defaults to 0 (first column in the file).
+        using `pandas.read_csv` \**kwargs. Defaults to 0 (first column in the file).
     height_to_columns: dict
         dictionary to map the wind speed and directions to its corresponding height. The key is a float
         with the height, and the value is a tuple (str,str) with the header for the wind speed and the
         header for the wind direction, respectively. If the parameter is `None`, the columns are inferred
         from the column names in the files. The function will find wind speeds for different heights and
         after that will look for wind direction columns, matching them to the closest height.
         Examples of autodetected header formats:
-        - ws_10, ws_10_mean, ws10, WS10 (wind speed at 10 m)
-        - windagl10, windagl_10, windagl_10_mean (wind speed at 10 m)
-        - wd_15, wd_15_mean, w15, WD15 (wind direction at 15m)
-        - wdiragl15, wdiragl_15, wdiragl_15_mean (wind direction at 15 m)
-    **kwargs: dict
+
+            - ws_10, ws_10_mean, ws10, WS10 (wind speed at 10 m)
+            - windagl10, windagl_10, windagl_10_mean (wind speed at 10 m)
+            - wd_15, wd_15_mean, w15, WD15 (wind direction at 15m)
+            - wdiragl15, wdiragl_15, wdiragl_15_mean (wind direction at 15 m)
+
+    ``**kwargs``: dict
         Optional arguments that are forwarded to `pandas.read_csv` for customizing its behavior.
 
     Returns
     -------
     da: xarray.Dataset
         Time series wind climate dataset  with variables 'wind_speed' and 'wind_direction'
         and with a coordinate and dimension 'time'.
@@ -228,17 +230,21 @@
     height_to_columns: dict
         dictionary to map the wind speed and directions to its corresponding height. The key is a float
         with the height, and the value is a tuple (str,str) with the header for the wind speed and the
         header for the wind direction, respectively. If the parameter is `None`, the columns are inferred
         from the column names in the dataframe. The function will find wind speeds for different heights
         and after that will look for wind direction columns, matching them to the closest height.
         Examples of autodetected header formats:
+
            - ws_10, ws_10_mean, ws10, WS10 (wind speed at 10 m)
+
            - windagl10, windagl_10, windagl_10_mean (wind speed at 10 m)
+
            - wd_15, wd_15_mean, w15, WD15 (wind direction at 15m)
+
            - wdiragl15, wdiragl_15, wdiragl_15_mean (wind direction at 15 m)
 
     Returns
     -------
     da: xarray.Dataset
         Time series wind climate dataset with variables 'wind_speed' and 'wind_direction'
         and with a coordinate and dimension 'time'.
```

### Comparing `windkit-0.6.2/windkit/vector_map.py` & `windkit-0.6.3/windkit/vector_map.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,33 +10,36 @@
 from and written to several different formats to support interoperability with different
 tools. We recommend using the Geopackage (.gpkg) format if you do not need to use one of
 the other formats. For interoperability with WAsP, you should use the .map format for
 elevation maps, and .gml for land-cover maps.
 """
 import argparse
 import logging
+import warnings
 from collections import defaultdict
 from inspect import cleandoc
 from pathlib import Path
 from typing import Union
 
 import numpy as np
 import pyproj
 from shapely.geometry import LineString, Polygon
 
 from ._vectormap_gml import read_vector_map_gml, write_vectormap_gml
 from ._vectormap_helpers import *
 from ._vectormap_helpers import (
     _MAP_TYPE_CODES,
+    _has_inline_lctable,
     _is_elev,
     _is_lc,
     _read_map_file_header_to_epsg_table,
     _z0_to_landcover,
 )
 from .landcover import LandCoverTable
+from .map_conversion.poly2lines import poly2lines
 from .spatial import BBox
 
 logger = logging.getLogger("__name__")
 
 __all__ = [
     "_MAP_TYPE_CODES",
     "read_vector_map",
@@ -214,26 +217,32 @@
             columns={
                 VECTORMAP_ROUL_COL: VECTORMAP_LMASKL_COL,
                 VECTORMAP_ROUR_COL: VECTORMAP_LMASKR_COL,
             }
         )
 
 
-def read_vector_map(filename, crs=None, map_type=None):
+def read_vector_map(filename, crs=None, map_type=None, background_lc_id=None):
     """
     Read a vector_map from a file.
 
     Parameters
     ----------
     filename : str or pathlib.Path
         File path
     crs : int, dict, str or pyproj.crs.CRS
         Value to initialize `pyproj.crs.CRS` Default reads from file.
     map_type : str
-        One of "elevation" or "roughness" to specify the type of map to create. Defaults to None.
+        One of "elevation" or "roughness" to specify the type of map to create.
+        Defaults to None.
+    background_lc_id: int, optional.
+        This option is used for polygon based landcover files. It sets the landcover id
+        for all areas not covered by a polygon. The default is None, but if your area
+        includes such areas, you should set it to an ID that is part of your landcover
+        table.
 
     Returns
     -------
     gdf: geopandas.GeoDataFrame
         Vectormap as a geodataframe.
     lc : LandCoverTable
         LandCoverTable optional.
@@ -261,30 +270,57 @@
         columns={v: VECTORMAP_ELEV_COL for v in VECTORMAP_ALT_ELEV_COL}
     )
 
     if crs is not None:
         if pyproj.CRS.from_user_input(gdf.crs) != pyproj.CRS.from_user_input(crs):
             raise ValueError(f"Dataset crs {gdf.crs} doesn't match crs argument {crs}.")
 
-    if _is_lc(gdf):
+    #########################################
+    # Convert polygons to lines if necessary
+    #########################################
+    if (np.array(gdf.geom_type) == "MultiPolygon").any() or (
+        np.array(gdf.geom_type) == "Polygon"
+    ).any():
+        if background_lc_id is None:
+            background_lc_id = -999
+        gdf = poly2lines(gdf, background_lc_id)
+
+    ###############################################
+    # Get landcover table from file if it is there
+    ###############################################
+    if _is_lc(gdf):  # Requires separate landcover table, either from gpkg or json
         if filetype == ".gpkg":
             try:
+                lcdf = gpd.read_file(filename, layer="landcover_table")
+                if "index" in lcdf.columns:
+                    lcdf = lcdf.rename(columns={"index": "id"})
+                    warnings.warn(
+                        "The use of the name 'index' to identify landcover ID's in the landcover table is deprecated, please use the name 'id' for this instead.",
+                        FutureWarning,
+                    )
+                lcdf = lcdf.set_index("id")
                 lctable = LandCoverTable(
-                    gpd.read_file(filename, layer="landcover_table")
-                    .set_index("index")
-                    .drop("geometry", axis=1)
-                    .transpose()
-                    .to_dict()
+                    lcdf.drop("geometry", axis=1).transpose().to_dict()
                 )
             except ValueError:
-                return gdf
+                return gdf  # CHECK: should this return an lctable of None?
         else:
             lctable = LandCoverTable.read_json(f"{filebase}.json")
+
         return (gdf, lctable)
 
+    if _has_inline_lctable(gdf):  # Landcover info is from each row of table
+        lctable = LandCoverTable(
+            gdf[["id", "d", "z0", "desc"]]
+            .drop_duplicates()
+            .set_index("id")
+            .to_dict(orient="index")
+        )
+        return gdf, lctable
+
     return gdf
 
 
 def vector_map_to_mapfile(gdf, filename, lctable=None, header="WindKit", mode="w"):
     """
     Write vector_map in GeoDataFrame format to WAsP mapfile format.
```

### Comparing `windkit-0.6.2/windkit/weibull.py` & `windkit-0.6.3/windkit/weibull.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/weibull_wind_climate.py` & `windkit-0.6.3/windkit/weibull_wind_climate.py`

 * *Files 16% similar despite different names*

```diff
@@ -309,14 +309,30 @@
     ds = ds.assign_coords(create_sector_coords(ds.sector.size).coords)
     ds = ds.expand_dims(spatial_dataset.dims)
     ds = ds.assign_coords(spatial_dataset.coords)
     wwc = update_var_attrs(ds, _WEIB_ATTRS)
     return update_history(wwc)
 
 
+def _can_be_int(x):
+    """Check if x can be converted to int."""
+    try:
+        int(x)
+        return True
+    except ValueError:
+        return False
+
+
+def _convert_to_int_or_fixed_decimals(x, decimals=1):
+    if _can_be_int(x):
+        return int(x)
+    else:
+        return np.round(x, decimals=decimals)
+
+
 def _wrg_header(wwc):
     """Write WWC grid dimensions to WRG header with the format:
           nx ny xmin ymin cell_size
 
     Parameters
     ----------
     wwc : xarray.Dataset
@@ -325,36 +341,143 @@
     Returns
     -------
     str
         WRG header.
 
     """
     nx, ny = _raster._shape(wwc)
-    xmin = wwc.west_east.values.min()
-    ymin = wwc.south_north.values.min()
-    size = _raster._spacing(wwc)
-    return f"{nx:>8}{ny:>8}{xmin:>18}{ymin:>18}{size:>15}"
+    xmin = _convert_to_int_or_fixed_decimals(wwc.west_east.values.min(), decimals=1)
+    ymin = _convert_to_int_or_fixed_decimals(wwc.south_north.values.min(), decimals=1)
+    size = _convert_to_int_or_fixed_decimals(_raster._spacing(wwc), decimals=1)
+    return f" {nx:<13} {ny:<13} {xmin:>9} {ymin:>13} {size:>8}"
+
+
+def _get_rsf_formatters(nsec=12, use_production=False, formatters=None):
+    """Returns a list of functions to format the data in the RSF/WRG file.
+
+    Parameters
+    ----------
+    nsec : int
+        Number of sectors.
+
+    use_production : bool
+        If true, the gross_aep variable will be used instead of power_density.
+
+    formatters : dict
+        Dictionary with the variable names as keys and the functions to format
+        the data as values.
+
+    Returns
+    -------
+    list
+        List of functions to format the data in the RSF/WRG file.
+    """
+
+    fixed_columns = [
+        "name",
+        "west_east",
+        "south_north",
+        "elevation",
+        "height",
+        "A_combined",
+        "k_combined",
+        "gross_aep" if use_production else "power_density",
+        "nsec",
+    ]
+
+    _formatters_default = {
+        "name": lambda x: f"{x:<10}",
+        "west_east": lambda x: f"{x:>9.1f}",
+        "south_north": lambda x: f"{x:>9.1f}",
+        "elevation": lambda x: f"{x:>7.0f}",
+        "height": lambda x: f"{x:>4.1f}",
+        "A_combined": lambda x: f"{x:>4.2f}",
+        "k_combined": lambda x: f"{x:>5.3f}",
+        "power_density": lambda x: f"{x:>14.4f}",
+        "gross_aep": lambda x: f"{x:>14.0f}",
+        "nsec": lambda x: f"{x:>2}",
+        "A": lambda x: f"{x:>3.0f}",
+        "k": lambda x: f"{x:>4.0f}",
+        "wdfreq": lambda x: f"{x:>3.0f}",
+    }
+    if formatters is None:
+        formatters = _formatters_default
+    else:
+        formatters = {**_formatters_default, **formatters}
+
+    formatters_list = []
+    for col in fixed_columns:
+        formatters_list.append(formatters[col])
+
+    for isec in range(nsec):
+        formatters_list.append(formatters["wdfreq"])
+        formatters_list.append(formatters["A"])
+        formatters_list.append(formatters["k"])
+
+    return formatters_list
 
 
 @wwc_validate_wrapper
-def _to_resource_file(wwc, rsffile, wrg_header=False):
+def _to_resource_file(
+    wwc,
+    rsffile,
+    wrg_header=False,
+    use_production=False,
+    formatters=None,
+):
     """Write weibull wind climate dataset to a resource file (.rsf or .wrg).
 
     Parameters
     ----------
     wwc : xarray.Dataset
         Weibull wind climate xarray dataset.
 
     rsffile : str
         Path to resource file
 
     wrg_header : bool
         If True, the WRG header will be added to the file.
         Requires a cuboid dataset.
 
+    use_production : bool
+        If true, the "gross_aep" variable will be used instead of "power_density".
+
+    formatters : dict
+        Dictionary with the variable names as keys and the functions to format
+        the data as values.
+
+        For each variable the expected widths in the formatter are:
+            name: 10
+            west_east: 9
+            south_north: 9
+            elevation: 7
+            height: 4
+            A_combined: 4
+            k_combined: 5
+            power_density: 14
+            gross_aep: 14
+            nsec: 2
+            A: 3
+            k: 4
+            wdfreq: 3
+
+        A space is added after each variable. Meaning the effective
+        width of the string representation of the variable is the
+        width in the formatter plus one (except for the first variable)
+
+        A formatter can look like:
+            formatters  = {
+                "west_east": lambda x: f"{x:<9.2f}",
+            }
+
+        In this case the width of the string representation of the
+        west_east variable will be 10 (9+1). And the number of decimals
+        will be 2 instead of the default 1. If a int representation
+        is desired, "{x:<9.0f}" can be used.
+
     """
 
     # Check if wwc has unsupported dimensions
     approved_dims = [
         "sector",
         "point",
         "stacked_point",
@@ -364,14 +487,25 @@
     ]
     if any([dim not in approved_dims for dim in wwc.dims]):
         raise ValueError(
             f"Unsupported dimensions in wwc: {wwc.dims}. "
             f"Supported dimensions: {approved_dims}"
         )
 
+    if use_production and "gross_aep" not in wwc.data_vars:
+        raise ValueError(
+            "The gross_aep variable is required to write a resource file with "
+            "use_production=True."
+        )
+
+    if use_production:
+        var_power = "gross_aep"
+    else:
+        var_power = "power_density"
+
     wwc_cp = wwc.copy()
 
     if wrg_header:
         if not is_cuboid(wwc):
             raise ValueError("WWC must be a 'cuboid' to add WRG header!")
         header = _wrg_header(wwc)
 
@@ -391,35 +525,41 @@
 
     # remove unneeded vars
     wwc_cp = wwc_cp.drop_vars(
         ["sector", "sector_ceil", "sector_floor", "crs"], errors="ignore"
     )
 
     nsec = wwc_cp.dims["sector"]
-    wwc_cp["A"] = (wwc_cp["A"] * 10.0).astype(np.int16)
-    wwc_cp["k"] = (wwc_cp["k"] * 100.0).astype(np.int16)
-    wwc_cp["wdfreq"] = (wwc_cp["wdfreq"] * 1000.0).astype(np.int16)
+
+    # round values in the order that fits best with WAsP values
+    wwc_cp["A"] = wwc_cp["A"].round(decimals=1) * 10.0
+    wwc_cp["k"] = wwc_cp["k"].round(decimals=2) * 100.0
+    wwc_cp["wdfreq"] = wwc_cp["wdfreq"].round(decimals=3) * 1000.0
+
     wwc_cp["site_elev"] = wwc_cp["site_elev"].astype(np.int16)
     wwc_cp["nsec"] = xr.full_like(wwc_cp["site_elev"], nsec, dtype=np.int16)
 
+    if use_production:
+        wwc_cp["gross_aep"] = wwc_cp["gross_aep"] * 1e9  # GWh/y -> Wh/y
+
     # select variables that do not depend on wind direction sector
     vars = [
         "name",
         "west_east",
         "south_north",
         "site_elev",
         "height",
         "A_combined",
         "k_combined",
-        "power_density",
+        var_power,
         "nsec",
     ]
 
     df = wwc_cp[
-        ["site_elev", "A_combined", "k_combined", "power_density", "nsec"]
+        ["site_elev", "A_combined", "k_combined", var_power, "nsec"]
     ].to_dataframe()
 
     if "name" not in df.columns:
         df["name"] = "GridPoint"  # insert text column at first position
 
     # select variables that depend on wind direction sector
     sec_vars = [str((var, sec)) for sec in range(nsec) for var in ["wdfreq", "A", "k"]]
@@ -434,76 +574,112 @@
         .reset_index()
         .drop(["point", "stacked_point"], axis=1, errors="ignore")
     )  # concat combined and sectorwise values
     # transform all column names to string to make it compatible with pandas 1.4
     df_total.columns = [str(x) for x in df_total.columns]
     df_total = df_total[vars + sec_vars]  # select vars in correct order
 
-    widths_offset = tuple([9, 9, 9, 7, 4, 4, 5, 14, 2] + [3, 3, 4] * nsec)
+    formatters_list = _get_rsf_formatters(
+        nsec=nsec, use_production=use_production, formatters=formatters
+    )
 
-    formatters = [
-        lambda x: f"{x:>9}",  # name
-        lambda x: f"{x:>9.1f}",  # west_east
-        lambda x: f"{x:>9.1f}",  # south_north
-        lambda x: f"{x:>7.0f}",  # elevation
-        lambda x: f"{x:>4.1f}",  # height
-        lambda x: f"{x:>4.2f}",  # A_combined
-        lambda x: f"{x:>5.3f}",  # k_combined
-        lambda x: f"{x:>14.0f}",  # power_density
-        lambda x: f"{x:>2}",  # nsec
-    ]
-
-    for isec in range(nsec):
-        formatters.extend(
-            [
-                lambda x: f"{x:>3}",  # wdfreq
-                lambda x: f"{x:>3}",  # A
-                lambda x: f"{x:>4}",  # k
-            ]
-        )
+    # When all values are missing for power/aep, i.e. valued as -9999,
+    # the value needs to be written as an integer
+    if all(df_total[var_power] == -9999):
+        formatters_list[7] = lambda x: f"{x:>14.0f}"
+
+    # When heights are > 100m, the height needs to be written as an integer
+    if df_total["height"].max() > 100.0:
+        formatters_list[4] = lambda x: f"{x:>4.0f}"
 
     str_list = df_total.to_string(
         header=False,
         index=False,
         index_names=False,
-        col_space=widths_offset,
-        formatters=formatters,
-        justify="left",
+        formatters=formatters_list,
     )
 
+    def _is_char_21_blank(s):
+        """Check that character 21 is blank."""
+        if s[20] != " ":
+            return False
+        else:
+            return True
+
+    def _remove_initial_blank_space(s):
+        """Remove initial blank space from each line of the string to be written.
+        This is required for the .rsf/.wrg format to get the correct widths written to file.
+        """
+        sout = ""
+        for line in s.split("\n"):
+            sout += line[1:] + "\n"
+        return sout
+
+    def _check_row_widths(s, nsec=12):
+        """Check that the row widths are correct for the number of sectors."""
+        width_expected = 72 + nsec * 13
+        for line in s.split("\n")[:-1]:
+            width = len(line)
+            if width != width_expected:
+                raise ValueError(
+                    f".rsf/.wrg row width is {width} Expected {width_expected} for {nsec} sectors!\nare the formatters correct?"
+                )
+
+    def _check_ncols(s, nsec=12):
+        """Check that the number of columns is correct read back in for the number of sectors."""
+        ncols_expected = 9 + nsec * 3
+        df = pd.read_fwf(
+            io.StringIO(s),
+            widths=tuple([10, 10, 10, 8, 5, 5, 6, 15, 3] + [4, 4, 5] * nsec),
+            header=None,
+        )
+        ncols = df.shape[1]
+        if ncols != ncols_expected:
+            raise ValueError(
+                f".rsf/.wrg has {ncols} columns. Expected {ncols_expected} for {nsec} sectors!"
+            )
+
+    # check that character 21 is blank and remove initial blank space if not
+    # This problem is related to the pandas version (or a dependency of pandas)
+    if not _is_char_21_blank(str_list):
+        str_list = _remove_initial_blank_space(str_list)
+
+    _check_row_widths(str_list, nsec=nsec)
+    _check_ncols(str_list, nsec=nsec)
+
     with open(rsffile, "w", newline="\r\n") as text_file:
         if wrg_header:
             text_file.write(header + "\n")
         text_file.write(str_list)
 
 
-def to_rsffile(wwc, rsffile, wrg_header=False):
+def to_rsffile(wwc, rsffile, wrg_header=False, formatters=None):
     """Write weibull wind climate dataset to .rsf file.
 
     Parameters
     ----------
     wwc : xarray.Dataset
         Weibull wind climate xarray dataset.
     rsffile: str
         Path to .rsf file
     """
-    return _to_resource_file(wwc, rsffile, wrg_header=wrg_header)
+    return _to_resource_file(wwc, rsffile, wrg_header=wrg_header, formatters=formatters)
 
 
-def to_wrgfile(wwc, wrgfile):
+def to_wrgfile(wwc, wrgfile, formatters=None):
     """Write weibull wind climate dataset to .wrg file.
 
     Parameters
     ----------
     wwc : xarray.Dataset
         Weibull wind climate xarray dataset.
     wrgfile: str
         Path to .wrg file
     """
-    return _to_resource_file(wwc, wrgfile, wrg_header=True)
+    return _to_resource_file(wwc, wrgfile, wrg_header=True, formatters=formatters)
 
 
 def read_grdfile(grdfiles, regex_pattern=None, regex_var_order=None):
     """Reads a .grd file into a weibull wind climate dataset.
 
     Parameters
     ----------
```

### Comparing `windkit-0.6.2/windkit/wind.py` & `windkit-0.6.3/windkit/wind.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/wind_climate.py` & `windkit-0.6.3/windkit/wind_climate.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit/wind_turbine.py` & `windkit-0.6.3/windkit/wind_turbine.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,25 +6,83 @@
 Created on Wed Sep  6 14:30:28 2017
 
 @author: jufen
 
 UPDATE 8 July 2021 by @btol: added xarray.dataset wind turbine structure
 """
 import xml.etree.ElementTree as ET
+from enum import Enum
 from functools import cached_property
 from pathlib import Path
 
 import numpy as np
 import xarray as xr
 
+from ._validate import create_validator
+from .metadata import ALL_VARS_META, update_var_attrs
 from .plot.wind_turbine import plot_wind_turbine_locations
 from .spatial import BBox, get_crs
 
 
-def _read_windpro_wtg_element(wt_element):
+class RegulationType(Enum):
+    UNDEFINED = 0
+    STALL = 1
+    PITCH = 2
+
+
+DATA_VAR_DICT_WTG = {
+    "power_output": ["mode", "wind_speed"],
+    "thrust_coefficient": ["mode", "wind_speed"],
+    "air_density": ["mode"],
+    "stationary_thrust_coefficient": ["mode"],
+    "wind_speed_cutin": ["mode"],
+    "wind_speed_cutout": ["mode"],
+    "rated_power": ["mode"],
+    "name": [],
+    "rotor_diameter": [],
+    "hub_height": [],
+    "regulation_type": [],
+}
+
+REQ_DIMS_WTG = ["mode", "wind_speed"]
+
+REQ_COORDS_WTG = [
+    "wind_speed",
+    "mode",
+]
+
+wtg_validate, wtg_validate_wrapper = create_validator(
+    DATA_VAR_DICT_WTG, REQ_DIMS_WTG, REQ_COORDS_WTG
+)
+
+
+def estimate_regulation_type(wtg: xr.Dataset):
+    """Estimate the regulation type of a WTG
+
+    Use the power_output array, to see how many points equal the max power output. This
+    does a good job detecting manufacturers power curves, but doesn't detect pitch
+    regulation from power curves derived from measurements.
+
+    Parameters
+    ----------
+    wtg : xr.Dataset
+        Wind Turbine Generator object
+
+    Returns
+    -------
+    RegulationType
+        Estimated regulation type object
+    """
+    if (wtg.power_output == wtg.power_output.max()).sum() >= 3:
+        return RegulationType.PITCH
+    else:
+        return RegulationType.STALL
+
+
+def _read_windpro_wtg_element(wt_element):  # pragma: no cover not implemented yet
     """Parse the ET element from WindPRO to initilize an WT_cls object.
 
     Parameters
     ----------
     WT_element : ET element
         Extracted from .xml file in the .optireq file from WindPRO.
 
@@ -111,15 +169,15 @@
             "air_density": (("mode",), air_dens),
         },
     )
 
     return wtg
 
 
-def _read_windpro_wtg(wtg_file):
+def _read_windpro_wtg(wtg_file):  # pragma: no cover not implemented yet
     """Read a windpro-formatted XML ".wtg" file.
 
     Parameters
     ----------
     wtg_file : string, pathlib.Path
         A string or pathlib.Path denoting the location of the .wtg file
 
@@ -315,18 +373,26 @@
     merged = xr.concat(datasets, dim="mode")
     merged["name"] = wtg_element.attrib["Description"]
     merged["rotor_diameter"] = np.float64(wtg_element.attrib["RotorDiameter"])
     merged["hub_height"] = np.float64(
         wtg_element.find("SuggestedHeights").find("Height").text
     )
 
+    root_attrs = wtg_element.attrib
+    if root_attrs["FormatVersion"] >= "1.02":
+        merged["regulation_type"] = RegulationType[
+            root_attrs["ControlSystem"].upper()
+        ].value
+    else:
+        merged["regulation_type"] = RegulationType.UNDEFINED.value
+
     return merged
 
 
-def _read_wasp_wt_element(wt_element):
+def _read_wasp_wt_element(wt_element):  # pragma no cover Not used anywhere
     """Convert a wasp-formatted XML element to a WindKit wtg xr.Dataset.
 
     Parameters
     ----------
     wt_element : ET WT element
         Extracted from .xml object in the .wwh file.
 
@@ -356,28 +422,29 @@
     """
     tree = ET.parse(wtg_file)
     root = tree.getroot()
 
     return _read_wasp_wtg_element(root)
 
 
-def read_wtg(wtg_file, file_format="wasp"):
+def read_wtg(wtg_file, file_format="wasp", regulation_type="pitch"):
     """Read in Wind Turbine Generator (WTG) data from a file.
 
     A WTG dataset contains the following:
 
     coordinates(dim):
         wind_speed(wind_speed) : wind speed
         mode(mode)             : each mode reprents different ct/power curves
-        air_density(mode)      : Air density of mode
 
     variables(dims):
         name                                  : name of the WTG
         rotor_diameter                        : rotor diameter in meters
         hub_height                            : hub height a.g.l. in meters
+        regulation_type                       : Regulation type (1: stall, 2: pitch)
+        air_density(mode)                     : Air density power curve table
         wind_speed_cutin(mode)                : Wind speed cutin
         wind_speed_cutout(mode)               : Wind speed cutout
         rated_power(mode)                     : Rated power
         power_output(mode, wind_speed)        : Power output
         thrust_coefficient(mode, wind_speed)  : Thrust coefficient
 
     Parameters
@@ -385,32 +452,51 @@
     wtg_file : str, pathlib.Path
         WTG file to read
 
     file_format : str
         XML file format to use. Only "wasp" formatting is
         supported currently.
 
+    regulation_type : str or None
+        One of "stall", "pitch" or None. If None, uses estimate_regulation_type to
+        determine the regulation type. (Default: "pitch")
+
     Returns
     -------
     xr.Dataset
         WTG dataset
-
     """
     wtg_file = Path(wtg_file)
     ext = wtg_file.suffix
     if ext == ".wtg":
         if file_format == "wasp":
-            return _read_wasp_wtg(wtg_file)
+            wtg_ds = _read_wasp_wtg(wtg_file)
         # elif file_format == "windpro":
-        #     return _read_windpro_wtg(wtg_file)
+        #     wtg_ds = _read_windpro_wtg(wtg_file)
     else:
         raise ValueError(
             f"File extension: {ext} not recognized as wind turbine generator!"
         )
 
+    # Update regulation type
+    # If undefined from the file and argument is None then estimate, else use argument
+    if ("regulation_type" not in wtg_ds.data_vars) or (
+        RegulationType(wtg_ds.regulation_type) == RegulationType.UNDEFINED
+    ):
+        if regulation_type is None:
+            wtg_ds["regulation_type"] = estimate_regulation_type(wtg_ds).value
+        else:
+            wtg_ds["regulation_type"] = RegulationType[regulation_type.upper()].value
+
+    # Validate
+    wtg_validate(wtg_ds)
+
+    # Add metadata
+    return update_var_attrs(wtg_ds, ALL_VARS_META)
+
 
 def wtg_power(wtg, ws=None, *, interp_method="linear", air_density=None, use_cp=False):
     """Get power output when the inflow wind speed is ws. If the
     given wind speed does not have an associated power output,
     it is linearly interpolated between data points.
 
     Parameters
@@ -420,14 +506,17 @@
     ws : array_like, floats
         Wind speeds to obtain WTG power for.
     interp_method : str
         Interpolation method to use between provided table values.
         Uses xr.DataArray.interp
     air_density : float, optional
         Air density, defaults to "air_density" from the WTG, or 1.225 kg/m^3 if it's missing.
+    use_cp : bool
+        If set to true, use the 'power_coefficient' values in the dataset to calculate the
+        power output. Defaults to False.
 
     Returns
     -------
     xr.DataArray
         Power for the given wind speeds
 
     """
@@ -480,14 +569,17 @@
     ws : array_like, floats
         Wind speeds to obtain WTG power for.
     air_density : float, optional
         Air density, defaults to "air_density" from the WTG, or 1.225 kg/m^3 if it's missing.
     interp_method : str
         Interpolation method to use between provided table values.
         Uses xr.DataArray.interp
+    use_power : bool
+        if set to True, use the 'power_output' values in the dataset to calculate cp. Defaults
+        to False.
 
     Returns
     -------
     xr.DataArray
         Power Coefficient for the given wind speeds
 
     """
@@ -535,15 +627,17 @@
     wtg : xr.Dataset
         WindKit Wind Turbine Generator (WTG) Dataset
     ws : array_like, floats
         Wind speeds to obtain WTG power for.
     interp_method : str
         Interpolation method to use between provided table values.
         Uses xr.DataArray.interp
-
+    ct_stat: float
+       Stationary thrust coefficient to be used when the dataset does
+       not have it.
     Returns
     -------
     xr.DataArray
         Thrust coefficients for the given wind speeds
 
     """
 
@@ -619,14 +713,19 @@
                     f"Expected two items in each tuple. {len(item)} found!"
                 )
             for obj in item:
                 if not isinstance(obj, xr.Dataset):
                     raise ValueError(
                         f"Expected pairs of xr.Dataset's in each tuple, but got {type(obj)}!"
                     )
+            if "mode" in item[0].dims:
+                raise ValueError(
+                    "Wind Turbine xarray.dataset has more than one mode, which is not"
+                    " supported yet. Please provide a dataset without 'mode' dimension"
+                )
         return self
 
     def _clear_cache(self):
         """Clear the cached objects."""
         props = [
             "coords",
             "counts",
```

### Comparing `windkit-0.6.2/windkit/workspace.py` & `windkit-0.6.3/windkit/workspace.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.2/windkit.egg-info/SOURCES.txt` & `windkit-0.6.3/windkit.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -5,30 +5,33 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README-Internal.md
 README.md
 pyproject.toml
 setup.cfg
+.conda_env/dev_unix.yml
+.conda_env/dev_win.yml
+.conda_env/prod_unix.yml
+.gitlab/issue_templates/release.md
 .gitlab/merge_request_templates/default.md
-CI_helper_scripts/post_build_test_nix.sh
-CI_helper_scripts/post_build_test_win.sh
 docs/.dockerignore
 docs/.gitignore
 docs/Dockerfile
 docs/Makefile
 docs/docker-compose.yml
 docs/nginx.conf
 docs/legacy/dev/dev-git.rst
 docs/legacy/dev/dev-intro.rst
 docs/legacy/dev/dev-pytest.rst
 docs/legacy/dev/dev-sphinx.rst
 docs/source/WAsP.bib
 docs/source/conf.py
 docs/source/development_roadmap.rst
+docs/source/getting_started.rst
 docs/source/index.rst
 docs/source/installation.rst
 docs/source/map_conversion.rst
 docs/source/map_conversion_examples_nb.nblink
 docs/source/plotting.rst
 docs/source/plotting_examples.rst
 docs/source/plotting_examples_nb.nblink
@@ -81,20 +84,14 @@
 windkit/vector_map.py
 windkit/weibull.py
 windkit/weibull_wind_climate.py
 windkit/wind.py
 windkit/wind_climate.py
 windkit/wind_turbine.py
 windkit/workspace.py
-windkit.egg-info/PKG-INFO
-windkit.egg-info/SOURCES.txt
-windkit.egg-info/dependency_links.txt
-windkit.egg-info/entry_points.txt
-windkit.egg-info/requires.txt
-windkit.egg-info/top_level.txt
 windkit/landcovertables/CGLS-LC100.json
 windkit/landcovertables/CORINE.json
 windkit/landcovertables/Globcover.json
 windkit/landcovertables/MODIS.json
 windkit/landcovertables/WorldCover.json
 windkit/map_conversion/__init__.py
 windkit/map_conversion/helper_functions.py
```

