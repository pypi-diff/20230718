# Comparing `tmp/iceberg_tools-0.0.3.tar.gz` & `tmp/iceberg_tools-0.0.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iceberg_tools-0.0.3.tar", last modified: Fri Jun 23 21:40:11 2023, max compression
+gzip compressed data, was "iceberg_tools-0.0.4rc1.tar", last modified: Mon Jul 17 23:39:33 2023, max compression
```

## Comparing `iceberg_tools-0.0.3.tar` & `iceberg_tools-0.0.4rc1.tar`

### file list

```diff
@@ -1,84 +1,86 @@
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.287735 iceberg_tools-0.0.3/
--rw-r--r--   0 walsbr   (320923486) 1971611142     3070 2023-06-23 21:40:11.287465 iceberg_tools-0.0.3/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     2337 2023-06-23 21:38:25.000000 iceberg_tools-0.0.3/README.md
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.213880 iceberg_tools-0.0.3/iceberg_tools/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-06-02 23:04:59.000000 iceberg_tools-0.0.3/iceberg_tools/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.224734 iceberg_tools-0.0.3/iceberg_tools/cli/
--rw-r--r--   0 walsbr   (320923486) 1971611142      510 2023-06-02 23:04:59.000000 iceberg_tools-0.0.3/iceberg_tools/cli/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     5947 2023-06-23 21:37:38.000000 iceberg_tools-0.0.3/iceberg_tools/cli/data.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4902 2023-06-02 23:04:59.000000 iceberg_tools-0.0.3/iceberg_tools/cli/schema.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.229253 iceberg_tools-0.0.3/iceberg_tools/data/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-06-02 23:04:59.000000 iceberg_tools-0.0.3/iceberg_tools/data/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.229629 iceberg_tools-0.0.3/iceberg_tools/data/migrator/
--rw-r--r--   0 walsbr   (320923486) 1971611142    13714 2023-06-02 23:04:59.000000 iceberg_tools-0.0.3/iceberg_tools/data/migrator/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     6137 2023-06-02 23:04:59.000000 iceberg_tools-0.0.3/iceberg_tools/data/pfb.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3530 2023-06-02 23:04:59.000000 iceberg_tools-0.0.3/iceberg_tools/data/report.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.230927 iceberg_tools-0.0.3/iceberg_tools/data/simplifier/
--rw-r--r--   0 walsbr   (320923486) 1971611142    29385 2023-06-11 13:19:39.000000 iceberg_tools-0.0.3/iceberg_tools/data/simplifier/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142   123504 2023-06-02 23:04:59.000000 iceberg_tools-0.0.3/iceberg_tools/data/simplifier/oid_lookup.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.232754 iceberg_tools-0.0.3/iceberg_tools/graph/
--rw-r--r--   0 walsbr   (320923486) 1971611142      212 2023-06-23 21:26:39.000000 iceberg_tools-0.0.3/iceberg_tools/graph/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.240782 iceberg_tools-0.0.3/iceberg_tools/schema/
--rw-r--r--   0 walsbr   (320923486) 1971611142    11282 2023-06-02 23:22:12.000000 iceberg_tools-0.0.3/iceberg_tools/schema/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.249711 iceberg_tools-0.0.3/iceberg_tools/schema/fhir_resources/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-06-02 23:09:01.000000 iceberg_tools-0.0.3/iceberg_tools/schema/fhir_resources/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3629 2023-06-02 23:24:05.000000 iceberg_tools-0.0.3/iceberg_tools/schema/fhir_resources/binding_lookup.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1349 2023-06-02 23:04:59.000000 iceberg_tools-0.0.3/iceberg_tools/schema/graph.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    24435 2023-06-09 19:07:39.000000 iceberg_tools-0.0.3/iceberg_tools/schema/simplified.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4355 2023-06-09 13:56:59.000000 iceberg_tools-0.0.3/iceberg_tools/schema/simplified_validator.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     6840 2023-06-02 23:04:59.000000 iceberg_tools-0.0.3/iceberg_tools/util.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.219869 iceberg_tools-0.0.3/iceberg_tools.egg-info/
--rw-r--r--   0 walsbr   (320923486) 1971611142     3070 2023-06-23 21:40:11.000000 iceberg_tools-0.0.3/iceberg_tools.egg-info/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     2610 2023-06-23 21:40:11.000000 iceberg_tools-0.0.3/iceberg_tools.egg-info/SOURCES.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142        1 2023-06-23 21:40:11.000000 iceberg_tools-0.0.3/iceberg_tools.egg-info/dependency_links.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       84 2023-06-23 21:40:11.000000 iceberg_tools-0.0.3/iceberg_tools.egg-info/entry_points.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142      146 2023-06-23 21:40:11.000000 iceberg_tools-0.0.3/iceberg_tools.egg-info/requires.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       20 2023-06-23 21:40:11.000000 iceberg_tools-0.0.3/iceberg_tools.egg-info/top_level.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       38 2023-06-23 21:40:11.287800 iceberg_tools-0.0.3/setup.cfg
--rw-r--r--   0 walsbr   (320923486) 1971611142     5748 2023-06-23 21:39:15.000000 iceberg_tools-0.0.3/setup.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.210299 iceberg_tools-0.0.3/tests/
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.250716 iceberg_tools-0.0.3/tests/integration/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-06-02 22:54:19.000000 iceberg_tools-0.0.3/tests/integration/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.252777 iceberg_tools-0.0.3/tests/integration/data/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/data/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      305 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/data/conftest.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.254346 iceberg_tools-0.0.3/tests/integration/data/simplifier/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/data/simplifier/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1296 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/data/simplifier/test_simplify.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     5605 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/data/test_pfb.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.281854 iceberg_tools-0.0.3/tests/integration/graph/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1834 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/graph/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      972 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/graph/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      782 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/graph/test_edge_load_granular_reference.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2743 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/graph/test_edge_validator.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1449 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/graph/test_invalid_edges.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      255 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/graph/test_lathe_lint.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      663 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/graph/test_negative_trivial_vertex_load.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      829 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/graph/test_schema.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      330 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/graph/test_schema_load.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1140 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/graph/test_spot_check_embedded_type.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      731 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/graph/test_trivial_edge_load.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      889 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/graph/test_trivial_vertex_load.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      340 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/graph/test_yaml_anonymous_schemas.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.285752 iceberg_tools-0.0.3/tests/integration/simplified/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      665 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      911 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/test_codeable_concept.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      378 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/test_embedded_types.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      503 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/test_identifiers.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      171 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/test_individual_yaml.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      275 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/test_keys.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      979 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/test_primitive.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      469 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/test_quantities.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      517 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/test_research_study_has_project.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      216 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/test_schema.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1830 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/test_simplify_medication.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1742 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/test_simplify_task.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      665 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/test_specimen_plucked_properties.py
--rw-r--r--   0 walsbr   (320923486) 1971611142       34 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/integration/simplified/test_task.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-23 21:40:11.287042 iceberg_tools-0.0.3/tests/unit/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-06-02 22:54:19.000000 iceberg_tools-0.0.3/tests/unit/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      176 2023-06-02 22:54:19.000000 iceberg_tools-0.0.3/tests/unit/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      565 2023-06-02 22:54:19.000000 iceberg_tools-0.0.3/tests/unit/test_coding_conventions.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3144 2023-06-02 23:05:00.000000 iceberg_tools-0.0.3/tests/unit/test_schema.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    11142 2023-06-09 18:29:35.000000 iceberg_tools-0.0.3/tests/unit/test_simplify.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-17 23:39:33.528067 iceberg_tools-0.0.4rc1/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3073 2023-07-17 23:39:33.527484 iceberg_tools-0.0.4rc1/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2337 2023-07-13 19:41:15.000000 iceberg_tools-0.0.4rc1/README.md
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-17 23:39:33.501570 iceberg_tools-0.0.4rc1/iceberg_tools/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1015 2023-07-13 19:41:15.000000 iceberg_tools-0.0.4rc1/iceberg_tools/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-17 23:39:33.504626 iceberg_tools-0.0.4rc1/iceberg_tools/cli/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      434 2023-07-13 19:41:15.000000 iceberg_tools-0.0.4rc1/iceberg_tools/cli/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5947 2023-07-13 19:41:15.000000 iceberg_tools-0.0.4rc1/iceberg_tools/cli/data.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4897 2023-07-14 18:40:28.000000 iceberg_tools-0.0.4rc1/iceberg_tools/cli/schema.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-17 23:39:33.505457 iceberg_tools-0.0.4rc1/iceberg_tools/data/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-13 19:41:15.000000 iceberg_tools-0.0.4rc1/iceberg_tools/data/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-17 23:39:33.505798 iceberg_tools-0.0.4rc1/iceberg_tools/data/migrator/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    13714 2023-07-13 19:41:15.000000 iceberg_tools-0.0.4rc1/iceberg_tools/data/migrator/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     6137 2023-07-13 19:41:15.000000 iceberg_tools-0.0.4rc1/iceberg_tools/data/pfb.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3530 2023-07-13 19:41:15.000000 iceberg_tools-0.0.4rc1/iceberg_tools/data/report.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-17 23:39:33.506728 iceberg_tools-0.0.4rc1/iceberg_tools/data/simplifier/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    29478 2023-07-13 19:41:15.000000 iceberg_tools-0.0.4rc1/iceberg_tools/data/simplifier/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)   123504 2023-07-13 19:41:15.000000 iceberg_tools-0.0.4rc1/iceberg_tools/data/simplifier/oid_lookup.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-17 23:39:33.507416 iceberg_tools-0.0.4rc1/iceberg_tools/graph/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    18477 2023-07-17 16:54:31.000000 iceberg_tools-0.0.4rc1/iceberg_tools/graph/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-17 23:39:33.509339 iceberg_tools-0.0.4rc1/iceberg_tools/schema/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    11281 2023-07-13 19:41:15.000000 iceberg_tools-0.0.4rc1/iceberg_tools/schema/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-17 23:39:33.509849 iceberg_tools-0.0.4rc1/iceberg_tools/schema/fhir_resources/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-13 19:41:15.000000 iceberg_tools-0.0.4rc1/iceberg_tools/schema/fhir_resources/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3629 2023-07-13 19:41:15.000000 iceberg_tools-0.0.4rc1/iceberg_tools/schema/fhir_resources/binding_lookup.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1417 2023-07-14 18:40:28.000000 iceberg_tools-0.0.4rc1/iceberg_tools/schema/graph.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    24435 2023-07-13 19:41:15.000000 iceberg_tools-0.0.4rc1/iceberg_tools/schema/simplified.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4355 2023-07-13 19:41:15.000000 iceberg_tools-0.0.4rc1/iceberg_tools/schema/simplified_validator.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     7057 2023-07-13 19:41:15.000000 iceberg_tools-0.0.4rc1/iceberg_tools/util.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-17 23:39:33.503587 iceberg_tools-0.0.4rc1/iceberg_tools.egg-info/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3073 2023-07-17 23:39:33.000000 iceberg_tools-0.0.4rc1/iceberg_tools.egg-info/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2680 2023-07-17 23:39:33.000000 iceberg_tools-0.0.4rc1/iceberg_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        1 2023-07-17 23:39:33.000000 iceberg_tools-0.0.4rc1/iceberg_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       84 2023-07-17 23:39:33.000000 iceberg_tools-0.0.4rc1/iceberg_tools.egg-info/entry_points.txt
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      163 2023-07-17 23:39:33.000000 iceberg_tools-0.0.4rc1/iceberg_tools.egg-info/requires.txt
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       20 2023-07-17 23:39:33.000000 iceberg_tools-0.0.4rc1/iceberg_tools.egg-info/top_level.txt
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       38 2023-07-17 23:39:33.528148 iceberg_tools-0.0.4rc1/setup.cfg
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5751 2023-07-17 23:38:19.000000 iceberg_tools-0.0.4rc1/setup.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-17 23:39:33.500203 iceberg_tools-0.0.4rc1/tests/
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-17 23:39:33.510205 iceberg_tools-0.0.4rc1/tests/integration/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-06-02 22:54:19.000000 iceberg_tools-0.0.4rc1/tests/integration/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-17 23:39:33.511084 iceberg_tools-0.0.4rc1/tests/integration/data/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/data/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      328 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/data/conftest.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-17 23:39:33.513374 iceberg_tools-0.0.4rc1/tests/integration/data/simplifier/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/data/simplifier/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2659 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/data/simplifier/test_simplify.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     6342 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/data/test_pfb.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-17 23:39:33.521083 iceberg_tools-0.0.4rc1/tests/integration/graph/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1834 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/graph/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      972 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/graph/conftest.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      782 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/graph/test_edge_load_granular_reference.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2743 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/graph/test_edge_validator.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1449 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/graph/test_invalid_edges.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      255 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/graph/test_lathe_lint.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      663 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/graph/test_negative_trivial_vertex_load.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      829 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/graph/test_schema.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      330 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/graph/test_schema_load.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1140 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/graph/test_spot_check_embedded_type.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      731 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/graph/test_trivial_edge_load.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      889 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/graph/test_trivial_vertex_load.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      340 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/graph/test_yaml_anonymous_schemas.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-17 23:39:33.525092 iceberg_tools-0.0.4rc1/tests/integration/simplified/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/simplified/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      665 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/simplified/conftest.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      911 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/simplified/test_codeable_concept.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      378 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/simplified/test_embedded_types.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      503 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/simplified/test_identifiers.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      171 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/simplified/test_individual_yaml.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      275 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/simplified/test_keys.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      979 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/simplified/test_primitive.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      469 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/simplified/test_quantities.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      517 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/simplified/test_research_study_has_project.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      216 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/simplified/test_schema.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1830 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/simplified/test_simplify_medication.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1742 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/simplified/test_simplify_task.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      665 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/simplified/test_specimen_plucked_properties.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       34 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/integration/simplified/test_task.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-17 23:39:33.527186 iceberg_tools-0.0.4rc1/tests/unit/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-06-02 22:54:19.000000 iceberg_tools-0.0.4rc1/tests/unit/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      176 2023-07-13 18:37:47.000000 iceberg_tools-0.0.4rc1/tests/unit/conftest.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      565 2023-06-27 19:02:17.000000 iceberg_tools-0.0.4rc1/tests/unit/test_coding_conventions.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3138 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/unit/test_schema.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    11142 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/unit/test_simplify.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     8221 2023-07-14 18:40:28.000000 iceberg_tools-0.0.4rc1/tests/unit/test_swapi.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      755 2023-07-13 19:41:16.000000 iceberg_tools-0.0.4rc1/tests/unit/test_url_validate_monkey_patch.py
```

### Comparing `iceberg_tools-0.0.3/PKG-INFO` & `iceberg_tools-0.0.4rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iceberg_tools
-Version: 0.0.3
+Version: 0.0.4rc1
 Summary: FHIR schemas tools for bioinformatics.
 Home-page: https://github.com/bmeg/iceberg-schema-tools
 Author: https://ellrottlab.org/
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bmeg/iceberg-schema-tools/issues
 Project-URL: Source, https://github.com/bmeg/iceberg-schema-tools
 Keywords: FHIR PFB gen3 bioinformatics graph
