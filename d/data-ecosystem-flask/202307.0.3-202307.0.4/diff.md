# Comparing `tmp/data_ecosystem_flask-202307.0.3.tar.gz` & `tmp/data_ecosystem_flask-202307.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_ecosystem_flask-202307.0.3.tar", max compression
+gzip compressed data, was "data_ecosystem_flask-202307.0.4.tar", max compression
```

## Comparing `data_ecosystem_flask-202307.0.3.tar` & `data_ecosystem_flask-202307.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      863 2023-07-17 03:11:53.293704 data_ecosystem_flask-202307.0.3/data_ecosystem_flask/Makefile.ps1
--rw-r--r--   0        0        0     1155 2023-07-17 03:11:53.293704 data_ecosystem_flask-202307.0.3/data_ecosystem_flask/__init__.py
--rw-r--r--   0        0        0    41602 2023-07-17 03:11:53.293704 data_ecosystem_flask-202307.0.3/data_ecosystem_flask/app.py
--rw-r--r--   0        0        0    13216 2023-07-17 03:11:53.293704 data_ecosystem_flask-202307.0.3/data_ecosystem_flask/app_startup.py
--rw-r--r--   0        0        0    28571 2023-07-17 03:11:53.293704 data_ecosystem_flask-202307.0.3/data_ecosystem_flask/install.py
--rw-r--r--   0        0        0     2082 2023-07-17 03:11:53.293704 data_ecosystem_flask-202307.0.3/data_ecosystem_flask/manifest.json
--rw-r--r--   0        0        0    16945 2023-07-17 03:11:53.293704 data_ecosystem_flask-202307.0.3/data_ecosystem_flask/requirements.txt
--rw-r--r--   0        0        0     1572 2023-07-17 03:11:53.293704 data_ecosystem_flask-202307.0.3/data_ecosystem_flask/templates/download.html
--rw-r--r--   0        0        0      432 2023-07-17 03:11:53.293704 data_ecosystem_flask-202307.0.3/data_ecosystem_flask/templates/error.html
--rw-r--r--   0        0        0     2723 2023-07-17 03:11:53.293704 data_ecosystem_flask-202307.0.3/data_ecosystem_flask/templates/log_file.html
--rw-r--r--   0        0        0     1905 2023-07-17 03:11:53.293704 data_ecosystem_flask-202307.0.3/data_ecosystem_flask/templates/upload.html
--rw-r--r--   0        0        0    11357 2023-07-17 03:11:53.333704 data_ecosystem_flask-202307.0.3/license.md
--rw-r--r--   0        0        0     2559 2023-07-17 03:18:42.623935 data_ecosystem_flask-202307.0.3/pyproject.toml
--rw-r--r--   0        0        0    15040 2023-07-17 03:11:53.337704 data_ecosystem_flask-202307.0.3/readme.md
--rw-r--r--   0        0        0      126 2023-07-17 03:11:53.337704 data_ecosystem_flask-202307.0.3/setup.cfg
--rw-r--r--   0        0        0      127 2023-07-17 03:11:53.337704 data_ecosystem_flask-202307.0.3/setup.py
--rw-r--r--   0        0        0     1796 1970-01-01 00:00:00.000000 data_ecosystem_flask-202307.0.3/PKG-INFO
+-rw-r--r--   0        0        0      863 2023-07-18 10:51:23.854973 data_ecosystem_flask-202307.0.4/data_ecosystem_flask/Makefile.ps1
+-rw-r--r--   0        0        0     1155 2023-07-18 10:51:23.854973 data_ecosystem_flask-202307.0.4/data_ecosystem_flask/__init__.py
+-rw-r--r--   0        0        0    42638 2023-07-18 10:51:23.854973 data_ecosystem_flask-202307.0.4/data_ecosystem_flask/app.py
+-rw-r--r--   0        0        0    13336 2023-07-18 10:51:23.854973 data_ecosystem_flask-202307.0.4/data_ecosystem_flask/app_startup.py
+-rw-r--r--   0        0        0    28571 2023-07-18 10:51:23.854973 data_ecosystem_flask-202307.0.4/data_ecosystem_flask/install.py
+-rw-r--r--   0        0        0     2082 2023-07-18 10:51:23.854973 data_ecosystem_flask-202307.0.4/data_ecosystem_flask/manifest.json
+-rw-r--r--   0        0        0    16945 2023-07-18 10:51:23.854973 data_ecosystem_flask-202307.0.4/data_ecosystem_flask/requirements.txt
+-rw-r--r--   0        0        0     1572 2023-07-18 10:51:23.854973 data_ecosystem_flask-202307.0.4/data_ecosystem_flask/templates/download.html
+-rw-r--r--   0        0        0      432 2023-07-18 10:51:23.854973 data_ecosystem_flask-202307.0.4/data_ecosystem_flask/templates/error.html
+-rw-r--r--   0        0        0     2723 2023-07-18 10:51:23.854973 data_ecosystem_flask-202307.0.4/data_ecosystem_flask/templates/log_file.html
+-rw-r--r--   0        0        0     1905 2023-07-18 10:51:23.854973 data_ecosystem_flask-202307.0.4/data_ecosystem_flask/templates/upload.html
+-rw-r--r--   0        0        0    11357 2023-07-18 10:51:23.906975 data_ecosystem_flask-202307.0.4/license.md
+-rw-r--r--   0        0        0     2559 2023-07-18 10:59:22.927276 data_ecosystem_flask-202307.0.4/pyproject.toml
+-rw-r--r--   0        0        0    15040 2023-07-18 10:51:23.910975 data_ecosystem_flask-202307.0.4/readme.md
+-rw-r--r--   0        0        0      126 2023-07-18 10:51:23.910975 data_ecosystem_flask-202307.0.4/setup.cfg
+-rw-r--r--   0        0        0      127 2023-07-18 10:51:23.910975 data_ecosystem_flask-202307.0.4/setup.py
+-rw-r--r--   0        0        0     1796 1970-01-01 00:00:00.000000 data_ecosystem_flask-202307.0.4/PKG-INFO
```

### Comparing `data_ecosystem_flask-202307.0.3/data_ecosystem_flask/Makefile.ps1` & `data_ecosystem_flask-202307.0.4/data_ecosystem_flask/Makefile.ps1`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.3/data_ecosystem_flask/__init__.py` & `data_ecosystem_flask-202307.0.4/data_ecosystem_flask/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.3/data_ecosystem_flask/app.py` & `data_ecosystem_flask-202307.0.4/data_ecosystem_flask/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,116 +1,110 @@
 """
-Flask App exposing JIRA and Alation services via Swagger.
+This module, app.py, serves as the primary entry point to the Program Agnostic Data Ecosystem (PADE) application. It initializes the application and sets up the endpoints for various services, including Alation.
 
-Summary:
-    This Flask app provides endpoints to interact with
-    JIRA and Alation services through a Swagger UI.
+The Alation service is specifically designed to manage and monitor Alation. It provides the following API endpoints:
 
-Returns:
-    None
+    GET /alation/metadata_excel_file_download/{schema_id}: Retrieves an Excel metadata file from Alation based on the provided schema_id.
+    POST /alation/metadata_excel_file_upload: Uploads an Excel metadata file to Alation via direct upload.
+    GET /alation/metadata_json_file_download/{schema_id}: Retrieves a JSON metadata file from Alation based on the provided schema_id.
+    POST /alation/metadata_json_file_upload: Uploads a JSON metadata file to Alation via direct upload.
+
+The module also integrates other services of the PADE, which include CDC Tech Environment service, Azure Key Vault service, CDC Self Service, CDC Admin service, CDC Security service, and Posit service.
+
+Besides, it includes HTTP enforcement, logging, exception handling, metrics reporting to Azure Monitor, and telemetry instrumentation functionalities.
+
+The app is primarily designed to serve as an HTTP server for the PADE, exposing various functionalities as HTTP endpoints for file uploads, downloads, log access, and error presentation.
+
+Usage:
+python app.py
 """
 
-from flask import Flask, send_file, request, render_template, Blueprint, g, jsonify, make_response, Response
-from opentelemetry import trace
-from opentelemetry.instrumentation.flask import FlaskInstrumentor
-from azure.monitor.opentelemetry.exporter import AzureMonitorMetricExporter
-from pathlib import Path
+import sys
+import os
+import time
+import traceback
 from datetime import datetime
-from io import BytesIO
-from pandas import ExcelWriter
-from requests.exceptions import HTTPError
-from openpyxl.utils.exceptions import InvalidFileException
-from flask_restx import Api, Resource, fields, Namespace, reqparse, marshal_with
-from json import JSONDecodeError
-from bs4 import BeautifulSoup
-from data_ecosystem_flask.app_startup import create_api, create_app
+import requests
+import pandas as pd
+import json
+from functools import wraps
 from datetime import datetime
 from werkzeug.datastructures import FileStorage
-from werkzeug.middleware.proxy_fix import ProxyFix
-import traceback
 from requests.exceptions import RequestException
-import requests
-import os
-import time
+from flask import redirect, send_file, request, render_template, Blueprint, g, jsonify, make_response, Response
+from flask_restx import Api, Resource, fields, Namespace, reqparse, marshal_with
+from opentelemetry.instrumentation.flask import FlaskInstrumentor
+from azure.monitor.opentelemetry.exporter import AzureMonitorMetricExporter
+from data_ecosystem_flask.app_startup import create_api, create_app
 
 from data_ecosystem_services.alation_service import (
-    schema as pade_schema,
-    datasource as pade_datasource,
-    tokenendpoint as pade_tokenendpoint,
-    manifest as pade_manifest
+    schema as pade_schema
 )
 from data_ecosystem_services.cdc_tech_environment_service import (
     environment_file as pade_env_file
 )
 from data_ecosystem_services.az_key_vault_service import (
     az_key_vault as pade_az_key_vault
 )
-from data_ecosystem_services.cdc_self_service import (
-    environment_metadata as pade_env_metadata
-)
 from data_ecosystem_services.cdc_admin_service import (
     environment_tracing as pade_env_tracing,
     environment_logging as pade_env_logging
 )
 from data_ecosystem_services.cdc_security_service import (
     security_core as pade_security_core,
 )
-
 from data_ecosystem_services.posit_service import (
     posit_connect as pade_posit_connect
 )
 
-import requests
-import openpyxl
-import pandas as pd
-import csv
-import json
-import sys
-import os
-import logging
-import io
-import importlib
-import base64
-import dotenv
-
-
 TIMEOUT_5_SEC = 5
 TIMEOUT_ONE_MIN = 60
-
 # Get the currently running file name
 SERVICE_NAME = os.path.basename(__file__)
 # Get the parent folder name of the running file
 NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
 
 print(f"SERVICE_NAME:{SERVICE_NAME}")
 print(f"NAMESPACE_NAME: {NAMESPACE_NAME}")
 sys.path.append(os.getcwd())
 app_dir = os.path.dirname(os.path.abspath(__file__))
 sys.path.append(app_dir)
 
-# app.config["PYTHONPATH"] = "../../../data_ecosystem_services/"
-
 app = create_app()
 
-
-@app.before_request
-def before_request():
-    g.base_url = request.url_root
-    g.log_url = g.base_url + "/logs/get_log_file_tail/1000"
-
-
 # Define the blueprint
 cdc_admin_bp = Blueprint('logs', __name__,
                          url_prefix='/logs')
 
 # Define the blueprint
 cdc_files_bp = Blueprint('files', __name__,
                          url_prefix='/files')
 
 
+def enforce_https(function_name):
+    """
+    Decorator function to enforce HTTPS. If a request is made using HTTP,
+    it redirects the request to HTTPS.
+
+    Args:
+        function_name (function): The Flask view function to decorate.
+
+    Returns:
+        function: The decorated function.
+    """
+    @wraps(function_name)
+    def decorated(*args, **kwargs):
+        if request.url.startswith('http://'):
+            url = request.url.replace('http://', 'https://', 1)
+            code = 301
+            return redirect(url, code=code)
+        return function_name(*args, **kwargs)
+    return decorated
+
+
 def get_datetime(entry):
 
     date_string = entry[0]
     if date_string == '0001-01-01 00:00:00':
         # Handle the specific string and return a valid datetime object
         return datetime.min
     try:
@@ -630,14 +624,15 @@
 
 class ConnectApiKeyVerification(Resource):
     """
     A Flask-RESTful resource for handling the verification of API keys.
 
     """
 
+    @enforce_https
     def get(self):
         """
         Verifies the key stored in key vault based on configuration setting: az_kv_posit_connect_secret_key
 
         Returns:
             tuple: A tuple containing the status code and response from the server.
             The response will be in JSON format if possible, otherwise it will be the raw text response.
@@ -667,14 +662,15 @@
 
 class DeploymentBundle(Resource):
     """
     A Flask-RESTful resource for handling POSIT Deployment Bundle.
 
     """
 
+    @enforce_https
     def get(self, content_id, bundle_id):
         """
         Generates DeploymentBundle
 
         Returns:
             tuple: A tuple containing the status code and response from the server.
             The response will be in JSON format if possible, otherwise it will be the raw text response.
@@ -704,14 +700,15 @@
 
 class PythonInformation(Resource):
     """
     A Flask-RESTful resource for handling POSIT Python Information.
 
     """
 
+    @enforce_https
     def get(self):
         """
         Generates python information about POSIT
 
         Returns:
             tuple: A tuple containing the status code and response from the server.
             The response will be in JSON format if possible, otherwise it will be the raw text response.
@@ -742,14 +739,15 @@
 
 class GeneratedManifest(Resource):
     """
     A Flask-RESTful resource for handling POSIT Manifest Generation
 
     """
 
+    @enforce_https
     def get(self):
         """
         Generates manifest JSON
 
         Returns:
             tuple: A tuple containing the status code and response from the server.
             The response will be in JSON format if possible, otherwise it will be the raw text response.
@@ -862,14 +860,15 @@
 
 class PublishManifest(Resource):
     """
     A Flask-RESTful resource for handling POSIT Manifest Publication
 
     """
 
+    @enforce_https
     def get(self):
         """
         Publishes manifest JSON
 
         Returns:
             tuple: A tuple containing the status code and response from the server.
             The response will be in JSON format if possible, otherwise it will be the raw text response.
@@ -922,30 +921,29 @@
 
 class ContentList(Resource):
     """
     A Flask-RESTful resource for handling POSIT Content Lists
 
     """
 
+    @enforce_https
     def get(self):
         """
-        Publishes manifest JSON
+        Retrieves the manifest JSON for the content list.
 
         Returns:
             tuple: A tuple containing the status code and response from the server.
-            The response will be in JSON format if possible, otherwise it will be the raw text response.
+                   The response will be in JSON format if possible, otherwise it will be the raw text response.
         """
 
-        with tracer.start_as_current_span(f"list_conent"):
+        with tracer.start_as_current_span("list_content"):
 
             config = app.cdc_config
 
             posit_connect_base_url = config.get("posit_connect_base_url")
-            az_kv_posit_connect_secret_key = config.get(
-                "az_kv_posit_connect_secret_key")
             connect_api_key = get_posit_api_key()
 
             posit_connect = pade_posit_connect.PositConnect()
 
             status_code, response_content, api_url = posit_connect.list_content(
                 connect_api_key, posit_connect_base_url)
 
@@ -959,14 +957,15 @@
 
 class DeploymentBundleList(Resource):
     """
     A Flask-RESTful resource for handling POSIT Bundle Lists
 
     """
 
+    @enforce_https
     def get(self, content_id):
         """
         Publishes manifest JSON
 
         Returns:
             tuple: A tuple containing the status code and response from the server.
             The response will be in JSON format if possible, otherwise it will be the raw text response.
@@ -996,14 +995,15 @@
 
 class TaskStatus(Resource):
     """
     A Flask-RESTful resource for handling POSIT Bundle Lists
 
     """
 
+    @enforce_https
     def get(self, task_id):
         """
         Gets Task Status
 
         Returns:
             tuple: A tuple containing the status code and response from the server.
             The response will be in JSON format if possible, otherwise it will be the raw text response.
```

