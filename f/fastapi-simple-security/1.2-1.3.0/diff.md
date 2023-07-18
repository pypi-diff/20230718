# Comparing `tmp/fastapi_simple_security-1.2.tar.gz` & `tmp/fastapi_simple_security-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_simple_security-1.2.tar", max compression
+gzip compressed data, was "fastapi_simple_security-1.3.0.tar", max compression
```

## Comparing `fastapi_simple_security-1.2.tar` & `fastapi_simple_security-1.3.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1062 2022-10-17 23:38:00.608411 fastapi_simple_security-1.2/LICENSE
--rw-r--r--   0        0        0     4425 2022-10-19 06:57:30.427928 fastapi_simple_security-1.2/README.md
--rw-r--r--   0        0        0      196 2022-10-19 06:49:45.600787 fastapi_simple_security-1.2/fastapi_simple_security/__init__.py
--rw-r--r--   0        0        0     2162 2022-10-18 01:56:29.876922 fastapi_simple_security-1.2/fastapi_simple_security/_security_secret.py
--rw-r--r--   0        0        0     8584 2022-10-19 06:51:55.931336 fastapi_simple_security-1.2/fastapi_simple_security/_sqlite_access.py
--rw-r--r--   0        0        0     2750 2022-10-19 06:51:55.931336 fastapi_simple_security-1.2/fastapi_simple_security/endpoints.py
--rw-r--r--   0        0        0     1208 2022-10-18 01:56:29.876922 fastapi_simple_security-1.2/fastapi_simple_security/security_api_key.py
--rw-r--r--   0        0        0      815 2022-10-18 01:56:29.876922 fastapi_simple_security-1.2/pyproject.toml
--rw-r--r--   0        0        0     5265 1970-01-01 00:00:00.000000 fastapi_simple_security-1.2/setup.py
--rw-r--r--   0        0        0     5132 1970-01-01 00:00:00.000000 fastapi_simple_security-1.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-23 07:28:26.536999 fastapi_simple_security-1.3.0/LICENSE
+-rw-r--r--   0        0        0     4734 2023-06-23 10:52:02.660633 fastapi_simple_security-1.3.0/README.md
+-rw-r--r--   0        0        0      248 2023-06-23 09:39:23.372089 fastapi_simple_security-1.3.0/fastapi_simple_security/__init__.py
+-rw-r--r--   0        0        0     2243 2023-07-18 14:04:24.531999 fastapi_simple_security-1.3.0/fastapi_simple_security/_security_secret.py
+-rw-r--r--   0        0        0     8581 2023-06-23 09:39:23.372433 fastapi_simple_security-1.3.0/fastapi_simple_security/_sqlite_access.py
+-rw-r--r--   0        0        0     2750 2023-06-23 07:28:26.537684 fastapi_simple_security-1.3.0/fastapi_simple_security/endpoints.py
+-rw-r--r--   0        0        0     1208 2023-06-23 07:28:26.537763 fastapi_simple_security-1.3.0/fastapi_simple_security/security_api_key.py
+-rw-r--r--   0        0        0      793 2023-07-18 14:06:30.609527 fastapi_simple_security-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5494 1970-01-01 00:00:00.000000 fastapi_simple_security-1.3.0/PKG-INFO
```

### Comparing `fastapi_simple_security-1.2/LICENSE` & `fastapi_simple_security-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_simple_security-1.2/README.md` & `fastapi_simple_security-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # FastAPI simple security
 
 [![codecov](https://codecov.io/github/mrtolkien/fastapi_simple_security/branch/master/graph/badge.svg?token=8VIKJ9J3XF)](https://codecov.io/github/mrtolkien/fastapi_simple_security)
 [![Python Tests](https://github.com/mrtolkien/fastapi_simple_security/actions/workflows/pr_python_tests.yml/badge.svg)](https://github.com/mrtolkien/fastapi_simple_security/actions/workflows/pr_python_tests.yml)
-[![Linting](https://github.com/mrtolkien/fastapi_simple_security/actions/workflows/push_sanity_check.yml/badge.svg)](https://github.com/mrtolkien/fastapi_simple_security/actions/workflows/push_sanity_check.yml)
+[![Linting](https://github.com/mrtolkien/fastapi_simple_security/actions/workflows/push_linting.yml/badge.svg)](https://github.com/mrtolkien/fastapi_simple_security/actions/workflows/push_linting.yml)
+
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![pre-commit enabled][pre-commit badge]][pre-commit project]
+[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white)](https://conventionalcommits.org)
 
 [pre-commit badge]: <https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white>
 [pre-commit project]: <https://pre-commit.com/>
 
 API key based security package for FastAPI, focused on simplicity of use:
 
 - Full functionality out of the box, no configuration required
@@ -75,24 +78,24 @@
 
 ## Configuration
 
 Environment variables:
 
 - `FASTAPI_SIMPLE_SECURITY_SECRET`: Secret administrator key
 
-    - Generated automatically on server startup if not provided
-    - Allows generation of new API keys, revoking of existing ones, and API key usage view
-    - It being compromised compromises the security of the API
+  - Generated automatically on server startup if not provided
+  - Allows generation of new API keys, revoking of existing ones, and API key usage view
+  - It being compromised compromises the security of the API
 
 - `FASTAPI_SIMPLE_SECURITY_HIDE_DOCS`: Whether or not to hide the API key related endpoints from the documentation
 - `FASTAPI_SIMPLE_SECURITY_DB_LOCATION`: Location of the local sqlite database file
-    - `sqlite.db` in the running directory by default
-    - When running the app inside Docker, use a bind mount for persistence
+  - `sqlite.db` in the running directory by default
+  - When running the app inside Docker, use a bind mount for persistence
 - `FAST_API_SIMPLE_SECURITY_AUTOMATIC_EXPIRATION`: Duration, in days, until an API key is deemed expired
-    - 15 days by default
+  - 15 days by default
 
 ## Contributing
 
 ### Setting up python environment
 
 ```shell script
 poetry install
```

### Comparing `fastapi_simple_security-1.2/fastapi_simple_security/_security_secret.py` & `fastapi_simple_security-1.3.0/fastapi_simple_security/_security_secret.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Secret dependency.
 """
 import os
+import secrets
 import uuid
 import warnings
+from typing import Optional
 
 from fastapi import Security
 from fastapi.security import APIKeyHeader
 from starlette.exceptions import HTTPException
 from starlette.status import HTTP_403_FORBIDDEN
 
 
@@ -46,36 +48,36 @@
 SECRET_KEY_NAME = "secret-key"
 
 secret_header = APIKeyHeader(
     name=SECRET_KEY_NAME, scheme_name="Secret header", auto_error=False
 )
 
 
-async def secret_based_security(header_param: str = Security(secret_header)):
+async def secret_based_security(header_param: Optional[str] = Security(secret_header)):
     """
     Args:
         header_param: parsed header field secret_header
 
     Returns:
         True if the authentication was successful
 
     Raises:
         HTTPException if the authentication failed
     """
 
-    # We simply return True if the given secret-key has the right value
-    if header_param == secret.value:
-        return True
-
-    # Error text without header param
     if not header_param:
-        error = "secret_key must be passed as a header field"
+        raise HTTPException(
+            status_code=HTTP_403_FORBIDDEN,
+            detail="secret_key must be passed as a header field",
+        )
 
-    # Error text with wrong header param
-    else:
-        error = (
-            "Wrong secret key. If not set through environment variable \
+    # We simply return True if the given secret-key has the right value
+    if not secrets.compare_digest(header_param, secret.value):
+        raise HTTPException(
+            status_code=HTTP_403_FORBIDDEN,
+            detail="Wrong secret key. If not set through environment variable \
                 'FASTAPI_SIMPLE_SECURITY_SECRET', it was "
-            "generated automatically at startup and appears in the server logs."
+            "generated automatically at startup and appears in the server logs.",
         )
 
-    raise HTTPException(status_code=HTTP_403_FORBIDDEN, detail=error)
+    else:
+        return True
```

### Comparing `fastapi_simple_security-1.2/fastapi_simple_security/_sqlite_access.py` & `fastapi_simple_security-1.3.0/fastapi_simple_security/_sqlite_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,16 +220,16 @@
                 # We return directly
                 return True
 
     def _update_usage(self, api_key: str, usage_count: int):
         with sqlite3.connect(self.db_location) as connection:
             c = connection.cursor()
 
-            # If we get there, this means it’s an active API key that’s in the database.\
-            #   We update the table.
+            # If we get there, this means it’s an active API key that’s in the database
+            #   We update the table
             c.execute(
                 """
             UPDATE fastapi_simple_security
             SET total_queries = ?, latest_query_date = ?
             WHERE api_key = ?
             """,
                 (
```

### Comparing `fastapi_simple_security-1.2/fastapi_simple_security/endpoints.py` & `fastapi_simple_security-1.3.0/fastapi_simple_security/endpoints.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_security-1.2/fastapi_simple_security/security_api_key.py` & `fastapi_simple_security-1.3.0/fastapi_simple_security/security_api_key.py`

 * *Files identical despite different names*

### Comparing `fastapi_simple_security-1.2/pyproject.toml` & `fastapi_simple_security-1.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi_simple_security"
-version = "1.2"
+version = "1.3.0"
 description = "API key-based security for FastAPI"
 authors = ["mrtolkien <gary.mialaret@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/mrtolkien/fastapi_simple_security"
 readme = "README.md"
 
 [tool.poetry.dependencies]
@@ -12,20 +12,19 @@
 # 0.70 is needed to have the TestClient object
 fastapi = ">=0.70"
 # Necessary as older versions don't work on python 3.10
 urllib3 = ">=1.26.12"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0.0"
-black = "^22.3.0"
+httpx = "^0.24.1"
 requests = "^2.26.0"
-pre-commit = "^2.20.0"
-pylint = "^2.15.4"
-isort = "^5.10.1"
 coverage = "^6.5.0"
+black = "^22.3.0"
+ruff = "^0.0.275"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `fastapi_simple_security-1.2/setup.py` & `fastapi_simple_security-1.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,150 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: fastapi-simple-security
+Version: 1.3.0
+Summary: API key-based security for FastAPI
+Home-page: https://github.com/mrtolkien/fastapi_simple_security
+License: MIT
+Author: mrtolkien
+Author-email: gary.mialaret@gmail.com
+Requires-Python: >=3.7.2,<4
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: fastapi (>=0.70)
+Requires-Dist: urllib3 (>=1.26.12)
+Project-URL: Repository, https://github.com/mrtolkien/fastapi_simple_security
+Description-Content-Type: text/markdown
 
-packages = \
-['fastapi_simple_security']
+# FastAPI simple security
 
-package_data = \
-{'': ['*']}
+[![codecov](https://codecov.io/github/mrtolkien/fastapi_simple_security/branch/master/graph/badge.svg?token=8VIKJ9J3XF)](https://codecov.io/github/mrtolkien/fastapi_simple_security)
+[![Python Tests](https://github.com/mrtolkien/fastapi_simple_security/actions/workflows/pr_python_tests.yml/badge.svg)](https://github.com/mrtolkien/fastapi_simple_security/actions/workflows/pr_python_tests.yml)
+[![Linting](https://github.com/mrtolkien/fastapi_simple_security/actions/workflows/push_linting.yml/badge.svg)](https://github.com/mrtolkien/fastapi_simple_security/actions/workflows/push_linting.yml)
 
-install_requires = \
-['fastapi>=0.70', 'urllib3>=1.26.12']
-
-setup_kwargs = {
-    'name': 'fastapi-simple-security',
-    'version': '1.2',
-    'description': 'API key-based security for FastAPI',
-    'long_description': '# FastAPI simple security\n\n[![codecov](https://codecov.io/github/mrtolkien/fastapi_simple_security/branch/master/graph/badge.svg?token=8VIKJ9J3XF)](https://codecov.io/github/mrtolkien/fastapi_simple_security)\n[![Python Tests](https://github.com/mrtolkien/fastapi_simple_security/actions/workflows/pr_python_tests.yml/badge.svg)](https://github.com/mrtolkien/fastapi_simple_security/actions/workflows/pr_python_tests.yml)\n[![Linting](https://github.com/mrtolkien/fastapi_simple_security/actions/workflows/push_sanity_check.yml/badge.svg)](https://github.com/mrtolkien/fastapi_simple_security/actions/workflows/push_sanity_check.yml)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![pre-commit enabled][pre-commit badge]][pre-commit project]\n\n[pre-commit badge]: <https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white>\n[pre-commit project]: <https://pre-commit.com/>\n\nAPI key based security package for FastAPI, focused on simplicity of use:\n\n- Full functionality out of the box, no configuration required\n- API key security with local `sqlite` backend, working with both header and query parameters\n- Default 15 days deprecation for generated API keys\n- Key creation, revocation, renewing, and usage logs handled through administrator endpoints\n- No dependencies, only requiring `FastAPI` and the python standard library\n\nThis module cannot be used for any kind of distributed deployment. It\'s goal is to help have some basic security features\nfor simple one-server API deployments, mostly during development.\n\n## Installation\n\n`pip install fastapi_simple_security`\n\n### Usage\n\n### Creating an application\n\n```python\nfrom fastapi_simple_security import api_key_router, api_key_security\nfrom fastapi import Depends, FastAPI\n\napp = FastAPI()\n\napp.include_router(api_key_router, prefix="/auth", tags=["_auth"])\n\n@app.get("/secure", dependencies=[Depends(api_key_security)])\nasync def secure_endpoint():\n    return {"message": "This is a secure endpoint"}\n```\n\nResulting app is:\n\n![app](images/auth_endpoints.png)\n\n### API key creation through docs\n\nStart your API and check the logs for the automatically generated secret key if you did not provide one through\nenvironment variables.\n\n![secret](images/secret.png)\n\nGo to `/docs` on your API and inform this secret key in the `Authorize/Secret header` box.\nAll the administrator endpoints only support header security to make sure the secret key is not inadvertently\nshared when sharing an URL.\n\n![secret_header](images/secret_header.png)\n\nThen, you can use `/auth/new` to generate a new API key.\n\n![api key](images/new_api_key.png)\n\nAnd finally, you can use this API key to access the secure endpoint.\n\n![secure endpoint](images/secure_endpoint.png)\n\n### API key creation in python\n\nYou can of course automate API key acquisition through python with `requests` and directly querying the endpoints.\n\nIf you do so, you can hide the endpoints from your API documentation with the environment variable\n`FASTAPI_SIMPLE_SECURITY_HIDE_DOCS`.\n\n## Configuration\n\nEnvironment variables:\n\n- `FASTAPI_SIMPLE_SECURITY_SECRET`: Secret administrator key\n\n    - Generated automatically on server startup if not provided\n    - Allows generation of new API keys, revoking of existing ones, and API key usage view\n    - It being compromised compromises the security of the API\n\n- `FASTAPI_SIMPLE_SECURITY_HIDE_DOCS`: Whether or not to hide the API key related endpoints from the documentation\n- `FASTAPI_SIMPLE_SECURITY_DB_LOCATION`: Location of the local sqlite database file\n    - `sqlite.db` in the running directory by default\n    - When running the app inside Docker, use a bind mount for persistence\n- `FAST_API_SIMPLE_SECURITY_AUTOMATIC_EXPIRATION`: Duration, in days, until an API key is deemed expired\n    - 15 days by default\n\n## Contributing\n\n### Setting up python environment\n\n```shell script\npoetry install\npoetry shell\n```\n\n### Setting up pre-commit hooks\n\n```shell script\npre-commit install\n```\n\n### Running tests\n\n```shell script\npytest\n```\n\n### Running the dev environment\n\nThe attached docker image runs a test app on `localhost:8080` with secret key `TEST_SECRET`. Run it with:\n\n```shell script\ndocker-compose build && docker-compose up\n```\n\n## Needed contributions\n\n- More options with sensible defaults\n- Logging per API key?\n- More back-end options for API key storage?\n',
-    'author': 'mrtolkien',
-    'author_email': 'gary.mialaret@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/mrtolkien/fastapi_simple_security',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.2,<4',
-}
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![pre-commit enabled][pre-commit badge]][pre-commit project]
+[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white)](https://conventionalcommits.org)
 
+[pre-commit badge]: <https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white>
+[pre-commit project]: <https://pre-commit.com/>
+
+API key based security package for FastAPI, focused on simplicity of use:
+
+- Full functionality out of the box, no configuration required
+- API key security with local `sqlite` backend, working with both header and query parameters
+- Default 15 days deprecation for generated API keys
+- Key creation, revocation, renewing, and usage logs handled through administrator endpoints
+- No dependencies, only requiring `FastAPI` and the python standard library
+
+This module cannot be used for any kind of distributed deployment. It's goal is to help have some basic security features
+for simple one-server API deployments, mostly during development.
+
+## Installation
+
+`pip install fastapi_simple_security`
+
+### Usage
+
+### Creating an application
+
+```python
+from fastapi_simple_security import api_key_router, api_key_security
+from fastapi import Depends, FastAPI
+
+app = FastAPI()
+
+app.include_router(api_key_router, prefix="/auth", tags=["_auth"])
+
+@app.get("/secure", dependencies=[Depends(api_key_security)])
+async def secure_endpoint():
+    return {"message": "This is a secure endpoint"}
+```
+
+Resulting app is:
+
+![app](images/auth_endpoints.png)
+
+### API key creation through docs
+
+Start your API and check the logs for the automatically generated secret key if you did not provide one through
+environment variables.
+
+![secret](images/secret.png)
+
+Go to `/docs` on your API and inform this secret key in the `Authorize/Secret header` box.
+All the administrator endpoints only support header security to make sure the secret key is not inadvertently
+shared when sharing an URL.
+
+![secret_header](images/secret_header.png)
+
+Then, you can use `/auth/new` to generate a new API key.
+
+![api key](images/new_api_key.png)
+
+And finally, you can use this API key to access the secure endpoint.
+
+![secure endpoint](images/secure_endpoint.png)
+
+### API key creation in python
+
+You can of course automate API key acquisition through python with `requests` and directly querying the endpoints.
+
+If you do so, you can hide the endpoints from your API documentation with the environment variable
+`FASTAPI_SIMPLE_SECURITY_HIDE_DOCS`.
+
+## Configuration
+
+Environment variables:
+
+- `FASTAPI_SIMPLE_SECURITY_SECRET`: Secret administrator key
+
+  - Generated automatically on server startup if not provided
+  - Allows generation of new API keys, revoking of existing ones, and API key usage view
+  - It being compromised compromises the security of the API
+
+- `FASTAPI_SIMPLE_SECURITY_HIDE_DOCS`: Whether or not to hide the API key related endpoints from the documentation
+- `FASTAPI_SIMPLE_SECURITY_DB_LOCATION`: Location of the local sqlite database file
+  - `sqlite.db` in the running directory by default
+  - When running the app inside Docker, use a bind mount for persistence
+- `FAST_API_SIMPLE_SECURITY_AUTOMATIC_EXPIRATION`: Duration, in days, until an API key is deemed expired
+  - 15 days by default
+
+## Contributing
+
+### Setting up python environment
+
+```shell script
+poetry install
+poetry shell
+```
+
+### Setting up pre-commit hooks
+
+```shell script
+pre-commit install
+```
+
+### Running tests
+
+```shell script
+pytest
+```
+
+### Running the dev environment
+
+The attached docker image runs a test app on `localhost:8080` with secret key `TEST_SECRET`. Run it with:
+
+```shell script
+docker-compose build && docker-compose up
+```
+
+## Needed contributions
+
+- More options with sensible defaults
+- Logging per API key?
+- More back-end options for API key storage?
 
-setup(**setup_kwargs)
```