```

### Comparing `iceberg_tools-0.0.3/README.md` & `iceberg_tools-0.0.4rc1/README.md`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.3/iceberg_tools/cli/data.py` & `iceberg_tools-0.0.4rc1/iceberg_tools/cli/data.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.3/iceberg_tools/cli/schema.py` & `iceberg_tools-0.0.4rc1/iceberg_tools/cli/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import logging
 import pathlib
 
 import click
 import yaml
 from yaml import SafeLoader
 
-from iceberg_tools.schema import _find_fhir_classes, BASE_URI, _extract_schemas
-from iceberg_tools.schema.graph import _bundle_schemas
+from iceberg_tools.schema import _find_fhir_classes, BASE_URI, extract_schemas
+from iceberg_tools.schema.graph import bundle_schemas
 from iceberg_tools.schema.simplified import _simplify_schemas
 from iceberg_tools.util import NaturalOrderGroup
 
 logger = logging.getLogger(__name__)
 
 
 @click.group('schema', cls=NaturalOrderGroup)
@@ -46,24 +46,24 @@
     config_path = pathlib.Path(config_path)
     assert output_path.is_dir()
     assert config_path.is_file()
     with open(config_path) as fp:
         gen3_config = yaml.load(fp, SafeLoader)
 
     classes = _find_fhir_classes(gen3_config, log_stats=stats)
-    schemas = _extract_schemas(classes, BASE_URI)
+    schemas = extract_schemas(classes, BASE_URI)
 
     output_path.mkdir(parents=True, exist_ok=True)
 
     for klass, schema in schemas.items():
         with open(output_path / pathlib.Path(klass + ".yaml"), "w") as fp:
             yaml.dump(schema, fp)
     logger.info(f"Individual yaml schemas written to {output_path}/*.yaml")
 
-    path = _bundle_schemas(output_path, BASE_URI)
+    path = bundle_schemas(output_path, BASE_URI)
     logger.info(f"Aggregated json schema written to {path}")
 
 
 @generate.command('simplified')
 @click.option('--output_path', required=True,
               default='iceberg/schemas/simplified',
               show_default=True,
@@ -89,15 +89,15 @@
     assert gen3_fixtures.is_dir()
     assert output_path.is_dir()
     assert config_path.is_file()
     with open(config_path) as fp:
         gen3_config = yaml.load(fp, SafeLoader)
 
     classes = _find_fhir_classes(gen3_config, log_stats=stats)
-    schemas = _extract_schemas(classes, BASE_URI)
+    schemas = extract_schemas(classes, BASE_URI)
     schemas = _simplify_schemas(gen3_config, gen3_fixtures, schemas, log_stats=stats)
 
     # also write out yaml files
     for k, v in schemas.items():
 
         fn = k
         if not k.startswith('_') and 'id' in v:
```

