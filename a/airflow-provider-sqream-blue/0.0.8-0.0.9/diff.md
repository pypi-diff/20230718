# Comparing `tmp/airflow-provider-sqream-blue-0.0.8.tar.gz` & `tmp/airflow-provider-sqream-blue-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-provider-sqream-blue-0.0.8.tar", last modified: Tue Apr 18 16:03:39 2023, max compression
+gzip compressed data, was "airflow-provider-sqream-blue-0.0.9.tar", last modified: Thu Jul  6 14:11:44 2023, max compression
```

## Comparing `airflow-provider-sqream-blue-0.0.8.tar` & `airflow-provider-sqream-blue-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:03:39.364681 airflow-provider-sqream-blue-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-18 16:02:57.000000 airflow-provider-sqream-blue-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-18 16:03:39.364681 airflow-provider-sqream-blue-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-18 16:02:57.000000 airflow-provider-sqream-blue-0.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:03:39.364681 airflow-provider-sqream-blue-0.0.8/airflow_provider_sqream_blue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-18 16:03:39.000000 airflow-provider-sqream-blue-0.0.8/airflow_provider_sqream_blue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-18 16:03:39.000000 airflow-provider-sqream-blue-0.0.8/airflow_provider_sqream_blue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:03:39.000000 airflow-provider-sqream-blue-0.0.8/airflow_provider_sqream_blue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-18 16:03:39.000000 airflow-provider-sqream-blue-0.0.8/airflow_provider_sqream_blue.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-18 16:03:39.000000 airflow-provider-sqream-blue-0.0.8/airflow_provider_sqream_blue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 16:03:39.000000 airflow-provider-sqream-blue-0.0.8/airflow_provider_sqream_blue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 16:03:39.364681 airflow-provider-sqream-blue-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-18 16:02:57.000000 airflow-provider-sqream-blue-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:03:39.364681 airflow-provider-sqream-blue-0.0.8/sqream_blue/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-18 16:02:57.000000 airflow-provider-sqream-blue-0.0.8/sqream_blue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:03:39.364681 airflow-provider-sqream-blue-0.0.8/sqream_blue/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:02:57.000000 airflow-provider-sqream-blue-0.0.8/sqream_blue/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-04-18 16:02:57.000000 airflow-provider-sqream-blue-0.0.8/sqream_blue/hooks/sqream_blue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:03:39.364681 airflow-provider-sqream-blue-0.0.8/sqream_blue/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:02:57.000000 airflow-provider-sqream-blue-0.0.8/sqream_blue/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-18 16:02:57.000000 airflow-provider-sqream-blue-0.0.8/sqream_blue/operators/sqream_blue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:11:44.485205 airflow-provider-sqream-blue-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-06 14:10:51.000000 airflow-provider-sqream-blue-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-06 14:11:44.485205 airflow-provider-sqream-blue-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-06 14:10:51.000000 airflow-provider-sqream-blue-0.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:11:44.485205 airflow-provider-sqream-blue-0.0.9/airflow_provider_sqream_blue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-06 14:11:44.000000 airflow-provider-sqream-blue-0.0.9/airflow_provider_sqream_blue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-06 14:11:44.000000 airflow-provider-sqream-blue-0.0.9/airflow_provider_sqream_blue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 14:11:44.000000 airflow-provider-sqream-blue-0.0.9/airflow_provider_sqream_blue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-06 14:11:44.000000 airflow-provider-sqream-blue-0.0.9/airflow_provider_sqream_blue.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-06 14:11:44.000000 airflow-provider-sqream-blue-0.0.9/airflow_provider_sqream_blue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 14:11:44.000000 airflow-provider-sqream-blue-0.0.9/airflow_provider_sqream_blue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 14:11:44.485205 airflow-provider-sqream-blue-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-06 14:10:51.000000 airflow-provider-sqream-blue-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:11:44.485205 airflow-provider-sqream-blue-0.0.9/sqream_blue/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-06 14:10:51.000000 airflow-provider-sqream-blue-0.0.9/sqream_blue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:11:44.485205 airflow-provider-sqream-blue-0.0.9/sqream_blue/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:10:51.000000 airflow-provider-sqream-blue-0.0.9/sqream_blue/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-07-06 14:10:51.000000 airflow-provider-sqream-blue-0.0.9/sqream_blue/hooks/sqream_blue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:11:44.485205 airflow-provider-sqream-blue-0.0.9/sqream_blue/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:10:51.000000 airflow-provider-sqream-blue-0.0.9/sqream_blue/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-06 14:10:51.000000 airflow-provider-sqream-blue-0.0.9/sqream_blue/operators/sqream_blue.py
```

### Comparing `airflow-provider-sqream-blue-0.0.8/LICENSE` & `airflow-provider-sqream-blue-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow-provider-sqream-blue-0.0.8/PKG-INFO` & `airflow-provider-sqream-blue-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: airflow-provider-sqream-blue
-Version: 0.0.8
+Version: 0.0.9
 Summary: About Apache Airflow - A platform to programmatically author, schedule, and monitor workflows.
 Home-page: https://github.com/SQream/apache-airflow-providers-sqream-blue
 Author: SQream
 Author-email: info@sqream.com
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -126,9 +125,7 @@
 
 
 The execution of the Dag File -
 
 .. image:: images/execution_dag.png
    :width: 600
  
