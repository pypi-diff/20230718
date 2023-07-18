# Comparing `tmp/openghg-0.6.0.tar.gz` & `tmp/openghg-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openghg-0.6.0.tar", last modified: Tue Jul 18 16:00:39 2023, max compression
+gzip compressed data, was "openghg-1.0.0.tar", last modified: Thu Mar  3 10:55:44 2022, max compression
```

## Comparing `openghg-0.6.0.tar` & `openghg-1.0.0.tar`

### file list

```diff
@@ -1,172 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.199224 openghg-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-07-18 16:00:24.000000 openghg-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-18 16:00:24.000000 openghg-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-07-18 16:00:39.199224 openghg-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-07-18 16:00:24.000000 openghg-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.171224 openghg-0.6.0/openghg/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23559 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.171224 openghg-0.6.0/openghg/analyse/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/analyse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    81288 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/analyse/_scenario.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.171224 openghg-0.6.0/openghg/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/cloud/_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/cloud/_packaging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.175224 openghg-0.6.0/openghg/data/
--rwxr-xr-x   0 runner    (1001) docker     (123)    16856 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/data/OpenGHG_Logo_NoText_transparent_200x200.png
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/data/acrg_obs_scale_convert.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/data/attributes.json
--rw-r--r--   0 runner    (1001) docker     (123)    33944 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/data/beaco2n_site_data.json
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/data/ceda_compliance.json
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/data/colour_maps.json
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/data/ecmwf_dataset_info.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.175224 openghg-0.6.0/openghg/data/job_controllers/
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/data/job_controllers/bc4_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9507 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/data/process_gcwerks_parameters.json
--rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/data/process_gcwerks_parameters_bp1.json
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/data/source_format_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.175224 openghg-0.6.0/openghg/dataobjects/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/dataobjects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/dataobjects/_basedata.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/dataobjects/_bc_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/dataobjects/_datamanager.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/dataobjects/_flux_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/dataobjects/_footprint_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/dataobjects/_metdata.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/dataobjects/_obscolumn_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/dataobjects/_obsdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/dataobjects/_ranksources.py
--rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/dataobjects/_searchresults.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/key_notes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.179224 openghg-0.6.0/openghg/objectstore/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/objectstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/objectstore/_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/objectstore/_integrity.py
--rw-r--r--   0 runner    (1001) docker     (123)    12612 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/objectstore/_local_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/objectstore/_oci_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/objectstore/_par.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.179224 openghg-0.6.0/openghg/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/plotting/_footprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/plotting/_timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.179224 openghg-0.6.0/openghg/retrieve/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/retrieve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29657 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/retrieve/_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/retrieve/_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    22983 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/retrieve/_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.179224 openghg-0.6.0/openghg/retrieve/ceda/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/retrieve/ceda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/retrieve/ceda/_retrieve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.179224 openghg-0.6.0/openghg/retrieve/icos/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/retrieve/icos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22467 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/retrieve/icos/_retrieve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.179224 openghg-0.6.0/openghg/retrieve/met/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/retrieve/met/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/retrieve/met/_ecmwf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.183224 openghg-0.6.0/openghg/retrieve/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    30343 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/retrieve/metadata/acrg_site_info.json
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/retrieve/metadata/process_gcwerks_parameters.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.183224 openghg-0.6.0/openghg/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/service/_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/service/_openghg_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.183224 openghg-0.6.0/openghg/standardise/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/standardise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20852 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/standardise/_standardise.py
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/standardise/_summarise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.183224 openghg-0.6.0/openghg/standardise/column/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/standardise/column/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11987 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/standardise/column/_openghg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.183224 openghg-0.6.0/openghg/standardise/emissions/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/standardise/emissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/standardise/emissions/_openghg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.183224 openghg-0.6.0/openghg/standardise/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/standardise/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/standardise/meta/_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/standardise/meta/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.187224 openghg-0.6.0/openghg/standardise/surface/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/standardise/surface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/standardise/surface/_aqmesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/standardise/surface/_beaco2n.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/standardise/surface/_btt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/standardise/surface/_cranfield.py
--rw-r--r--   0 runner    (1001) docker     (123)    12907 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/standardise/surface/_crds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/standardise/surface/_eurocom.py
--rw-r--r--   0 runner    (1001) docker     (123)    21039 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/standardise/surface/_gcwerks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/standardise/surface/_glasgow_licor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/standardise/surface/_glasgow_picarro.py
--rw-r--r--   0 runner    (1001) docker     (123)    13017 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/standardise/surface/_icos.py
--rw-r--r--   0 runner    (1001) docker     (123)    25372 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/standardise/surface/_noaa.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/standardise/surface/_npl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9391 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/standardise/surface/_openghg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/standardise/surface/_thamesbarrier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.191224 openghg-0.6.0/openghg/store/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/store/_boundary_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/store/_data_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/store/_emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/store/_eulerian_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/store/_footprints.py
--rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/store/_infer_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/store/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/store/_metstore.py
--rw-r--r--   0 runner    (1001) docker     (123)    10136 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/store/_obscolumn.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/store/_obsmobile.py
--rw-r--r--   0 runner    (1001) docker     (123)    24794 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/store/_obssurface.py
--rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/store/_populate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/store/_recombination.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/store/_segment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.191224 openghg-0.6.0/openghg/store/base/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/store/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17463 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/store/base/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    35755 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/store/base/_datasource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.191224 openghg-0.6.0/openghg/store/spec/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/store/spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/store/spec/_specification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.191224 openghg-0.6.0/openghg/transform/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/transform/_regrid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.191224 openghg-0.6.0/openghg/transform/emissions/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/transform/emissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42057 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/transform/emissions/_edgar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.191224 openghg-0.6.0/openghg/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/tutorial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/tutorial/_tutorial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.195224 openghg-0.6.0/openghg/types/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/types/_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/types/_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/types/_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.199224 openghg-0.6.0/openghg/util/
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/util/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/util/_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/util/_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/util/_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/util/_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/util/_hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/util/_inlet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/util/_site.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/util/_species.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/util/_strings.py
--rw-r--r--   0 runner    (1001) docker     (123)    25271 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/util/_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/util/_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/util/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-07-18 16:00:24.000000 openghg-0.6.0/openghg/util/_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:39.171224 openghg-0.6.0/openghg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-07-18 16:00:39.000000 openghg-0.6.0/openghg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-07-18 16:00:39.000000 openghg-0.6.0/openghg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 16:00:39.000000 openghg-0.6.0/openghg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-18 16:00:39.000000 openghg-0.6.0/openghg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-18 16:00:39.000000 openghg-0.6.0/openghg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 16:00:39.000000 openghg-0.6.0/openghg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 16:00:24.000000 openghg-0.6.0/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-18 16:00:24.000000 openghg-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-18 16:00:24.000000 openghg-0.6.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-18 16:00:24.000000 openghg-0.6.0/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-18 16:00:24.000000 openghg-0.6.0/requirements-server.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-18 16:00:24.000000 openghg-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-18 16:00:39.199224 openghg-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-18 16:00:24.000000 openghg-0.6.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83491 2023-07-18 16:00:24.000000 openghg-0.6.0/versioneer.py
+drwxr-xr-x   0 gar       (1000) gar       (1000)        0 2022-03-03 10:55:44.584626 openghg-1.0.0/
+-rw-r--r--   0 gar       (1000) gar       (1000)    10172 2021-08-04 10:42:48.000000 openghg-1.0.0/LICENSE
+-rw-r--r--   0 gar       (1000) gar       (1000)      234 2022-03-02 14:55:56.000000 openghg-1.0.0/MANIFEST.in
+-rw-r--r--   0 gar       (1000) gar       (1000)     3725 2022-03-03 10:55:44.584626 openghg-1.0.0/PKG-INFO
+-rw-r--r--   0 gar       (1000) gar       (1000)     2853 2022-03-03 10:48:06.000000 openghg-1.0.0/README.md
+drwxr-xr-x   0 gar       (1000) gar       (1000)        0 2022-03-03 10:55:44.561292 openghg-1.0.0/openghg/
+drwxr-xr-x   0 gar       (1000) gar       (1000)        0 2022-03-03 10:55:44.564626 openghg-1.0.0/openghg/.vscode/
+-rw-r--r--   0 gar       (1000) gar       (1000)       45 2020-10-09 13:29:47.000000 openghg-1.0.0/openghg/.vscode/settings.json
+-rw-r--r--   0 gar       (1000) gar       (1000)      762 2022-02-23 17:44:32.000000 openghg-1.0.0/openghg/__init__.py
+-rw-r--r--   0 gar       (1000) gar       (1000)    23080 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/_version.py
+drwxr-xr-x   0 gar       (1000) gar       (1000)        0 2022-03-03 10:55:44.564626 openghg-1.0.0/openghg/analyse/
+-rw-r--r--   0 gar       (1000) gar       (1000)      181 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/analyse/__init__.py
+-rw-r--r--   0 gar       (1000) gar       (1000)    30110 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/analyse/_footprint.py
+-rw-r--r--   0 gar       (1000) gar       (1000)    64355 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/analyse/_scenario.py
+drwxr-xr-x   0 gar       (1000) gar       (1000)        0 2022-03-03 10:55:44.564626 openghg-1.0.0/openghg/client/
+-rw-r--r--   0 gar       (1000) gar       (1000)      178 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/client/__init__.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     6906 2022-02-25 11:44:47.000000 openghg-1.0.0/openghg/client/_jobrunner.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     2767 2022-03-02 18:09:56.000000 openghg-1.0.0/openghg/client/_observations.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     7647 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/client/_process.py
+-rw-r--r--   0 gar       (1000) gar       (1000)      601 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/client/_rank_sources.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     3190 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/client/_search.py
+-rw-r--r--   0 gar       (1000) gar       (1000)      445 2022-02-25 11:44:47.000000 openghg-1.0.0/openghg/client/_test_service.py
+-rw-r--r--   0 gar       (1000) gar       (1000)      952 2022-02-25 11:44:47.000000 openghg-1.0.0/openghg/client/_user.py
+drwxr-xr-x   0 gar       (1000) gar       (1000)        0 2022-03-03 10:55:44.571292 openghg-1.0.0/openghg/data/
+-rw-r--r--   0 gar       (1000) gar       (1000)      263 2021-09-24 10:13:40.000000 openghg-1.0.0/openghg/data/README
+-rw-r--r--   0 gar       (1000) gar       (1000)      160 2021-09-20 13:36:26.000000 openghg-1.0.0/openghg/data/acrg_obs_scale_convert.csv
+-rw-r--r--   0 gar       (1000) gar       (1000)    76611 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/data/acrg_site_info.json
+-rw-r--r--   0 gar       (1000) gar       (1000)    13357 2021-09-20 13:36:26.000000 openghg-1.0.0/openghg/data/acrg_species_info.json
+-rw-r--r--   0 gar       (1000) gar       (1000)    28938 2021-09-20 13:36:26.000000 openghg-1.0.0/openghg/data/acrg_with_locations.json
+-rw-r--r--   0 gar       (1000) gar       (1000)     9002 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/data/attributes.json
+-rw-r--r--   0 gar       (1000) gar       (1000)    33944 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/data/beaco2n_site_data.json
+-rw-r--r--   0 gar       (1000) gar       (1000)      947 2021-09-20 13:36:26.000000 openghg-1.0.0/openghg/data/ceda_compliance.json
+-rw-r--r--   0 gar       (1000) gar       (1000)      878 2021-09-20 13:36:26.000000 openghg-1.0.0/openghg/data/colour_maps.json
+-rw-r--r--   0 gar       (1000) gar       (1000)      569 2021-09-20 13:36:26.000000 openghg-1.0.0/openghg/data/ecmwf_dataset_info.json
+-rw-r--r--   0 gar       (1000) gar       (1000)     3036 2021-09-20 13:36:26.000000 openghg-1.0.0/openghg/data/icos_eurocom_sites.json
+drwxr-xr-x   0 gar       (1000) gar       (1000)        0 2022-03-03 10:55:44.571292 openghg-1.0.0/openghg/data/job_controllers/
+-rw-r--r--   0 gar       (1000) gar       (1000)     2290 2022-02-25 11:44:47.000000 openghg-1.0.0/openghg/data/job_controllers/bc4_template.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     1022 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/data/lghg_data.json
+-rw-r--r--   0 gar       (1000) gar       (1000)    10709 2022-01-19 15:51:23.000000 openghg-1.0.0/openghg/data/name_code_lookup.json
+-rw-r--r--   0 gar       (1000) gar       (1000)    24265 2020-10-30 14:26:53.000000 openghg-1.0.0/openghg/data/noaa_data.json
+-rw-r--r--   0 gar       (1000) gar       (1000)    24265 2020-10-30 14:26:59.000000 openghg-1.0.0/openghg/data/noaa_sites.json
+-rw-r--r--   0 gar       (1000) gar       (1000)     9507 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/data/process_gcwerks_parameters.json
+-rw-r--r--   0 gar       (1000) gar       (1000)     7799 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/data/process_gcwerks_parameters_bp1.json
+drwxr-xr-x   0 gar       (1000) gar       (1000)        0 2022-03-03 10:55:44.571292 openghg-1.0.0/openghg/data/processing/
+-rw-r--r--   0 gar       (1000) gar       (1000)     2195 2021-09-24 10:22:00.000000 openghg-1.0.0/openghg/data/processing/site_processing_params.json
+-rw-r--r--   0 gar       (1000) gar       (1000)     3264 2021-09-20 13:36:26.000000 openghg-1.0.0/openghg/data/site_codes.json
+-rw-r--r--   0 gar       (1000) gar       (1000)    10676 2022-01-19 12:22:05.000000 openghg-1.0.0/openghg/data/site_longname.json
+-rw-r--r--   0 gar       (1000) gar       (1000)    30744 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/data/site_lookup.json
+-rw-r--r--   0 gar       (1000) gar       (1000)    12718 2021-09-20 13:36:26.000000 openghg-1.0.0/openghg/data/species_attributes.json
+-rw-r--r--   0 gar       (1000) gar       (1000)     2205 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/data/species_translator.json
+drwxr-xr-x   0 gar       (1000) gar       (1000)        0 2022-03-03 10:55:44.571292 openghg-1.0.0/openghg/dataobjects/
+-rw-r--r--   0 gar       (1000) gar       (1000)      249 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/dataobjects/__init__.py
+-rw-r--r--   0 gar       (1000) gar       (1000)      413 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/dataobjects/_basedata.py
+-rw-r--r--   0 gar       (1000) gar       (1000)      885 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/dataobjects/_flux_data.py
+-rw-r--r--   0 gar       (1000) gar       (1000)      900 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/dataobjects/_footprint_data.py
+-rw-r--r--   0 gar       (1000) gar       (1000)      163 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/dataobjects/_metdata.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     2921 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/dataobjects/_obsdata.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     8635 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/dataobjects/_ranksources.py
+-rw-r--r--   0 gar       (1000) gar       (1000)    13649 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/dataobjects/_searchresults.py
+drwxr-xr-x   0 gar       (1000) gar       (1000)        0 2022-03-03 10:55:44.574626 openghg-1.0.0/openghg/jobs/
+-rw-r--r--   0 gar       (1000) gar       (1000)      126 2021-09-20 13:36:26.000000 openghg-1.0.0/openghg/jobs/__init__.py
+-rw-r--r--   0 gar       (1000) gar       (1000)      887 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/jobs/_create.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     2523 2022-02-25 11:44:47.000000 openghg-1.0.0/openghg/jobs/_jobdrive.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     4287 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/jobs/_run.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     4095 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/jobs/_sshconnect.py
+-rw-r--r--   0 gar       (1000) gar       (1000)      972 2021-09-20 13:36:26.000000 openghg-1.0.0/openghg/key_notes
+drwxr-xr-x   0 gar       (1000) gar       (1000)        0 2022-03-03 10:55:44.574626 openghg-1.0.0/openghg/objectstore/
+-rw-r--r--   0 gar       (1000) gar       (1000)      755 2022-02-25 11:44:47.000000 openghg-1.0.0/openghg/objectstore/__init__.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     6309 2021-07-19 16:09:02.000000 openghg-1.0.0/openghg/objectstore/_hugs_objstore.py.bak
+-rw-r--r--   0 gar       (1000) gar       (1000)     9779 2022-02-25 11:44:47.000000 openghg-1.0.0/openghg/objectstore/_local_store.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     6090 2022-02-25 11:44:47.000000 openghg-1.0.0/openghg/objectstore/_openghg_objstore.py
+drwxr-xr-x   0 gar       (1000) gar       (1000)        0 2022-03-03 10:55:44.574626 openghg-1.0.0/openghg/plotting/
+-rw-r--r--   0 gar       (1000) gar       (1000)       39 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/plotting/__init__.py
+-rw-r--r--   0 gar       (1000) gar       (1000)      974 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/plotting/_footprint.py
+drwxr-xr-x   0 gar       (1000) gar       (1000)        0 2022-03-03 10:55:44.574626 openghg-1.0.0/openghg/retrieve/
+-rw-r--r--   0 gar       (1000) gar       (1000)      125 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/retrieve/__init__.py
+-rw-r--r--   0 gar       (1000) gar       (1000)    16928 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/retrieve/_access.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     5739 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/retrieve/_export.py
+-rw-r--r--   0 gar       (1000) gar       (1000)    16335 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/retrieve/_search.py
+drwxr-xr-x   0 gar       (1000) gar       (1000)        0 2022-03-03 10:55:44.574626 openghg-1.0.0/openghg/retrieve/met/
+-rw-r--r--   0 gar       (1000) gar       (1000)       33 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/retrieve/met/__init__.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     8299 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/retrieve/met/_ecmwf.py
+drwxr-xr-x   0 gar       (1000) gar       (1000)        0 2022-03-03 10:55:44.574626 openghg-1.0.0/openghg/retrieve/metadata/
+-rw-r--r--   0 gar       (1000) gar       (1000)    30343 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/retrieve/metadata/acrg_site_info.json
+-rw-r--r--   0 gar       (1000) gar       (1000)     8570 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/retrieve/metadata/process_gcwerks_parameters.json
+drwxr-xr-x   0 gar       (1000) gar       (1000)        0 2022-03-03 10:55:44.574626 openghg-1.0.0/openghg/service/
+-rw-r--r--   0 gar       (1000) gar       (1000)        0 2021-09-20 13:36:26.000000 openghg-1.0.0/openghg/service/__init__.py
+-rw-r--r--   0 gar       (1000) gar       (1000)       83 2022-02-25 11:44:47.000000 openghg-1.0.0/openghg/service/_errors.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     1090 2021-09-20 13:36:26.000000 openghg-1.0.0/openghg/service/_openghg_service.py
+drwxr-xr-x   0 gar       (1000) gar       (1000)        0 2022-03-03 10:55:44.574626 openghg-1.0.0/openghg/standardise/
+-rw-r--r--   0 gar       (1000) gar       (1000)       43 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/standardise/__init__.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     4501 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/standardise/_summarise.py
+drwxr-xr-x   0 gar       (1000) gar       (1000)        0 2022-03-03 10:55:44.577959 openghg-1.0.0/openghg/standardise/meta/
+-rw-r--r--   0 gar       (1000) gar       (1000)      102 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/standardise/meta/__init__.py
+-rw-r--r--   0 gar       (1000) gar       (1000)    12955 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/standardise/meta/_attributes.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     2312 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/standardise/meta/_metadata.py
+drwxr-xr-x   0 gar       (1000) gar       (1000)        0 2022-03-03 10:55:44.577959 openghg-1.0.0/openghg/standardise/surface/
+-rw-r--r--   0 gar       (1000) gar       (1000)      434 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/standardise/surface/__init__.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     3558 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/standardise/surface/_aqmesh.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     3418 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/standardise/surface/_beaco2n.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     3465 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/standardise/surface/_btt.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     2560 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/standardise/surface/_cranfield.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     9870 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/standardise/surface/_crds.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     3971 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/standardise/surface/_eurocom.py
+-rw-r--r--   0 gar       (1000) gar       (1000)    20059 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/standardise/surface/_gcwerks.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     1319 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/standardise/surface/_glasgow_licor.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     1723 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/standardise/surface/_glasgow_picarro.py
+-rw-r--r--   0 gar       (1000) gar       (1000)    23752 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/standardise/surface/_noaa.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     2692 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/standardise/surface/_npl.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     2843 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/standardise/surface/_thamesbarrier.py
+drwxr-xr-x   0 gar       (1000) gar       (1000)        0 2022-03-03 10:55:44.581292 openghg-1.0.0/openghg/store/
+-rw-r--r--   0 gar       (1000) gar       (1000)      357 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/store/__init__.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     9239 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/store/_emissions.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     9041 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/store/_eulerian_model.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     9316 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/store/_footprints.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     4129 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/store/_metstore.py
+-rw-r--r--   0 gar       (1000) gar       (1000)      263 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/store/_obsmobile.py
+-rw-r--r--   0 gar       (1000) gar       (1000)    14269 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/store/_obssurface.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     8566 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/store/_populate.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     6980 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/store/_recombination.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     4692 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/store/_segment.py
+drwxr-xr-x   0 gar       (1000) gar       (1000)        0 2022-03-03 10:55:44.581292 openghg-1.0.0/openghg/store/base/
+-rw-r--r--   0 gar       (1000) gar       (1000)       65 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/store/base/__init__.py
+-rw-r--r--   0 gar       (1000) gar       (1000)    12945 2022-02-25 11:44:47.000000 openghg-1.0.0/openghg/store/base/_base.py
+-rw-r--r--   0 gar       (1000) gar       (1000)    28512 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/store/base/_datasource.py
+drwxr-xr-x   0 gar       (1000) gar       (1000)        0 2022-03-03 10:55:44.581292 openghg-1.0.0/openghg/types/
+-rw-r--r--   0 gar       (1000) gar       (1000)      199 2022-02-25 11:44:47.000000 openghg-1.0.0/openghg/types/__init__.py
+-rw-r--r--   0 gar       (1000) gar       (1000)      869 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/types/_enum.py
+-rw-r--r--   0 gar       (1000) gar       (1000)      464 2022-02-25 11:44:47.000000 openghg-1.0.0/openghg/types/_errors.py
+-rw-r--r--   0 gar       (1000) gar       (1000)      180 2022-02-07 16:07:20.000000 openghg-1.0.0/openghg/types/_types.py
+drwxr-xr-x   0 gar       (1000) gar       (1000)        0 2022-03-03 10:55:44.584626 openghg-1.0.0/openghg/util/
+-rw-r--r--   0 gar       (1000) gar       (1000)      927 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/util/__init__.py
+-rw-r--r--   0 gar       (1000) gar       (1000)      186 2021-05-28 13:02:30.000000 openghg-1.0.0/openghg/util/_daterange.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     3888 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/util/_export.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     2244 2022-03-02 18:09:56.000000 openghg-1.0.0/openghg/util/_file.py
+-rw-r--r--   0 gar       (1000) gar       (1000)      968 2022-01-27 16:35:32.000000 openghg-1.0.0/openghg/util/_hashing.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     2334 2022-03-01 10:48:55.000000 openghg-1.0.0/openghg/util/_strings.py
+-rw-r--r--   0 gar       (1000) gar       (1000)    17127 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/util/_time.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     1567 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/util/_tutorial.py
+-rw-r--r--   0 gar       (1000) gar       (1000)     4050 2022-03-03 09:58:15.000000 openghg-1.0.0/openghg/util/_util.py
+drwxr-xr-x   0 gar       (1000) gar       (1000)        0 2022-03-03 10:55:44.564626 openghg-1.0.0/openghg.egg-info/
+-rw-r--r--   0 gar       (1000) gar       (1000)     3725 2022-03-03 10:55:44.000000 openghg-1.0.0/openghg.egg-info/PKG-INFO
+-rw-r--r--   0 gar       (1000) gar       (1000)     3949 2022-03-03 10:55:44.000000 openghg-1.0.0/openghg.egg-info/SOURCES.txt
+-rw-r--r--   0 gar       (1000) gar       (1000)        1 2022-03-03 10:55:44.000000 openghg-1.0.0/openghg.egg-info/dependency_links.txt
+-rw-r--r--   0 gar       (1000) gar       (1000)      173 2022-03-03 10:55:44.000000 openghg-1.0.0/openghg.egg-info/requires.txt
+-rw-r--r--   0 gar       (1000) gar       (1000)        8 2022-03-03 10:55:44.000000 openghg-1.0.0/openghg.egg-info/top_level.txt
+-rw-r--r--   0 gar       (1000) gar       (1000)      103 2022-02-25 11:44:47.000000 openghg-1.0.0/pyproject.toml
+-rw-r--r--   0 gar       (1000) gar       (1000)      402 2022-03-03 09:58:15.000000 openghg-1.0.0/requirements-dev.txt
+-rw-r--r--   0 gar       (1000) gar       (1000)      165 2022-01-27 16:35:32.000000 openghg-1.0.0/requirements-doc.txt
+-rw-r--r--   0 gar       (1000) gar       (1000)      201 2022-02-25 11:44:47.000000 openghg-1.0.0/requirements-server.txt
+-rw-r--r--   0 gar       (1000) gar       (1000)      179 2022-03-03 09:58:15.000000 openghg-1.0.0/requirements.txt
+-rw-r--r--   0 gar       (1000) gar       (1000)     1577 2022-03-03 10:55:44.584626 openghg-1.0.0/setup.cfg
+-rw-r--r--   0 gar       (1000) gar       (1000)     1137 2022-03-03 10:55:28.000000 openghg-1.0.0/setup.py
+-rw-r--r--   0 gar       (1000) gar       (1000)    80044 2022-03-03 09:58:16.000000 openghg-1.0.0/versioneer.py
```

### Comparing `openghg-0.6.0/LICENSE` & `openghg-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openghg-0.6.0/openghg/_version.py` & `openghg-1.0.0/openghg/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-# type: ignore
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
-# This file is released into the public domain.
-# Generated by versioneer-0.28
-# https://github.com/python-versioneer/python-versioneer
+# This file is released into the public domain. Generated by
+# versioneer-0.21 (https://github.com/python-versioneer/python-versioneer)
+
+# type: ignore
 
 """Git implementation of _version.py."""
 
 import errno
 import os
 import re
 import subprocess
 import sys
 from typing import Callable, Dict
-import functools
 
 
 def get_keywords():
     """Get the keywords needed to look up the version information."""
     # these strings will be replaced by git during git-archive.
     # setup.py/versioneer.py will grep for the variable names, so they must
     # each be defined on a line of their own. _version.py will just call
@@ -72,33 +71,24 @@
     return decorate
 
 
 def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False, env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
     process = None
-
-    popen_kwargs = {}
-    if sys.platform == "win32":
-        # This hides the console window if pythonw.exe is used
-        startupinfo = subprocess.STARTUPINFO()
-        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
-        popen_kwargs["startupinfo"] = startupinfo
-
     for command in commands:
         try:
             dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
             process = subprocess.Popen(
                 [command] + args,
                 cwd=cwd,
                 env=env,
                 stdout=subprocess.PIPE,
                 stderr=(subprocess.PIPE if hide_stderr else None),
-                **popen_kwargs,
             )
             break
         except OSError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
@@ -249,35 +239,38 @@
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
+    TAG_PREFIX_REGEX = "*"
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
+        TAG_PREFIX_REGEX = r"\*"
 
-    # GIT_DIR can interfere with correct operation of Versioneer.
-    # It may be intended to be passed to the Versioneer-versioned project,
-    # but that should not change where we get our version from.
-    env = os.environ.copy()
-    env.pop("GIT_DIR", None)
-    runner = functools.partial(runner, env=env)
-
-    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=not verbose)
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=True)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
     describe_out, rc = runner(
         GITS,
-        ["describe", "--tags", "--dirty", "--always", "--long", "--match", f"{tag_prefix}[[:digit:]]*"],
+        [
+            "describe",
+            "--tags",
+            "--dirty",
+            "--always",
+            "--long",
+            "--match",
+            "%s%s" % (tag_prefix, TAG_PREFIX_REGEX),
+        ],
         cwd=root,
     )
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
@@ -357,16 +350,16 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
-        pieces["distance"] = len(out.split())  # total number of commits
+        count_out, rc = runner(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
+        pieces["distance"] = int(count_out)  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
     date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
     # Use only the last line.  Previous lines may contain GPG signature
     # information.
     date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
```

### Comparing `openghg-0.6.0/openghg/analyse/_scenario.py` & `openghg-1.0.0/openghg/analyse/_scenario.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,120 +1,94 @@
 """
 The ModelScenario class allows users to collate related data sources and calculate
 modelled output based on this data. The types of data currently included are:
  - Timeseries observation data (ObsData)
  - Fixed domain sensitivity maps known as footprints (FootprintData)
  - Fixed domain flux maps (FluxData) - multiple maps can be included and
  referenced by source name
- - Fixed domain vertical curtains at each boundary (BoundaryConditionsData)
+
+TODO: Also need to incorporate boundary conditions
 
 A ModelScenario instance can be created by searching the object store manually
 and providing these outputs:
->>> obs = get_obs_surface(site, species, inlet, ...)
->>> footprint = get_footprint(site, domain, inlet, ...)
->>> flux = get_flux(species, source, domain, ...)
->>> bc = get_bc(species, domain, bc_input, ...)
->>> model = ModelScenario(obs=obs, footprint=footprint, flux=flux, bc=bc)
+>>> obs = get_obs_surface(site, species, ...)
+>>> footprint = get_footprint(site, domain, ...)
+>>> flux = get_flux(species, source, ...)
+>>> model = ModelScenario(obs=obs, footprint=footprint, flux=flux)
 
 A ModelScenario instance can also be created using keywords to search the object store:
 >>> model = ModelScenario(site,
                           species,
                           inlet,
                           network,
                           domain,
                           sources=sources,
-                          bc_input=bc_input,
                           start_date=start_date,
                           end_date=end_date)
 
 A ModelScenario instance can also be initialised and then populated after creation:
 >>> model = ModelScenario()
 >>> model.add_obs(obs=obs)
 >>> model.add_footprint(site, inlet, domain, ...)
 >>> model.add_flux(species, domain, sources, ...)
->>> model.add_bc(species, domain, bc_input, ...)
 
 Once created, methods can be called on ModelScenario which will combine these
 data sources and cache the outputs (if requested) to make for quicker calculation.
 
 >>> modelled_obs = model.calc_modelled_obs()
->>> modelled_baseline = model.calc_modelled_baseline()
 >>> combined_data = model.footprints_data_merge()
 
 If some input types needed for these operations are missing, the user will be alerted
 on which data types are missing.
 """
 
-import logging
-from typing import Any, Dict, List, Literal, Optional, Sequence, Tuple, Union, cast
+from typing import Any, Dict, List, Optional, Sequence, Tuple, Union, cast
 
-import numpy as np
-from openghg.dataobjects import BoundaryConditionsData, FluxData, FootprintData, ObsData
-from openghg.retrieve import (
-    get_obs_surface,
-    get_bc,
-    get_flux,
-    get_footprint,
-    search_surface,
-    search_bc,
-    search_flux,
-    search_footprints,
-)
-from openghg.util import synonyms
-from openghg.types import SearchError
+from openghg.dataobjects import FluxData, FootprintData, ObsData
+from openghg.retrieve import get_flux, get_footprint, get_obs_surface, search
 from pandas import Timestamp
 from xarray import DataArray, Dataset
 
 __all__ = ["ModelScenario", "combine_datasets", "stack_datasets", "calc_dim_resolution", "match_dataset_dims"]
 
 
 # TODO: Really with the emissions, they shouldn't need to match against a domain
 # We should be able to grab global/bigger area emissions and cut that down
 # to whichever area our LPDM model covers.
 
 # TODO: Add static methods for different ways of creating the class
 # e.g. from_existing_data(), from_search(), empty() , ...
 
-ParamType = Union[List[Dict[str, Optional[str]]], Dict[str, Optional[str]]]
-methodType = Optional[Literal["nearest", "pad", "ffill", "backfill", "bfill"]]
-
+# TODO: Incorporate boundary conditions when possible
 
-logger = logging.getLogger("openghg.analyse")
-logger.setLevel(logging.INFO)  # Have to set level for logger as well as handler
+ParamType = Union[List[Dict[str, Optional[str]]], Dict[str, Optional[str]]]
 
 
 class ModelScenario:
     """
     This class stores together observation data with ancillary data and allows
     operations to be performed combining these inputs.
     """
 
-    def __bool__(self) -> bool:
-        return bool(self.obs) or bool(self.footprint) or bool(self.fluxes) or bool(self.bc)
-
     def __init__(
         self,
         site: Optional[str] = None,
         species: Optional[str] = None,
         inlet: Optional[str] = None,
-        height: Optional[str] = None,
         network: Optional[str] = None,
         domain: Optional[str] = None,
         model: Optional[str] = None,
         metmodel: Optional[str] = None,
-        fp_inlet: Optional[Union[str, list]] = None,
         source: Optional[str] = None,
         sources: Optional[Union[str, Sequence]] = None,
-        bc_input: Optional[str] = None,
         start_date: Optional[Union[str, Timestamp]] = None,
         end_date: Optional[Union[str, Timestamp]] = None,
         obs: Optional[ObsData] = None,
         footprint: Optional[FootprintData] = None,
         flux: Optional[Union[FluxData, Dict[str, FluxData]]] = None,
-        bc: Optional[BoundaryConditionsData] = None,
     ):
         """
         Create a ModelScenario instance based on a set of keywords to be
         or directly supplied objects. This can be created as an empty class to be
         populated.
 
         The keywords are related to observation, footprint and flux data
@@ -124,74 +98,65 @@
          - Footprint data: site, inlet, domain, model, metmodel, species, start_date, end_date
          - Flux data: species, sources, domain, start_date, end_date
 
         Args:
             site : Site code e.g. "TAC"
             species : Species code e.g. "ch4"
             inlet : Inlet value e.g. "10m"
-            height: Alias for inlet.
             network : Network name e.g. "AGAGE"
             domain : Domain name e.g. "EUROPE"
             model : Model name used in creation of footprint e.g. "NAME"
             metmodel : Name of met model used in creation of footprint e.g. "UKV"
-            fp_inlet : Specify footprint release height options if this doesn't match to site value.
             sources : Emissions sources
-            bc_input : Input keyword for boundary conditions e.g. "mozart" or "cams"
             start_date : Start of date range to use. Note for flux this may not be applied
             end_date : End of date range to use. Note for flux this may not be applied
             obs : Supply ObsData object directly (e.g. from get_obs...() functions)
             footprint : Supply FootprintData object directly (e.g. from get_footprint() function)
             flux : Supply FluxData object directly (e.g. from get_flux() function)
+
         Returns:
             None
 
             Sets up instance of class with associated values.
 
         TODO: For obs, footprint, flux should we also allow Dataset input and turn
         these into the appropriate class?
         """
 
         self.obs: Optional[ObsData] = None
         self.footprint: Optional[FootprintData] = None
         self.fluxes: Optional[Dict[str, FluxData]] = None
-        self.bc: Optional[BoundaryConditionsData] = None
-
-        if species is not None:
-            species = synonyms(species)
 
         # Add observation data (directly or through keywords)
         self.add_obs(
             site=site,
             species=species,
             inlet=inlet,
-            height=height,
             network=network,
             start_date=start_date,
             end_date=end_date,
             obs=obs,
         )
 
         # Make sure obs data is present, make sure inputs match to metadata
         if self.obs is not None:
             obs_metadata = self.obs.metadata
             site = obs_metadata["site"]
             species = obs_metadata["species"]
             inlet = obs_metadata["inlet"]
-            logger.info("Updating any inputs based on observation data")
-            logger.info(f"site: {site}, species: {species}, inlet: {inlet}")
+            print("Updating any inputs based on observation data")
+            print(f"site: {site}, species: {species}, inlet: {inlet}")
 
         # Add footprint data (directly or through keywords)
         self.add_footprint(
             site=site,
             inlet=inlet,
-            height=height,
             domain=domain,
             model=model,
             metmodel=metmodel,
-            fp_inlet=fp_inlet,
             start_date=start_date,
             end_date=end_date,
             species=species,
             footprint=footprint,
         )
 
         # Add flux data (directly or through keywords)
@@ -201,218 +166,151 @@
             source=source,
             sources=sources,
             start_date=start_date,
             end_date=end_date,
             flux=flux,
         )
 
-        # Add boundary conditions (directly or through keywords)
-        self.add_bc(
-            species=species,
-            bc_input=bc_input,
-            domain=domain,
-            start_date=start_date,
-            end_date=end_date,
-            bc=bc,
-        )
-
         # Initialise attributes used for caching
         self.scenario: Optional[Dataset] = None
         self.modelled_obs: Optional[DataArray] = None
-        self.modelled_baseline: Optional[DataArray] = None
         self.flux_stacked: Optional[Dataset] = None
 
         # TODO: Check species, site etc. values align between inputs?
 
-    def _get_data(self, keywords: ParamType, data_type: str) -> Any:
+    def _get_data(self, keywords: ParamType, input_type: str) -> Any:
         """
         Use appropriate get function to search for data in object store.
         """
 
-        get_functions = {
-            "obs_surface": get_obs_surface,
-            "footprint": get_footprint,
-            "flux": get_flux,
-            "boundary_conditions": get_bc,
-        }
+        get_functions = {"obs_surface": get_obs_surface, "footprint": get_footprint, "flux": get_flux}
 
-        search_functions = {
-            "obs_surface": search_surface,
-            "footprint": search_footprints,
-            "flux": search_flux,
-            "boundary_conditions": search_bc,
-        }
+        # TODO: Add/write footprint and flux search? What's the syntax?
+        search_functions = {"obs_surface": search}
 
-        get_fn = get_functions[data_type]
-        search_fn = search_functions.get(data_type)
+        get_fn = get_functions[input_type]
+        search_fn = search_functions.get(input_type)
 
         if isinstance(keywords, dict):
             keywords = [keywords]
 
-        data = None
         num_checks = len(keywords)
         for i, keyword_set in enumerate(keywords):
             try:
                 data = get_fn(**keyword_set)  # type:ignore
-            except (SearchError, AttributeError):
+            except (ValueError, AttributeError):
                 num = i + 1
                 if num == num_checks:
-                    logger.warning(f"Unable to add {data_type} data based on keywords supplied.")
-                    logger.warning(" Inputs -")
+                    print(f"Unable to add {input_type} data based on keywords supplied.")
+                    print(" Inputs - \n")
                     for key, value in keyword_set.items():
-                        logger.info(f" {key}: {value}")
+                        print(f" {key}: {value}\n")
                     if search_fn is not None:
-                        data_search = search_fn(**keyword_set)  # type:ignore
-                        logger.info("---- Search results ---")
-                        logger.info(f"Number of results returned: {len(data_search)}")
-                        logger.info(data_search.results)
-                    print("\n")
+                        data_search = search_fn(**keyword_set)
+                        print("---- Search results ---")
+                        print(data_search)
+                        # TODO: If we can determine how many results are returned from search
+                        # we can use this to give better information about why no data has
+                        # been found for these inputs.
                 data = None
             else:
-                logger.info(f"Adding {data_type} to model scenario")
+                print(f"Adding {input_type} to model scenario")
                 break
 
         return data
 
     def add_obs(
         self,
         site: Optional[str] = None,
         species: Optional[str] = None,
         inlet: Optional[str] = None,
-        height: Optional[str] = None,
         network: Optional[str] = None,
         start_date: Optional[Union[str, Timestamp]] = None,
         end_date: Optional[Union[str, Timestamp]] = None,
         obs: Optional[ObsData] = None,
     ) -> None:
         """
         Add observation data based on keywords or direct ObsData object.
         """
-        from openghg.util import clean_string, format_inlet
+        from openghg.util import clean_string
 
         # Search for obs data based on keywords
         if site is not None and obs is None:
             site = clean_string(site)
-
-            if height is not None and inlet is None:
-                inlet = height
-            inlet = clean_string(inlet)
-            inlet = format_inlet(inlet)
-
             # search for obs based on suitable keywords - site, species, inlet
             obs_keywords = {
                 "site": site,
                 "species": species,
                 "inlet": inlet,
                 "network": network,
                 "start_date": start_date,
                 "end_date": end_date,
             }
 
-            obs = self._get_data(obs_keywords, data_type="obs_surface")
+            obs = self._get_data(obs_keywords, input_type="obs_surface")
 
         self.obs = obs
 
         # Add keywords to class for convenience
         if self.obs is not None:
             self.site = self.obs.metadata["site"]
             self.species = self.obs.metadata["species"]
-            self.inlet = self.obs.metadata["inlet"]
 
     def add_footprint(
         self,
         site: Optional[str] = None,
         inlet: Optional[str] = None,
-        height: Optional[str] = None,
         domain: Optional[str] = None,
         model: Optional[str] = None,
         metmodel: Optional[str] = None,
         start_date: Optional[Union[str, Timestamp]] = None,
         end_date: Optional[Union[str, Timestamp]] = None,
         species: Optional[str] = None,
-        fp_inlet: Optional[Union[str, list]] = None,
-        network: Optional[str] = None,
         footprint: Optional[FootprintData] = None,
     ) -> None:
         """
         Add footprint data based on keywords or direct FootprintData object.
         """
-        from openghg.util import (
-            clean_string,
-            format_inlet,
-            species_lifetime,
-            extract_height_name,
-        )
+        from openghg.util import clean_string
 
         # Search for footprint data based on keywords
-        # - site, domain, inlet (can extract from obs / height_name), model, metmodel
+        # - site, domain, inlet (can extract from obs), model, metmodel
         if site is not None and footprint is None:
             site = clean_string(site)
-
-            if fp_inlet is None:
-                height_name = extract_height_name(site, network, inlet)
-                if height_name is not None:
-                    fp_inlet = height_name
-                    logger.info(f"Using height_name option(s) for footprint inlet: {fp_inlet}")
-
-            if fp_inlet is None:
-                if inlet is None and self.obs is not None:
-                    fp_inlet = self.obs.metadata["inlet"]
-                elif inlet is None and height is not None:
-                    fp_inlet = clean_string(height)
-                else:
-                    fp_inlet = clean_string(inlet)
+            if inlet is None and self.obs is not None:
+                inlet = self.obs.metadata["inlet"]
 
             # TODO: Add case to deal with "multiple" inlets
-            # In this case would need to find different footprints for different inlet values
-            if fp_inlet == "multiple":
+            if inlet == "multiple":
                 raise ValueError(
                     "Unable to deal with multiple inlets yet:\n Please change date range or specify a specific inlet"
                 )
 
-            if isinstance(fp_inlet, list):
-                fp_inlet_options = fp_inlet
-            else:
-                fp_inlet_options = [fp_inlet]
-
-            fp_inlet_options = [format_inlet(value) for value in fp_inlet_options]
-
-            footprint_keyword_options = []
-            for fp_inlet_option in fp_inlet_options:
+            footprint_keywords_1 = {
+                "site": site,
+                "height": inlet,
+                "domain": domain,
+                "model": model,  # Not currently used in get_footprint - should be added
+                # "metmodel": metmodel,  # Should be added to inputs for get_footprint()
+                "start_date": start_date,
+                "end_date": end_date,
+                "species": species,
+            }
 
-                footprint_keywords = {
-                    "site": site,
-                    "height": fp_inlet_option,
-                    "inlet": fp_inlet_option,
-                    "domain": domain,
-                    "model": model,
-                    # "metmodel": metmodel,  # Should be added to inputs for get_footprint()
-                    "start_date": start_date,
-                    "end_date": end_date,
-                }
-
-                # Check whether general inert footprint should be extracted (suitable for long-lived species)
-                # or species specific footprint
-                #  - needed for short-lived species (includes additional parameters for age of particles)
-                #  - needed for carbon dioxide (include high time resolution footprint)
-                species_lifetime_value = species_lifetime(species)
-                if species_lifetime_value is not None or species == "co2":
-                    footprint_keywords["species"] = species
+            footprint_keywords_2 = footprint_keywords_1.copy()
+            footprint_keywords_2.pop("species")
 
-                footprint_keyword_options.append(footprint_keywords)
+            footprint_keywords = [footprint_keywords_1, footprint_keywords_2]
 
-            footprint = self._get_data(footprint_keyword_options, data_type="footprint")
+            footprint = self._get_data(footprint_keywords, input_type="footprint")
 
         self.footprint = footprint
 
-        if self.footprint is not None:
-            fp_inlet = self.footprint.metadata["inlet"]
-            self.fp_inlet = fp_inlet
-            if not hasattr(self, "site"):
-                self.site = self.footprint.metadata["site"]
+        if self.footprint is not None and not hasattr(self, "site"):
+            self.site = self.footprint.metadata["site"]
 
     def add_flux(
         self,
         species: Optional[str] = None,
         domain: Optional[str] = None,
         source: Optional[str] = None,
         sources: Optional[Union[str, Sequence]] = None,
@@ -456,72 +354,39 @@
                     flux_keywords_1["start_date"] = start_date
                     flux_keywords_1["end_date"] = end_date
 
                     flux_keywords = [flux_keywords_1, flux_keywords_2]
 
                 # TODO: Add something to allow for e.g. global domain or no domain
 
-                flux_source = self._get_data(flux_keywords, data_type="flux")
+                flux_source = self._get_data(flux_keywords, input_type="flux")
                 # TODO: May need to update this check if flux_source is empty FluxData() object
                 if flux_source is not None:
                     flux[name] = flux_source
 
         elif flux is not None:
             if not isinstance(flux, dict):
                 name = flux.metadata["source"]
                 flux = {name: flux}
 
         # TODO: Make this so flux.anthro can be called etc. - link in some way
         if self.fluxes is not None:
-            if flux:
+            if flux is not None:
                 self.fluxes.update(flux)
         else:
-            # Flux can be None or empty dict.
-            if flux:
-                self.fluxes = flux
+            self.fluxes = flux
 
         if self.fluxes is not None:
             if not hasattr(self, "species"):
                 flux_values = list(self.fluxes.values())
-
                 flux_1 = flux_values[0]
                 self.species = flux_1.metadata["species"]
 
             self.flux_sources = list(self.fluxes.keys())
 
-    def add_bc(
-        self,
-        species: Optional[str] = None,
-        bc_input: Optional[str] = None,
-        domain: Optional[str] = None,
-        start_date: Optional[Union[str, Timestamp]] = None,
-        end_date: Optional[Union[str, Timestamp]] = None,
-        bc: Optional[BoundaryConditionsData] = None,
-    ) -> None:
-        """
-        Add boundary conditions data based on keywords or direct BoundaryConditionsData object.
-        """
-
-        # Search for boundary conditions data based on keywords
-        # - domain, species, bc_input
-        if domain is not None and bc is None:
-
-            bc_keywords = {
-                "species": species,
-                "domain": domain,
-                "bc_input": bc_input,
-                "start_date": start_date,
-                "end_date": end_date,
-                "species": species,
-            }
-
-            bc = self._get_data(bc_keywords, data_type="boundary_conditions")
-
-        self.bc = bc
-
     def _check_data_is_present(self, need: Optional[Union[str, Sequence]] = None) -> None:
         """
         Check whether correct data types have been included. This should
         be used by functions to check whether they can perform the requested
         operation with the data types available.
 
         Args:
@@ -541,39 +406,38 @@
         need = ["fluxes" if value == "flux" else value for value in need]  # Make sure attributes match
         missing = []
         for attr in need:
             value = getattr(self, attr)
             if value is None:
                 missing.append(attr)
 
-                logger.error(f"Must have {attr} data linked to this ModelScenario to run this function")
-                logger.error("Include this by using the add function, with appropriate inputs:")
-                logger.error("  ModelScenario.add_{attr}(...)")
+                print(f"Must have {attr} data linked to this ModelScenario to run this function")
+                print("Include this by using the add function, with appropriate inputs:")
+                print("  ModelScenario.add_{attr}(...)")
 
         if missing:
             raise ValueError(f"Missing necessary {' and '.join(missing)} data.")
 
     def _get_platform(self) -> Optional[str]:
         """
         Find the platform for a site, if present.
 
-        This will access the "site_info.json" file from openghg_defs dependency to 
-        find this information.
+        This will access the "acrg_site_info.json" file to find this information.
         """
-        from openghg.util import get_site_info
+        from openghg.util import load_json
 
         try:
             site = self.site
             site_upper = site.upper()
         except AttributeError:
             return None
         else:
-            site_data = get_site_info()
+            site_info = load_json(filename="acrg_site_info.json")
             try:
-                site_details = site_data[site_upper]
+                site_details = site_info[site_upper]
             except KeyError:
                 return None
             else:
                 platform: str = site_details.get("platform")
                 return platform
 
     def _align_obs_footprint(self, resample_to: str = "coarsest", platform: Optional[str] = None) -> Tuple:
@@ -592,32 +456,27 @@
         Args:
             resample_to: Resample option to use: either data based or using a valid pandas resample period.
             platform: Observation platform used to decide whether to resample
 
         Returns:
             tuple: Two xarray.Dataset with aligned time dimensions
         """
+        import numpy as np
         from pandas import Timedelta
 
         # Check data is present (not None) and cast to correct type
         self._check_data_is_present(need=["obs", "footprint"])
         obs = cast(ObsData, self.obs)
         footprint = cast(FootprintData, self.footprint)
 
         obs_data = obs.data
         footprint_data = footprint.data
 
         resample_keyword_choices = ("obs", "footprint", "coarsest")
 
-        # Check whether resample has been requested by specifying a specific period rather than a keyword
-        if resample_to in resample_keyword_choices:
-            force_resample = False
-        else:
-            force_resample = True
-
         if platform is not None:
             platform = platform.lower()
             # Do not apply resampling for "satellite" (but have re-included "flask" for now)
             if platform == "satellite":
                 return obs_data, footprint_data
 
         # Whether sampling period is present or we need to try to infer this
@@ -631,15 +490,15 @@
             if sampling_period == "NOT_SET":
                 infer_sampling_period = True
             else:
                 obs_data_period_s = float(sampling_period)
             obs_data_period_s = float(obs_attributes["sampling_period"])
         elif "sampling_period_estimate" in obs_attributes:
             estimate = obs_attributes["sampling_period_estimate"]
-            logger.warning(f"Using estimated sampling period of {estimate}s for observational data")
+            print(f"WARNING: Using estimated sampling period of {estimate}s for observational data")
             obs_data_period_s = float(estimate)
         else:
             infer_sampling_period = True
 
         if infer_sampling_period:
             # Attempt to derive sampling period from frequency of data
             obs_data_period_s = np.nanmedian(
@@ -654,58 +513,61 @@
             # Check if the periods differ by more than 1 second
             if max_diff > 1.0:
                 raise ValueError("Sample period can be not be derived from observations")
 
         # TODO: Check regularity of the data - will need this to decide is resampling
         # is appropriate or need to do checks on a per time point basis
 
-        obs_data_period_ns = obs_data_period_s * 1e9
-        obs_data_timeperiod = Timedelta(obs_data_period_ns, unit="ns")
+        obs_data_timeperiod = Timedelta(seconds=obs_data_period_s)
 
         # Derive the footprints period from the frequency of the data
         footprint_data_period_ns = np.nanmedian(
             (footprint_data.time.data[1:] - footprint_data.time.data[0:-1]).astype("int64")
         )
         footprint_data_timeperiod = Timedelta(footprint_data_period_ns, unit="ns")
 
-        # If resample_to is set to "coarsest", check whether "obs" or "footprint" have lower resolution
-        if resample_to == "coarsest":
-            if obs_data_timeperiod >= footprint_data_timeperiod:
-                resample_to = "obs"
-            elif obs_data_timeperiod < footprint_data_timeperiod:
-                resample_to = "footprint"
-
         # Here we want timezone naive Timestamps
         # Add sampling period to end date to make sure resample includes these values when matching
         obs_startdate = Timestamp(obs_data.time[0].values)
-        obs_enddate = Timestamp(obs_data.time[-1].values) + obs_data_timeperiod
+        obs_enddate = Timestamp(obs_data.time[-1].values) + Timedelta(obs_data_timeperiod, unit="seconds")
         footprint_startdate = Timestamp(footprint_data.time[0].values)
-        footprint_enddate = Timestamp(footprint_data.time[-1].values) + footprint_data_timeperiod
+        footprint_enddate = Timestamp(footprint_data.time[-1].values) + Timedelta(
+            footprint_data_timeperiod, unit="nanoseconds"
+        )
 
         start_date = max(obs_startdate, footprint_startdate)
         end_date = min(obs_enddate, footprint_enddate)
 
-        # Ensure lower range is covered for obs
-        start_obs_slice = start_date - Timedelta("1ns")
-        # Ensure extra buffer is added for footprint based on fp timeperiod.
-        # This is to ensure footprint can be forward-filled to obs (in later steps)
-        start_footprint_slice = start_date - (footprint_data_timeperiod - Timedelta("1ns"))
+        # Subtract half a second to ensure lower range covered
+        start_slice = start_date - Timedelta("0.5s")
         # Subtract very small time increment (1 nanosecond) to make this an exclusive selection
         end_slice = end_date - Timedelta("1ns")
 
-        obs_data = obs_data.sel(time=slice(start_obs_slice, end_slice))
-        footprint_data = footprint_data.sel(time=slice(start_footprint_slice, end_slice))
+        obs_data = obs_data.sel(time=slice(start_slice, end_slice))
+        footprint_data = footprint_data.sel(time=slice(start_slice, end_slice))
+
+        # Check whether resample has been requested by specifying a specific period rather than a keyword
+        if resample_to in resample_keyword_choices:
+            force_resample = False
+        else:
+            force_resample = True
 
         # Only non satellite datasets with different periods need to be resampled
         timeperiod_diff_s = np.abs(obs_data_timeperiod - footprint_data_timeperiod).total_seconds()
         tolerance = 1e-9  # seconds
 
         if timeperiod_diff_s >= tolerance or force_resample:
             base = start_date.hour + start_date.minute / 60.0 + start_date.second / 3600.0
 
+            if resample_to == "coarsest":
+                if obs_data_timeperiod >= footprint_data_timeperiod:
+                    resample_to = "obs"
+                elif obs_data_timeperiod < footprint_data_timeperiod:
+                    resample_to = "footprint"
+
             if resample_to == "obs":
                 resample_period = str(round(obs_data_timeperiod / np.timedelta64(1, "h"), 5)) + "H"
                 footprint_data = footprint_data.resample(indexer={"time": resample_period}, base=base).mean()
 
             elif resample_to == "footprint":
                 resample_period = str(round(footprint_data_timeperiod / np.timedelta64(1, "h"), 5)) + "H"
                 obs_data = obs_data.resample(indexer={"time": resample_period}, base=base).mean()
@@ -779,20 +641,15 @@
         except AttributeError:
             raise AttributeError("Unable to read mf attribute from observation data.")
 
         if units is not None:
             combined_dataset.update({"fp": (combined_dataset.fp.dims, (combined_dataset["fp"].data / units))})
             if self.species == "co2":
                 combined_dataset.update(
-                    {
-                        "fp_HiTRes": (
-                            combined_dataset.fp_HiTRes.dims,
-                            (combined_dataset.fp_HiTRes.data / units),
-                        )
-                    }
+                    {"fp_HiTRes": (combined_dataset.fp_HiTRes.dims, (combined_dataset.fp_HiTRes / units))}
                 )
 
         attributes = {}
         attributes_obs = obs.data.attrs
         attributes_footprint = footprint.data.attrs
         attributes.update(attributes_footprint)
         attributes.update(attributes_obs)
@@ -884,146 +741,93 @@
             footprint_data = footprint.data
             time = footprint_data["time"].values
             start_date = Timestamp(time[0])
             base = start_date.hour + start_date.minute / 60.0 + start_date.second / 3600.0
             footprint_data = footprint_data.resample(indexer={"time": resample_to}, base=base).mean()
             return footprint_data
 
-    def _param_setup(
+    def calc_modelled_obs(
         self,
-        param: str = "modelled_obs",
+        sources: Optional[Union[str, List]] = None,
         resample_to: str = "coarsest",
         platform: Optional[str] = None,
+        cache: bool = True,
         recalculate: bool = False,
-    ) -> bool:
+    ) -> DataArray:
         """
-        Decide if calculation is needed for input parameter and set up
-        underlying parameters accordingly. This will populate the
-        self.scenario attribute if not already present or if this needs
-        to be recalculated.
+        Calculate the modelled observation points based on site footprint and fluxes.
+
+        The time points returned are dependent on the resample_to option chosen.
+        If obs data is also linked to the ModelScenario instance, this will be used
+        to derive the time points where appropriate.
 
         Args:
-            param : Name of the parameter being calculated.
-                    Should be one of "modelled_obs", "modelled_baseline"
+            sources: Sources to use for flux. All will be used and stacked if not specified.
             resample_to: Resample option to use for averaging:
                           - either one of ["coarsest", "obs", "footprint"] to match to the datasets
                           - or using a valid pandas resample period e.g. "2H".
                          Default = "coarsest".
             platform: Observation platform used to decide whether to resample e.g. "site", "satellite".
             cache: Cache this data after calculation. Default = True.
             recalculate: Make sure to recalculate this data rather than return from cache. Default = False.
 
         Returns:
-            bool: True if param should be calculated, False otherwise
+            xarray.DataArray: Modelled observation values along the time axis
 
-            Populates details of ModelScenario.scenario to use in calculation.
+            If cache is True:
+                This data will also be cached as the ModelScenario.modelled_obs attribute.
+                The associated scenario data will be cached as the ModelScenario.scenario attribute.
         """
 
-        try:
-            parameter = getattr(self, param)
-        except AttributeError:
-            raise ValueError(f"Did not recognise input for {param}")
+        self._check_data_is_present(need=["footprint", "fluxes"])
 
         # Check if cached modelled observations exist
-        # if self.modelled_obs is None or recalculate:
-        if parameter is None or recalculate:
+        if self.modelled_obs is None:
             # Check if observations are present and use these for resampling
             if self.obs is not None:
-                self.combine_obs_footprint(
-                    resample_to, platform=platform, recalculate=recalculate, cache=True
-                )
+                self.combine_obs_footprint(resample_to, platform=platform, cache=True)
             else:
                 self.scenario = self._check_footprint_resample(resample_to)
         else:
             if self.obs is not None:
                 # Check previous resample_to input for cached data
-                # prev_resample_to = self.modelled_obs.attrs.get("resample_to")
-                prev_resample_to = parameter.attrs.get("resample_to")
+                prev_resample_to = self.modelled_obs.attrs.get("resample_to")
 
                 # Check if this previous resample period matches input value
                 # - if not (or explicit recalculation requested), recreate scenario
                 # - if so return cached modelled observations
                 if prev_resample_to != resample_to or recalculate:
                     self.combine_obs_footprint(resample_to, platform=platform, cache=True)
                 else:
-                    # return self.modelled_obs
-                    return False
+                    return self.modelled_obs
             elif recalculate:
                 # Recalculate based on footprint data if obs not present
                 self.scenario = self._check_footprint_resample(resample_to)
-
-            # TODO: Add check for matching sources and recalculate otherwise
             else:
                 # Return cached modelled observations if explicit recalculation not requested
-                # return self.modelled_obs
-                return False
-
-        return True
-
-    def calc_modelled_obs(
-        self,
-        sources: Optional[Union[str, List]] = None,
-        resample_to: str = "coarsest",
-        platform: Optional[str] = None,
-        cache: bool = True,
-        recalculate: bool = False,
-    ) -> DataArray:
-        """
-        Calculate the modelled observation points based on site footprint and fluxes.
-
-        The time points returned are dependent on the resample_to option chosen.
-        If obs data is also linked to the ModelScenario instance, this will be used
-        to derive the time points where appropriate.
-
-        Args:
-            sources: Sources to use for flux. All will be used and stacked if not specified.
-            resample_to: Resample option to use for averaging:
-                          - either one of ["coarsest", "obs", "footprint"] to match to the datasets
-                          - or using a valid pandas resample period e.g. "2H".
-                         Default = "coarsest".
-            platform: Observation platform used to decide whether to resample e.g. "site", "satellite".
-            cache: Cache this data after calculation. Default = True.
-            recalculate: Make sure to recalculate this data rather than return from cache. Default = False.
-
-        Returns:
-            xarray.DataArray: Modelled observation values along the time axis
-
-            If cache is True:
-                This data will also be cached as the ModelScenario.modelled_obs attribute.
-                The associated scenario data will be cached as the ModelScenario.scenario attribute.
-        """
-
-        self._check_data_is_present(need=["footprint", "fluxes"])
-
-        param_calculate = self._param_setup(
-            param="modelled_obs", resample_to=resample_to, platform=platform, recalculate=recalculate
-        )
-
-        if not param_calculate:
-            modelled_obs = cast(DataArray, self.modelled_obs)
-            return modelled_obs
+                return self.modelled_obs
 
         # Check species and use high time resolution steps if this is carbon dioxide
         if self.species == "co2":
-            modelled_obs = self._calc_modelled_obs_HiTRes(
+            modelled_obs: DataArray = self._calc_modelled_obs_HiTRes(
                 sources=sources, output_TS=True, output_fpXflux=False
             )
             name = "mf_mod_high_res"
         else:
             modelled_obs = self._calc_modelled_obs_integrated(
                 sources=sources, output_TS=True, output_fpXflux=False
             )
             name = "mf_mod"
 
         modelled_obs.attrs["resample_to"] = resample_to
         modelled_obs = modelled_obs.rename(name)
 
         # Cache output from calculations
         if cache:
-            logger.info("Caching calculated data")
+            print("Caching calculated data")
             self.modelled_obs = modelled_obs
             # self.scenario[name] = modelled_obs
         else:
             self.modelled_obs = None  # Make sure this is reset and not cached
             self.scenario = None  # Reset this to None after calculation completed
 
         return modelled_obs
@@ -1063,16 +867,14 @@
         flux = self.combine_flux_sources(sources)
         scenario, flux = match_dataset_dims([scenario, flux], dims=["lat", "lon"])
 
         flux = flux.reindex_like(scenario, "ffill")
         flux_modelled: DataArray = scenario["fp"] * flux["flux"]
         timeseries: DataArray = flux_modelled.sum(["lat", "lon"])
 
-        # TODO: Add details about units to output
-
         if output_TS and output_fpXflux:
             return timeseries, flux_modelled
         elif output_TS:
             return timeseries
         elif output_fpXflux:
             return flux_modelled
 
@@ -1125,31 +927,28 @@
         they are introduced or to find a way to remove this requirement.
         TODO: mypy having trouble with different types options and incompatible types,
         included as Any for now.
         """
         from math import gcd
 
         import dask.array as da  # type: ignore
+        import numpy as np
         from pandas import date_range
         from tqdm import tqdm
 
         # TODO: Need to work out how this fits in with high time resolution method
         # Do we need to flag low resolution to use a different method? natural / anthro for example
 
         if self.scenario is None:
             raise ValueError("Combined data must have been defined before calling this function.")
 
         fp_HiTRes = self.scenario.fp_HiTRes
         flux_ds = self.combine_flux_sources(sources)
         fp_HiTRes, flux_ds = match_dataset_dims([fp_HiTRes, flux_ds], dims=["lat", "lon"])
 
-        # Make sure any NaN values are set to zero as this is a multiplicative and summing operation
-        fp_HiTRes = fp_HiTRes.fillna(0.0)
-        flux_ds["flux"] = flux_ds["flux"].fillna(0.0)
-
         # Calculate time resolution for both the flux and footprints data
         nanosecond_to_hour = 1 / (1e9 * 60.0 * 60.0)
         flux_res_H = int(flux_ds.time.diff(dim="time").values.mean() * nanosecond_to_hour)
         fp_res_time_H = int(fp_HiTRes.time.diff(dim="time").values.mean() * nanosecond_to_hour)
 
         fp_res_Hback_H = int(fp_HiTRes["H_back"].diff(dim="H_back").values.mean())
 
@@ -1198,29 +997,29 @@
 
         ntime = len(time_array)
         nlat = len(lat)
         nlon = len(lon)
         # nh_back = len(hback)
 
         # Define maximum hour back
-        max_h_back = int(hback.values[-1])
+        max_h_back = hback.values[-1]
 
         # Define full range of dates to select from the flux input
         date_start = time_array[0]
         date_start_back = date_start - np.timedelta64(max_h_back, "h")
         date_end = time_array[-1] + np.timedelta64(1, "s")
 
         start = {
             dd: getattr(np.datetime64(time_array[0].values, "h").astype(object), dd)
             for dd in ["month", "year"]
         }
 
         # Create times for matching to the flux
         full_dates = date_range(
-            date_start_back.values, date_end.values, freq=highest_resolution, inclusive="left"
+            date_start_back.values, date_end.values, freq=highest_resolution, closed="left"
         ).to_numpy()
 
         # Create low frequency flux data (monthly)
         flux_ds_low_freq = flux_ds.resample({"time": "1MS"}).mean().sel(time=slice(date_start_back, date_end))
         flux_ds_low_freq = flux_ds_low_freq.transpose(*("lat", "lon", "time"))
 
         # Select and align high frequency flux data
@@ -1260,15 +1059,15 @@
 
         if output_TS:
             timeseries = da.zeros(ntime)
 
         # Iterate through the time coord to get the total mf at each time step using the H back coord
         # at each release time we disaggregate the particles backwards over the previous 24hrs
         # The final value then contains the 29-day integrated residual footprints
-        logger.info("Calculating modelled timeseries comparison:")
+        print("Calculating modelled timeseries comparison:")
         iters = tqdm(time_array.values)
         for tt, time in enumerate(iters):
 
             # Get correct index for low resolution data based on start and current date
             current = {dd: getattr(np.datetime64(time, "h").astype(object), dd) for dd in ["month", "year"]}
             tt_low = current["month"] - start["month"] + 12 * (current["year"] - start["year"])
 
@@ -1324,16 +1123,14 @@
                 # Sum over time (H back) to give the total mf at this timestep
                 fpXflux[:, :, tt] = fpXflux_time.sum(axis=2)
 
             if output_TS:
                 # work out timeseries by summing over lat, lon (24 hrs)
                 timeseries[tt] = fpXflux_time.sum()
 
-        # TODO: Add details about units to output
-
         if output_fpXflux:
             fpXflux = DataArray(
                 fpXflux,
                 dims=("lat", "lon", "time"),
                 coords={"lat": lat, "lon": lon, "time": time_array},
             )
 
@@ -1349,163 +1146,14 @@
             return fpXflux
         elif output_TS:
             timeseries.compute()
             return timeseries
 
         return None
 
-    def calc_modelled_baseline(
-        self,
-        resample_to: str = "coarsest",
-        platform: Optional[str] = None,
-        output_units: float = 1e-9,
-        cache: bool = True,
-        recalculate: bool = False,
-    ) -> DataArray:
-        """
-        Calculate the modelled baseline points based on site footprint and boundary conditions.
-        Boundary conditions are multipled by any loss (exp(-t/lifetime)) for the species.
-
-        The time points returned are dependent on the resample_to option chosen.
-        If obs data is also linked to the ModelScenario instance, this will be used
-        to derive the time points where appropriate.
-
-        Args:
-            resample_to: Resample option to use for averaging:
-                          - either one of ["coarsest", "obs", "footprint"] to match to the datasets
-                          - or using a valid pandas resample period e.g. "2H".
-                         Default = "coarsest".
-            platform: Observation platform used to decide whether to resample e.g. "site", "satellite".
-            cache: Cache this data after calculation. Default = True.
-            recalculate: Make sure to recalculate this data rather than return from cache. Default = False.
-
-        Returns:
-            xarray.DataArray: Modelled baselined values along the time axis
-
-            If cache is True:
-                This data will also be cached as the ModelScenario.modelled_baseline attribute.
-                The associated scenario data will be cached as the ModelScenario.scenario attribute.
-        """
-        from openghg.util import check_lifetime_monthly, species_lifetime, time_offset
-
-        self._check_data_is_present(need=["footprint", "bc"])
-        bc = cast(BoundaryConditionsData, self.bc)
-
-        param_calculate = self._param_setup(
-            param="modelled_baseline", resample_to=resample_to, platform=platform, recalculate=recalculate
-        )
-
-        if not param_calculate:
-            modelled_baseline = cast(DataArray, self.modelled_baseline)
-            return modelled_baseline
-
-        scenario = cast(Dataset, self.scenario)
-        bc_data = bc.data
-
-        bc_data = bc_data.reindex_like(scenario, "ffill")
-
-        lifetime_value = species_lifetime(self.species)
-        check_monthly = check_lifetime_monthly(lifetime_value)
-
-        if check_monthly:
-            lifetime_monthly = cast(Optional[List[str]], lifetime_value)
-            lifetime: Optional[str] = None
-        else:
-            lifetime_monthly = None
-            lifetime = cast(Optional[str], lifetime_value)
-
-        if lifetime is not None:
-            short_lifetime = True
-            lt_time_delta = time_offset(period=lifetime)
-            lifetime_hrs: Union[float, np.ndarray] = lt_time_delta.total_seconds() / 3600.0
-        elif lifetime_monthly:
-            short_lifetime = True
-            lifetime_monthly_hrs = []
-            for lt in lifetime_monthly:
-                lt_time_delta = time_offset(period=lt)
-                lt_hrs = lt_time_delta.total_seconds() / 3600.0
-                lifetime_monthly_hrs.append(lt_hrs)
-
-            # calculate the lifetime_hrs associated with each time point in scenario data
-            # this is because lifetime can be a list of monthly values
-            time_month = scenario["time"].dt.month
-            lifetime_hrs = np.array([lifetime_monthly_hrs[item - 1] for item in time_month.values])
-        else:
-            short_lifetime = False
-
-        # Include loss condition if lifetime of species is specified
-        if short_lifetime:
-            expected_vars = (
-                "mean_age_particles_n",
-                "mean_age_particles_e",
-                "mean_age_particles_s",
-                "mean_age_particles_w",
-            )
-            for var in expected_vars:
-                if var not in scenario.data_vars:
-                    raise ValueError(
-                        f"Unable to calculate baseline for short-lived species {self.species} without species specific footprint."
-                    )
-
-            # Ignoring type below -  - problem with xarray patching np.exp to return DataArray rather than ndarray
-            loss_n: Union[DataArray, float] = np.exp(-1 * scenario["mean_age_particles_n"] / lifetime_hrs).rename("loss_n")  # type: ignore
-            loss_e: Union[DataArray, float] = np.exp(-1 * scenario["mean_age_particles_e"] / lifetime_hrs).rename("loss_e")  # type: ignore
-            loss_s: Union[DataArray, float] = np.exp(-1 * scenario["mean_age_particles_s"] / lifetime_hrs).rename("loss_s")  # type: ignore
-            loss_w: Union[DataArray, float] = np.exp(-1 * scenario["mean_age_particles_w"] / lifetime_hrs).rename("loss_w")  # type: ignore
-
-        else:
-
-            loss_n = 1.0
-            loss_e = 1.0
-            loss_s = 1.0
-            loss_w = 1.0
-
-        # Check and extract units as float, if present.
-        units_default = 1.0
-        units_n = check_units(bc_data["vmr_n"], default=units_default)
-        units_e = check_units(bc_data["vmr_e"], default=units_default)
-        units_s = check_units(bc_data["vmr_s"], default=units_default)
-        units_w = check_units(bc_data["vmr_w"], default=units_default)
-
-        modelled_baseline = (
-            (scenario["particle_locations_n"] * bc_data["vmr_n"] * loss_n * units_n / output_units).sum(
-                ["height", "lon"]
-            )
-            + (scenario["particle_locations_e"] * bc_data["vmr_e"] * loss_e * units_e / output_units).sum(
-                ["height", "lat"]
-            )
-            + (scenario["particle_locations_s"] * bc_data["vmr_s"] * loss_s * units_s / output_units).sum(
-                ["height", "lon"]
-            )
-            + (scenario["particle_locations_w"] * bc_data["vmr_w"] * loss_w * units_w / output_units).sum(
-                ["height", "lat"]
-            )
-        )
-
-        modelled_baseline.attrs["resample_to"] = resample_to
-        modelled_baseline.attrs["units"] = output_units
-        modelled_baseline = modelled_baseline.rename("bc_mod")
-
-        # Cache output from calculations
-        if cache:
-            logger.info("Caching calculated data")
-            self.modelled_baseline = modelled_baseline
-            # self.scenario[name] = modelled_obs
-        else:
-            self.modelled_baseline = None  # Make sure this is reset and not cached
-            self.scenario = None  # Reset this to None after calculation completed
-
-        return modelled_baseline
-
-    # def _calc_modelled_baseline_long_lived():
-    #     pass
-
-    # def _calc_modelled_baseline_short_lived():
-    #     pass
-
     def footprints_data_merge(
         self,
         resample_to: str = "coarsest",
         platform: Optional[str] = None,
         calc_timeseries: bool = True,
         sources: Optional[Union[str, List]] = None,
         calc_bc: bool = True,
@@ -1521,15 +1169,15 @@
                           - either one of ["coarsest", "obs", "footprint"] to match to the datasets
                           - or using a valid pandas resample period e.g. "2H".
                          Default = "coarsest".
             platform: Observation platform used to decide whether to resample.
             calc_timeseries: Calculate modelled timeseries based on flux sources.
             sources: Sources to use for flux if calc_timseries is True.
                      All will be used and stacked if not specified.
-            calc_baseline: Calculate modelled baseline.
+            calc_bc: Calculate boundary conditions (not currently implemented)
             cache: Cache this data after calculation. Default = True.
             recalculate: Make sure to recalculate this data rather than return from cache. Default = False.
 
         Returns:
             xarray.Dataset: Combined dataset containing footprint and observation data
         """
         combined_dataset = self.combine_obs_footprint(
@@ -1545,27 +1193,17 @@
                 recalculate=recalculate,
             )
 
             name = modelled_obs.name
             combined_dataset = combined_dataset.assign({name: modelled_obs})
 
         if calc_bc:
-            if self.bc is not None:
-                modelled_baseline = self.calc_modelled_baseline(
-                    resample_to=resample_to,
-                    platform=platform,
-                    cache=cache,
-                    recalculate=recalculate,
-                )
-                name = modelled_baseline.name
-                combined_dataset = combined_dataset.assign({name: modelled_baseline})
-            else:
-                logger.warning(
-                    "Unable to calculate baseline data. Add boundary conditions using ModelScenarion.add_bc(...) to do this."
-                )
+            # TODO: Add this in when BoundaryConditions have been incorporated
+            print("WARNING: calc_bc keyword has not been used to create output")
+            print(" BoundaryConditions have not been implemented yet.")
 
         if cache:
             self.scenario = combined_dataset
 
         return combined_dataset
 
     def plot_timeseries(self) -> Any:
@@ -1582,29 +1220,24 @@
 
         fig = obs.plot_timeseries()  # Calling method on ObsData class
 
         return fig
 
     def plot_comparison(
         self,
-        baseline: Optional[str] = "boundary_conditions",
         sources: Optional[Union[str, List]] = None,
         resample_to: str = "coarsest",
         platform: Optional[str] = None,
         cache: bool = True,
         recalculate: bool = False,
     ) -> Any:
         """
         Plot comparison between observation and modelled timeseries data.
 
         Args:
-            baseline: Add baseline to data. One of:
-                          - "boundary_conditions" - Uses added boundary conditions to calculate modelled baseline
-                          - "percentile" - Calculates the 1% value across the whole time period
-                          - None - don't add a baseline and only plot the modelled observations
             sources: Sources to use for flux. All will be used and stacked if not specified.
             resample_to: Resample option to use for averaging:
                           - either one of ["coarsest", "obs", "footprint"] to match to the datasets
                           - or using a valid pandas resample period e.g. "2H".
                          Default = "coarsest".
             platform: Observation platform used to decide whether to resample e.g. "site", "satellite".
             cache: Cache this data after calculation. Default = True.
@@ -1637,31 +1270,14 @@
 
         if sources is not None:
             source_str = ", ".join(sources)
             label = f"Modelled {species.upper()}: {source_str}"
         else:
             label = f"Modelled {species.upper()}"
 
-        # TODO: Check modelled_obs units and ensure these match to modelled_baseline
-        # - currently modelled_baseline outputs in 1e-9 (ppb) by default.
-
-        if baseline == "boundary_conditions":
-            if self.bc is not None:
-                modelled_baseline = self.calc_modelled_baseline(
-                    resample_to=resample_to, platform=platform, cache=cache, recalculate=recalculate
-                )
-                y_baseline = modelled_baseline.data
-                y_data = y_data + y_baseline
-            else:
-                logger.warning("Unable to calculate baseline from boundary conditions")
-        elif baseline == "percentile":
-            mf = obs.data["mf"]
-            y_baseline = mf.quantile(1.0, dim="time").values
-            y_data = y_data + y_baseline
-
         fig.add_trace(go.Scatter(x=x_data, y=y_data, mode="lines", name=label))
 
         return fig
 
 
 def _indexes_match(dataset_A: Dataset, dataset_B: Dataset) -> bool:
     """
@@ -1669,14 +1285,16 @@
 
     Args:
         dataset_A: First dataset to check
         dataset_B: Second dataset to check
     Returns:
         bool: True if indexes match, else False
     """
+    import numpy as np
+
     common_indices = (key for key in dataset_A.indexes.keys() if key in dataset_B.indexes.keys())
 
     for index in common_indices:
         if not len(dataset_A.indexes[index]) == len(dataset_B.indexes[index]):
             return False
 
         # Check number of values that are not close (testing for equality with floating point)
@@ -1697,15 +1315,15 @@
         if not index_diff == 0:
             return False
 
     return True
 
 
 def combine_datasets(
-    dataset_A: Dataset, dataset_B: Dataset, method: methodType = "ffill", tolerance: Optional[float] = None
+    dataset_A: Dataset, dataset_B: Dataset, method: str = "ffill", tolerance: Optional[float] = None
 ) -> Dataset:
     """
     Merges two datasets and re-indexes to the first dataset.
 
     If "fp" variable is found within the combined dataset,
     the "time" values where the "lat", "lon" dimensions didn't match are removed.
 
@@ -1715,14 +1333,16 @@
         method: One of None, nearest, ffill, bfill.
                 See xarray.DataArray.reindex_like for list of options and meaning.
                 Defaults to ffill (forward fill)
         tolerance: Maximum allowed tolerance between matches.
     Returns:
         xarray.Dataset: Combined dataset indexed to dataset_A
     """
+    import numpy as np
+
     if _indexes_match(dataset_A, dataset_B):
         dataset_B_temp = dataset_B
     else:
         dataset_B_temp = dataset_B.reindex_like(dataset_A, method=method, tolerance=tolerance)
 
     merged_ds = dataset_A.merge(dataset_B_temp)
 
@@ -1733,15 +1353,15 @@
 
     return merged_ds
 
 
 def match_dataset_dims(
     datasets: Sequence[Dataset],
     dims: Union[str, Sequence] = [],
-    method: methodType = "nearest",
+    method: str = "nearest",
     tolerance: Union[float, Dict[str, float]] = 1e-5,
 ) -> List[Dataset]:
     """
     Aligns datasets to the selected dimensions within a tolerance.
     All datasets will be aligned to the first dataset within the list.
 
     Args:
@@ -1789,48 +1409,42 @@
                     ds = ds.reindex({dim: compare_coord}, method=method, tolerance=tolerance[dim])
 
         datasets_aligned.append(ds)
 
     return datasets_aligned
 
 
-# ResType = Union[np.timedelta64, float, np.floating, np.integer]
-
-
 def calc_dim_resolution(dataset: Dataset, dim: str = "time") -> Any:
     """
     Calculates the average frequency along a given dimension.
 
     Args:
         dataset : Dataset. Must contain the specified dimension
         dim : Dimension name
 
     Returns:
         np.timedelta64 / np.float / np.int : Resolution with input dtype
 
-        NaT : If unsuccessful and input dtype is np.timedelta64
+        NaT : If unsuccessful and input dtype is np.datetime64
         NaN : If unsuccessful for all other dtypes.
     """
+    import numpy as np
+
     try:
-        resolution = dataset[dim].diff(dim=dim).mean().item()
+        resolution = dataset[dim].diff(dim=dim).mean().values
     except ValueError:
         if np.issubdtype(dataset[dim].dtype, np.datetime64):
             resolution = np.timedelta64("NaT")
         else:
             resolution = np.NaN
-    else:
-        if np.issubdtype(dataset[dim].dtype, np.datetime64):
-            # Extract units from original datetime string and use to recreate timedelta64
-            unit = dataset[dim].dtype.name.lstrip("timedelta64").lstrip("[").rstrip("]")
-            resolution = np.timedelta64(resolution, unit)
 
     return resolution
 
 
-def stack_datasets(datasets: Sequence[Dataset], dim: str = "time", method: methodType = "ffill") -> Dataset:
+def stack_datasets(datasets: Sequence[Dataset], dim: str = "time", method: str = "ffill") -> Dataset:
     """
     Stacks multiple datasets based on the input dimension. By default this is time
     and this will be aligned to the highest resolution / frequency
     (smallest difference betweeen coordinate values).
 
     At the moment, the two datasets must have identical coordinate values for all
     other dimensions and variable names for these to be stacked.
@@ -1863,35 +1477,14 @@
             data_stacked.attrs = {}
         else:
             data_stacked += data_match
 
     return data_stacked
 
 
-def check_units(data_var: DataArray, default: float) -> float:
-    """
-    Check "units" attribute within a DataArray. Expect this to be a float
-    or possible to convert to a float.
-    If not present, use default value.
-    """
-
-    attrs = data_var.attrs
-    if "units" in attrs:
-        units_from_attrs = attrs["units"]
-        if not isinstance(units_from_attrs, float):
-            try:
-                units = float(units_from_attrs)
-            except ValueError:
-                raise ValueError(f"Cannot extract {units_from_attrs} value as float")
-    else:
-        units = default
-
-    return units
-
-
 # def footprints_data_merge(data: Union[dict, ObsData],
 #                           domain: str,
 #                           met_model: Optional[str] = None,
 #                           load_flux: bool = True,
 #                           load_bc: bool = True,
 #                           calc_timeseries: bool = True,
 #                           calc_bc: bool = True,
```

### Comparing `openghg-0.6.0/openghg/data/attributes.json` & `openghg-1.0.0/openghg/data/attributes.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.46801388888888895%*

 * *Differences: {"'EUROCOM'": "{'locations': {'CBW': {'latitude': 58.97, 'longitude': -4.926}}}",*

 * * "'TMB'": "{'inlet': '5 m'}",*

 * * "'species_translation'": "OrderedDict([('CO2', OrderedDict([('chem', 'co2'), ('name', "*

 * *                          "'carbon_dioxide')])), ('CH4', OrderedDict([('chem', 'ch4'), ('name', "*

 * *                          "'methane')])), ('ETHANE', OrderedDict([('chem', 'c2h6'), ('name', "*

 * *                          "'ethane')])), ('PROPANE', OrderedDict([('chem', 'c3h8'), ('name', "*

 * *                        […]*

```diff
@@ -131,16 +131,16 @@
                 "longitude": 8.15
             },
             "BIS": {
                 "latitude": 44.38,
                 "longitude": -1.23
             },
             "CBW": {
-                "latitude": 51.9703,
-                "longitude": 4.926
+                "latitude": 58.97,
+                "longitude": -4.926
             },
             "CMN": {
                 "latitude": 44.193889,
                 "longitude": 10.701389
             },
             "HEI": {
                 "latitude": 49.417,
@@ -270,62 +270,163 @@
     },
     "TMB": {
         "global_attributes": {
             "Notes": "~5m above high tide water level, in tidal region of the Thames",
             "data_owner": "Valerio Ferracci",
             "data_owner_email": "V.Ferracci@cranfield.ac.uk"
         },
-        "inlet": "5m",
+        "inlet": "5 m",
         "instrument": "Picarro G2401",
         "scale": {
             "CH4": "WMO-CH4-X2004",
             "CO": "WMO-CO-X2014",
             "CO2": "WMO-CO2-X2007"
         },
         "unit_species": {
             "CH4": "ppb",
             "CO": "ppm",
             "CO2": "ppm"
         }
     },
+    "species_translation": {
+        "APO": {
+            "chem": "apo",
+            "name": "atmospheric_potential_oxygen"
+        },
+        "BENZENE": {
+            "chem": "c6h6",
+            "name": "benzene"
+        },
+        "C-PROPANE": {
+            "chem": "cc3h8",
+            "name": "cpropane"
+        },
+        "CH4": {
+            "chem": "ch4",
+            "name": "methane"
+        },
+        "CO": {
+            "chem": "co",
+            "name": "carbon_monoxide"
+        },
+        "CO2": {
+            "chem": "co2",
+            "name": "carbon_dioxide"
+        },
+        "DCH4C13": {
+            "chem": "dch4c13",
+            "name": "delta_ch4_c13"
+        },
+        "DCH4D": {
+            "chem": "dch4d",
+            "name": "delta_ch4_d"
+        },
+        "DCO2C13": {
+            "chem": "dco2c13",
+            "name": "delta_co2_c13"
+        },
+        "DCO2C14": {
+            "chem": "dco2c14",
+            "name": "delta_co2_c14"
+        },
+        "DO2N2": {
+            "chem": "do2n2",
+            "name": "ratio_of_oxygen_to_nitrogen"
+        },
+        "ETHANE": {
+            "chem": "c2h6",
+            "name": "ethane"
+        },
+        "ETHENE": {
+            "chem": "c2f4",
+            "name": "ethene"
+        },
+        "ETHYNE": {
+            "chem": "c2h2",
+            "name": "ethyne"
+        },
+        "F-113": {
+            "chem": "cfc113",
+            "name": "cfc113"
+        },
+        "H-1211": {
+            "chem": "halon1211",
+            "name": "halon1211"
+        },
+        "H-1301": {
+            "chem": "halon1301",
+            "name": "halon1301"
+        },
+        "H-2402": {
+            "chem": "halon2402",
+            "name": "halon2402"
+        },
+        "H2_PDD": {
+            "chem": "h2",
+            "name": "hydrogen"
+        },
+        "N2O": {
+            "chem": "n2o",
+            "name": "nitrous_oxide"
+        },
+        "NE_PDD": {
+            "chem": "ne",
+            "name": "neon"
+        },
+        "PCE": {
+            "chem": "c2cl4",
+            "name": "tetrachloroethylene"
+        },
+        "PFC-116": {
+            "chem": "c2f6",
+            "name": "hexafluoroethane"
+        },
+        "PFC-218": {
+            "chem": "c3f8",
+            "name": "octafluoropropane"
+        },
+        "PFC-318": {
+            "chem": "c4f8",
+            "name": "cyclooctafluorobutane"
+        },
+        "PROPANE": {
+            "chem": "c3h8",
+            "name": "propane"
+        },
+        "TCE": {
+            "chem": "c2hcl3",
+            "name": "trichloroethylene"
+        },
+        "TOLUENE": {
+            "chem": "c6h5ch3",
+            "name": "methylbenzene"
+        }
+    },
     "unit_interpret": {
         "else": "unknown",
-        "micromol mol-1": "1e-6",
-        "millimol mol-1": "1e-3",
-        "mol mol-1": "1",
-        "nanomol mol-1": "1e-9",
-        "nmol mol-1": "1e-9",
-        "per meg": "1",
-        "per mil": "1",
-        "permeg": "1",
-        "permil": "1",
-        "pmol mol-1": "1e-12",
         "ppb": "1e-9",
         "ppm": "1e-6",
         "ppq": "1e-15",
         "ppt": "1e-12"
     },
-    "unit_mol_fraction": [
-        "ppm",
-        "ppb",
-        "ppt",
-        "ppq",
-        "mol mol-1",
-        "millimol mol-1",
-        "micromol mol-1",
-        "nmol mol-1",
-        "nanomol mol-1",
-        "pmol mol-1"
-    ],
-    "unit_non_standard": [
-        "permil",
-        "permeg",
-        "per mil",
-        "per meg"
-    ],
-    "unit_print": {
-        "1e-12": "pmol mol$^{-1}$",
-        "1e-3": "mmol mol$^{-1}$",
-        "1e-6": "\u03bcmol mol$^{-1}$",
-        "1e-9": "nmol mol$^{-1}$"
+    "unit_species": {
+        "APO": "1",
+        "C2H6": "1e-9",
+        "CH4": "1e-9",
+        "CO": "1e-9",
+        "CO2": "1e-6",
+        "DCH4C13": "1",
+        "DCH4D": "1",
+        "DCO2C13": "1",
+        "DCO2C14": "1",
+        "DO2N2": "1",
+        "N2O": "1e-9"
+    },
+    "unit_species_long": {
+        "APO": "per meg",
+        "DCH4C13": "permil",
+        "DCH4D": "permil",
+        "DCO2C13": "permil",
+        "DCO2C14": "permil",
+        "DO2N2": "per meg"
     }
 }
```

### Comparing `openghg-0.6.0/openghg/data/beaco2n_site_data.json` & `openghg-1.0.0/openghg/data/beaco2n_site_data.json`

 * *Files identical despite different names*

### Comparing `openghg-0.6.0/openghg/data/ceda_compliance.json` & `openghg-1.0.0/openghg/data/ceda_compliance.json`

 * *Files identical despite different names*

### Comparing `openghg-0.6.0/openghg/data/colour_maps.json` & `openghg-1.0.0/openghg/data/colour_maps.json`

 * *Files identical despite different names*

### Comparing `openghg-0.6.0/openghg/data/ecmwf_dataset_info.json` & `openghg-1.0.0/openghg/data/ecmwf_dataset_info.json`

 * *Files identical despite different names*

### Comparing `openghg-0.6.0/openghg/data/job_controllers/bc4_template.py` & `openghg-1.0.0/openghg/data/job_controllers/bc4_template.py`

 * *Files identical despite different names*

### Comparing `openghg-0.6.0/openghg/data/process_gcwerks_parameters.json` & `openghg-1.0.0/openghg/data/process_gcwerks_parameters.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965277777777777%*

 * *Differences: {"'CRDS'": "{'default_scales': {'CO2': 'WMO-X2007'}}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "CRDS": {
         "comment": "Cavity ring-down measurements. Output from GCWerks",
         "default_scales": {
             "CH4": "WMO-X2004A",
             "CO": "WMO-X2014A",
-            "CO2": "WMO-X2019",
+            "CO2": "WMO-X2007",
             "N2O": "WMO-X2006A"
         },
         "sites": {
             "BSD": {
                 "gcwerks_site_name": "bilsdale",
                 "global_attributes": {
                     "data_owner": "Simon O'Doherty",
```

### Comparing `openghg-0.6.0/openghg/data/process_gcwerks_parameters_bp1.json` & `openghg-1.0.0/openghg/data/process_gcwerks_parameters_bp1.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990530303030303%*

 * *Differences: {"'CRDS'": "{'default_scales': {'CO2': 'WMO-X2007'}}"}*

```diff
@@ -49,15 +49,15 @@
                 "data_owner_email": "s.odoherty@bristol.ac.uk"
             }
         },
         "comment": "Cavity ring-down measurements. Output from GCWerks",
         "default_scales": {
             "CH4": "WMO-X2004A",
             "CO": "WMO-X2014A",
-            "CO2": "WMO-X2019",
+            "CO2": "WMO-X2007",
             "N2O": "WMO-X2006A"
         },
         "directory": "/work/chxmr/shared/obs_raw/AGAGE_GCWerks/data-picarro/%site/",
         "directory_output": "/work/chxmr/shared/obs"
     },
     "GC": {
         "BSD": {
```

### Comparing `openghg-0.6.0/openghg/dataobjects/_obsdata.py` & `openghg-1.0.0/openghg/dataobjects/_obsdata.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,11 @@
-from collections import abc
 from dataclasses import dataclass
-from json import dumps
-from pathlib import Path
-from tempfile import NamedTemporaryFile
-from typing import Any, Dict, Iterator, Union, Optional
-from openghg.plotting import plot_timeseries as general_plot_timeseries
+from collections import abc
+from typing import Any, Iterator
 import plotly.graph_objects as go
-
 from ._basedata import _BaseData
 
 __all__ = ["ObsData"]
 
 
 @dataclass(frozen=True)
 class ObsData(_BaseData, abc.Mapping):
@@ -52,47 +47,52 @@
         """
         Returns number of key values (fixed at 1 at present)
         """
         # Fixed length as 1 at the moment but may need to update if other key
         # values are added.
         return 1
 
-    def __eq__(self, other: object) -> bool:
-        if not isinstance(other, ObsData):
-            return NotImplemented
+    def plot_timeseries(
+        self, title: str = None, xlabel: str = None, ylabel: str = None, units: str = None
+    ) -> go.Figure:
+        """Plot a timeseries"""
 
-        return self.data.equals(other.data) and self.metadata == other.metadata
+        species = self.metadata["species"]
+        site = self.metadata["site"]
+        inlet = self.metadata["inlet"]
 
-    def to_data(self) -> Dict:
-        """Creates a dictionary package of this ObsData's metadata and data.
+        if title is None:
+            title = f"{species.upper()} at {site.upper()} - {inlet}"
 
-        Returns:
-            dict: Dictionary of metadata and bytes
-        """
-        to_transfer: Dict[str, Union[str, bytes]] = {}
-        to_transfer["metadata"] = dumps(self.metadata)
+        if xlabel is None:
+            xlabel = "Date"
 
-        # TODO - get better bytes
-        with NamedTemporaryFile() as tmpfile:
-            self.data.to_netcdf(tmpfile.name)
-            to_transfer["data"] = Path(tmpfile.name).read_bytes()
+        if ylabel is None:
+            ylabel = "Concentration"
 
-        return to_transfer
+        if units is not None:
+            ylabel += f"  ({units})"
 
-    def plot_timeseries(
-        self,
-        title: Optional[str] = None,
-        xlabel: Optional[str] = None,
-        ylabel: Optional[str] = None,
-        units: Optional[str] = None,
-        logo: Optional[bool] = True,
-    ) -> go.Figure:
-        """Plot a timeseries"""
+        data = self.data
+        x_data = data.time
+
+        try:
+            y_data = data[species]
+        except KeyError:
+            y_data = data["mf"]
 
-        return general_plot_timeseries(
-            data=self,
-            title=title,
-            xlabel=xlabel,
-            ylabel=ylabel,
-            units=units,
-            logo=logo,
+        font = {"size": 14}
+
+        title_layout = {"text": title, "y": 0.9, "x": 0.5, "xanchor": "center", "yanchor": "top"}
+
+        layout = go.Layout(
+            title=title_layout,
+            xaxis=dict(title=xlabel),
+            yaxis=dict(title=ylabel),
+            font=font,
         )
+
+        # Create traces
+        fig = go.Figure(layout=layout)
+        fig.add_trace(go.Scatter(x=x_data, y=y_data, mode="lines", name=species.upper()))
+
+        return fig
```

### Comparing `openghg-0.6.0/openghg/dataobjects/_ranksources.py` & `openghg-1.0.0/openghg/dataobjects/_ranksources.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,270 +1,274 @@
-# # type: ignore
-# from typing import Dict, Union
+from typing import Dict, Union
 
-# from openghg.store import ObsSurface
-# from openghg.store.base import Datasource
-# from openghg.util import create_daterange_str, verify_site
-
-
-# class RankSources:
-#     def __init__(self, cloud: bool = False) -> None:
-#         self._cloud = cloud
-
-#         raise NotImplementedError("Ranking currently not supported.")
-
-#         if cloud:
-#             raise NotImplementedError
-
-#     def raw(self) -> Dict:
-#         """Return the raw ranking data
-
-#         Args:
-#             None
-#         Returns:
-#             dict: Raw ranking data
-#         """
-#         return self._user_info
-
-#     def get_sources(self, site: str, species: str) -> Dict:
-#         """Get the datasources for this site and species to allow a ranking to be set
-
-#         Args:
-#             site: Three letter site code
-#             species: Species name
-#         Returns:
-#             dict: Dictionary of datasource metadata
-#         """
-#         if self._cloud:
-#             raise NotImplementedError
-#             # return self._get_sources_cloud(site=site, species=species)
-#         else:
-#             return self._get_sources_local(site=site, species=species)
-
-#     # def _get_sources_cloud(self, site: str, species: str) -> Dict:
-#     #     site = verify_site(site=site)
-
-#     #     args = {"site": site, "species": species}
-
-#     #     self.site = site
-#     #     self.species = species
-
-#     #     response: Dict = self._service.call_function(function="rank.get_sources", args=args)
-
-#     #     if not response:
-#     #         raise ValueError(f"No sources found for {species} at {site}")
-
-#     #     self._user_info: Dict = response["user_info"]
-#     #     self._key_lookup: Dict = response["key_lookup"]
-#     #     self._needs_update = False
-
-#     #     return self._user_info
-
-#     def _get_sources_local(self, site: str, species: str) -> Dict:
-#         raise NotImplementedError
-#         site = verify_site(site=site)
-
-#         # Save these
-#         self.site = site
-#         self.species = species
-
-#         obs = ObsSurface.load()
-#         datasource_uuids = obs.datasources()
-#         rank_table = obs.rank_data()
-
-#         # Shallow load the Datasources (only get their JSON metadata)
-#         datasources = (Datasource.load(uuid=uuid, shallow=True) for uuid in datasource_uuids)
-
-#         matching_sources = [d for d in datasources if d.search_metadata(site=site, species=species)]
-
-#         if matching_sources:
-#             self._user_info = {
-#                 d.inlet(): {
-#                     "rank_data": rank_table.get(d.uuid(), "NA"),
-#                     "data_range": d.daterange_str(),
-#                 }
-#                 for d in matching_sources
-#             }
-
-#             self._key_lookup = {d.inlet(): d.uuid() for d in matching_sources}
-#             self._needs_update = False
-#         else:
-#             self._user_info = {}
-
-#         return self._user_info
-
-#     def get_specific_source(self, inlet: str) -> Dict:
-#         """Return the ranking data of a specific key
-
-#         Args:
-#             key: Key
-#         Returns:
-#             dict: Dictionary of ranking data
-#         """
-#         if self._needs_update:
-#             self.get_sources(site=self.site, species=self.species)
-
-#         rank_data: Dict[str, Union[str, Dict]] = self._user_info[inlet]["rank_data"]
-#         return rank_data
-
-#     def set_rank(
-#         self,
-#         inlet: str,
-#         rank: Union[int, str],
-#         start_date: str,
-#         end_date: str,
-#         overwrite: bool = False,
-#     ) -> None:
-#         """Set the rank data for the
-
-#         Args:
-#             inlet: Inlet to set ranking data
-#             rank: Number between 1 and 9
-#             start_date: Start date
-#             end_date: End date
-#             overwrite: If True overwrite current ranking data
-#         Returns:
-#             None
-#         """
-#         if self._cloud:
-#             raise NotImplementedError
-#         else:
-#             return self._set_rank_local(
-#                 inlet=inlet,
-#                 rank=rank,
-#                 start_date=start_date,
-#                 end_date=end_date,
-#                 overwrite=overwrite,
-#             )
-
-#     # def _set_rank_cloud(
-#     #     self,
-#     #     inlet: str,
-#     #     rank: Union[int, str],
-#     #     start_date: str,
-#     #     end_date: str,
-#     #     overwrite: bool = False,
-#     # ) -> None:
-#     #     inlet = inlet.lower()
-#     #     uuid = self._key_lookup[inlet]
-
-#     #     dateranges = create_daterange_str(start=start_date, end=end_date)
-
-#     #     args: Dict[str, Union[str, int, List]] = {}
-#     #     args["rank"] = rank
-#     #     args["uuid"] = uuid
-#     #     args["dateranges"] = dateranges
-#     #     args["overwrite"] = overwrite
-
-#     #     self._service.call_function(function="rank.set_rank", args=args)
-#     #     self._needs_update = True
-
-#     def _set_rank_local(
-#         self,
-#         inlet: str,
-#         rank: Union[int, str],
-#         start_date: str,
-#         end_date: str,
-#         overwrite: bool = False,
-#     ) -> None:
-#         obs = ObsSurface.load()
-
-#         inlet = inlet.lower()
-#         uuid = self._key_lookup[inlet]
-
-#         daterange = create_daterange_str(start=start_date, end=end_date)
-
-#         obs.set_rank(uuid=uuid, rank=rank, date_range=daterange, overwrite=overwrite)
-
-#         self._needs_update = True
-
-#     def clear_rank(self, inlet: str) -> None:
-#         """Clear the ranking data for a Datasource
-
-#         Args:
-#             key: Key for specific source
-#         Returns:
-#             None
-#         """
-#         if self._cloud:
-#             raise NotImplementedError
-#             # return self._clear_rank_cloud(inlet=inlet)
-#         else:
-#             return self._clear_rank_local(inlet=inlet)
-
-#     def _clear_rank_local(self, inlet: str) -> None:
-#         """Clear the ranking data for a Datasource
-
-#         Args:
-#             key: Key for specific source
-#         Returns:
-#             None
-#         """
-#         obs = ObsSurface.load()
-#         inlet = inlet.lower()
-#         uuid = self._key_lookup[inlet]
-#         obs.clear_rank(uuid=uuid)
-#         self._needs_update = True
-
-#     # def _clear_rank_cloud(self, inlet: str) -> None:
-#     #     """Clear the ranking data for a Datasource
-
-#     #     Args:
-#     #         key: Key for specific source
-#     #     Returns:
-#     #         None
-#     #     """
-#     #     uuid = self._key_lookup[inlet]
-#     #     args = {"uuid": uuid}
-#     #     self._service.call_function(function="rank.clear_rank", args=args)
-#     #     self._needs_update = True
-
-#     # def visualise_rankings(self) -> Network:
-#     #     """ Creates a small network graph of ranked data with each rank given a colour
-
-#     #         Note that this function should only be run from a Jupyter Notebook
-
-#     #         Args:
-#     #             rank_data (dict): Dictionary of the form given by RankSources.get_sources()
-#     #         Returns:
-#     #             pyvis.network.Network: Network graph
-#     #     """
-#     #     header_text = "OpenGHG ranked data"
-#     #     net = Network("800px", "100%", notebook=True, heading=header_text)
-#     #     # Set the physics layout of the network
-#     #     net.force_atlas_2based()
-
-#     #     rank_data = self._key_lookup
-
-#     #     a_key = list(rank_data.keys())[0]
-#     #     site = rank_data[a_key]["metadata"]["site"].upper()
-
-#     #     norm = matplotlib.colors.Normalize(vmin=0, vmax=10, clip=True)
-#     #     mapper = cm.ScalarMappable(norm=norm, cmap=cm.tab10)
-
-#     #     def colour_mapper(x):
-#     #         return matplotlib.colors.to_hex(mapper.to_rgba(int(x)))
-
-#     #     net.add_node(site, label=site, color="brown", value=5000)
-
-#     #     for key, data in rank_data.items():
-#     #         rank = data["rank"]
-#     #         site_name = data["metadata"]["site"].upper()
-#     #         data_range = data["data_range"]
-
-#     #         # HTML to show when the mouse is hovered over a node
-#     #         title = "</br>".join([f"<b>Rank:</b> {str(rank)}", f"<b>Site:</b> {site_name}", f"<b>Data range:</b> {data_range}"])
-
-#     #         if rank == 0:
-#     #             colour = colour_mapper(rank)
-#     #         else:
-#     #             # For now just use the highest rank for the color
-#     #             highest_rank = sorted(list(rank.keys()))[-1]
-#     #             colour = colour_mapper(highest_rank)
+from openghg.store import ObsSurface
+from openghg.store.base import Datasource
+from openghg.util import create_daterange_str, verify_site
+
+
+class RankSources:
+    def __init__(self, cloud: bool = False, service_url: str = None) -> None:
+        self._cloud = cloud
+
+        if cloud:
+            raise NotImplementedError
+            # from Acquire.Client import Wallet
+
+            # wallet = Wallet()
+
+            # if service_url is None:
+            #     service_url = "https://fn.openghg.org/t"
+
+            # self._service = wallet.get_service(service_url=f"{service_url}/openghg")
+
+    def raw(self) -> Dict:
+        """Return the raw ranking data
+
+        Args:
+            None
+        Returns:
+            dict: Raw ranking data
+        """
+        return self._user_info
+
+    def get_sources(self, site: str, species: str) -> Dict:
+        """Get the datasources for this site and species to allow a ranking to be set
+
+        Args:
+            site: Three letter site code
+            species: Species name
+        Returns:
+            dict: Dictionary of datasource metadata
+        """
+        if self._cloud:
+            raise NotImplementedError
+            # return self._get_sources_cloud(site=site, species=species)
+        else:
+            return self._get_sources_local(site=site, species=species)
+
+    # def _get_sources_cloud(self, site: str, species: str) -> Dict:
+    #     site = verify_site(site=site)
+
+    #     args = {"site": site, "species": species}
+
+    #     self.site = site
+    #     self.species = species
+
+    #     response: Dict = self._service.call_function(function="rank.get_sources", args=args)
+
+    #     if not response:
+    #         raise ValueError(f"No sources found for {species} at {site}")
+
+    #     self._user_info: Dict = response["user_info"]
+    #     self._key_lookup: Dict = response["key_lookup"]
+    #     self._needs_update = False
+
+    #     return self._user_info
+
+    def _get_sources_local(self, site: str, species: str) -> Dict:
+        site = verify_site(site=site)
+
+        # Save these
+        self.site = site
+        self.species = species
+
+        obs = ObsSurface.load()
+        datasource_uuids = obs.datasources()
+        rank_table = obs.rank_data()
+
+        # Shallow load the Datasources (only get their JSON metadata)
+        datasources = (Datasource.load(uuid=uuid, shallow=True) for uuid in datasource_uuids)
+
+        matching_sources = [d for d in datasources if d.search_metadata(site=site, species=species)]
+
+        if matching_sources:
+            self._user_info = {
+                d.inlet(): {
+                    "rank_data": rank_table.get(d.uuid(), "NA"),
+                    "data_range": d.daterange_str(),
+                }
+                for d in matching_sources
+            }
+
+            self._key_lookup = {d.inlet(): d.uuid() for d in matching_sources}
+            self._needs_update = False
+        else:
+            self._user_info = {}
+
+        return self._user_info
+
+    def get_specific_source(self, inlet: str) -> Dict:
+        """Return the ranking data of a specific key
+
+        Args:
+            key: Key
+        Returns:
+            dict: Dictionary of ranking data
+        """
+        if self._needs_update:
+            self.get_sources(site=self.site, species=self.species)
+
+        rank_data: Dict[str, Union[str, Dict]] = self._user_info[inlet]["rank_data"]
+        return rank_data
+
+    def set_rank(
+        self,
+        inlet: str,
+        rank: Union[int, str],
+        start_date: str,
+        end_date: str,
+        overwrite: bool = False,
+    ) -> None:
+        """Set the rank data for the
+
+        Args:
+            inlet: Inlet to set ranking data
+            rank: Number between 1 and 9
+            start_date: Start date
+            end_date: End date
+            overwrite: If True overwrite current ranking data
+        Returns:
+            None
+        """
+        if self._cloud:
+            raise NotImplementedError
+        else:
+            return self._set_rank_local(
+                inlet=inlet,
+                rank=rank,
+                start_date=start_date,
+                end_date=end_date,
+                overwrite=overwrite,
+            )
+
+    # def _set_rank_cloud(
+    #     self,
+    #     inlet: str,
+    #     rank: Union[int, str],
+    #     start_date: str,
+    #     end_date: str,
+    #     overwrite: bool = False,
+    # ) -> None:
+    #     inlet = inlet.lower()
+    #     uuid = self._key_lookup[inlet]
+
+    #     dateranges = create_daterange_str(start=start_date, end=end_date)
+
+    #     args: Dict[str, Union[str, int, List]] = {}
+    #     args["rank"] = rank
+    #     args["uuid"] = uuid
+    #     args["dateranges"] = dateranges
+    #     args["overwrite"] = overwrite
+
+    #     self._service.call_function(function="rank.set_rank", args=args)
+    #     self._needs_update = True
+
+    def _set_rank_local(
+        self,
+        inlet: str,
+        rank: Union[int, str],
+        start_date: str,
+        end_date: str,
+        overwrite: bool = False,
+    ) -> None:
+        obs = ObsSurface.load()
+
+        inlet = inlet.lower()
+        uuid = self._key_lookup[inlet]
+
+        daterange = create_daterange_str(start=start_date, end=end_date)
+
+        obs.set_rank(uuid=uuid, rank=rank, date_range=daterange, overwrite=overwrite)
+
+        self._needs_update = True
+
+    def clear_rank(self, inlet: str) -> None:
+        """Clear the ranking data for a Datasource
+
+        Args:
+            key: Key for specific source
+        Returns:
+            None
+        """
+        if self._cloud:
+            raise NotImplementedError
+            # return self._clear_rank_cloud(inlet=inlet)
+        else:
+            return self._clear_rank_local(inlet=inlet)
+
+    def _clear_rank_local(self, inlet: str) -> None:
+        """Clear the ranking data for a Datasource
+
+        Args:
+            key: Key for specific source
+        Returns:
+            None
+        """
+        obs = ObsSurface.load()
+        inlet = inlet.lower()
+        uuid = self._key_lookup[inlet]
+        obs.clear_rank(uuid=uuid)
+        self._needs_update = True
+
+    # def _clear_rank_cloud(self, inlet: str) -> None:
+    #     """Clear the ranking data for a Datasource
+
+    #     Args:
+    #         key: Key for specific source
+    #     Returns:
+    #         None
+    #     """
+    #     uuid = self._key_lookup[inlet]
+    #     args = {"uuid": uuid}
+    #     self._service.call_function(function="rank.clear_rank", args=args)
+    #     self._needs_update = True
+
+    # def visualise_rankings(self) -> Network:
+    #     """ Creates a small network graph of ranked data with each rank given a colour
+
+    #         Note that this function should only be run from a Jupyter Notebook
+
+    #         Args:
+    #             rank_data (dict): Dictionary of the form given by RankSources.get_sources()
+    #         Returns:
+    #             pyvis.network.Network: Network graph
+    #     """
+    #     header_text = "OpenGHG ranked data"
+    #     net = Network("800px", "100%", notebook=True, heading=header_text)
+    #     # Set the physics layout of the network
+    #     net.force_atlas_2based()
+
+    #     rank_data = self._key_lookup
+
+    #     a_key = list(rank_data.keys())[0]
+    #     site = rank_data[a_key]["metadata"]["site"].upper()
+
+    #     norm = matplotlib.colors.Normalize(vmin=0, vmax=10, clip=True)
+    #     mapper = cm.ScalarMappable(norm=norm, cmap=cm.tab10)
+
+    #     def colour_mapper(x):
+    #         return matplotlib.colors.to_hex(mapper.to_rgba(int(x)))
+
+    #     net.add_node(site, label=site, color="brown", value=5000)
+
+    #     for key, data in rank_data.items():
+    #         rank = data["rank"]
+    #         site_name = data["metadata"]["site"].upper()
+    #         data_range = data["data_range"]
+
+    #         # HTML to show when the mouse is hovered over a node
+    #         title = "</br>".join([f"<b>Rank:</b> {str(rank)}", f"<b>Site:</b> {site_name}", f"<b>Data range:</b> {data_range}"])
+
+    #         if rank == 0:
+    #             colour = colour_mapper(rank)
+    #         else:
+    #             # For now just use the highest rank for the color
+    #             highest_rank = sorted(list(rank.keys()))[-1]
+    #             colour = colour_mapper(highest_rank)
 
-#     #         split_key = key.split("_")
-#     #         label = " ".join((split_key[0].upper(), split_key[1].upper(), split_key[2], split_key[3]))
+    #         split_key = key.split("_")
+    #         label = " ".join((split_key[0].upper(), split_key[1].upper(), split_key[2], split_key[3]))
 
-#     #         net.add_node(key, label=label, title=title, color=colour, value=2000)
-#     #         net.add_edge(source=site, to=key)
+    #         net.add_node(key, label=label, title=title, color=colour, value=2000)
+    #         net.add_edge(source=site, to=key)
 
-#     #     return net.show("openghg_rankings.html")
+    #     return net.show("openghg_rankings.html")
```

### Comparing `openghg-0.6.0/openghg/key_notes` & `openghg-1.0.0/openghg/key_notes`

 * *Files identical despite different names*

### Comparing `openghg-0.6.0/openghg/objectstore/_local_store.py` & `openghg-1.0.0/openghg/objectstore/_local_store.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,133 +1,52 @@
 import glob
 import json
 import os
-import threading
 from pathlib import Path
-import shutil
-from typing import Dict, List, Optional, Union
-from uuid import uuid4
-import logging
-import pyvis
+import threading
 from openghg.types import ObjectStoreError
-from openghg.util import read_local_config
+import pyvis
+from uuid import uuid4
+from typing import Dict, List, Optional, Union
 
 rlock = threading.RLock()
 
 __all__ = [
     "delete_object",
-    "get_user_objectstore_path",
-    "get_tutorial_store_path",
+    "get_openghg_local_path",
     "get_all_object_names",
     "get_object_names",
+    "get_bucket",
+    "get_local_bucket",
     "get_object",
     "set_object",
     "set_object_from_json",
     "set_object_from_file",
     "get_object_from_json",
     "exists",
     "visualise_store",
 ]
 
-logger = logging.getLogger("openghg.objectstore")
-logger.setLevel(logging.DEBUG)  # Have to set level for logger as well as handler
-
-
-def get_readable_buckets() -> Dict[str, str]:
-    """Get a dictionary of readable buckets - {store_name: store_path, ...}
-
-    Returns:
-        dict: List of readable buckets
-    """
-    config = read_local_config()
-    object_stores = config["object_store"]
-
-    return {
-        store_name: data["path"] for store_name, data in object_stores.items() if "r" in data["permissions"]
-    }
 
+def get_openghg_local_path() -> Path:
+    """Returns the path to the local OpenGHG object store bucket
 
-def get_writable_buckets() -> Dict[str, str]:
-    """Get a dictionary of writable buckets - {store_name: store_path, ...}
-
-    Returns:
-        dict: Dictionary of buckets this user can write to
-    """
-    config = read_local_config()
-    object_stores = config["object_store"]
-
-    return {
-        store_name: data["path"] for store_name, data in object_stores.items() if "w" in data["permissions"]
-    }
-
-
-def get_writable_bucket(name: Optional[str] = None) -> str:
-    """Get the path to a writable bucket, passing in the name of a bucket if
-    more than one writable bucket available.
-
-    Args:
-        name: Name of writable bucket
     Returns:
-        str: Path to writable bucket
+        pathlib.Path: Path of object store
     """
-    if os.getenv("OPENGHG_TUT_STORE") is not None:
-        return str(get_tutorial_store_path())
-
-    writable_buckets = get_writable_buckets()
-
-    if not writable_buckets:
-        raise ObjectStoreError("No writable object stores found. Check configuration file.")
+    env_path = os.getenv("OPENGHG_PATH")
 
-    if len(writable_buckets) == 1:
-        return next(iter(writable_buckets.values()))
-    elif name is not None:
-        try:
-            bucket_path = writable_buckets[name]
-        except KeyError:
-            raise ObjectStoreError(
-                f"Invalid object store name, stores you can write to are: {', '.join(writable_buckets)}"
-            )
-        return bucket_path
+    if env_path is not None:
+        return Path(env_path)
     else:
-        raise ObjectStoreError(
-            f"More than one writable store, stores you can write to are: {', '.join(writable_buckets)}."
+        raise ValueError(
+            "No environment variable OPENGHG_PATH found, please set to use the local object store"
         )
 
 
-def get_tutorial_store_path() -> Path:
-    """Get the path to the local tutorial store
-
-    Returns:
-        pathlib.Path: Path of tutorial store
-    """
-    return get_user_objectstore_path() / "tutorial_store"
-
-
-# @lru_cache
-def get_user_objectstore_path() -> Path:
-    """Returns the path of the user's local object store
-
-    Returns:
-        pathlib.Path: Path of object store
-    """
-    config = read_local_config()
-    return Path(config["object_store"]["user"]["path"])
-
-
-def get_objectstore_info() -> Dict:
-    """Read the local config file and return the data of each of the object stores the
-    user has access to.
-
-    Returns:
-        dict: Dictionary of object store data
-    """
-    config = read_local_config()
-    return config["object_store"]
-
-
 def get_all_object_names(bucket: str, prefix: Optional[str] = None, without_prefix: bool = False) -> List:
     """Returns the names of all objects in the passed bucket
 
     Args:
         bucket: Bucket path
         prefix: Prefix for keys
         without_prefix: If True don't use prefix
@@ -187,15 +106,15 @@
     key = f"{bucket}/{key}._data"
     try:
         os.remove(key)
     except FileNotFoundError:
         pass
 
 
-def get_object_names(bucket: str, prefix: Optional[str] = None) -> List[str]:
+def get_object_names(bucket: str, prefix: str = None) -> List[str]:
     """List all the keys in the object store
 
     Args:
         bucket: Bucket containing data
     Returns:
         list: List of keys in object store
     """
@@ -205,15 +124,15 @@
 def get_object(bucket: str, key: str) -> bytes:
     """Gets the object at key in the passed bucket
 
     Args:
         bucket: Bucket containing data
         key: Key for data in bucket
     Returns:
-        bytes: Binary data from the store
+        Object: Object from store
     """
     with rlock:
         filepath = Path(f"{bucket}/{key}._data")
 
         if filepath.exists():
             return filepath.read_bytes()
         else:
@@ -269,15 +188,16 @@
     Returns:
         None
     """
     set_object(bucket=bucket, key=key, data=open(filename, "rb").read())
 
 
 def get_object_from_json(bucket: str, key: str) -> Dict[str, Union[str, Dict]]:
-    """Return an object constructed from JSON stored at key.
+    """Removes the daterange from the passed key and uses the reduced
+    key to get an object from the object store.
 
     Args:
         bucket: Bucket containing data
         key: Key for data in bucket
     Returns:
         dict: Dictionary
     """
@@ -297,67 +217,58 @@
         bool: True if key exists in store
     """
     names = get_all_object_names(bucket=bucket, prefix=key)
 
     return len(names) > 0
 
 
-def get_bucket(name: Optional[str] = None) -> str:
-    """Find and return the local object store path. This will return
-    the path to the user's local object store if no name is given.
-
-    Args:
-        name: Object store name in config file
-    Returns:
-        str: Path to object store
+def get_bucket() -> str:
+    """Find and return a new bucket in the object store called
+    'bucket_name'. If 'create_if_needed' is True
+    then the bucket will be created if it doesn't exist. Otherwise,
+    if the bucket does not exist then an exception will be raised.
     """
-    config = read_local_config()
-
-    if name is not None:
-        try:
-            return config["object_store"][name]["path"]
-        except KeyError:
-            raise ObjectStoreError("Invalid object store name.")
-
-    tutorial_store = os.getenv("OPENGHG_TUT_STORE")
-
-    if tutorial_store is not None:
-        return str(get_tutorial_store_path())
+    bucket_path = get_openghg_local_path()
 
-    local_store = get_user_objectstore_path()
+    if not bucket_path.exists():
+        bucket_path.mkdir(parents=True)
 
-    return str(local_store)
+    return str(bucket_path)
 
 
-def clear_object_store() -> None:
-    """Delete the object store. This will only delete a local object store and not
-    a group level or other store. You will be asked for input to confirm the path.
+def get_local_bucket(empty: bool = False) -> str:
+    """Creates and returns a local bucket
 
+    Args:
+        empty: If True return an empty bucket
     Returns:
-        None
+        str: Path to local bucket
     """
-    local_store = str(get_user_objectstore_path())
-    logger.warning(f"You have requested to delete {local_store}.")
+    import shutil
+
+    local_buckets_dir = get_openghg_local_path()
 
-    confirmed_path = input("Please enter the full path of the store: ")
-    if confirmed_path == local_store:
-        shutil.rmtree(local_store, ignore_errors=True)
+    if local_buckets_dir.exists():
+        if empty is True:
+            shutil.rmtree(local_buckets_dir)
+            local_buckets_dir.mkdir(parents=True)
     else:
-        logger.warning("Cannot delete object store.")
+        local_buckets_dir.mkdir(parents=True)
+
+    return str(local_buckets_dir)
 
 
 def query_store() -> Dict:
     """Create a dictionary that can be used to visualise the object store
 
     Returns:
         dict: Dictionary for data to be shown in force graph
     """
-    raise NotImplementedError
-    from openghg.store import ObsSurface
     from openghg.store.base import Datasource
+    from openghg.store import ObsSurface
 
     obs = ObsSurface.load()
 
     datasource_uuids = obs.datasources()
     datasources = (Datasource.load(uuid=uuid, shallow=True) for uuid in datasource_uuids)
 
     data = {}
@@ -380,15 +291,14 @@
     """View the object store using a pyvis force graph.
 
     This function should only be called from within a notebook
 
     Returns:
         pyvis.network.Network
     """
-    raise NotImplementedError
     from addict import Dict as aDict
 
     data = query_store()
 
     net = pyvis.network.Network("800px", "100%", notebook=True)
     net.force_atlas_2based()
```

### Comparing `openghg-0.6.0/openghg/plotting/_footprint.py` & `openghg-1.0.0/openghg/plotting/_footprint.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,27 @@
-from typing import Optional
 from xarray import Dataset
 
 __all__ = ["plot_footprint"]
 
 
-def plot_footprint(
-    data: Dataset, label: Optional[str] = None, vmin: Optional[float] = None, vmax: Optional[float] = None
-) -> None:
+def plot_footprint(data: Dataset, label: str = None, vmin: float = None, vmax: float = None) -> None:
     """Plot a footprint
 
     Args:
         data: Dataset containing fp variable
         label: Label for colourbar
         vmin: Minimum value for colours
         vmax: MinimumMax value for colours
     Returns:
         None
     """
-    import matplotlib.colors as colors
     import matplotlib.pyplot as plt
+    import matplotlib.colors as colors
 
-    _, ax = plt.subplots()
+    fig, ax = plt.subplots()
 
     # Plot footprints as a 2D colour map
     data_fp = data.fp.isel(time=0)  # First time point
     lat = data_fp.lat
     lon = data_fp.lon
     footprint = data_fp.values
```

### Comparing `openghg-0.6.0/openghg/retrieve/_export.py` & `openghg-1.0.0/openghg/retrieve/_export.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,17 +26,16 @@
         write_yaml (bool, default=False): If True write to YAML, otherwise JSON file is written
         date_range (tuple, default=None): Start, end Python datetime objects
     Returns:
         dict: Dictionary for upload to CEDA
 
     """
     import json
-    from pathlib import Path
-
     import yaml
+    from pathlib import Path
     from openghg.util import get_datapath
 
     if filepath:
         filepath = Path(filepath)
 
     compliance_file = "ceda_compliance.json"
     compliance_path = get_datapath(filename=compliance_file)
```

### Comparing `openghg-0.6.0/openghg/retrieve/icos/_retrieve.py` & `openghg-1.0.0/openghg/standardise/surface/_noaa.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,545 +1,687 @@
-from typing import Any, Dict, List, Optional, Union
-from openghg.dataobjects import ObsData
-from openghg.objectstore import get_writable_bucket
-from openghg.util import running_on_hub, load_json
-import openghg_defs
-import logging
+from pathlib import Path
+from typing import Dict, Optional, Union
+from xarray import Dataset
+import numpy as np
 
-logger = logging.getLogger("openghg.retrieve")
-logger.setLevel(logging.DEBUG)  # Have to set level for logger as well as handler
 
-
-def retrieve_atmospheric(
+def parse_noaa(
+    data_filepath: Union[str, Path],
     site: str,
-    species: Optional[Union[str, List]] = None,
+    measurement_type: str,
     inlet: Optional[str] = None,
-    sampling_height: Optional[str] = None,
-    start_date: Optional[str] = None,
-    end_date: Optional[str] = None,
-    force_retrieval: bool = False,
-    data_level: int = 2,
-    dataset_source: Optional[str] = None,
-    store: Optional[str] = None,
-    update_mismatch: str = "never",
-) -> Union[ObsData, List[ObsData], None]:
-    """Retrieve ICOS atmospheric measurement data. If data is found in the object store it is returned. Otherwise
-    data will be retrieved from the ICOS Carbon Portal. Data retrieval from the Carbon Portal may take a short time.
-    If only a single data source is found an ObsData object is returned, if multiple a list of ObsData objects
-    if returned, if nothing then None.
+    network: str = "NOAA",
+    instrument: Optional[str] = None,
+    sampling_period: Optional[str] = None,
+) -> Dict:
+    """Read NOAA data from raw text file or ObsPack NetCDF
 
     Args:
-        site: Site code
-        species: Species name
-        inlet: Height of the inlet for sampling in metres.
-        sampling_height: Alias for inlet
-        start_date: Start date
-        end_date: End date
-        force_retrieval: Force the retrieval of data from the ICOS Carbon Portal
-        data_level: ICOS data level (1, 2)
-        - Data level 1: Near Real Time Data (NRT) or Internal Work data (IW).
-        - Data level 2: The final quality checked ICOS RI data set, published by the CFs,
-                        to be distributed through the Carbon Portal.
-                        This level is the ICOS-data product and free available for users.
-        See https://icos-carbon-portal.github.io/pylib/modules/#stationdatalevelnone
-        dataset_source: Dataset source name, for example ICOS, InGOS, European ObsPack
-        store: Name of object to search/store data to
-        update_mismatch: This determines how mismatches between the "metadata" derived from
-            stored data and "attributes" derived from ICOS Header are handled.
-            This includes the options:
-                - "never" - don't update mismatches and raise an AttrMismatchError
-                - "from_source" / "attributes" - update mismatches based on attributes from ICOS Header
-                - "from_definition" / "metadata" - update mismatches based on input metadata
+        data_filepath: Data filepath
+        site: Three letter site code
+        inlet: Inlet height, if no height use measurement type e.g. flask
+        measurement_type: One of ("flask", "insitu", "pfp")
+        network: Network, defaults to NOAA
+        instrument: Instrument name
+        sampling_period: Sampling period
     Returns:
-        ObsData, list[ObsData] or None
+        dict: Dictionary of data and metadata
     """
-    return retrieve(
-        site=site,
-        species=species,
-        inlet=inlet,
-        sampling_height=sampling_height,
-        start_date=start_date,
-        end_date=end_date,
-        force_retrieval=force_retrieval,
-        data_level=data_level,
-        dataset_source=dataset_source,
-        update_mismatch=update_mismatch,
-        store=store,
-    )
+    if sampling_period is None:
+        sampling_period = "NOT_SET"
 
+    sampling_period = str(sampling_period)
 
-def retrieve(**kwargs: Any) -> Union[ObsData, List[ObsData], None]:
-    """Retrieve data from the ICOS Carbon Portal. If data is found in the local object store
-    it will be retrieved from there first.
+    file_extension = Path(data_filepath).suffix
+
+    if file_extension == ".nc":
+        return _read_obspack(
+            data_filepath=data_filepath,
+            site=site,
+            inlet=inlet,
+            measurement_type=measurement_type,
+            instrument=instrument,
+            sampling_period=sampling_period,
+        )
+    else:
+        return _read_raw_file(
+            data_filepath=data_filepath,
+            site=site,
+            inlet=inlet,
+            measurement_type=measurement_type,
+            instrument=instrument,
+            sampling_period=sampling_period,
+        )
 
-    This function detects the running environment and routes the call
-    to either the cloud or local search function.
 
-    Example / commonly used arguments are given below.
+def _format_inlet(inlet: Union[str, float, int]) -> str:
+    """
+    Output inlet name in expected format. This will include 1 decimal place for floats with a fractional component
+    and 0 decimal places otherwise.
 
     Args:
-        site: Site code
-        species: Species name
-        start_date: Start date
-        end_date: End date
-        inlet: Height of the inlet for sampling in metres.
-        sampling_height: Alias for inlet
-        force_retrieval: Force the retrieval of data from the ICOS Carbon Portal
-        data_level: ICOS data level (1, 2)
-        - Data level 1: Near Real Time Data (NRT) or Internal Work data (IW).
-        - Data level 2: The final quality checked ICOS RI data set, published by the CFs,
-                        to be distributed through the Carbon Portal.
-                        This level is the ICOS-data product and free available for users.
-        See https://icos-carbon-portal.github.io/pylib/modules/#stationdatalevelnone
-        update_mismatch: This determines how mismatches between the "metadata" derived from
-            stored data and "attributes" derived from ICOS Header are handled.
-            This includes the options:
-                - "never" - don't update mismatches and raise an AttrMismatchError
-                - "from_source" / "attributes" - update mismatches based on attributes from ICOS Header
-                - "from_definition" / "metadata" - update mismatches based on input metadata
+        inlet : Inlet value. This can be a string as long as this can be converted directly to a float
+
     Returns:
-        ObsData, list[ObsData] or None
+        str : Formatted string of inlet name
+
+    Examples:
+        >>> _format_inlet(40)
+        "40m"
+        >>> _format_inlet("10.0")
+        "10m"
+        >>> _format_inlet(2.511432)
+        "2.5m"
     """
-    from io import BytesIO
-    from xarray import load_dataset
-    from openghg.cloud import call_function, unpackage
+    if isinstance(inlet, str):
+        try:
+            inlet_value = float(inlet)
+        except ValueError:
+            inlet_values_str = inlet.split("-")
+            try:
+                inlet_values = [float(value) for value in inlet_values_str]
+            except ValueError:
+                raise ValueError("Unable to convert inlet {inlet} to a float")
+            else:
+                inlet_value = np.mean(inlet_values)
+    else:
+        inlet_value = inlet
 
-    # The hub is the only place we want to make remote calls
-    if running_on_hub():
-        post_data: Dict[str, Union[str, Dict]] = {}
-        post_data["function"] = "retrieve_icos"
-        post_data["search_terms"] = kwargs
+    if inlet_value % 1 == 0:
+        inlet_str = f"{inlet_value:.0f}m"
+    else:
+        inlet_str = f"{inlet_value:.1f}m"
 
-        call_result = call_function(data=post_data)
+    return inlet_str
 
-        content = call_result["content"]
-        found = content["found"]
 
-        if not found:
-            return None
+def _standarise_variables(obspack_ds: Dataset, species: str) -> Dataset:
+    """
+    Converts data from NOAA ObsPack dataset into our standardised variables to be stored within the object store.
+    The species is also needed so this name can be used to label the variables in the new dataset.
 
-        observations = content["data"]
+    Expects inputs with: "value", "value_std_dev" or "value_unc", "nvalue" as per NOAA ObsPack standard.
 
-        obs_data = []
-        for package in observations.values():
-            unpackaged = unpackage(data=package)
-            buf = BytesIO(unpackaged["data"])
-            ds = load_dataset(buf)
-            obs = ObsData(data=ds, metadata=unpackaged["metadata"])
+    Args:
+        obspack_ds : Dataset derived from a netcdf file within the NOAA obspack
+        species : Standardised species name (e.g. "ch4")
 
-            obs_data.append(obs)
+    Returns:
+        Dataset : Standardised dataset with variables extracted and renamed
 
-        if len(obs_data) == 1:
-            return obs_data[0]
-        else:
-            return obs_data
-    else:
-        return local_retrieve(**kwargs)
+    Example output:
+        For species = "ch4":
+            xarray.Dataset("ch4":[...]
+                           "ch4_variability":[...]
+                           "ch4_number_of_observations": [...])
+    """
 
+    processed_ds = obspack_ds.copy()
+
+    # Rename variables to match our internal standard
+    # "value_std_dev" --> f"{species}_variability"
+    # "value_unc" --> ??
+    # TODO: Clarify what "value_unc" should be renamed to
+
+    variable_names = {
+        "value": species,
+        "value_std_dev": f"{species}_variability",
+        "value_unc": f"{species}_variability",  # May need to be updated
+        "nvalue": f"{species}_number_of_observations",
+    }
+
+    to_extract = [name for name in variable_names.keys() if name in obspack_ds]
+
+    # For the error variables we only want to take one set of values from the
+    # obspack dataset but multiple variables may be available.
+    # If multiple are present, combine these together and only extract one
+    error_names = ["value_std_dev", "value_unc"]
+    error_variables = [name for name in error_names if name in to_extract]
+
+    if len(error_variables) > 1:
+        main_ev = error_variables[0]  # Treat first item in the list at the one to keep
+
+        history_attr = "history"
+        processed_ds[main_ev].attrs[history_attr] = f"Merged {main_ev} variable from original file with "
+
+        for ev in error_variables[1:]:
+            # Combine details from additional additional error variable with main variable
+            variable = processed_ds[main_ev]
+            new_variable = processed_ds[ev]
+
+            # Update Dataset and add details within attributes
+            updated_variable = variable.combine_first(new_variable)
+            processed_ds[main_ev] = updated_variable
+            processed_ds[main_ev].attrs[history_attr] += f"{ev}, "
+
+            # Remove this extra variables from the list of variables to extract from the dataset
+            to_extract.remove(ev)
+
+    # Create dictionary of names to convert obspack ds to our format
+    name_dict = {name: key for name, key in variable_names.items() if name in to_extract}
+
+    if not to_extract:
+        wanted = variable_names.keys()
+        raise ValueError(
+            f"No valid data variables columns found in obspack dataset. We expect the following data variables in the passed NetCDF: {wanted}"
+        )
+
+    # Grab only the variables we want to keep and rename these
+    processed_ds = processed_ds[to_extract]
+    processed_ds = processed_ds.rename(name_dict)
+    processed_ds = processed_ds.sortby("time")
+
+    return processed_ds
 
-def local_retrieve(
-    site: str,
-    species: Optional[Union[str, List]] = None,
-    inlet: Optional[str] = None,
-    sampling_height: Optional[str] = None,
-    start_date: Optional[str] = None,
-    end_date: Optional[str] = None,
-    force_retrieval: bool = False,
-    data_level: int = 2,
-    dataset_source: Optional[str] = None,
-    store: Optional[str] = None,
-    update_mismatch: str = "never",
-    **kwargs: Any,
-) -> Union[ObsData, List[ObsData], None]:
-    """Retrieve ICOS atmospheric measurement data. If data is found in the object store it is returned. Otherwise
-    data will be retrieved from the ICOS Carbon Portal. Data retrieval from the Carbon Portal may take a short time.
-    If only a single data source is found an ObsData object is returned, if multiple a list of ObsData objects
-    if returned, if nothing then None.
+
+def _split_inlets(obspack_ds: Dataset, attributes: Dict, metadata: Dict, inlet: Optional[str] = None) -> Dict:
+    """
+    Splits the overall dataset by different inlet values, if present. The expected dataset input should be from the NOAA ObsPack.
 
     Args:
-        site: Site code
-        species: Species name
-        inlet: Height of the inlet for sampling in metres.
-        sampling_height: Alias for inlet
-        start_date: Start date
-        end_date: End date
-        force_retrieval: Force the retrieval of data from the ICOS Carbon Portal
-        data_level: ICOS data level (1, 2)
-        - Data level 1: Near Real Time Data (NRT) or Internal Work data (IW).
-        - Data level 2: The final quality checked ICOS RI data set, published by the CFs,
-                        to be distributed through the Carbon Portal.
-                        This level is the ICOS-data product and free available for users.
-        See https://icos-carbon-portal.github.io/pylib/modules/#stationdatalevelnone
-        dataset_source: Dataset source name, for example ICOS, InGOS, European ObsPack
-        store: Name of object to search/store data to
-        update_mismatch: This determines how mismatches between the "metadata" derived from
-            stored data and "attributes" derived from ICOS Header are handled.
-            This includes the options:
-                - "never" - don't update mismatches and raise an AttrMismatchError
-                - "from_source" / "attributes" - update mismatches based on attributes from ICOS Header
-                - "from_definition" / "metadata" - update mismatches based on input metadata
+        obspack_ds : Dataset derived from a netcdf file within the NOAA obspack
+        attributes: Attributes extracted from the NOAA obspack. Should contain at least "species" and "measurement_type"
+        metadata: Metadata to store alongside standardised data
+
     Returns:
-        ObsData, list[ObsData] or None
+        Dict: gas data containing "data", "metadata", "attributes" for each inlet
+
+    Example output:
+        {"ch4": {"data": xr.Dataset(...), "attributes": {...}, "metadata": {...}}}
+        or
+        {"ch4_40m": {"data": xr.Dataset(...), "attributes": {...}, "metadata": {...}}, "ch4_60m": {...}, ...}
+
     """
-    from openghg.retrieve import search_surface
-    from openghg.store import ObsSurface
-    from openghg.util import to_lowercase
-
-    if not 1 <= data_level <= 2:
-        logger.error("Error: data level must be 1 or 2.")
-
-    if sampling_height and inlet is None:
-        inlet = sampling_height
-    elif sampling_height and inlet:
-        logger.warning(f"Both sampling height and inlet specified. Using inlet value of {inlet}")
-
-    # NOTE - we skip ranking here, will we be ranking ICOS data?
-    results = search_surface(
-        site=site,
-        species=species,
-        inlet=inlet,
-        network="ICOS",
-        data_source="icoscp",
-        start_date=start_date,
-        end_date=end_date,
-        icos_data_level=data_level,
-        dataset_source=dataset_source,
-        store=store,
-    )
 
-    if results and not force_retrieval:
-        obs_data = results.retrieve_all()
-    else:
-        # We'll also need to check we have current data
-        standardised_data = _retrieve_remote(
-            site=site,
-            species=species,
-            data_level=data_level,
-            dataset_source=dataset_source,
-            inlet=inlet,
-            sampling_height=sampling_height,
-            update_mismatch=update_mismatch,
-        )
+    orig_attrs = obspack_ds.attrs
+    species = attributes["species"]
+    measurement_type = attributes["measurement_type"]
+
+    height_var = "intake_height"
+
+    # Check whether the input data contains different inlet height values for each data point ("intake_height" data variable)
+    # If so we need to select the data for each inlet and indicate this is a separate Datasource
+    # Each data key is labelled based on the species and the inlet (if needed)
+
+    gas_data: Dict[str, Dict] = {}
+    if height_var in obspack_ds.data_vars:
+
+        if inlet is not None:
+            # TODO: Add to logging?
+            print(
+                f"WARNING: Ignoring inlet value of {inlet} since file has each data point has an associated height (contains 'intake_height' variable)"
+            )
+
+        # Group dataset by the height values
+        # Note: could use ds.groupby_bins(...) if necessary if there are lots of small height differences to group these
+        obspack_ds_grouped = obspack_ds.groupby(height_var)
+        num_groups = len(obspack_ds_grouped.groups)
+
+        # For each group standardise and store with id based on species and inlet height
+        for ht, obspack_ds_ht in obspack_ds_grouped:
+
+            # Creating id keys of the form "<species>_<inlet>" e.g. "ch4_40m" or "co_12.5m"
+            inlet_str = _format_inlet(ht)
+            inlet_num_str = inlet_str.strip("m")
+
+            if num_groups > 1:
+                id_key = f"{species}_{inlet_str}"
+            else:
+                id_key = f"{species}"
+
+            # Extract wanted variables and convert to standardised names
+            standarised_ds = _standarise_variables(obspack_ds_ht, species)
+
+            gas_data[id_key] = {}
+            gas_data[id_key]["data"] = standarised_ds
+
+            # Add inlet details to attributes and metadata
+            attrs_copy = attributes.copy()
+            meta_copy = metadata.copy()
 
-        if standardised_data is None:
-            return None
+            attrs_copy["inlet"] = inlet_str
+            attrs_copy["inlet_height_magl"] = inlet_num_str
+            meta_copy["inlet"] = inlet_str
+            meta_copy["inlet_height_magl"] = inlet_num_str
 
-        bucket = get_writable_bucket(name=store)
-        with ObsSurface(bucket=bucket) as obs:
-            obs.store_data(data=standardised_data)
-
-        # Create the expected ObsData type
-        obs_data = []
-        for data in standardised_data.values():
-            measurement_data = data["data"]
-            # These contain URLs that are case sensitive so skip lowercasing these
-            skip_keys = ["citation_string", "instrument_data", "dobj_pid", "dataset_source"]
-            metadata = to_lowercase(data["metadata"], skip_keys=skip_keys)
-            obs_data.append(ObsData(data=measurement_data, metadata=metadata))
+            gas_data[id_key]["metadata"] = meta_copy
+            gas_data[id_key]["attributes"] = attrs_copy
 
-    if isinstance(obs_data, list) and len(obs_data) == 1:
-        return obs_data[0]
     else:
-        return obs_data
+        try:
+            inlet_value = orig_attrs["dataset_intake_ht"]
+        except KeyError:
+            inlet_from_file = None
+        else:
+            inlet_from_file = _format_inlet(inlet_value)
+
+        if measurement_type == "flask":
+            inlet_from_file = "flask"
+
+        # Check inlet from file against any provided inlet
+        if inlet is None and inlet_from_file:
+            inlet = inlet_from_file
+        elif inlet is not None and inlet_from_file:
+            if inlet != inlet_from_file:
+                print(
+                    f"WARNING: Provided inlet {inlet} does not match inlet derived from the input file: {inlet_from_file}"
+                )
+        else:
+            raise ValueError(
+                "Unable to derive inlet from NOAA file. Please pass as an input. If flask data pass 'flask' as inlet."
+            )
 
+        id_key = f"{species}"
 
-def _retrieve_remote(
+        if inlet != "flask":
+            inlet_num_str = inlet.strip("m")
+        else:
+            inlet_num_str = ""
+
+        metadata["inlet"] = inlet
+        metadata["inlet_height_magl"] = inlet_num_str
+        attributes["inlet"] = inlet
+        attributes["inlet_height_magl"] = inlet_num_str
+
+        standardised_ds = _standarise_variables(obspack_ds, species)
+
+        gas_data[id_key] = {"data": standardised_ds, "metadata": metadata, "attributes": attributes}
+
+    return gas_data
+
+
+def _read_obspack(
+    data_filepath: Union[str, Path],
     site: str,
-    data_level: int,
-    species: Optional[Union[str, List]] = None,
+    sampling_period: str,
+    measurement_type: str,
     inlet: Optional[str] = None,
-    sampling_height: Optional[str] = None,
-    dataset_source: Optional[str] = None,
-    update_mismatch: str = "never",
-) -> Optional[Dict]:
-    """Retrieve ICOS data from the ICOS Carbon Portal and standardise it into
-    a format expected by OpenGHG. A dictionary of metadata and Datasets
+    instrument: Optional[str] = None,
+) -> Dict[str, Dict]:
+    """Read NOAA ObsPack NetCDF files
 
     Args:
-        site: ICOS site code, for site codes see
-        https://www.icos-cp.eu/observations/atmosphere/stations
-        data_level: ICOS data level (1, 2)
-        - Data level 1: Near Real Time Data (NRT) or Internal Work data (IW).
-        - Data level 2: The final quality checked ICOS RI data set, published by the CFs,
-                        to be distributed through the Carbon Portal.
-                        This level is the ICOS-data product and free available for users.
-        See https://icos-carbon-portal.github.io/pylib/modules/#stationdatalevelnone
-        species: Species name
-        inlet: Height of the inlet for sampling in metres.
-        sampling_height: Alias for inlet
-        dataset_source: Dataset source name, for example ICOS, InGOS, European ObsPack
-        update_mismatch: This determines how mismatches between the "metadata" derived from
-            stored data and "attributes" derived from ICOS Header are handled.
-            This includes the options:
-                - "never" - don't update mismatches and raise an AttrMismatchError
-                - "from_source" / "attributes" - update mismatches based on attributes from ICOS Header
-                - "from_definition" / "metadata" - update mismatches based on input metadata
+        data_filepath: Path to file
+        site: Three letter site code
+        sampling_period: Sampling period
+        measurement_type: One of flask, insitu or pfp
+        inlet: Inlet height, if no height use measurement type e.g. flask
+        instrument: Instrument name
+
     Returns:
-        dict or None: Dictionary of processed data and metadata if found
+        dict: Dictionary of results
     """
-    # icoscp isn't available to conda so we've got to resort to this for now
+    import xarray as xr
+    from openghg.util import clean_string
+    from openghg.standardise.meta import assign_attributes
+
+    valid_types = ("flask", "insitu", "pfp")
+
+    if measurement_type not in valid_types:
+        raise ValueError(f"measurement_type must be one of {valid_types}")
+
+    obspack_ds = xr.open_dataset(data_filepath)
+    orig_attrs = obspack_ds.attrs
+
+    # Want to find and drop any duplicate time values for the original dataset
+    # Using xarray directly we have to do in a slightly convoluted way as this is not well built
+    # into the xarray workflow yet - https://github.com/pydata/xarray/pull/5239
+    # - can use da.drop_duplicates() but only on one variable at a time and not on the whole Dataset
+    # This method keeps attributes for each of the variables including units
+
+    # The dimension within the original dataset is called "obs" and has no associated coordinates
+    # Extract time from original Dataset (dimension is "obs")
+    time = obspack_ds.time
+
+    # To keep associated "obs" dimension, need to assign coordinate values to this (just 0, len(obs))
+    time = time.assign_coords(obs=obspack_ds.obs)
+
+    # Make "time" the primary dimension (while retaining "obs") and add "time" values as coordinates
+    time = time.swap_dims(dims_dict={"obs": "time"})
+    time = time.assign_coords(time=time)
+
+    # Drop any duplicate time values and extract the associated "obs" values
+    # TODO: Work out what to do with duplicates - may be genuine multiple measurements
+    time_unique = time.drop_duplicates(dim="time", keep="first")
+    obs_unique = time_unique.obs
+
+    # Use these obs values to filter the original dataset to remove any repeated times
+    processed_ds = obspack_ds.sel(obs=obs_unique)
+    processed_ds = processed_ds.set_coords(["time"])
+
+    # Estimate sampling period using metadata and midpoint time
+    if sampling_period == "NOT_SET":
+        sampling_period_estimate = _estimate_sampling_period(obspack_ds)
+    else:
+        sampling_period_estimate = -1.0
+
+    species = clean_string(obspack_ds.attrs["dataset_parameter"])
+    network = "NOAA"
+
     try:
-        from icoscp.cpb.dobj import Dobj  # type: ignore
-        from icoscp.station import station  # type: ignore
-    except ImportError:
-        raise ImportError(
-            "Cannot import icoscp, if you've installed OpenGHG using conda please run: pip install icoscp"
-        )
+        # Extract units attribute from value data variable
+        units = processed_ds["value"].units
+    except (KeyError, AttributeError):
+        print("Unable to extract units from 'value' within input dataset")
+    else:
+        if units == "mol mol-1":
+            units = "1"
+        elif units == "millimol mol-1":
+            units = "1e-3"
+        elif units == "micromol mol-1":
+            units = "1e-6"
+        elif units in ["nmol mol-1", "nanomol mol-1"]:
+            units = "1e-9"
+        elif units == "pmol mol-1":
+            units = "1e-12"
+        else:
+            print(f"Using unit {units} directly")
+            # raise ValueError(f"Did not recognise input units from file: {units}")
 
-    import re
-    from openghg.standardise.meta import assign_attributes
-    from openghg.util import format_inlet
-    from pandas import to_datetime
+    metadata = {}
+    metadata["site"] = site
+    metadata["network"] = network
+    metadata["measurement_type"] = measurement_type
+    metadata["species"] = species
+    metadata["units"] = units
+    metadata["sampling_period"] = sampling_period
+
+    # Add additional sampling_period_estimate if sampling_period is not set
+    if sampling_period_estimate >= 0.0:
+        metadata["sampling_period_estimate"] = str(
+            sampling_period_estimate
+        )  # convert to string to keep consistent with "sampling_period"
+
+    # Add instrument if present
+    if instrument is not None:
+        metadata["instrument"] = instrument
+    else:
+        metadata["instrument"] = orig_attrs.get("instrument", "NOT_SET")
 
-    if species is None:
-        species = ["CO", "CO2", "CH4"]
+    # Add data owner details, station position and calibration scale, if present
+    metadata["data_owner"] = orig_attrs.get("provider_1_name", "NOT_SET")
+    metadata["data_owner_email"] = orig_attrs.get("provider_1_email", "NOT_SET")
+    metadata["station_longitude"] = orig_attrs.get("site_longitude", "NOT_SET")
+    metadata["station_latitude"] = orig_attrs.get("site_latitude", "NOT_SET")
+    metadata["calibration_scale"] = orig_attrs.get("dataset_calibration_scale", "NOT_SET")
+
+    # Create attributes with copy of metadata values
+    attributes = metadata.copy()
+
+    # TODO: At the moment all attributes from the NOAA ObsPack are being copied
+    # plus any variables we're adding - decide if we want to reduce this
+    attributes.update(orig_attrs)
+
+    # expected_keys = {
+    #     "site",
+    #     "species",
+    #     "inlet",
+    #     "instrument",
+    #     "sampling_period",
+    #     "calibration_scale",
+    #     "station_longitude",
+    #     "station_latitude",
+    # }
+
+    gas_data = _split_inlets(processed_ds, attributes, metadata, inlet=inlet)
 
-    if not isinstance(species, list):
-        species = [species]
+    gas_data = assign_attributes(data=gas_data, site=site, network=network)
 
-    if sampling_height and inlet is None:
-        inlet = sampling_height
-    elif sampling_height and inlet:
-        logger.warning(f"Both sampling height and inlet specified. Using inlet value of {inlet}")
-
-    # We should first check if it's stored in the object store
-    # Will need to make sure ObsSurface can accept the datasets we
-    # create from the ICOS data
-    stat = station.get(stationId=site.upper())
-
-    if not stat.valid:
-        logger.error("Please check you have passed a valid ICOS site.")
-        return None
-
-    data_pids = stat.data(level=data_level)
-
-    # We want to get the PIDs of the data for each species here
-    species_upper = [s.upper() for s in species]
-    # For this see https://stackoverflow.com/a/55335207
-    search_str = r"\b(?:{})\b".format("|".join(map(re.escape, species_upper)))
-    # Now filter the dataframe so we can extract the PIDS
-    filtered_sources = data_pids[data_pids["specLabel"].str.contains(search_str)]
-
-    if inlet is not None:
-        inlet = str(float(inlet.rstrip("m")))
-        height_filter = [inlet in str(x) for x in filtered_sources["samplingheight"]]
-        filtered_sources = filtered_sources[height_filter]
-
-    if filtered_sources.empty:
-        logger.error(
-            f"No sources found for {species} at {site}. Please check with the ICOS Carbon Portal that this data is available."
-        )
-        return None
+    return gas_data
 
-    # Now extract the PIDs along with some data about them
-    dobj_urls = filtered_sources["dobj"].tolist()
 
-    # Load our site metadata for a few things like the station's long_name that
-    # isn't in the ICOS metadata in the way we want it at the momenet - 2023-03-20
-    site_info_fpath = openghg_defs.site_info_file
-    openghg_site_metadata = load_json(path=site_info_fpath)
-
-    standardised_data: Dict[str, Dict] = {}
-
-    for n, dobj_url in enumerate(dobj_urls):
-        dobj = Dobj(dobj_url)
-        logger.info(f"Retrieving {dobj_url}...")
-        # We've got to jump through some hoops here to try and avoid the NOAA
-        # ObsPack GlobalView data
-        try:
-            if "globalview" in dobj.meta["references"]["doi"]["titles"][0]["title"].lower():
-                logger.info(f"Skipping {dobj_url} as ObsPack GlobalView detected.")
-                continue
-        except KeyError:
-            pass
+def _read_raw_file(
+    data_filepath: Union[str, Path],
+    site: str,
+    sampling_period: str,
+    measurement_type: str,
+    inlet: Optional[str] = None,
+    instrument: Optional[str] = None,
+) -> Dict:
+    """Reads NOAA data files and returns a dictionary of processed
+    data and metadata.
 
-        try:
-            dobj_dataset_source = dobj.meta["specification"]["project"]["self"]["label"]
-        except KeyError:
-            dobj_dataset_source = "NA"
-            logger.warning("Unable to read project information from dobj.")
+    Args:
+        data_filepath: Path of file to load
+        site: Site name
+        sampling_period: Sampling period
+        measurement_type: One of flask, insitu or pfp
+        inlet: Inlet height, if no height use measurement type e.g. flask
+        instrument: Instrument name
 
-        if dataset_source is not None and dataset_source.lower() != dobj_dataset_source.lower():
-            continue
+    Returns:
+        list: UUIDs of Datasources data has been assigned to
+    """
+    from openghg.standardise.meta import assign_attributes
 
-        # We need to pull the data down as .info (metadata) is populated further on this step
-        dataframe = dobj.get()
-        # This is the metadata, dobj.info and dobj.meta are equal
-        dobj_info = dobj.meta
+    # TODO: Added this for now to make sure inlet is specified but may be able to remove
+    # if this can be derived from the data format.
+    if inlet is None:
+        raise ValueError("Inlet must be specified to derive data from NOAA raw (txt) files.")
 
-        attributes = {}
+    data_filepath = Path(data_filepath)
+    filename = data_filepath.name
 
-        specific_info = dobj_info["specificInfo"]
-        col_data = specific_info["columns"]
+    species = filename.split("_")[0].lower()
 
-        # Get the species this dobj holds information for
-        not_the_species = {"TIMESTAMP", "Flag", "NbPoints", "Stdev"}
-        species_info = next(i for i in col_data if i["label"] not in not_the_species)
+    source_name = data_filepath.stem
+    source_name = source_name.split("-")[0]
 
-        measurement_type = species_info["valueType"]["self"]["label"].lower()
-        units = species_info["valueType"]["unit"].lower()
-        the_species = species_info["label"]
+    gas_data = _read_raw_data(
+        data_filepath=data_filepath,
+        inlet=inlet,
+        species=species,
+        measurement_type=measurement_type,
+        sampling_period=sampling_period,
+    )
 
-        species_info = next(item for item in col_data if str(item["label"]).lower() == the_species.lower())
+    gas_data = assign_attributes(data=gas_data, site=site, network="NOAA")
 
-        attributes["species"] = the_species
-        acq_data = specific_info["acquisition"]
-        station_data = acq_data["station"]
+    return gas_data
 
-        to_store: Dict[str, Any] = {}
-        try:
-            instrument_attributes = acq_data["instrument"]
-        except KeyError:
-            to_store["instrument"] = "NA"
-            to_store["instrument_data"] = "NA"
-        else:
-            # Do some tidying of the instrument attributes
-            instruments = set()
-            cleaned_instrument_attributes = []
-
-            if not isinstance(instrument_attributes, list):
-                instrument_attributes = [instrument_attributes]
-
-            for inst in instrument_attributes:
-                instrument_name = inst["label"]
-                instruments.add(instrument_name)
-                uri = inst["uri"]
 
-                cleaned_instrument_attributes.extend([instrument_name, uri])
+def _read_raw_data(
+    data_filepath: Path,
+    species: str,
+    inlet: str,
+    sampling_period: str,
+    measurement_type: str = "flask",
+) -> Dict:
+    """Separates the gases stored in the dataframe in
+    separate dataframes and returns a dictionary of gases
+    with an assigned UUID as gas:UUID and a list of the processed
+    dataframes
 
-            if len(instruments) == 1:
-                instrument = instruments.pop()
-            else:
-                instrument = "multiple"
+    Args:
+        data_filepath: Path of datafile
+        species: Species string such as CH4, CO
+        measurement_type: Type of measurements e.g. flask
+    Returns:
+        dict: Dictionary containing attributes, data and metadata keys
+    """
+    from openghg.util import clean_string, read_header, load_json
+    from pandas import read_csv, Timestamp
 
-            to_store["instrument"] = instrument
-            to_store["instrument_data"] = cleaned_instrument_attributes
+    header = read_header(filepath=data_filepath)
 
-        attributes.update(to_store)
+    column_names = header[-1][14:].split()
 
-        attributes["site"] = station_data["id"]
-        attributes["measurement_type"] = measurement_type
-        # TODO: Remove this from general attributes but make sure this is
-        # included as a specific value on the appropriate variable.
-        attributes["units"] = units
+    def date_parser(year: str, month: str, day: str, hour: str, minute: str, second: str) -> Timestamp:
+        return Timestamp(year, month, day, hour, minute, second)
+
+    date_parsing = {
+        "time": [
+            "sample_year",
+            "sample_month",
+            "sample_day",
+            "sample_hour",
+            "sample_minute",
+            "sample_seconds",
+        ]
+    }
+
+    data_types = {
+        "sample_year": int,
+        "sample_month": int,
+        "sample_day": int,
+        "sample_hour": int,
+        "sample_minute": int,
+        "sample_seconds": int,
+    }
+
+    # Number of header lines to skip
+    n_skip = len(header)
+
+    data = read_csv(
+        data_filepath,
+        skiprows=n_skip,
+        names=column_names,
+        sep=r"\s+",
+        dtype=data_types,
+        parse_dates=date_parsing,
+        date_parser=date_parser,
+        index_col="time",
+        skipinitialspace=True,
+    )
 
-        _sampling_height = acq_data["samplingHeight"]
-        attributes["sampling_height"] = format_inlet(_sampling_height, key_name="sampling_height")
-        attributes["sampling_height_units"] = "metres"
-        attributes["inlet"] = format_inlet(_sampling_height, key_name="inlet")
-        attributes["inlet_height_magl"] = format_inlet(_sampling_height, key_name="inlet_height_magl")
+    # Drop duplicates
+    data = data.loc[~data.index.duplicated(keep="first")]
 
-        loc_data = station_data["location"]
+    # Check if the index is sorted
+    if not data.index.is_monotonic_increasing:
+        data = data.sort_index()
+
+    # Read the site code from the Dataframe
+    site = str(data["sample_site_code"][0]).upper()
+
+    site_data = load_json("acrg_site_info.json")
+    # If this isn't a site we recognize try and read it from the filename
+    if site not in site_data:
+        site = str(data_filepath.name).split("_")[1].upper()
+
+        if site not in site_data:
+            raise ValueError(f"The site {site} is not recognized.")
+
+    if species is not None:
+        # If we're passed a species ensure that it is in fact the correct species
+        data_species = str(data["parameter_formula"].values[0]).lower()
+
+        passed_species = species.lower()
+        if data_species != passed_species:
+            raise ValueError(
+                f"Mismatch between passed species ({passed_species}) and species read from data ({data_species})"
+            )
+
+    species = species.upper()
+
+    flag = []
+    selection_flag = []
+    for flag_str in data.analysis_flag:
+        flag.append(flag_str[0] == ".")
+        selection_flag.append(int(flag_str[1] != "."))
+
+    combined_data = {}
+
+    data[species + "_status_flag"] = flag
+    data[species + "_selection_flag"] = selection_flag
+
+    data = data[data[species + "_status_flag"]]
+
+    data = data[
+        [
+            "sample_latitude",
+            "sample_longitude",
+            "sample_altitude",
+            "analysis_value",
+            "analysis_uncertainty",
+            species + "_selection_flag",
+        ]
+    ]
+
+    rename_dict = {
+        "analysis_value": species,
+        "analysis_uncertainty": species + "_repeatability",
+        "sample_longitude": "longitude",
+        "sample_latitude": "latitude",
+        "sample_altitude": "altitude",
+    }
+
+    data = data.rename(columns=rename_dict, inplace=False)
+    data = data.to_xarray()
+
+    # TODO  - this could do with a better name
+    noaa_params = load_json("attributes.json")["NOAA"]
+
+    site_attributes = noaa_params["global_attributes"]
+    site_attributes["inlet_height_magl"] = "NA"
+    site_attributes["instrument"] = noaa_params["instrument"][species.upper()]
+    site_attributes["sampling_period"] = sampling_period
+
+    metadata = {}
+    metadata["species"] = clean_string(species)
+    metadata["site"] = site
+    metadata["measurement_type"] = measurement_type
+    metadata["network"] = "NOAA"
+    metadata["inlet"] = inlet
+    metadata["sampling_period"] = sampling_period
+    metadata["instrument"] = noaa_params["instrument"][species.upper()]
+
+    combined_data[species.lower()] = {
+        "metadata": metadata,
+        "data": data,
+        "attributes": site_attributes,
+    }
 
-        attributes["station_long_name"] = loc_data["label"]
-        attributes["station_latitude"] = str(loc_data["lat"])
-        attributes["station_longitude"] = str(loc_data["lon"])
+    return combined_data
 
-        # 03/05/2023: Updated attributes to include altitude for "station_height_masl" explicitly.
-        # attributes["station_altitude"] = format_inlet(loc_data["alt"], key_name="station_altitude")
-        # attributes["station_height_masl"] = format_inlet(str(stat.eas), key_name="station_height_masl")
-        attributes["station_height_masl"] = format_inlet(loc_data["alt"], key_name="station_height_masl")
 
-        attributes["data_owner"] = f"{stat.firstName} {stat.lastName}"
-        attributes["data_owner_email"] = str(stat.email)
+def _estimate_sampling_period(obspack_ds: Dataset, min_estimate: float = 10.0) -> float:
+    """
+    Estimate the sampling period for the NOAA data using either the "data_selection_tag"
+    attribute (this sometimes contains useful information such as "HourlyData") or by using
+    the midpoint_time within the data itself.
 
-        attributes["citation_string"] = dobj_info["references"]["citationString"]
-        attributes["licence_name"] = dobj_info["references"]["licence"]["name"]
-        attributes["licence_info"] = dobj_info["references"]["licence"]["url"]
+    Note: midpoint_time often seems to match start_time implying instantaneous measurement
+    or that this value has not been correctly included.
 
-        metadata = {}
+    If the estimate is less than `min_estimate` the estimate sampling period will be set to
+    this value.
 
-        network = "ICOS"
+    Args:
+        obspack_ds : Dataset of raw obs pack file opened as an xarray Dataset
+        min_estimate : Minimum sampling period estimate to use in seconds.
 
-        try:
-            site_info = openghg_site_metadata[site.upper()][network]
-        except KeyError:
-            pass
-        else:
-            metadata["station_long_name"] = site_info["long_name"]
-            metadata["station_latitude"] = site_info["latitude"]
-            metadata["station_longitude"] = site_info["longitude"]
-
-        # Add some values directly for attributes (for now)
-        metadata["species"] = attributes["species"]
-
-        # Add ICOS in directly here for now
-        additional_data = {}
-        additional_data["network"] = network
-        additional_data["data_type"] = "surface"
-        additional_data["data_source"] = "icoscp"
-        additional_data["source_format"] = "icos"
-        additional_data["icos_data_level"] = str(data_level)
-        additional_data["dataset_source"] = dobj_dataset_source
-        additional_data["site"] = site
-
-        attributes.update(additional_data)
-        metadata.update(additional_data)
-
-        dataframe.columns = [x.lower() for x in dataframe.columns]
-        dataframe = dataframe.dropna(axis="index")
-
-        if not dataframe.index.is_monotonic_increasing:
-            dataframe = dataframe.sort_index()
-
-        spec = attributes["species"]
-
-        rename_cols = {
-            "stdev": spec + " variability",
-            "nbpoints": spec + " number_of_observations",
-        }
-
-        # TODO - add this back in once we've merged the fixes in
-        # Try and conver the flag / userflag column to str
-        # possible_flag_cols = ("flag", "userflag")
-        # flag_col = [x for x in dataframe.columns if x in possible_flag_cols]
-
-        # PR328
-        # if flag_col:
-        #     flag_str = flag_col[0]
-        #     dataframe = dataframe.astype({flag_str: str})
-
-        dataframe = dataframe.rename(columns=rename_cols).set_index("timestamp")
-
-        dataframe.index.name = "time"
-        dataframe.index = to_datetime(dataframe.index, format="%Y-%m-%d %H:%M:%S")
-
-        dataset = dataframe.to_xarray()
-        dataset.attrs.update(attributes)
-
-        # So there isn't an easy way of getting a hash of a Dataset, can we do something
-        # simple here we can compare data that's being added? Then we'll be able to make sure
-        # ObsSurface.store_data won't accept data it's already seen
-        data_key = f"key-{n}"
-        # TODO - do we need both attributes and metadata here?
-        standardised_data[data_key] = {
-            "metadata": metadata,
-            "data": dataset,
-            "attributes": attributes,
-        }
-
-    standardised_data = assign_attributes(data=standardised_data, update_mismatch=update_mismatch)
-
-    return standardised_data
-
-
-# def _read_site_metadata():
-#     """ Read site metadata from object store, if it doesn't exist we'll
-#     retrieve it from the ICOS CP and store it.
-
-#     Returns:
-#         dict: Dictionary of site data
-#     """
-#     from openghg.objectstore import get_bucket, get_object_from_json
-#     from openghg.types import ObjectStoreError
-#     from openghg.util import timestamp_now
-# raise NotImplementedError
-#     key = "metadata/icos_atmos_site_metadata"
-#     bucket = get_bucket()
-
-#     try:
-#         data = get_object_from_json(bucket=bucket, key=key)
-#     except ObjectStoreError:
-#         # Retrieve and store
-#         from icoscp import station
-#         station_data = station.getIdList()
-#         metadata = {d.id: dict(d) for _, d in df.iterrows()}
+    Returns:
+        int: Seconds for the estimated sampling period.
+    """
+    # Check useful attributes
+    data_selection = obspack_ds.attrs["dataset_selection_tag"]
+
+    hourly_s = 60 * 60
+    daily_s = hourly_s * 24
+    weekly_s = daily_s * 7
+    monthly_s = weekly_s * 28  # approx
+    yearly_s = daily_s * 365  # approx
+
+    sampling_period_estimate = 0.0  # seconds
+
+    frequency_keywords = {
+        "hourly": hourly_s,
+        "daily": daily_s,
+        "weekly": weekly_s,
+        "monthly": monthly_s,
+        "yearly": yearly_s,
+    }
+    for freq, time_s in frequency_keywords.items():
+        if freq in data_selection.lower():
+            sampling_period_estimate = time_s
+
+    if not sampling_period_estimate:
+        if "start_time" in obspack_ds and "midpoint_time" in obspack_ds:
+            half_sample_time = (obspack_ds["midpoint_time"] - obspack_ds["start_time"]).values
+            half_sample_time_s = half_sample_time.astype("timedelta64[s]").mean().astype(float)
+            sampling_period_estimate = round(half_sample_time_s * 2, 1)
+
+    if sampling_period_estimate < min_estimate:
+        sampling_period_estimate = min_estimate
+
+    return sampling_period_estimate
```

### Comparing `openghg-0.6.0/openghg/retrieve/met/_ecmwf.py` & `openghg-1.0.0/openghg/retrieve/met/_ecmwf.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from __future__ import annotations
-
-# import cdsapi  # type: ignore
-# import numpy as np
-from typing import TYPE_CHECKING, List, Optional, Union
-
-# import requests
-# from xarray import open_dataset, Dataset
-# from requests.adapters import HTTPAdapter
-# from requests.packages.urllib3.util.retry import Retry
-# from openghg.util import timestamp_tzaware
+import cdsapi  # type: ignore
+import numpy as np
+from typing import TYPE_CHECKING, List, Tuple, Union, Optional
+import requests
+from xarray import open_dataset, Dataset
+from requests.adapters import HTTPAdapter
+from requests.packages.urllib3.util.retry import Retry
+from openghg.util import timestamp_tzaware
 
 if TYPE_CHECKING:
     from openghg.dataobjects import METData
 
 __all__ = ["retrieve_met", "METData"]
 
 
@@ -30,234 +28,233 @@
     Args:
         site: Three letter sitec code
         network: Network
         years: Year(s) of data required
     Returns:
         METData: METData object holding data and metadata
     """
-    raise NotImplementedError("The met retrieval module needs updating and doesn't currently work.")
-    # from openghg.dataobjects import METData
+    from openghg.dataobjects import METData
+
+    if variables is None:
+        variables = ["u_component_of_wind", "v_component_of_wind"]
+
+    latitude, longitude, site_height, inlet_heights = _get_site_data(site=site, network=network)
+
+    # Get the area to retrieve data for
+    ecmwf_area = _get_ecmwf_area(site_lat=latitude, site_long=longitude)
+    # Calculate the pressure at measurement height(s)
+    measure_pressure = _get_site_pressure(inlet_heights=inlet_heights, site_height=site_height)
+    # Calculate the ERA5 pressure levels required
+    ecmwf_pressure_levels = _altitude_to_ecmwf_pressure(measure_pressure=measure_pressure)
+
+    if not isinstance(years, list):
+        years = [years]
+    else:
+        years = sorted(years)
+
+    # TODO - we might need to customise this further in the future to
+    # request other types of weather data
+    request = {
+        "product_type": "reanalysis",
+        "format": "netcdf",
+        "variable": variables,
+        "pressure_level": ecmwf_pressure_levels,
+        "year": [str(x) for x in years],
+        "month": [str(x).zfill(2) for x in range(1, 13)],
+        "day": [str(x).zfill(2) for x in range(1, 32)],
+        "time": [f"{str(x).zfill(2)}:00" for x in range(0, 24)],
+        "area": ecmwf_area,
+    }
+
+    cds_client = cdsapi.Client()
+    dataset_name = "reanalysis-era5-pressure-levels"
+
+    # Retrieve metadata from Copernicus about the dataset, this includes
+    # the location of the data netCDF file.
+    result = cds_client.retrieve(name=dataset_name, request=request)
+
+    # Download the data itself
+    dataset = _download_data(url=result.location)
+    # dataset = xr.open_dataset("/home/gar/Documents/Devel/RSE/openghg/tests/data/request_return.nc")
+
+    # We replace the date data with a start and end date here
+    start_date = str(timestamp_tzaware(f"{years[0]}-1-1"))
+    end_date = str(timestamp_tzaware(f"{years[-1]}-12-31"))
+
+    metadata = {
+        "product_type": request["product_type"],
+        "format": request["format"],
+        "variable": request["variable"],
+        "pressure_level": request["pressure_level"],
+        "area": request["area"],
+        "site": site,
+        "network": network,
+        "start_date": start_date,
+        "end_date": end_date,
+    }
+
+    return METData(data=dataset, metadata=metadata)
+
+
+def _download_data(url: str) -> Dataset:
+    """Retrieve data from the passed URL. This is used to retrieve data from
+    the Copernicus data store.
+
+    Args:
+        url: URL string
+    Returns:
+        xarray.Dataset: NetCDF data retrieved
+    """
+    # If we get any of these codes we'll try again
+    retriable_status_codes = [
+        requests.codes.internal_server_error,
+        requests.codes.bad_gateway,
+        requests.codes.service_unavailable,
+        requests.codes.gateway_timeout,
+        requests.codes.too_many_requests,
+        requests.codes.request_timeout,
+    ]
+
+    timeout = 20  # seconds
+
+    retry_strategy = Retry(
+        total=3,
+        status_forcelist=retriable_status_codes,
+        allowed_methods=["HEAD", "GET", "OPTIONS"],
+        backoff_factor=1,
+    )  # type: ignore
+
+    adapter = HTTPAdapter(max_retries=retry_strategy)
+
+    http = requests.Session()
+    http.mount("https://", adapter)
+    http.mount("http://", adapter)
+
+    data = http.get(url, timeout=timeout).content
+
+    try:
+        dataset: Dataset = open_dataset(data)
+    except ValueError:
+        raise ValueError("Invalid data returned, cannot create dataset.")
+
+    return dataset
+
+
+def _two_closest_values(diff: np.ndarray) -> np.ndarray:
+    """Get location of two closest values in an array of differences.
+
+    Args:
+        diff: Numpy array of values
+    Returns:
+        np.ndarry: Numpy array of two closes values
+    """
+    closest_values: np.ndarray = np.argpartition(np.abs(diff), 2)[:2]
+    return closest_values
+
+
+def _get_site_data(site: str, network: str) -> Tuple[float, float, float, List]:
+    """Extract site location data from site attributes file.
+
+    Args:
+        site: Site code
+    Returns:
+        dict: Dictionary of site data
+    """
+    from openghg.util import load_json
+
+    network = network.upper()
+    site = site.upper()
+
+    site_info = load_json("acrg_site_info.json")
+
+    try:
+        site_data = site_info[site][network]
+        latitude = float(site_data["latitude"])
+        longitute = float(site_data["longitude"])
+        site_height = float(site_data["height_station_masl"])
+        inlet_heights = site_data["height_name"]
+    except KeyError as e:
+        raise KeyError(f"Incorrect site or network : {e}")
+
+    return latitude, longitute, site_height, inlet_heights
+
+
+def _get_ecmwf_area(site_lat: float, site_long: float) -> List:
+    """Find out the area required from ERA5.
+
+    Args:
+        site_lat: Latitude of site
+        site_long: Site longitude
+    Returns:
+        list: List of min/max lat long values
+    """
+    ecwmf_lat = np.arange(-90, 90.25, 0.25)
+    ecwmf_lon = np.arange(-180, 180.25, 0.25)
+
+    ecwmf_lat_indices = _two_closest_values(ecwmf_lat - site_lat)
+    ecwmf_lon_indices = _two_closest_values(ecwmf_lon - site_long)
+
+    return [
+        np.max(ecwmf_lat[ecwmf_lat_indices]),
+        np.min(ecwmf_lon[ecwmf_lon_indices]),
+        np.min(ecwmf_lat[ecwmf_lat_indices]),
+        np.max(ecwmf_lon[ecwmf_lon_indices]),
+    ]
+
+
+def _get_site_pressure(inlet_heights: List, site_height: float) -> List[float]:
+    """Calculate the pressure levels required
+
+    Args:
+        inlet_height: Height(s) of inlets
+        site_height: Height of site
+    Returns:
+        list: List of pressures
+    """
+    import re
+
+    if not isinstance(inlet_heights, list):
+        inlet_heights = [inlet_heights]
+
+    measured_pressure = []
+    for h in inlet_heights:
+        try:
+            # Extract the number from the inlet height str using regex
+            inlet = float(re.findall(r"\d+(?:\.\d+)?", h)[0])
+            measurement_height = inlet + float(site_height)
+            # Calculate the pressure
+            pressure = 1000 * np.exp((-1 * measurement_height) / 7640)
+            measured_pressure.append(pressure)
+        except IndexError:
+            pass
+
+    return measured_pressure
+
+
+def _altitude_to_ecmwf_pressure(measure_pressure: List[float]) -> List[str]:
+    """Find out what pressure levels are required from ERA5.
+
+    Args:
+        measure_pressure: List of pressures
+    Returns:
+        list: List of desired pressures
+    """
+    from openghg.util import load_json
 
-    # if variables is None:
-    #     variables = ["u_component_of_wind", "v_component_of_wind"]
+    ecmwf_metadata = load_json("ecmwf_dataset_info.json")
+    dataset_metadata = ecmwf_metadata["datasets"]
+    valid_levels = dataset_metadata["reanalysis_era5_pressure_levels"]["valid_levels"]
 
-    # latitude, longitude, site_height, inlet_heights = _get_site_data(site=site, network=network)
+    # Available ERA5 pressure levels
+    era5_pressure_levels = np.array(valid_levels)
 
-    # # Get the area to retrieve data for
-    # ecmwf_area = _get_ecmwf_area(site_lat=latitude, site_long=longitude)
-    # # Calculate the pressure at measurement height(s)
-    # measure_pressure = _get_site_pressure(inlet_heights=inlet_heights, site_height=site_height)
-    # # Calculate the ERA5 pressure levels required
-    # ecmwf_pressure_levels = _altitude_to_ecmwf_pressure(measure_pressure=measure_pressure)
-
-    # if not isinstance(years, list):
-    #     years = [years]
-    # else:
-    #     years = sorted(years)
-
-    # # TODO - we might need to customise this further in the future to
-    # # request other types of weather data
-    # request = {
-    #     "product_type": "reanalysis",
-    #     "format": "netcdf",
-    #     "variable": variables,
-    #     "pressure_level": ecmwf_pressure_levels,
-    #     "year": [str(x) for x in years],
-    #     "month": [str(x).zfill(2) for x in range(1, 13)],
-    #     "day": [str(x).zfill(2) for x in range(1, 32)],
-    #     "time": [f"{str(x).zfill(2)}:00" for x in range(0, 24)],
-    #     "area": ecmwf_area,
-    # }
-
-    # cds_client = cdsapi.Client()
-    # dataset_name = "reanalysis-era5-pressure-levels"
-
-    # # Retrieve metadata from Copernicus about the dataset, this includes
-    # # the location of the data netCDF file.
-    # result = cds_client.retrieve(name=dataset_name, request=request)
-
-    # # Download the data itself
-    # dataset = _download_data(url=result.location)
-    # # dataset = xr.open_dataset("/home/gar/Documents/Devel/RSE/openghg/tests/data/request_return.nc")
-
-    # # We replace the date data with a start and end date here
-    # start_date = str(timestamp_tzaware(f"{years[0]}-1-1"))
-    # end_date = str(timestamp_tzaware(f"{years[-1]}-12-31"))
-
-    # metadata = {
-    #     "product_type": request["product_type"],
-    #     "format": request["format"],
-    #     "variable": request["variable"],
-    #     "pressure_level": request["pressure_level"],
-    #     "area": request["area"],
-    #     "site": site,
-    #     "network": network,
-    #     "start_date": start_date,
-    #     "end_date": end_date,
-    # }
-
-    # return METData(data=dataset, metadata=metadata)
-
-
-# def _download_data(url: str) -> Dataset:
-#     """Retrieve data from the passed URL. This is used to retrieve data from
-#     the Copernicus data store.
-
-#     Args:
-#         url: URL string
-#     Returns:
-#         xarray.Dataset: NetCDF data retrieved
-#     """
-#     # If we get any of these codes we'll try again
-#     retriable_status_codes = [
-#         requests.codes.internal_server_error,
-#         requests.codes.bad_gateway,
-#         requests.codes.service_unavailable,
-#         requests.codes.gateway_timeout,
-#         requests.codes.too_many_requests,
-#         requests.codes.request_timeout,
-#     ]
-
-#     timeout = 20  # seconds
-
-#     retry_strategy = Retry(
-#         total=3,
-#         status_forcelist=retriable_status_codes,
-#         allowed_methods=["HEAD", "GET", "OPTIONS"],
-#         backoff_factor=1,
-#     )  # type: ignore
-
-#     adapter = HTTPAdapter(max_retries=retry_strategy)
-
-#     http = requests.Session()
-#     http.mount("https://", adapter)
-#     http.mount("http://", adapter)
-
-#     data = http.get(url, timeout=timeout).content
-
-#     try:
-#         dataset: Dataset = open_dataset(data)
-#     except ValueError:
-#         raise ValueError("Invalid data returned, cannot create dataset.")
-
-#     return dataset
-
-
-# def _two_closest_values(diff: np.ndarray) -> np.ndarray:
-#     """Get location of two closest values in an array of differences.
-
-#     Args:
-#         diff: Numpy array of values
-#     Returns:
-#         np.ndarry: Numpy array of two closes values
-#     """
-#     closest_values: np.ndarray = np.argpartition(np.abs(diff), 2)[:2]
-#     return closest_values
-
-
-# def _get_site_data(site: str, network: str) -> Tuple[float, float, float, List]:
-#     """Extract site location data from site attributes file.
-
-#     Args:
-#         site: Site code
-#     Returns:
-#         dict: Dictionary of site data
-#     """
-#     from openghg.util import load_json
-
-#     network = network.upper()
-#     site = site.upper()
-
-#     site_info = load_json("site_info.json")
-
-#     try:
-#         site_data = site_info[site][network]
-#         latitude = float(site_data["latitude"])
-#         longitute = float(site_data["longitude"])
-#         site_height = float(site_data["height_station_masl"])
-#         inlet_heights = site_data["height_name"]
-#     except KeyError as e:
-#         raise KeyError(f"Incorrect site or network : {e}")
-
-#     return latitude, longitute, site_height, inlet_heights
-
-
-# def _get_ecmwf_area(site_lat: float, site_long: float) -> List:
-#     """Find out the area required from ERA5.
-
-#     Args:
-#         site_lat: Latitude of site
-#         site_long: Site longitude
-#     Returns:
-#         list: List of min/max lat long values
-#     """
-#     ecwmf_lat = np.arange(-90, 90.25, 0.25)
-#     ecwmf_lon = np.arange(-180, 180.25, 0.25)
-
-#     ecwmf_lat_indices = _two_closest_values(ecwmf_lat - site_lat)
-#     ecwmf_lon_indices = _two_closest_values(ecwmf_lon - site_long)
-
-#     return [
-#         np.max(ecwmf_lat[ecwmf_lat_indices]),
-#         np.min(ecwmf_lon[ecwmf_lon_indices]),
-#         np.min(ecwmf_lat[ecwmf_lat_indices]),
-#         np.max(ecwmf_lon[ecwmf_lon_indices]),
-#     ]
-
-
-# def _get_site_pressure(inlet_heights: List, site_height: float) -> List[float]:
-#     """Calculate the pressure levels required
-
-#     Args:
-#         inlet_height: Height(s) of inlets
-#         site_height: Height of site
-#     Returns:
-#         list: List of pressures
-#     """
-#     import re
-
-#     if not isinstance(inlet_heights, list):
-#         inlet_heights = [inlet_heights]
-
-#     measured_pressure = []
-#     for h in inlet_heights:
-#         try:
-#             # Extract the number from the inlet height str using regex
-#             inlet = float(re.findall(r"\d+(?:\.\d+)?", h)[0])
-#             measurement_height = inlet + float(site_height)
-#             # Calculate the pressure
-#             pressure = 1000 * np.exp((-1 * measurement_height) / 7640)
-#             measured_pressure.append(pressure)
-#         except IndexError:
-#             pass
-
-#     return measured_pressure
-
-
-# def _altitude_to_ecmwf_pressure(measure_pressure: List[float]) -> List[str]:
-#     """Find out what pressure levels are required from ERA5.
-
-#     Args:
-#         measure_pressure: List of pressures
-#     Returns:
-#         list: List of desired pressures
-#     """
-#     from openghg.util import load_json
-
-#     ecmwf_metadata = load_json("ecmwf_dataset_info.json")
-#     dataset_metadata = ecmwf_metadata["datasets"]
-#     valid_levels = dataset_metadata["reanalysis_era5_pressure_levels"]["valid_levels"]
-
-#     # Available ERA5 pressure levels
-#     era5_pressure_levels = np.array(valid_levels)
-
-#     # Match pressure to ERA5 pressure levels
-#     ecwmf_pressure_indices = np.zeros(len(measure_pressure) * 2)
+    # Match pressure to ERA5 pressure levels
+    ecwmf_pressure_indices = np.zeros(len(measure_pressure) * 2)
 
-#     for index, m in enumerate(measure_pressure):
-#         ecwmf_pressure_indices[(index * 2) : (index * 2 + 2)] = _two_closest_values(m - era5_pressure_levels)
+    for index, m in enumerate(measure_pressure):
+        ecwmf_pressure_indices[(index * 2) : (index * 2 + 2)] = _two_closest_values(m - era5_pressure_levels)
 
-#     desired_era5_pressure = era5_pressure_levels[np.unique(ecwmf_pressure_indices).astype(int)]
+    desired_era5_pressure = era5_pressure_levels[np.unique(ecwmf_pressure_indices).astype(int)]
 
-#     pressure_levels: List = desired_era5_pressure.astype(str).tolist()
+    pressure_levels: List = desired_era5_pressure.astype(str).tolist()
 
-#     return pressure_levels
+    return pressure_levels
```

### Comparing `openghg-0.6.0/openghg/retrieve/metadata/acrg_site_info.json` & `openghg-1.0.0/openghg/retrieve/metadata/acrg_site_info.json`

 * *Files identical despite different names*

### Comparing `openghg-0.6.0/openghg/retrieve/metadata/process_gcwerks_parameters.json` & `openghg-1.0.0/openghg/retrieve/metadata/process_gcwerks_parameters.json`

 * *Files identical despite different names*

### Comparing `openghg-0.6.0/openghg/service/_openghg_service.py` & `openghg-1.0.0/openghg/service/_openghg_service.py`

 * *Files identical despite different names*

### Comparing `openghg-0.6.0/openghg/standardise/column/_openghg.py` & `openghg-1.0.0/openghg/standardise/meta/_attributes.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,327 +1,342 @@
-from pathlib import Path
-from typing import Dict, List, MutableMapping, Optional, Union, cast
+from typing import cast, Any, Dict, Optional, List
+from xarray import Dataset
 
-import xarray as xr
 
-
-def parse_openghg(
-    data_filepath: Union[str, Path],
-    satellite: Optional[str] = None,
-    domain: Optional[str] = None,
-    selection: Optional[str] = None,
-    site: Optional[str] = None,
-    species: Optional[str] = None,
-    network: Optional[str] = None,
-    instrument: Optional[str] = None,
-    platform: str = "satellite",
-    **kwargs: str,
+def assign_attributes(
+    data: Dict,
+    site: str,
+    network: str = None,
+    sampling_period: str = None,
 ) -> Dict:
+    """Assign attributes to each site and species dataset. This ensures that the xarray Datasets produced
+    are CF 1.7 compliant. Some of the attributes written to the Dataset are saved as metadata
+    to the Datasource allowing more detailed searching of data.
+
+    Args:
+        data: Dictionary containing data, metadata and attributes
+        site: Site code
+        sampling_period: Number of seconds for which air
+                         sample is taken. Only for time variable attribute
+        network: Network name
+    Returns:
+        dict: Dictionary of combined data with correct attributes assigned to Datasets
+    """
+    from openghg.standardise.meta import surface_standardise
+
+    for key, gas_data in data.items():
+        site_attributes = gas_data["attributes"]
+        species = gas_data["metadata"]["species"]
+
+        units = gas_data.get("metadata", {}).get("units")
+        scale = gas_data.get("metadata", {}).get("calibration_scale")
+
+        if sampling_period is None:
+            sampling_period = str(gas_data.get("metadata", {}).get("sampling_period", "NOT_SET"))
+
+        gas_data["data"] = get_attributes(
+            ds=gas_data["data"],
+            species=species,
+            site=site,
+            network=network,
+            units=units,
+            scale=scale,
+            global_attributes=site_attributes,
+            sampling_period=sampling_period,
+        )
+
+        measurement_data = gas_data["data"]
+        metadata = gas_data["metadata"]
+
+        attrs = measurement_data.attrs
+
+        gas_data["metadata"] = surface_standardise(metadata=metadata, attributes=attrs)
+
+    return data
+
+
+def get_attributes(
+    ds: Dataset,
+    species: str,
+    site: str,
+    network: str = None,
+    global_attributes: Dict[str, str] = None,
+    units: str = None,
+    scale: str = None,
+    sampling_period: str = None,
+    date_range: List[str] = None,
+) -> Dataset:
     """
-    Parse and extract data from pre-formatted netcdf file which already
-    matches expected OpenGHG format.
+    This function writes attributes to an xarray.Dataset so that they conform with
+    the CF Convention v1.6
 
-    The arguments specified below are the metadata needed to store this
-    surface observation file within the object store. If these keywords are
-    not included within the attributes of the netcdf file being passed then
-    these arguments must be specified.
-
-    For column data this can either be a satellite (e.g. satellite="GOSAT") or a
-    site (site="RUN", network="TCCON"). Either can be specified or this function
-    will attempt to extract this from the data file.
+    Attributes of the xarray DataSet are modified, and variable names are changed
 
-    Args:
-        data_filepath: Path of observation file
-        satellite: Name of satellite (if relevant)
-        domain: For satellite only. If data has been selected on an area include the
-            identifier name for domain covered. This can map to previously defined domains
-            (see openghg_defs "domain_info.json" file) or a newly defined domain.
-        selection: For satellite only, identifier for any data selection which has been
-            performed on satellite data. This can be based on any form of filtering, binning etc.
-            but should be unique compared to other selections made e.g. "land", "glint", "upperlimit".
-            If not specified, domain will be used.
-        site : Site code/name (if relevant). Can include satellite OR site.
-        species: Species name or synonym e.g. "ch4"
-        instrument: Instrument name e.g. "TANSO-FTS"
-        network: Name of in-situ or satellite network e.g. "TCCON", "GOSAT"
-        platform: Type of platform. Should be one of:
-            - "satellite"
-            - "site"
-            Note: this will be superceded if site or satellite keywords are specified.
-        kwargs: Any additional attributes to be associated with the data.
+    If the species is a standard mole fraction then either:
+        - species name will used in lower case in the file and variable names
+            but with any hyphens taken out
+        - name will be changed according to the species_translator dictionary
+
+    If the species is isotopic data or a non-standard variable (e.g. APO):
+        - Isotopes species names should begin with a "D"
+            (Annoyingly, the code currently picks up "Desflurane" too. I've
+             fixed this for now, but if we get a lot of other "D" species, we
+             should make this better)
+        - I suggest naming for isotopologues should be d<species><isotope>, e.g.
+            dCH4C13, or dCO2C14
+        - Any non-standard variables should be listed in the species_translator
+            dictionary
 
-    Returns:
-        Dict : Dictionary of source_name : data, metadata, attributes
+    Args:
+        ds: Should contain variables such as "ch4", "ch4 repeatability".
+            Must have a "time" dimension.
+        species: Species name. e.g. "CH4", "HFC-134a", "dCH4C13"
+        site: Three-letter site code
+        network: Network site is associated with
+        global_attribuates: Dictionary containing any info you want to
+            add to the file header (e.g. {"Contact": "Contact_Name"})
+        units: This routine will try to guess the units
+            unless this is specified. Options are in units_interpret
+        scale: Calibration scale for species.
+        sampling_period: Number of seconds for which air
+            sample is taken. Only for time variable attribute
+        date_range: Start and end date for output
+            If you only want an end date, just put a very early start date
+            (e.g. ["1900-01-01", "2010-01-01"])
     """
-    from openghg.standardise.meta import define_species_label
-    from openghg.util import clean_string
+    from pandas import Timestamp as pd_Timestamp
+    from openghg.util import clean_string, load_json, timestamp_now
 
-    # from openghg.standardise.meta import metadata_default_keys, assign_attributes
+    # from numpy import unique as np_unique
 
-    data_filepath = Path(data_filepath)
+    if not isinstance(ds, Dataset):
+        raise TypeError("This function only accepts xarray Datasets")
 
-    if data_filepath.suffix != ".nc":
-        raise ValueError("Input file must be a .nc (netcdf) file.")
-
-    with xr.open_dataset(data_filepath) as temp:
-        data = temp
-
-    # Extract current attributes from input data
-    attributes = cast(MutableMapping, data.attrs)
-
-    if satellite is not None or platform == "satellite":
-        metadata_required = metadata_default_satellite_column()
-        metadata_required.remove("selection")
-        platform = "satellite"
-    elif site is not None or platform == "site":
-        metadata_required = metadata_default_site_column()
-        platform = "site"
-
-    if platform == "satellite":
-        if domain is None:
-            raise ValueError(
-                "For satellite data, please specify selected domain."
-                "This can be 'global' if no selection has been made."
-            )
-
-    # Define metadata based on input arguments.
-    metadata_initial = {
-        "site": site,
-        "satellite": satellite,
-        "instrument": instrument,
-        "species": species,
-        "domain": domain,
-        "network": network,
-        "platform": platform,
-        "data_type": "column",
-        "source_format": "openghg",
-    }
+    # Current CF Conventions (v1.8) demand that valid variable names
+    # begin with a letter and be composed of letters, digits and underscores
+    # Here variable names are also made lowercase to enable easier matching below
 
-    # TODO: Tidy this up a bit (maybe split some into a separate function?)
-    # and incorporate kwargs
+    # TODO - could I just cast ds.variables as as type for mypy instead of doing this?
+    # variable_names = [str(v) for v in ds.variables]
+    # Is this better?
+    variable_names = cast(Dict[str, Any], ds.variables)
+    to_underscores = {var: var.lower().replace(" ", "_") for var in variable_names}
+    ds = ds.rename(to_underscores)  # type: ignore
 
-    metadata = {}
-    key_translation = satellite_attribute_translation()
-    # Populate metadata with values from attributes if inputs have not been passed
-    for key, value in metadata_initial.items():
-        if key in metadata_required:
-            # Extract equivalent key from passed file if present using translation
-            try:
-                attr_keys = key_translation[key]
-            except KeyError:
-                attr_keys = key
-
-            # Make sure this is a list for cases with multiple options
-            if isinstance(attr_keys, str):
-                attr_keys = [attr_keys]
-
-            if value is None:
-                # Extract value from attributes if this has not been specified
-                for attr_key in attr_keys:
-                    try:
-                        metadata[key] = attributes[attr_key]
-                    except KeyError:
-                        continue
-                    else:
-                        break
-                else:
-                    raise ValueError(f"Input '{key}' must be specified if not included in data attributes.")
-            else:
-                # If attributes are present, check these match to inputs passed
-                for attr_key in attr_keys:
-                    if attr_key in key_translation and attr_key in attributes:
-                        attributes_value = attributes[attr_key]
-                        if value != attributes_value:
-                            # If inputs do not match attribute values, raise a ValueError
-                            raise ValueError(
-                                f"Input for '{key}': {value} does not match value in file attributes: {attributes_value}"
-                            )
-                metadata[key] = value
-
-    # metadata = cast(Dict[str, str], metadata_initial)
-
-    if selection is not None:
-        metadata["selection"] = selection
-    elif platform == "satellite":
-        metadata["selection"] = domain
-
-    # TODO: Add loose domain checking? If known domain is specified, make sure points
-    # are within this for example.
-
-    species = define_species_label(metadata["species"])[0]
-    metadata["species"] = species
-
-    if "site" in metadata:
-        metadata["site"] = clean_string(metadata["site"])
+    species_attrs = load_json(filename="species_attributes.json")
+    attributes_data = load_json("attributes.json")
+
+    species_translator = attributes_data["species_translation"]
+    unit_species = attributes_data["unit_species"]
+    unit_species_long = attributes_data["unit_species_long"]
+    unit_interpret = attributes_data["unit_interpret"]
 
-    # Add data type to metadata
-    metadata["data_type"] = "column"
+    species_upper = species.upper()
+    species_lower = species.lower()
 
-    # Define remaining keys needed for metadata
-    metadata_needed = [param for param in metadata_required if param not in metadata]
+    variable_names = cast(Dict[str, Any], ds.variables)
+    matched_keys = [var for var in variable_names if species_lower in var]
 
-    for key in metadata_needed:
+    # If we don't have any variables to rename, raise an error
+    if not matched_keys:
+        raise NameError(f"Cannot find species {species} in Dataset variables")
+
+    species_rename = {}
+    for var in matched_keys:
         try:
-            attr_keys = key_translation[key]
+            species_label = species_translator[species_upper]["chem"]
         except KeyError:
-            attr_keys = key
+            species_label = clean_string(species_lower)
+
+        species_rename[var] = var.replace(species_lower, species_label)
 
-        if isinstance(attr_keys, str):
-            attr_keys = [attr_keys]
+    ds = ds.rename(species_rename)  # type: ignore
+
+    # Global attributes
+    global_attributes_default = {
+        "conditions_of_use": "Ensure that you contact the data owner at the outset of your project.",
+        "source": "In situ measurements of air",
+        "Conventions": "CF-1.8",
+    }
 
-        for attr_key in attr_keys:
-            for attr_key in attr_keys:
-                try:
-                    metadata[key] = attributes[attr_key]
-                except KeyError:
-                    continue
+    if global_attributes is not None:
+        # TODO - for some reason mypy doesn't see a Dict[str,str] as a valid Mapping[Hashable, Any] type
+        global_attributes.update(global_attributes_default)  # type: ignore
+    else:
+        global_attributes = global_attributes_default
+
+    global_attributes["file_created"] = str(timestamp_now())
+    global_attributes["processed_by"] = "OpenGHG_Cloud"
+    global_attributes["species"] = species_label
+
+    if scale is None:
+        global_attributes["calibration_scale"] = "unknown"
+    else:
+        global_attributes["calibration_scale"] = scale
+
+    if sampling_period is None:
+        global_attributes["sampling_period"] = "NOT_SET"
+    else:
+        global_attributes["sampling_period"] = sampling_period
+        global_attributes["sampling_period_unit"] = "s"
+
+    # Update the Dataset attributes
+    ds.attrs.update(global_attributes)  # type: ignore
+
+    # Add some site attributes
+    site_attributes = _site_info_attributes(site.upper(), network)
+    ds.attrs.update(site_attributes)
+
+    # Species-specific attributes
+    # Long name
+    if species_upper.startswith("D") and species_upper != "DESFLURANE" or species_upper == "APD":
+        sp_long = species_translator[species_upper]["name"]
+    elif species_upper == "RN":
+        sp_long = "radioactivity_concentration_of_222Rn_in_air"
+    elif species_upper in species_translator:
+        name = species_translator[species_upper]["name"]
+        sp_long = f"mole_fraction_of_{name}_in_air"
+    else:
+        sp_long = f"mole_fraction_of_{species_label}_in_air"
+
+    ancillary_variables = []
+
+    variable_names = cast(Dict[str, Any], ds.variables)
+    matched_keys = [var for var in variable_names if species_lower in var.lower()]
+
+    # Write units as attributes to variables containing any of these
+    match_words = ["variability", "repeatability", "stdev", "count"]
+
+    for key in variable_names:
+        key = key.lower()
+
+        if species_label.lower() in key:
+            # Standard name attribute
+            # ds[key].attrs["standard_name"]=key.replace(species_label, sp_long)
+            ds[key].attrs["long_name"] = key.replace(species_label, sp_long)
+
+            # If units are required for variable, add attribute
+            if key == species_label or any(word in key for word in match_words):
+                if units is not None:
+                    if units in unit_interpret:
+                        ds[key].attrs["units"] = unit_interpret[units]
+                    else:
+                        ds[key].attrs["units"] = unit_interpret["else"]
                 else:
-                    break
-            else:
-                raise ValueError(f"Input '{key}' must be specified if not included in data attributes.")
-
-    # In GOSAT UoL files (and copied into our files)
-    #  - platform = "GOSAT"; sensor = "TANSO-FTS"
-    # In TROPOMI S5P_OFFL_...nc files
-    #  - platform = 'S5P'; sensor = "TROPOMI"
-    # Could "platform" --> "satellite" perhaps?
-
-    # site = metadata["site"]
-    # network = metadata["network"]
-    # species = metadata["species"]
-
-    # # Allow site and network data to be treated in a case insensitive way
-    # site_case_options = [site, site.upper(), site.lower()]
-    # network_case_options = [network, network.upper(), network.lower()]
-
-    # # Extract centralised data for site (if present)
-    # site_data = load_json(filename="site_info.json")
-    # for site_value in site_case_options:
-    #     if site_value in site_data:
-    #         site_info_all = site_data[site_value]
-    #         break
-    # else:
-    #     print("Unknown site. Will attempt to extract metadata from dataset attributes or input keywords")
-    #     site_info_all = {}
-
-    # for network_value in network_case_options:
-    #     if network_value in site_info_all:
-    #         site_info = site_info_all[network_value]
-    #         break
-    # else:
-    #     print(
-    #         "Network {network} does not match with site {site}. Will attempt to extract metadata from dataset attributes or input keywords"
-    #     )
-    #     site_info = {}
-
-    # if site_info:
-    #     # Ensure keywords match to metadata names for station values
-    #     # e.g. "station_longitude" derived from "longitude"
-    #     for key in metadata_needed:
-    #         prefix = "station_"
-    #         if key.startswith(prefix):
-    #             split_key = key.split("_")[1:]
-    #             short_key_option1 = "_".join(split_key)
-
-    #             split_key.insert(1, "station")  # to catch "height_station_masl"
-    #             short_key_option2 = "_".join(split_key)
-
-    #             short_key_options = [short_key_option1, short_key_option2]
-    #             for short_key in short_key_options:
-    #                 if short_key in site_info:
-    #                     site_info[key] = site_info[short_key]
-    #                     break
-
-    # # Load attributes data for network if present
-    # param_data = load_json(filename="attributes.json")
-    # for network_value in network_case_options:
-    #     if network_value in param_data:
-    #         network_params = param_data[network_value]
-    #         site_attributes = network_params["global_attributes"]
-    #         break
-    # else:
-    #     site_attributes = {}
-
-    # # Define sources of attributes to use when defining metadata
-    # # The order here influences the hierarchy if keys appear multiple times.
-    # # kwargs allow additional variables such as "station_longitude" to be included if needed.
-    # attribute_sources = [attributes, kwargs, site_info, site_attributes]
-
-    # # Search attributes sources (in order) and populate metadata
-    # for param in metadata_needed:
-    #     for source in attribute_sources:
-    #         if param in source:
-    #             metadata[param] = source[param]
-    #             break
-    #     else:
-    #         raise ValueError(
-    #             f"Cannot extract or infer '{param}' parameter needed for metadata from stored data, attributes or keywords"
-    #         )
-
-    # Update attributes to match metadata after cleaning
-    attributes.update(metadata)
-
-    # TODO: Decide if the key here should be more descriptive that just `species`
-    gas_data = {species: {"metadata": metadata, "data": data, "attributes": attributes}}
+                    # TODO - merge these species attributes into a single simpler JSON
+                    try:
+                        ds[key].attrs["units"] = unit_species[species_upper]
+                    except KeyError:
+                        try:
+                            ds[key].attrs["units"] = species_attrs[species_label.upper()]["units"]
+                        except KeyError:
+                            ds[key].attrs["units"] = "NA"
+
+                # If units are non-standard, add explanation
+                if species_upper in unit_species_long:
+                    ds[key].attrs["units_description"] = unit_species_long[species_upper]
+
+            # Add to list of ancilliary variables
+            if key != species_label:
+                ancillary_variables.append(key)
+
+    # TODO - for the moment skip this step - check status of ancilliary variables in standard
+    # Write ancilliary variable list
+    # ds[species_label].attrs["ancilliary_variables"] = ", ".join(ancillary_variables)
+
+    # Add quality flag attributes
+    # NOTE - I've removed the whitespace before status_flag and integration_flag here
+    variable_names = cast(Dict[str, Any], ds.variables)
+    quality_flags = [key for key in variable_names if "status_flag" in key]
 
-    # gas_data = assign_attributes(data=gas_data, site=site, network=network)
+    # Not getting long_name for c2f6
 
-    return gas_data
+    for key in quality_flags:
+        ds[key] = ds[key].astype(int)
+        try:
+            long_name = ds[species_label].attrs["long_name"]
+        except KeyError:
+            raise KeyError(key, quality_flags)
 
+        ds[key].attrs = {
+            "flag_meaning": "0 = unflagged, 1 = flagged",
+            "long_name": f"{long_name} status_flag",
+        }
 
-def metadata_default_satellite_column() -> List[str]:
-    """
-    Define default keys for satellite column data
-    """
-    default_keys = [
-        "satellite",
-        "species",
-        "network",
-        "instrument",
-        "platform",
-        "domain",
-        "selection",
-        "data_owner",
-        "data_owner_email",
-    ]
+    variable_names = cast(Dict[str, Any], ds.variables)
+    # Add integration flag attributes
+    integration_flags = [key for key in variable_names if "integration_flag" in key]
 
-    return default_keys
+    for key in integration_flags:
+        ds[key] = ds[key].astype(int)
+        long_name = ds[species_label].attrs["long_name"]
+        ds[key].attrs = {
+            "flag_meaning": "0 = area, 1 = height",
+            "standard_name": f"{long_name} integration_flag",
+            "comment": "GC peak integration method (by height or by area). Does not indicate data quality",
+        }
 
+    first_year = pd_Timestamp(str(ds.time[0].values)).year
 
-def metadata_default_site_column() -> List[str]:
-    """
-    Define default keys for site column data
-    """
-    default_keys = [
-        "site",
-        "species",
-        "network",
-        "instrument",
-        "platform",
-        "data_owner",
-        "data_owner_email",
-    ]
+    ds.time.encoding = {"units": f"seconds since {str(first_year)}-01-01 00:00:00"}
 
-    return default_keys
+    time_attributes: Dict[str, str] = {}
+    time_attributes["label"] = "left"
+    time_attributes["standard_name"] = "time"
+    time_attributes["comment"] = (
+        "Time stamp corresponds to beginning of sampling period. "
+        + "Time since midnight UTC of reference date. "
+        + "Note that sampling periods are approximate."
+    )
 
+    if sampling_period is not None:
+        time_attributes["sampling_period_seconds"] = sampling_period
 
-TranslationDict = Dict[str, Union[str, List[str]]]
+    ds.time.attrs.update(time_attributes)
 
+    # If a date range is specified, slice dataset
+    if date_range:
+        ds = ds.loc[dict(time=slice(*date_range))]
 
-def satellite_attribute_translation() -> TranslationDict:
-    """
-    Define translation between openghg keyword and input files.
-    Currently includes:
-     - GOSAT (University of Leicester product)
-     - TROPOMI
+    return ds
+
+
+def _site_info_attributes(site: str, network: Optional[str] = None) -> Dict:
+    """Reads site attributes from JSON
+
+    Args:
+        site: Site code
+        network: Network name
+    Returns:
+        dict: Dictionary of site attributes
     """
-    # Current values within (at least) GOSAT, TROPOMI files
-    # - values can contain lists as well as single string values
-    keywords: TranslationDict = {
-        "instrument": "sensor",
-        "satellite": "platform",
-        "network": "platform",
-        "data_owner": "creator_name",
-        "data_owner_email": "creator_email",
+    from openghg.util import load_json
+
+    site = site.upper()
+
+    # Read site info file
+    data_filename = "acrg_site_info.json"
+    site_params = load_json(filename=data_filename)
+
+    if network is None:
+        network = list(site_params[site].keys())[0]
+    else:
+        network = network.upper()
+
+    attributes_dict = {
+        "longitude": "station_longitude",
+        "latitude": "station_latitude",
+        "long_name": "station_long_name",
+        "height_station_masl": "station_height_masl",
     }
 
-    return keywords
+    attributes = {}
+    if site in site_params:
+        for attr in attributes_dict:
+            if attr in site_params[site][network]:
+                attr_key = attributes_dict[attr]
+
+                attributes[attr_key] = site_params[site][network][attr]
+    else:
+        raise ValueError(f"Invalid site {site} passed. Please use a valid site code such as BSD for Bilsdale")
+
+    return attributes
```

### Comparing `openghg-0.6.0/openghg/standardise/surface/_aqmesh.py` & `openghg-1.0.0/openghg/standardise/surface/_aqmesh.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
+from typing import Dict, Union, Optional
 from pathlib import Path
-from typing import Dict, Optional, Union
+
 
 pathType = Union[str, Path]
 
 
 def parse_aqmesh(
     data_filepath: pathType,
     metadata_filepath: pathType,
     sampling_period: Optional[str] = None,
-    **kwargs: Dict,
 ) -> Dict:
     """Read AQMesh data files
 
     Args:
         data_filepath: Data filepath
         metadata_filepath: Metadata filepath
         sampling_period: Measurement sampling period (str)
@@ -77,16 +77,16 @@
     Args:
         filepath: Path to metadata CSV
         pipeline: If running in pipeline skip the writing of metadata to file
     Returns:
         dict: Dictionary of metadata
     """
     from addict import Dict as aDict
-    from openghg.util import check_date, format_inlet
     from pandas import read_csv
+    from openghg.util import check_date
 
     filepath = Path(filepath)
     raw_metadata = read_csv(filepath)
 
     site_metadata = aDict()
 
     for _, row in raw_metadata.iterrows():
@@ -100,16 +100,14 @@
         site_data["relocate_date"] = check_date(row["relocate_date_UTC"])
         site_data["long_name"] = row["location_name"]
         site_data["borough"] = row["Borough"]
         site_data["site_type"] = row["Type"]
         site_data["in_ulez"] = row["ULEZ"]
         site_data["latitude"] = row["Latitude"]
         site_data["longitude"] = row["Longitude"]
-        site_data["inlet"] = format_inlet(row["Height"], key_name="inlet")
+        site_data["inlet"] = row["Height"]
         site_data["network"] = "aqmesh_glasgow"
         site_data["sampling_period"] = "NA"
-        site_data["data_type"] = "surface"
-        site_data["source_format"] = "aqmesh"
 
     # TODO - I feel this is a bit clunky
     dict_metadata: Dict = site_metadata.to_dict()
     return dict_metadata
```

### Comparing `openghg-0.6.0/openghg/standardise/surface/_beaco2n.py` & `openghg-1.0.0/openghg/standardise/surface/_beaco2n.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-from pathlib import Path
 from typing import DefaultDict, Dict, Optional, Union
-
+from pathlib import Path
 from pandas import DataFrame
 
 __all__ = ["parse_beaco2n"]
 
 
 def parse_beaco2n(
     data_filepath: Union[str, Path],
     site: str,
     network: str,
     inlet: str,
     instrument: Optional[str] = "shinyei",
     sampling_period: Optional[str] = None,
-    **kwargs: Dict,
 ) -> Dict:
     """Read BEACO2N data files
 
     Args:
         data_filepath: Data filepath
         site: Site name
         network: Network name
         inlet: Inlet height in metres
         instrument: Instrument name
         sampling_period: Measurement sampling period
     Returns:
         dict: Dictionary of data
     """
-    from collections import defaultdict
-
     import pandas as pd
-    from openghg.util import clean_string, load_internal_json, format_inlet
+    from openghg.util import load_json
+    from collections import defaultdict
+    from openghg.util import clean_string
 
     if sampling_period is None:
         sampling_period = "NOT_SET"
 
     data_filepath = Path(data_filepath)
     datetime_columns = {"time": ["datetime"]}
     use_cols = [1, 5, 6, 7, 8, 9, 10]
@@ -51,15 +49,15 @@
             na_values=na_values,
         )
     except ValueError as e:
         raise ValueError(
             f"Unable to read data file, please make sure it is in the standard BEACO2N format.\nError: {e}"
         )
 
-    beaco2n_site_data = load_internal_json(filename="beaco2n_site_data.json")
+    beaco2n_site_data = load_json("beaco2n_site_data.json")
 
     try:
         site_metadata = beaco2n_site_data[site.upper()]
     except KeyError:
         raise ValueError(f"Site {site} not recognized.")
 
     site_metadata["comment"] = "Retrieved from http://beacon.berkeley.edu/"
@@ -91,32 +89,24 @@
 
         # Some sites don't have data for each type, skip that type if all NaNs
         if m_data.index.empty:
             continue
 
         m_data = m_data.to_xarray()
 
-        inlet = clean_string(inlet)
-        inlet = format_inlet(inlet, key_name="inlet")
-
         species_metadata = {
             "units": units[mt],
             "site": site,
             "species": clean_string(mt),
-            "inlet": inlet,
+            "inlet": clean_string(inlet),
             "network": "beaco2n",
             "sampling_period": str(sampling_period),
             "instrument": instrument,
-            "data_type": "surface",
-            "source_format": "beaco2n",
         }
 
-        # We'll put everything into metadata
-        species_metadata.update(site_metadata)
-
         gas_data[mt]["data"] = m_data
         gas_data[mt]["metadata"] = species_metadata
         gas_data[mt]["attributes"] = site_metadata
 
     # TODO - add CF Compliant attributes?
 
     return gas_data
```

### Comparing `openghg-0.6.0/openghg/standardise/surface/_btt.py` & `openghg-1.0.0/openghg/standardise/surface/_btt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,31 @@
-from pathlib import Path
 from typing import Dict, Optional, Union
+from pathlib import Path
 
 
 def parse_btt(
     data_filepath: Union[str, Path],
     site: Optional[str] = "BTT",
     network: Optional[str] = "LGHG",
     inlet: Optional[str] = None,
     instrument: Optional[str] = None,
-    update_mismatch: str = "never",
 ) -> Dict:
     """Reads NPL data files and returns the UUIDS of the Datasources
     the processed data has been assigned to
 
     Args:
         data_filepath: Path of file to load
         site: Site name
-        update_mismatch: This determines how mismatches between the internal data
-            "attributes" and the supplied / derived "metadata" are handled.
-            This includes the options:
-              - "never" - don't update mismatches and raise an AttrMismatchError
-              - "from_source" / "attributes" - update mismatches based on input data (e.g. data attributes)
-              - "from_definition" / "metadata" - update mismatches based on associated data (e.g. site_info.json)
     Returns:
         dict: Dictionary of gas data
     """
-    from numpy import nan as np_nan
     from openghg.standardise.meta import assign_attributes
-    from openghg.util import clean_string, load_internal_json, get_site_info, format_inlet
-    from pandas import Timestamp, isnull, read_csv, to_timedelta
+    from pandas import read_csv, Timestamp, to_timedelta, isnull
+    from numpy import nan as np_nan
+    from openghg.util import clean_string, load_json
 
     # TODO: Decide what to do about inputs which aren't use anywhere
     # at present - inlet, instrument, sampling_period, measurement_type
 
     data_filepath = Path(data_filepath)
 
     site = "BTT"
@@ -40,37 +33,35 @@
     # Rename these columns
     rename_dict = {"co2.cal": "CO2", "ch4.cal.ppb": "CH4"}
     # We only want these species
     species_extract = ["CO2", "CH4"]
     # Take std-dev measurements from these columns for these species
     species_sd = {"CO2": "co2.sd.ppm", "CH4": "ch4.sd.ppb"}
 
-    site_data = get_site_info()
+    site_data = load_json(filename="acrg_site_info.json")
     site_info = site_data[site][network]
 
-    param_data = load_internal_json(filename="attributes.json")
+    param_data = load_json(filename="attributes.json")
     network_params = param_data["BTT"]
     site_attributes = network_params["global_attributes"]
 
     sampling_period = int(network_params["sampling_period"])
     sampling_period_seconds = str(sampling_period) + "s"
 
     metadata = {}
     metadata["site"] = site
-    metadata["inlet"] = format_inlet(network_params["inlet"], key_name="inlet")
+    metadata["inlet"] = network_params["inlet"]
     metadata["instrument"] = network_params["instrument"]
     metadata["sampling_period"] = str(sampling_period)
     metadata["station_longitude"] = site_info["longitude"]
     metadata["station_latitude"] = site_info["latitude"]
     metadata["station_long_name"] = site_info["long_name"]
-    metadata["data_type"] = "surface"
-    metadata["source_format"] = "btt"
 
     attributes = network_params["global_attributes"]
-    attributes["inlet_height_magl"] = format_inlet(network_params["inlet"], key_name="inlet_height_magl")
+    attributes["inlet_height_magl"] = network_params["inlet"].strip("m")
     attributes.update(metadata)
 
     data = read_csv(data_filepath)
     data["time"] = Timestamp("2019-01-01 00:00") + to_timedelta(data["DOY"] - 1, unit="D")
     data["time"] = data["time"].dt.round(sampling_period_seconds)
     data = data[~isnull(data.time)]
 
@@ -99,10 +90,10 @@
 
         gas_data[species] = {
             "metadata": species_metadata,
             "data": processed_data,
             "attributes": site_attributes,
         }
 
-    gas_data = assign_attributes(data=gas_data, site=site, network=network, update_mismatch=update_mismatch)
+    gas_data = assign_attributes(data=gas_data, site=site, network=network)
 
     return gas_data
```

### Comparing `openghg-0.6.0/openghg/standardise/surface/_cranfield.py` & `openghg-1.0.0/openghg/standardise/surface/_cranfield.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-from pathlib import Path
 from typing import Dict, List, Optional, Union
+from pathlib import Path
 
 
 def parse_cranfield(
     data_filepath: Union[str, Path],
     site: Optional[str] = None,
     network: Optional[str] = None,
     inlet: Optional[str] = None,
     instrument: Optional[str] = None,
     sampling_period: Optional[str] = None,
     measurement_type: Optional[str] = None,
-    **kwargs: Dict,
 ) -> Dict:
     """Creates a CRDS object holding data stored within Datasources
 
     Args:
         filepath: Path of file to load
         data_filepath : Filepath of data to be read
         site: Name of site
         network: Name of network
     Returns:
         dict: Dictionary of gas data
     """
-    from openghg.util import clean_string, format_inlet
     from pandas import read_csv
+    from openghg.util import clean_string
 
     if sampling_period is None:
         sampling_period = "NOT_SET"
 
     data_filepath = Path(data_filepath)
     data = read_csv(data_filepath, parse_dates=["Date"], index_col="Date")
 
@@ -45,25 +44,21 @@
 
     # Convert CH4 and CO to ppb
     data["ch4"] = data["ch4"] * 1e3
     data["ch4 variability"] = data["ch4 variability"] * 1e3
     data["co"] = data["co"] * 1e3
     data["co variability"] = data["co variability"] * 1e3
 
-    inlet = "10m"
-
     metadata = {}
     metadata["site"] = "THB"
     metadata["instrument"] = "CRDS"
     metadata["sampling_period"] = str(sampling_period)
-    metadata["height"] = format_inlet(inlet, key_name="height")
-    metadata["inlet"] = format_inlet(inlet, key_name="inlet")
-    metadata["inlet_height_magl"] = format_inlet(inlet, key_name="inlet_height_magl")
+    metadata["height"] = "10magl"
+    metadata["inlet"] = "10magl"
     metadata["network"] = "CRANFIELD"
-    metadata["data_type"] = "surface"
 
     # TODO - this feels fragile
     species: List[str] = [col for col in data.columns if " " not in col]
 
     combined_data = {}
     # Number of columns of data for each species
     n_cols = 2
```

### Comparing `openghg-0.6.0/openghg/standardise/surface/_crds.py` & `openghg-1.0.0/openghg/standardise/surface/_crds.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,116 +1,84 @@
+from openghg.util import load_json
+from pandas import DataFrame, Timedelta
 from pathlib import Path
 from typing import Dict, Optional, Tuple, Union
 
-from openghg.types import optionalPathType
-from pandas import DataFrame, Timedelta
-
 
 def parse_crds(
     data_filepath: Union[str, Path],
     site: str,
     network: str,
     inlet: Optional[str] = None,
     instrument: Optional[str] = None,
-    sampling_period: Optional[Union[str, float, int]] = None,
+    sampling_period: Optional[str] = None,
     measurement_type: Optional[str] = None,
-    drop_duplicates: bool = True,
-    update_mismatch: str = "never",
-    site_filepath: optionalPathType = None,
-    **kwargs: Dict,
 ) -> Dict:
-    """Parses a CRDS data file and creates a dictionary of xarray Datasets
-    ready for storage in the object store.
+    """Creates a CRDS object holding data stored within Datasources
 
     Args:
         data_filepath: Path to file
         site: Three letter site code
         network: Network name
         inlet: Inlet height
         instrument: Instrument name
-        sampling_period: Sampling period in seconds
+        sampling_period: Sampling period e.g. 2 hour: 2H, 2 minute: 2m
         measurement_type: Measurement type e.g. insitu, flask
-        drop_duplicates: Drop measurements at duplicate timestamps, keeping the first.
-        update_mismatch: This determines how mismatches between the internal data
-            "attributes" and the supplied / derived "metadata" are handled.
-            This includes the options:
-              - "never" - don't update mismatches and raise an AttrMismatchError
-              - "from_source" / "attributes" - update mismatches based on input data (e.g. data attributes)
-              - "from_definition" / "metadata" - update mismatches based on associated data (e.g. site_info.json)
-        site_filepath: Alternative site info file (see openghg/supplementary_data repository for format).
-            Otherwise will use the data stored within openghg_defs/data/site_info JSON file by default.
-
     Returns:
         dict: Dictionary of gas data
     """
     from pathlib import Path
-
     from openghg.standardise.meta import assign_attributes
-    from openghg.util import format_inlet
 
     if not isinstance(data_filepath, Path):
         data_filepath = Path(data_filepath)
 
-    inlet = format_inlet(inlet)
-
     # This may seem like an almost pointless function as this is all we do
     # but it makes it a lot easier to test assign_attributes
     gas_data = _read_data(
         data_filepath=data_filepath,
         site=site,
         network=network,
         inlet=inlet,
         instrument=instrument,
         sampling_period=sampling_period,
         measurement_type=measurement_type,
-        drop_duplicates=drop_duplicates,
     )
 
     # Ensure the data is CF compliant
-    gas_data = assign_attributes(
-        data=gas_data,
-        site=site,
-        sampling_period=sampling_period,
-        update_mismatch=update_mismatch,
-        site_filepath=site_filepath,
-    )
+    gas_data = assign_attributes(data=gas_data, site=site, sampling_period=sampling_period)
 
     return gas_data
 
 
 def _read_data(
     data_filepath: Path,
     site: str,
     network: str,
     inlet: Optional[str] = None,
     instrument: Optional[str] = None,
-    sampling_period: Optional[Union[str, float, int]] = None,
+    sampling_period: Optional[str] = None,
     measurement_type: Optional[str] = None,
-    site_filepath: optionalPathType = None,
-    drop_duplicates: bool = True,
 ) -> Dict:
     """Read the datafile passed in and extract the data we require.
 
     Args:
         data_filepath: Path to file
         site: Three letter site code
         network: Network name
         inlet: Inlet height
         instrument: Instrument name
-        sampling_period: Sampling period in seconds
+        sampling_period: Sampling period including the unit (using pandas frequency aliases like '1H' or '1min')
         measurement_type: Measurement type e.g. insitu, flask
-        site_filepath: Alternative site info file (see openghg/supplementary_data repository for format).
-            Otherwise will use the data stored within openghg_defs/data/site_info JSON file by default.
-        drop_duplicates: Drop measurements at duplicate timestamps, keeping the first.
     Returns:
         dict: Dictionary of gas data
     """
-    import warnings
-    from openghg.util import clean_string, find_duplicate_timestamps, format_inlet, load_internal_json
     from pandas import RangeIndex, read_csv, to_datetime
+    import warnings
+    from openghg.util import clean_string
 
     split_fname = data_filepath.stem.split(".")
     site = site.lower()
 
     try:
         site_fname = clean_string(split_fname[0])
         inlet_fname = clean_string(split_fname[3])
@@ -143,50 +111,41 @@
             index_col="time",
         )
 
     # Drop any rows with NaNs
     # This is now done before creating metadata
     data = data.dropna(axis="rows", how="any")
 
-    dupes = find_duplicate_timestamps(data=data)
-
-    if dupes and not drop_duplicates:
-        raise ValueError(f"Duplicate dates detected: {dupes}")
-
-    data = data.loc[~data.index.duplicated(keep="first")]
-
     # Get the number of gases in dataframe and number of columns of data present for each gas
     n_gases, n_cols = _gas_info(data=data)
 
     header = data.head(2)
     skip_cols = sum([header[column][0] == "-" for column in header.columns])
 
     metadata = _read_metadata(filepath=data_filepath, data=data)
 
     if network is not None:
         metadata["network"] = network
 
     if sampling_period is not None:
-        sampling_period = float(sampling_period)
         # Compare against value extracted from the file name
-        file_sampling_period = Timedelta(seconds=float(metadata["sampling_period"]))
-        given_sampling_period = Timedelta(seconds=sampling_period)
+        file_sampling_period = Timedelta(seconds=metadata["sampling_period"])
 
-        comparison_seconds = abs(given_sampling_period - file_sampling_period).total_seconds()
+        comparison_seconds = abs(sampling_period - file_sampling_period).total_seconds()
         tolerance_seconds = 1
 
         if comparison_seconds > tolerance_seconds:
             raise ValueError(
                 f"Input sampling period {sampling_period} does not match to value "
                 f"extracted from the file name of {metadata['sampling_period']} seconds."
             )
 
     # Read the scale from JSON
     # I'll leave this here for the possible future movement from class to functions
-    network_metadata = load_internal_json(filename="process_gcwerks_parameters.json")
+    network_metadata = load_json(filename="process_gcwerks_parameters.json")
     crds_metadata = network_metadata["CRDS"]
 
     # This dictionary is used to store the gas data and its associated metadata
     combined_data = {}
 
     for n in range(n_gases):
         # Slice the columns
@@ -200,39 +159,36 @@
         column_labels = [
             species,
             f"{species}_variability",
             f"{species}_number_of_observations",
         ]
 
         # Name columns
-        gas_data = gas_data.set_axis(column_labels, axis="columns")
+        gas_data = gas_data.set_axis(column_labels, axis="columns", inplace=False)
 
         header_rows = 2
         # Drop the first two rows now we have the name
-        gas_data = gas_data.drop(index=gas_data.head(header_rows).index)
+        gas_data = gas_data.drop(index=gas_data.head(header_rows).index, inplace=False)
         gas_data.index = to_datetime(gas_data.index, format="%y%m%d %H%M%S")
         # Cast data to float64 / double
         gas_data = gas_data.astype("float64")
 
         # Here we can convert the Dataframe to a Dataset and then write the attributes
         gas_data = gas_data.to_xarray()
 
-        site_attributes = _get_site_attributes(
-            site=site, inlet=inlet, crds_metadata=crds_metadata, site_filepath=site_filepath
-        )
+        site_attributes = _get_site_attributes(site=site, inlet=inlet, crds_metadata=crds_metadata)
 
         scale = crds_metadata["default_scales"].get(species.upper(), "NA")
 
         # Create a copy of the metadata dict
         species_metadata = metadata.copy()
         species_metadata["species"] = clean_string(species)
-        species_metadata["inlet"] = format_inlet(inlet, key_name="inlet")
+        species_metadata["inlet"] = inlet
         species_metadata["calibration_scale"] = scale
         species_metadata["long_name"] = site_attributes["long_name"]
-        species_metadata["data_type"] = "surface"
 
         # Make sure metadata keys are included in attributes
         site_attributes.update(species_metadata)
 
         combined_data[species] = {
             "metadata": species_metadata,
             "data": gas_data,
@@ -247,16 +203,14 @@
 
     Args:
         filepath: Data filepath
         data: Raw pandas DataFrame
     Returns:
         dict: Dictionary containing metadata
     """
-    from openghg.util import format_inlet
-
     # Find gas measured and port used
     type_meas = data[2][2]
     port = data[3][2]
 
     # Split the filename to get the site and resolution
     split_filename = str(filepath.name).split(".")
 
@@ -268,74 +222,52 @@
 
     site = split_filename[0]
     instrument = split_filename[1]
     sampling_period_str = split_filename[2]
     inlet = split_filename[3]
 
     if sampling_period_str == "1minute":
-        sampling_period = "60.0"
+        # sampling_period = "1min"
+        sampling_period = 60
     elif sampling_period_str == "hourly":
-        sampling_period = "3600.0"
+        # sampling_period = "1H"
+        sampling_period = 60 * 60
     else:
         raise ValueError("Unable to read sampling period from filename.")
 
     metadata = {}
     metadata["site"] = site
     metadata["instrument"] = instrument
     metadata["sampling_period"] = str(sampling_period)
-    metadata["inlet"] = format_inlet(inlet, key_name="inlet")
+    metadata["inlet"] = inlet
     metadata["port"] = port
     metadata["type"] = type_meas
 
     return metadata
 
 
-def _get_site_attributes(
-    site: str,
-    inlet: str,
-    crds_metadata: Dict,
-    site_filepath: optionalPathType = None,
-) -> Dict:
+def _get_site_attributes(site: str, inlet: str, crds_metadata: Dict) -> Dict:
     """Gets the site specific attributes for writing to Datsets
 
     Args:
         site: Site name
         inlet: Inlet height, example: 108m
         crds_metadata: General CRDS metadata
-        site_filepath: Alternative site info file (see openghg/supplementary_data repository for format).
-            Otherwise will use the data stored within openghg_defs/data/site_info JSON file by default.
     Returns:
         dict: Dictionary of attributes
     """
-    from openghg.util import get_site_info, format_inlet
-
     try:
         site_attributes: Dict = crds_metadata["sites"][site.upper()]
         global_attributes: Dict = site_attributes["global_attributes"]
     except KeyError:
         raise ValueError(f"Unable to read attributes for site: {site}")
 
-    # TODO - we need to combine the metadata
-    full_site_metadata = get_site_info(site_filepath)
-
     attributes = global_attributes.copy()
 
-    try:
-        metadata = full_site_metadata[site.upper()]
-    except KeyError:
-        pass
-    else:
-        network_key = next(iter(metadata))
-        site_metadata = metadata[network_key]
-        attributes["station_latitude"] = str(site_metadata["latitude"])
-        attributes["station_longitude"] = str(site_metadata["longitude"])
-        attributes["station_long_name"] = site_metadata["long_name"]
-        attributes["station_height_masl"] = site_metadata["height_station_masl"]
-
-    attributes["inlet_height_magl"] = format_inlet(inlet, key_name="inlet_height_magl")
+    attributes["inlet_height_magl"] = inlet
     attributes["comment"] = crds_metadata["comment"]
     attributes["long_name"] = site_attributes["gcwerks_site_name"]
 
     return attributes
 
 
 def _gas_info(data: DataFrame) -> Tuple[int, int]:
```

### Comparing `openghg-0.6.0/openghg/standardise/surface/_eurocom.py` & `openghg-1.0.0/openghg/standardise/surface/_eurocom.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,34 @@
-from pathlib import Path
 from typing import Dict, Optional, Union
+from pathlib import Path
 
 
 def parse_eurocom(
     data_filepath: Union[str, Path],
     site: str,
     sampling_period: str,
     network: Optional[str] = None,
     inlet: Optional[str] = None,
     instrument: Optional[str] = None,
-    update_mismatch: str = "never",
 ) -> Dict:
     """Parses EUROCOM data files into a format expected by OpenGHG
 
     Args:
         data_filepath: Path of file to read
         site: Site code
         sampling_period: Sampling period in seconds
         network: Network name
         Inlet: Inlet height in metres
         Instrument: Instrument name
-        update_mismatch: This determines how mismatches between the internal data
-            "attributes" and the supplied / derived "metadata" are handled.
-            This includes the options:
-              - "never" - don't update mismatches and raise an AttrMismatchError
-              - "from_source" / "attributes" - update mismatches based on input data (e.g. data attributes)
-              - "from_definition" / "metadata" - update mismatches based on associated data (e.g. site_info.json)
     Returns:
         dict: Dictionary of measurement data
     """
     from openghg.standardise.meta import assign_attributes, get_attributes
-    from openghg.util import load_internal_json, read_header, format_inlet
-    from pandas import Timestamp, read_csv
+    from pandas import read_csv, Timestamp
+    from openghg.util import read_header, load_json
 
     data_filepath = Path(data_filepath)
 
     if site is None:
         site = data_filepath.stem.split("_")[0]
 
     if sampling_period is None:
@@ -100,22 +93,22 @@
     data = data[data[species.lower()] >= 0.0]
     data = data.dropna(axis="rows", how="any")
     # Drop duplicate indices
     data = data.loc[~data.index.duplicated(keep="first")]
     # Convert to xarray Dataset
     data = data.to_xarray()
 
-    attributes_data = load_internal_json(filename="attributes.json")
+    attributes_data = load_json(filename="attributes.json")
     eurocom_attributes = attributes_data["EUROCOM"]
     global_attributes = eurocom_attributes["global_attributes"]
 
     if inlet_height == "NA":
         try:
             inlet = eurocom_attributes["intake_height"][site]
-            global_attributes["inlet_height_m"] = format_inlet(inlet, key_name="inlet_height_m")
+            global_attributes["inlet_height_m"] = inlet
             calibration_scale = eurocom_attributes["calibration"][site]
         except KeyError:
             calibration_scale = {}
             raise ValueError(f"Unable to find inlet from filename or attributes file for {site}")
 
     gas_data = get_attributes(
         ds=data,
@@ -125,24 +118,21 @@
         units="ppm",
     )
 
     # Create a copy of the metadata dict
     metadata = {}
     metadata["site"] = site
     metadata["species"] = species
-    metadata["inlet"] = format_inlet(global_attributes["inlet_height_m"], key_name="inlet")
+    metadata["inlet_height"] = global_attributes["inlet_height_m"]
     metadata["calibration_scale"] = calibration_scale
     metadata["network"] = "EUROCOM"
     metadata["sampling_period"] = str(sampling_period)
-    metadata["data_type"] = "surface"
 
     combined_data[species] = {
         "metadata": metadata,
         "data": gas_data,
         "attributes": global_attributes,
     }
 
-    combined_data = assign_attributes(
-        data=combined_data, site=site, sampling_period=sampling_period, update_mismatch=update_mismatch
-    )
+    combined_data = assign_attributes(data=combined_data, site=site, sampling_period=sampling_period)
 
     return combined_data
```

### Comparing `openghg-0.6.0/openghg/standardise/surface/_gcwerks.py` & `openghg-1.0.0/openghg/standardise/surface/_gcwerks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,11 @@
+from typing import Dict, List, Optional, Union, Tuple
 from pathlib import Path
-from typing import Dict, List, Optional, Tuple, Union
 from pandas import DataFrame
 
-from openghg.types import optionalPathType
-
 
 def find_files(
     data_path: Union[str, Path], skip_str: Union[str, List[str]] = "sf6"
 ) -> List[Tuple[Path, Path]]:
     """A helper file to find GCWERKS data and precisions file in a given folder.
     It searches for .C files of the format macehead.19.C, looks for a precisions file
     named macehead.19.precions.C and if it exists creates a tuple for these files.
@@ -57,47 +55,36 @@
     precision_filepath: Union[str, Path],
     site: str,
     network: str,
     inlet: Optional[str] = None,
     instrument: Optional[str] = None,
     sampling_period: Optional[str] = None,
     measurement_type: Optional[str] = None,
-    update_mismatch: str = "never",
-    site_filepath: optionalPathType = None,
 ) -> Dict:
     """Reads a GC data file by creating a GC object and associated datasources
 
     Args:
         data_filepath: Path of data file
         precision_filepath: Path of precision file
         site: Three letter code or name for site
         instrument: Instrument name
         network: Network name
-        update_mismatch: This determines how mismatches between the internal data
-            "attributes" and the supplied / derived "metadata" are handled.
-            This includes the options:
-              - "never" - don't update mismatches and raise an AttrMismatchError
-              - "from_source" / "attributes" - update mismatches based on input data (e.g. data attributes)
-              - "from_definition" / "metadata" - update mismatches based on associated data (e.g. site_info.json)
-        site_filepath: Alternative site info file (see openghg/supplementary_data repository for format).
-            Otherwise will use the data stored within openghg_defs/data/site_info JSON file by default.
     Returns:
         dict: Dictionary of source_name : UUIDs
     """
     from pathlib import Path
-
     from openghg.standardise.meta import assign_attributes
-    from openghg.util import clean_string, load_internal_json
+    from openghg.util import clean_string, load_json
 
     data_filepath = Path(data_filepath)
     precision_filepath = Path(precision_filepath)
 
     # Do some setup for processing
     # Load site data
-    gcwerks_data = load_internal_json(filename="process_gcwerks_parameters.json")
+    gcwerks_data = load_json(filename="process_gcwerks_parameters.json")
     gc_params = gcwerks_data["GCWERKS"]
 
     network = clean_string(network)
     # We don't currently do anything with inlet here as it's always read from data
     # or taken from process_gcwerks_parameters.json
     if inlet is not None:
         inlet = clean_string(inlet)
@@ -131,17 +118,15 @@
         instrument=instrument,
         network=network,
         sampling_period=sampling_period,
         gc_params=gc_params,
     )
 
     # Assign attributes to the data for CF compliant NetCDFs
-    gas_data = assign_attributes(
-        data=gas_data, site=site, update_mismatch=update_mismatch, site_filepath=site_filepath
-    )
+    gas_data = assign_attributes(data=gas_data, site=site)
 
     return gas_data
 
 
 def _check_site(filepath: Path, site_code: str, gc_params: Dict) -> str:
     """Check if the site passed in matches that in the filename
 
@@ -228,17 +213,16 @@
         instrument: Instrument name
         network: Network name
         gc_params: GCWERKS parameters
         sampling_period: Period over which the measurement was samplied.
     Returns:
         dict: Dictionary of gas data keyed by species
     """
-    from pandas import Series
+    from pandas import read_csv, to_datetime, Series
     from pandas import Timedelta as pd_Timedelta
-    from pandas import read_csv, to_datetime
 
     # Read header
     header = read_csv(data_filepath, skiprows=2, nrows=2, header=None, sep=r"\s+")
 
     # Read the data in and automatically create a datetime column from the 5 columns
     # Dropping the yyyy', 'mm', 'dd', 'hh', 'mi' columns here
     data = read_csv(
@@ -260,17 +244,16 @@
     }
 
     extracted_sampling_period = _get_sampling_period(instrument=instrument, gc_params=gc_params)
     metadata["sampling_period"] = extracted_sampling_period
 
     if sampling_period is not None:
         # Compare input to definition within json file
-        file_sampling_period_td = pd_Timedelta(seconds=float(extracted_sampling_period))
-        sampling_period_td = pd_Timedelta(seconds=float(sampling_period))
-        comparison_seconds = abs(sampling_period_td - file_sampling_period_td).total_seconds()
+        file_sampling_period = pd_Timedelta(seconds=extracted_sampling_period)
+        comparison_seconds = abs(sampling_period - file_sampling_period).total_seconds()
         tolerance_seconds = 1
 
         if comparison_seconds > tolerance_seconds:
             raise ValueError(
                 f"Input sampling period {sampling_period} does not match to value "
                 f"extracted from the file name of {metadata['sampling_period']} seconds."
             )
@@ -353,17 +336,16 @@
 
     Args:
         filepath: Path of precision file
     Returns:
         tuple (Pandas.DataFrame, list): Precision DataFrame and list of species in
         precision data
     """
-    from datetime import datetime
-
     from pandas import read_csv
+    from datetime import datetime
 
     # Function for parsing datetime
     def prec_date_parser(date: str) -> datetime:
         return datetime.strptime(date, "%y%m%d")
 
     # Read precision species
     precision_header = read_csv(filepath, skiprows=3, nrows=1, header=None, sep=r"\s+")
@@ -407,19 +389,21 @@
         metadata: Dictionary of metadata
         units: Dictionary of units for each species
         scale: Dictionary of scales for each species
         gc_params: GCWERKS parameter dictionary
     Returns:
         dict: Dataframe of gas data and metadata
     """
+    from addict import Dict as aDict
     from fnmatch import fnmatch
+    from openghg.util import load_json, clean_string
 
-    from addict import Dict as aDict
-    from openghg.util import format_inlet
-    from openghg.standardise.meta import define_species_label
+    # Load species translator so we can keep species names consistent
+    attributes_data = load_json("attributes.json")
+    species_translator = attributes_data["species_translation"]
 
     # Read inlets from the parameters
     expected_inlets = _get_inlets(site_code=site, gc_params=gc_params)
 
     try:
         data_inlets = data["Inlet"].unique().tolist()
     except KeyError:
@@ -432,15 +416,14 @@
     for spec in species:
         # Skip this species if the data is all NaNs
         if data[spec].isnull().all():
             continue
 
         # Here inlet is the inlet in the data and inlet_label is the label we want to use as metadata
         for inlet, inlet_label in expected_inlets.items():
-            inlet_label = format_inlet(inlet_label)
             # Create a copy of metadata for local modification
             spec_metadata = metadata.copy()
             spec_metadata["units"] = units[spec]
             spec_metadata["calibration_scale"] = scale[spec]
 
             # If we've only got a single inlet
             if inlet == "any" or inlet == "air":
@@ -508,20 +491,21 @@
             )
             attributes = attributes.copy()
 
             # We want an xarray Dataset
             spec_data = spec_data.to_xarray()
 
             # Create a standardised / cleaned species label
-            comp_species = define_species_label(spec)[0]
+            try:
+                comp_species = species_translator[spec.upper()]["chem"]
+            except KeyError:
+                comp_species = clean_string(spec.lower())
 
             # Add the cleaned species name to the metadata and alternative name if present
             spec_metadata["species"] = comp_species
-            spec_metadata["data_type"] = "surface"
-
             if comp_species != spec.lower() and comp_species != spec.upper():
                 spec_metadata["species_alt"] = spec
 
             # Rename variables so they have lowercase and alphanumeric names
             to_rename = {}
             for var in spec_data.variables:
                 if spec in var:
@@ -595,22 +579,20 @@
         site: Site code
         inlet: Inlet height in metres
         instrument: Instrument name
         gc_params: GCWERKS parameters
     Returns:
         dict: Dictionary of attributes
     """
-    from openghg.util import format_inlet
-
     site = site.upper()
     instrument = instrument.lower()
 
     attributes: Dict[str, str] = gc_params["sites"][site]["global_attributes"]
 
-    attributes["inlet_height_magl"] = format_inlet(inlet, key_name="inlet_height_magl")
+    attributes["inlet_height_magl"] = inlet
     try:
         attributes["comment"] = gc_params["comment"][instrument]
     except KeyError:
         valid_instruments = list(gc_params["comment"].keys())
         raise KeyError(f"Invalid instrument {instrument} passed, valid instruments : {valid_instruments}")
 
     return attributes
```

### Comparing `openghg-0.6.0/openghg/standardise/surface/_glasgow_licor.py` & `openghg-1.0.0/openghg/standardise/surface/_glasgow_licor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
+from pandas import read_csv, to_datetime
 from pathlib import Path
 from typing import Dict, Optional
-
 from addict import Dict as aDict
-from pandas import read_csv, to_datetime
 
 
-def parse_glasow_licor(filepath: Path, sampling_period: Optional[str] = None, **kwargs: Dict) -> Dict:
+def parse_glasow_licor(filepath: Path, sampling_period: Optional[str] = None) -> Dict:
     """Read the Glasgow LICOR data from NPL
 
     Args:
         filepath: Path to data file
     Returns:
         dict: Dictionary of data
     """
@@ -38,15 +37,14 @@
     if sampling_period is None:
         sampling_period = "NOT_SET"
 
     metadata = {
         "units": "ppb",
         "notes": "measurement value is methane enhancement over background",
         "sampling_period": sampling_period,
-        "data_type": "surface",
     }
 
     data = aDict()
     data["ch4"]["metadata"] = metadata
     data["ch4"]["data"] = ds
 
     to_return: Dict = data.to_dict()
```

### Comparing `openghg-0.6.0/openghg/standardise/surface/_glasgow_picarro.py` & `openghg-1.0.0/openghg/standardise/surface/_glasgow_picarro.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,30 @@
+import pandas as pd
+from typing import Dict, Union, Optional
 from pathlib import Path
-from typing import Dict, Optional, Union
 from warnings import warn
-
-import pandas as pd
 from addict import Dict as aDict
 
 
 def parse_glasow_picarro(
     data_filepath: Union[str, Path],
     site: str,
     network: str,
     inlet: str,
     instrument: str = "picarro",
     sampling_period: Optional[str] = None,
-    measurement_type: str = "surface",
-    **kwargs: Dict,
+    measurement_type: str = "timeseries",
 ) -> Dict:
     """Read the Glasgow Science Tower Picarro data
 
     Args:
         data_filepath: Path to data file
     Returns:
         dict: Dictionary of processed data
     """
-    from openghg.util import format_inlet
-
     warn(message="Temporary function used to read Glasgow Science Tower Picarro data")
 
     df = pd.read_csv(data_filepath, index_col=[0], parse_dates=True)
     df = df.dropna(axis="rows", how="any")
     # We just want the concentration values for now
     species = ["co2", "ch4"]
     rename_cols = {f" {s}_C": s for s in species}
@@ -42,27 +38,24 @@
     if sampling_period is None:
         sampling_period = "NOT_SET"
 
     gas_data = aDict()
     for s in species:
         gas_data[s]["data"] = df[[s]].to_xarray()
 
-        inlet = format_inlet("124m")
-
         gas_data[s]["metadata"] = {
             "species": s,
             "long_name": long_site_name,
             "latitude": 55.859238,
             "longitude": -4.296180,
             "network": "npl_picarro",
-            "inlet": inlet,
+            "inlet": "124m",
             "sampling_period": sampling_period,
             "site": site,
             "instrument": "picarro",
             "units": units[s],
-            "data_type": "surface",
         }
 
     # TODO - remove this once mypy stubs for addict are added
     to_return: Dict = gas_data.to_dict()
 
     return to_return
```

### Comparing `openghg-0.6.0/openghg/standardise/surface/_icos.py` & `openghg-1.0.0/openghg/store/_obssurface.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,413 +1,393 @@
+from openghg.store.base import BaseStore
+from openghg.types import pathType, multiPathType, resultsType
 from pathlib import Path
-from typing import Dict, Optional, Union
-import logging
+from typing import DefaultDict, Dict, Optional, Union
 
-from openghg.types import optionalPathType
 
-logger = logging.getLogger("openghg.standardise.surface")
-logger.setLevel(logging.DEBUG)  # Have to set level for logger as well as handler
+__all__ = ["ObsSurface"]
 
 
-def parse_icos(
-    data_filepath: Union[str, Path],
-    site: str,
-    inlet: str,
-    instrument: str,
-    network: str = "ICOS",
-    sampling_period: Optional[str] = None,
-    measurement_type: Optional[str] = None,
-    header_type: str = "large",
-    update_mismatch: str = "never",
-    site_filepath: optionalPathType = None,
-    **kwargs: Dict,
-) -> Dict:
-    """Parses an ICOS data file and creates a dictionary containing the Dataset and metadata
-
-    Args:
-        data_filepath: Path to file
-        site: Three letter site code
-        network: Network name
-        inlet: Inlet height
-        instrument: Instrument name
-        sampling_period: Sampling period e.g. 2 hour: 2H, 2 minute: 2m
-        measurement_type: Measurement type e.g. insitu, flask
-        header_type: ICOS data file with large (40 line) header or shorter single line header
-            Options: large, small
-        update_mismatch: This determines how mismatches between the internal data
-            "attributes" and the supplied / derived "metadata" are handled.
-            This includes the options:
-              - "never" - don't update mismatches and raise an AttrMismatchError
-              - "from_source" / "attributes" - update mismatches based on input data (e.g. data attributes)
-              - "from_definition" / "metadata" - update mismatches based on associated data (e.g. site_info.json)
-        site_filepath: Alternative site info file (see openghg/supplementary_data repository for format).
-            Otherwise will use the data stored within openghg_defs/data/site_info JSON file by default.
-    Returns:
-        dict: Dictionary of gas data
-    """
-    from pathlib import Path
-
-    from openghg.standardise.meta import assign_attributes
-    from openghg.util import clean_string, format_inlet
-
-    site = clean_string(site)
-    instrument = clean_string(instrument)
-    network = clean_string(network)
-    sampling_period = clean_string(sampling_period)
-    measurement_type = clean_string(measurement_type)
+class ObsSurface(BaseStore):
+    """This class is used to process surface observation data"""
 
-    inlet = clean_string(inlet)
-    inlet = format_inlet(inlet)
+    _root = "ObsSurface"
+    _uuid = "da0b8b44-6f85-4d3c-b6a3-3dde34f6dea1"
+
+    @staticmethod
+    def read_file(
+        filepath: multiPathType,
+        data_type: str,
+        network: str,
+        site: str,
+        inlet: Optional[str] = None,
+        instrument: Optional[str] = None,
+        sampling_period: Optional[str] = None,
+        measurement_type: str = "insitu",
+        overwrite: bool = False,
+    ) -> Dict:
+        """Process files and store in the object store. This function
+            utilises the process functions of the other classes in this submodule
+            to handle each data type.
+
+        Args:
+            filepath: Filepath(s)
+            data_type: Data type, for example CRDS, GCWERKS
+            site: Site code/name
+            network: Network name
+            inlet: Inlet height. If retrieve multiple files pass None, OpenGHG will attempt to
+            read inlets from data.
+            instrument: Instrument name
+            sampling_period: Sampling period in pandas style (e.g. 2H for 2 hour period, 2m for 2 minute period).
+            measurement_type: Type of measurement e.g. insitu, flask
+            overwrite: Overwrite previously uploaded data
+        Returns:
+            dict: Dictionary of Datasource UUIDs
+        """
+        from collections import defaultdict
+        from pathlib import Path
+        from pandas import Timedelta
+        import sys
+        from tqdm import tqdm
+        from openghg.util import load_surface_parser, hash_file, clean_string, verify_site
+        from openghg.types import SurfaceTypes
+        from openghg.store import assign_data
+
+        if not isinstance(filepath, list):
+            filepath = [filepath]
+
+        try:
+            data_type = SurfaceTypes[data_type.upper()].value
+        except KeyError:
+            raise ValueError(f"Unknown data type {data_type} selected.")
+
+        # Test that the passed values are valid
+        # Check validity of site, instrument, inlet etc in acrg_site_info.json
+        # Clean the strings
+        site = verify_site(site=site)
+
+        network = clean_string(network)
+        inlet = clean_string(inlet)
+        instrument = clean_string(instrument)
+        sampling_period = clean_string(sampling_period)
+
+        sampling_period_seconds: Union[str, None] = None
+        # If we have a sampling period passed we want the number of seconds
+        if sampling_period is not None:
+            sampling_period_seconds = str(Timedelta(sampling_period).total_seconds())
+
+        # Load the data retrieve object
+        parser_fn = load_surface_parser(data_type=data_type)
+
+        obs = ObsSurface.load()
+
+        results: resultsType = defaultdict(dict)
+
+        # Create a progress bar object using the filepaths, iterate over this below
+        with tqdm(total=len(filepath), file=sys.stdout) as progress_bar:
+            for fp in filepath:
+                if data_type == "GCWERKS":
+                    try:
+                        data_filepath = Path(fp[0])
+                        precision_filepath = Path(fp[1])
+                    except ValueError:
+                        raise ValueError("For GCWERKS data both data and precision filepaths must be given.")
+                else:
+                    data_filepath = Path(fp)
+
+                # try:
+                file_hash = hash_file(filepath=data_filepath)
+                if file_hash in obs._file_hashes and overwrite is False:
+                    print(
+                        f"This file has been uploaded previously with the filename : {obs._file_hashes[file_hash]} - skipping."
+                    )
+
+                progress_bar.set_description(f"Processing: {data_filepath.name}")
+
+                if data_type == "GCWERKS":
+                    data = parser_fn(
+                        data_filepath=data_filepath,
+                        precision_filepath=precision_filepath,
+                        site=site,
+                        network=network,
+                        inlet=inlet,
+                        instrument=instrument,
+                        sampling_period=sampling_period_seconds,
+                        measurement_type=measurement_type,
+                    )
+                else:
+                    data = parser_fn(
+                        data_filepath=data_filepath,
+                        site=site,
+                        network=network,
+                        inlet=inlet,
+                        instrument=instrument,
+                        sampling_period=sampling_period_seconds,
+                        measurement_type=measurement_type,
+                    )
+
+                # Extract the metadata for each set of measurements to perform a Datasource lookup
+                metadata = {key: data["metadata"] for key, data in data.items()}
+
+                lookup_results = obs.datasource_lookup(metadata=metadata)
+
+                # Create Datasources, save them to the object store and get their UUIDs
+                datasource_uuids = assign_data(
+                    data_dict=data, lookup_results=lookup_results, overwrite=overwrite
+                )
+
+                results["processed"][data_filepath.name] = datasource_uuids
+
+                # Record the Datasources we've created / appended to
+                obs.add_datasources(datasource_uuids, metadata)
+
+                # Store the hash as the key for easy searching, store the filename as well for
+                # ease of checking by user
+                obs._file_hashes[file_hash] = data_filepath.name
+                # except Exception:
+                #     results["error"][data_filepath.name] = traceback.format_exc()
+
+                progress_bar.update(1)
+
+        # Save this object back to the object store
+        obs.save()
+
+        return results
+
+    @staticmethod
+    def read_multisite_aqmesh(
+        data_filepath: pathType,
+        metadata_filepath: pathType,
+        network: str = "aqmesh_glasgow",
+        instrument: str = "aqmesh",
+        sampling_period: int = 60,
+        measurement_type: str = "insitu",
+        overwrite: bool = False,
+    ) -> DefaultDict:
+        """Read AQMesh data for the Glasgow network
+
+        NOTE - temporary function until we know what kind of AQMesh data
+        we'll be retrieve in the future.
+
+        This data is different in that it contains multiple sites in the same file.
+        """
+        from openghg.standardise.surface import parse_aqmesh
+        from openghg.store import assign_data
+        from openghg.util import hash_file
+        from collections import defaultdict
+        from tqdm import tqdm
 
-    if not isinstance(data_filepath, Path):
         data_filepath = Path(data_filepath)
+        metadata_filepath = Path(metadata_filepath)
 
-    if header_type == "large":
-        gas_data = _read_data_large_header(
-            data_filepath=data_filepath,
-            site=site,
-            inlet=inlet,
-            network=network,
-            instrument=instrument,
-            sampling_period=sampling_period,
-            measurement_type=measurement_type,
-        )
-    else:
-        gas_data = _read_data_small_header(
-            data_filepath=data_filepath,
-            site=site,
-            inlet=inlet,
-            network=network,
-            instrument=instrument,
-            sampling_period=sampling_period,
-            measurement_type=measurement_type,
-        )
-
-    # Ensure the data is CF compliant
-    gas_data = assign_attributes(
-        data=gas_data,
-        site=site,
-        sampling_period=sampling_period,
-        update_mismatch=update_mismatch,
-        site_filepath=site_filepath,
-    )
-
-    return gas_data
-
-
-def _read_data_large_header(
-    data_filepath: Path,
-    site: str,
-    inlet: str,
-    network: str,
-    instrument: str,
-    sampling_period: Optional[str] = None,
-    measurement_type: Optional[str] = None,
-    **kwargs: Dict,
-) -> Dict:
-    """Parses ICOS files with the larger (~40) line header
-
-    Args:
-        data_filepath: Path to file
-        site: Three letter site code
-        network: Network name
-        inlet: Inlet height
-        instrument: Instrument name
-        sampling_period: Sampling period e.g. 2 hour: 2H, 2 minute: 2m
-        measurement_type: Measurement type e.g. insitu, flask
-    Returns:
-        dict: Dictionary of gas data
-    """
-    from openghg.util import read_header, format_inlet
-    from pandas import read_csv, to_datetime
-
-    # Read metadata from the filename and cross check to make sure the passed
-    # arguments match
-    split_filename = data_filepath.name.split(".")
-
-    try:
-        site_fname = split_filename[0]
-        species_fname = split_filename[1]
-        file_sampling_period = split_filename[2]
-        instrument_fname = split_filename[3]
-        inlet_height_fname = split_filename[4]
-    except IndexError:
-        raise ValueError(
-            "Unable to read metadata from filename. We expect a filename such as mhd.ch4.hourly.g2401.15m.dat"
-        )
-
-    if site_fname.lower() != site:
-        raise ValueError("Site mismatch between site argument passed and filename.")
-
-    inlet_height_fname = format_inlet(inlet_height_fname)
-    if inlet is not None and inlet_height_fname.lower() != inlet:
-        raise ValueError("Mismatch between inlet height passed and in filename.")
-
-    if instrument is not None and instrument_fname.lower() != instrument:
-        raise ValueError("Mismatch between instrument passed and that in filename.")
-
-    # Read the header and check its length
-    header = read_header(filepath=data_filepath)
-    len_header = len(header)
-
-    if len_header != 40:
-        logger.warning(
-            f"We expect a header length of 40 but got {len_header}, \
-            note that some metadata may not be collected, \
-            please raise an issue on GitHub if this file format is to be expected."
-        )
-
-    dtypes = {
-        "#Site": "string",
-        "SamplingHeight": "string",
-        "DecimalDate": "float",
-        "Stdev": "float",
-        "NbPoints": "int",
-        "Flag": "string",
-        "InstrumentId": "int",
-        "QualityId": "string",
-        "InternalFlag": "string",
-        "AutoDescriptiveFlag": "string",
-        "ManualDescriptiveFlag": "string",
-    }
-
-    df = read_csv(
-        data_filepath,
-        header=len_header - 1,
-        sep=";",
-        parse_dates={"time": [2, 3, 4, 5, 6]},
-        index_col="time",
-        na_values=["-9.990", "-999.990"],
-        dtype=dtypes,
-    )
-
-    df.index = to_datetime(df.index, format="%Y %m %d %H %M")
-
-    # Lowercase all the column titles
-    df.columns = [str(c).lower() for c in df.columns]
-
-    # Read some metadata before dropping the columns
-    # sampling_height_data = df["samplingheight"][0]
-    site_name_data = df["#site"][0]
-    species_name_data = df.columns[3]
-
-    if site != site_name_data.lower():
-        raise ValueError("Site mismatch between site argument passed and site in data.")
-
-    if species_fname != species_name_data.lower():
-        raise ValueError("Speices mismatch between site passed and species in data.")
-
-    # Drop the columns we don't want
-    cols_to_keep = [species_name_data, "stdev", "nbpoints", "flag", "instrumentid"]
-    df = df[cols_to_keep]
-
-    # Remove rows with NaNs in the species or stdev columns
-    df = df.dropna(axis="rows", subset=[species_name_data, "stdev"])
-
-    # Drop duplicate indices
-    df = df.loc[~df.index.duplicated(keep="first")]
-
-    # Check if the index is sorted
-    if not df.index.is_monotonic_increasing:
-        df = df.sort_index()
-
-    rename_dict = {
-        "stdev": species_name_data + " variability",
-        "nbpoints": species_name_data + " number_of_observations",
-    }
-
-    df = df.rename(columns=rename_dict)
-
-    # Convert to xarray Dataset
-    data = df.to_xarray()
-
-    data["flag"] = data["flag"].astype(str)
-
-    if file_sampling_period == "1minute":
-        file_sampling_period = "60.0"
-    elif file_sampling_period == "hourly":
-        file_sampling_period = "3600.0"
-
-    if sampling_period is not None:
-        if file_sampling_period != sampling_period:
-            raise ValueError("Mismatch between sampling period read from filename and that passed.")
-    else:
-        sampling_period = file_sampling_period
-
-    metadata = {
-        "site": site,
-        "species": species_name_data,
-        "inlet": inlet_height_fname,
-        "sampling_period": file_sampling_period,
-        "network": network,
-        "instrument": instrument_fname,
-    }
-
-    if measurement_type is not None:
-        metadata["measurement_type"] = measurement_type
-
-    unit_line = header[22]
-    if "MEASUREMENT UNIT" in unit_line:
-        units = unit_line.split(":")[1].lower().strip()
-        metadata["units"] = units
-
-    scale_line = header[26]
-    if "MEASUREMENT SCALE" in scale_line:
-        calibration_scale = scale_line.split(":")[1].lower().lstrip(" ").replace(" ", "_").strip()
-        metadata["calibration_scale"] = calibration_scale
-
-    data_owner_line = header[18]
-    if "CONTACT POINT" in data_owner_line:
-        data_owner_email = data_owner_line.split(":")[1].split(",")[1].strip()
-        metadata["data_owner_email"] = data_owner_email
-
-    species_data = {
-        species_name_data: {
-            "metadata": metadata,
-            "data": data,
-        }
-    }
-
-    return species_data
-
-
-def _read_data_small_header(
-    data_filepath: Path,
-    site: str,
-    inlet: str,
-    network: str,
-    instrument: str,
-    sampling_period: Optional[str] = None,
-    measurement_type: Optional[str] = None,
-) -> Dict:
-    """Parses ICOS files with a single line header
-
-    Args:
-        data_filepath: Path to file
-        site: Three letter site code
-        network: Network name
-        inlet: Inlet height
-        instrument: Instrument name
-        sampling_period: Sampling period e.g. 2 hour: 2H, 2 minute: 2m
-        measurement_type: Measurement type e.g. insitu, flask
-    Returns:
-        dict: Dictionary of gas data
-    """
-    from openghg.util import read_header, format_inlet
-    from pandas import Timestamp, read_csv
-
-    # Read some metadata from the filename
-    split_filename = data_filepath.name.split(".")
-
-    try:
-        site_fname = split_filename[0]
-        species_fname = split_filename[1]
-        file_sampling_period = split_filename[2]
-        inlet_height = split_filename[3]
-    except IndexError:
-        raise ValueError(
-            "Unable to read metadata from filename. We expect a filename such as tta.co2.1minute.222m.dat"
-        )
-
-    # metadata = read_metadata(filepath=data_filepath, data=data, data_type="ICOS")
-    header = read_header(filepath=data_filepath)
-    n_skip = len(header) - 1
-
-    def date_parser(year: str, month: str, day: str, hour: str, minute: str) -> Timestamp:
-        return Timestamp(year, month, day, hour, minute)
-
-    datetime_columns = {"time": ["Year", "Month", "Day", "Hour", "Minute"]}
-
-    use_cols = [
-        "Year",
-        "Month",
-        "Day",
-        "Hour",
-        "Minute",
-        str(species_fname.lower()),
-        "Stdev",
-        "NbPoints",
-    ]
-
-    dtypes = {
-        "Day": int,
-        "Month": int,
-        "Year": int,
-        "Hour": int,
-        "Minute": int,
-        species_fname.lower(): float,
-        "Stdev": float,
-        "SamplingHeight": float,
-        "NbPoints": int,
-    }
-
-    data = read_csv(
-        data_filepath,
-        skiprows=n_skip,
-        parse_dates=datetime_columns,
-        index_col="time",
-        sep=" ",
-        usecols=use_cols,
-        dtype=dtypes,
-        na_values="-999.99",
-        date_parser=date_parser,
-    )
-
-    data = data[data[species_fname.lower()] >= 0.0]
-
-    # Drop duplicate indices
-    data = data.loc[~data.index.duplicated(keep="first")]
-
-    # Check if the index is sorted
-    if not data.index.is_monotonic_increasing:
-        data = data.sort_index()
-
-    rename_dict = {
-        "Stdev": species_fname + " variability",
-        "NbPoints": species_fname + " number_of_observations",
-    }
-
-    data = data.rename(columns=rename_dict)
-
-    # Convert to xarray Dataset
-    data = data.to_xarray()
-
-    if site_fname.lower() != site:
-        raise ValueError("Site mismatch between site argument passed and filename")
-
-    inlet_height = format_inlet(inlet_height)
-    if inlet_height.lower() != inlet:
-        raise ValueError("Mismatch between inlet height passed and in filename")
-
-    if file_sampling_period == "1minute":
-        file_sampling_period = "60.0"
-    elif file_sampling_period == "1hour":
-        file_sampling_period = "3600.0"
-
-    if sampling_period is not None:
-        if file_sampling_period != sampling_period:
-            raise ValueError("Mismatch between sampling period read from filename and that passed in.")
-    else:
-        sampling_period = file_sampling_period
-
-    metadata = {
-        "site": site,
-        "species": species_fname,
-        "inlet": inlet_height,
-        "sampling_period": sampling_period,
-        "network": network,
-        "instrument": instrument,
-        "data_type": "surface",
-        "source_format": "icos",
-    }
-
-    if measurement_type is not None:
-        metadata["measurement_type"] = measurement_type
-
-    species_data = {
-        species_fname: {
-            "metadata": metadata,
-            "data": data,
-        }
-    }
+        # Load the ObsSurface object for retrieve
+        obs = ObsSurface.load()
+        # Get a dict of data and metadata
+        processed_data = parse_aqmesh(data_filepath=data_filepath, metadata_filepath=metadata_filepath)
+
+        results: resultsType = defaultdict(dict)
+        for site, site_data in tqdm(processed_data.items()):
+            metadata = site_data["metadata"]
+            measurement_data = site_data["data"]
+
+            inlet = metadata["inlet"]
+            species = metadata["species"]
+
+            file_hash = hash_file(filepath=data_filepath)
+
+            if obs.seen_hash(file_hash=file_hash) and overwrite is False:
+                raise ValueError(
+                    f"This file has been uploaded previously with the filename : {obs._file_hashes[file_hash]}."
+                )
+
+            uuid = obs.lookup_uuid(
+                site=site,
+                network=network,
+                inlet=inlet,
+                species=species,
+                sampling_period=sampling_period,
+            )
+
+            # Jump through these hoops until we can rework the data assignment functionality to split it out
+            # into more sensible functions
+            # TODO - fix the assign data function to avoid this kind of hoop jumping
+            combined = {site: {"data": measurement_data, "metadata": metadata}}
+            lookup_result = {site: uuid}
+
+            # Create Datasources, save them to the object store and get their UUIDs
+            datasource_uuids = assign_data(
+                data_dict=combined, lookup_results=lookup_result, overwrite=overwrite
+            )
+
+            results[site] = datasource_uuids
+
+            # TODO - fix add_datasources as well
+            _metadata = {site: metadata}
+
+            # Record the Datasources we've created / appended to
+            obs.add_datasources(datasource_uuids=datasource_uuids, metadata=_metadata)
+
+            # Store the hash as the key for easy searching, store the filename as well for
+            # ease of checking by user
+            obs.set_hash(file_hash=file_hash, filename=data_filepath.name)
+
+        obs.save()
+
+        return results
+
+    def datasource_lookup(self, metadata: Dict) -> Dict:
+        """Find the Datasource we should assign the data to
+
+        Args:
+            metadata: Dictionary of metadata returned from the data_obj.read_file function
+        Returns:
+            dict: Dictionary of datasource information
+        """
+        lookup_results = {}
+        for key, data in metadata.items():
+            site = data["site"]
+            network = data["network"]
+            inlet = data["inlet"]
+            sampling_period = data["sampling_period"]
+
+            # TODO - remove these once further checks for metadata inputs are in place
+            if inlet is None:
+                raise ValueError("No valid inlet height.")
+
+            if sampling_period is None:
+                raise ValueError("No valid sampling period.")
+
+            species = data["species"]
+
+            lookup_results[key] = self.lookup_uuid(
+                site=site,
+                network=network,
+                inlet=inlet,
+                species=species,
+                sampling_period=sampling_period,
+            )
+
+        return lookup_results
+
+    def add_datasources(self, datasource_uuids: Dict, metadata: Dict) -> None:
+        """Add the passed list of Datasources to the current list
+
+        Args:
+            datasource_uuids: Datasource UUIDs
+            metadata: Metadata for each species
+        Returns:
+            None
+        """
+        for key, uid in datasource_uuids.items():
+            md = metadata[key]
+            site = md["site"]
+            network = md["network"]
+            inlet = md["inlet"]
+            species = md["species"]
+            sampling_period = md["sampling_period"]
+
+            # TODO - remove this check when improved input sanitisation is in place
+            if not any((site, network, inlet, species, sampling_period)):
+                raise ValueError(
+                    "Please ensure site, network, inlet, species and sampling_period are not None"
+                )
+
+            result = self.lookup_uuid(
+                site=site,
+                network=network,
+                inlet=inlet,
+                species=species,
+                sampling_period=sampling_period,
+            )
+
+            if result and result != uid:
+                raise ValueError("Mismatch between assigned uuid and stored Datasource uuid.")
+
+            self.set_uuid(
+                site=site,
+                network=network,
+                inlet=inlet,
+                species=species,
+                sampling_period=sampling_period,
+                uuid=uid,
+            )
+            self._datasource_uuids[uid] = key
+
+    def lookup_uuid(
+        self, site: str, network: str, inlet: str, species: str, sampling_period: int
+    ) -> Union[str, bool]:
+        """Perform a lookup for the UUID of a Datasource
+
+        Args:
+            site: Site code
+            network: Network name
+            inlet: Inlet height
+            species: Species name
+            sampling_period: Sampling period in seconds
+        Returns:
+            str or bool: UUID if exists else None
+        """
+        uuid = self._datasource_table[site][network][species][inlet][sampling_period]
+
+        return uuid if uuid else False
+
+    def set_uuid(
+        self,
+        site: str,
+        network: str,
+        inlet: str,
+        species: str,
+        sampling_period: int,
+        uuid: str,
+    ) -> None:
+        """Record a UUID of a Datasource in the datasource table
+
+        Args:
+            site: Site code
+            network: Network name
+            inlet: Inlet height
+            species: Species name
+            sampling_period: Sampling period in seconds
+            uuid: UUID of Datasource
+        Returns:
+            None
+        """
+        self._datasource_table[site][network][species][inlet][sampling_period] = uuid
+
+    def delete(self, uuid: str) -> None:
+        """Delete a Datasource with the given UUID
+
+        This function deletes both the record of the object store in he
+
+        Args:
+            uuid (str): UUID of Datasource
+        Returns:
+            None
+        """
+        from openghg.objectstore import delete_object, get_bucket
+        from openghg.store.base import Datasource
+
+        bucket = get_bucket()
+        # Load the Datasource and get all its keys
+        # iterate over these keys and delete them
+        datasource = Datasource.load(uuid=uuid)
+
+        data_keys = datasource.raw_keys()
+
+        for version in data_keys:
+            key_data = data_keys[version]["keys"]
+
+            for daterange in key_data:
+                key = key_data[daterange]
+                delete_object(bucket=bucket, key=key)
+
+        # Then delete the Datasource itself
+        key = f"{Datasource._datasource_root}/uuid/{uuid}"
+        delete_object(bucket=bucket, key=key)
 
-    return species_data
+        del self._datasource_uuids[uuid]
+
+    def seen_hash(self, file_hash: str) -> bool:
+        return file_hash in self._file_hashes
+
+    def set_hash(self, file_hash: str, filename: str) -> None:
+        self._file_hashes[file_hash] = filename
```

### Comparing `openghg-0.6.0/openghg/standardise/surface/_noaa.py` & `openghg-1.0.0/openghg/analyse/_footprint.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,685 +1,772 @@
-from pathlib import Path
-from typing import Any, Dict, Hashable, Optional, Union, cast
-import logging
-import xarray as xr
+"""
+This hopes to recreate the functionality of the ACRG repo function
+footprints_data_merge
+"""
+from pandas import Timestamp
+from xarray import Dataset, DataArray
+from typing import Optional, Tuple, Union, Dict, Any
+from openghg.dataobjects import FootprintData
 
-from openghg.types import optionalPathType
+# from openghg.dataobjects import FluxData
 
-logger = logging.getLogger("openghg.standardise.surface")
-logger.setLevel(logging.DEBUG)  # Have to set level for logger as well as handler
 
+__all__ = ["single_site_footprint", "footprints_data_merge"]
 
-def parse_noaa(
-    data_filepath: Union[str, Path],
+
+def single_site_footprint(
     site: str,
-    measurement_type: str,
-    inlet: Optional[str] = None,
-    network: str = "NOAA",
+    height: str,
+    network: str,
+    domain: str,
+    species: str,
+    start_date: Union[str, Timestamp],
+    end_date: Union[str, Timestamp],
+    resample_to: str = "coarsest",
+    site_modifier: Optional[str] = None,
+    platform: Optional[str] = None,
     instrument: Optional[str] = None,
-    sampling_period: Optional[str] = None,
-    update_mismatch: str = "never",
-    site_filepath: optionalPathType = None,
-    **kwarg: Dict,
-) -> Dict:
-    """Read NOAA data from raw text file or ObsPack NetCDF
+) -> Dataset:
+    """Creates a Dataset for a single site's measurement data and footprints
 
     Args:
-        data_filepath: Data filepath
-        site: Three letter site code
-        inlet: Inlet height (as value unit e.g. "10m")
-        measurement_type: One of ("flask", "insitu", "pfp")
-        network: Network, defaults to NOAA
-        instrument: Instrument name
-        sampling_period: Sampling period
-        update_mismatch: This determines how mismatches between the internal data
-            attributes and the supplied / derived metadata are handled.
-            This includes the options:
-                - "never" - don't update mismatches and raise an AttrMismatchError
-                - "attributes" - update mismatches based on input attributes
-                - "metadata" - update mismatches based on input metadata
-        site_filepath: Alternative site info file (see openghg/supplementary_data repository for format).
-            Otherwise will use the data stored within openghg_defs/data/site_info JSON file by default.
+        site: Site name
+        height: Height of inlet in metres
+        network: Network name
+        resample_to: Resample the data to a given time dataset.
+        Valid options are ["obs", "footprints", "coarsen"].
+            - "obs" resamples the footprints to the observation time series data
+            - "footprints" resamples to to the footprints time series
+            - "coarsest" resamples to the data with the coarsest time resolution
+        site_modifier: The name of the site given in the footprints.
+                       This is useful for example if the same site footprints are run with a different met and
+                       they are named slightly differently from the obs file. E.g.
+                       site="DJI", site_modifier = "DJI-SAM" - station called DJI, footprints site called DJI-SAM
+        platform: Observation platform used to decide whether to resample
+        instrument:
+        species: Species type
     Returns:
-        dict: Dictionary of data and metadata
+        xarray.Dataset
     """
-    if sampling_period is None:
-        sampling_period = "NOT_SET"
-
-    sampling_period = str(sampling_period)
+    from openghg.retrieve import get_obs_surface, get_footprint
+    from openghg.util import timestamp_tzaware
 
-    file_extension = Path(data_filepath).suffix
+    start_date = timestamp_tzaware(start_date)
+    end_date = timestamp_tzaware(end_date)
 
-    if file_extension == ".nc":
-        return _read_obspack(
-            data_filepath=data_filepath,
-            site=site,
-            inlet=inlet,
-            measurement_type=measurement_type,
-            instrument=instrument,
-            sampling_period=sampling_period,
-            update_mismatch=update_mismatch,
-            site_filepath=site_filepath,
-        )
-    else:
-        return _read_raw_file(
-            data_filepath=data_filepath,
-            site=site,
-            inlet=inlet,
-            measurement_type=measurement_type,
-            instrument=instrument,
-            sampling_period=sampling_period,
-            update_mismatch=update_mismatch,
-            site_filepath=site_filepath,
+    resample_to = resample_to.lower()
+    resample_choices = ("obs", "footprints", "coarsest")
+    if resample_to not in resample_choices:
+        raise ValueError(
+            f"Invalid resample choice {resample_to} past, please select from one of {resample_choices}"
         )
 
+    # As we're not retrieve any satellite data yet just set tolerance to None
+    tolerance = None
+    platform = None
 
-def _standarise_variables(obspack_ds: xr.Dataset, species: str) -> xr.Dataset:
-    """
-    Converts data from NOAA ObsPack dataset into our standardised variables to be stored within the object store.
-    The species is also needed so this name can be used to label the variables in the new dataset.
-
-    Expects inputs with: "value", "value_std_dev" or "value_unc", "nvalue" as per NOAA ObsPack standard.
+    # Here we want to use get_obs_surface
+    obs_results = get_obs_surface(
+        site=site,
+        inlet=height,
+        start_date=start_date,
+        end_date=end_date,
+        species=species,
+        instrument=instrument,
+    )
 
-    Args:
-        obspack_ds : Dataset derived from a netcdf file within the NOAA obspack
-        species : Standardised species name (e.g. "ch4")
+    obs_data = obs_results.data
 
-    Returns:
-        Dataset : Standardised dataset with variables extracted and renamed
+    # Save the observation data units
+    try:
+        units: Union[float, None] = float(obs_data.mf.attrs["units"])
+    except KeyError:
+        units = None
+    except AttributeError:
+        raise AttributeError("Unable to read mf attribute from observation data.")
+
+    # If the site for the footprints has a different name, pass that in
+    if site_modifier:
+        footprint_site = site_modifier
+    else:
+        footprint_site = site
 
-    Example output:
-        For species = "ch4":
-            xarray.Dataset("ch4":[...]
-                           "ch4_variability":[...]
-                           "ch4_number_of_observations": [...])
-    """
-
-    processed_ds = obspack_ds.copy()
-
-    # Rename variables to match our internal standard
-    # "value_std_dev" --> f"{species}_variability"
-    # "value_unc" --> ??
-    # TODO: Clarify what "value_unc" should be renamed to
-
-    variable_names = {
-        "value": species,
-        "value_std_dev": f"{species}_variability",
-        "value_unc": f"{species}_variability",  # May need to be updated
-        "nvalue": f"{species}_number_of_observations",
-    }
+    # Try to find appropriate footprints file first with and then without species name
+    try:
+        footprint = get_footprint(
+            site=footprint_site,
+            domain=domain,
+            height=height,
+            start_date=start_date,
+            end_date=end_date,
+            species=species,
+        )
+    except ValueError:
+        footprint = get_footprint(
+            site=footprint_site,
+            domain=domain,
+            height=height,
+            start_date=start_date,
+            end_date=end_date,
+        )
 
-    to_extract = [name for name in variable_names.keys() if name in obspack_ds]
+    # TODO: Add checks for particular species e.g. co2 and short-lived species
+    # which should have a specific footprints available rather than the generic one
 
-    # For the error variables we only want to take one set of values from the
-    # obspack dataset but multiple variables may be available.
-    # If multiple are present, combine these together and only extract one
-    error_names = ["value_std_dev", "value_unc"]
-    error_variables = [name for name in error_names if name in to_extract]
-
-    if len(error_variables) > 1:
-        main_ev = error_variables[0]  # Treat first item in the list at the one to keep
-
-        history_attr = "history"
-        processed_ds[main_ev].attrs[history_attr] = f"Merged {main_ev} variable from original file with "
-
-        for ev in error_variables[1:]:
-            # Combine details from additional additional error variable with main variable
-            variable = processed_ds[main_ev]
-            new_variable = processed_ds[ev]
-
-            # Update Dataset and add details within attributes
-            updated_variable = variable.combine_first(new_variable)
-            processed_ds[main_ev] = updated_variable
-            processed_ds[main_ev].attrs[history_attr] += f"{ev}, "
+    # Extract dataset
+    footprint_data = footprint.data
 
-            # Remove this extra variables from the list of variables to extract from the dataset
-            to_extract.remove(ev)
+    # Align the two Datasets
+    aligned_obs, aligned_footprint = align_datasets(
+        obs_data=obs_data,
+        footprint_data=footprint_data,
+        platform=platform,
+        resample_to=resample_to,
+    )
 
-    # Create dictionary of names to convert obspack ds to our format
-    name_dict = {name: key for name, key in variable_names.items() if name in to_extract}
+    combined_dataset = combine_datasets(
+        dataset_A=aligned_obs, dataset_B=aligned_footprint, tolerance=tolerance
+    )
 
-    if not to_extract:
-        wanted = variable_names.keys()
-        raise ValueError(
-            f"No valid data variables columns found in obspack dataset. We expect the following data variables in the passed NetCDF: {wanted}"
-        )
+    # Transpose to keep time in the last dimension position in case it has been moved in resample
+    combined_dataset = combined_dataset.transpose(..., "time")
 
-    # Grab only the variables we want to keep and rename these
-    processed_ds = processed_ds[to_extract]
-    processed_ds = processed_ds.rename(name_dict)
-    processed_ds = processed_ds.sortby("time")
+    if units is not None:
+        combined_dataset["fp"].values = combined_dataset["fp"].values / units
+        # if HiTRes:
+        #     combined_dataset.update({"fp_HiTRes": (combined_dataset.fp_HiTRes.dims, (combined_dataset.fp_HiTRes / units))})
 
-    return processed_ds
+    return combined_dataset
 
 
-def _split_inlets(
-    obspack_ds: xr.Dataset, attributes: Dict, metadata: Dict, inlet: Optional[str] = None
-) -> Dict:
+def footprints_data_merge(
+    site: str,
+    height: str,
+    network: str,
+    domain: str,
+    species: str,
+    start_date: Union[str, Timestamp],
+    end_date: Union[str, Timestamp],
+    resample_to: str = "coarsest",
+    site_modifier: Optional[str] = None,
+    platform: Optional[str] = None,
+    instrument: Optional[str] = None,
+    load_flux: Optional[bool] = True,
+    flux_source: Optional[str] = None,
+    load_bc: Optional[bool] = True,
+    calc_timeseries: Optional[bool] = True,
+    calc_bc: Optional[bool] = True,
+    time_resolution: Optional[str] = "standard",
+) -> FootprintData:
     """
-    Splits the overall dataset by different inlet values, if present. The expected dataset input should be from the NOAA ObsPack.
+    TODO - Should this be renamed?
 
     Args:
-        obspack_ds : Dataset derived from a netcdf file within the NOAA obspack
-        attributes: Attributes extracted from the NOAA obspack. Should contain at least "species" and "measurement_type"
-        metadata: Metadata to store alongside standardised data
-
+        site: Three letter site code
+        height: Height of inlet in metres
+        network: Network name
+        domain: Domain name
+        start_date: Start date
+        end_date: End date
+        resample_to: Overrides resampling to coarsest time resolution, can be one of ["coarsest", "footprints", "obs"]
+        site_modifier: The name of the site given in the footprints.
+                This is useful for example if the same site footprints are run with a different met and
+                they are named slightly differently from the obs file. E.g.
+                site="DJI", site_modifier = "DJI-SAM" - station called DJI, footprints site called DJI-SAM
+        platform: Observation platform used to decide whether to resample
+        instrument: Instrument name
+        species: Species name
+        load_flux: Load flux
+        flux_source: Flux source name
+        load_bc: Load boundary conditions (not currently implemented)
+        calc_timeseries: Calculate timeseries data (not currently implemented)
+        calc_bc: Calculate boundary conditions (not currently implemented)
+        time_resolution: One of ["standard", "high"]
     Returns:
-        Dict: gas data containing "data", "metadata", "attributes" for each inlet
-
-    Example output:
-        {"ch4": {"data": xr.Dataset(...), "attributes": {...}, "metadata": {...}}}
-        or
-        {"ch4_40m": {"data": xr.Dataset(...), "attributes": {...}, "metadata": {...}}, "ch4_60m": {...}, ...}
-
+        dict: Dictionary footprints data objects
     """
-    from openghg.util import format_inlet
-
-    orig_attrs = obspack_ds.attrs
-    species = attributes["species"]
-    measurement_type = attributes["measurement_type"]
+    from openghg.retrieve import get_flux
+    from pandas import Timedelta
 
-    height_var = "intake_height"
-
-    # Check whether the input data contains different inlet height values for each data point ("intake_height" data variable)
-    # If so we need to select the data for each inlet and indicate this is a separate Datasource
-    # Each data key is labelled based on the species and the inlet (if needed)
-
-    gas_data: Dict[str, Dict] = {}
-    if height_var in obspack_ds.data_vars:
-        if inlet is not None:
-            # TODO: Add to logging?
-            logger.warning(
-                f"Ignoring inlet value of {inlet} since file has each data point has an associated height (contains 'intake_height' variable)"
-            )
+    # First get the site data
+    combined_dataset = single_site_footprint(
+        site=site,
+        height=height,
+        network=network,
+        domain=domain,
+        start_date=start_date,
+        end_date=end_date,
+        resample_to=resample_to,
+        site_modifier=site_modifier,
+        platform=platform,
+        instrument=instrument,
+        species=species,
+    )
 
-        # Group dataset by the height values
-        # Note: could use ds.groupby_bins(...) if necessary if there are lots of small height differences to group these
-        obspack_ds_grouped = obspack_ds.groupby(height_var)
-        num_groups = len(obspack_ds_grouped.groups)
-
-        # For each group standardise and store with id based on species and inlet height
-        for ht, obspack_ds_ht in obspack_ds_grouped:
-            # Creating id keys of the form "<species>_<inlet>" e.g. "ch4_40m" or "co_12.5m"
-            inlet_str = format_inlet(str(ht), key_name="inlet")
-            inlet_magl_str = format_inlet(str(ht), key_name="inlet_height_magl")
+    # So here we iterate over the emissions types and get the fluxes
+    flux_dict = {}
+    if load_flux:
+        if flux_source is None:
+            raise ValueError("If you want to load flux you must pass a flux source")
+
+        flux_dict["standard"] = get_flux(
+            species=species,
+            domain=domain,
+            source=flux_source,
+            time_resolution=time_resolution,
+            start_date=start_date,
+            end_date=end_date,
+        ).data
+
+        if time_resolution == "high":
+
+            # TODO: Check appropriate date range and file formats for other species
+            if species == "co2":
+                max_h_back = str(combined_dataset["H_back"][-1].values) + "H"
+                if isinstance(start_date, str):
+                    start_date = Timestamp(start_date)
 
-            if num_groups > 1:
-                id_key = f"{species}_{inlet_str}"
+                start_date_hr = start_date - Timedelta(max_h_back)
             else:
-                id_key = f"{species}"
+                start_date_hr = start_date
 
-            # Extract wanted variables and convert to standardised names
-            standarised_ds = _standarise_variables(obspack_ds_ht, species)
+            flux_dict["high_time_res"] = get_flux(
+                species=species,
+                domain=domain,
+                source=flux_source,
+                time_resolution=time_resolution,
+                start_date=start_date_hr,
+                end_date=end_date,
+            ).data
+
+    # Calculate model time series, if required
+    if calc_timeseries:
+        combined_dataset = add_timeseries(combined_dataset=combined_dataset, flux_dict=flux_dict)
+
+    return FootprintData(
+        data=combined_dataset,
+        metadata={},
+        flux=flux_dict,
+        bc={},
+        species=species,
+        scales="scale",
+        units="units",
+    )
 
-            gas_data[id_key] = {}
-            gas_data[id_key]["data"] = standarised_ds
 
-            # Add inlet details to attributes and metadata
-            attrs_copy = attributes.copy()
-            meta_copy = metadata.copy()
+def combine_datasets(
+    dataset_A: Dataset,
+    dataset_B: Dataset,
+    method: str = "ffill",
+    tolerance: Optional[float] = None,
+) -> Dataset:
+    """Merges two datasets and re-indexes to the first dataset.
 
-            attrs_copy["inlet"] = inlet_str
-            attrs_copy["inlet_height_magl"] = inlet_magl_str
-            meta_copy["inlet"] = inlet_str
-            meta_copy["inlet_height_magl"] = inlet_magl_str
+        If "fp" variable is found within the combined dataset,
+        the "time" values where the "lat", "lon" dimensions didn't match are removed.
 
-            gas_data[id_key]["metadata"] = meta_copy
-            gas_data[id_key]["attributes"] = attrs_copy
+    Args:
+        dataset_A: First dataset to merge
+        dataset_B: Second dataset to merge
+        method: One of None, nearest, ffill, bfill.
+                See xarray.DataArray.reindex_like for list of options and meaning.
+                Defaults to ffill (forward fill)
+        tolerance: Maximum allowed tolerance between matches.
+    Returns:
+        xarray.Dataset: Combined dataset indexed to dataset_A
+    """
+    import numpy as np
 
+    if indexes_match(dataset_A, dataset_B):
+        dataset_B_temp = dataset_B
     else:
-        try:
-            inlet_value = orig_attrs["dataset_intake_ht"]
-        except KeyError:
-            inlet_from_file = None
-        else:
-            inlet_from_file = format_inlet(str(inlet_value))
-
-        if measurement_type == "flask":
-            inlet_from_file = "flask"
+        dataset_B_temp = dataset_B.reindex_like(other=dataset_A, method=method, tolerance=tolerance)  # type: ignore
 
-        # Check inlet from file against any provided inlet
-        if inlet is None and inlet_from_file:
-            inlet = inlet_from_file
-        elif inlet is not None and inlet_from_file:
-            if inlet != inlet_from_file:
-                logger.warning(
-                    f"Provided inlet {inlet} does not match inlet derived from the input file: {inlet_from_file}"
-                )
-        else:
-            raise ValueError(
-                "Unable to derive inlet from NOAA file. Please pass as an input. If flask data pass 'flask' as inlet."
-            )
+    merged_ds = dataset_A.merge(other=dataset_B_temp)
 
-        id_key = f"{species}"
-
-        if inlet != "flask":
-            inlet_magl_str = format_inlet(inlet, key_name="inlet_height_magl")
-        else:
-            inlet_magl_str = "NA"
+    if "fp" in merged_ds:
+        if all(k in merged_ds.fp.dims for k in ("lat", "long")):
+            flag = np.where(np.isfinite(merged_ds.fp.mean(dim=["lat", "lon"]).values))
+            merged_ds = merged_ds[dict(time=flag[0])]
 
-        metadata["inlet"] = inlet
-        metadata["inlet_height_magl"] = inlet_magl_str
-        attributes["inlet"] = inlet
-        attributes["inlet_height_magl"] = inlet_magl_str
+    return merged_ds
 
-        standardised_ds = _standarise_variables(obspack_ds, species)
 
-        gas_data[id_key] = {"data": standardised_ds, "metadata": metadata, "attributes": attributes}
-
-    return gas_data
-
-
-def _read_obspack(
-    data_filepath: Union[str, Path],
-    site: str,
-    sampling_period: str,
-    measurement_type: str,
-    inlet: Optional[str] = None,
-    instrument: Optional[str] = None,
-    update_mismatch: str = "never",
-    site_filepath: optionalPathType = None,
-) -> Dict[str, Dict]:
-    """Read NOAA ObsPack NetCDF files
+def indexes_match(dataset_A: Dataset, dataset_B: Dataset) -> bool:
+    """Check if two datasets need to be reindexed_like for combine_datasets
 
     Args:
-        data_filepath: Path to file
-        site: Three letter site code
-        sampling_period: Sampling period
-        measurement_type: One of flask, insitu or pfp
-        inlet: Inlet height, if no height use measurement type e.g. flask
-        instrument: Instrument name
-        update_mismatch: This determines how mismatches between the internal data
-            "attributes" and the supplied / derived "metadata" are handled.
-            This includes the options:
-              - "never" - don't update mismatches and raise an AttrMismatchError
-              - "from_source" / "attributes" - update mismatches based on input data (e.g. data attributes)
-              - "from_definition" / "metadata" - update mismatches based on associated data (e.g. site_info.json)
-        site_filepath: Alternative site info file (see openghg/supplementary_data repository for format).
-            Otherwise will use the data stored within openghg_defs/data/site_info JSON file by default.
+        dataset_A: First dataset to check
+        dataset_B: Second dataset to check
     Returns:
-        dict: Dictionary of results
+        bool: True if indexes match, else False
     """
-    from openghg.standardise.meta import assign_attributes
-    from openghg.util import clean_string
+    import numpy as np
 
-    valid_types = ("flask", "insitu", "pfp")
+    common_indices = (key for key in dataset_A.indexes.keys() if key in dataset_B.indexes.keys())
 
-    if measurement_type not in valid_types:
-        raise ValueError(f"measurement_type must be one of {valid_types}")
-
-    with xr.open_dataset(data_filepath) as temp:
-        obspack_ds = temp
-        orig_attrs = temp.attrs
+    for index in common_indices:
+        if not len(dataset_A.indexes[index]) == len(dataset_B.indexes[index]):
+            return False
+
+        # Check number of values that are not close (testing for equality with floating point)
+        if index == "time":
+            # For time override the default to have ~ second precision
+            rtol = 1e-10
+        else:
+            rtol = 1e-5
 
-    # Want to find and drop any duplicate time values for the original dataset
-    # Using xarray directly we have to do in a slightly convoluted way as this is not well built
-    # into the xarray workflow yet - https://github.com/pydata/xarray/pull/5239
-    # - can use da.drop_duplicates() but only on one variable at a time and not on the whole Dataset
-    # This method keeps attributes for each of the variables including units
+        index_diff = np.sum(
+            ~np.isclose(
+                dataset_A.indexes[index].values.astype(float),
+                dataset_B.indexes[index].values.astype(float),
+                rtol=rtol,
+            )
+        )
 
-    # The dimension within the original dataset is called "obs" and has no associated coordinates
-    # Extract time from original Dataset (dimension is "obs")
-    time = obspack_ds.time
+        if not index_diff == 0:
+            return False
 
-    # To keep associated "obs" dimension, need to assign coordinate values to this (just 0, len(obs))
-    time = time.assign_coords(obs=obspack_ds.obs)
+    return True
 
-    # Make "time" the primary dimension (while retaining "obs") and add "time" values as coordinates
-    time = time.swap_dims(dims_dict={"obs": "time"})
-    time = time.assign_coords(time=time)
 
-    # Drop any duplicate time values and extract the associated "obs" values
-    # TODO: Work out what to do with duplicates - may be genuine multiple measurements
-    time_unique = time.drop_duplicates(dim="time", keep="first")
-    obs_unique = time_unique.obs
+def align_datasets(
+    obs_data: Dataset,
+    footprint_data: Dataset,
+    resample_to: Optional[str] = "coarsest",
+    platform: Optional[str] = None,
+) -> Tuple[Dataset, Dataset]:
+    """Slice and resample two datasets to align along time
+
+    This slices the date to the smallest time frame
+    spanned by both the footprints and obs, then resamples the data
+    using the mean to the one with coarsest median resolution
+    starting from the sliced start date.
 
-    # Use these obs values to filter the original dataset to remove any repeated times
-    processed_ds = obspack_ds.sel(obs=obs_unique)
-    processed_ds = processed_ds.set_coords(["time"])
+    Args:
+        obs_data: Observations Dataset
+        footprint_data: Footprint Dataset
+        resample_to: Overrides resampling to coarsest time resolution, can be one of ["coarsest", "footprints", "obs"]
+        platform: Observation platform used to decide whether to resample
+    Returns:
+        tuple: Two xarray.Dataset with aligned time dimensions
+    """
+    import numpy as np
+    from pandas import Timedelta
 
-    # Estimate sampling period using metadata and midpoint time
-    if sampling_period == "NOT_SET":
-        sampling_period_estimate = _estimate_sampling_period(obspack_ds)
+    if platform is not None:
+        platform = platform.lower()
+        # Do not apply resampling for "satellite" (but have re-included "flask" for now)
+        if platform == "satellite":
+            return obs_data, footprint_data
+
+    # Whether sampling period is present or we need to try to infer this
+    infer_sampling_period = False
+    # Get the period of measurements in time
+    obs_attributes = obs_data.attrs
+    if "averaged_period" in obs_attributes:
+        obs_data_period_s = float(obs_attributes["averaged_period"])
+    elif "sampling_period" in obs_attributes:
+        sampling_period = obs_attributes["sampling_period"]
+        if sampling_period == "NOT_SET":
+            infer_sampling_period = True
+        else:
+            obs_data_period_s = float(sampling_period)
+        obs_data_period_s = float(obs_attributes["sampling_period"])
+    elif "sampling_period_estimate" in obs_attributes:
+        estimate = obs_attributes["sampling_period_estimate"]
+        print(f"WARNING: Using estimated sampling period of {estimate}s for observational data")
+        obs_data_period_s = float(estimate)
     else:
-        sampling_period_estimate = -1.0
+        infer_sampling_period = True
 
-    species = clean_string(obspack_ds.attrs["dataset_parameter"])
-    network = "NOAA"
-
-    try:
-        # Extract units attribute from value data variable
-        units = processed_ds["value"].units
-    except (KeyError, AttributeError):
-        logger.warning("Unable to extract units from 'value' within input dataset")
-        units = "NA"
-
-    metadata = {}
-    metadata["site"] = site
-    metadata["network"] = network
-    metadata["measurement_type"] = measurement_type
-    metadata["species"] = species
-    metadata["units"] = units
-    metadata["sampling_period"] = sampling_period
-    metadata["data_source"] = "noaa_obspack"
-    metadata["data_type"] = "surface"
-
-    # Add additional sampling_period_estimate if sampling_period is not set
-    if sampling_period_estimate >= 0.0:
-        metadata["sampling_period_estimate"] = str(
-            sampling_period_estimate
-        )  # convert to string to keep consistent with "sampling_period"
-
-    # Add instrument if present
-    if instrument is not None:
-        metadata["instrument"] = instrument
-    else:
-        metadata["instrument"] = orig_attrs.get("instrument", "NOT_SET")
+    if infer_sampling_period:
+        # Attempt to derive sampling period from frequency of data
+        obs_data_period_s = np.nanmedian((obs_data.time.data[1:] - obs_data.time.data[0:-1]) / 1e9).astype(
+            "float32"
+        )
 
-    # Add data owner details, station position and calibration scale, if present
-    metadata["data_owner"] = orig_attrs.get("provider_1_name", "NOT_SET")
-    metadata["data_owner_email"] = orig_attrs.get("provider_1_email", "NOT_SET")
-    metadata["station_longitude"] = orig_attrs.get("site_longitude", "NOT_SET")
-    metadata["station_latitude"] = orig_attrs.get("site_latitude", "NOT_SET")
-    metadata["calibration_scale"] = orig_attrs.get("dataset_calibration_scale", "NOT_SET")
-
-    # Create attributes with copy of metadata values
-    attributes = cast(Dict[Hashable, Any], metadata.copy())  # Cast to match xarray attributes type
-
-    # TODO: At the moment all attributes from the NOAA ObsPack are being copied
-    # plus any variables we're adding - decide if we want to reduce this
-    attributes.update(orig_attrs)
-
-    # expected_keys = {
-    #     "site",
-    #     "species",
-    #     "inlet",
-    #     "instrument",
-    #     "sampling_period",
-    #     "calibration_scale",
-    #     "station_longitude",
-    #     "station_latitude",
-    # }
+        obs_data_period_s_min = np.diff(obs_data.time.data).min() / 1e9
+        obs_data_period_s_max = np.diff(obs_data.time.data).max() / 1e9
 
-    gas_data = _split_inlets(processed_ds, attributes, metadata, inlet=inlet)
+        # Check if the periods differ by more than 1 second
+        if np.isclose(obs_data_period_s_min, obs_data_period_s_max, 1):
+            raise ValueError("Sample period can be not be derived from observations")
+
+    obs_data_timeperiod = Timedelta(seconds=obs_data_period_s)
+
+    # Derive the footprints period from the frequency of the data
+    footprint_data_period_ns = np.nanmedian(
+        (footprint_data.time.data[1:] - footprint_data.time.data[0:-1]).astype("int64")
+    )
+    footprint_data_timeperiod = Timedelta(footprint_data_period_ns, unit="ns")
 
-    gas_data = assign_attributes(
-        data=gas_data,
-        site=site,
-        network=network,
-        update_mismatch=update_mismatch,
-        site_filepath=site_filepath,
+    # Here we want timezone naive Timestamps
+    # Add sampling period to end date to make sure resample includes these values when matching
+    obs_startdate = Timestamp(obs_data.time[0].values)
+    obs_enddate = Timestamp(obs_data.time[-1].values) + Timedelta(obs_data_timeperiod, unit="seconds")
+    footprint_startdate = Timestamp(footprint_data.time[0].values)
+    footprint_enddate = Timestamp(footprint_data.time[-1].values) + Timedelta(
+        footprint_data_timeperiod, unit="nanoseconds"
     )
 
-    return gas_data
+    start_date = max(obs_startdate, footprint_startdate)
+    end_date = min(obs_enddate, footprint_enddate)
 
+    # Subtract half a second to ensure lower range covered
+    start_slice = start_date - Timedelta("0.5s")
+    # Add half a second to ensure upper range covered
+    end_slice = end_date + Timedelta("0.5s")
 
-def _read_raw_file(
-    data_filepath: Union[str, Path],
-    site: str,
-    sampling_period: str,
-    measurement_type: str,
-    inlet: Optional[str] = None,
-    instrument: Optional[str] = None,
-    update_mismatch: str = "never",
-    site_filepath: optionalPathType = None,
-) -> Dict:
-    """Reads NOAA data files and returns a dictionary of processed
-    data and metadata.
+    obs_data = obs_data.sel(time=slice(start_slice, end_slice))
+    footprint_data = footprint_data.sel(time=slice(start_slice, end_slice))
 
-    Args:
-        data_filepath: Path of file to load
-        site: Site name
-        sampling_period: Sampling period
-        measurement_type: One of flask, insitu or pfp
-        inlet: Inlet height, if no height use measurement type e.g. flask
-        instrument: Instrument name
-        update_mismatch: This determines how mismatches between the internal data
-            "attributes" and the supplied / derived "metadata" are handled.
-            This includes the options:
-              - "never" - don't update mismatches and raise an AttrMismatchError
-              - "from_source" / "attributes" - update mismatches based on input data (e.g. data attributes)
-              - "from_definition" / "metadata" - update mismatches based on associated data (e.g. site_info.json)
-        site_filepath: Alternative site info file (see openghg/supplementary_data repository for format).
-            Otherwise will use the data stored within openghg_defs/data/site_info JSON file by default.
+    # Only non satellite datasets with different periods need to be resampled
+    timeperiod_diff_s = np.abs(obs_data_timeperiod - footprint_data_timeperiod).total_seconds()
+    tolerance = 1e-9  # seconds
 
-    Returns:
-        list: UUIDs of Datasources data has been assigned to
-    """
-    from openghg.standardise.meta import assign_attributes
+    if timeperiod_diff_s >= tolerance:
+        base = start_date.hour + start_date.minute / 60.0 + start_date.second / 3600.0
 
-    # TODO: Added this for now to make sure inlet is specified but may be able to remove
-    # if this can be derived from the data format.
-    if inlet is None:
-        raise ValueError("Inlet must be specified to derive data from NOAA raw (txt) files.")
+        if resample_to == "coarsest":
+            if obs_data_timeperiod >= footprint_data_timeperiod:
+                resample_to = "obs"
+            elif obs_data_timeperiod < footprint_data_timeperiod:
+                resample_to = "footprints"
 
-    data_filepath = Path(data_filepath)
-    filename = data_filepath.name
+        if resample_to == "obs":
 
-    species = filename.split("_")[0].lower()
+            resample_period = str(round(obs_data_timeperiod / np.timedelta64(1, "h"), 5)) + "H"
 
-    source_name = data_filepath.stem
-    source_name = source_name.split("-")[0]
+            footprint_data = footprint_data.resample(indexer={"time": resample_period}, base=base).mean()
 
-    gas_data = _read_raw_data(
-        data_filepath=data_filepath,
-        inlet=inlet,
-        species=species,
-        measurement_type=measurement_type,
-        sampling_period=sampling_period,
-    )
+        elif resample_to == "footprints":
 
-    gas_data = assign_attributes(
-        data=gas_data, site=site, network="NOAA", update_mismatch=update_mismatch, site_filepath=site_filepath
-    )
+            resample_period = str(round(footprint_data_timeperiod / np.timedelta64(1, "h"), 5)) + "H"
 
-    return gas_data
+            obs_data = obs_data.resample(indexer={"time": resample_period}, base=base).mean()
 
+    return obs_data, footprint_data
 
-def _read_raw_data(
-    data_filepath: Path,
-    species: str,
-    inlet: str,
-    sampling_period: str,
-    measurement_type: str = "flask",
-) -> Dict:
-    """Separates the gases stored in the dataframe in
-    separate dataframes and returns a dictionary of gases
-    with an assigned UUID as gas:UUID and a list of the processed
-    dataframes
 
-    Args:
-        data_filepath: Path of datafile
-        species: Species string such as CH4, CO
-        measurement_type: Type of measurements e.g. flask
-    Returns:
-        dict: Dictionary containing attributes, data and metadata keys
+def add_timeseries(combined_dataset: Dataset, flux_dict: Dict[str, Dataset]) -> Dataset:
     """
-    from openghg.util import clean_string, read_header, get_site_info, load_internal_json
-    from pandas import Timestamp, read_csv
-
-    header = read_header(filepath=data_filepath)
-
-    column_names = header[-1][14:].split()
+    Add timeseries mole fraction values in footprint_data_merge
 
-    def date_parser(year: str, month: str, day: str, hour: str, minute: str, second: str) -> Timestamp:
-        return Timestamp(year, month, day, hour, minute, second)
-
-    date_parsing = {
-        "time": [
-            "sample_year",
-            "sample_month",
-            "sample_day",
-            "sample_hour",
-            "sample_minute",
-            "sample_seconds",
-        ]
-    }
-
-    data_types = {
-        "sample_year": int,
-        "sample_month": int,
-        "sample_day": int,
-        "sample_hour": int,
-        "sample_minute": int,
-        "sample_seconds": int,
-    }
+    Args:
+        combined_dataset [Dataset]:
+            output created during footprint_data_merge
+        flux_dict [dict]:
+            Dictionary containing flux datasets
+    """
+    # TODO: Extend to include multiple sources
+    # TODO: Improve ability to merge high time resolution footprints (e.g. species as co2)
+    # What do we expect flux_dict to look like?
+    for key, flux_ds in flux_dict.items():
+        if key == "high_time_res":
+            mf_mod: DataArray = timeseries_HiTRes(combined_dataset, flux_ds)
+            name = "mf_mod_high_res"
+            # TODO: May want to reindex afterwards? But can be expensive operation.
+        else:
+            # flux_reindex = flux_ds.reindex_like(combined_dataset, 'ffill')
+            # combined_dataset['mf_mod'] = DataArray((combined_dataset.fp * flux_reindex.flux).sum(["lat", "lon"]), coords={'time': combined_dataset.time})
+            mf_mod = timeseries_integrated(combined_dataset, flux_ds)
+            name = "mf_mod"
 
-    # Number of header lines to skip
-    n_skip = len(header)
+        combined_dataset[name] = DataArray(mf_mod, coords={"time": combined_dataset.time})
 
-    data = read_csv(
-        data_filepath,
-        skiprows=n_skip,
-        names=column_names,
-        sep=r"\s+",
-        dtype=data_types,
-        parse_dates=date_parsing,
-        date_parser=date_parser,
-        index_col="time",
-        skipinitialspace=True,
-    )
+    return combined_dataset
 
-    # Drop duplicates
-    data = data.loc[~data.index.duplicated(keep="first")]
 
-    # Check if the index is sorted
-    if not data.index.is_monotonic_increasing:
-        data = data.sort_index()
-
-    # Read the site code from the Dataframe
-    site = str(data["sample_site_code"][0]).upper()
-
-    site_data = get_site_info()
-    # If this isn't a site we recognize try and read it from the filename
-    if site not in site_data:
-        site = str(data_filepath.name).split("_")[1].upper()
-
-        if site not in site_data:
-            raise ValueError(f"The site {site} is not recognized.")
-
-    if species is not None:
-        # If we're passed a species ensure that it is in fact the correct species
-        data_species = str(data["parameter_formula"].values[0]).lower()
-
-        passed_species = species.lower()
-        if data_species != passed_species:
-            raise ValueError(
-                f"Mismatch between passed species ({passed_species}) and species read from data ({data_species})"
-            )
+def timeseries_integrated(combined_dataset: Dataset, flux_ds: Dataset) -> DataArray:
+    """
+    Calculate modelled mole fraction timeseries using integrated footprints data.
 
-    species = species.upper()
+    Args:
+        combined_dataset [Dataset]:
+            output created during footprint_data_merge
+        flux_ds [Dataset]:
+            Dataset containing flux values
 
-    flag = []
-    selection_flag = []
-    for flag_str in data.analysis_flag:
-        flag.append(flag_str[0] == ".")
-        selection_flag.append(int(flag_str[1] != "."))
-
-    combined_data = {}
-
-    data[species + "_status_flag"] = flag
-    data[species + "_selection_flag"] = selection_flag
-
-    data = data[data[species + "_status_flag"]]
-
-    data = data[
-        [
-            "sample_latitude",
-            "sample_longitude",
-            "sample_altitude",
-            "analysis_value",
-            "analysis_uncertainty",
-            species + "_selection_flag",
-        ]
-    ]
-
-    rename_dict = {
-        "analysis_value": species,
-        "analysis_uncertainty": species + "_repeatability",
-        "sample_longitude": "longitude",
-        "sample_latitude": "latitude",
-        "sample_altitude": "altitude",
-    }
+    Returns:
+        DataArray :
+            Modelled mole fraction timeseries, dimensions = (time)
 
-    data = data.rename(columns=rename_dict, inplace=False)
-    data = data.to_xarray()
+    TODO: Also allow flux_mod to be returned as an option? Include flags if so.
+    """
+    flux_reindex = flux_ds.reindex_like(combined_dataset, "ffill")
+    flux_mod: DataArray = combined_dataset.fp * flux_reindex.flux
+    timeseries: DataArray = flux_mod.sum(["lat", "lon"])
+    # combined_dataset['mf_mod'] = DataArray((combined_dataset.fp * flux_reindex.flux).sum(["lat", "lon"]), coords={'time': combined_dataset.time})
+
+    return timeseries
 
-    # TODO  - this could do with a better name
-    noaa_params = load_internal_json(filename="attributes.json")["NOAA"]
 
-    site_attributes = noaa_params["global_attributes"]
-    site_attributes["inlet_height_magl"] = "NA"
-    site_attributes["instrument"] = noaa_params["instrument"][species.upper()]
-    site_attributes["sampling_period"] = sampling_period
-
-    metadata = {}
-    metadata["species"] = clean_string(species)
-    metadata["site"] = site
-    metadata["measurement_type"] = measurement_type
-    metadata["network"] = "NOAA"
-    metadata["inlet"] = inlet
-    metadata["sampling_period"] = sampling_period
-    metadata["instrument"] = noaa_params["instrument"][species.upper()]
-    metadata["data_type"] = "surface"
-    metadata["source_format"] = "noaa"
-
-    combined_data[species.lower()] = {
-        "metadata": metadata,
-        "data": data,
-        "attributes": site_attributes,
-    }
+def timeseries_HiTRes(
+    combined_dataset: Dataset,
+    flux_ds: Dataset,
+    averaging: Optional[str] = None,
+    output_TS: Optional[bool] = True,
+    output_fpXflux: Optional[bool] = False,
+) -> Any:
+    """
+     Calculate modelled mole fraction timeseries using high time resolution
+     footprints data and emissions data.
 
-    return combined_data
+    Args:
+         combined_dataset:
+             output created during footprint_data_merge. Expect dataset containing
+             "fp_HiTRes" data variable with dimensions (lat, lon, time, H_back).
+             Where H_back represents the hourly footprints related to the footprints
+             time.
+         flux_ds:
+             Dataset containing flux values. Expect dataset containing "flux"
+             data variable with dimensions (lat, lon, time).
+         averaging:
+             Time resolution to use to average the time dimension.
+             Default = None
+         output_TS:
+             Whether to output the modelled mole fraction timeseries DataArray.
+             Default = True
+         output_fpXflux:
+             Whether to output the modelled flux map DataArray used to create
+             the timeseries.
+             Default = False
+     Returns:
+         DataArray / DataArray :
+             Modelled mole fraction timeseries, dimensions = (time)
+             Modelled flux map, dimensions = (lat, lon, time)
+
+         If one of output_TS and output_fpXflux are True:
+             DataArray is returned for the respective output
+
+         If both output_TS and output_fpXflux are both True:
+             Both DataArrays are returned.
+
+     TODO: Low frequency flux values may need to be selected from the month before
+     (currently selecting the same month).
+     TODO: Indexing for low frequency flux should be checked to make sure this
+     allows for crossing over the end of the year.
+     TODO: Currently using pure dask arrays (based on Hannah's original code)
+     but would be good to update this to add more pre-indexing using xarray
+     and/or use dask as part of datasets.
+     TODO: May want to update this to not rely on indexing when selecting
+     the appropriate flux values. At the moment this solution has been chosen
+     because selecting on a dimension, rather than indexing, can be *very* slow
+     depending on the operations performed beforehand on the Dataset (e.g.
+     resample and reindex)
+     TODO: This code currently resamples the frequency to be regular. This will
+     have no effect if the time frequency was already regular but this may
+     not be what we want and may want to add extra code to remove any NaNs, if
+     they are introduced or to find a way to remove this requirement.
+     TODO: mypy having trouble with different types options and incompatible types,
+     included as Any for now.
+    """
+    import numpy as np
+    import dask.array as da  # type: ignore
+    from tqdm import tqdm
+    from pandas import date_range
+    from math import gcd
+
+    fp_HiTRes = combined_dataset.fp_HiTRes
+
+    # Calculate time resolution for both the flux and footprints data
+    nanosecond_to_hour = 1 / (1e9 * 60.0 * 60.0)
+    flux_res_H = int(flux_ds.time.diff(dim="time").values.mean() * nanosecond_to_hour)
+    fp_res_time_H = int(fp_HiTRes.time.diff(dim="time").values.mean() * nanosecond_to_hour)
 
+    fp_res_Hback_H = int(fp_HiTRes["H_back"].diff(dim="H_back").values.mean())
 
-def _estimate_sampling_period(obspack_ds: xr.Dataset, min_estimate: float = 10.0) -> float:
-    """
-    Estimate the sampling period for the NOAA data using either the "data_selection_tag"
-    attribute (this sometimes contains useful information such as "HourlyData") or by using
-    the midpoint_time within the data itself.
+    # Define resolution on time dimension in number in hours
+    if averaging:
+        try:
+            time_res_H = int(averaging)
+            time_resolution = f"{time_res_H}H"
+        except (ValueError, TypeError):
+            time_res_H = int(averaging[0])
+            time_resolution = averaging
+    else:
+        # If not specified derive from time from combined dataset
+        time_res_H = fp_res_time_H
+        time_resolution = f"{time_res_H}H"
+
+    # Resample fp timeseries to match time resolution
+    if fp_res_time_H != time_res_H:
+        fp_HiTRes = fp_HiTRes.resample(time=time_resolution).ffill()
+
+    # Define resolution on high frequency dimension in number of hours
+    # At the moment this is matched to the Hback dimension
+    time_hf_res_H = fp_res_Hback_H
+
+    # Only allow for high frequency resolution < 24 hours
+    if time_hf_res_H > 24:
+        raise ValueError(f"High frequency resolution must be <= 24 hours. Current: {time_hf_res_H}H")
+    elif 24 % time_hf_res_H != 0 or 24 % time_hf_res_H != 0.0:
+        raise ValueError(
+            f"High frequency resolution must exactly divide into 24 hours. Current: {time_hf_res_H}H"
+        )
 
-    Note: midpoint_time often seems to match start_time implying instantaneous measurement
-    or that this value has not been correctly included.
+    # Find the greatest common denominator between time and high frequency resolutions.
+    # This is needed to make sure suitable flux frequency is used to allow for indexing.
+    # e.g. time: 1H; hf (high frequency): 2H, highest_res_H would be 1H
+    # e.g. time: 2H; hf (high frequency): 3H, highest_res_H would be 1H
+    highest_res_H = gcd(time_res_H, time_hf_res_H)
+    highest_resolution = f"{highest_res_H}H"
+
+    # create time array to loop through, with the required resolution
+    # fp_HiTRes.time is the release time of particles into the model
+    time_array = fp_HiTRes["time"]
+    lat = fp_HiTRes["lat"]
+    lon = fp_HiTRes["lon"]
+    hback = fp_HiTRes["H_back"]
+
+    ntime = len(time_array)
+    nlat = len(lat)
+    nlon = len(lon)
+    # nh_back = len(hback)
+
+    # Define maximum hour back
+    max_h_back = hback.values[-1]
+
+    # Define full range of dates to select from the flux input
+    date_start = time_array[0]
+    date_start_back = date_start - np.timedelta64(max_h_back, "h")
+    date_end = time_array[-1] + np.timedelta64(1, "s")
 
-    If the estimate is less than `min_estimate` the estimate sampling period will be set to
-    this value.
+    start = {
+        dd: getattr(np.datetime64(time_array[0].values, "h").astype(object), dd) for dd in ["month", "year"]
+    }
 
-    Args:
-        obspack_ds : Dataset of raw obs pack file opened as an xarray Dataset
-        min_estimate : Minimum sampling period estimate to use in seconds.
+    # Create times for matching to the flux
+    full_dates = date_range(
+        date_start_back.values, date_end.values, freq=highest_resolution, closed="left"
+    ).to_numpy()
+
+    # Create low frequency flux data (monthly)
+    flux_ds_low_freq = flux_ds.resample({"time": "1MS"}).mean().sel(time=slice(date_start_back, date_end))
+    flux_ds_low_freq = flux_ds_low_freq.transpose(*("lat", "lon", "time"))
+
+    # Select and align high frequency flux data
+    flux_ds_high_freq = flux_ds.sel(time=slice(date_start_back, date_end))
+    if flux_res_H <= 24:
+        base = (
+            date_start_back.dt.hour.data
+            + date_start_back.dt.minute.data / 60.0
+            + date_start_back.dt.second.data / 3600.0
+        )
+        if flux_res_H <= highest_res_H:
+            # Downsample flux to match to footprints frequency
+            flux_ds_high_freq = flux_ds_high_freq.resample({"time": highest_resolution}, base=base).mean()
+        elif flux_res_H > highest_res_H:
+            # Upsample flux to match footprints frequency and forward fill
+            flux_ds_high_freq = flux_ds_high_freq.resample({"time": highest_resolution}, base=base).ffill()
+        # Reindex to match to correct values
+        flux_ds_high_freq = flux_ds_high_freq.reindex({"time": full_dates}, method="ffill")
+    elif flux_res_H > 24:
+        # If flux is not high frequency use the monthly averages instead.
+        flux_ds_high_freq = flux_ds_low_freq
+
+    # TODO: Add check to make sure time values are exactly aligned based on date range
+
+    # Make sure the dimensions match the expected order for indexing
+    fp_HiTRes = fp_HiTRes.transpose(*("lat", "lon", "time", "H_back"))
+    flux_ds_high_freq = flux_ds_high_freq.transpose(*("lat", "lon", "time"))
+
+    # Extract footprints array to use in numba loop
+    fp_HiTRes = da.array(fp_HiTRes)
+
+    # Set up a numpy array to calculate the product of the footprints (H matrix) with the fluxes
+    if output_fpXflux:
+        fpXflux = da.zeros((nlat, nlon, ntime))
+
+    if output_TS:
+        timeseries = da.zeros(ntime)
+
+    # Iterate through the time coord to get the total mf at each time step using the H back coord
+    # at each release time we disaggregate the particles backwards over the previous 24hrs
+    # The final value then contains the 29-day integrated residual footprints
+    print("Calculating modelled timeseries comparison:")
+    iters = tqdm(time_array.values)
+    for tt, time in enumerate(iters):
+
+        # Get correct index for low resolution data based on start and current date
+        current = {dd: getattr(np.datetime64(time, "h").astype(object), dd) for dd in ["month", "year"]}
+        tt_low = current["month"] - start["month"] + 12 * (current["year"] - start["year"])
+
+        # get 4 dimensional chunk of high time res footprints for this timestep
+        # units : mol/mol/mol/m2/s
+        # reverse the time coordinate to be chronological
+        fp_time = fp_HiTRes[:, :, tt, ::-1]
+
+        fp_high_freq = fp_time[:, :, 1:]
+        fp_residual = fp_time[:, :, 0:1]  # First element (reversed) contains residual footprints
+
+        # Extract flux data from dataset
+        flux_high_freq = flux_ds_high_freq.flux
+        flux_low_freq = flux_ds_low_freq.flux
+
+        # Define high and low frequency fluxes based on inputs
+        # Allow for variable frequency within 24 hours
+        flux_low_freq = flux_low_freq[:, :, tt_low : tt_low + 1]
+        if flux_res_H <= 24:
+            # Define indices to correctly select matching date range from flux data
+            # This will depend on the various frequencies of the inputs
+            # At present, highest_res_H matches the flux frequency
+            tt_start = tt * int(time_res_H / highest_res_H) + 1
+            tt_end = tt_start + int(max_h_back / highest_res_H)
+            selection = int(time_hf_res_H / highest_res_H)
+
+            # Extract matching time range from whole flux array
+            flux_high_freq = flux_high_freq[..., tt_start:tt_end]
+            if selection > 1:
+                # If flux frequency does not match to the high frequency (hf, H_back)
+                # dimension, select entries which do. Reversed to make sure
+                # entries matching to the correct times are selected
+                flux_high_freq = flux_high_freq[..., ::-selection]
+                flux_high_freq = flux_high_freq[..., ::-1]
+        else:
+            flux_high_freq = flux_high_freq[:, :, tt_low : tt_low + 1]
 
-    Returns:
-        int: Seconds for the estimated sampling period.
-    """
-    # Check useful attributes
-    data_selection = obspack_ds.attrs["dataset_selection_tag"]
+        # convert to array to use in numba loop
+        flux_high_freq = da.array(flux_high_freq)
+        flux_low_freq = da.array(flux_low_freq)
+
+        # Multiply the HiTRes footprints with the HiTRes emissions to give mf
+        # Multiply residual footprints by low frequency emissions data to give residual mf
+        # flux units : mol/m2/s;       fp units : mol/mol/mol/m2/s
+        # --> mol/mol/mol/m2/s * mol/m2/s === mol / mol
+        fpXflux_time = flux_high_freq * fp_high_freq
+        fpXflux_residual = flux_low_freq * fp_residual
+
+        # append the residual emissions
+        fpXflux_time = np.dstack((fpXflux_time, fpXflux_residual))
+
+        if output_fpXflux:
+            # Sum over time (H back) to give the total mf at this timestep
+            fpXflux[:, :, tt] = fpXflux_time.sum(axis=2)
+
+        if output_TS:
+            # work out timeseries by summing over lat, lon (24 hrs)
+            timeseries[tt] = fpXflux_time.sum()
+
+    if output_fpXflux:
+        fpXflux = DataArray(
+            fpXflux,
+            dims=("lat", "lon", "time"),
+            coords={"lat": lat, "lon": lon, "time": time_array},
+        )
 
-    hourly_s = 60 * 60
-    daily_s = hourly_s * 24
-    weekly_s = daily_s * 7
-    monthly_s = weekly_s * 28  # approx
-    yearly_s = daily_s * 365  # approx
-
-    sampling_period_estimate = 0.0  # seconds
-
-    frequency_keywords = {
-        "hourly": hourly_s,
-        "daily": daily_s,
-        "weekly": weekly_s,
-        "monthly": monthly_s,
-        "yearly": yearly_s,
-    }
-    for freq, time_s in frequency_keywords.items():
-        if freq in data_selection.lower():
-            sampling_period_estimate = time_s
-
-    if not sampling_period_estimate:
-        if "start_time" in obspack_ds and "midpoint_time" in obspack_ds:
-            half_sample_time = (obspack_ds["midpoint_time"] - obspack_ds["start_time"]).values
-            half_sample_time_s = half_sample_time.astype("timedelta64[s]").mean().astype(float)
-            sampling_period_estimate = round(half_sample_time_s * 2, 1)
+    if output_TS:
+        timeseries = DataArray(timeseries, dims=("time"), coords={"time": time_array})
 
-    if sampling_period_estimate < min_estimate:
-        sampling_period_estimate = min_estimate
+    if output_fpXflux and output_TS:
+        timeseries.compute()
+        fpXflux.compute()
+        return timeseries, fpXflux
+    elif output_fpXflux:
+        fpXflux.compute()
+        return fpXflux
+    elif output_TS:
+        timeseries.compute()
+        return timeseries
 
-    return sampling_period_estimate
+    return None
```

### Comparing `openghg-0.6.0/openghg/standardise/surface/_npl.py` & `openghg-1.0.0/openghg/util/_export.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,131 +1,118 @@
-from datetime import datetime
+from addict import Dict as aDict
+from typing import Dict, List, Union
+from json import loads, dump
 from pathlib import Path
-from typing import Dict, Optional
+from openghg.dataobjects import ObsData
 
-from openghg.standardise.meta import assign_attributes
-from openghg.types import pathType
-from openghg.util import clean_string, load_internal_json
-from pandas import NaT, read_csv
-
-
-def parse_npl(
-    data_filepath: pathType,
-    site: str = "NPL",
-    network: str = "LGHG",
-    inlet: Optional[str] = None,
-    instrument: Optional[str] = None,
-    sampling_period: Optional[str] = None,
-    measurement_type: Optional[str] = None,
-    update_mismatch: str = "never",
-) -> Dict:
-    """Reads NPL data files and returns the UUIDS of the Datasources
-    the processed data has been assigned to
+
+__all__ = ["to_dashboard", "to_dashboard_mobile"]
+
+
+def to_dashboard(
+    data: Dict, selected_vars: List, downsample_n: int = 3, filename: str = None
+) -> Union[Dict, None]:
+    """Takes a Dataset produced by OpenGHG and outputs it into a JSON
+    format readable by the OpenGHG dashboard or a related project.
+
+    This also exports a separate file with the locations of the sites
+    for use with map selector component.
+
+    Note - this function does not currently support export of data from multiple
+    inlets.
 
     Args:
-        data_filepath: Path of file to load
-        site: Site name
-        network: Network, defaults to LGHG
-        inlet: Inlet height. Will be inferred if not specified
-        instrument: Instrument name
-        sampling_period: Sampling period
-        measurement_type: Type of measurement taken e.g."flask", "insitu"
-        update_mismatch: This determines how mismatches between the internal data
-            "attributes" and the supplied / derived "metadata" are handled.
-            This includes the options:
-              - "never" - don't update mismatches and raise an AttrMismatchError
-              - "from_source" / "attributes" - update mismatches based on input data (e.g. data attributes)
-              - "from_definition" / "metadata" - update mismatches based on associated data (e.g. site_info.json)
+        data: Dictionary of retrieved data
+        selected_vars: The variables to want to export
+        downsample_n: Take every nth value from the data
+        filename: filename to write output to
     Returns:
-        list: UUIDs of Datasources data has been assigned to
+        None
     """
-    from openghg.util import get_site_info, format_inlet, synonyms
+    to_export = aDict()
 
-    if sampling_period is None:
-        sampling_period = "NOT_SET"
+    if not isinstance(selected_vars, list):
+        selected_vars = [selected_vars]
 
-    data_filepath = Path(data_filepath)
+    selected_vars = [str(c).lower() for c in selected_vars]
 
-    site_upper = site.upper()
-    network_upper = network.upper()
-
-    attributes_data = load_internal_json(filename="attributes.json")
-    npl_params = attributes_data[site_upper]
-
-    site_data = get_site_info()
-    site_info = site_data[site_upper][network_upper]
-
-    # mypy doesn't like NaT or NaNs - look into this
-    def parser(date: str):  # type: ignore
-        try:
-            return datetime.strptime(str(date), "%d/%m/%Y %H:%M")
-        except ValueError:
-            return NaT
-
-    data = read_csv(data_filepath, index_col=0, date_parser=parser)
-
-    # Drop the NaT/NaNs
-    data = data.loc[data.index.dropna()]
-
-    # Rename columns
-    rename_dict = {"Cal_CO2_dry": "CO2", "Cal_CH4_dry": "CH4"}
-
-    data = data.rename(columns=rename_dict)
-    data.index.name = "time"
-
-    try:
-        site_inlet_values = site_info["height"]
-    except KeyError:
-        raise ValueError(
-            f"Unable to extract inlet height details for site '{site}'. Please input inlet value."
-        )
-
-    inlet = format_inlet(inlet)
-    if inlet is None:
-        inlet = site_inlet_values[0]  # Use first entry
-        inlet = format_inlet(inlet)
-    elif inlet not in site_inlet_values:
-        print(f"WARNING: inlet value of '{inlet}' does not match to known inlet values")
-
-    gas_data = {}
-    for species_column in data.columns:
-        processed_data = data.loc[:, [species_column]].sort_index().to_xarray()
-
-        # Convert methane to ppb
-        if species_column == "CH4":
-            processed_data[species_column] *= 1000
-
-        species = clean_string(species_column)
-        species = synonyms(species, allow_new_species=True)
-
-        # No averaging applied to raw obs, set variability to 0 to allow get_obs to calculate
-        # when averaging
-        processed_data["{} variability".format(species)] = processed_data[species_column] * 0.0
-
-        site_attributes = npl_params["global_attributes"]
-        site_attributes["inlet"] = inlet
-        site_attributes["inlet_height_magl"] = format_inlet(inlet, key_name="inlet_height_magl")
-        site_attributes["instrument"] = npl_params["instrument"]
-
-        attributes = site_attributes
-        attributes["species"] = species
-
-        metadata = {
-            "species": species,
-            "sampling_period": str(sampling_period),
-            "site": "NPL",
-            "network": "LGHG",
-            "inlet": inlet,
-            "data_type": "surface",
-            "source_format": "npl",
-        }
-
-        # TODO - add in better metadata reading
-        gas_data[species] = {
-            "metadata": metadata,
-            "data": processed_data,
-            "attributes": attributes,
-        }
+    for site, species_data in data.items():
+        for species, inlet_data in species_data.items():
+            measurement_data: ObsData
+            for inlet, measurement_data in inlet_data.items():
+                dataset = measurement_data.data
+                metadata = measurement_data.metadata
+                attributes = dataset.attrs
+
+                df = dataset.to_dataframe()
+
+                rename_lower = {c: str(c).lower() for c in df.columns}
+                df = df.rename(columns=rename_lower)
+                # We just want the selected variables
+                to_extract = [c for c in df.columns if c in selected_vars]
+
+                if not to_extract:
+                    continue
+
+                df = df[to_extract]
+
+                # Downsample the data
+                if downsample_n > 1:
+                    df = df.iloc[::downsample_n]
+
+                network = metadata["network"]
+                instrument = metadata["instrument"]
+
+                # TODO - remove this if we add site location to standard metadata
+                location = {
+                    "latitude": attributes["station_latitude"],
+                    "longitude": attributes["station_longitude"],
+                }
+                metadata.update(location)
+
+                json_data = loads(df.to_json())
+                metadata = measurement_data.metadata
+
+                to_export[species][network][site][inlet][instrument] = {
+                    "data": json_data,
+                    "metadata": metadata,
+                }
+
+    if filename is not None:
+        with open(filename, "w") as f:
+            dump(obj=to_export, fp=f)
+        return None
+    else:
+        # TODO - remove this once addict is stubbed
+        export_dict: Dict = to_export.to_dict()
+        return export_dict
 
-    gas_data = assign_attributes(data=gas_data, site=site, network=network, update_mismatch=update_mismatch)
 
-    return gas_data
+def to_dashboard_mobile(data: Dict, filename: Union[str, Path] = None) -> Union[Dict, None]:
+    """Export the Glasgow LICOR data to JSON for the dashboard
+
+    Args:
+        data: Data dictionary
+        filename: Filename for export of JSON
+    Returns:
+        dict or None: Dictonary if no filename given
+    """
+    to_export = aDict()
+
+    for species, species_data in data.items():
+        spec_data = species_data["data"]
+        metadata = species_data["metadata"]
+
+        latitude = spec_data["latitude"].values.tolist()
+        longitude = spec_data["longitude"].values.tolist()
+        ch4 = spec_data["ch4"].values.tolist()
+
+        to_export[species]["data"] = {"lat": latitude, "lon": longitude, "z": ch4}
+        to_export[species]["metadata"] = metadata
+
+    if filename is not None:
+        with open(filename, "w") as f:
+            dump(to_export, f)
+        return None
+    else:
+        to_return: Dict = to_export.to_dict()
+        return to_return
```

### Comparing `openghg-0.6.0/openghg/store/_emissions.py` & `openghg-1.0.0/openghg/store/_emissions.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,268 +1,273 @@
-from __future__ import annotations
-from pathlib import Path
-from tempfile import TemporaryDirectory
-from typing import Any, Dict, Literal, Optional, Tuple, Union
-import logging
-import numpy as np
-from numpy import ndarray
-from openghg.store import DataSchema
 from openghg.store.base import BaseStore
-from xarray import DataArray, Dataset
-from types import TracebackType
-import warnings
-
-ArrayType = Optional[Union[ndarray, DataArray]]
+from pathlib import Path
+from typing import DefaultDict, Dict, Optional, Union
+from xarray import Dataset
 
-logger = logging.getLogger("openghg.store")
-logger.setLevel(logging.DEBUG)  # Have to set level for logger as well as handler
+__all__ = ["Emissions"]
 
 
 class Emissions(BaseStore):
     """This class is used to process emissions / flux data"""
 
     _root = "Emissions"
     _uuid = "c5c88168-0498-40ac-9ad3-949e91a30872"
-    _metakey = f"{_root}/uuid/{_uuid}/metastore"
-
-    def __enter__(self) -> Emissions:
-        return self
-
-    def __exit__(
-        self,
-        exc_type: Optional[BaseException],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
-    ) -> None:
-        if exc_type is not None:
-            logger.error(msg=f"{exc_type}, {exc_tb}")
-        else:
-            self.save()
 
-    def read_data(self, binary_data: bytes, metadata: Dict, file_metadata: Dict) -> Optional[Dict]:
-        """Ready a footprint from binary data
+    def save(self) -> None:
+        """Save the object to the object store
 
-        Args:
-            binary_data: Footprint data
-            metadata: Dictionary of metadata
-            file_metadat: File metadata
         Returns:
-            dict: UUIDs of Datasources data has been assigned to
+            None
         """
-        with TemporaryDirectory() as tmpdir:
-            tmpdir_path = Path(tmpdir)
+        from openghg.objectstore import get_bucket, set_object_from_json
 
-            try:
-                filename = file_metadata["filename"]
-            except KeyError:
-                raise KeyError("We require a filename key for metadata read.")
-
-            filepath = tmpdir_path.joinpath(filename)
-            filepath.write_bytes(binary_data)
+        bucket = get_bucket()
+        obs_key = f"{Emissions._root}/uuid/{Emissions._uuid}"
 
-            return self.read_file(filepath=filepath, **metadata)
+        self._stored = True
+        set_object_from_json(bucket=bucket, key=obs_key, data=self.to_data())
 
+    @staticmethod
     def read_file(
-        self,
         filepath: Union[str, Path],
         species: str,
         source: str,
         domain: str,
-        database: Optional[str] = None,
-        database_version: Optional[str] = None,
-        model: Optional[str] = None,
-        source_format: str = "openghg",
+        date: str,
         high_time_resolution: Optional[bool] = False,
-        period: Optional[Union[str, tuple]] = None,
-        chunks: Union[int, Dict, Literal["auto"], None] = None,
-        continuous: bool = True,
+        period: Optional[str] = None,
         overwrite: bool = False,
-    ) -> Optional[Dict]:
+    ) -> Dict:
         """Read emissions file
 
         Args:
             filepath: Path of emissions file
             species: Species name
             domain: Emissions domain
             source: Emissions source
-            database: Name of database source for this input (if relevant)
-            database_version: Name of database version (if relevant)
-            model: Model name (if relevant)
-            source_format : Type of data being input e.g. openghg (internal format)
             high_time_resolution: If this is a high resolution file
-            period: Period of measurements. Only needed if this can not be inferred from the time coords
-            If specified, should be one of:
-                - "yearly", "monthly"
-                - suitable pandas Offset Alias
-                - tuple of (value, unit) as would be passed to pandas.Timedelta function
-            continuous: Whether time stamps have to be continuous.
+            period: Period of measurements, if not passed this is inferred from the time coords
             overwrite: Should this data overwrite currently stored data.
         Returns:
             dict: Dictionary of datasource UUIDs data assigned to
         """
-        from openghg.types import EmissionsTypes
-        from openghg.util import clean_string, hash_file, load_emissions_parser
+        from collections import defaultdict
+        from xarray import open_dataset
+        from openghg.store import assign_data
+        from openghg.util import (
+            clean_string,
+            hash_file,
+            pairwise,
+            timestamp_tzaware,
+            timestamp_now,
+        )
 
         species = clean_string(species)
         source = clean_string(source)
         domain = clean_string(domain)
+        date = clean_string(date)
 
         filepath = Path(filepath)
 
-        try:
-            source_format = EmissionsTypes[source_format.upper()].value
-        except KeyError:
-            raise ValueError(f"Unknown data type {source_format} selected.")
-
-        # Load the data retrieve object
-        parser_fn = load_emissions_parser(source_format=source_format)
+        em_store = Emissions.load()
 
         file_hash = hash_file(filepath=filepath)
-        if file_hash in self._file_hashes and not overwrite:
-            warnings.warn(
-                f"This file has been uploaded previously with the filename : {self._file_hashes[file_hash]} - skipping."
+        if file_hash in em_store._file_hashes and not overwrite:
+            print(
+                f"This file has been uploaded previously with the filename : {em_store._file_hashes[file_hash]} - skipping."
             )
-            return None
 
-        # Define parameters to pass to the parser function
-        # TODO: Update this to match against inputs for parser function.
-        param = {
-            "filepath": filepath,
-            "species": species,
-            "domain": domain,
-            "source": source,
-            "high_time_resolution": high_time_resolution,
-            "period": period,
-            "continuous": continuous,
-            "data_type": "emissions",
-            "chunks": chunks,
-        }
-
-        optional_keywords = {"database": database, "database_version": database_version, "model": model}
-
-        param.update(optional_keywords)
-
-        emissions_data = parser_fn(**param)
-
-        # Checking against expected format for Emissions
-        for split_data in emissions_data.values():
-            em_data = split_data["data"]
-            Emissions.validate_data(em_data)
-
-        min_required = ["species", "source", "domain"]
-        for key, value in optional_keywords.items():
-            if value is not None:
-                min_required.append(key)
+        em_data = open_dataset(filepath)
 
-        required = tuple(min_required)
+        # Some attributes are numpy types we can't serialise to JSON so convert them
+        # to their native types here
+        attrs = {}
+        for key, value in em_data.attrs.items():
+            try:
+                attrs[key] = value.item()
+            except AttributeError:
+                attrs[key] = value
+
+        author_name = "OpenGHG Cloud"
+        em_data.attrs["author"] = author_name
+
+        metadata = {}
+        metadata.update(attrs)
+
+        metadata["species"] = species
+        metadata["domain"] = domain
+        metadata["source"] = source
+        metadata["date"] = date
+        metadata["author"] = author_name
+        metadata["processed"] = str(timestamp_now())
+
+        # As emissions files handle things slightly differently we need to check the time values
+        # more carefully.
+        # e.g. a flux / emissions file could contain e.g. monthly data and be labelled as 2012 but
+        # contain 12 time points labelled as 2012-01-01, 2012-02-01, etc.
+        n_dates = em_data.time.size
+
+        # This covers the whole year
+        if n_dates == 1:
+            year = timestamp_tzaware(em_data.time[0].values).year
+            year_start = timestamp_tzaware(f"{year}-1-1-00:00:00")
+            year_end = timestamp_tzaware(f"{year}-12-31-23:59:59")
+
+            start_date = year_start
+            end_date = year_end
+            freq = "annual"
+        # We have values for each month / week
+        elif n_dates == 12:
+            # Check they're successive months
+            timestamps = [timestamp_tzaware(t) for t in em_data.time.values]
+
+            for a, b in pairwise(timestamps):
+                if a.month != b.month - 1:
+                    raise ValueError("We expect successive months for the data")
+
+            if timestamps[0].year != timestamps[-1].year:
+                raise ValueError("We expect a single year of data")
+
+            year = timestamps[0].year
+
+            year_start = timestamp_tzaware(f"{year}-1-1-00:00:00")
+            year_end = timestamp_tzaware(f"{year}-12-31-23:59:59")
+
+            start_date = year_start
+            end_date = year_end
+            freq = "month"
+        # Work run through the timestamps and check for gap between them ?
+        # Add something to metadata for this?
+        else:
+            timestamps = [timestamp_tzaware(t) for t in em_data.time.values]
+            timestamps.sort()
 
-        data_type = "emissions"
-        datasource_uuids = self.assign_data(
-            data=emissions_data, overwrite=overwrite, data_type=data_type, required_keys=required
-        )
-        # Record the file hash in case we see this file again
-        self._file_hashes[file_hash] = filepath.name
+            frequency = set()
 
-        return datasource_uuids
+            for a, b in pairwise(timestamps):
+                delta = b - a
+                frequency.add(delta)
 
-    def transform_data(
-        self,
-        datapath: Union[str, Path],
-        database: str,
-        overwrite: bool = False,
-        **kwargs: Dict,
-    ) -> Dict:
-        """
-        Read and transform an emissions database. This will find the appropriate
-        parser function to use for the database specified. The necessary inputs
-        are determined by which database ie being used.
-
-        The underlying parser functions will be of the form:
-            - openghg.transform.emissions.parse_{database.lower()}
-                - e.g. openghg.transform.emissions.parse_edgar()
+            start_date = timestamps[0]
+            end_date = timestamps[-1]
 
-        Args:
-            datapath: Path to local copy of database archive (for now)
-            database: Name of database
-            overwrite: Should this data overwrite currently stored data
-                which matches.
-            **kwargs: Inputs for underlying parser function for the database.
-                Necessary inputs will depend on the database being parsed.
-
-        TODO: Could allow Callable[..., Dataset] type for a pre-defined function be passed
-        """
-        import inspect
-        from openghg.types import EmissionsDatabases
-        from openghg.util import load_emissions_database_parser
+            if len(frequency) == 1:
+                freq = str(frequency.pop())
+            else:
+                freq = "varies"
 
-        datapath = Path(datapath)
+        metadata["start_date"] = str(start_date)
+        metadata["end_date"] = str(end_date)
 
-        try:
-            data_type = EmissionsDatabases[database.upper()].value
-        except KeyError:
-            raise ValueError(f"Unable to transform '{database}' selected.")
+        metadata["max_longitude"] = round(float(em_data["lon"].max()), 5)
+        metadata["min_longitude"] = round(float(em_data["lon"].min()), 5)
+        metadata["max_latitude"] = round(float(em_data["lat"].max()), 5)
+        metadata["min_latitude"] = round(float(em_data["lat"].min()), 5)
 
-        # Load the data retrieve object
-        parser_fn = load_emissions_database_parser(database=database)
+        metadata["time_resolution"] = "high" if high_time_resolution else "standard"
+        metadata["frequency"] = freq
 
-        # Find all parameters that can be accepted by parse function
-        all_param = list(inspect.signature(parser_fn).parameters.keys())
+        if period is not None:
+            metadata["time_period"] = period
 
-        # Define parameters to pass to the parser function from kwargs
-        param: Dict[Any, Any] = {key: value for key, value in kwargs.items() if key in all_param}
-        param["datapath"] = datapath  # Add datapath explicitly (for now)
+        key = "_".join((species, source, domain, date))
 
-        emissions_data = parser_fn(**param)
+        emissions_data: DefaultDict[str, Dict[str, Union[Dict, Dataset]]] = defaultdict(dict)
+        emissions_data[key]["data"] = em_data
+        emissions_data[key]["metadata"] = metadata
 
-        # Checking against expected format for Emissions
-        for split_data in emissions_data.values():
-            em_data = split_data["data"]
-            Emissions.validate_data(em_data)
+        keyed_metadata = {key: metadata}
 
-        required_keys = ("species", "source", "domain")
+        lookup_results = em_store.datasource_lookup(metadata=keyed_metadata)
 
         data_type = "emissions"
-        overwrite = False
-        datasource_uuids = self.assign_data(
-            data=emissions_data, overwrite=overwrite, data_type=data_type, required_keys=required_keys
+        datasource_uuids = assign_data(
+            data_dict=emissions_data,
+            lookup_results=lookup_results,
+            overwrite=overwrite,
+            data_type=data_type,
         )
 
-        return datasource_uuids
+        em_store.add_datasources(datasource_uuids=datasource_uuids, metadata=keyed_metadata)
 
-    @staticmethod
-    def schema() -> DataSchema:
-        """
-        Define schema for emissions Dataset.
+        # Record the file hash in case we see this file again
+        em_store._file_hashes[file_hash] = filepath.name
+
+        em_store.save()
 
-        Includes flux/emissions for each time and position:
-            - "flux"
-                - expected dimensions: ("time", "lat", "lon")
+        return datasource_uuids
 
-        Expected data types for all variables and coordinates also included.
+    def lookup_uuid(self, species: str, source: str, domain: str, date: str) -> Union[str, bool]:
+        """Perform a lookup for the UUID of a Datasource
 
+        Args:
+            species: Site code
+            domain: Domain
+            model: Model name
+            height: Height
         Returns:
-            DataSchema : Contains schema for Emissions.
+            str or dict: UUID or False if no entry
         """
-        data_vars: Dict[str, Tuple[str, ...]] = {"flux": ("time", "lat", "lon")}
-        dtypes = {"lat": np.floating, "lon": np.floating, "time": np.datetime64, "flux": np.floating}
+        uuid = self._datasource_table[species][source][domain][date]
 
-        data_format = DataSchema(data_vars=data_vars, dtypes=dtypes)
+        return uuid if uuid else False
 
-        return data_format
+    def set_uuid(self, species: str, source: str, domain: str, date: str, uuid: str) -> None:
+        """Record a UUID of a Datasource in the datasource table
 
-    @staticmethod
-    def validate_data(data: Dataset) -> None:
+        Args:
+            site: Site code
+            domain: Domain
+            model: Model name
+            height: Height
+            uuid: UUID of Datasource
+        Returns:
+            None
         """
-        Validate input data against Emissions schema - definition from
-        Emissions.schema() method.
+        self._datasource_table[species][source][domain][date] = uuid
+
+    def datasource_lookup(self, metadata: Dict) -> Dict[str, Union[str, bool]]:
+        """Find the Datasource we should assign the data to
 
         Args:
-            data : xarray Dataset in expected format
+            metadata: Dictionary of metadata
+        Returns:
+            dict: Dictionary of datasource information
+        """
+        # TODO - I'll leave this as a function for now as the way we read emissions may
+        # change in the near future
+        # GJ - 2021-04-20
+        lookup_results = {}
+
+        for key, data in metadata.items():
+            species = data["species"]
+            source = data["source"]
+            domain = data["domain"]
+            date = data["date"]
 
+            lookup_results[key] = self.lookup_uuid(species=species, source=source, domain=domain, date=date)
+
+        return lookup_results
+
+    def add_datasources(self, datasource_uuids: Dict, metadata: Dict) -> None:
+        """Add the passed list of Datasources to the current list
+
+        Args:
+            datasource_uuids: Datasource UUIDs
+            metadata: Metadata for each species
         Returns:
             None
-
-            Raises a ValueError with details if the input data does not adhere
-            to the Emissions schema.
         """
-        data_schema = Emissions.schema()
-        data_schema.validate_data(data)
+        for key, uid in datasource_uuids.items():
+            md = metadata[key]
+            species = md["species"]
+            source = md["source"]
+            domain = md["domain"]
+            date = md["date"]
+
+            result = self.lookup_uuid(species=species, source=source, domain=domain, date=date)
+
+            if result and result != uid:
+                raise ValueError("Mismatch between assigned uuid and stored Datasource uuid.")
+            else:
+                self.set_uuid(species=species, source=source, domain=domain, date=date, uuid=uid)
+                self._datasource_uuids[uid] = key
```

### Comparing `openghg-0.6.0/openghg/store/_metstore.py` & `openghg-1.0.0/openghg/store/_metstore.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from __future__ import annotations
-
-from typing import TYPE_CHECKING, List, Union
-
 from openghg.store.base import BaseStore
 from pandas import Timestamp
+from typing import TYPE_CHECKING, List, Union
 
 if TYPE_CHECKING:
     from openghg.dataobjects import METData
 
 
 class METStore(BaseStore):
     """Controls the storage and retrieveal of meteorological data.
@@ -23,15 +21,14 @@
         """Save the object to the object store
 
         Args:
             bucket: Bucket for data
         Returns:
             None
         """
-        raise NotImplementedError("We are working to replace the MetStore.")
         from openghg.objectstore import get_bucket, set_object_from_json
 
         bucket = get_bucket()
 
         obs_key = f"{METStore._root}/uuid/{METStore._uuid}"
 
         self._stored = True
@@ -45,15 +42,14 @@
         Args:
             site: Three letter site code
             network: Network name
             years: Year(s) required
         Returns:
             METData: METData object holding data and metadata
         """
-        raise NotImplementedError("We are working to replace the MetStore.")
         from openghg.retrieve.met import retrieve_met
         from pandas import Timestamp
 
         if not isinstance(years, list):
             years = [years]
         else:
             years = sorted(years)
@@ -88,17 +84,16 @@
             network: Network name
             start_date: Start date
             end_date: End date
 
         Returns:
             METData or None: METData object if found else None
         """
-        raise NotImplementedError("We are working to replace the MetStore.")
-        from openghg.dataobjects import METData
         from openghg.store.base import Datasource
+        from openghg.dataobjects import METData
 
         datasources = (Datasource.load(uuid=uuid, shallow=True) for uuid in self._datasource_uuids)
 
         # We should only get one datasource here currently
         for datasource in datasources:
             if datasource.search_metadata(site=site, network=network, find_all=True):
                 if datasource.in_daterange(start_date=start_date, end_date=end_date):
@@ -115,15 +110,14 @@
         format to Datasources used in other modules of OpenGHG.
 
         Args:
             met_data: Dataset
         Returns:
             None
         """
-        raise NotImplementedError("We are working to replace the MetStore.")
         from openghg.store.base import Datasource
 
         metadata = met_data.metadata
 
         datasource = Datasource()
         datasource.add_data(metadata=metadata, data=met_data.data, data_type="met")
         datasource.save()
```

### Comparing `openghg-0.6.0/openghg/store/_populate.py` & `openghg-1.0.0/openghg/store/_populate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 from pathlib import Path
 from typing import Dict, List, Optional, Union
-import logging
-from openghg.objectstore import get_writable_bucket
 from openghg.store import ObsSurface
 
-logger = logging.getLogger("openghg.store")
-logger.setLevel(logging.DEBUG)  # Have to set level for logger as well as handler
-
 
 def add_noaa_obspack(
-    data_directory: Union[str, Path],
-    project: Optional[str] = None,
-    overwrite: bool = False,
-    store: Optional[str] = None,
+    data_directory: Union[str, Path], project: Optional[str] = None, overwrite: bool = False
 ) -> Dict:
     """
     Function to detect and add files from the NOAA ObsPack to the object store.
 
     Args:
         data_directory: Top level directory for the downloaded NOAA ObsPack
         project (optional) : Can specify project or type to process only e.g. "surface"
         or "surface-flask"
         overwrite : Whether to overwrite existing entries in the object store
-        store: Name of object store to write to
     Returns:
         Dict: Details of data which has been processed into the object store
     Examples:
         To add all NOAA ObsPack data (which can be processed) to the object store:
         >>> add_noaa_obspack(Path("/home/user/obspack_ch4_1_GLOBALVIEWplus_v2.0_2020-04-24"))
         {"processed": {"ch4_esp_surface-flask_2_representative.nc":{"ch4": ...}, ...}}
 
@@ -56,82 +47,66 @@
         "shipboard": ["flask"],
         "aircorenoaa": [""],
     }
 
     project_names_not_implemented = _create_project_names(project_options_not_implemented_yet)
 
     # If a specific project has been specified, extract file matching strings
-    if project is not None:
+    if project:
         if project in project_names:
             projects_to_read = [project]
         elif project in project_options:
             projects_to_read = [name for name in project_names if project in name]
         elif project in project_options_not_implemented_yet or project in project_names_not_implemented:
             raise ValueError(f"Functionality to process {project} data has not been implemented yet.")
         else:
             raise ValueError(f"Did not recognise input {project} for project")
     else:
         projects_to_read = project_names
-        logger.info(f"Reading subset of data from {','.join(projects_to_read)}")
+        print(f"Reading subset of data from {','.join(projects_to_read)}")
 
     if isinstance(data_directory, str):
         data_directory = Path(data_directory)
 
     # ObsPack may contain nc or txt files
     # Try and extract one and then the other if possible
-    files = _find_noaa_files(data_directory=data_directory, ext=".nc")
+    files = _find_noaa_files(data_directory, ".nc")
     if not files:
-        files = _find_noaa_files(data_directory=data_directory, ext=".txt")
-
-    bucket = get_writable_bucket(name=store)
+        files = _find_noaa_files(data_directory, ".txt")
 
-    # TODO - remove this once we can ensure all files will be processed correctly
-    files_with_errors = []
     # Find relevant details for each file and call parse_noaa() function
     processed_summary: Dict[str, Dict] = {}
     for filepath in files:
         param = _param_from_filename(filepath)
         site = param["site"]
-        _project = param["project"]
+        project = param["project"]
         measurement_type = param["measurement_type"]
 
-        if _project in projects_to_read:
-            try:
-                # TODO - can we streamline this a bit to save repeated loads?
-                with ObsSurface(bucket=bucket) as obs:
-                    processed = obs.read_file(
-                        filepath,
-                        site=site,
-                        measurement_type=measurement_type,
-                        network="NOAA",
-                        source_format="NOAA",
-                        overwrite=overwrite,
-                    )
-            except Exception:
-                files_with_errors.append(filepath.name)
-
-        elif _project in project_names_not_implemented:
-            logger.warning(
-                f"Not processing {filepath.name} - no standardisation for {_project} data implemented yet."
+        if project in projects_to_read:
+            processed = ObsSurface.read_file(
+                filepath,
+                site=site,
+                measurement_type=measurement_type,
+                network="NOAA",
+                data_type="NOAA",
+                overwrite=overwrite,
             )
+        elif project in project_names_not_implemented:
+            print(f"Not processing {filepath.name} - no standardisation for {project} data implemented yet.")
             processed = {}
         else:
             processed = {}
 
         # Expect "processed" dictionary and/or "error" dictionary within `processed`
         for key, value in processed.items():
             if key not in processed_summary:
                 processed_summary[key] = {}
             for key_in, value_in in value.items():
                 processed_summary[key][key_in] = value_in
 
-    if files_with_errors:
-        err_string = "\n".join(files_with_errors)
-        logger.info(f"We were unable to process {len(files_with_errors)} files - these were:\n {err_string}.")
-
     return processed_summary
 
 
 def _param_from_filename(filename: Union[str, Path]) -> Dict:
     """
     Extract parameter from the NOAA filename based on the agreed naming convention.
     See: https://gml.noaa.gov/ccgg/obspack/documentation.html
@@ -142,30 +117,31 @@
         filename: NOAA ObsPack filename with expected naming convention
     Returns:
         Dict : Extracted parameters from filename
     Examples:
         >>> _param_from_filename("ch4_esp_surface-flask_2_representative.nc")
         {"species": "ch4", "site" : "esp", "project": "surface-flask", "measurement_type": "flask"}
     """
+
     if isinstance(filename, str):
         extracted_param = filename.split("_")
     else:
         extracted_param = filename.name.split("_")
-
     param = {}
     param["species"] = extracted_param[0]
     param["site"] = extracted_param[1]
     param["project"] = extracted_param[2]
     param["measurement_type"] = param["project"].split("-")[-1]
 
     return param
 
 
 def _create_project_names(input_dict: Dict) -> List:
-    """Creates full project names as would be included in the NOAA filepath
+    """
+    Creates full project names as would be included in the NOAA filepath
 
     Expects input dictionary for each the type e.g. "surface" and the
     associated measurement types e.g. ["flask", "insitu", "pfp"]
 
     Args:
         input_dict: In format described above
     Returns:
@@ -176,27 +152,26 @@
         >>> _create_project_names(input_dict)
            ["surface-flask", "surface-insitu", "surface-php"]
     """
     projects = []
     for key, values in input_dict.items():
         if not isinstance(values, list):
             values = [values]
-
         full_names = ["-".join([key, value]) for value in values]
         projects.extend(full_names)
-
     return projects
 
 
-def _find_noaa_files(data_directory: Union[str, Path], ext: str) -> List[Path]:
-    """Find obs files in NOAA ObsPack.
+def _find_noaa_files(data_directory: Union[str, Path], ext: str) -> List:
+    """
+    Find obs files in NOAA ObsPack.
 
     Expected directory structure is:
      - <ObsPack>/data/<filetype>/
-         - e.g. obspack_ch4_1_GLOBALVIEWplus_v2.0_2020-04-24/data/nc/
+       - e.g. obspack_ch4_1_GLOBALVIEWplus_v2.0_2020-04-24/data/nc/
 
     Args:
         data_directory: Top level ObsPack data directory to search
         ext: Extension for files. Should be either ".txt" or ".nc"
     Returns:
         list: Filenames with appropriate extension
     Examples:
@@ -204,36 +179,34 @@
         >>> _find_noaa_files(Path("/home/user/obspack_ch4_1_GLOBALVIEWplus_v2.0_2020-04-24"), ".txt")
         ["co_pocn25_surface-flask_1_ccgg_event.txt", ...]
 
         Or optionally can include more direct subdirectory (for nc files):
         >>> _find_noaa_files("/home/user/obspack_ch4_1_GLOBALVIEWplus_v2.0_2020-04-24/data/nc", ".nc")
         ["ch4_esp_surface-flask_2_representative.nc", ...]
     """
+
     # ObsPack may contain nc or txt files:
     # - For nc files found, these should all the data files
     # - For txt files found, we need to make sure files are found in the correct
     # sub-directory as otherwise this may find README and summary files
     if ext == ".nc":
         subdirectories = ["data/nc", "nc", ""]
     elif ext == ".txt":
         subdirectories = ["data/txt", "txt"]
     else:
-        raise ValueError(f"Did not recognise input for extension: {ext}. Should be one of '.txt' or '.nc'")
+        raise ValueError("Did not recognise input for extension: {ext}. Should be one of '.txt' or '.nc'")
 
     data_directory = Path(data_directory).expanduser().resolve()
 
     # Allow user to specify various levels within ObsPack to e.g. just
     # extract nc files.
     for subdir in subdirectories:
         path_to_search = data_directory / subdir
-
-        logger.info(f"Searching for {ext} files within {path_to_search}")
-
+        print(f"Searching for {ext} files within {path_to_search}")
         files = list(path_to_search.glob(f"*{ext}"))
         suffix_values = [file.suffix for file in files]
-
         if ext in suffix_values:
             break
     else:
         files = []
 
     return files
```

### Comparing `openghg-0.6.0/openghg/store/_recombination.py` & `openghg-1.0.0/openghg/store/_recombination.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 """ Handles the recombination of dataframes stored in the object store
     into the data requested by the user
 
 """
 from typing import Dict, List, Optional, Union
-
+from xarray import Dataset, DataArray
+from xarray.core.coordinates import DatasetCoordinates
 import numpy as np
 import xarray as xr
-from xarray.core.coordinates import DatasetCoordinates
 
 __all__ = ["recombine_multisite", "recombine_datasets"]
 
 
 def recombine_multisite(keys: Dict, sort: Optional[bool] = True) -> Dict:
     """Recombine the keys from multiple sites into a single Dataset for each site
 
     Args:
         site_keys: A dictionary of lists of keys, keyed by site
         sort: Sort the resulting Dataset by the time dimension
     Returns:
         dict: Dictionary of xarray.Datasets
     """
-    raise NotImplementedError
-    # result = {}
-    # for key, key_list in keys.items():
-    #     result[key] = recombine_datasets(keys=key_list, sort=sort)
+    result = {}
+    for key, key_list in keys.items():
+        result[key] = recombine_datasets(keys=key_list, sort=sort)
 
-    # return result
+    return result
 
 
 def recombine_datasets(
-    bucket: str,
     keys: List[str],
     sort: Optional[bool] = True,
-    attrs_to_check: Optional[Dict[str, str]] = None,
+    attrs_to_check: Dict[str, str] = None,
     elevate_inlet: bool = False,
-) -> xr.Dataset:
+) -> Dataset:
     """Combines datasets stored separately in the object store
     into a single dataset
 
     Args:
-        bucket: Object store bucket to retrieve data from
         keys: List of object store keys
-        sort: Sort the resulting Dataset by the time dimension, defaults to False
+        sort: Sort the resulting Dataset by the time dimension. Default = True
         attrs_to_check: Attributes to check for duplicates. If duplicates are present
             a new data variable will be created containing the values from each dataset
             If a dictionary is passed, the attribute(s) will be retained and the new value assigned.
             If a list/string is passed, the attribute(s) will be removed.
         elevate_inlet: Force the elevation of the inlet attribute
     Returns:
         xarray.Dataset: Combined Dataset
     """
-    from openghg.store.base import Datasource
     from xarray import concat as xr_concat
+    from openghg.store.base import Datasource
+    from openghg.objectstore import get_bucket
 
     if not keys:
         raise ValueError("No data keys passed.")
 
+    bucket = get_bucket()
+
     data = [Datasource.load_dataset(bucket=bucket, key=k) for k in keys]
 
     # Check if we've got multiple inlet heights
     inlets_to_check = check_inlets(data=data, elevate_inlet=elevate_inlet)
 
     if attrs_to_check is None:
         attrs_to_check = {}
@@ -80,18 +80,15 @@
         # else:
         #     attributes = attrs_to_check
         #     replace_values = [""] * len(attributes)
 
         data = elevate_duplicate_attrs(ds_list=data, attributes=attributes, elevate_inlet=elevate_inlet)
 
     # Concatenate datasets along time dimension
-    if len(data) > 1:
-        combined = xr_concat(data, dim="time")
-    else:
-        combined = data[0]
+    combined = xr_concat(data, dim="time")
 
     # Replace/remove incorrect attributes
     #  - xr.concat will only take value from first dataset if duplicated
     if attrs_to_check:
         for attr, value in zip(attributes, replace_values):
             if attr in combined:  # Only update if attr was elevated to a data variable
                 if value:
@@ -100,39 +97,29 @@
                     combined.attrs.pop(attr)
 
     if sort:
         combined = combined.sortby("time")
 
     # This is modified from https://stackoverflow.com/a/51077784/1303032
     unique, index, count = np.unique(combined.time, return_counts=True, return_index=True)
-    n_dupes = unique[count > 1].size
-    # dupes = unique[count > 1]
 
+    n_dupes = unique[count > 1].size
     if n_dupes > 5:
         raise ValueError("Large number of duplicate timestamps, check data overlap.")
 
-    # print(f"\n\nNumber of dupes: {n_dupes}")
-    # Using isel is a memory hungry operation, there's no point doing it if we don't have any dupes
-    # if n_dupes > 0:
-    #     combined = combined.isel(time=index)
-
-    # Only keep the unique values if we have dupes
-    # if index.size != combined.time.size:
-    #    combined = combined.isel(time=index)
-    if sort:
-        combined = combined.sortby("time")
+    combined = combined.isel(time=index)
 
     return combined
 
 
 def create_array_from_value(
     value: str,
     coords: Union[DatasetCoordinates, Dict[str, DatasetCoordinates]],  # type: ignore
     name: Union[str, None] = None,
-) -> xr.DataArray:
+) -> DataArray:
     """
     Create a new xarray.DataArray object containing a single value repeated
     for each coordinate.
 
     Args:
         value: Value to be repeated within the DataArray object
         coords: Co-ordinates to use for this new DataArray.
@@ -151,16 +138,16 @@
     variable = np.tile(value, dims)
     data_variable = xr.DataArray(variable, coords=coords, name=name)
 
     return data_variable
 
 
 def elevate_duplicate_attrs(
-    ds_list: List[xr.Dataset], attributes: Union[str, List[str]], elevate_inlet: bool
-) -> List[xr.Dataset]:
+    ds_list: List[Dataset], attributes: Union[str, List[str]], elevate_inlet: bool
+) -> List[Dataset]:
     """
     For a list of Datasets, if the specified attributes are being repeated
     these will be added as new data variables to each Dataset.
 
     Args:
         ds_list: List of xarray Datasets
         attributes: Attribute values to check within the Datasets. If None is passed
@@ -186,15 +173,15 @@
                 updated_ds = ds.assign({attr: new_variable})
 
                 ds_list[i] = updated_ds
 
     return ds_list
 
 
-def check_inlets(data: List[xr.Dataset], elevate_inlet: bool) -> Dict:
+def check_inlets(data: List[Dataset], elevate_inlet: bool) -> Dict:
     """Check the inlets of the data to be processed
 
     Args:
         data: List of Datasets
     Returns:
         dict: Dictionary with single or multiple inlet replacement value
     """
```

### Comparing `openghg-0.6.0/openghg/store/_segment.py` & `openghg-1.0.0/openghg/store/_segment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 """ Segment the data into Datasources
 
 """
 from typing import Dict
-import logging
 
 __all__ = ["assign_data"]
 
 
-logger = logging.getLogger("openghg.store")
-logger.setLevel(logging.DEBUG)  # Have to set level for logger as well as handler
-
-
 def assign_data(
     data_dict: Dict,
     lookup_results: Dict,
-    data_type: str,
     overwrite: bool,
-) -> Dict[str, Dict]:
+    data_type: str = "timeseries",
+) -> Dict[str, str]:
     """Assign data to a Datasource. This will either create a new Datasource
     Create or get an existing Datasource for each gas in the file
 
         Args:
             data_dict: Dictionary containing data and metadata for species
             lookup_results: Dictionary of lookup results]
-            data_type: Type of data, one of ["surface", "emissions", "met", "footprints", "eulerian_model"].
             overwrite: If True overwrite current data stored
         Returns:
             dict: Dictionary of UUIDs of Datasources data has been assigned to keyed by species name
     """
-    raise NotImplementedError("This will be removed.")
     from openghg.store.base import Datasource
 
     uuids = {}
 
     for key in data_dict:
         metadata = data_dict[key]["metadata"]
         data = data_dict[key]["data"]
 
         # Our lookup results and gas data have the same keys
         uuid = lookup_results[key]
 
+        # TODO - Could this be done somewhere else? It doesn't feel quite right it
+        # being here
+
         # Add the read metadata to the Dataset attributes being careful
         # not to overwrite any attributes that are already there
         to_add = {k: v for k, v in metadata.items() if k not in data.attrs}
         data.attrs.update(to_add)
 
         # If we have a UUID for this Datasource load the existing object
         # from the object store
@@ -53,16 +49,15 @@
             datasource = Datasource.load(uuid=uuid)
 
         # Add the dataframe to the datasource
         datasource.add_data(metadata=metadata, data=data, overwrite=overwrite, data_type=data_type)
         # Save Datasource to object store
         datasource.save()
 
-        new_datasource = uuid is False
-        uuids[key] = {"uuid": datasource.uuid(), "new": new_datasource}
+        uuids[key] = datasource.uuid()
 
     return uuids
 
 
 # def assign_footprint_data(footprint_data: Dict, lookup_results: Dict, overwrite: bool) -> Dict:
 #     """ Create Datasources for the passed footprints data
```

### Comparing `openghg-0.6.0/openghg/store/base/_base.py` & `openghg-1.0.0/openghg/store/base/_base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,245 +1,184 @@
-""" This file contains the BaseStore class from which other storage
+""" This file contains the BaseStore class from which other retrieve
     modules inherit.
 """
-from typing import Any, Dict, List, Optional, Sequence, TypeVar, Union
+from typing import Dict, List, Optional, Union, Type, TypeVar
 from pandas import Timestamp
-import tinydb
-import logging
-from functools import reduce
-from openghg.types import DatasourceLookupError
-from openghg.objectstore import get_object_from_json, exists, set_object_from_json
-from openghg.util import timestamp_now
 
+__all__ = ["BaseStore"]
 
 T = TypeVar("T", bound="BaseStore")
 
-logger = logging.getLogger("openghg.store")
-logger.setLevel(logging.DEBUG)  # Have to set level for logger as well as handler
-
-
-def _find_and(x: Any, y: Any) -> Any:
-    return x & y
-
 
 class BaseStore:
     _root = "root"
     _uuid = "root_uuid"
 
-    def __init__(self, bucket: str) -> None:
-        from openghg.store import load_metastore
+    def __init__(self) -> None:
+        from openghg.util import timestamp_now
+        from addict import Dict as aDict
 
-        self._creation_datetime = str(timestamp_now())
+        self._creation_datetime = timestamp_now()
         self._stored = False
+
+        # Use an addict Dict here for easy nested data storage
+        self._datasource_table = aDict()
         # Keyed by Datasource UUID
         self._datasource_uuids: Dict[str, str] = {}
         # Hashes of previously uploaded files
         self._file_hashes: Dict[str, str] = {}
-        # Hashes of previously stored data from other data platforms
-        self._retrieved_hashes: Dict[str, Dict] = {}
-        # Where we'll store this object
-        self._bucket = bucket
-        self._metakey = ""
-        self._metastore = load_metastore(bucket=bucket, key=self.metakey())
-
-        if exists(bucket=bucket, key=self.key()):
-            data = get_object_from_json(bucket=bucket, key=self.key())
-            # Update myself
-            self.__dict__.update(data)
+        # Keyed by UUID
+        self._rank_data = aDict()
+
+    def is_null(self) -> bool:
+        return not self.datasources
 
     @classmethod
-    def metakey(cls) -> str:
-        return str(cls._metakey)
+    def exists(cls: Type[T], bucket: Optional[str] = None) -> bool:
+        """Check if the object is already saved in the object
+        store
+
+        Args:
+            bucket: Bucket for data storage
+        Returns:
+            bool: True if object exists
+        """
+        from openghg.objectstore import exists, get_bucket
+
+        if bucket is None:
+            bucket = get_bucket()
+
+        key = f"{cls._root}/uuid/{cls._uuid}"
+
+        does_exist: bool = exists(bucket=bucket, key=key)
+
+        return does_exist
 
     @classmethod
-    def key(cls) -> str:
-        return f"{cls._root}/uuid/{cls._uuid}"
+    def from_data(cls: Type[T], data: Dict) -> T:
+        """Create an object from data
+
+        Args:
+            data: JSON data
+        Returns:
+            cls: Class object of cls type
+        """
+        from openghg.util import timestamp_tzaware
+        from addict import Dict as aDict
 
-    def save(self) -> None:
-        self._metastore.close()
-        set_object_from_json(bucket=self._bucket, key=self.key(), data=self.to_data())
+        if not data:
+            raise ValueError("Unable to create object with empty dictionary")
+
+        c = cls()
+        c._creation_datetime = timestamp_tzaware(data["creation_datetime"])
+        c._datasource_uuids = data["datasource_uuids"]
+        c._file_hashes = data["file_hashes"]
+        c._datasource_table = aDict(data["datasource_table"])
+        c._rank_data = aDict(data["rank_data"])
+        c._stored = False
+
+        return c
 
     def to_data(self) -> Dict:
-        # We don't need to store the metadata store, it has its own location
-        # QUESTION - Is this cleaner than the previous specifying
-        DO_NOT_STORE = ["_metastore"]
-        return {k: v for k, v in self.__dict__.items() if k not in DO_NOT_STORE}
-
-    def assign_data(
-        self,
-        data: Dict,
-        overwrite: bool,
-        data_type: str,
-        required_keys: Sequence[str],
-        min_keys: Optional[int] = None,
-        update_keys: Optional[List] = None,
-    ) -> Dict[str, Dict]:
-        """Assign data to a Datasource. This will either create a new Datasource
-        Create or get an existing Datasource for each gas in the file
-
-            Args:
-                data: Dictionary containing data and metadata for species
-                overwrite: If True overwrite current data stored
-                data_type: Type of data, timeseries etc
-                required_keys: Required minimum keys to lookup unique Datasource
-                min_keys: Minimum number of metadata keys needed to uniquely match a Datasource
-            Returns:
-                dict: Dictionary of UUIDs of Datasources data has been assigned to keyed by species name
+        """Return a JSON-serialisable dictionary of object
+        for storage in object store
+
+        Returns:
+            dict: Dictionary version of object
         """
-        from openghg.store.base import Datasource
-        from openghg.util import to_lowercase
+        data: Dict[str, Union[str, bool, Dict]] = {}
+        data["creation_datetime"] = str(self._creation_datetime)
+        data["stored"] = self._stored
+        data["datasource_table"] = self._datasource_table
+        data["datasource_uuids"] = self._datasource_uuids
+        data["file_hashes"] = self._file_hashes
+        data["rank_data"] = self._rank_data
 
-        uuids = {}
+        return data
 
-        lookup_results = self.datasource_lookup(data=data, required_keys=required_keys, min_keys=min_keys)
-        # TODO - remove this when the lowercasing of metadata gets removed
-        # We currently lowercase all the metadata and some keys we don't want to change, such as paths to the object store
-        skip_keys = ["object_store"]
-
-        for key, parsed_data in data.items():
-            metadata = parsed_data["metadata"]
-            _data = parsed_data["data"]
-
-            # Our lookup results and gas data have the same keys
-            uuid = lookup_results[key]
-
-            # Add the read metadata to the Dataset attributes being careful
-            # not to overwrite any attributes that are already there
-            to_add = {k: v for k, v in metadata.items() if k not in _data.attrs}
-            _data.attrs.update(to_add)
-
-            # If we have a UUID for this Datasource load the existing object
-            # from the object store
-            # If we haven't stored data with this metadata before we create a new Datasource
-            # and add the metadata to our metastore
-
-            # Take a copy of the metadata so we can update it
-            meta_copy = metadata.copy()
-
-            new_ds = uuid is False
-
-            if new_ds:
-                datasource = Datasource()
-                uid = datasource.uuid()
-                meta_copy["uuid"] = uid
-                # For retrieval later we'll need to know which bucket this is stored in
-                meta_copy["object_store"] = self._bucket
-
-                # Make sure all the metadata is lowercase for easier searching later
-                # TODO - do we want to do this or should be just perform lowercase comparisons?
-                meta_copy = to_lowercase(d=meta_copy, skip_keys=skip_keys)
-                # TODO - 2023-05-25 - Remove the need for this key, this should just be a set
-                # so we can have rapid
-                self._datasource_uuids[uid] = key
-            else:
-                datasource = Datasource.load(bucket=self._bucket, uuid=uuid)
-
-            # Add the dataframe to the datasource
-            datasource.add_data(
-                metadata=meta_copy, data=_data, overwrite=overwrite, data_type=data_type, skip_keys=skip_keys
-            )
-            # Save Datasource to object store
-            datasource.save(bucket=self._bucket)
-
-            # Add the metadata to the metastore and make sure it's up to date with the metadata stored
-            # in the Datasource
-            datasource_metadata = datasource.metadata()
-            if new_ds:
-                self._metastore.insert(datasource_metadata)
-            else:
-                self._metastore.update(datasource_metadata, tinydb.where("uuid") == datasource.uuid())
-
-            uuids[key] = {"uuid": datasource.uuid(), "new": new_ds}
-
-        return uuids
-
-    def datasource_lookup(
-        self, data: Dict, required_keys: Sequence[str], min_keys: Optional[int] = None
-    ) -> Dict:
-        """Search the metadata store for a Datasource UUID using the metadata in data. We expect the required_keys
-        to be present and will require at leas min_keys of these to be present when searching.
+    @classmethod
+    def load(cls: Type[T], bucket: Optional[str] = None) -> T:
+        """Load an object from the datastore using the passed
+        bucket and UUID
+
+        Args:
+            bucket: Bucket to store object
+        Returns:
+            class: Class created from JSON data
+        """
+        from openghg.objectstore import get_bucket, get_object_from_json
+
+        if not cls.exists():
+            return cls()
 
-        As some metadata value might change (such as data owners etc) we don't want to do an exact
-        search on *all* the metadata so we extract a subset (the required keys) and search for these.
+        if bucket is None:
+            bucket = get_bucket()
+
+        key = f"{cls._root}/uuid/{cls._uuid}"
+        data = get_object_from_json(bucket=bucket, key=key)
+
+        return cls.from_data(data=data)
+
+    def save(cls) -> None:
+        """Save the object to the object store
 
         Args:
-            metastore: Metadata database
-            data: Combined data dictionary of form {key: {data: Dataset, metadata: Dict}}
-            required_keys: Iterable of keys to extract from metadata
-            min_keys: The minimum number of required keys, if not given it will be set
-            to the length of required_keys
-        Return:
-            dict: Dictionary of datasource information
-        """
-        if min_keys is None:
-            min_keys = len(required_keys)
-
-        results = {}
-        for key, _data in data.items():
-            metadata = _data["metadata"]
-            required_metadata = {k.lower(): str(v).lower() for k, v in metadata.items() if k in required_keys}
-
-            if len(required_metadata) < min_keys:
-                raise ValueError(
-                    f"The given metadata doesn't contain enough information, we need: {required_keys}"
-                )
-
-            q = tinydb.Query()
-            search_attrs = [getattr(q, k) == v for k, v in required_metadata.items()]
-            required_result = self._metastore.search(reduce(_find_and, search_attrs))
-
-            if not required_result:
-                results[key] = False
-            elif len(required_result) > 1:
-                raise DatasourceLookupError("More than once Datasource found for metadata, refine lookup.")
-            else:
-                results[key] = required_result[0]["uuid"]
+            bucket: Bucket for data
+        Returns:
+            None
+        """
+        from openghg.objectstore import get_bucket, set_object_from_json
+
+        bucket = get_bucket()
+
+        obs_key = f"{cls._root}/uuid/{cls._uuid}"
 
-        return results
+        cls._stored = True
+        set_object_from_json(bucket=bucket, key=obs_key, data=cls.to_data())
 
-    def uuid(self) -> str:
+    @classmethod
+    def uuid(cls: Type[T]) -> str:
         """Return the UUID of this object
 
         Returns:
             str: UUID of object
         """
-        return self._uuid
+        return cls._uuid
 
-    def datasources(self) -> List[str]:
+    def datasources(self: T) -> List[str]:
         """Return the list of Datasources UUIDs associated with this object
 
         Returns:
             list: List of Datasource UUIDs
         """
         return list(self._datasource_uuids.keys())
 
-    def remove_datasource(self, uuid: str) -> None:
+    def remove_datasource(self: T, uuid: str) -> None:
         """Remove the Datasource with the given uuid from the list
         of Datasources
 
         Args:
-            uuid: UUID of Datasource to be removed
+            uuid (str): UUID of Datasource to be removed
         Returns:
             None
         """
         del self._datasource_uuids[uuid]
 
-    def get_rank(self, uuid: str, start_date: Timestamp, end_date: Timestamp) -> Dict:
+    def get_rank(self: T, uuid: str, start_date: Timestamp, end_date: Timestamp) -> Dict:
         """Get the rank for the given Datasource for a given date range
 
         Args:
             uuid: UUID of Datasource
             start_date: Start date
             end_date: End date
         Returns:
             dict: Dictionary of rank and daterange covered by that rank
         """
-        raise NotImplementedError("Ranking is being reworked and will be reactivated in a future release.")
+        from openghg.util import daterange_overlap, create_daterange_str
         from collections import defaultdict
-        from openghg.util import create_daterange_str, daterange_overlap
 
         if uuid not in self._rank_data:
             return {}
 
         search_daterange = create_daterange_str(start=start_date, end=end_date)
 
         rank_data = self._rank_data[uuid]
@@ -248,31 +187,30 @@
         # Check if this Datasource is ranked for the dates passed
         for daterange, rank in rank_data.items():
             if daterange_overlap(daterange_a=search_daterange, daterange_b=daterange):
                 ranked[rank].append(daterange)
 
         return ranked
 
-    def clear_rank(self, uuid: str) -> None:
+    def clear_rank(self: T, uuid: str) -> None:
         """Clear the ranking data for a Datasource
 
         Args:
             uuid: UUID of Datasource
         Returns:
             None
         """
-        raise NotImplementedError("Ranking is being reworked and will be reactivated in a future release.")
         if uuid in self._rank_data:
             del self._rank_data[uuid]
             self.save()
         else:
             raise ValueError("No ranking data set for that UUID.")
 
     def set_rank(
-        self,
+        self: T,
         uuid: str,
         rank: Union[int, str],
         date_range: Union[str, List[str]],
         overwrite: Optional[bool] = False,
     ) -> None:
         """Set the rank of a Datasource associated with this object.
 
@@ -286,24 +224,22 @@
             uuid: UUID of Datasource
             rank: Rank of data
             date_range: Daterange(s)
             overwrite: Overwrite current ranking data
         Returns:
             None
         """
-        raise NotImplementedError("Ranking is being reworked and will be reactivated in a future release.")
         from copy import deepcopy
-
         from openghg.util import (
             combine_dateranges,
-            daterange_contains,
             daterange_overlap,
-            sanitise_daterange,
-            split_encompassed_daterange,
             trim_daterange,
+            daterange_contains,
+            split_encompassed_daterange,
+            sanitise_daterange,
         )
 
         rank = int(rank)
 
         if not 1 <= rank <= 10:
             raise TypeError("Rank can only take values 1 to 10 (for unranked). Where 1 is the highest rank.")
 
@@ -407,26 +343,26 @@
                 self._rank_data[uuid][d] = rank
         else:
             for d in date_range:
                 self._rank_data[uuid][d] = rank
 
         self.save()
 
-    def rank_data(self) -> Dict:
+    def rank_data(self: T) -> Dict:
         """Return a dictionary of rank data keyed
         by UUID
 
             Returns:
                 dict: Dictionary of rank data
         """
-        raise NotImplementedError("Ranking is being reworked and will be reactivated in a future release.")
         rank_dict: Dict = self._rank_data.to_dict()
         return rank_dict
 
-    def clear_datasources(self) -> None:
+    def clear_datasources(self: T) -> None:
         """Remove all Datasources from the object
 
         Returns:
             None
         """
+        self._datasource_table.clear()
         self._datasource_uuids.clear()
         self._file_hashes.clear()
```

### Comparing `openghg-0.6.0/openghg/store/base/_datasource.py` & `openghg-1.0.0/openghg/store/base/_datasource.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,46 @@
-from pandas import DataFrame, Timestamp, Timedelta
+from pandas import DataFrame, Timestamp
+from typing import DefaultDict, Dict, List, Optional, Tuple, Union, TypeVar, Type
 from xarray import Dataset
-from collections import defaultdict
-from typing import DefaultDict, Dict, List, Optional, Tuple, Type, TypeVar, Union
-import logging
-import numpy as np
-from openghg.store.spec import define_data_types
-from openghg.types import ObjectStoreError
-
-
-logger = logging.getLogger("openghg.store.base")
-logger.setLevel(logging.DEBUG)  # Have to set level for logger as well as handler
 
 dataKeyType = DefaultDict[str, Dict[str, Dict[str, str]]]
 
 __all___ = ["Datasource"]
 
 T = TypeVar("T", bound="Datasource")
 
 
 class Datasource:
     """A Datasource holds data relating to a single source, such as a specific species
     at a certain height on a specific instrument
     """
 
     _datasource_root = "datasource"
+    _datavalues_root = "values"
     _data_root = "data"
 
     def __init__(self) -> None:
         from openghg.util import timestamp_now
+        from collections import defaultdict
         from uuid import uuid4
 
         self._uuid: str = str(uuid4())
-
         self._creation_datetime = timestamp_now()
         self._metadata: Dict[str, str] = {}
         # Dictionary keyed by daterange of data in each Dataset
         self._data: Dict[str, Dataset] = {}
 
         self._start_date = None
         self._end_date = None
 
-        self._bucket = ""
-
         self._stored = False
+        # This dictionary stored the keys for each version of data uploaded
+        # data_key = d._data_keys["latest"]["keys"][date_key]
         self._data_keys: dataKeyType = defaultdict(dict)
-        self._data_type: str = ""
+        self._data_type: str = "timeseries"
         # Hold information regarding the versions of the data
         # Currently unused
         self._latest_version: str = "latest"
         self._versions: Dict[str, List] = {}
 
     def start_date(self) -> Timestamp:
         """Returns the starting datetime for the data in this Datasource
@@ -80,202 +72,205 @@
         self._metadata[key.lower()] = value.lower()
 
     def add_data(
         self,
         metadata: Dict,
         data: Dataset,
         data_type: str,
-        skip_keys: Optional[List] = None,
         overwrite: Optional[bool] = False,
     ) -> None:
         """Add data to this Datasource and segment the data by size.
         The data is stored as a tuple of the data and the daterange it covers.
 
         Args:
             metadata: Metadata on the data for this Datasource
             data: xarray.Dataset
-            data_type: Type of data, one of ["surface", "emissions", "met", "footprints", "eulerian_model"].
+            data_type: Type of data, one of ["timeseries", "emissions", "met", "footprints", "eulerian_model"].
             overwrite: Overwrite existing data
         Returns:
             None
         """
-        expected_data_types = define_data_types()
+        expected_data_types = (
+            "timeseries",
+            "emissions",
+            "met",
+            "footprints",
+            "eulerian_model",
+        )
 
         data_type = data_type.lower()
         if data_type not in expected_data_types:
             raise TypeError(f"Incorrect data type selected. Please select from one of {expected_data_types}")
 
-        self.add_metadata(metadata=metadata, skip_keys=skip_keys)
+        self.add_metadata(metadata=metadata)
 
-        if "time" in data.coords:
-            return self.add_timed_data(data=data, data_type=data_type)
-        else:
+        if data_type == "timeseries":
+            return self.add_timeseries_data(data=data)
+        elif data_type == "footprints":
+            return self.add_footprint_data(data=data, metadata=metadata)
+        elif data_type == "emissions":
+            return self.add_emissions_data(data=data, metadata=metadata)
+        elif data_type == "met":
             raise NotImplementedError()
+        elif data_type == "eulerian_model":
+            return self.add_eulerian_model_data(data=data, metadata=metadata)
 
-    def add_timed_data(self, data: Dataset, data_type: str) -> None:
-        """Add data to this Datasource, splitting along the time axis
+    def add_timeseries_data(self, data: Dataset) -> None:
+        """Add timeseries data to this Datasource
 
         Args:
             data: An xarray.Dataset
         Returns:
             None
         """
-        from numpy import unique as np_unique
         from openghg.util import daterange_overlap
-        from xarray import concat as xr_concat
 
-        # Extract period associated with data from metadata
-        # TODO: May want to add period as a potential data variable so would need to extract from there if needed
-        period = self.get_period()
-
-        # Ensure data is in time order
-        time_coord = "time"
-        data = data.sortby(time_coord)
+        # Group by year
+        year_group = data.groupby("time.year")
+        year_data = [data for _, data in year_group if data]
 
         # Use a dictionary keyed with the daterange covered by each segment of data
-        # Group by year
-        new_data = {
-            self.get_representative_daterange_str(year_data, period=period): year_data
-            for _, year_data in data.groupby(f"{time_coord}.year")
-        }
-
-        # Ensure daterange strings are independent and do not overlap each other
-        # (this can occur due to representative date strings)
-        new_data = self._clip_daterange_label(new_data)
+        additional_data = {}
+
+        for year in year_data:
+            daterange_str = self.get_dataset_daterange_str(dataset=year)
+            additional_data[daterange_str] = year
 
         if self._data:
-            # We need to remove them from the current daterange
-            overlapping = []
-            for existing_daterange in self._data:
-                for new_daterange in new_data:
-                    if daterange_overlap(daterange_a=existing_daterange, daterange_b=new_daterange):
-                        overlapping.append((existing_daterange, new_daterange))
+            # We don't want the same data twice, this will be stored in previous versions
+            # Check for overlap between exisiting and new dateranges
+            to_keep = []
+            for current_daterange in self._data:
+                for new_daterange in additional_data:
+                    if not daterange_overlap(daterange_a=current_daterange, daterange_b=new_daterange):
+                        to_keep.append(current_daterange)
+
+            updated_data = {}
+            for k in to_keep:
+                updated_data[k] = self._data[k]
+            # Add in the additional new data
+            updated_data.update(additional_data)
 
-            # If we have overlapping data, we print a warning and then combine the datasets
-            # if we have duplicate timestamps, we first check if the data is just the same
-            # or if it's not, we keep the first value and drop the others, we also
-            # print that we've done this
-            if overlapping:
-                combined_datasets = {}
-                for existing_daterange, new_daterange in overlapping:
-                    ex = self._data.pop(existing_daterange)
-                    new = new_data.pop(new_daterange)
-
-                    logger.info("Combining overlapping data dateranges")
-                    # Concatenate datasets along time dimension
-                    try:
-                        combined = xr_concat((ex, new), dim=time_coord)
-                    except (ValueError, KeyError):
-                        # If data variables in the two datasets are not identical,
-                        # xr_concat will raise an error
-                        dv_ex = set(ex.data_vars.keys())
-                        dv_new = set(new.data_vars.keys())
-
-                        # Check difference between datasets and fill any
-                        # missing variables with NaN values.
-                        dv_not_in_new = dv_ex - dv_new
-                        for dv in dv_not_in_new:
-                            fill_values = np.zeros(len(new[time_coord])) * np.nan
-                            new = new.assign({dv: (time_coord, fill_values)})
-
-                        dv_not_in_ex = dv_new - dv_ex
-                        for dv in dv_not_in_ex:
-                            fill_values = np.zeros(len(ex[time_coord])) * np.nan
-                            ex = ex.assign({dv: (time_coord, fill_values)})
-
-                        # Should now be able to concatenate successfully
-                        combined = xr_concat((ex, new), dim=time_coord)
-
-                    combined = combined.sortby(time_coord)
-
-                    unique, index, count = np_unique(combined.time, return_counts=True, return_index=True)
-
-                    # We may have overlapping dates but not duplicate times
-                    if unique[count > 1].size > 0:
-                        logger.info("Dropping measurements at duplicate timestamps")
-                        combined = combined.isel(time=index)
-
-                    # TODO: May need to find a way to find period for *last point* rather than *current point*
-                    # combined_daterange = self.get_dataset_daterange_str(dataset=combined)
-                    combined_daterange = self.get_representative_daterange_str(
-                        dataset=combined, period=period
-                    )
-                    combined_datasets[combined_daterange] = combined
-
-                # Checking for overlapping date range strings in combined
-                # data and clipping the labels as necessary.
-                combined_datasets = self._clip_daterange_label(combined_datasets)
-
-                self._data.update(combined_datasets)
-            else:
-                self._data.update(new_data)
+            self._data = updated_data
         else:
-            self._data = new_data
+            self._data = additional_data
 
+        data_type = "timeseries"
         self._data_type = data_type
         self.add_metadata_key(key="data_type", value=data_type)
         self.update_daterange()
-        # Store the start and end date of the most recent data
-        start, end = self.daterange()
-        self.add_metadata_key(key="start_date", value=str(start))
-        self.add_metadata_key(key="end_date", value=str(end))
 
-    def delete_all_data(self) -> None:
-        """Delete the data associated with this Datasource
+    def add_metadata(self, metadata: Dict) -> None:
+        """Add all metadata in the dictionary to this Datasource
 
+        Args:
+            metadata: Dictionary of metadata
         Returns:
             None
         """
-        from openghg.objectstore import delete_object
+        from openghg.util import to_lowercase
 
-        if not self._bucket:
-            raise ObjectStoreError("No bucket set, has this Datasource been previously saved?")
+        lowercased: Dict = to_lowercase(metadata)
+        self._metadata.update(lowercased)
 
-        to_delete = []
-        for key_data in self._data_keys.values():
-            keys = list(key_data["keys"].values())
-            to_delete.extend(keys)
+    def add_emissions_data(self, data: Dataset, metadata: Dict) -> None:
+        """Add flux data to this Datasource
 
-        for key in set(to_delete):
-            delete_object(bucket=self._bucket, key=key)
+        Args:
+            data: Flux data as an xarray.Dataset
+            metadata: Metadata
+        Returns:
+            None
+        """
+        self.add_field_data(data=data, metadata=metadata, data_type="emissions")
 
-    def delete_data(self, bucket: str, keys: List) -> None:
-        """Delete specific keys
+    def add_footprint_data(self, data: Dataset, metadata: Dict) -> None:
+        """Add footprints data to this Datasource
 
         Args:
-            keys: List of keys to delete
+            data: Footprint data in an xarray.Dataset
+            metadata: Metadata
+        Returns:
+            None
         """
-        from openghg.objectstore import delete_object
+        self.add_field_data(data=data, metadata=metadata, data_type="footprints")
 
-        for key in set(keys):
-            delete_object(bucket=bucket, key=key)
+    def add_field_data(self, data: Dataset, metadata: Dict, data_type: str) -> None:
+        """Add footprints data to this Datasource
 
-    def add_metadata(self, metadata: Dict, skip_keys: Optional[List] = None) -> None:
-        """Add all metadata in the dictionary to this Datasource
+        TODO - unsure if add_field_data is the best name for this function
+        Could add a more general function that allows toggle of chunking
 
         Args:
-            metadata: Dictionary of metadata
+            data: Footprint data in an xarray.Dataset
+            metadata: Metadata
+            data_type: Type of data (footprints, flux, met)
         Returns:
             None
         """
-        from openghg.util import to_lowercase
+        from openghg.util import daterange_overlap, create_daterange_str
 
-        lowercased: Dict = to_lowercase(metadata, skip_keys=skip_keys)
-        self._metadata.update(lowercased)
+        # Use a dictionary keyed with the daterange covered by each segment of data
+        new_data = {}
+        # This daterange string covers the whole of the Dataset
+        # For the moment we're not going to chunk footprints
+
+        # As data is stored diffrently for footprint / emissions files we'll
+        # take the daterange from the metadata
+        start_date = metadata["start_date"]
+        end_date = metadata["end_date"]
+
+        daterange_str = create_daterange_str(start=start_date, end=end_date)
+
+        new_data[daterange_str] = data
+
+        if self._data:
+            # We don't want the same data twice, this will be stored in previous versions
+            # Check for overlap between exisiting and new dateranges
+            to_keep = []
+            for current_daterange in self._data:
+                for new_daterange in new_data:
+                    if not daterange_overlap(daterange_a=current_daterange, daterange_b=new_daterange):
+                        to_keep.append(current_daterange)
+
+            updated_data = {}
+            for k in to_keep:
+                updated_data[k] = self._data[k]
+            # Add in the additional new data
+            updated_data.update(new_data)
+
+            self._data = updated_data
+        else:
+            self._data = new_data
+
+        self._data_type = data_type
+        self.add_metadata_key(key="data_type", value=data_type)
+        self.update_daterange()
+
+    def add_eulerian_model_data(self, data: Dataset, metadata: Dict) -> None:
+        """Add Eulerian model data to this Datasource
+
+        Args:
+            data: Eulerian model data as an xarray.Dataset
+            metadata: Metadata
+        Returns:
+            None
+        """
+        self.add_field_data(data=data, metadata=metadata, data_type="eulerian_model")
 
     def get_dataframe_daterange(self, dataframe: DataFrame) -> Tuple[Timestamp, Timestamp]:
         """Returns the daterange for the passed DataFrame
 
         Args:
             dataframe: DataFrame to parse
         Returns:
             tuple (Timestamp, Timestamp): Start and end Timestamps for data
         """
-        from openghg.util import timestamp_tzaware
         from pandas import DatetimeIndex
+        from openghg.util import timestamp_tzaware
 
         if not isinstance(dataframe.index, DatetimeIndex):
             raise TypeError("Only DataFrames with a DatetimeIndex must be passed")
 
         # Here we want to make the pandas Timestamps timezone aware
         start = timestamp_tzaware(dataframe.first_valid_index())
         end = timestamp_tzaware(dataframe.last_valid_index())
@@ -290,16 +285,16 @@
         Returns:
             tuple (Timestamp, Timestamp): Start and end datetimes for DataSet
 
         """
         from openghg.util import timestamp_tzaware
 
         try:
-            start = timestamp_tzaware(dataset.time.min().values)
-            end = timestamp_tzaware(dataset.time.max().values)
+            start = timestamp_tzaware(dataset.time[0].values)
+            end = timestamp_tzaware(dataset.time[-1].values)
 
             return start, end
         except AttributeError:
             raise AttributeError("This dataset does not have a time attribute, unable to read date range")
 
     def get_dataset_daterange_str(self, dataset: Dataset) -> str:
         start, end = self.get_dataset_daterange(dataset=dataset)
@@ -308,156 +303,31 @@
         start = str(start).replace(" ", "-")
         end = str(end).replace(" ", "-")
 
         daterange_str: str = start + "_" + end
 
         return daterange_str
 
-    def get_representative_daterange_str(self, dataset: Dataset, period: Optional[str] = None) -> str:
-        """
-        Get representative daterange which incorporates any period the data covers.
-
-        A representative daterange covers the start - end time + any additional period that is covered
-        by each time point. The start and end times can be extracted from the input dataset and
-        any supplied period used to extend the end of the date range to cover the representative period.
-
-        If there is only one time point (i.e. start and end datetimes are the same) and no period is
-        supplied 1 additional second will be added to ensure these values are not identical.
-
-        Args:
-            dataset: Data containing (at least) a time dimension. Used to extract start and end datetimes.
-            period: Value representing a time period e.g. "12H", "1AS" "3MS". Should be suitable for
-                creation of a pandas Timedelta or DataOffset object.
-
-        Returns:
-            str : Date string covering representative date range e.g. "YYYY-MM-DD hh:mm:ss_YYYY-MM-DD hh:mm:ss"
-        """
-        from openghg.util import create_daterange_str, relative_time_offset
-        from pandas import Timedelta
-
-        # Extract start and end dates from grouped data
-        start_date, end_date = self.get_dataset_daterange(dataset)
-
-        # If period is defined add this to the end date
-        # This ensure start-end range includes time period covered by data
-        if period is not None:
-            period_td = relative_time_offset(period=period)
-            end_date = (
-                end_date + period_td - Timedelta(seconds=1)
-            )  # Subtract 1 second to make this exclusive end.
-
-        # If start and end times are identical add 1 second to ensure the range duration is > 0 seconds
-        if start_date == end_date:
-            end_date += Timedelta(seconds=1)
-
-        daterange_str = create_daterange_str(start=start_date, end=end_date)
-
-        return daterange_str
-
-    def clip_daterange(self, end_date: Timestamp, start_date_next: Timestamp) -> Timestamp:
-        """
-        Clip any end_date greater than the next start date (start_date_next) to be
-        1 second less.
-        """
-        if end_date >= start_date_next:
-            end_date = start_date_next - Timedelta(seconds=1)
-
-        return end_date
-
-    def clip_daterange_from_str(self, daterange_str1: str, daterange_str2: str) -> str:
-        """
-        Ensure the end date of a daterange string is not greater than the start
-        date of the next daterange string. Update as needed.
-        """
-        from openghg.util import create_daterange_str
-
-        start_date_str, end_date_str = daterange_str1.split("_")
-        start_date_next_str, _ = daterange_str2.split("_")
-
-        start_date = Timestamp(start_date_str)
-        end_date = Timestamp(end_date_str)
-        start_date_next = Timestamp(start_date_next_str)
-
-        end_date = self.clip_daterange(end_date, start_date_next)
-
-        daterange_str1_clipped = create_daterange_str(start_date, end_date)
-
-        return daterange_str1_clipped
-
-    def _clip_daterange_label(self, labelled_datasets: Dict[str, Dataset]) -> Dict[str, Dataset]:
-        """
-        Check the daterange string labels for the datasets and ensure neighbouring
-        date ranges are not overlapping. The daterange string labels will be updated
-        as required.
+    @staticmethod
+    def exists(datasource_id: str, bucket: Optional[str] = None) -> bool:
+        """Check if a datasource with this ID is already stored in the object store
 
         Args:
-            labelled_datasets : Dictionary of datasets labelled by date range strings.
-                These are expected to be in time order.
-
+            datasource_id (str): ID of datasource created from data
         Returns:
-            Dict : Same format as input with labels updated as necessary.
+            bool: True if Datasource exists
         """
+        from openghg.objectstore import exists, get_bucket
 
-        datestr_labels = list(labelled_datasets.keys())
-        num_data_groups = len(datestr_labels)
-
-        labelled_datasets_clipped = {}
-        for i in range(num_data_groups):
-            daterange_str_1 = datestr_labels[i]
-            if i < num_data_groups - 1:
-                daterange_str_2 = datestr_labels[i + 1]
-                daterange_str = self.clip_daterange_from_str(daterange_str_1, daterange_str_2)
-            else:
-                daterange_str = daterange_str_1
-            dataset = labelled_datasets[daterange_str_1]
-            labelled_datasets_clipped[daterange_str] = dataset
+        if bucket is None:
+            bucket = get_bucket()
 
-        return labelled_datasets_clipped
-
-    def get_period(self) -> Optional[str]:
-        """
-        Extract period value from metadata. This expects keywords of either "sampling_period" (observation data) or
-        "time_period" (derived or ancillary data). If neither keyword is found, None is returned.
+        key = f"{Datasource._datasource_root}/uuid/{datasource_id}"
 
-        This is a suitable format to use to create a pandas Timedelta or DataOffset object.
-
-        Returns:
-            str : time period in the form of number and time unit e.g. "12s"
-        """
-        # Extract period associated with data from metadata
-        # This will be the "sampling_period" for obs and "time_period" for other
-        metadata = self._metadata
-
-        time_period_attrs = ["sampling_period", "time_period"]
-        for attr in time_period_attrs:
-            value = metadata.get(attr)
-            if value is not None:
-                # For sampling period data, expect this to be in seconds
-                if attr == "sampling_period":
-                    if value.endswith("s"):  # Check if str includes "s"
-                        period: Optional[str] = value
-                    else:
-                        try:
-                            value_num: Optional[int] = int(value)
-                        except ValueError:
-                            try:
-                                value_num = int(float(value))
-                            except ValueError:
-                                value_num = None
-                                continue
-                        period = f"{value_num}s"
-                else:
-                    # Expect period data to include value and time unit
-                    period = value
-
-                break
-        else:
-            period = None
-
-        return period
+        return exists(bucket=bucket, key=key)
 
     def to_data(self) -> Dict:
         """Return a JSON-serialisable dictionary of object
         for storage in object store
 
         Storing of the data within the Datasource is done in
         the save function
@@ -488,19 +358,31 @@
 
         Args:
             bucket: Bucket containing data
             key: Key for data
         Returns:
             xarray.Dataset: Dataset from NetCDF file
         """
-        import io
         from openghg.objectstore import get_object
         from xarray import load_dataset
+        import tempfile
+        from pathlib import Path
+
+        data = get_object(bucket, key)
+
+        # TODO - is there a cleaner way of doing this?
+        with tempfile.TemporaryDirectory() as tmpdir:
+            tmp_path = Path(tmpdir).joinpath("tmp.nc")
 
-        return load_dataset(io.BytesIO(get_object(bucket=bucket, key=key)))
+            with open(tmp_path, "wb") as f:
+                f.write(data)
+
+            ds: Dataset = load_dataset(tmp_path)
+
+            return ds
 
     @classmethod
     def from_data(cls: Type[T], bucket: str, data: Dict, shallow: bool) -> T:
         """Construct a Datasource from JSON
 
         Args:
             bucket: Bucket containing data
@@ -508,49 +390,54 @@
             shallow: Load only the JSON data, do not retrieve data from the object store
         Returns:
             Datasource: Datasource created from JSON
         """
         from openghg.util import timestamp_tzaware
 
         d = cls()
-        # TODO: May want to merge these steps within the @classmethod
-        # into __init__() so this is not added twice.
         d._uuid = data["UUID"]
         d._creation_datetime = timestamp_tzaware(data["creation_datetime"])
         d._metadata = data["metadata"]
         d._stored = data["stored"]
         d._data_keys = data["data_keys"]
         d._data = {}
         d._data_type = data["data_type"]
         d._latest_version = data["latest_version"]
-        d._bucket = bucket
 
         if d._stored and not shallow:
             for date_key in d._data_keys["latest"]["keys"]:
                 data_key = d._data_keys["latest"]["keys"][date_key]
                 d._data[date_key] = Datasource.load_dataset(bucket=bucket, key=data_key)
 
         d._stored = False
 
         d.update_daterange()
 
         return d
 
-    def save(self, bucket: str) -> None:
+    def save(self, bucket: Optional[str] = None) -> None:
         """Save this Datasource object as JSON to the object store
 
         Args:
             bucket: Bucket to hold data
         Returns:
             None
         """
+        import tempfile
         from copy import deepcopy
-        from pathlib import Path
-        from openghg.objectstore import set_object_from_json
+
         from openghg.util import timestamp_now
+        from openghg.objectstore import (
+            get_bucket,
+            set_object_from_file,
+            set_object_from_json,
+        )
+
+        if bucket is None:
+            bucket = get_bucket()
 
         if self._data:
             # Ensure we have the latest key
             if "latest" not in self._data_keys:
                 self._data_keys["latest"] = {}
 
             # Backup the old data keys at "latest"
@@ -561,91 +448,88 @@
             # Iterate over the keys (daterange string) of the data dictionary
             for daterange in self._data:
                 data_key = f"{Datasource._data_root}/uuid/{self._uuid}/{version_str}/{daterange}"
 
                 new_keys[daterange] = data_key
                 data = self._data[daterange]
 
-                filepath = Path(f"{bucket}/{data_key}._data")
-                parent_folder = filepath.parent
-                if not parent_folder.exists():
-                    parent_folder.mkdir(parents=True, exist_ok=True)
-
-                data.to_netcdf(filepath, engine="netcdf4")
-
-                # Can we just take the bytes from the data here and then write then straight?
                 # TODO - for now just create a temporary directory - will have to update Acquire
                 # or work on a PR for xarray to allow returning a NetCDF as bytes
-                # with tempfile.TemporaryDirectory() as tmpdir:
-                #     filepath = f"{tmpdir}/temp.nc"
-                #     data.to_netcdf(filepath)
-                #     set_object_from_file(bucket=bucket, key=data_key, filename=filepath)
-                # path = f"{bucket_path}/data"
+                with tempfile.TemporaryDirectory() as tmpdir:
+                    filepath = f"{tmpdir}/temp.nc"
+                    data.to_netcdf(filepath)
+                    set_object_from_file(bucket=bucket, key=data_key, filename=filepath)
 
             # Copy the last version
             if "latest" in self._data_keys:
                 self._data_keys[version_str] = deepcopy(self._data_keys["latest"])
 
             # Save the new keys and create a timestamp
             self._data_keys[version_str]["keys"] = new_keys
             self._data_keys[version_str]["timestamp"] = str(timestamp_now())  # type: ignore
 
             # Link latest to the newest version
             self._data_keys["latest"] = self._data_keys[version_str]
             self._latest_version = version_str
-            self.add_metadata_key(key="latest_version", value=version_str)
 
         self._stored = True
         datasource_key = f"{Datasource._datasource_root}/uuid/{self._uuid}"
 
         set_object_from_json(bucket=bucket, key=datasource_key, data=self.to_data())
 
-    def key(self) -> str:
-        """Returns the Datasource's key
-
-        Returns:
-            str: Key for Datasource in object store
-        """
-        return f"{Datasource._datasource_root}/uuid/{self._uuid}"
-
     @classmethod
     def load(
         cls: Type[T],
-        bucket: str,
-        uuid: str,
+        bucket: str = None,
+        uuid: str = None,
+        key: str = None,
         shallow: bool = False,
     ) -> T:
         """Load a Datasource from the object store either by name or UUID
 
         Args:
             bucket: Bucket to store object
             uuid: UID of Datasource
             key: Key of Datasource
             shallow: Only load JSON data, do not read Datasets from object store.
             This will speed up creation of the Datasource object.
         Returns:
             Datasource: Datasource object created from JSON
         """
-        from openghg.objectstore import get_object_from_json
+        from openghg.objectstore import get_bucket, get_object_from_json
+
+        if uuid is None and key is None:
+            raise ValueError("Both uuid and key cannot be None")
+
+        if bucket is None:
+            bucket = get_bucket()
+
+        if key is None:
+            key = f"{Datasource._datasource_root}/uuid/{uuid}"
 
-        key = f"{Datasource._datasource_root}/uuid/{uuid}"
         data = get_object_from_json(bucket=bucket, key=key)
 
-        return cls.from_data(bucket=bucket, data=data, shallow=shallow)
+        datasource = cls.from_data(bucket=bucket, data=data, shallow=shallow)
+
+        return datasource
 
     def data(self) -> Dict:
         """Get the data stored in this Datasource
 
         Returns:
             dict: Dictionary of data keyed by daterange
         """
+        from openghg.objectstore import get_bucket
+
         if not self._data:
+            bucket = get_bucket()
+
             for date_key in self._data_keys["latest"]["keys"]:
                 data_key = self._data_keys["latest"]["keys"][date_key]
-                self._data[date_key] = Datasource.load_dataset(bucket=self._bucket, key=data_key)
+                self._data[date_key] = Datasource.load_dataset(bucket=bucket, key=data_key)
 
         return self._data
 
     def update_daterange(self) -> None:
         """Update the dates stored by this Datasource
 
         Returns:
@@ -794,23 +678,23 @@
 
         Args:
             start: Start datetime
             end: End datetime
         Returns:
             bool: True if overlap
         """
-        from openghg.util import in_daterange as _in_daterange
         from openghg.util import timestamp_tzaware
 
+        # if self._start_date is None or self._end_date is None:
+        #     self.update_daterange()
+
         start_date = timestamp_tzaware(start_date)
         end_date = timestamp_tzaware(end_date)
 
-        return _in_daterange(
-            start_a=start_date, end_a=end_date, start_b=self._start_date, end_b=self._end_date
-        )
+        return bool((start_date <= self._end_date) and (end_date >= self._start_date))
 
     def keys_in_daterange(
         self, start_date: Union[str, Timestamp], end_date: Union[str, Timestamp]
     ) -> List[str]:
         """Return the keys for data between the two passed dates
 
         Args:
@@ -970,22 +854,7 @@
     def latest_version(self) -> str:
         """Return the string of the latest version
 
         Returns:
             str: Latest version
         """
         return self._latest_version
-
-    def integrity_check(self) -> None:
-        """Checks to ensure all data stored by this Datasource exists in the object store.
-
-        Returns:
-            None
-        """
-        from openghg.objectstore import exists
-
-        for version, key_data in self._data_keys.items():
-            for key in key_data["keys"].values():
-                if not exists(bucket=self._bucket, key=key):
-                    raise ObjectStoreError(
-                        f"The key {key} for version {version} of this Datasource does not exist in the object store {self._bucket}"
-                    )
```

### Comparing `openghg-0.6.0/openghg/util/_hashing.py` & `openghg-1.0.0/openghg/util/_file.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,99 +1,84 @@
-"""
-Some functions for hashing data or strings for idendification of sources
-"""
-import hashlib
 from pathlib import Path
-from typing import Dict
+from typing import Any, Dict, List, Union, Optional, Callable
 
+__all__ = ["load_surface_parser", "get_datapath", "read_header", "load_json"]
 
-def hash_string(to_hash: str) -> str:
-    """Return the SHA-1 hash of a string
+
+def load_surface_parser(data_type: str) -> Callable:
+    """Load a parsing object of type class_name
 
     Args:
-        to_hash: String to hash
+        data_type: Name of data type such as CRDS
     Returns:
-        str: SHA1 hash of string
+        callable: class_name object
     """
-    return hashlib.sha1(str(to_hash).encode("utf-8")).hexdigest()
-
+    from importlib import import_module
 
-def hash_file(filepath: Path) -> str:
-    """Opens the file at filepath and calculates its SHA1 hash
+    module_name = "openghg.standardise.surface"
+    surface_module = import_module(name=module_name)
 
-    Taken from https://stackoverflow.com/a/22058673
-
-    Args:
-        filepath (pathlib.Path): Path to file
-    Returns:
-        str: SHA1 hash
-    """
-    # Let's read stuff in 64kB chunks
-    BUF_SIZE = 65536
-    sha1 = hashlib.sha1()
-
-    filepath = Path(filepath).expanduser().resolve()
-
-    with open(filepath, "rb") as f:
-        while True:
-            data = f.read(BUF_SIZE)
-            if not data:
-                break
-            sha1.update(data)
+    function_name = f"parse_{data_type.lower()}"
+    fn: Callable = getattr(surface_module, function_name)
 
-    return sha1.hexdigest()
+    return fn
 
 
-def hash_bytes(data: bytes) -> str:
-    """Calculate the SHA1 sum of some data
+def get_datapath(filename: str, directory: Optional[str] = None) -> Path:
+    """Returns the correct path to JSON files used for assigning attributes
 
     Args:
-        data: Binary data
+        filename (str): Name of JSON file
     Returns:
-        str: SHA1 hash
+        pathlib.Path: Path of file
     """
-    return hashlib.sha1(data).hexdigest()
+    from pathlib import Path
+
+    filename = str(filename)
 
+    if directory is None:
+        return Path(__file__).resolve().parent.parent.joinpath(f"data/{filename}")
+    else:
+        return Path(__file__).resolve().parent.parent.joinpath(f"data/{directory}/{filename}")
 
-def hash_retrieved_data(to_hash: Dict[str, Dict]) -> Dict:
-    """Hash data retrieved from a data platform. This calculates the SHA1 of the metadata
-    and the start date, end date and the number of timestamps in the Dataset.
+
+def load_json(filename: str) -> Dict:
+    """Returns a dictionary deserialised from JSON. This function only
+    works for JSON files in the openghg/data directory.
 
     Args:
-        to_hash: Dictionary to hash
-        We expected this to be a dictionary such as
-        {species_key: {"data": xr.Dataset, "metadata": {...}}}
+        filename (str): Name of JSON file
     Returns:
-        dict: Dictionary of hash: species_key
+        dict: Dictionary created from JSON
     """
-    from hashlib import sha1
-    from json import dumps
-
-    from openghg.util import timestamp_now
+    from json import load
 
-    current_timestamp = str(timestamp_now())
-    hashes: Dict[str, Dict] = {}
-    for key, data in to_hash.items():
-        metadata = data["metadata"].copy()
+    path = get_datapath(filename)
 
-        try:
-            del metadata["file_created"]
-        except KeyError:
-            pass
+    with open(path, "r") as f:
+        data: Dict[str, Any] = load(f)
 
-        metadata_hash = sha1(dumps(metadata, sort_keys=True).encode("utf8")).hexdigest()
+    return data
 
-        ds = data["data"]
 
-        start_date = str(ds.time.min())
-        end_date = str(ds.time.max())
-        n_timestamps = str(ds.time.size)
+def read_header(filepath: Union[str, Path], comment_char: str = "#") -> List:
+    """Reads the header lines denoted by the comment_char
 
-        basic_info = f"{start_date}_{end_date}_{n_timestamps}".encode("utf8")
-        time_hash = sha1(basic_info).hexdigest()
-
-        combo = (metadata_hash + time_hash).encode("utf8")
-        combo_hash = sha1(combo).hexdigest()
+    Args:
+        filepath: Path to file
+        comment_char: Character that denotes a comment line
+        at the start of a file
+    Returns:
+        list: List of lines in the header
+    """
+    comment_char = str(comment_char)
 
-        hashes[combo_hash] = {key: current_timestamp}
+    header = []
+    # Get the number of header lines
+    with open(filepath, "r") as f:
+        for line in f:
+            if line.startswith(comment_char):
+                header.append(line)
+            else:
+                break
 
-    return hashes
+    return header
```

### Comparing `openghg-0.6.0/openghg.egg-info/SOURCES.txt` & `openghg-1.0.0/openghg.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,142 +1,129 @@
 LICENSE
 MANIFEST.in
 README.md
-py.typed
 pyproject.toml
 requirements-dev.txt
 requirements-doc.txt
 requirements-server.txt
 requirements.txt
 setup.cfg
 setup.py
 versioneer.py
 openghg/__init__.py
 openghg/_version.py
 openghg/key_notes
 openghg.egg-info/PKG-INFO
 openghg.egg-info/SOURCES.txt
 openghg.egg-info/dependency_links.txt
-openghg.egg-info/entry_points.txt
 openghg.egg-info/requires.txt
 openghg.egg-info/top_level.txt
+openghg/.vscode/settings.json
 openghg/analyse/__init__.py
+openghg/analyse/_footprint.py
 openghg/analyse/_scenario.py
-openghg/cloud/__init__.py
-openghg/cloud/_call.py
-openghg/cloud/_packaging.py
-openghg/data/OpenGHG_Logo_NoText_transparent_200x200.png
+openghg/client/__init__.py
+openghg/client/_jobrunner.py
+openghg/client/_observations.py
+openghg/client/_process.py
+openghg/client/_rank_sources.py
+openghg/client/_search.py
+openghg/client/_test_service.py
+openghg/client/_user.py
+openghg/data/README
 openghg/data/acrg_obs_scale_convert.csv
+openghg/data/acrg_site_info.json
+openghg/data/acrg_species_info.json
+openghg/data/acrg_with_locations.json
 openghg/data/attributes.json
 openghg/data/beaco2n_site_data.json
 openghg/data/ceda_compliance.json
 openghg/data/colour_maps.json
 openghg/data/ecmwf_dataset_info.json
+openghg/data/icos_eurocom_sites.json
+openghg/data/lghg_data.json
+openghg/data/name_code_lookup.json
+openghg/data/noaa_data.json
+openghg/data/noaa_sites.json
 openghg/data/process_gcwerks_parameters.json
 openghg/data/process_gcwerks_parameters_bp1.json
-openghg/data/source_format_data.csv
+openghg/data/site_codes.json
+openghg/data/site_longname.json
+openghg/data/site_lookup.json
+openghg/data/species_attributes.json
+openghg/data/species_translator.json
 openghg/data/job_controllers/bc4_template.py
+openghg/data/processing/site_processing_params.json
 openghg/dataobjects/__init__.py
 openghg/dataobjects/_basedata.py
-openghg/dataobjects/_bc_data.py
-openghg/dataobjects/_datamanager.py
 openghg/dataobjects/_flux_data.py
 openghg/dataobjects/_footprint_data.py
 openghg/dataobjects/_metdata.py
-openghg/dataobjects/_obscolumn_data.py
 openghg/dataobjects/_obsdata.py
 openghg/dataobjects/_ranksources.py
 openghg/dataobjects/_searchresults.py
+openghg/jobs/__init__.py
+openghg/jobs/_create.py
+openghg/jobs/_jobdrive.py
+openghg/jobs/_run.py
+openghg/jobs/_sshconnect.py
 openghg/objectstore/__init__.py
-openghg/objectstore/_encoding.py
-openghg/objectstore/_integrity.py
+openghg/objectstore/_hugs_objstore.py.bak
 openghg/objectstore/_local_store.py
-openghg/objectstore/_oci_store.py
-openghg/objectstore/_par.py
+openghg/objectstore/_openghg_objstore.py
 openghg/plotting/__init__.py
 openghg/plotting/_footprint.py
-openghg/plotting/_timeseries.py
 openghg/retrieve/__init__.py
 openghg/retrieve/_access.py
 openghg/retrieve/_export.py
 openghg/retrieve/_search.py
-openghg/retrieve/ceda/__init__.py
-openghg/retrieve/ceda/_retrieve.py
-openghg/retrieve/icos/__init__.py
-openghg/retrieve/icos/_retrieve.py
 openghg/retrieve/met/__init__.py
 openghg/retrieve/met/_ecmwf.py
 openghg/retrieve/metadata/acrg_site_info.json
 openghg/retrieve/metadata/process_gcwerks_parameters.json
 openghg/service/__init__.py
 openghg/service/_errors.py
 openghg/service/_openghg_service.py
 openghg/standardise/__init__.py
-openghg/standardise/_standardise.py
 openghg/standardise/_summarise.py
-openghg/standardise/column/__init__.py
-openghg/standardise/column/_openghg.py
-openghg/standardise/emissions/__init__.py
-openghg/standardise/emissions/_openghg.py
 openghg/standardise/meta/__init__.py
 openghg/standardise/meta/_attributes.py
 openghg/standardise/meta/_metadata.py
 openghg/standardise/surface/__init__.py
 openghg/standardise/surface/_aqmesh.py
 openghg/standardise/surface/_beaco2n.py
 openghg/standardise/surface/_btt.py
 openghg/standardise/surface/_cranfield.py
 openghg/standardise/surface/_crds.py
 openghg/standardise/surface/_eurocom.py
 openghg/standardise/surface/_gcwerks.py
 openghg/standardise/surface/_glasgow_licor.py
 openghg/standardise/surface/_glasgow_picarro.py
-openghg/standardise/surface/_icos.py
 openghg/standardise/surface/_noaa.py
 openghg/standardise/surface/_npl.py
-openghg/standardise/surface/_openghg.py
 openghg/standardise/surface/_thamesbarrier.py
 openghg/store/__init__.py
-openghg/store/_boundary_conditions.py
-openghg/store/_data_schema.py
 openghg/store/_emissions.py
 openghg/store/_eulerian_model.py
 openghg/store/_footprints.py
-openghg/store/_infer_time.py
-openghg/store/_metadata.py
 openghg/store/_metstore.py
-openghg/store/_obscolumn.py
 openghg/store/_obsmobile.py
 openghg/store/_obssurface.py
 openghg/store/_populate.py
 openghg/store/_recombination.py
 openghg/store/_segment.py
 openghg/store/base/__init__.py
 openghg/store/base/_base.py
 openghg/store/base/_datasource.py
-openghg/store/spec/__init__.py
-openghg/store/spec/_specification.py
-openghg/transform/__init__.py
-openghg/transform/_regrid.py
-openghg/transform/emissions/__init__.py
-openghg/transform/emissions/_edgar.py
-openghg/tutorial/__init__.py
-openghg/tutorial/_tutorial.py
 openghg/types/__init__.py
 openghg/types/_enum.py
 openghg/types/_errors.py
 openghg/types/_types.py
 openghg/util/__init__.py
-openghg/util/_cli.py
-openghg/util/_domain.py
-openghg/util/_download.py
+openghg/util/_daterange.py
 openghg/util/_export.py
 openghg/util/_file.py
 openghg/util/_hashing.py
-openghg/util/_inlet.py
-openghg/util/_site.py
-openghg/util/_species.py
 openghg/util/_strings.py
 openghg/util/_time.py
-openghg/util/_user.py
-openghg/util/_util.py
-openghg/util/_versions.py
+openghg/util/_tutorial.py
+openghg/util/_util.py
```

### Comparing `openghg-0.6.0/setup.cfg` & `openghg-1.0.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -23,28 +23,25 @@
 	Operating System :: POSIX :: Linux
 	Programming Language :: C
 	Programming Language :: Cython
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 
-[isort]
-profile = hug
-src_paths = isort,test
-
 [flake8]
 ignore = E203, W503, E501, W291, E127, E128
+exclude = openghg/interface/
 max-line-length = 110
 per-file-ignores = 
 	*/__init__.py: F401, E402
+	openghg/interface/__init__.py: F401, F403
+	openghg/processing/__init__.py: F401, F403
 
 [options.packages.find]
 where = openghg
 
 [versioneer]
 VCS = git
 style = pep440
```

### Comparing `openghg-0.6.0/setup.py` & `openghg-1.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,37 @@
-# type: ignore
-import sys
-
 import setuptools
+import sys
 
 sys.path.insert(0, ".")  # noqa
-import versioneer  # noqa
+import versioneer
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 files = ["openghg/*"]
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
-    version=versioneer.get_version(),
+    version="1.0.0",
     install_requires=requirements,
     name="openghg",
     author="Gareth Jones",
     author_email="g.m.jones@bristol.ac.uk",
     description="OpenGHG - a cloud platform for greenhouse gas data analysis",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/openghg/openghg",
     packages=setuptools.find_packages(include=["openghg", "openghg.*"]),
-    package_data={"": ["data/*", "py.typed"]},
+    package_data={"": ["data/*"]},
     classifiers=[
+        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS",
     ],
-    entry_points={
-        "console_scripts": [
-            "openghg = openghg.util:cli",
-        ]
-    },
-    python_requires=">=3.8",
+    python_requires=">=3.7",
 )
```

### Comparing `openghg-0.6.0/versioneer.py` & `openghg-1.0.0/versioneer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,64 +1,36 @@
-# type: ignore
-# Version: 0.28
+
+# Version: 0.21
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
 * like a rocketeer, but for versions!
 * https://github.com/python-versioneer/python-versioneer
 * Brian Warner
-* License: Public Domain (Unlicense)
-* Compatible with: Python 3.7, 3.8, 3.9, 3.10 and pypy3
+* License: Public Domain
+* Compatible with: Python 3.6, 3.7, 3.8, 3.9 and pypy3
 * [![Latest Version][pypi-image]][pypi-url]
 * [![Build Status][travis-image]][travis-url]
 
-This is a tool for managing a recorded version number in setuptools-based
+This is a tool for managing a recorded version number in distutils-based
 python projects. The goal is to remove the tedious and error-prone "update
 the embedded version string" step from your release process. Making a new
 release should be as easy as recording a new tag in your version-control
 system, and maybe making new tarballs.
 
 
 ## Quick Install
 
-Versioneer provides two installation modes. The "classic" vendored mode installs
-a copy of versioneer into your repository. The experimental build-time dependency mode
-is intended to allow you to skip this step and simplify the process of upgrading.
-
-### Vendored mode
-
-* `pip install versioneer` to somewhere in your $PATH
-   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
-     available, so you can also use `conda install -c conda-forge versioneer`
-* add a `[tool.versioneer]` section to your `pyproject.toml` or a
-  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
-   * Note that you will need to add `tomli; python_version < "3.11"` to your
-     build-time dependencies if you use `pyproject.toml`
-* run `versioneer install --vendor` in your source tree, commit the results
-* verify version information with `python setup.py version`
-
-### Build-time dependency mode
-
 * `pip install versioneer` to somewhere in your $PATH
-   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
-     available, so you can also use `conda install -c conda-forge versioneer`
-* add a `[tool.versioneer]` section to your `pyproject.toml` or a
-  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
-* add `versioneer` (with `[toml]` extra, if configuring in `pyproject.toml`)
-  to the `requires` key of the `build-system` table in `pyproject.toml`:
-  ```toml
-  [build-system]
-  requires = ["setuptools", "versioneer[toml]"]
-  build-backend = "setuptools.build_meta"
-  ```
-* run `versioneer install --no-vendor` in your source tree, commit the results
-* verify version information with `python setup.py version`
+* add a `[versioneer]` section to your setup.cfg (see [Install](INSTALL.md))
+* run `versioneer install` in your source tree, commit the results
+* Verify version information with `python setup.py version`
 
 ## Version Identifiers
 
 Source trees come from a variety of places:
 
 * a version-control system checkout (mostly used by developers)
 * a nightly tarball, produced by build automation
@@ -255,18 +227,17 @@
 
 
 ## Updating Versioneer
 
 To upgrade your project to a new release of Versioneer, do the following:
 
 * install the new Versioneer (`pip install -U versioneer` or equivalent)
-* edit `setup.cfg` and `pyproject.toml`, if necessary,
-  to include any new configuration settings indicated by the release notes.
-  See [UPGRADING](./UPGRADING.md) for details.
-* re-run `versioneer install --[no-]vendor` in your source tree, to replace
+* edit `setup.cfg`, if necessary, to include any new configuration settings
+  indicated by the release notes. See [UPGRADING](./UPGRADING.md) for details.
+* re-run `versioneer install` in your source tree, to replace
   `SRC/_version.py`
 * commit any changed files
 
 ## Future Directions
 
 This tool is designed to make it easily extended to other version-control
 systems: all VCS-specific components are in separate directories like
@@ -288,16 +259,17 @@
 * [versioningit](https://github.com/jwodder/versioningit) - a PEP 518-based setuptools
   plugin
 
 ## License
 
 To make Versioneer easier to embed, all its code is dedicated to the public
 domain. The `_version.py` that it creates is also in the public domain.
-Specifically, both are released under the "Unlicense", as described in
-https://unlicense.org/.
+Specifically, both are released under the Creative Commons "Public Domain
+Dedication" license (CC0-1.0), as described in
+https://creativecommons.org/publicdomain/zero/1.0/ .
 
 [pypi-image]: https://img.shields.io/pypi/v/versioneer.svg
 [pypi-url]: https://pypi.python.org/pypi/versioneer/
 [travis-image]:
 https://img.shields.io/travis/com/python-versioneer/python-versioneer.svg
 [travis-url]: https://travis-ci.com/github/python-versioneer/python-versioneer
 
@@ -311,26 +283,15 @@
 import configparser
 import errno
 import json
 import os
 import re
 import subprocess
 import sys
-from pathlib import Path
 from typing import Callable, Dict
-import functools
-
-have_tomllib = True
-if sys.version_info >= (3, 11):
-    import tomllib
-else:
-    try:
-        import tomli as tomllib
-    except ImportError:
-        have_tomllib = False
 
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
 
 def get_root():
@@ -344,74 +305,60 @@
     versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
         setup_py = os.path.join(root, "setup.py")
         versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
-        err = (
-            "Versioneer was unable to run the project root directory. "
-            "Versioneer requires setup.py to be executed from "
-            "its immediate directory (like 'python setup.py COMMAND'), "
-            "or in a way that lets it use sys.argv[0] to find the root "
-            "(like 'python path/to/setup.py COMMAND')."
-        )
+        err = ("Versioneer was unable to run the project root directory. "
+               "Versioneer requires setup.py to be executed from "
+               "its immediate directory (like 'python setup.py COMMAND'), "
+               "or in a way that lets it use sys.argv[0] to find the root "
+               "(like 'python path/to/setup.py COMMAND').")
         raise VersioneerBadRootError(err)
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
         my_path = os.path.realpath(os.path.abspath(__file__))
         me_dir = os.path.normcase(os.path.splitext(my_path)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
-        if me_dir != vsr_dir and "VERSIONEER_PEP518" not in globals():
-            print(
-                "Warning: build in %s is using versioneer.py from %s"
-                % (os.path.dirname(my_path), versioneer_py)
-            )
+        if me_dir != vsr_dir:
+            print("Warning: build in %s is using versioneer.py from %s"
+                  % (os.path.dirname(my_path), versioneer_py))
     except NameError:
         pass
     return root
 
 
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
     # This might raise OSError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
-    root = Path(root)
-    pyproject_toml = root / "pyproject.toml"
-    setup_cfg = root / "setup.cfg"
-    section = None
-    if pyproject_toml.exists() and have_tomllib:
-        try:
-            with open(pyproject_toml, "rb") as fobj:
-                pp = tomllib.load(fobj)
-            section = pp["tool"]["versioneer"]
-        except (tomllib.TOMLDecodeError, KeyError):
-            pass
-    if not section:
-        parser = configparser.ConfigParser()
-        with open(setup_cfg) as cfg_file:
-            parser.read_file(cfg_file)
-        parser.get("versioneer", "VCS")  # raise error if missing
+    setup_cfg = os.path.join(root, "setup.cfg")
+    parser = configparser.ConfigParser()
+    with open(setup_cfg, "r") as cfg_file:
+        parser.read_file(cfg_file)
+    VCS = parser.get("versioneer", "VCS")  # mandatory
 
-        section = parser["versioneer"]
+    # Dict-like interface for non-mandatory entries
+    section = parser["versioneer"]
 
     cfg = VersioneerConfig()
-    cfg.VCS = section["VCS"]
+    cfg.VCS = VCS
     cfg.style = section.get("style", "")
     cfg.versionfile_source = section.get("versionfile_source")
     cfg.versionfile_build = section.get("versionfile_build")
     cfg.tag_prefix = section.get("tag_prefix")
-    if cfg.tag_prefix in ("''", '""', None):
+    if cfg.tag_prefix in ("''", '""'):
         cfg.tag_prefix = ""
     cfg.parentdir_prefix = section.get("parentdir_prefix")
     cfg.verbose = section.get("verbose")
     return cfg
 
 
 class NotThisMethod(Exception):
@@ -421,47 +368,34 @@
 # these dictionaries contain VCS-specific tools
 LONG_VERSION_PY: Dict[str, str] = {}
 HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
     """Create decorator to mark a method as the handler of a VCS."""
-
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
         HANDLERS.setdefault(vcs, {})[method] = f
         return f
-
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False, env=None):
+def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
+                env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
     process = None
-
-    popen_kwargs = {}
-    if sys.platform == "win32":
-        # This hides the console window if pythonw.exe is used
-        startupinfo = subprocess.STARTUPINFO()
-        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
-        popen_kwargs["startupinfo"] = startupinfo
-
     for command in commands:
         try:
             dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            process = subprocess.Popen(
-                [command] + args,
-                cwd=cwd,
-                env=env,
-                stdout=subprocess.PIPE,
-                stderr=(subprocess.PIPE if hide_stderr else None),
-                **popen_kwargs,
-            )
+            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
+                                       stdout=subprocess.PIPE,
+                                       stderr=(subprocess.PIPE if hide_stderr
+                                               else None))
             break
         except OSError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
@@ -476,36 +410,32 @@
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
         return None, process.returncode
     return stdout, process.returncode
 
 
-LONG_VERSION_PY[
-    "git"
-] = r'''
+LONG_VERSION_PY['git'] = r'''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
-# This file is released into the public domain.
-# Generated by versioneer-0.28
-# https://github.com/python-versioneer/python-versioneer
+# This file is released into the public domain. Generated by
+# versioneer-0.21 (https://github.com/python-versioneer/python-versioneer)
 
 """Git implementation of _version.py."""
 
 import errno
 import os
 import re
 import subprocess
 import sys
 from typing import Callable, Dict
-import functools
 
 
 def get_keywords():
     """Get the keywords needed to look up the version information."""
     # these strings will be replaced by git during git-archive.
     # setup.py/versioneer.py will grep for the variable names, so they must
     # each be defined on a line of their own. _version.py will just call
@@ -555,30 +485,22 @@
 
 
 def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
                 env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
     process = None
-
-    popen_kwargs = {}
-    if sys.platform == "win32":
-        # This hides the console window if pythonw.exe is used
-        startupinfo = subprocess.STARTUPINFO()
-        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
-        popen_kwargs["startupinfo"] = startupinfo
-
     for command in commands:
         try:
             dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
             process = subprocess.Popen([command] + args, cwd=cwd, env=env,
                                        stdout=subprocess.PIPE,
                                        stderr=(subprocess.PIPE if hide_stderr
-                                               else None), **popen_kwargs)
+                                               else None))
             break
         except OSError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %%s" %% dispcmd)
@@ -718,37 +640,33 @@
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
+    TAG_PREFIX_REGEX = "*"
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
-
-    # GIT_DIR can interfere with correct operation of Versioneer.
-    # It may be intended to be passed to the Versioneer-versioned project,
-    # but that should not change where we get our version from.
-    env = os.environ.copy()
-    env.pop("GIT_DIR", None)
-    runner = functools.partial(runner, env=env)
+        TAG_PREFIX_REGEX = r"\*"
 
     _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                   hide_stderr=not verbose)
+                   hide_stderr=True)
     if rc != 0:
         if verbose:
             print("Directory %%s not under git control" %% root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = runner(GITS, [
-        "describe", "--tags", "--dirty", "--always", "--long",
-        "--match", f"{tag_prefix}[[:digit:]]*"
-    ], cwd=root)
+    describe_out, rc = runner(GITS, ["describe", "--tags", "--dirty",
+                                     "--always", "--long",
+                                     "--match",
+                                     "%%s%%s" %% (tag_prefix, TAG_PREFIX_REGEX)],
+                              cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
@@ -829,16 +747,16 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
-        pieces["distance"] = len(out.split())  # total number of commits
+        count_out, rc = runner(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
+        pieces["distance"] = int(count_out)  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
     date = runner(GITS, ["show", "-s", "--format=%%ci", "HEAD"], cwd=root)[0].strip()
     # Use only the last line.  Previous lines may contain GPG signature
     # information.
     date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
@@ -926,15 +844,15 @@
     """
     if pieces["closest-tag"]:
         if pieces["distance"]:
             # update the post release segment
             tag_version, post_version = pep440_split_post(pieces["closest-tag"])
             rendered = tag_version
             if post_version is not None:
-                rendered += ".post%%d.dev%%d" %% (post_version + 1, pieces["distance"])
+                rendered += ".post%%d.dev%%d" %% (post_version+1, pieces["distance"])
             else:
                 rendered += ".post0.dev%%d" %% (pieces["distance"])
         else:
             # no commits, use the tag as the version
             rendered = pieces["closest-tag"]
     else:
         # exception #1
@@ -1194,105 +1112,95 @@
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
     refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = {r[len(TAG) :] for r in refs if r.startswith(TAG)}
+    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = {r for r in refs if re.search(r"\d", r)}
+        tags = {r for r in refs if re.search(r'\d', r)}
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
-            r = ref[len(tag_prefix) :]
+            r = ref[len(tag_prefix):]
             # Filter out refs that exactly match prefix or that don't start
             # with a number once the prefix is stripped (mostly a concern
             # when prefix is '')
-            if not re.match(r"\d", r):
+            if not re.match(r'\d', r):
                 continue
             if verbose:
                 print("picking %s" % r)
-            return {
-                "version": r,
-                "full-revisionid": keywords["full"].strip(),
-                "dirty": False,
-                "error": None,
-                "date": date,
-            }
+            return {"version": r,
+                    "full-revisionid": keywords["full"].strip(),
+                    "dirty": False, "error": None,
+                    "date": date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
     if verbose:
         print("no suitable tags, using unknown + full revision id")
-    return {
-        "version": "0+unknown",
-        "full-revisionid": keywords["full"].strip(),
-        "dirty": False,
-        "error": "no suitable tags",
-        "date": None,
-    }
+    return {"version": "0+unknown",
+            "full-revisionid": keywords["full"].strip(),
+            "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
 def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
+    TAG_PREFIX_REGEX = "*"
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
+        TAG_PREFIX_REGEX = r"\*"
 
-    # GIT_DIR can interfere with correct operation of Versioneer.
-    # It may be intended to be passed to the Versioneer-versioned project,
-    # but that should not change where we get our version from.
-    env = os.environ.copy()
-    env.pop("GIT_DIR", None)
-    runner = functools.partial(runner, env=env)
-
-    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=not verbose)
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                   hide_stderr=True)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = runner(
-        GITS,
-        ["describe", "--tags", "--dirty", "--always", "--long", "--match", f"{tag_prefix}[[:digit:]]*"],
-        cwd=root,
-    )
+    describe_out, rc = runner(GITS, ["describe", "--tags", "--dirty",
+                                     "--always", "--long",
+                                     "--match",
+                                     "%s%s" % (tag_prefix, TAG_PREFIX_REGEX)],
+                              cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
     pieces = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
-    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"], cwd=root)
+    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
+                             cwd=root)
     # --abbrev-ref was added in git-1.6.3
     if rc != 0 or branch_name is None:
         raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
     branch_name = branch_name.strip()
 
     if branch_name == "HEAD":
         # If we aren't exactly on a branch, pick a branch which represents
@@ -1324,79 +1232,80 @@
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
     if dirty:
-        git_describe = git_describe[: git_describe.rindex("-dirty")]
+        git_describe = git_describe[:git_describe.rindex("-dirty")]
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
-        mo = re.search(r"^(.+)-(\d+)-g([0-9a-f]+)$", git_describe)
+        mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
             # unparsable. Maybe git-describe is misbehaving?
-            pieces["error"] = "unable to parse git-describe output: '%s'" % describe_out
+            pieces["error"] = ("unable to parse git-describe output: '%s'"
+                               % describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
             if verbose:
                 fmt = "tag '%s' doesn't start with prefix '%s'"
                 print(fmt % (full_tag, tag_prefix))
-            pieces["error"] = "tag '%s' doesn't start with prefix '%s'" % (full_tag, tag_prefix)
+            pieces["error"] = ("tag '%s' doesn't start with prefix '%s'"
+                               % (full_tag, tag_prefix))
             return pieces
-        pieces["closest-tag"] = full_tag[len(tag_prefix) :]
+        pieces["closest-tag"] = full_tag[len(tag_prefix):]
 
         # distance: number of commits since tag
         pieces["distance"] = int(mo.group(2))
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
-        pieces["distance"] = len(out.split())  # total number of commits
+        count_out, rc = runner(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
+        pieces["distance"] = int(count_out)  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
     date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
     # Use only the last line.  Previous lines may contain GPG signature
     # information.
     date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def do_vcs_install(versionfile_source, ipy):
+def do_vcs_install(manifest_in, versionfile_source, ipy):
     """Git-specific installation logic for Versioneer.
 
     For Git, this means creating/changing .gitattributes to mark _version.py
     for export-subst keyword substitution.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
-    files = [versionfile_source]
+    files = [manifest_in, versionfile_source]
     if ipy:
         files.append(ipy)
-    if "VERSIONEER_PEP518" not in globals():
-        try:
-            my_path = __file__
-            if my_path.endswith((".pyc", ".pyo")):
-                my_path = os.path.splitext(my_path)[0] + ".py"
-            versioneer_file = os.path.relpath(my_path)
-        except NameError:
-            versioneer_file = "versioneer.py"
-        files.append(versioneer_file)
+    try:
+        my_path = __file__
+        if my_path.endswith(".pyc") or my_path.endswith(".pyo"):
+            my_path = os.path.splitext(my_path)[0] + ".py"
+        versioneer_file = os.path.relpath(my_path)
+    except NameError:
+        versioneer_file = "versioneer.py"
+    files.append(versioneer_file)
     present = False
     try:
         with open(".gitattributes", "r") as fobj:
             for line in fobj:
                 if line.strip().startswith(versionfile_source):
                     if "export-subst" in line.strip().split()[1:]:
                         present = True
@@ -1418,31 +1327,28 @@
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
     for _ in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
-            return {
-                "version": dirname[len(parentdir_prefix) :],
-                "full-revisionid": None,
-                "dirty": False,
-                "error": None,
-                "date": None,
-            }
+            return {"version": dirname[len(parentdir_prefix):],
+                    "full-revisionid": None,
+                    "dirty": False, "error": None, "date": None}
         rootdirs.append(root)
         root = os.path.dirname(root)  # up a level
 
     if verbose:
-        print("Tried directories %s but none started with prefix %s" % (str(rootdirs), parentdir_prefix))
+        print("Tried directories %s but none started with prefix %s" %
+              (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
-# This file was generated by 'versioneer.py' (0.28) from
+# This file was generated by 'versioneer.py' (0.21) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
@@ -1458,26 +1364,29 @@
 def versions_from_file(filename):
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
     except OSError:
         raise NotThisMethod("unable to read _version.py")
-    mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S)
+    mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
+                   contents, re.M | re.S)
     if not mo:
-        mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S)
+        mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
+                       contents, re.M | re.S)
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
 def write_to_version_file(filename, versions):
     """Write the given version number to the given _version.py file."""
     os.unlink(filename)
-    contents = json.dumps(versions, sort_keys=True, indent=1, separators=(",", ": "))
+    contents = json.dumps(versions, sort_keys=True,
+                          indent=1, separators=(",", ": "))
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
     print("set %s to '%s'" % (filename, versions["version"]))
 
 
 def plus_or_dot(pieces):
@@ -1501,15 +1410,16 @@
         if pieces["distance"] or pieces["dirty"]:
             rendered += plus_or_dot(pieces)
             rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
-        rendered = "0+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
+        rendered = "0+untagged.%d.g%s" % (pieces["distance"],
+                                          pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def render_pep440_branch(pieces):
     """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
@@ -1530,15 +1440,16 @@
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
         rendered = "0"
         if pieces["branch"] != "master":
             rendered += ".dev0"
-        rendered += "+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
+        rendered += "+untagged.%d.g%s" % (pieces["distance"],
+                                          pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def pep440_split_post(ver):
     """Split pep440 version string at the post-release segment.
@@ -1558,15 +1469,15 @@
     """
     if pieces["closest-tag"]:
         if pieces["distance"]:
             # update the post release segment
             tag_version, post_version = pep440_split_post(pieces["closest-tag"])
             rendered = tag_version
             if post_version is not None:
-                rendered += ".post%d.dev%d" % (post_version + 1, pieces["distance"])
+                rendered += ".post%d.dev%d" % (post_version+1, pieces["distance"])
             else:
                 rendered += ".post0.dev%d" % (pieces["distance"])
         else:
             # no commits, use the tag as the version
             rendered = pieces["closest-tag"]
     else:
         # exception #1
@@ -1691,21 +1602,19 @@
         rendered += "-dirty"
     return rendered
 
 
 def render(pieces, style):
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
-        return {
-            "version": "unknown",
-            "full-revisionid": pieces.get("long"),
-            "dirty": None,
-            "error": pieces["error"],
-            "date": None,
-        }
+        return {"version": "unknown",
+                "full-revisionid": pieces.get("long"),
+                "dirty": None,
+                "error": pieces["error"],
+                "date": None}
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
     elif style == "pep440-branch":
@@ -1721,21 +1630,17 @@
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%s'" % style)
 
-    return {
-        "version": rendered,
-        "full-revisionid": pieces["long"],
-        "dirty": pieces["dirty"],
-        "error": None,
-        "date": pieces.get("date"),
-    }
+    return {"version": rendered, "full-revisionid": pieces["long"],
+            "dirty": pieces["dirty"], "error": None,
+            "date": pieces.get("date")}
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
 def get_versions(verbose=False):
@@ -1750,15 +1655,16 @@
     root = get_root()
     cfg = get_config_from_root(root)
 
     assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
     verbose = verbose or cfg.verbose
-    assert cfg.versionfile_source is not None, "please set versioneer.versionfile_source"
+    assert cfg.versionfile_source is not None, \
+        "please set versioneer.versionfile_source"
     assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
     # extract version from first of: _version.py, VCS command (e.g. 'git
     # describe'), parentdir. This is meant to work for developers using a
     # source checkout, for users of a tarball created by 'setup.py sdist',
@@ -1804,30 +1710,26 @@
             return ver
     except NotThisMethod:
         pass
 
     if verbose:
         print("unable to compute version")
 
-    return {
-        "version": "0+unknown",
-        "full-revisionid": None,
-        "dirty": None,
-        "error": "unable to compute version",
-        "date": None,
-    }
+    return {"version": "0+unknown", "full-revisionid": None,
+            "dirty": None, "error": "unable to compute version",
+            "date": None}
 
 
 def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
 def get_cmdclass(cmdclass=None):
-    """Get the custom setuptools subclasses used by Versioneer.
+    """Get the custom setuptools/distutils subclasses used by Versioneer.
 
     If the package uses a different cmdclass (e.g. one from numpy), it
     should be provide as an argument.
     """
     if "versioneer" in sys.modules:
         del sys.modules["versioneer"]
         # this fixes the "python setup.py develop" case (also 'install' and
@@ -1841,16 +1743,16 @@
         # parent is protected against the child's "import versioneer". By
         # removing ourselves from sys.modules here, before the child build
         # happens, we protect the child from the parent's versioneer too.
         # Also see https://github.com/python-versioneer/python-versioneer/issues/52
 
     cmds = {} if cmdclass is None else cmdclass.copy()
 
-    # we add "version" to setuptools
-    from setuptools import Command
+    # we add "version" to both distutils and setuptools
+    from distutils.core import Command
 
     class cmd_version(Command):
         description = "report generated version string"
         user_options = []
         boolean_options = []
 
         def initialize_options(self):
@@ -1863,64 +1765,60 @@
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
-
     cmds["version"] = cmd_version
 
-    # we override "build_py" in setuptools
+    # we override "build_py" in both distutils and setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
     #  setuptools/bdist_wheel -> distutils/install ->..
     #  setuptools/bdist_egg -> distutils/install_lib -> build_py
     #  setuptools/install -> bdist_egg ->..
     #  setuptools/develop -> ?
     #  pip install:
     #   copies source tree to a tempdir before running egg_info/etc
     #   if .git isn't copied too, 'git describe' will fail
     #   then does setup.py bdist_wheel, or sometimes setup.py install
     #  setup.py egg_info -> ?
 
-    # pip install -e . and setuptool/editable_wheel will invoke build_py
-    # but the build_py command is not expected to copy any files.
-
     # we override different "build_py" commands for both environments
-    if "build_py" in cmds:
-        _build_py = cmds["build_py"]
-    else:
+    if 'build_py' in cmds:
+        _build_py = cmds['build_py']
+    elif "setuptools" in sys.modules:
         from setuptools.command.build_py import build_py as _build_py
+    else:
+        from distutils.command.build_py import build_py as _build_py
 
     class cmd_build_py(_build_py):
         def run(self):
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
-            if getattr(self, "editable_mode", False):
-                # During editable installs `.py` and data files are
-                # not copied to build_lib
-                return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
-                target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
+                target_versionfile = os.path.join(self.build_lib,
+                                                  cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
-
     cmds["build_py"] = cmd_build_py
 
-    if "build_ext" in cmds:
-        _build_ext = cmds["build_ext"]
-    else:
+    if 'build_ext' in cmds:
+        _build_ext = cmds['build_ext']
+    elif "setuptools" in sys.modules:
         from setuptools.command.build_ext import build_ext as _build_ext
+    else:
+        from distutils.command.build_ext import build_ext as _build_ext
 
     class cmd_build_ext(_build_ext):
         def run(self):
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_ext.run(self)
@@ -1928,32 +1826,22 @@
                 # build_ext --inplace will only build extensions in
                 # build/lib<..> dir with no _version.py to write to.
                 # As in place builds will already have a _version.py
                 # in the module dir, we do not need to write one.
                 return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
-            if not cfg.versionfile_build:
-                return
-            target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
-            if not os.path.exists(target_versionfile):
-                print(
-                    f"Warning: {target_versionfile} does not exist, skipping "
-                    "version update. This can happen if you are running build_ext "
-                    "without first running build_py."
-                )
-                return
+            target_versionfile = os.path.join(self.build_lib,
+                                              cfg.versionfile_build)
             print("UPDATING %s" % target_versionfile)
             write_to_version_file(target_versionfile, versions)
-
     cmds["build_ext"] = cmd_build_ext
 
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
         from cx_Freeze.dist import build_exe as _build_exe
-
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
 
@@ -1966,102 +1854,56 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _build_exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(
-                        LONG
-                        % {
-                            "DOLLAR": "$",
-                            "STYLE": cfg.style,
-                            "TAG_PREFIX": cfg.tag_prefix,
-                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                        }
-                    )
-
+                    f.write(LONG %
+                            {"DOLLAR": "$",
+                             "STYLE": cfg.style,
+                             "TAG_PREFIX": cfg.tag_prefix,
+                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                             })
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
-    if "py2exe" in sys.modules:  # py2exe enabled?
-        try:
-            from py2exe.setuptools_buildexe import py2exe as _py2exe
-        except ImportError:
-            from py2exe.distutils_buildexe import py2exe as _py2exe
+    if 'py2exe' in sys.modules:  # py2exe enabled?
+        from py2exe.distutils_buildexe import py2exe as _py2exe
 
         class cmd_py2exe(_py2exe):
             def run(self):
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _py2exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(
-                        LONG
-                        % {
-                            "DOLLAR": "$",
-                            "STYLE": cfg.style,
-                            "TAG_PREFIX": cfg.tag_prefix,
-                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                        }
-                    )
-
+                    f.write(LONG %
+                            {"DOLLAR": "$",
+                             "STYLE": cfg.style,
+                             "TAG_PREFIX": cfg.tag_prefix,
+                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                             })
         cmds["py2exe"] = cmd_py2exe
 
-    # sdist farms its file list building out to egg_info
-    if "egg_info" in cmds:
-        _egg_info = cmds["egg_info"]
-    else:
-        from setuptools.command.egg_info import egg_info as _egg_info
-
-    class cmd_egg_info(_egg_info):
-        def find_sources(self):
-            # egg_info.find_sources builds the manifest list and writes it
-            # in one shot
-            super().find_sources()
-
-            # Modify the filelist and normalize it
-            root = get_root()
-            cfg = get_config_from_root(root)
-            self.filelist.append("versioneer.py")
-            if cfg.versionfile_source:
-                # There are rare cases where versionfile_source might not be
-                # included by default, so we must be explicit
-                self.filelist.append(cfg.versionfile_source)
-            self.filelist.sort()
-            self.filelist.remove_duplicates()
-
-            # The write method is hidden in the manifest_maker instance that
-            # generated the filelist and was thrown away
-            # We will instead replicate their final normalization (to unicode,
-            # and POSIX-style paths)
-            from setuptools import unicode_utils
-
-            normalized = [unicode_utils.filesys_decode(f).replace(os.sep, "/") for f in self.filelist.files]
-
-            manifest_filename = os.path.join(self.egg_info, "SOURCES.txt")
-            with open(manifest_filename, "w") as fobj:
-                fobj.write("\n".join(normalized))
-
-    cmds["egg_info"] = cmd_egg_info
-
     # we override different "sdist" commands for both environments
-    if "sdist" in cmds:
-        _sdist = cmds["sdist"]
-    else:
+    if 'sdist' in cmds:
+        _sdist = cmds['sdist']
+    elif "setuptools" in sys.modules:
         from setuptools.command.sdist import sdist as _sdist
+    else:
+        from distutils.command.sdist import sdist as _sdist
 
     class cmd_sdist(_sdist):
         def run(self):
             versions = get_versions()
             self._versioneer_generated_versions = versions
             # unless we update this, the command will keep using the old
             # version
@@ -2073,16 +1915,16 @@
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
             print("UPDATING %s" % target_versionfile)
-            write_to_version_file(target_versionfile, self._versioneer_generated_versions)
-
+            write_to_version_file(target_versionfile,
+                                  self._versioneer_generated_versions)
     cmds["sdist"] = cmd_sdist
 
     return cmds
 
 
 CONFIG_ERROR = """
 setup.cfg is missing the necessary Versioneer configuration. You need
@@ -2134,37 +1976,36 @@
 
 
 def do_setup():
     """Do main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (OSError, configparser.NoSectionError, configparser.NoOptionError) as e:
+    except (OSError, configparser.NoSectionError,
+            configparser.NoOptionError) as e:
         if isinstance(e, (OSError, configparser.NoSectionError)):
-            print("Adding sample versioneer config to setup.cfg", file=sys.stderr)
+            print("Adding sample versioneer config to setup.cfg",
+                  file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
     print(" creating %s" % cfg.versionfile_source)
     with open(cfg.versionfile_source, "w") as f:
         LONG = LONG_VERSION_PY[cfg.VCS]
-        f.write(
-            LONG
-            % {
-                "DOLLAR": "$",
-                "STYLE": cfg.style,
-                "TAG_PREFIX": cfg.tag_prefix,
-                "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                "VERSIONFILE_SOURCE": cfg.versionfile_source,
-            }
-        )
+        f.write(LONG % {"DOLLAR": "$",
+                        "STYLE": cfg.style,
+                        "TAG_PREFIX": cfg.tag_prefix,
+                        "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                        "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        })
 
-    ipy = os.path.join(os.path.dirname(cfg.versionfile_source), "__init__.py")
+    ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
+                       "__init__.py")
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
         except OSError:
             old = ""
         module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
@@ -2179,18 +2020,50 @@
                 f.write(snippet)
         else:
             print(" %s unmodified" % ipy)
     else:
         print(" %s doesn't exist, ok" % ipy)
         ipy = None
 
+    # Make sure both the top-level "versioneer.py" and versionfile_source
+    # (PKG/_version.py, used by runtime code) are in MANIFEST.in, so
+    # they'll be copied into source distributions. Pip won't be able to
+    # install the package without this.
+    manifest_in = os.path.join(root, "MANIFEST.in")
+    simple_includes = set()
+    try:
+        with open(manifest_in, "r") as f:
+            for line in f:
+                if line.startswith("include "):
+                    for include in line.split()[1:]:
+                        simple_includes.add(include)
+    except OSError:
+        pass
+    # That doesn't cover everything MANIFEST.in can do
+    # (http://docs.python.org/2/distutils/sourcedist.html#commands), so
+    # it might give some false negatives. Appending redundant 'include'
+    # lines is safe, though.
+    if "versioneer.py" not in simple_includes:
+        print(" appending 'versioneer.py' to MANIFEST.in")
+        with open(manifest_in, "a") as f:
+            f.write("include versioneer.py\n")
+    else:
+        print(" 'versioneer.py' already in MANIFEST.in")
+    if cfg.versionfile_source not in simple_includes:
+        print(" appending versionfile_source ('%s') to MANIFEST.in" %
+              cfg.versionfile_source)
+        with open(manifest_in, "a") as f:
+            f.write("include %s\n" % cfg.versionfile_source)
+    else:
+        print(" versionfile_source already in MANIFEST.in")
+
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
     # substitution.
-    do_vcs_install(cfg.versionfile_source, ipy)
+    do_vcs_install(manifest_in, cfg.versionfile_source, ipy)
     return 0
 
 
 def scan_setup_py():
     """Validate the contents of setup.py against Versioneer's expectations."""
     found = set()
     setters = False
@@ -2223,18 +2096,14 @@
         print("'versioneer.versionfile_source = ' . This configuration")
         print("now lives in setup.cfg, and should be removed from setup.py")
         print("")
         errors += 1
     return errors
 
 
-def setup_command():
-    """Set up Versioneer and exit with appropriate error code."""
-    errors = do_setup()
-    errors += scan_setup_py()
-    sys.exit(1 if errors else 0)
-
-
 if __name__ == "__main__":
     cmd = sys.argv[1]
     if cmd == "setup":
-        setup_command()
+        errors = do_setup()
+        errors += scan_setup_py()
+        if errors:
+            sys.exit(1)
```