### Comparing `iceberg_tools-0.0.3/iceberg_tools/data/migrator/__init__.py` & `iceberg_tools-0.0.4rc1/iceberg_tools/data/migrator/__init__.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.3/iceberg_tools/data/pfb.py` & `iceberg_tools-0.0.4rc1/iceberg_tools/data/pfb.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.3/iceberg_tools/data/report.py` & `iceberg_tools-0.0.4rc1/iceberg_tools/data/report.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.3/iceberg_tools/data/simplifier/__init__.py` & `iceberg_tools-0.0.4rc1/iceberg_tools/data/simplifier/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -600,18 +600,19 @@
             transformed_references.append(f"{type_}/{id_}")
         THREAD_LOCAL.references = transformed_references
     return simplified, THREAD_LOCAL.references
 
 
 def check_simplified_schemas(simplified: dict, schemas: dict):
     """Compare simplified fields vs schema."""
-    resource_type = inflection.underscore(simplified['resourceType'])
+    resource_type = f"{inflection.underscore(simplified['resourceType'])}.yaml"
     assert resource_type in schemas, f"{resource_type} not in schemas"
-    extra_fields = [k for k in simplified if k not in schemas[resource_type]['properties']]
-    assert len(extra_fields) == 0, ('extra_fields_not_in_schema', resource_type, extra_fields)
+    # TODO - extra fields are in $ref, need to resolve
+    # extra_fields = [k for k in simplified if k not in schemas[resource_type]['properties']]
+    # assert len(extra_fields) == 0, ('extra_fields_not_in_schema', resource_type, extra_fields)
 
 
 def _default_json_serializer(obj):
     """JSON Serializer, render decimal and bytes types."""
     if isinstance(obj, decimal.Decimal):
         return float(obj)
     if isinstance(obj, bytes):
