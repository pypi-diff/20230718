# Comparing `tmp/cbcflow-0.3.0.tar.gz` & `tmp/cbcflow-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcflow-0.3.0.tar", last modified: Thu Jul  6 21:26:55 2023, max compression
+gzip compressed data, was "cbcflow-0.3.1.tar", last modified: Tue Jul 18 14:24:09 2023, max compression
```

## Comparing `cbcflow-0.3.0.tar` & `cbcflow-0.3.1.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:55.416123 cbcflow-0.3.0/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       37 2022-09-02 21:51:00.000000 cbcflow-0.3.0/.gitattributes
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      217 2023-04-17 16:08:35.000000 cbcflow-0.3.0/.gitignore
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1542 2023-06-13 21:02:31.000000 cbcflow-0.3.0/.gitlab-ci.yml
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      873 2023-03-15 15:11:03.000000 cbcflow-0.3.0/.pre-commit-config.yaml
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1078 2023-05-10 19:01:56.000000 cbcflow-0.3.0/CHANGELOG.md
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1084 2023-04-17 16:08:35.000000 cbcflow-0.3.0/LICENSE.md
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      123 2023-04-17 16:08:35.000000 cbcflow-0.3.0/MANIFEST.in
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3027 2023-07-06 21:26:55.417123 cbcflow-0.3.0/PKG-INFO
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2390 2023-04-21 18:28:00.000000 cbcflow-0.3.0/README.md
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-06-23 01:08:35.000000 cbcflow-0.3.0/asimov.log
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:54.890118 cbcflow-0.3.0/docs/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      613 2023-04-07 19:31:48.000000 cbcflow-0.3.0/docs/Makefile
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       53 2023-06-13 21:02:31.000000 cbcflow-0.3.0/docs/requirements.txt
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:55.134120 cbcflow-0.3.0/docs/source/
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:55.143120 cbcflow-0.3.0/docs/source/_templates/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      662 2023-04-07 19:31:48.000000 cbcflow-0.3.0/docs/source/_templates/custom-class-template.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1408 2023-04-07 19:31:48.000000 cbcflow-0.3.0/docs/source/_templates/custom-module-template.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1158 2023-06-13 21:02:31.000000 cbcflow-0.3.0/docs/source/actionitems.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      690 2023-04-17 16:08:35.000000 cbcflow-0.3.0/docs/source/adding-to-the-schema.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       39 2023-06-13 21:02:31.000000 cbcflow-0.3.0/docs/source/asimov.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4404 2023-05-05 16:21:05.000000 cbcflow-0.3.0/docs/source/cbcflow-git-merging.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2616 2023-06-13 21:02:31.000000 cbcflow-0.3.0/docs/source/conf.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1770 2023-06-13 21:02:31.000000 cbcflow-0.3.0/docs/source/configuration.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1444 2023-06-13 21:02:31.000000 cbcflow-0.3.0/docs/source/development-setup.rst
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:55.154120 cbcflow-0.3.0/docs/source/example_mini_schema/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2924 2023-04-17 16:08:35.000000 cbcflow-0.3.0/docs/source/example_mini_schema/example.schema
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     6391 2023-04-17 16:08:35.000000 cbcflow-0.3.0/docs/source/example_mini_schema/schema_doc.css
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    27212 2023-04-17 16:08:35.000000 cbcflow-0.3.0/docs/source/example_mini_schema/schema_doc.html
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      984 2023-04-17 16:08:35.000000 cbcflow-0.3.0/docs/source/example_mini_schema/schema_doc.min.js
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      458 2023-06-13 21:02:31.000000 cbcflow-0.3.0/docs/source/gwosc.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1255 2023-06-13 21:02:31.000000 cbcflow-0.3.0/docs/source/index.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2799 2023-04-07 19:31:49.000000 cbcflow-0.3.0/docs/source/libraries.rst
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:55.323122 cbcflow-0.3.0/docs/source/libraries_images/
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:55.325122 cbcflow-0.3.0/docs/source/libraries_images/.ipynb_checkpoints/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    72683 2023-04-07 19:31:49.000000 cbcflow-0.3.0/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     8993 2023-04-07 19:31:49.000000 cbcflow-0.3.0/docs/source/libraries_images/part_1.png
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    15966 2023-04-07 19:31:49.000000 cbcflow-0.3.0/docs/source/libraries_images/part_2.png
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    38016 2023-04-07 19:31:49.000000 cbcflow-0.3.0/docs/source/libraries_images/part_3.png
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    51488 2023-04-07 19:31:49.000000 cbcflow-0.3.0/docs/source/libraries_images/part_4.png
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    41435 2023-04-07 19:31:49.000000 cbcflow-0.3.0/docs/source/libraries_images/part_5.png
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    54941 2023-04-07 19:31:49.000000 cbcflow-0.3.0/docs/source/libraries_images/part_6.png
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    67345 2023-04-07 19:31:49.000000 cbcflow-0.3.0/docs/source/libraries_images/part_7.png
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    72180 2023-04-07 19:31:49.000000 cbcflow-0.3.0/docs/source/libraries_images/part_8.png
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    10255 2023-04-17 16:08:35.000000 cbcflow-0.3.0/docs/source/library-index-labelling.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1352 2023-06-13 21:02:31.000000 cbcflow-0.3.0/docs/source/library-indices.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3620 2023-05-09 00:07:03.000000 cbcflow-0.3.0/docs/source/library-setup-from-scratch.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1287 2023-06-13 21:02:31.000000 cbcflow-0.3.0/docs/source/local-library-copy-setup.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1782 2023-06-13 21:02:31.000000 cbcflow-0.3.0/docs/source/monitor-usage.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4809 2023-04-17 16:08:35.000000 cbcflow-0.3.0/docs/source/reading-the-schema.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      106 2023-04-07 19:31:49.000000 cbcflow-0.3.0/docs/source/schema-visualization.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    15476 2023-06-13 21:02:31.000000 cbcflow-0.3.0/docs/source/updating-metadata-from-the-command-line.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    12152 2023-06-13 21:02:31.000000 cbcflow-0.3.0/docs/source/updating-metadata-with-the-python-api.rst
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4916 2023-04-17 16:08:35.000000 cbcflow-0.3.0/docs/source/what-is-metadata.rst
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:55.328122 cbcflow-0.3.0/examples/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     7368 2022-09-29 19:29:06.000000 cbcflow-0.3.0/examples/initial_example.md
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      856 2023-04-21 18:28:00.000000 cbcflow-0.3.0/pyproject.toml
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:55.333122 cbcflow-0.3.0/schema/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    40294 2023-03-16 15:08:33.000000 cbcflow-0.3.0/schema/cbc-meta-data-v1.schema
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    88906 2023-04-25 20:47:59.000000 cbcflow-0.3.0/schema/cbc-meta-data-v2.schema
--rwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)     1766 2023-05-10 19:01:56.000000 cbcflow-0.3.0/schema/index-v1.schema
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1650 2023-07-06 21:26:55.419123 cbcflow-0.3.0/setup.cfg
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      567 2023-04-08 00:03:25.000000 cbcflow-0.3.0/setup.py
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:54.840117 cbcflow-0.3.0/src/
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:55.358122 cbcflow-0.3.0/src/cbcflow/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1870 2023-06-15 19:48:21.000000 cbcflow-0.3.0/src/cbcflow/__init__.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      160 2023-07-06 21:26:54.000000 cbcflow-0.3.0/src/cbcflow/_version.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    15920 2023-06-23 20:14:29.000000 cbcflow-0.3.0/src/cbcflow/asimov.py
--rwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)     9326 2023-05-30 19:09:00.000000 cbcflow-0.3.0/src/cbcflow/cbcflow.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1437 2023-06-23 01:08:35.000000 cbcflow-0.3.0/src/cbcflow/configuration.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    42220 2023-07-06 21:24:53.000000 cbcflow-0.3.0/src/cbcflow/database.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    14617 2023-06-23 20:14:29.000000 cbcflow-0.3.0/src/cbcflow/gracedb.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    15338 2023-06-23 01:08:45.000000 cbcflow-0.3.0/src/cbcflow/metadata.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     6270 2023-06-22 21:22:36.000000 cbcflow-0.3.0/src/cbcflow/monitor.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     9016 2023-05-16 15:26:32.000000 cbcflow-0.3.0/src/cbcflow/parser.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    10017 2023-06-23 20:14:29.000000 cbcflow-0.3.0/src/cbcflow/pe_scraper.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    35849 2023-05-10 19:01:56.000000 cbcflow-0.3.0/src/cbcflow/process.py
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:55.371122 cbcflow-0.3.0/src/cbcflow/schema/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    40294 2023-07-06 21:26:54.000000 cbcflow-0.3.0/src/cbcflow/schema/cbc-meta-data-v1.schema
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    88906 2023-07-06 21:26:54.000000 cbcflow-0.3.0/src/cbcflow/schema/cbc-meta-data-v2.schema
--rwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)     1766 2023-07-06 21:26:54.000000 cbcflow-0.3.0/src/cbcflow/schema/index-v1.schema
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2779 2023-04-25 20:47:59.000000 cbcflow-0.3.0/src/cbcflow/schema.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     7294 2023-05-10 19:01:56.000000 cbcflow-0.3.0/src/cbcflow/utils.py
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:55.366122 cbcflow-0.3.0/src/cbcflow.egg-info/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3027 2023-07-06 21:26:54.000000 cbcflow-0.3.0/src/cbcflow.egg-info/PKG-INFO
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3302 2023-07-06 21:26:54.000000 cbcflow-0.3.0/src/cbcflow.egg-info/SOURCES.txt
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)        1 2023-07-06 21:26:54.000000 cbcflow-0.3.0/src/cbcflow.egg-info/dependency_links.txt
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      599 2023-07-06 21:26:54.000000 cbcflow-0.3.0/src/cbcflow.egg-info/entry_points.txt
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      144 2023-07-06 21:26:54.000000 cbcflow-0.3.0/src/cbcflow.egg-info/requires.txt
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)        8 2023-07-06 21:26:54.000000 cbcflow-0.3.0/src/cbcflow.egg-info/top_level.txt
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:55.380123 cbcflow-0.3.0/tests/
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:55.395123 cbcflow-0.3.0/tests/files_for_testing/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    26759 2023-04-07 19:31:49.000000 cbcflow-0.3.0/tests/files_for_testing/cbc-meta-data-example.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     5972 2023-05-05 16:21:05.000000 cbcflow-0.3.0/tests/files_for_testing/merge_test.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       56 2023-04-07 19:31:49.000000 cbcflow-0.3.0/tests/files_for_testing/test-file-for-linking-1.txt
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       86 2023-04-07 19:31:49.000000 cbcflow-0.3.0/tests/files_for_testing/test-file-for-linking-2.txt
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       53 2023-05-05 16:21:05.000000 cbcflow-0.3.0/tests/files_for_testing/test-file-for-linking-3.txt
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3091 2023-04-07 19:31:49.000000 cbcflow-0.3.0/tests/files_for_testing/update_json_1.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1221 2023-04-07 19:31:49.000000 cbcflow-0.3.0/tests/files_for_testing/update_json_2.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1626 2023-04-07 19:31:49.000000 cbcflow-0.3.0/tests/files_for_testing/update_yaml_1.yaml
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      571 2023-04-07 19:31:49.000000 cbcflow-0.3.0/tests/files_for_testing/update_yaml_2.yaml
-drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-06 21:26:55.414123 cbcflow-0.3.0/tests/library_for_testing/
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     5338 2023-04-08 00:03:25.000000 cbcflow-0.3.0/tests/library_for_testing/S230227hp-cbc-metadata.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4289 2023-04-08 00:03:25.000000 cbcflow-0.3.0/tests/library_for_testing/S230331e-cbc-metadata.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4275 2023-04-08 00:03:25.000000 cbcflow-0.3.0/tests/library_for_testing/S230401h-cbc-metadata.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2416 2023-04-08 00:03:25.000000 cbcflow-0.3.0/tests/library_for_testing/S230402dv-cbc-metadata.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3353 2023-04-08 00:03:25.000000 cbcflow-0.3.0/tests/library_for_testing/S230403ae-cbc-metadata.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     5238 2023-04-08 00:03:25.000000 cbcflow-0.3.0/tests/library_for_testing/S230404hb-cbc-metadata.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3256 2023-04-08 00:03:25.000000 cbcflow-0.3.0/tests/library_for_testing/S230404jc-cbc-metadata.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      193 2023-04-07 19:31:48.000000 cbcflow-0.3.0/tests/library_for_testing/library.cfg
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       90 2023-04-07 19:31:48.000000 cbcflow-0.3.0/tests/library_for_testing/testing-library-index.json
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3519 2023-06-02 08:52:01.000000 cbcflow-0.3.0/tests/test_database.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    38496 2023-05-05 16:21:05.000000 cbcflow-0.3.0/tests/test_merging.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    32821 2023-06-23 01:08:45.000000 cbcflow-0.3.0/tests/test_metadata.py
--rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      755 2023-03-27 22:27:03.000000 cbcflow-0.3.0/tests/test_schema.py
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-18 14:24:09.181838 cbcflow-0.3.1/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       37 2022-09-02 21:51:00.000000 cbcflow-0.3.1/.gitattributes
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      217 2023-04-17 16:08:35.000000 cbcflow-0.3.1/.gitignore
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1542 2023-06-13 21:02:31.000000 cbcflow-0.3.1/.gitlab-ci.yml
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      873 2023-03-15 15:11:03.000000 cbcflow-0.3.1/.pre-commit-config.yaml
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1078 2023-05-10 19:01:56.000000 cbcflow-0.3.1/CHANGELOG.md
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1084 2023-04-17 16:08:35.000000 cbcflow-0.3.1/LICENSE.md
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      123 2023-04-17 16:08:35.000000 cbcflow-0.3.1/MANIFEST.in
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3027 2023-07-18 14:24:09.181838 cbcflow-0.3.1/PKG-INFO
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2390 2023-04-21 18:28:00.000000 cbcflow-0.3.1/README.md
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-06-23 01:08:35.000000 cbcflow-0.3.1/asimov.log
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-18 14:24:08.839835 cbcflow-0.3.1/docs/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      613 2023-04-07 19:31:48.000000 cbcflow-0.3.1/docs/Makefile
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       53 2023-06-13 21:02:31.000000 cbcflow-0.3.1/docs/requirements.txt
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-18 14:24:08.957836 cbcflow-0.3.1/docs/source/
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-18 14:24:08.960836 cbcflow-0.3.1/docs/source/_templates/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      662 2023-04-07 19:31:48.000000 cbcflow-0.3.1/docs/source/_templates/custom-class-template.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1408 2023-04-07 19:31:48.000000 cbcflow-0.3.1/docs/source/_templates/custom-module-template.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1158 2023-06-13 21:02:31.000000 cbcflow-0.3.1/docs/source/actionitems.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      690 2023-04-17 16:08:35.000000 cbcflow-0.3.1/docs/source/adding-to-the-schema.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       39 2023-06-13 21:02:31.000000 cbcflow-0.3.1/docs/source/asimov.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4404 2023-05-05 16:21:05.000000 cbcflow-0.3.1/docs/source/cbcflow-git-merging.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2616 2023-06-13 21:02:31.000000 cbcflow-0.3.1/docs/source/conf.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1770 2023-06-13 21:02:31.000000 cbcflow-0.3.1/docs/source/configuration.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1444 2023-06-13 21:02:31.000000 cbcflow-0.3.1/docs/source/development-setup.rst
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-18 14:24:08.966836 cbcflow-0.3.1/docs/source/example_mini_schema/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2924 2023-04-17 16:08:35.000000 cbcflow-0.3.1/docs/source/example_mini_schema/example.schema
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     6391 2023-04-17 16:08:35.000000 cbcflow-0.3.1/docs/source/example_mini_schema/schema_doc.css
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    27212 2023-04-17 16:08:35.000000 cbcflow-0.3.1/docs/source/example_mini_schema/schema_doc.html
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      984 2023-04-17 16:08:35.000000 cbcflow-0.3.1/docs/source/example_mini_schema/schema_doc.min.js
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      458 2023-06-13 21:02:31.000000 cbcflow-0.3.1/docs/source/gwosc.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1255 2023-06-13 21:02:31.000000 cbcflow-0.3.1/docs/source/index.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2799 2023-04-07 19:31:49.000000 cbcflow-0.3.1/docs/source/libraries.rst
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-18 14:24:09.110837 cbcflow-0.3.1/docs/source/libraries_images/
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-18 14:24:09.113837 cbcflow-0.3.1/docs/source/libraries_images/.ipynb_checkpoints/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    72683 2023-04-07 19:31:49.000000 cbcflow-0.3.1/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     8993 2023-04-07 19:31:49.000000 cbcflow-0.3.1/docs/source/libraries_images/part_1.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    15966 2023-04-07 19:31:49.000000 cbcflow-0.3.1/docs/source/libraries_images/part_2.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    38016 2023-04-07 19:31:49.000000 cbcflow-0.3.1/docs/source/libraries_images/part_3.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    51488 2023-04-07 19:31:49.000000 cbcflow-0.3.1/docs/source/libraries_images/part_4.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    41435 2023-04-07 19:31:49.000000 cbcflow-0.3.1/docs/source/libraries_images/part_5.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    54941 2023-04-07 19:31:49.000000 cbcflow-0.3.1/docs/source/libraries_images/part_6.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    67345 2023-04-07 19:31:49.000000 cbcflow-0.3.1/docs/source/libraries_images/part_7.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    72180 2023-04-07 19:31:49.000000 cbcflow-0.3.1/docs/source/libraries_images/part_8.png
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    10255 2023-04-17 16:08:35.000000 cbcflow-0.3.1/docs/source/library-index-labelling.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1352 2023-06-13 21:02:31.000000 cbcflow-0.3.1/docs/source/library-indices.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3620 2023-05-09 00:07:03.000000 cbcflow-0.3.1/docs/source/library-setup-from-scratch.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1287 2023-06-13 21:02:31.000000 cbcflow-0.3.1/docs/source/local-library-copy-setup.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1782 2023-06-13 21:02:31.000000 cbcflow-0.3.1/docs/source/monitor-usage.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4809 2023-04-17 16:08:35.000000 cbcflow-0.3.1/docs/source/reading-the-schema.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      106 2023-04-07 19:31:49.000000 cbcflow-0.3.1/docs/source/schema-visualization.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    15476 2023-06-13 21:02:31.000000 cbcflow-0.3.1/docs/source/updating-metadata-from-the-command-line.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    12152 2023-06-13 21:02:31.000000 cbcflow-0.3.1/docs/source/updating-metadata-with-the-python-api.rst
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4916 2023-04-17 16:08:35.000000 cbcflow-0.3.1/docs/source/what-is-metadata.rst
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-18 14:24:09.115837 cbcflow-0.3.1/examples/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     7368 2022-09-29 19:29:06.000000 cbcflow-0.3.1/examples/initial_example.md
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      856 2023-04-21 18:28:00.000000 cbcflow-0.3.1/pyproject.toml
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-18 14:24:09.120837 cbcflow-0.3.1/schema/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    40294 2023-03-16 15:08:33.000000 cbcflow-0.3.1/schema/cbc-meta-data-v1.schema
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    88906 2023-04-25 20:47:59.000000 cbcflow-0.3.1/schema/cbc-meta-data-v2.schema
+-rwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)     1766 2023-05-10 19:01:56.000000 cbcflow-0.3.1/schema/index-v1.schema
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1650 2023-07-18 14:24:09.183838 cbcflow-0.3.1/setup.cfg
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      567 2023-04-08 00:03:25.000000 cbcflow-0.3.1/setup.py
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-18 14:24:08.798834 cbcflow-0.3.1/src/
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-18 14:24:09.136837 cbcflow-0.3.1/src/cbcflow/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1870 2023-06-15 19:48:21.000000 cbcflow-0.3.1/src/cbcflow/__init__.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      160 2023-07-18 14:24:08.000000 cbcflow-0.3.1/src/cbcflow/_version.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    15920 2023-06-23 20:14:29.000000 cbcflow-0.3.1/src/cbcflow/asimov.py
+-rwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)     9326 2023-05-30 19:09:00.000000 cbcflow-0.3.1/src/cbcflow/cbcflow.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1437 2023-06-23 01:08:35.000000 cbcflow-0.3.1/src/cbcflow/configuration.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    42220 2023-07-06 21:24:53.000000 cbcflow-0.3.1/src/cbcflow/database.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    14629 2023-07-18 14:21:47.000000 cbcflow-0.3.1/src/cbcflow/gracedb.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    15338 2023-06-23 01:08:45.000000 cbcflow-0.3.1/src/cbcflow/metadata.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     6270 2023-06-22 21:22:36.000000 cbcflow-0.3.1/src/cbcflow/monitor.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     9016 2023-05-16 15:26:32.000000 cbcflow-0.3.1/src/cbcflow/parser.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    10017 2023-06-23 20:14:29.000000 cbcflow-0.3.1/src/cbcflow/pe_scraper.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    35849 2023-05-10 19:01:56.000000 cbcflow-0.3.1/src/cbcflow/process.py
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-18 14:24:09.147837 cbcflow-0.3.1/src/cbcflow/schema/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    40294 2023-07-18 14:24:08.000000 cbcflow-0.3.1/src/cbcflow/schema/cbc-meta-data-v1.schema
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    88906 2023-07-18 14:24:08.000000 cbcflow-0.3.1/src/cbcflow/schema/cbc-meta-data-v2.schema
+-rwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)     1766 2023-07-18 14:24:08.000000 cbcflow-0.3.1/src/cbcflow/schema/index-v1.schema
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2779 2023-04-25 20:47:59.000000 cbcflow-0.3.1/src/cbcflow/schema.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     7294 2023-05-10 19:01:56.000000 cbcflow-0.3.1/src/cbcflow/utils.py
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-18 14:24:09.143837 cbcflow-0.3.1/src/cbcflow.egg-info/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3027 2023-07-18 14:24:08.000000 cbcflow-0.3.1/src/cbcflow.egg-info/PKG-INFO
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3302 2023-07-18 14:24:08.000000 cbcflow-0.3.1/src/cbcflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)        1 2023-07-18 14:24:08.000000 cbcflow-0.3.1/src/cbcflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      599 2023-07-18 14:24:08.000000 cbcflow-0.3.1/src/cbcflow.egg-info/entry_points.txt
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      144 2023-07-18 14:24:08.000000 cbcflow-0.3.1/src/cbcflow.egg-info/requires.txt
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)        8 2023-07-18 14:24:08.000000 cbcflow-0.3.1/src/cbcflow.egg-info/top_level.txt
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-18 14:24:09.152837 cbcflow-0.3.1/tests/
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-18 14:24:09.165837 cbcflow-0.3.1/tests/files_for_testing/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    26759 2023-04-07 19:31:49.000000 cbcflow-0.3.1/tests/files_for_testing/cbc-meta-data-example.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     5972 2023-05-05 16:21:05.000000 cbcflow-0.3.1/tests/files_for_testing/merge_test.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       56 2023-04-07 19:31:49.000000 cbcflow-0.3.1/tests/files_for_testing/test-file-for-linking-1.txt
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       86 2023-04-07 19:31:49.000000 cbcflow-0.3.1/tests/files_for_testing/test-file-for-linking-2.txt
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       53 2023-05-05 16:21:05.000000 cbcflow-0.3.1/tests/files_for_testing/test-file-for-linking-3.txt
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3091 2023-04-07 19:31:49.000000 cbcflow-0.3.1/tests/files_for_testing/update_json_1.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1221 2023-04-07 19:31:49.000000 cbcflow-0.3.1/tests/files_for_testing/update_json_2.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     1626 2023-04-07 19:31:49.000000 cbcflow-0.3.1/tests/files_for_testing/update_yaml_1.yaml
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      571 2023-04-07 19:31:49.000000 cbcflow-0.3.1/tests/files_for_testing/update_yaml_2.yaml
+drwxrwxr-x   0 rhiannon.udall (45200) rhiannon.udall (45200)        0 2023-07-18 14:24:09.180837 cbcflow-0.3.1/tests/library_for_testing/
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     5338 2023-04-08 00:03:25.000000 cbcflow-0.3.1/tests/library_for_testing/S230227hp-cbc-metadata.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4289 2023-04-08 00:03:25.000000 cbcflow-0.3.1/tests/library_for_testing/S230331e-cbc-metadata.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     4275 2023-04-08 00:03:25.000000 cbcflow-0.3.1/tests/library_for_testing/S230401h-cbc-metadata.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     2416 2023-04-08 00:03:25.000000 cbcflow-0.3.1/tests/library_for_testing/S230402dv-cbc-metadata.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3353 2023-04-08 00:03:25.000000 cbcflow-0.3.1/tests/library_for_testing/S230403ae-cbc-metadata.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     5238 2023-04-08 00:03:25.000000 cbcflow-0.3.1/tests/library_for_testing/S230404hb-cbc-metadata.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3256 2023-04-08 00:03:25.000000 cbcflow-0.3.1/tests/library_for_testing/S230404jc-cbc-metadata.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      193 2023-04-07 19:31:48.000000 cbcflow-0.3.1/tests/library_for_testing/library.cfg
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)       90 2023-04-07 19:31:48.000000 cbcflow-0.3.1/tests/library_for_testing/testing-library-index.json
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)     3519 2023-06-02 08:52:01.000000 cbcflow-0.3.1/tests/test_database.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    38496 2023-05-05 16:21:05.000000 cbcflow-0.3.1/tests/test_merging.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)    32821 2023-06-23 01:08:45.000000 cbcflow-0.3.1/tests/test_metadata.py
+-rw-rw-r--   0 rhiannon.udall (45200) rhiannon.udall (45200)      755 2023-03-27 22:27:03.000000 cbcflow-0.3.1/tests/test_schema.py
```

### Comparing `cbcflow-0.3.0/.gitlab-ci.yml` & `cbcflow-0.3.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/.pre-commit-config.yaml` & `cbcflow-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/CHANGELOG.md` & `cbcflow-0.3.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/LICENSE.md` & `cbcflow-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/PKG-INFO` & `cbcflow-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcflow
-Version: 0.3.0
+Version: 0.3.1
 Summary: A package for enabling CBC analyses
 Home-page: https://git.ligo.org/cbc/cbcflow
 Author: Gregory Ashton
 Author-email: Gregory Ashton <gregory.ashton@ligo.org>, Rhiannon Udall <rhiannon.udall@ligo.org>
 Project-URL: Homepage, https://git.ligo.org/cbc/projects/cbcflow
 Project-URL: Bug Tracker, https://git.ligo.org/cbc/projects/cbcflow/-/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cbcflow-0.3.0/README.md` & `cbcflow-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/Makefile` & `cbcflow-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/_templates/custom-class-template.rst` & `cbcflow-0.3.1/docs/source/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/_templates/custom-module-template.rst` & `cbcflow-0.3.1/docs/source/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/actionitems.rst` & `cbcflow-0.3.1/docs/source/actionitems.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/adding-to-the-schema.rst` & `cbcflow-0.3.1/docs/source/adding-to-the-schema.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/cbcflow-git-merging.rst` & `cbcflow-0.3.1/docs/source/cbcflow-git-merging.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/conf.py` & `cbcflow-0.3.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/configuration.rst` & `cbcflow-0.3.1/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/development-setup.rst` & `cbcflow-0.3.1/docs/source/development-setup.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/example_mini_schema/example.schema` & `cbcflow-0.3.1/docs/source/example_mini_schema/example.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/example_mini_schema/schema_doc.css` & `cbcflow-0.3.1/docs/source/example_mini_schema/schema_doc.css`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/example_mini_schema/schema_doc.html` & `cbcflow-0.3.1/docs/source/example_mini_schema/schema_doc.html`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/example_mini_schema/schema_doc.min.js` & `cbcflow-0.3.1/docs/source/example_mini_schema/schema_doc.min.js`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/index.rst` & `cbcflow-0.3.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/libraries.rst` & `cbcflow-0.3.1/docs/source/libraries.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png` & `cbcflow-0.3.1/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/libraries_images/part_1.png` & `cbcflow-0.3.1/docs/source/libraries_images/part_1.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/libraries_images/part_2.png` & `cbcflow-0.3.1/docs/source/libraries_images/part_2.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/libraries_images/part_3.png` & `cbcflow-0.3.1/docs/source/libraries_images/part_3.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/libraries_images/part_4.png` & `cbcflow-0.3.1/docs/source/libraries_images/part_4.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/libraries_images/part_5.png` & `cbcflow-0.3.1/docs/source/libraries_images/part_5.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/libraries_images/part_6.png` & `cbcflow-0.3.1/docs/source/libraries_images/part_6.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/libraries_images/part_7.png` & `cbcflow-0.3.1/docs/source/libraries_images/part_7.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/libraries_images/part_8.png` & `cbcflow-0.3.1/docs/source/libraries_images/part_8.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/library-index-labelling.rst` & `cbcflow-0.3.1/docs/source/library-index-labelling.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/library-indices.rst` & `cbcflow-0.3.1/docs/source/library-indices.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/library-setup-from-scratch.rst` & `cbcflow-0.3.1/docs/source/library-setup-from-scratch.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/local-library-copy-setup.rst` & `cbcflow-0.3.1/docs/source/local-library-copy-setup.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/monitor-usage.rst` & `cbcflow-0.3.1/docs/source/monitor-usage.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/reading-the-schema.rst` & `cbcflow-0.3.1/docs/source/reading-the-schema.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/updating-metadata-from-the-command-line.rst` & `cbcflow-0.3.1/docs/source/updating-metadata-from-the-command-line.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/updating-metadata-with-the-python-api.rst` & `cbcflow-0.3.1/docs/source/updating-metadata-with-the-python-api.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/docs/source/what-is-metadata.rst` & `cbcflow-0.3.1/docs/source/what-is-metadata.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/examples/initial_example.md` & `cbcflow-0.3.1/examples/initial_example.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/pyproject.toml` & `cbcflow-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/schema/cbc-meta-data-v1.schema` & `cbcflow-0.3.1/schema/cbc-meta-data-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/schema/cbc-meta-data-v2.schema` & `cbcflow-0.3.1/schema/cbc-meta-data-v2.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/schema/index-v1.schema` & `cbcflow-0.3.1/schema/index-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/setup.cfg` & `cbcflow-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/setup.py` & `cbcflow-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/src/cbcflow/__init__.py` & `cbcflow-0.3.1/src/cbcflow/__init__.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/src/cbcflow/asimov.py` & `cbcflow-0.3.1/src/cbcflow/asimov.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/src/cbcflow/cbcflow.py` & `cbcflow-0.3.1/src/cbcflow/cbcflow.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/src/cbcflow/configuration.py` & `cbcflow-0.3.1/src/cbcflow/configuration.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/src/cbcflow/database.py` & `cbcflow-0.3.1/src/cbcflow/database.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/src/cbcflow/gracedb.py` & `cbcflow-0.3.1/src/cbcflow/gracedb.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             # Get the json of metadata for the superevent
             superevent = gdb.superevent(sname).json()
         except HTTPError:
             msg = f"Superevent {sname} not found on {service_url}. "
             msg += "Either it does not exist, or you may need to run ligo-proxy-init."
             raise ValueError(msg)
         # We want the one best event per pipeline
