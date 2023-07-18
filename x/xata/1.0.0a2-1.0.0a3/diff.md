# Comparing `tmp/xata-1.0.0a2.tar.gz` & `tmp/xata-1.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xata-1.0.0a2.tar", max compression
+gzip compressed data, was "xata-1.0.0a3.tar", max compression
```

## Comparing `xata-1.0.0a2.tar` & `xata-1.0.0a3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11357 2023-07-05 15:15:08.613422 xata-1.0.0a2/LICENSE
--rw-r--r--   0        0        0     1156 2023-07-05 15:15:08.613422 xata-1.0.0a2/README.md
--rw-r--r--   0        0        0      818 2023-07-05 15:15:08.637422 xata-1.0.0a2/pyproject.toml
--rw-r--r--   0        0        0      873 2023-07-05 15:15:08.669422 xata-1.0.0a2/xata/__init__.py
--rw-r--r--   0        0        0      769 2023-07-05 15:15:08.669422 xata-1.0.0a2/xata/api/__init__.py
--rw-r--r--   0        0        0     2694 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/api/authentication.py
--rw-r--r--   0        0        0    12385 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/api/branch.py
--rw-r--r--   0        0        0     7577 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/api/databases.py
--rw-r--r--   0        0        0     8958 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/api/files.py
--rw-r--r--   0        0        0     6103 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/api/invites.py
--rw-r--r--   0        0        0    11716 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/api/migrations.py
--rw-r--r--   0        0        0    12533 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/api/records.py
--rw-r--r--   0        0        0    31571 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/api/search_and_filter.py
--rw-r--r--   0        0        0    12278 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/api/table.py
--rw-r--r--   0        0        0     2544 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/api/users.py
--rw-r--r--   0        0        0     7346 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/api/workspaces.py
--rw-r--r--   0        0        0     2637 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/api_response.py
--rw-r--r--   0        0        0    13637 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/client.py
--rw-r--r--   0        0        0     1188 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/errors.py
--rw-r--r--   0        0        0    15894 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/helpers.py
--rw-r--r--   0        0        0     3077 2023-07-05 15:15:08.673422 xata-1.0.0a2/xata/namespace.py
--rw-r--r--   0        0        0     1869 1970-01-01 00:00:00.000000 xata-1.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-07 13:58:14.054969 xata-1.0.0a3/LICENSE
+-rw-r--r--   0        0        0     1156 2023-07-07 13:58:14.054969 xata-1.0.0a3/README.md
+-rw-r--r--   0        0        0      818 2023-07-07 13:58:14.086971 xata-1.0.0a3/pyproject.toml
+-rw-r--r--   0        0        0      873 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/__init__.py
+-rw-r--r--   0        0        0      769 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/api/__init__.py
+-rw-r--r--   0        0        0     2694 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/api/authentication.py
+-rw-r--r--   0        0        0    12773 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/api/branch.py
+-rw-r--r--   0        0        0     7627 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/api/databases.py
+-rw-r--r--   0        0        0     8958 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/api/files.py
+-rw-r--r--   0        0        0     6103 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/api/invites.py
+-rw-r--r--   0        0        0    12076 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/api/migrations.py
+-rw-r--r--   0        0        0    12641 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/api/records.py
+-rw-r--r--   0        0        0    31571 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/api/search_and_filter.py
+-rw-r--r--   0        0        0    12638 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/api/table.py
+-rw-r--r--   0        0        0     2544 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/api/users.py
+-rw-r--r--   0        0        0     7478 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/api/workspaces.py
+-rw-r--r--   0        0        0     3186 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/api_response.py
+-rw-r--r--   0        0        0    13637 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/client.py
+-rw-r--r--   0        0        0     1188 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/errors.py
+-rw-r--r--   0        0        0    15894 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/helpers.py
+-rw-r--r--   0        0        0     3077 2023-07-07 13:58:14.122972 xata-1.0.0a3/xata/namespace.py
+-rw-r--r--   0        0        0     1869 1970-01-01 00:00:00.000000 xata-1.0.0a3/PKG-INFO
```

### Comparing `xata-1.0.0a2/LICENSE` & `xata-1.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a2/README.md` & `xata-1.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a2/pyproject.toml` & `xata-1.0.0a3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xata"
-version = "1.0.0a2"
+version = "1.0.0a3"
 description = "Python client for Xata.io"
 authors = ["Xata <support@xata.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 documentation = "https://xata-py.readthedocs.io"
 
 [tool.poetry.dependencies]
```

### Comparing `xata-1.0.0a2/xata/__init__.py` & `xata-1.0.0a3/xata/__init__.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a2/xata/api/__init__.py` & `xata-1.0.0a3/xata/api/__init__.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a2/xata/api/authentication.py` & `xata-1.0.0a3/xata/api/authentication.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a2/xata/api/branch.py` & `xata-1.0.0a3/xata/api/branch.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,26 +27,27 @@
 from xata.namespace import Namespace
 
 
 class Branch(Namespace):
 
     scope = "workspace"
 
-    def get_branches(self, db_name: str) -> ApiResponse:
+    def list(self, db_name: str) -> ApiResponse:
         """
         List all available Branches
 
         Path: /dbs/{db_name}
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
         Response: application/json
 
         :param db_name: str The Database Name
 
         :returns ApiResponse
         """
         url_path = f"/dbs/{db_name}"
@@ -60,14 +61,15 @@
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
         Response: application/json
 
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
         :returns ApiResponse
         """
@@ -84,14 +86,15 @@
         Response status codes:
         - 201: Created
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 423: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
         Response: application/json
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
         :param from_: str = None Name of source branch to branch the new schema from
 
@@ -113,14 +116,15 @@
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 409: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
         Response: application/json
 
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
         :returns ApiResponse
         """
@@ -136,14 +140,15 @@
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
         Response: application/json
 
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
         :returns ApiResponse
         """
@@ -159,14 +164,15 @@
         Method: PUT
         Response status codes:
         - 204: No Content
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
         :returns ApiResponse
         """
@@ -183,14 +189,15 @@
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Example response
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
         Response: application/json
 
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
         :returns ApiResponse
         """
@@ -209,14 +216,15 @@
         Path: /dbs/{db_name}/gitBranches
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 5XX: Unexpected Error
+        - default: Unexpected Error
         Response: application/json
 
         :param db_name: str The Database Name
 
         :returns ApiResponse
         """
         url_path = f"/dbs/{db_name}/gitBranches"
@@ -237,14 +245,15 @@
         Method: POST
         Response status codes:
         - 201: Operation was successful with warnings
         - 204: Operation was successful without warnings
         - 400: Bad Request
         - 401: Authentication Error
         - 5XX: Unexpected Error
+        - default: Unexpected Error
         Response: application/json
 
         :param db_name: str The Database Name
         :param payload: dict content
 
         :returns ApiResponse
         """
@@ -263,14 +272,15 @@
         Method: DELETE
         Response status codes:
         - 204: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: The git branch was not found in the mapping
         - 5XX: Unexpected Error
+        - default: Unexpected Error
 
         :param db_name: str The Database Name
         :param git_branch: str The Git Branch to remove from the mapping
 
         :returns ApiResponse
         """
         url_path = f"/dbs/{db_name}/gitBranches"
@@ -294,14 +304,15 @@
         Path: /dbs/{db_name}/resolveBranch
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 5XX: Unexpected Error
+        - default: Unexpected Error
         Response: application/json
 
         :param db_name: str The Database Name
         :param git_branch: str = None The Git Branch
         :param fallback_branch: str = None Default branch to fallback to
 
         :returns ApiResponse
```

### Comparing `xata-1.0.0a2/xata/api/databases.py` & `xata-1.0.0a3/xata/api/databases.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,37 +157,38 @@
         """
         if workspace_id is None:
             workspace_id = self.client.get_workspace_id()
         url_path = f"/workspaces/{workspace_id}/dbs/{db_name}"
         headers = {"content-type": "application/json"}
         return self.request("PATCH", url_path, headers, payload)
 
-    def rename(self, db_name: str, payload: dict, workspace_id: str = None) -> ApiResponse:
+    def rename(self, db_name: str, new_name: str, workspace_id: str = None) -> ApiResponse:
         """
         Change the name of an existing database
 
         Path: /workspaces/{workspace_id}/dbs/{db_name}/rename
         Method: POST
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 422: Example response
         - 423: Example response
         - 5XX: Unexpected Error
         Response: application/json
 
-        :param db_name: str The Database Name
-        :param payload: dict content
+        :param db_name: str Current database name
+        :param new_name: str New database name
         :param workspace_id: str = None The workspace identifier. Default: workspace Id from the client.
 
-        :returns ApiResponse
+        :return Response
         """
         if workspace_id is None:
             workspace_id = self.client.get_workspace_id()
+        payload = {"newName": new_name}
         url_path = f"/workspaces/{workspace_id}/dbs/{db_name}/rename"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def get_regions(self, workspace_id: str = None) -> ApiResponse:
         """
         List regions available to create a database on
```

### Comparing `xata-1.0.0a2/xata/api/files.py` & `xata-1.0.0a3/xata/api/files.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a2/xata/api/invites.py` & `xata-1.0.0a3/xata/api/invites.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a2/xata/api/migrations.py` & `xata-1.0.0a3/xata/api/migrations.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
         Response: application/json
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
         :returns ApiResponse
@@ -64,14 +65,15 @@
         Method: POST
         Response status codes:
         - 200: Example response
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
         :returns ApiResponse
         """
@@ -88,14 +90,15 @@
         Method: POST
         Response status codes:
         - 200: Schema migration response with ID and migration status.
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
         :returns ApiResponse
         """
@@ -112,14 +115,15 @@
         Method: POST
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
         Response: application/json
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
         :returns ApiResponse
@@ -139,14 +143,15 @@
         Method: POST
         Response status codes:
         - 200: Schema comparison response.
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
         :returns ApiResponse
         """
@@ -163,14 +168,15 @@
         Method: POST
         Response status codes:
         - 200: Schema comparison response.
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
         :returns ApiResponse
         """
@@ -187,14 +193,15 @@
         Method: POST
         Response status codes:
         - 200: Schema migration response with ID and migration status.
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
         :returns ApiResponse
         """
@@ -211,14 +218,15 @@
         Method: POST
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
         Response: application/json
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
         :returns ApiResponse
@@ -236,14 +244,15 @@
         Method: POST
         Response status codes:
         - 200: Schema migration response with ID and migration status.
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
         :returns ApiResponse
         """
@@ -266,14 +275,15 @@
         Method: POST
         Response status codes:
         - 200: Schema migration response with ID and migration status.
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
         :returns ApiResponse
         """
```

### Comparing `xata-1.0.0a2/xata/api/records.py` & `xata-1.0.0a3/xata/api/records.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         Method: POST
         Response status codes:
         - 200: Returns the results of a successful transaction.
         - 400: Returns errors from a failed transaction.
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
         Response: application/json
 
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
         :returns ApiResponse
@@ -66,14 +67,15 @@
         Method: POST
         Response status codes:
         - 201: Record ID and metadata
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
 
         :param table_name: str The Table name
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
         :param columns: list = None Column filters
 
@@ -96,14 +98,15 @@
         Method: GET
         Response status codes:
         - 200: Table Record Reponse
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
 
         :param table_name: str The Table name
         :param record_id: str The Record name
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
         :param columns: list = None Column filters
```

### Comparing `xata-1.0.0a2/xata/api/search_and_filter.py` & `xata-1.0.0a3/xata/api/search_and_filter.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a2/xata/api/table.py` & `xata-1.0.0a3/xata/api/table.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         - 201: Created
         - 204: No Content
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 422: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
         Response: application/json
 
         :param table_name: str The Table name
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
         :returns ApiResponse
@@ -66,14 +67,15 @@
         Method: DELETE
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Not Found
         - 5XX: Unexpected Error
+        - default: Unexpected Error
         Response: application/json
 
         :param table_name: str The Table name
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
         :returns ApiResponse
@@ -93,14 +95,15 @@
         Response status codes:
         - 200: Schema migration response with ID and migration status.
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 422: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
 
         :param table_name: str The Table name
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
         :returns ApiResponse
@@ -118,14 +121,15 @@
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
         Response: application/json
 
         :param table_name: str The Table name
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
         :returns ApiResponse
@@ -144,14 +148,15 @@
         - 200: Schema migration response with ID and migration status.
         - 204: No Content
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 409: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
 
         :param table_name: str The Table name
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
         :returns ApiResponse
@@ -171,14 +176,15 @@
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
         Response: application/json
 
         :param table_name: str The Table name
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
         :returns ApiResponse
@@ -196,14 +202,15 @@
         Method: POST
         Response status codes:
         - 200: Schema migration response with ID and migration status.
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
 
         :param table_name: str The Table name
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
         :returns ApiResponse
@@ -223,14 +230,15 @@
         Method: GET
         Response status codes:
         - 200: OK
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
         Response: application/json
 
         :param table_name: str The Table name
         :param column_name: str The Column name
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
@@ -250,14 +258,15 @@
         Method: DELETE
         Response status codes:
         - 200: Schema migration response with ID and migration status.
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
 
         :param table_name: str The Table name
         :param column_name: str The Column name
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
 
         :returns ApiResponse
@@ -277,14 +286,15 @@
         Method: PATCH
         Response status codes:
         - 200: Schema migration response with ID and migration status.
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
+        - default: Unexpected Error
 
         :param table_name: str The Table name
         :param column_name: str The Column name
         :param payload: dict content
         :param db_name: str = None The name of the database to query. Default: database name from the client.
         :param branch_name: str = None The name of the branch to query. Default: branch name from the client.
```

### Comparing `xata-1.0.0a2/xata/api/users.py` & `xata-1.0.0a3/xata/api/users.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a2/xata/api/workspaces.py` & `xata-1.0.0a3/xata/api/workspaces.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from xata.namespace import Namespace
 
 
 class Workspaces(Namespace):
 
     scope = "core"
 
-    def get_workspaces(self) -> ApiResponse:
+    def list(self) -> ApiResponse:
         """
         Retrieve the list of workspaces the user belongs to
 
         Path: /workspaces
         Method: GET
         Response status codes:
         - 200: OK
@@ -47,32 +47,36 @@
 
 
         :returns ApiResponse
         """
         url_path = "/workspaces"
         return self.request("GET", url_path)
 
-    def create(self, payload: dict) -> ApiResponse:
+    def create(self, name: str, slug: str = None) -> ApiResponse:
         """
         Creates a new workspace with the user requesting it as its single owner.
 
         Path: /workspaces
         Method: POST
         Response status codes:
         - 201: Created
         - 400: Bad Request
         - 401: Authentication Error
         - 404: Example response
         - 5XX: Unexpected Error
         Response: application/json
 
-        :param payload: dict content
+        :param name: str Workspace name
+        :param slug: str = None Slug to use
 
-        :returns ApiResponse
+        :return Response
         """
+        payload = {"name": name}
+        if slug:
+            payload["slug"] = slug
         url_path = "/workspaces"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def get(self, workspace_id: str = None) -> ApiResponse:
         """
         Retrieve workspace info from a workspace ID
```

### Comparing `xata-1.0.0a2/xata/api_response.py` & `xata-1.0.0a3/xata/api_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,14 +50,34 @@
     def is_success(self) -> bool:
         """
         Was the request successful?
         :returns bool
         """
         return 200 <= self.status_code < 300
 
+    def get_cursor(self) -> Union[str, None]:
+        """
+        If the response has a cursor, return it
+        :returns str or None
+        """
+        try:
+            return self.response.json()["meta"]["page"]["cursor"]
+        except Exception:
+            return None
+
+    def has_more_results(self) -> bool:
+        """
+        Are there more result pages available?
+        :return bool
+        """
+        try:
+            return self.response.json()["meta"]["page"].get("more", False)
+        except Exception:
+            return False
+
     @deprecation.deprecated(
         deprecated_in="1.0.0a2",
         removed_in="2.0.0",
         details="This method is obsolete as this class directly returns a dict",
     )
     def json(self) -> dict:
         """
```

### Comparing `xata-1.0.0a2/xata/client.py` & `xata-1.0.0a3/xata/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from .api.search_and_filter import SearchAndFilter
 from .api.table import Table
 from .api.users import Users
 from .api.workspaces import Workspaces
 
 # TODO this is a manual task, to keep in sync with pyproject.toml
 # could/should be automated to keep in sync
-__version__ = "1.0.0a2"
+__version__ = "1.0.0a3"
 
 PERSONAL_API_KEY_LOCATION = "~/.config/xata/key"
 DEFAULT_DATA_PLANE_DOMAIN = "xata.sh"
 DEFAULT_CONTROL_PLANE_DOMAIN = "api.xata.io"
 DEFAULT_REGION = "us-east-1"
 DEFAULT_BRANCH_NAME = "main"
 CONFIG_LOCATION = ".xatarc"
```

### Comparing `xata-1.0.0a2/xata/errors.py` & `xata-1.0.0a3/xata/errors.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a2/xata/helpers.py` & `xata-1.0.0a3/xata/helpers.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a2/xata/namespace.py` & `xata-1.0.0a3/xata/namespace.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a2/PKG-INFO` & `xata-1.0.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xata
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: Python client for Xata.io
 License: Apache-2.0
 Author: Xata
 Author-email: support@xata.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