@@ -690,15 +691,15 @@
         gen3_config = yaml.load(fp, SafeLoader)
     limit_links = gen3_config['limit_links']
     nested_objects = gen3_config['nested_objects']
 
     with SimplifierContextManager():
         with EmitterContextManager(output_path) as emitter:
             for parse_result in directory_reader(directory_path=input_path, pattern=pattern,
-                                                 validate=False):
+                                                 validate=False, ignore_path=output_path):
                 if parse_result.exception is not None:
                     if 'resourceType' not in str(parse_result.exception):
                         logger.error(f"{parse_result.path} has exception {parse_result.exception}")
                     continue
                 resource = parse_result.resource
 
                 simplified, references = simplify(resource, dialect, nested_objects, transform_ids)
@@ -716,15 +717,15 @@
                 fp.write(orjson.dumps(simplified, default=_default_json_serializer,
                                       option=orjson.OPT_APPEND_NEWLINE).decode())
 
 
 def _debug_once(msg):
     if msg not in LOGGED_ALREADY:
         LOGGED_ALREADY.append(msg)
-        logger.debug(msg)
+        logger.info(msg)
 
 
 def _assert_all_ok(all_ok, parse_result, resource, simplified):
     """Utility, log simplified check problems."""
     if not all_ok:
         reference = f"{resource.resource_type}/{resource.id}"
         logger.warning(f"{parse_result.path} {reference} {parse_result.offset}")
```

### Comparing `iceberg_tools-0.0.3/iceberg_tools/data/simplifier/oid_lookup.py` & `iceberg_tools-0.0.4rc1/iceberg_tools/data/simplifier/oid_lookup.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.3/iceberg_tools/schema/__init__.py` & `iceberg_tools-0.0.4rc1/iceberg_tools/schema/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             del stats[existing_stat_property]
             existing_stat_property += f".{embedded_class.__name__}"
             stats[existing_stat_property] = property_count + len(list(embedded_class.element_properties()))
     else:
         stats[stat_property] += 1
 
 
-def _extract_schemas(classes: List[type], base_uri: str) -> dict:
+def extract_schemas(classes: List[type], base_uri: str) -> dict:
     """Get json schema for all classes."""
     schemas = {}
     for klass in classes:
         schema = klass.schema()
 
         assert 'title' in schema, schema
         schema['$id'] = schema['title']
