# Comparing `tmp/dbt_metricflow-0.0.2.tar.gz` & `tmp/dbt_metricflow-0.0.3.tar.gz`

## Comparing `dbt_metricflow-0.0.2.tar` & `dbt_metricflow-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 dbt_metricflow-0.0.2/.gitignore
--rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 dbt_metricflow-0.0.2/LICENSE
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 dbt_metricflow-0.0.2/README.md
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 dbt_metricflow-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 dbt_metricflow-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 dbt_metricflow-0.0.3/.gitignore
+-rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 dbt_metricflow-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 dbt_metricflow-0.0.3/README.md
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 dbt_metricflow-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 dbt_metricflow-0.0.3/PKG-INFO
```

### Comparing `dbt_metricflow-0.0.2/.gitignore` & `dbt_metricflow-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_metricflow-0.0.2/LICENSE` & `dbt_metricflow-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_metricflow-0.0.2/README.md` & `dbt_metricflow-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dbt_metricflow-0.0.2/pyproject.toml` & `dbt_metricflow-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling~=1.14.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dbt-metricflow"
-version = "0.0.2"
+version = "0.0.3"
 description = "Execute commands against the MetricFlow semantic layer with dbt."
 readme = "README.md"
 requires-python = ">=3.8,<3.10"
 license = "BUSL-1.1"
 authors = [
   { name = "dbt Labs", email = "info@dbtlabs.com" },
 ]
@@ -18,16 +18,16 @@
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "dbt-core==1.6.0b6",
-  "metricflow==0.200.0.dev10"
+  "dbt-core~=1.6.0rc1",
+  "metricflow==0.200.0.dev13"
 ]
 
 [project.optional-dependencies]
 postgres = [
   "dbt-postgres>=1.6.0b6"
 ]
 snowflake = [
```

### Comparing `dbt_metricflow-0.0.2/PKG-INFO` & `dbt_metricflow-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: dbt-metricflow
-Version: 0.0.2
+Version: 0.0.3
 Summary: Execute commands against the MetricFlow semantic layer with dbt.
 Author-email: dbt Labs <info@dbtlabs.com>
 License-Expression: BUSL-1.1
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: <3.10,>=3.8
-Requires-Dist: dbt-core==1.6.0b6
-Requires-Dist: metricflow==0.200.0.dev10
+Requires-Dist: dbt-core~=1.6.0rc1
+Requires-Dist: metricflow==0.200.0.dev13
 Provides-Extra: postgres
 Requires-Dist: dbt-postgres>=1.6.0b6; extra == 'postgres'
 Provides-Extra: snowflake
 Requires-Dist: dbt-snowflake>=1.6.0b3; extra == 'snowflake'
 Description-Content-Type: text/markdown
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: dbt-metricflow Version: 0.0.2 Summary: Execute
+Metadata-Version: 2.1 Name: dbt-metricflow Version: 0.0.3 Summary: Execute
 commands against the MetricFlow semantic layer with dbt. Author-email: dbt Labs
 dbtlabs.com> License-Expression: BUSL-1.1 License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Requires-Python: <3.10,>=3.8 Requires-Dist: dbt-
-core==1.6.0b6 Requires-Dist: metricflow==0.200.0.dev10 Provides-Extra: postgres
-Requires-Dist: dbt-postgres>=1.6.0b6; extra == 'postgres' Provides-Extra:
-snowflake Requires-Dist: dbt-snowflake>=1.6.0b3; extra == 'snowflake'
+core~=1.6.0rc1 Requires-Dist: metricflow==0.200.0.dev13 Provides-Extra:
+postgres Requires-Dist: dbt-postgres>=1.6.0b6; extra == 'postgres' Provides-
+Extra: snowflake Requires-Dist: dbt-snowflake>=1.6.0b3; extra == 'snowflake'
 Description-Content-Type: text/markdown
                     [https://img.shields.io/twitter/follow/
  dbt_labs?labelColor=image.png&color=163B36&logo=twitter&style=flat] [https://
     img.shields.io/badge/Slack-join-163B36] [https://img.shields.io/badge/
                         code%20style-black-000000.svg]
 # Welcome to dbt-metricflow This repo encapsulates the dbt-core, MetricFlow,
 and supported dbt-adapters packages. This package will manage the versioning
```