-
-
```

### Comparing `airflow-provider-sqream-blue-0.0.8/README.rst` & `airflow-provider-sqream-blue-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `airflow-provider-sqream-blue-0.0.8/airflow_provider_sqream_blue.egg-info/PKG-INFO` & `airflow-provider-sqream-blue-0.0.9/airflow_provider_sqream_blue.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: airflow-provider-sqream-blue
-Version: 0.0.8
+Version: 0.0.9
 Summary: About Apache Airflow - A platform to programmatically author, schedule, and monitor workflows.
 Home-page: https://github.com/SQream/apache-airflow-providers-sqream-blue
 Author: SQream
 Author-email: info@sqream.com
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -126,9 +125,7 @@
 
 
 The execution of the Dag File -
 
 .. image:: images/execution_dag.png
    :width: 600
  
-
-
```

### Comparing `airflow-provider-sqream-blue-0.0.8/setup.py` & `airflow-provider-sqream-blue-0.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 """Perform the package sqream_blue-provider setup."""
 setup(
     name='airflow-provider-sqream-blue',
-    version="0.0.8",
+    version="0.0.9",
     description='About Apache Airflow - A platform to programmatically author, schedule, and monitor workflows.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
@@ -23,13 +23,13 @@
     entry_points={
         "apache_airflow_provider": [
             "provider_info=sqream_blue.__init__:get_provider_info"
         ]
     },
     license='Apache License 2.0',
     packages=['sqream_blue', 'sqream_blue.hooks','sqream_blue.operators'],
-    install_requires=['pysqream-blue>=1.0.26', 'apache-airflow>=2.0', 'apache-airflow-providers-common-sql==1.3.2'],
+    install_requires=['pysqream-blue>=1.0.28', 'apache-airflow>=2.6', 'apache-airflow-providers-common-sql==1.3.2'],
     setup_requires=['setuptools', 'wheel'],
     author='SQream',
     author_email='info@sqream.com',
     url='https://github.com/SQream/apache-airflow-providers-sqream-blue',
 )
```

### Comparing `airflow-provider-sqream-blue-0.0.8/sqream_blue/__init__.py` & `airflow-provider-sqream-blue-0.0.9/sqream_blue/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-sqream-blue-0.0.8/sqream_blue/hooks/sqream_blue.py` & `airflow-provider-sqream-blue-0.0.9/sqream_blue/hooks/sqream_blue.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     provider manager from that version.
     """
 
     def dec(func):
         @wraps(func)
         def inner():
             field_behaviors = func()
-            conn_attrs = {"host", "access_token", "port", "extra"}
+            conn_attrs = {"host", "access_token", "pool_name", "port", "extra"}
 
             def _ensure_prefix(field):
                 if field not in conn_attrs and not field.startswith("extra__"):
                     return f"extra__{conn_type}__{field}"
                 else:
                     return field
 
@@ -48,15 +48,16 @@
         """Returns connection widgets to add to connection form"""
         from flask_appbuilder.fieldwidgets import BS3TextFieldWidget
         from flask_babel import lazy_gettext
         from wtforms import StringField
 
         return {
             "database": StringField(lazy_gettext("Database"), widget=BS3TextFieldWidget()),
-            "access_token": StringField(lazy_gettext("Access token"), widget=BS3TextFieldWidget())
+            "access_token": StringField(lazy_gettext("Access token"), widget=BS3TextFieldWidget()),
+            "pool_name": StringField(lazy_gettext("Pool name"), widget=BS3TextFieldWidget())
         }
 
     @staticmethod
     @_ensure_prefixes(conn_type="sqream_blue")
     def get_ui_field_behaviour() -> dict[str, Any]:
         """Returns custom field behaviour"""
         fileds = {
@@ -70,14 +71,15 @@
             "placeholders": fileds,
         }
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.database = kwargs.pop("database", None)
         self.access_token = kwargs.pop("access_token", None)
+        self.pool_name = kwargs.pop("pool_name", None)
         self.query_ids: list[str] = []
 
     def _get_field(self, extra_dict, field_name):
         backcompat_prefix = "extra__sqream_blue__"
         backcompat_key = f"{backcompat_prefix}{field_name}"
         if field_name.startswith("extra__"):
             raise ValueError(
@@ -101,17 +103,19 @@
         One method to fetch connection params as a dict
         used in get_uri() and get_connection()
         """
         conn = self.get_connection(self.sqream_blue_conn_id)  # type: ignore[attr-defined]
         extra_dict = conn.extra_dejson
         database = self._get_field(extra_dict, "database") or "master"
         access_token = self._get_field(extra_dict, "access_token")
+        pool_name = self._get_field(extra_dict, "pool_name")
         conn_config = {
             "host": conn.host,
             "access_token": self.access_token or access_token,
+            "pool_name": self.pool_name or pool_name,
             "database": self.database or database
         }
         return conn_config
 
     def get_conn(self):
         """Returns a sqream_blue.connection object"""
         conn_config = self._get_conn_params()
```

### Comparing `airflow-provider-sqream-blue-0.0.8/sqream_blue/operators/sqream_blue.py` & `airflow-provider-sqream-blue-0.0.9/sqream_blue/operators/sqream_blue.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,21 +11,23 @@
 
     def __init__(
             self,
             *,
             sqream_blue_conn_id: str = "sqream_blue_default",
             database: str | None = None,
             access_token: str | None = None,
+            pool_name: str | None = None,
             **kwargs,
     ) -> None:
-        if any([database]) and any([access_token]):
+        if any([database]) and any([access_token, pool_name]):
             hook_params = kwargs.pop("hook_params", {})
             kwargs["hook_params"] = {
                 "database": database,
                 "access_token": access_token,
+                "pool_name": pool_name
                 **hook_params,
             }
         super().__init__(conn_id=sqream_blue_conn_id, **kwargs)
 
     def _process_output(self, results: list[Any], descriptions: list[Sequence[Sequence] | None]) -> list[Any]:
         validated_descriptions: list[Sequence[Sequence]] = []
         for idx, description in enumerate(descriptions):
```