```

### Comparing `iceberg_tools-0.0.3/iceberg_tools/schema/fhir_resources/binding_lookup.py` & `iceberg_tools-0.0.4rc1/iceberg_tools/schema/fhir_resources/binding_lookup.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.3/iceberg_tools/schema/graph.py` & `iceberg_tools-0.0.4rc1/iceberg_tools/schema/graph.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import pathlib
 
 import yaml
 logger = logging.getLogger(__name__)
 
 
-def _bundle_schemas(output_path, base_uri) -> pathlib.Path:
+def bundle_schemas(output_path, base_uri, file_name="graph-fhir.json") -> pathlib.Path:
     """Create a single uber schema in json with all """
     schemas = {
         '$schema': 'https://json-schema.org/draft/2020-12/schema',
         '$id': base_uri,
         '$defs': {},
         'anyOf': []
     }
@@ -18,27 +18,27 @@
     for input_file in output_path.glob('*.yaml'):
 
         if input_file.stem.startswith('_'):
             continue
 
         with open(input_file) as fp:
             schema_str = fp.read()
-            schema_str = schema_str.replace('.yaml', '').replace('$ref: ', f'$ref: {base_uri}/')
+            schema_str = schema_str.replace('.yaml', '').replace('$ref: ', f'$ref: {base_uri}/').replace(f'$ref: {base_uri}/http', '$ref: http')
             schema = yaml.safe_load(schema_str)
 
             if 'title' not in schema:
                 vertex = next(
                     iter([k for k in schema.keys() if not k.startswith('$') and k not in ['description', 'allOf']]), None)
                 _ = schema
                 schema = schema[vertex]
 
             assert 'title' in schema, schema
             schema['$id'] = f"{base_uri}/{schema['title']}"
 
             schemas['$defs'][schema['title']] = schema
             schemas['anyOf'].append({'$ref': f"{base_uri}/{schema['title']}"})
 
-    path = output_path / pathlib.Path("graph-fhir.json")
+    path = output_path / pathlib.Path(file_name)
     with open(path, "w") as fp:
         json.dump(schemas, fp, indent=2)
 
     return path
```

### Comparing `iceberg_tools-0.0.3/iceberg_tools/schema/simplified.py` & `iceberg_tools-0.0.4rc1/iceberg_tools/schema/simplified.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.3/iceberg_tools/schema/simplified_validator.py` & `iceberg_tools-0.0.4rc1/iceberg_tools/schema/simplified_validator.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.3/iceberg_tools/util.py` & `iceberg_tools-0.0.4rc1/iceberg_tools/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,28 +113,32 @@
     pass
 
 
 def directory_reader(
         directory_path: pathlib.Path,
         pattern: str = '*.*',
         parse=True,
-        validate=True) -> Iterator[ParseResult]:
+        validate=True,
+        ignore_path:str =None) -> Iterator[ParseResult]:
     """Extract FHIR resources from directory
 
     Args:
         directory_path (pathlib.Path): directory to read
         pattern (str, optional): glob pattern. Defaults to '*.*'.
         parse (bool, optional): parse FHIR resources. Defaults to True.
         validate (bool, optional): validate FHIR resources. Defaults to True.
+        ignore_path (str, optional): ignore files with this string in path. Defaults to None.
     """
 
     assert directory_path.is_dir(), f"{directory_path.name} is not a directory"
 
     input_files = [_ for _ in directory_path.glob(pattern) if _is_json_file(_.name)]
     for input_file in input_files:
+        if ignore_path is not None and ignore_path in str(input_file):
+            continue
         logger.info(input_file)
         if not input_file.is_file():
             continue
         is_ndjson = _is_ndjson(input_file)
         fp = _to_file(input_file)
         with fp:
             if is_ndjson:
```

### Comparing `iceberg_tools-0.0.3/iceberg_tools.egg-info/PKG-INFO` & `iceberg_tools-0.0.4rc1/iceberg_tools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iceberg-tools
-Version: 0.0.3
+Version: 0.0.4rc1
 Summary: FHIR schemas tools for bioinformatics.
 Home-page: https://github.com/bmeg/iceberg-schema-tools
 Author: https://ellrottlab.org/
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bmeg/iceberg-schema-tools/issues
 Project-URL: Source, https://github.com/bmeg/iceberg-schema-tools
 Keywords: FHIR PFB gen3 bioinformatics graph
```

### Comparing `iceberg_tools-0.0.3/iceberg_tools.egg-info/SOURCES.txt` & `iceberg_tools-0.0.4rc1/iceberg_tools.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -58,8 +58,10 @@
 tests/integration/simplified/test_simplify_task.py
 tests/integration/simplified/test_specimen_plucked_properties.py
 tests/integration/simplified/test_task.py
 tests/unit/__init__.py
 tests/unit/conftest.py
 tests/unit/test_coding_conventions.py
 tests/unit/test_schema.py
-tests/unit/test_simplify.py
+tests/unit/test_simplify.py
+tests/unit/test_swapi.py
+tests/unit/test_url_validate_monkey_patch.py
```

### Comparing `iceberg_tools-0.0.3/setup.py` & `iceberg_tools-0.0.4rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name='iceberg_tools',  # Required
 
     # Versions should comply with PEP 440:
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.3',  # Required
+    version='0.0.4rc1',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='FHIR schemas tools for bioinformatics.',
     # Optional