### Comparing `data_ecosystem_flask-202307.0.3/data_ecosystem_flask/app_startup.py` & `data_ecosystem_flask-202307.0.4/data_ecosystem_flask/app_startup.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,15 +179,16 @@
     ns_jira = api.namespace(
         "jira",
         description=JIRA_DESCRIPTION,
     )
 
     POSIT_DESCRIPTION = (
         "The POSIT service provides read-only reporting and query services for "
-        "POSIT."
+        "POSIT.  It also provides methods for automated app creation and publication "
+        "of web applications via manifest files."
     )
 
     ns_posit = api.namespace(
         "posit",
         description=POSIT_DESCRIPTION,
     )
```

### Comparing `data_ecosystem_flask-202307.0.3/data_ecosystem_flask/install.py` & `data_ecosystem_flask-202307.0.4/data_ecosystem_flask/install.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.3/data_ecosystem_flask/manifest.json` & `data_ecosystem_flask-202307.0.4/data_ecosystem_flask/manifest.json`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.3/data_ecosystem_flask/requirements.txt` & `data_ecosystem_flask-202307.0.4/data_ecosystem_flask/requirements.txt`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.3/data_ecosystem_flask/templates/download.html` & `data_ecosystem_flask-202307.0.4/data_ecosystem_flask/templates/download.html`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.3/data_ecosystem_flask/templates/log_file.html` & `data_ecosystem_flask-202307.0.4/data_ecosystem_flask/templates/log_file.html`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.3/data_ecosystem_flask/templates/upload.html` & `data_ecosystem_flask-202307.0.4/data_ecosystem_flask/templates/upload.html`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.3/license.md` & `data_ecosystem_flask-202307.0.4/license.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.3/pyproject.toml` & `data_ecosystem_flask-202307.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 [project.urls]
 "Homepage" = "https://test.pypi.org/project/data-ecosystem-services"
 "Documentation" = "https://gift.readthedocs.io"
 "Repository" = "https://github.com/cdcent/data-ecosystem-services"
 
 [tool.poetry]
 name = "data_ecosystem_flask"
-version="202307.0.3"
+version="202307.0.4"
 description = "Program Agnostic Data Ecosystem (PADE) - Flask Web Service"
 authors = ["John Bowyer <zfi4@cdc.gov>"]
 license = "Apache"
 homepage="https://test.pypi.org/project/data-ecosystem-services"
 repository="https://github.com/cdcent/data-ecosystem-services"
 classifiers=[
     "Development Status :: 4 - Beta",
```

### Comparing `data_ecosystem_flask-202307.0.3/readme.md` & `data_ecosystem_flask-202307.0.4/readme.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.3/PKG-INFO` & `data_ecosystem_flask-202307.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-ecosystem-flask
-Version: 202307.0.3
+Version: 202307.0.4
 Summary: Program Agnostic Data Ecosystem (PADE) - Flask Web Service
 Home-page: https://test.pypi.org/project/data-ecosystem-services
 License: Apache
 Author: John Bowyer
 Author-email: zfi4@cdc.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

