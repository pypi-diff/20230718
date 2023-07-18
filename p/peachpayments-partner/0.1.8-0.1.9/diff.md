# Comparing `tmp/peachpayments-partner-0.1.8.tar.gz` & `tmp/peachpayments-partner-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peachpayments-partner-0.1.8.tar", max compression
+gzip compressed data, was "peachpayments-partner-0.1.9.tar", max compression
```

## Comparing `peachpayments-partner-0.1.8.tar` & `peachpayments-partner-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1088 2022-05-19 05:10:59.392757 peachpayments-partner-0.1.8/LICENSE.txt
--rw-r--r--   0        0        0     3769 2022-05-19 05:10:59.392757 peachpayments-partner-0.1.8/README.md
--rw-r--r--   0        0        0       22 2022-05-19 05:10:59.392757 peachpayments-partner-0.1.8/peachpayments_partner/__init__.py
--rw-r--r--   0        0        0     5337 2022-05-19 05:10:59.392757 peachpayments-partner-0.1.8/peachpayments_partner/authentication.py
--rw-r--r--   0        0        0      243 2022-05-19 05:10:59.392757 peachpayments-partner-0.1.8/peachpayments_partner/config.py
--rw-r--r--   0        0        0     2634 2022-05-19 05:10:59.392757 peachpayments-partner-0.1.8/peachpayments_partner/error_response.py
--rw-r--r--   0        0        0      245 2022-05-19 05:10:59.392757 peachpayments-partner-0.1.8/peachpayments_partner/exceptions.py
--rw-r--r--   0        0        0     7452 2022-05-19 05:10:59.392757 peachpayments-partner-0.1.8/peachpayments_partner/fixtures.py
--rw-r--r--   0        0        0     1354 2022-05-19 05:10:59.392757 peachpayments-partner-0.1.8/peachpayments_partner/jwt_formatter.py
--rw-r--r--   0        0        0    17858 2022-05-19 05:10:59.392757 peachpayments-partner-0.1.8/peachpayments_partner/result_codes.py
--rw-r--r--   0        0        0     1376 2022-05-19 05:10:59.396757 peachpayments-partner-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     4771 2022-05-19 05:23:36.380003 peachpayments-partner-0.1.8/setup.py
--rw-r--r--   0        0        0     4963 2022-05-19 05:23:36.380682 peachpayments-partner-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1088 2022-06-15 17:40:18.900100 peachpayments-partner-0.1.9/LICENSE.txt
+-rw-r--r--   0        0        0     3769 2022-06-15 17:40:18.900100 peachpayments-partner-0.1.9/README.md
+-rw-r--r--   0        0        0       22 2022-06-15 17:47:43.514103 peachpayments-partner-0.1.9/peachpayments_partner/__init__.py
+-rw-r--r--   0        0        0     5337 2022-06-15 17:40:18.900100 peachpayments-partner-0.1.9/peachpayments_partner/authentication.py
+-rw-r--r--   0        0        0      243 2022-06-15 17:40:18.900100 peachpayments-partner-0.1.9/peachpayments_partner/config.py
+-rw-r--r--   0        0        0     2634 2022-06-15 17:40:18.900100 peachpayments-partner-0.1.9/peachpayments_partner/error_response.py
+-rw-r--r--   0        0        0      245 2022-06-15 17:40:18.900100 peachpayments-partner-0.1.9/peachpayments_partner/exceptions.py
+-rw-r--r--   0        0        0     7452 2022-06-15 17:40:18.904100 peachpayments-partner-0.1.9/peachpayments_partner/fixtures.py
+-rw-r--r--   0        0        0     1354 2022-06-15 17:40:18.904100 peachpayments-partner-0.1.9/peachpayments_partner/jwt_formatter.py
+-rw-r--r--   0        0        0    17858 2022-06-15 17:40:18.904100 peachpayments-partner-0.1.9/peachpayments_partner/result_codes.py
+-rw-r--r--   0        0        0     1382 2022-06-15 17:47:43.514103 peachpayments-partner-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4771 2022-06-15 17:58:12.056661 peachpayments-partner-0.1.9/setup.py
+-rw-r--r--   0        0        0     4963 2022-06-15 17:58:12.057264 peachpayments-partner-0.1.9/PKG-INFO
```

### Comparing `peachpayments-partner-0.1.8/LICENSE.txt` & `peachpayments-partner-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `peachpayments-partner-0.1.8/README.md` & `peachpayments-partner-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `peachpayments-partner-0.1.8/peachpayments_partner/authentication.py` & `peachpayments-partner-0.1.9/peachpayments_partner/authentication.py`

 * *Files identical despite different names*

### Comparing `peachpayments-partner-0.1.8/peachpayments_partner/error_response.py` & `peachpayments-partner-0.1.9/peachpayments_partner/error_response.py`

 * *Files identical despite different names*

### Comparing `peachpayments-partner-0.1.8/peachpayments_partner/fixtures.py` & `peachpayments-partner-0.1.9/peachpayments_partner/fixtures.py`

 * *Files identical despite different names*

### Comparing `peachpayments-partner-0.1.8/peachpayments_partner/jwt_formatter.py` & `peachpayments-partner-0.1.9/peachpayments_partner/jwt_formatter.py`

 * *Files identical despite different names*

### Comparing `peachpayments-partner-0.1.8/peachpayments_partner/result_codes.py` & `peachpayments-partner-0.1.9/peachpayments_partner/result_codes.py`

 * *Files identical despite different names*

### Comparing `peachpayments-partner-0.1.8/pyproject.toml` & `peachpayments-partner-0.1.9/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peachpayments-partner"
-version = "0.1.8"
+version = "0.1.9"
 description = "PeachPayments Partner Library is a platform agnostic Python package to help integrating PeachPayments with their partners."
 readme = "README.md"
 license = "MIT"
 authors = ["PeachPayments <support@peachpayments.com>"]
 repository = "https://gitlab.com/peachpayments/peach-partner-python/"
 classifiers = [
   "Development Status :: 4 - Beta",
@@ -14,37 +14,37 @@
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Utilities",
   "Typing :: Typed"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-iso4217 = "^1.6.20180829"
-requests = "^2.26.0"
-cryptography = "^36.0.0"
-PyJWT = "^2.3.0"
+iso4217 = "^1.9.20220401"
+requests = "^2.28.0"
+cryptography = "^37.0.2"
+PyJWT = "^2.4.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^5.2"
-mypy = "^0.942"
-flake8 = "^3.9.2"
 autoflake = "^1.4"
 black = "^22.3.0"
-isort = "^5.9.1"
-pytest-cov = "^2.12.1"
-pytest-mypy = "^0.8.1"
 pydocstyle = "^6.1.1"
-freezegun = "^1.1.0"
-types-freezegun = "^1.1.0"
-pre-commit = "^2.15.0"
 mock = "^4.0.3"
-types-mock = "^4.0.1"
-types-requests = "^2.25.6"
-Sphinx = "4.2.0"
 sphinx-rtd-theme = "^1.0.0"
+pytest = "^7.1.2"
+mypy = "^0.961"
+flake8 = "^4.0.1"
+isort = "^5.10.1"
+pytest-cov = "^3.0.0"
+pytest-mypy = "^0.9.1"
+freezegun = "^1.2.1"
+types-freezegun = "^1.1.10"
+pre-commit = "^2.19.0"
+types-mock = "^4.0.15"
+types-requests = "^2.27.30"
+Sphinx = "^5.0.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `peachpayments-partner-0.1.8/setup.py` & `peachpayments-partner-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 packages = \
 ['peachpayments_partner']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['PyJWT>=2.3.0,<3.0.0',
- 'cryptography>=36.0.0,<37.0.0',
- 'iso4217>=1.6.20180829,<2.0.0',
- 'requests>=2.26.0,<3.0.0']
+['PyJWT>=2.4.0,<3.0.0',
+ 'cryptography>=37.0.2,<38.0.0',
+ 'iso4217>=1.9.20220401,<2.0.0',
+ 'requests>=2.28.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'peachpayments-partner',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'PeachPayments Partner Library is a platform agnostic Python package to help integrating PeachPayments with their partners.',
     'long_description': '# Peach Partner Library\n\n## Overview\n\n**Peach Partner Library** is a platform-agnostic Python package to help Payment Service Providers in integrating with PeachPayments.\n\n**Documentation**:\n\n**Source Code**: <https://gitlab.com/peachpayments/peach-partner-python/>\n\n* * *\n\n### Key terms\n\n| Term                     | Definition                                                                                                         |\n| ------------------------ | ------------------------------------------------------------------------------------------------------------------ |\n| Partner API              | A service provided by Peach Payments to enable Payment Service Providers to become available on the Peach Platform |\n| Payment Service Provider | A payment service provider who integrates with the Partner API                                                     |\n| Outbound API call        | API calls sent from Partner API to the Payment Service Provider                                                    |\n| Inbound API call         | API calls sent from Payment Service Provider to Partner API                                                        |\n\n## Installation\n\nPackage requires Python 3.9+\n\n```sh\n# pip\n$ pip3 install peachpayments-partner\n```\n\n```sh\n# poetry\n$ poetry add peachpayments-partner\n```\n\n## Result codes\n\n```python\nfrom peachpayments_partner.result_codes import result_codes\n\nresult_codes.TRANSACTION_SUCCEEDED.code == "000.000.000"\nresult_codes.get("000.000.000").name == "TRANSACTION_SUCCEEDED"\nresult_codes.get("000.000.000").description == "Transaction succeeded"\n```\n\n## Authentication\n\n### Requests to Payment Service Provider\n\nPeachPayments uses an authorization token (JWT) in each request made to the Payment Service Provider.\nThis library provides the `authentication.is_authenticated` method, which takes the token as an argument and the `authentication.get_key` to collect the signing_key.\n\nThe `is_authenticated` method has only one required argument, the token. If it\'s called without the optional `signing_key` it will collect the key using the `get_key` method. If it\'s called without the optional `audience` it will try to use the environment variable `AUTH0_AUDIENCE`.\n\nThe method decodes the token. If that succeeds, it returns `True`. Otherwise, it raises an `AuthError` exception.\n\n## Formatting error responses\n\nPeachPayments requires the error responses to be formatted in a specific way. This library provides the `format_error_response` method, which takes a dict containing error response as an argument and returns a formatted error response.\n\n```python\ndef format_error_response(code, errors, data):\n```\nThe `errors` dict might look like this:\n\n```python\n{\n    "status": ["Not a valid string."],\n    "code": ["Missing data for required field."],\n}\n```\n\nThe `data` dict might look like this:\n\n```python\n{\n  "status": 10\n}\n```\n\nWith the `code` as `ResultCodes.INVALID_OR_MISSING_PARAMETER`, the formatted error response will look similar to this:\n\n```python\n{\n    "result": {\n      "code": "200.300.404",\n      "description": "invalid or missing parameter",\n      "parameterErrors": [\n          {\n              "value": 10,\n              "name": "status",\n              "message": "Not a valid string."\n          },\n          {\n              "name": "code",\n              "message": "Missing data for required field."\n          }\n      ]\n  },\n  "timestamp": "2021-08-03T16:16:30.992618Z"\n}\n```\n\n## Fixtures\n\nThis library provides examples of valid requests and responses.\n\nAn example of the recommended usage for testing:\n\n```python\nimport pytest\nfrom copy import deepcopy\nfrom peachpayments_partner.fixtures import DEBIT_RESPONSE\n\n@pytest.fixture\ndef debit_response():\n    return deepcopy(DEBIT_RESPONSE)\n```',
     'author': 'PeachPayments',
     'author_email': 'support@peachpayments.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.com/peachpayments/peach-partner-python/',
```

### Comparing `peachpayments-partner-0.1.8/PKG-INFO` & `peachpayments-partner-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peachpayments-partner
-Version: 0.1.8
+Version: 0.1.9
 Summary: PeachPayments Partner Library is a platform agnostic Python package to help integrating PeachPayments with their partners.
 Home-page: https://gitlab.com/peachpayments/peach-partner-python/
 License: MIT
 Author: PeachPayments
 Author-email: support@peachpayments.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -14,18 +14,18 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Dist: PyJWT (>=2.3.0,<3.0.0)
-Requires-Dist: cryptography (>=36.0.0,<37.0.0)
-Requires-Dist: iso4217 (>=1.6.20180829,<2.0.0)
-Requires-Dist: requests (>=2.26.0,<3.0.0)
+Requires-Dist: PyJWT (>=2.4.0,<3.0.0)
+Requires-Dist: cryptography (>=37.0.2,<38.0.0)
+Requires-Dist: iso4217 (>=1.9.20220401,<2.0.0)
+Requires-Dist: requests (>=2.28.0,<3.0.0)
 Project-URL: Repository, https://gitlab.com/peachpayments/peach-partner-python/
 Description-Content-Type: text/markdown
 
 # Peach Partner Library
 
 ## Overview
```