```

### Comparing `iceberg_tools-0.0.3/tests/integration/data/simplifier/test_simplify.py` & `iceberg_tools-0.0.4rc1/tests/integration/data/simplifier/test_simplify.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,7 +23,34 @@
                     # 'content_md5'
                     expected = set(
                         ['content_attachment_contentType', 'content_attachment_url', 'content_attachment_size',
                          'content_attachment_extension_md5']
                     )
                     actual = set([_ for _ in simplified if _.startswith('content')])
                     assert expected == actual, (file_name, line)
+
+
+def test_simplify_foo():
+    """Ensure we can validate a synthetic study"""
+
+    simplify_directory('tests/fixtures/simplify/foo/', '**/*.*', 'tmp/foo/extractions',
+                       'iceberg/schemas/simplified/simplified-fhir.json', 'PFB', 'config.yaml')
+
+    directory_path = pathlib.Path('tmp/foo/extractions')
+    input_files = [_ for _ in directory_path.glob("*.ndjson")]
+    for file_name in input_files:
+        with open(file_name) as fp:
+            for line in fp.readlines():
+                pfb_ready = orjson.loads(line)
+                simplified = pfb_ready['object']
+                all_ok = all([validate_simplified_value(_) for _ in simplified.values()])
+                print((file_name, line))
+                assert all_ok, (file_name, line)
+                if simplified['resourceType'] == 'DocumentReference':
+                    # 'content_md5'
+                    expected = set(
+                        ['content_attachment_contentType', 'content_attachment_url', 'content_attachment_size',
+                         'content_attachment_extension_md5']
+                    )
+                    actual = set([_ for _ in simplified if _.startswith('content')])
+                    assert expected == actual, (file_name, line)
+                    assert len(pfb_ready['relations']) > 0, "DocumentReference should have relationships"
```

### Comparing `iceberg_tools-0.0.3/tests/integration/data/test_pfb.py` & `iceberg_tools-0.0.4rc1/tests/integration/data/test_pfb.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,65 @@
+import pathlib
+
 from iceberg_tools.data.pfb import SimplePFBWriter
 from iceberg_tools.data.simplifier import simplify_directory
 
 
+def setup_module(module):
+    """Setup the test module"""
+    msg = '\n'.join(
+        [
+            "# please run the following before running this test",
+            "iceberg schema generate simplified --config_path tests/integration/data/config.yaml --output_path tests/integration/data/schemas",
+            "iceberg schema compile simplified --output_path tests/integration/data/schemas"
+        ]
+    )
+    assert pathlib.Path('tests/integration/data/schemas/simplified-fhir.json').exists(), msg
+
+
 def test_studies(caplog, dependency_order):
     """Ensure we can create a pfb file from a synthetic study."""
     simplify_directory('tests/fixtures/simplify/study/', '**/*.*', 'tmp/study/extractions',
-                       'iceberg/schemas/simplified/simplified-fhir.json', 'PFB', 'config.yaml')
+                       'tests/integration/data/schemas/simplified-fhir.json', 'PFB', 'tests/integration/data/config.yaml')
 
-    pfb_writer = SimplePFBWriter(schema_path='iceberg/schemas/simplified/simplified-fhir.json',
+    pfb_writer = SimplePFBWriter(schema_path='tests/integration/data/schemas/simplified-fhir.json',
                                  output_path='tmp/CohesiveDataSet.avro',
                                  dependency_order=dependency_order)
 
     list(pfb_writer.transform_directory('tmp/study/extractions'))
 
     inspection = pfb_writer.inspect()
     assert len(inspection.errors) == 0, "Unexpected errors"
     if len(inspection.warnings) > 0:
         print(inspection.warnings)
 
 
 def test_synthea(caplog, dependency_order):
     """Ensure we can create a pfb file from a synthetic study."""
     simplify_directory('tests/fixtures/simplify/synthea', '**/*.*', 'tmp/synthea/extractions',
-                       'iceberg/schemas/simplified/simplified-fhir.json', 'PFB', 'config.yaml')
+                       'tests/integration/data/schemas/simplified-fhir.json', 'PFB', 'tests/integration/data/config.yaml')
 
-    pfb_writer = SimplePFBWriter(schema_path='iceberg/schemas/simplified/simplified-fhir.json',
+    pfb_writer = SimplePFBWriter(schema_path='tests/integration/data/schemas/simplified-fhir.json',
                                  output_path='tmp/Synthea.avro',
                                  dependency_order=dependency_order)
 
     list(pfb_writer.transform_directory('tmp/synthea/extractions'))
 
     inspection = pfb_writer.inspect()
     assert len(inspection.errors) == 0, "Unexpected errors"
     if len(inspection.warnings) > 0:
         print(inspection.warnings)
 
 
 def test_kf(caplog, dependency_order):
     """Ensure we can create a pfb file from a Kids first study."""
     simplify_directory('tests/fixtures/simplify/kf', '**/*.*', 'tmp/kf/extractions',
-                       'iceberg/schemas/simplified/simplified-fhir.json', 'PFB', 'config.yaml')
+                       'tests/integration/data/schemas/simplified-fhir.json', 'PFB', 'tests/integration/data/config.yaml')
 