-        event_dict = superevent["pipeline_preferred_events"]
+        event_dict = superevent.get("pipeline_preferred_events", dict())
         preferred_event = superevent["preferred_event_data"]
         if "ADVNO" in superevent["labels"]:
             # If ADVNO is here that means this event is retracted
             data["Info"]["Notes"].append("Retracted: ADVNO applied in GraceDB")
         if len(event_dict) == 0:
             event_dict[preferred_event["pipeline"]] = preferred_event
         for pipeline, event in superevent["pipeline_preferred_events"].items():
```

### Comparing `cbcflow-0.3.0/src/cbcflow/metadata.py` & `cbcflow-0.3.1/src/cbcflow/metadata.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/src/cbcflow/monitor.py` & `cbcflow-0.3.1/src/cbcflow/monitor.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/src/cbcflow/parser.py` & `cbcflow-0.3.1/src/cbcflow/parser.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/src/cbcflow/pe_scraper.py` & `cbcflow-0.3.1/src/cbcflow/pe_scraper.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/src/cbcflow/process.py` & `cbcflow-0.3.1/src/cbcflow/process.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/src/cbcflow/schema/cbc-meta-data-v1.schema` & `cbcflow-0.3.1/src/cbcflow/schema/cbc-meta-data-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/src/cbcflow/schema/cbc-meta-data-v2.schema` & `cbcflow-0.3.1/src/cbcflow/schema/cbc-meta-data-v2.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/src/cbcflow/schema/index-v1.schema` & `cbcflow-0.3.1/src/cbcflow/schema/index-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/src/cbcflow/schema.py` & `cbcflow-0.3.1/src/cbcflow/schema.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/src/cbcflow/utils.py` & `cbcflow-0.3.1/src/cbcflow/utils.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/src/cbcflow.egg-info/PKG-INFO` & `cbcflow-0.3.1/src/cbcflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcflow
-Version: 0.3.0
+Version: 0.3.1
 Summary: A package for enabling CBC analyses
 Home-page: https://git.ligo.org/cbc/cbcflow
 Author: Gregory Ashton
 Author-email: Gregory Ashton <gregory.ashton@ligo.org>, Rhiannon Udall <rhiannon.udall@ligo.org>
 Project-URL: Homepage, https://git.ligo.org/cbc/projects/cbcflow
 Project-URL: Bug Tracker, https://git.ligo.org/cbc/projects/cbcflow/-/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cbcflow-0.3.0/src/cbcflow.egg-info/SOURCES.txt` & `cbcflow-0.3.1/src/cbcflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/src/cbcflow.egg-info/entry_points.txt` & `cbcflow-0.3.1/src/cbcflow.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/tests/files_for_testing/cbc-meta-data-example.json` & `cbcflow-0.3.1/tests/files_for_testing/cbc-meta-data-example.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/tests/files_for_testing/merge_test.json` & `cbcflow-0.3.1/tests/files_for_testing/merge_test.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/tests/files_for_testing/update_json_1.json` & `cbcflow-0.3.1/tests/files_for_testing/update_json_1.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/tests/files_for_testing/update_json_2.json` & `cbcflow-0.3.1/tests/files_for_testing/update_json_2.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/tests/files_for_testing/update_yaml_1.yaml` & `cbcflow-0.3.1/tests/files_for_testing/update_yaml_1.yaml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/tests/files_for_testing/update_yaml_2.yaml` & `cbcflow-0.3.1/tests/files_for_testing/update_yaml_2.yaml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/tests/library_for_testing/S230227hp-cbc-metadata.json` & `cbcflow-0.3.1/tests/library_for_testing/S230227hp-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/tests/library_for_testing/S230331e-cbc-metadata.json` & `cbcflow-0.3.1/tests/library_for_testing/S230331e-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/tests/library_for_testing/S230401h-cbc-metadata.json` & `cbcflow-0.3.1/tests/library_for_testing/S230401h-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/tests/library_for_testing/S230402dv-cbc-metadata.json` & `cbcflow-0.3.1/tests/library_for_testing/S230402dv-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/tests/library_for_testing/S230403ae-cbc-metadata.json` & `cbcflow-0.3.1/tests/library_for_testing/S230403ae-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/tests/library_for_testing/S230404hb-cbc-metadata.json` & `cbcflow-0.3.1/tests/library_for_testing/S230404hb-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/tests/library_for_testing/S230404jc-cbc-metadata.json` & `cbcflow-0.3.1/tests/library_for_testing/S230404jc-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/tests/test_database.py` & `cbcflow-0.3.1/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/tests/test_merging.py` & `cbcflow-0.3.1/tests/test_merging.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/tests/test_metadata.py` & `cbcflow-0.3.1/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.3.0/tests/test_schema.py` & `cbcflow-0.3.1/tests/test_schema.py`

 * *Files identical despite different names*