-    pfb_writer = SimplePFBWriter(schema_path='iceberg/schemas/simplified/simplified-fhir.json',
+    pfb_writer = SimplePFBWriter(schema_path='tests/integration/data/schemas/simplified-fhir.json',
                                  output_path='tmp/KidsFirst.avro',
                                  dependency_order=dependency_order)
 
     list(pfb_writer.transform_directory('tmp/kf/extractions'))
 
     inspection = pfb_writer.inspect()
     assert len(inspection.errors) == 0, "Unexpected errors"
@@ -53,17 +67,17 @@
         print(inspection.warnings)
 
 
 def test_ncpi(caplog, dependency_order):
     """Ensure we can create a pfb file from a NCPI IG examples."""
 
     simplify_directory('tests/fixtures/simplify/ncpi/examples-5.0', '*.*', 'tmp/ncpi/extractions',
-                       'iceberg/schemas/simplified/simplified-fhir.json', 'PFB', 'config.yaml')
+                       'tests/integration/data/schemas/simplified-fhir.json', 'PFB', 'tests/integration/data/config.yaml')
 
-    pfb_writer = SimplePFBWriter(schema_path='iceberg/schemas/simplified/simplified-fhir.json',
+    pfb_writer = SimplePFBWriter(schema_path='tests/integration/data/schemas/simplified-fhir.json',
                                  output_path='tmp/NCPI.avro',
                                  dependency_order=dependency_order)
 
     list(pfb_writer.transform_directory('tmp/ncpi/extractions'))
 
     inspection = pfb_writer.inspect()
     assert len(inspection.errors) == 0, "Unexpected errors"
@@ -72,17 +86,17 @@
 
 
 def test_genomics_reporting(caplog, dependency_order):
     """Ensure we can create a pfb file from a Genomics Reporting IG examples."""
 
     simplify_directory('tests/fixtures/simplify/genomics-reporting/examples-5.0',
                        '*.*', 'tmp/genomics-reporting/extractions',
-                       'iceberg/schemas/simplified/simplified-fhir.json', 'PFB', 'config.yaml')
+                       'tests/integration/data/schemas/simplified-fhir.json', 'PFB', 'tests/integration/data/config.yaml')
 
-    pfb_writer = SimplePFBWriter(schema_path='iceberg/schemas/simplified/simplified-fhir.json',
+    pfb_writer = SimplePFBWriter(schema_path='tests/integration/data/schemas/simplified-fhir.json',
                                  output_path='tmp/GenomicsReporting.avro',
                                  dependency_order=dependency_order)
 
     list(pfb_writer.transform_directory('tmp/genomics-reporting/extractions'))
 
     inspection = pfb_writer.inspect()
     assert len(inspection.errors) == 0, "Unexpected errors"
@@ -90,17 +104,17 @@
         print(inspection.warnings)
 
 
 def test_dbgap(caplog, dependency_order):
     """Ensure we can create a pfb file from dbGAP examples."""
 
     simplify_directory('tests/fixtures/simplify/dbgap/examples-5.0', '*.*', 'tmp/dbgap/extractions',
-                       'iceberg/schemas/simplified/simplified-fhir.json', 'PFB', 'config.yaml')
+                       'tests/integration/data/schemas/simplified-fhir.json', 'PFB', 'tests/integration/data/config.yaml')
 
-    pfb_writer = SimplePFBWriter(schema_path='iceberg/schemas/simplified/simplified-fhir.json',
+    pfb_writer = SimplePFBWriter(schema_path='tests/integration/data/schemas/simplified-fhir.json',
                                  output_path='tmp/dbGap.avro',
                                  dependency_order=dependency_order)
 
     list(pfb_writer.transform_directory('tmp/dbgap/extractions'))
 
     inspection = pfb_writer.inspect()
     assert len(inspection.errors) == 0, "Unexpected errors"
@@ -108,17 +122,17 @@
         print(inspection.warnings)
 
 
 def test_anvil(caplog, dependency_order):
     """Ensure we can create a pfb file from AnVIL examples."""
 
     simplify_directory('tests/fixtures/simplify/anvil/fhir-5.0/', '**/*.*', 'tmp/anvil/extractions',
-                       'iceberg/schemas/simplified/simplified-fhir.json', 'PFB', 'config.yaml')
+                       'tests/integration/data/schemas/simplified-fhir.json', 'PFB', 'tests/integration/data/config.yaml')
 
-    pfb_writer = SimplePFBWriter(schema_path='iceberg/schemas/simplified/simplified-fhir.json',
+    pfb_writer = SimplePFBWriter(schema_path='tests/integration/data/schemas/simplified-fhir.json',
                                  output_path='tmp/AnVIL.avro',
                                  dependency_order=dependency_order)
 
     list(pfb_writer.transform_directory('tmp/anvil/extractions'))
 
     inspection = pfb_writer.inspect()
     assert len(inspection.errors) == 0, "Unexpected errors"
```

### Comparing `iceberg_tools-0.0.3/tests/integration/graph/__init__.py` & `iceberg_tools-0.0.4rc1/tests/integration/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.3/tests/integration/graph/conftest.py` & `iceberg_tools-0.0.4rc1/tests/integration/graph/conftest.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.3/tests/integration/graph/test_edge_load_granular_reference.py` & `iceberg_tools-0.0.4rc1/tests/integration/graph/test_edge_load_granular_reference.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.3/tests/integration/graph/test_edge_validator.py` & `iceberg_tools-0.0.4rc1/tests/integration/graph/test_edge_validator.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.3/tests/integration/graph/test_invalid_edges.py` & `iceberg_tools-0.0.4rc1/tests/integration/graph/test_invalid_edges.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.3/tests/integration/graph/test_negative_trivial_vertex_load.py` & `iceberg_tools-0.0.4rc1/tests/integration/graph/test_negative_trivial_vertex_load.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.3/tests/integration/graph/test_schema.py` & `iceberg_tools-0.0.4rc1/tests/integration/graph/test_schema.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.3/tests/integration/graph/test_spot_check_embedded_type.py` & `iceberg_tools-0.0.4rc1/tests/integration/graph/test_spot_check_embedded_type.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.3/tests/integration/graph/test_trivial_edge_load.py` & `iceberg_tools-0.0.4rc1/tests/integration/graph/test_trivial_edge_load.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.3/tests/integration/graph/test_trivial_vertex_load.py` & `iceberg_tools-0.0.4rc1/tests/integration/graph/test_trivial_vertex_load.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.3/tests/integration/simplified/conftest.py` & `iceberg_tools-0.0.4rc1/tests/integration/simplified/conftest.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.3/tests/integration/simplified/test_codeable_concept.py` & `iceberg_tools-0.0.4rc1/tests/integration/simplified/test_codeable_concept.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.3/tests/integration/simplified/test_primitive.py` & `iceberg_tools-0.0.4rc1/tests/integration/simplified/test_primitive.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.3/tests/integration/simplified/test_research_study_has_project.py` & `iceberg_tools-0.0.4rc1/tests/integration/simplified/test_research_study_has_project.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.3/tests/integration/simplified/test_simplify_medication.py` & `iceberg_tools-0.0.4rc1/tests/integration/simplified/test_simplify_medication.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.3/tests/integration/simplified/test_simplify_task.py` & `iceberg_tools-0.0.4rc1/tests/integration/simplified/test_simplify_task.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.3/tests/integration/simplified/test_specimen_plucked_properties.py` & `iceberg_tools-0.0.4rc1/tests/integration/simplified/test_specimen_plucked_properties.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.3/tests/unit/test_coding_conventions.py` & `iceberg_tools-0.0.4rc1/tests/unit/test_coding_conventions.py`

 * *Files identical despite different names*

### Comparing `iceberg_tools-0.0.3/tests/unit/test_schema.py` & `iceberg_tools-0.0.4rc1/tests/unit/test_schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 from fhir.resources.documentreference import DocumentReference
 from fhir.resources.patient import Patient, PatientLink, PatientCommunication
 from fhir.resources.task import Task
 
-from iceberg_tools.schema import _find_fhir_classes, _extract_schemas, BASE_URI
+from iceberg_tools.schema import _find_fhir_classes, extract_schemas, BASE_URI
 
 
 def test_find_fhir_classes():
     """Assert we find classes descending from Patient."""
     classes = _find_fhir_classes({'dependency_order': ['Patient']})
     expected_classes = [Patient, PatientLink, PatientCommunication]
     for _ in expected_classes:
         assert _ in classes, ('No find', _)
 
 
 def test_schemas():
     """Assert we find schemas descending from Patient."""
     classes = _find_fhir_classes({'dependency_order': ['Patient']})
-    schemas = _extract_schemas(classes, BASE_URI)
+    schemas = extract_schemas(classes, BASE_URI)
     expected_classes = ['Patient', 'PatientLink', 'PatientCommunication']
     for _ in expected_classes:
         assert _ in schemas, ('No find expected class', _)
 
     patient = schemas['Patient']
     assert patient['$id'] == 'Patient'
     assert 'Disclaimer' not in patient['description'], "Did not edit vertex description"
 
 
 def test_bindings():
     """Ensure bindings are attached to expected properties."""
-    schemas = _extract_schemas([Patient], BASE_URI)
+    schemas = extract_schemas([Patient], BASE_URI)
     patient = schemas['Patient']
     gender = patient['properties']['gender']
     expected_property_attributes = ['type', 'binding_strength', 'binding_description', 'binding_uri', 'enum_values']
     for _ in expected_property_attributes:
         assert _ in gender, ('Did not find binding. Missing attribute in Patient.gender', _)
 
 
 def test_backref():
     """Test simple and itemized backref."""
-    schemas = _extract_schemas([Task], BASE_URI)
+    schemas = extract_schemas([Task], BASE_URI)
     assert 'Task' in schemas, "Should have found Task"
 
     task = schemas['Task']
     expected_references_with_itemized_backref = ['focus', 'owner', 'requester']
     for _ in expected_references_with_itemized_backref:
         assert _ in task['properties'], task['properties'].keys()
         assert task['properties'][_]['backref'] == f'{_}_task', "Should have itemized backref"
     expected_references_with_simple_backref = ['location']
     for _ in expected_references_with_simple_backref:
         assert task['properties'][_]['backref'] == 'task', "Should have simple backref"
 
 
 def test_backref_array():
     """Test simple and itemized backref."""
-    schemas = _extract_schemas([DocumentReference], BASE_URI)
+    schemas = extract_schemas([DocumentReference], BASE_URI)
     assert 'DocumentReference' in schemas, "Should have found DocumentReference"
 
     document_reference = schemas['DocumentReference']
     # select property that is a list of references.
     author = document_reference['properties']['author']
     print(author)
     assert 'backref' in author, "lists of References should have a backref"
 
 
 def test_task():
     """Test CodeableReference."""
-    schemas = _extract_schemas([Task], BASE_URI)
+    schemas = extract_schemas([Task], BASE_URI)
     assert 'Task' in schemas, "Should have found Task"
 
     task = schemas['Task']
     # select property that is a CodeableReference.
     requested_performer = task['properties']['requestedPerformer']
     print(requested_performer)
     assert 'backref' in requested_performer, "requested_performer should have a backref"
```

### Comparing `iceberg_tools-0.0.3/tests/unit/test_simplify.py` & `iceberg_tools-0.0.4rc1/tests/unit/test_simplify.py`

 * *Files identical despite different names*

