# Comparing `tmp/salesforce-tools-0.1.9.tar.gz` & `tmp/salesforce_tools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salesforce-tools-0.1.9.tar", max compression
+gzip compressed data, was "salesforce_tools-0.2.0.tar", max compression
```

## Comparing `salesforce-tools-0.1.9.tar` & `salesforce_tools-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0      821 2022-09-25 00:51:07.339524 salesforce-tools-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      545 2022-09-25 00:50:43.720137 salesforce-tools-0.1.9/salesforce_tools/__init__.py
--rw-r--r--   0        0        0     6460 2022-09-06 00:27:08.955178 salesforce-tools-0.1.9/salesforce_tools/auth.py
--rw-r--r--   0        0        0     6280 2022-09-03 22:52:28.858802 salesforce-tools-0.1.9/salesforce_tools/bulk.py
--rw-r--r--   0        0        0     5879 2022-09-05 02:34:33.026876 salesforce-tools-0.1.9/salesforce_tools/bulk_models.py
--rw-r--r--   0        0        0     1519 2022-08-28 19:09:24.339050 salesforce-tools-0.1.9/salesforce_tools/oauth_server.py
--rw-r--r--   0        0        0    81520 2022-09-25 00:35:32.399290 salesforce-tools-0.1.9/salesforce_tools/salesforce.py
--rw-r--r--   0        0        0     1511 2022-09-03 22:40:31.857193 salesforce-tools-0.1.9/salesforce_tools/util.py
--rw-r--r--   0        0        0      895 2022-09-25 00:51:17.260267 salesforce-tools-0.1.9/setup.py
--rw-r--r--   0        0        0      844 2022-09-25 00:51:17.260443 salesforce-tools-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0      838 2023-07-18 18:11:24.446289 salesforce_tools-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      548 2023-02-19 15:59:55.189773 salesforce_tools-0.2.0/salesforce_tools/__init__.py
+-rw-r--r--   0        0        0      207 2022-12-03 15:34:19.193841 salesforce_tools-0.2.0/salesforce_tools/async_sf/__init__.py
+-rw-r--r--   0        0        0     3862 2023-06-23 19:31:44.774633 salesforce_tools-0.2.0/salesforce_tools/async_sf/client.py
+-rw-r--r--   0        0        0     3227 2023-02-18 15:51:24.662020 salesforce_tools-0.2.0/salesforce_tools/async_sf/metadata.py
+-rw-r--r--   0        0        0     7544 2022-12-01 15:42:09.307115 salesforce_tools-0.2.0/salesforce_tools/auth.py
+-rw-r--r--   0        0        0     6263 2023-06-29 17:05:59.004227 salesforce_tools-0.2.0/salesforce_tools/bulk.py
+-rw-r--r--   0        0        0     5882 2023-06-29 17:05:16.303395 salesforce_tools-0.2.0/salesforce_tools/bulk_models.py
+-rw-r--r--   0        0        0     1612 2022-11-12 16:32:21.055825 salesforce_tools-0.2.0/salesforce_tools/oauth_server.py
+-rw-r--r--   0        0        0    82405 2023-06-29 17:06:14.252247 salesforce_tools-0.2.0/salesforce_tools/salesforce.py
+-rw-r--r--   0        0        0     1879 2023-06-25 06:39:25.160760 salesforce_tools-0.2.0/salesforce_tools/util.py
+-rw-r--r--   0        0        0      986 1970-01-01 00:00:00.000000 salesforce_tools-0.2.0/setup.py
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 salesforce_tools-0.2.0/PKG-INFO
```

### Comparing `salesforce-tools-0.1.9/pyproject.toml` & `salesforce_tools-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 [tool.poetry]
 name = "salesforce-tools"
-version = "0.1.9"
+version = "0.2.0"
 description = "Salesforce API tools"
 authors = ["David Manuel <david@dcmanjr.com>"]
 license = "MIT"
 homepage = "https://github.com/dacmanj/salesforce-tools"
 repository = "https://github.com/dacmanj/salesforce-tools"
 
 [tool.poetry.dependencies]
-python = "^3.10"
-pandas = "^1.4.3"
+python = "^3.8"
 requests = "^2.28.1"
 requests-oauthlib = "^1.3.1"
 Flask = "^2.2.1"
 xmltodict = "^0.13.0"
-pydantic = "^1.9.2"
 flatten-json = "^0.1.13"
 PyJWT = "^2.4.0"
-cryptography = "^37.0.4"
+cryptography = "^41.0.2"
+authlib = "^1.1.0"
+httpx = "^0.24.1"
+pydantic = "^2.0"
+python-dateutil = "^2.8.2"
 
 [tool.poetry.dev-dependencies]
-viztracer = "^0.15.3"
+viztracer = "^0.15.6"
 pytest-faker = "^2.0.0"
-pytest = "^7.1.2"
+pytest = "^7.2.1"
 Faker = "^13.15.1"
 StringGenerator = "^0.4.4"
 pytest-mock = "^3.8.2"
 requests-mock = "^1.9.3"
-python-dotenv = "^0.20.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `salesforce-tools-0.1.9/salesforce_tools/__init__.py` & `salesforce_tools-0.2.0/salesforce_tools/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 from salesforce_tools.salesforce import SalesforceAPI, SalesforceModelFactory, RestAPI, ToolingAPI
-from salesforce_tools.auth import login, SalesforceOAuthClient, SalesforceJWTClient
-from salesforce_tools.bulk import SalesforceBulkAPI, SalesforceBulkJobException
+from salesforce_tools.auth import login, SalesforceOAuthClient, SalesforceJWTClient, sfdx_auth_url_to_dict
+from salesforce_tools.bulk import BulkAPI, BulkJobException
 from salesforce_tools.bulk_models import JobInfo, JobInfoList, JobTypeEnum, JobStateEnum, OperationEnum, ContentTypeEnum
 from salesforce_tools.oauth_server import CallbackServer, OAuthCallbackHandler
 from salesforce_tools.util import SFDateTime, EmailValidator, EMAIL_ADDRESS_REGEX
```

### Comparing `salesforce-tools-0.1.9/salesforce_tools/auth.py` & `salesforce_tools-0.2.0/salesforce_tools/auth.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,36 +6,35 @@
 from datetime import datetime, timedelta
 import webbrowser
 from salesforce_tools.oauth_server import CallbackServer
 from urllib.parse import urlsplit, urljoin
 import os
 from typing import Callable
 import jwt
+from urllib.parse import urlparse
+
 
 os.environ['OAUTHLIB_INSECURE_TRANSPORT'] = "1"
 AUTH_URL = 'https://login.salesforce.com'
 AUTH_REL_URL = '/services/oauth2/authorize'
 TOKEN_REL_URL = '/services/oauth2/token'
 TOKEN_LIFE = timedelta(hours=2)
 
 
-def login(client_id: str = None, client_secret: str = None, token: dict = None,
+def login(client_id: str = None, client_secret: str = None, token: dict = {},
           token_updater: Callable = lambda x: True, callback_port: int = 8000,
           force_login: bool = False, scope: str = 'refresh_token openid web full',
           auth_url: str = AUTH_URL, redirect_url: str = None, private_key: str = None,
-          private_key_filename: str = None):
+          private_key_filename: str = None, username: str = None, **kwargs):
     auth_code_url = urljoin(auth_url, AUTH_REL_URL)
-    token_url = urljoin(auth_code_url, TOKEN_REL_URL)
+    token_url = urljoin(auth_url, TOKEN_REL_URL)
     redirect_url = redirect_url or f"http://localhost:{callback_port}/callback"
     if private_key or private_key_filename:
-        client = SalesforceJWTClient(client_id,
-                                     auth_url,
-                                     private_key_filename=private_key_filename,
-                                     private_key=private_key
-                                     )
+        client = SalesforceJWTClient(client_id, username=username, auth_url=auth_url,
+                                     private_key_filename=private_key_filename, private_key=private_key)
         salesforce = salesforce_compliance_fix(
             SalesforceOAuth2Session(client=client, auto_refresh_url=token_url, token_updater=token_updater)
         )
         salesforce.fetch_token(token_url)
         if token_updater:
             token_updater(salesforce.token)
     else:
@@ -66,23 +65,24 @@
     return salesforce
 
 
 def salesforce_compliance_fix(sess):
     token = ''
 
     def _compliance_fix(response):
-        token = json.loads(response.text)
+        token = response.json()
         if token.get('issued_at'):
             iat = int(token["issued_at"]) / 1000
             token["expires_in"] = (datetime.fromtimestamp(iat) + TOKEN_LIFE - datetime.now()).seconds
         else:
             token["expires_in"] = TOKEN_LIFE.seconds
         fixed_token = json.dumps(token)
         response._content = to_unicode(fixed_token).encode("utf-8")
-
+        if token.get('instance_url'):
+            sess.instance_url = token.get('instance_url')
         return response
 
     sess.register_compliance_hook("access_token_response", _compliance_fix)
     sess.register_compliance_hook("refresh_token_response", _compliance_fix)
 
     return sess
 
@@ -101,32 +101,33 @@
         headers['X-SFDC-Session'] = self.token.get('access_token')
         return uri, headers, body
 
 
 class SalesforceJWTClient(BackendApplicationClient):
     grant_type = 'urn:ietf:params:oauth:grant-type:jwt-bearer'
 
-    def __init__(self, client_id,
-                 audience: str = None,
+    def __init__(self, client_id: str, username: str,
+                 auth_url: str = 'https://test.salesforce.com',
                  private_key_filename: str = None,
                  private_key: str = None,
                  **kwargs):
         super().__init__(client_id, **kwargs)
-        self.audience = audience
+        self.audience = auth_url
         self.private_key = private_key
+        self.user_name = username
         if private_key_filename:
             with open(private_key_filename, mode='r') as f:
                 self.private_key = ''.join(f.readlines())
 
     def prepare_refresh_body(self, body: str = '', **kwargs):
         return self.prepare_request_body(body)
 
     def prepare_request_body(self, body: str = '', **kwargs):
         claims = {"iss": self.client_id,
-                  "sub": "arroyo2207@fionta.com",
+                  "sub": self.user_name,
                   "aud": self.audience,
                   "exp": int(datetime.now().timestamp()) + 60 * 3
                   }
 
         signed_claims = jwt.encode(claims, self.private_key, "RS256")
         return prepare_token_request(self.grant_type, assertion=signed_claims, format="json", **kwargs)
 
@@ -140,16 +141,41 @@
             token_placement=token_placement
         )
 
         headers['X-SFDC-Session'] = self.token.get('access_token')
         return uri, headers, body
 
 
+def sfdx_auth_url_to_dict(url):
+    p_url = urlparse(url)
+    if p_url.scheme == 'force':
+        i_url = f"https://{p_url.hostname}"
+        return {
+            "client_id": p_url.username,
+            "client_secret": p_url.password.split(':')[0],
+            "token": {
+                "refresh_token": p_url.password.split(':')[1],
+                "instance_url": i_url,
+                "access_token": 'REFRESH_ME',
+                "expires_at": int(datetime.now().timestamp())
+
+            },
+            "auth_url": i_url
+
+        }
+
+
 class SalesforceOAuth2Session(OAuth2Session):
-    def __init__(self, instance_url=None, *args, **kwargs):
+    def __init__(self, instance_url=None, api_root=None, *args, **kwargs):
         super(SalesforceOAuth2Session, self).__init__(*args, **kwargs)
         self.instance_url = instance_url
+        if not self.instance_url and self.token and self.token.get('instance_url'):
+            self.instance_url = self.token.get('instance_url')
+        self.api_root = api_root
 
     def request(self, method, url, *args, **kwargs):
-        url = urljoin(self.instance_url, url)
+        if not self.instance_url and self.token and self.token.get('instance_url'):
+            self.instance_url = self.token.get('instance_url')
+        base_url = ''.join(filter(None, [self.instance_url, self.api_root]))
+        url = urljoin(base_url, url)
         return super(SalesforceOAuth2Session, self).request(method, url, *args, **kwargs)
```

### Comparing `salesforce-tools-0.1.9/salesforce_tools/bulk.py` & `salesforce_tools-0.2.0/salesforce_tools/bulk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import urllib.parse
 from salesforce_tools.salesforce import SalesforceAPI
 from enum import Enum
 from salesforce_tools.bulk_models import JobInfo, JobInfoList, BatchInfo, BatchInfoList, \
     OperationEnum, ContentTypeEnum, ContentTypeHeaderEnum, JobTypeEnum, JobStateEnum, BulkAPIError, APIError,\
     BulkException
 from typing import Union, Optional, List
-from pydantic import BaseModel, ValidationError, parse_obj_as
+from pydantic.v1 import BaseModel, ValidationError, parse_obj_as
 
 
-class SalesforceBulkJobException(Exception):
+class BulkJobException(Exception):
     pass
 
 
 def get_enum_or_val(e):
     return e.value if isinstance(e, Enum) else e
 
 
-class SalesforceBulkAPI(SalesforceAPI):
+class BulkAPI(SalesforceAPI):
     job: Optional[Union[JobInfo, BulkAPIError]]
     batches: List[BatchInfo] = []
 
     @property
     def job(self):
         return self.__job
```

### Comparing `salesforce-tools-0.1.9/salesforce_tools/bulk_models.py` & `salesforce_tools-0.2.0/salesforce_tools/bulk_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pydantic import BaseModel, ValidationError, validator, Field
+from pydantic.v1 import BaseModel, ValidationError, validator, Field
 from typing import Literal, Optional, List
 from enum import Enum
 import datetime
 
 
 class JobStateEnum(str, Enum):
     Open = 'Open'
```

### Comparing `salesforce-tools-0.1.9/salesforce_tools/oauth_server.py` & `salesforce_tools-0.2.0/salesforce_tools/oauth_server.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,31 +16,34 @@
             http_body = f"error: {args['error'][0]}\nerror description: {args['error_description'][0]}"
         else:
             http_status = http.client.OK
             emoji = random.choice(["🎉", "👍", "👍🏿", "🥳", "🎈"])
             http_body = f"""<html>
                <h1 style="font-size: large">{emoji}</h1>
                <p>Congratulations! Your authentication succeeded.</p>"""
-            auth_code = args["code"]
-            self.parent.auth_code = auth_code[0]
-            self.parent.path = self.path
+            if not hasattr(self.parent, "path"):
+                auth_code = args.get("code")
+                self.parent.auth_code = auth_code[0]
+                self.parent.path = self.path
         self.send_response(http_status)
         self.send_header("Content-Type", "text/html; charset=utf-8")
 
         self.end_headers()
         self.wfile.write(http_body.encode("utf-8"))
 
         threading.Thread(target=self.server.shutdown).start()
 
+    def log_message(self, fmt, *args):
+        pass
+
 
 class CallbackServer:
     def get_auth(self, port=8000):
         OAuthCallbackHandler.parent = self
         httpd = HTTPServer(('localhost', port), OAuthCallbackHandler)
         httpd.timeout = 30
         httpd.serve_forever()
         return self.path
 
 
 if __name__ == "__main__":
     cs = CallbackServer()
-    print(cs.get_auth())
```

### Comparing `salesforce-tools-0.1.9/salesforce_tools/salesforce.py` & `salesforce_tools-0.2.0/salesforce_tools/salesforce.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,48 +1,62 @@
 from salesforce_tools.auth import login
 from urllib.parse import urljoin, urlencode
 import webbrowser
 import xmltodict
 from salesforce_tools.util import SFDateTime, EMAIL_ADDRESS_REGEX
-from pydantic import Field, create_model, constr
+from pydantic.v1 import Field, create_model, constr
 from typing import Optional, Literal
 from decimal import Decimal
 from datetime import date
 import re
 
 
 class SalesforceAPI(object):
     session = None
-    api_version = None
     api_root = None
     instance_url = None
     args = {}
 
-    def __init__(self, api_version='54.0', **kwargs):
-        self.session = login(**kwargs)
-        self.instance_url = self.session.token.get('instance_url')
-        self.api_version = api_version
+    def __init__(self, api_version=None, api_root=None, **kwargs):
         self.args = kwargs
+        self.args['api_version'] = api_version
+        self.api_root = api_root.format(api_version=self.api_version, version=self.api_version) if api_root else None
+        self.session = login(**kwargs)
+        self.session.api_root = self.api_root
+        self.instance_url = self.session.instance_url
 
-    def request(self, url, method='GET', api=None, **kwargs):
-        api = (api or self.api_root).format(api_version=self.api_version, version=self.api_version)
+    @property
+    def api_version(self):
+        return self.args.get('api_version') or '56.0'
+
+    def request(self, url, method='GET', **kwargs):
         kwargs['headers'] = kwargs.get('headers', {'Content-Type': 'application/json',
                                                    'Accepts': 'application/json',
                                                    'charset': 'UTF-8'})
-
-        base_url = urljoin(self.instance_url, api) if api else self.instance_url
-        url = urljoin(base_url, url)
         req = self.session.request(method, url, **kwargs)
         return self._force_dict_response(req)
 
-    def get(self, url, **kwargs):
-        return self.request(url, **kwargs)
-
-    def post(self, url, **kwargs):
-        return self.request(url, method='POST', **kwargs)
+    def get(self, url, auto_next=False, **kwargs):
+        t = self.request(url, **kwargs)
+        try:
+            next_records_url = t[0].get('nextRecordsUrl')
+            while auto_next and t[0].get('records') and next_records_url:
+                t2 = self.request(next_records_url)
+                next_records_url = t2[0].get('nextRecordsUrl')
+                t[0]['records'] = t[0]['records'] + t2[0]['records']
+        except AttributeError:
+            pass
+
+        return t
+
+    def __getattr__(self, name):
+        def wrapper(*args, **kwargs):
+            kwargs['method'] = name.upper()
+            return self.request(*args, **kwargs)
+        return wrapper
 
     def _force_dict_response(self, resp):
         if 'application/xml' in resp.headers.get('Content-Type', ''):
             data = xmltodict.parse(resp.text)
         elif 'application/json' in resp.headers.get('Content-Type', ''):
             data = resp.json()
         else:
@@ -53,35 +67,45 @@
         sid = self.session.token.get('access_token')
         qs = urlencode({'sid': sid, 'retURL': url})
         url = urljoin(self.instance_url, f'/secur/frontdoor.jsp?{qs}')
         webbrowser.open(url)
 
 
 class RestAPI(SalesforceAPI):
-    api_root = '/services/data/v{api_version}/'
+    def __init__(self, **kwargs):
+        super().__init__(api_root='/services/data/v{api_version}/', **kwargs)
 
     def get_metadata(self, sobject):
         return self.request(f'sobjects/{sobject}/describe/')
 
     def get_record(self, sobject, sfid):
         return self.request(f'sobjects/{sobject}/{sfid}')
 
+    def query(self, query, **kwargs):
+        qs = urlencode({'q': query})
+        return self.get(f'query?{qs}', **kwargs)
+
 
 class ToolingAPI(SalesforceAPI):
-    api_root = '/services/data/v{api_version}/tooling/'
+    def __init__(self, **kwargs):
+        super().__init__(api_root='/services/data/v{api_version}/tooling/', **kwargs)
+
+    def query(self, query, **kwargs):
+        qs = urlencode({'q': query})
+        return self.get(f'query?{qs}', **kwargs)
 
 
 class SalesforceModelFactory(object):
     address_md_template = [{'aggregatable': True, 'aiPredictionField': False, 'autoNumber': False, 'byteLength': 765, 'calculated': False, 'calculatedFormula': None, 'cascadeDelete': False, 'caseSensitive': False, 'compoundFieldName': 'BillingAddress', 'controllerName': None, 'createable': True, 'custom': False, 'defaultValue': None, 'defaultValueFormula': None, 'defaultedOnCreate': False, 'dependentPicklist': False, 'deprecatedAndHidden': False, 'digits': 0, 'displayLocationInDecimal': False, 'encrypted': False, 'externalId': False, 'extraTypeInfo': 'plaintextarea', 'filterable': True, 'filteredLookupInfo': None, 'formulaTreatNullNumberAsZero': False, 'groupable': True, 'highScaleNumber': False, 'htmlFormatted': False, 'idLookup': False, 'inlineHelpText': None, 'label': 'Billing Street', 'length': 255, 'mask': None, 'maskType': None, 'name': 'street', 'nameField': False, 'namePointing': False, 'nillable': True, 'permissionable': True, 'picklistValues': [], 'polymorphicForeignKey': False, 'precision': 0, 'queryByDistance': False, 'referenceTargetField': None, 'referenceTo': [], 'relationshipName': None, 'relationshipOrder': None, 'restrictedDelete': False, 'restrictedPicklist': False, 'scale': 0, 'searchPrefilterable': False, 'soapType': 'xsd:string', 'sortable': True, 'type': 'textarea', 'unique': False, 'updateable': True, 'writeRequiresMasterRead': False}, {'aggregatable': True, 'aiPredictionField': False, 'autoNumber': False, 'byteLength': 120, 'calculated': False, 'calculatedFormula': None, 'cascadeDelete': False, 'caseSensitive': False, 'compoundFieldName': 'BillingAddress', 'controllerName': None, 'createable': True, 'custom': False, 'defaultValue': None, 'defaultValueFormula': None, 'defaultedOnCreate': False, 'dependentPicklist': False, 'deprecatedAndHidden': False, 'digits': 0, 'displayLocationInDecimal': False, 'encrypted': False, 'externalId': False, 'extraTypeInfo': None, 'filterable': True, 'filteredLookupInfo': None, 'formulaTreatNullNumberAsZero': False, 'groupable': True, 'highScaleNumber': False, 'htmlFormatted': False, 'idLookup': False, 'inlineHelpText': None, 'label': 'Billing City', 'length': 40, 'mask': None, 'maskType': None, 'name': 'city', 'nameField': False, 'namePointing': False, 'nillable': True, 'permissionable': True, 'picklistValues': [], 'polymorphicForeignKey': False, 'precision': 0, 'queryByDistance': False, 'referenceTargetField': None, 'referenceTo': [], 'relationshipName': None, 'relationshipOrder': None, 'restrictedDelete': False, 'restrictedPicklist': False, 'scale': 0, 'searchPrefilterable': False, 'soapType': 'xsd:string', 'sortable': True, 'type': 'string', 'unique': False, 'updateable': True, 'writeRequiresMasterRead': False}, {'aggregatable': True, 'aiPredictionField': False, 'autoNumber': False, 'byteLength': 240, 'calculated': False, 'calculatedFormula': None, 'cascadeDelete': False, 'caseSensitive': False, 'compoundFieldName': 'BillingAddress', 'controllerName': None, 'createable': True, 'custom': False, 'defaultValue': None, 'defaultValueFormula': None, 'defaultedOnCreate': False, 'dependentPicklist': False, 'deprecatedAndHidden': False, 'digits': 0, 'displayLocationInDecimal': False, 'encrypted': False, 'externalId': False, 'extraTypeInfo': None, 'filterable': True, 'filteredLookupInfo': None, 'formulaTreatNullNumberAsZero': False, 'groupable': True, 'highScaleNumber': False, 'htmlFormatted': False, 'idLookup': False, 'inlineHelpText': None, 'label': 'Billing State/Province', 'length': 80, 'mask': None, 'maskType': None, 'name': 'state', 'nameField': False, 'namePointing': False, 'nillable': True, 'permissionable': True, 'picklistValues': [], 'polymorphicForeignKey': False, 'precision': 0, 'queryByDistance': False, 'referenceTargetField': None, 'referenceTo': [], 'relationshipName': None, 'relationshipOrder': None, 'restrictedDelete': False, 'restrictedPicklist': False, 'scale': 0, 'searchPrefilterable': False, 'soapType': 'xsd:string', 'sortable': True, 'type': 'string', 'unique': False, 'updateable': True, 'writeRequiresMasterRead': False}, {'aggregatable': True, 'aiPredictionField': False, 'autoNumber': False, 'byteLength': 60, 'calculated': False, 'calculatedFormula': None, 'cascadeDelete': False, 'caseSensitive': False, 'compoundFieldName': 'BillingAddress', 'controllerName': None, 'createable': True, 'custom': False, 'defaultValue': None, 'defaultValueFormula': None, 'defaultedOnCreate': False, 'dependentPicklist': False, 'deprecatedAndHidden': False, 'digits': 0, 'displayLocationInDecimal': False, 'encrypted': False, 'externalId': False, 'extraTypeInfo': None, 'filterable': True, 'filteredLookupInfo': None, 'formulaTreatNullNumberAsZero': False, 'groupable': True, 'highScaleNumber': False, 'htmlFormatted': False, 'idLookup': False, 'inlineHelpText': None, 'label': 'Billing Zip/Postal Code', 'length': 20, 'mask': None, 'maskType': None, 'name': 'postalCode', 'nameField': False, 'namePointing': False, 'nillable': True, 'permissionable': True, 'picklistValues': [], 'polymorphicForeignKey': False, 'precision': 0, 'queryByDistance': False, 'referenceTargetField': None, 'referenceTo': [], 'relationshipName': None, 'relationshipOrder': None, 'restrictedDelete': False, 'restrictedPicklist': False, 'scale': 0, 'searchPrefilterable': False, 'soapType': 'xsd:string', 'sortable': True, 'type': 'string', 'unique': False, 'updateable': True, 'writeRequiresMasterRead': False}, {'aggregatable': True, 'aiPredictionField': False, 'autoNumber': False, 'byteLength': 240, 'calculated': False, 'calculatedFormula': None, 'cascadeDelete': False, 'caseSensitive': False, 'compoundFieldName': 'BillingAddress', 'controllerName': None, 'createable': True, 'custom': False, 'defaultValue': None, 'defaultValueFormula': None, 'defaultedOnCreate': False, 'dependentPicklist': False, 'deprecatedAndHidden': False, 'digits': 0, 'displayLocationInDecimal': False, 'encrypted': False, 'externalId': False, 'extraTypeInfo': None, 'filterable': True, 'filteredLookupInfo': None, 'formulaTreatNullNumberAsZero': False, 'groupable': True, 'highScaleNumber': False, 'htmlFormatted': False, 'idLookup': False, 'inlineHelpText': None, 'label': 'Billing Country', 'length': 80, 'mask': None, 'maskType': None, 'name': 'country', 'nameField': False, 'namePointing': False, 'nillable': True, 'permissionable': True, 'picklistValues': [], 'polymorphicForeignKey': False, 'precision': 0, 'queryByDistance': False, 'referenceTargetField': None, 'referenceTo': [], 'relationshipName': None, 'relationshipOrder': None, 'restrictedDelete': False, 'restrictedPicklist': False, 'scale': 0, 'searchPrefilterable': False, 'soapType': 'xsd:string', 'sortable': True, 'type': 'string', 'unique': False, 'updateable': True, 'writeRequiresMasterRead': False}, {'aggregatable': True, 'aiPredictionField': False, 'autoNumber': False, 'byteLength': 30, 'calculated': False, 'calculatedFormula': None, 'cascadeDelete': False, 'caseSensitive': False, 'compoundFieldName': 'BillingAddress', 'controllerName': 'BillingCountryCode', 'createable': True, 'custom': False, 'defaultValue': None, 'defaultValueFormula': None, 'defaultedOnCreate': False, 'dependentPicklist': True, 'deprecatedAndHidden': False, 'digits': 0, 'displayLocationInDecimal': False, 'encrypted': False, 'externalId': False, 'extraTypeInfo': None, 'filterable': True, 'filteredLookupInfo': None, 'formulaTreatNullNumberAsZero': False, 'groupable': True, 'highScaleNumber': False, 'htmlFormatted': False, 'idLookup': False, 'inlineHelpText': None, 'label': 'Billing State/Province Code', 'length': 10, 'mask': None, 'maskType': None, 'name': 'stateCode', 'nameField': False, 'namePointing': False, 'nillable': True, 'permissionable': True, 'picklistValues': [{'active': True, 'defaultValue': False, 'label': 'Acre', 'validFor': 'AAAAAgAA', 'value': 'AC'}, {'active': True, 'defaultValue': False, 'label': 'Agrigento', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'AG'}, {'active': True, 'defaultValue': False, 'label': 'Aguascalientes', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'AG'}, {'active': True, 'defaultValue': False, 'label': 'Alabama', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'AL'}, {'active': True, 'defaultValue': False, 'label': 'Alagoas', 'validFor': 'AAAAAgAA', 'value': 'AL'}, {'active': True, 'defaultValue': False, 'label': 'Alaska', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'AK'}, {'active': True, 'defaultValue': False, 'label': 'Alberta', 'validFor': 'AAAAAAIA', 'value': 'AB'}, {'active': True, 'defaultValue': False, 'label': 'Alessandria', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'AL'}, {'active': True, 'defaultValue': False, 'label': 'Amapá', 'validFor': 'AAAAAgAA', 'value': 'AP'}, {'active': True, 'defaultValue': False, 'label': 'Amazonas', 'validFor': 'AAAAAgAA', 'value': 'AM'}, {'active': True, 'defaultValue': False, 'label': 'Ancona', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'AN'}, {'active': True, 'defaultValue': False, 'label': 'Andaman and Nicobar Islands', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'AN'}, {'active': True, 'defaultValue': False, 'label': 'Andhra Pradesh', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'AP'}, {'active': True, 'defaultValue': False, 'label': 'Anhui', 'validFor': 'AAAAAAAI', 'value': '34'}, {'active': True, 'defaultValue': False, 'label': 'Aosta', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'AO'}, {'active': True, 'defaultValue': False, 'label': 'Arezzo', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'AR'}, {'active': True, 'defaultValue': False, 'label': 'Arizona', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'AZ'}, {'active': True, 'defaultValue': False, 'label': 'Arkansas', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'AR'}, {'active': True, 'defaultValue': False, 'label': 'Arunachal Pradesh', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'AR'}, {'active': True, 'defaultValue': False, 'label': 'Ascoli Piceno', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'AP'}, {'active': True, 'defaultValue': False, 'label': 'Assam', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'AS'}, {'active': True, 'defaultValue': False, 'label': 'Asti', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'AT'}, {'active': True, 'defaultValue': False, 'label': 'Australian Capital Territory', 'validFor': 'AAgA', 'value': 'ACT'}, {'active': True, 'defaultValue': False, 'label': 'Avellino', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'AV'}, {'active': True, 'defaultValue': False, 'label': 'Bahia', 'validFor': 'AAAAAgAA', 'value': 'BA'}, {'active': True, 'defaultValue': False, 'label': 'Baja California', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'BC'}, {'active': True, 'defaultValue': False, 'label': 'Baja California Sur', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'BS'}, {'active': True, 'defaultValue': False, 'label': 'Bari', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'BA'}, {'active': True, 'defaultValue': False, 'label': 'Barletta-Andria-Trani', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'BT'}, {'active': True, 'defaultValue': False, 'label': 'Beijing', 'validFor': 'AAAAAAAI', 'value': '11'}, {'active': True, 'defaultValue': False, 'label': 'Belluno', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'BL'}, {'active': True, 'defaultValue': False, 'label': 'Benevento', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'BN'}, {'active': True, 'defaultValue': False, 'label': 'Bergamo', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'BG'}, {'active': True, 'defaultValue': False, 'label': 'Biella', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'BI'}, {'active': True, 'defaultValue': False, 'label': 'Bihar', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'BR'}, {'active': True, 'defaultValue': False, 'label': 'Bologna', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'BO'}, {'active': True, 'defaultValue': False, 'label': 'Bolzano', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'BZ'}, {'active': True, 'defaultValue': False, 'label': 'Brescia', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'BS'}, {'active': True, 'defaultValue': False, 'label': 'Brindisi', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'BR'}, {'active': True, 'defaultValue': False, 'label': 'British Columbia', 'validFor': 'AAAAAAIA', 'value': 'BC'}, {'active': True, 'defaultValue': False, 'label': 'Cagliari', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'CA'}, {'active': True, 'defaultValue': False, 'label': 'California', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'CA'}, {'active': True, 'defaultValue': False, 'label': 'Caltanissetta', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'CL'}, {'active': True, 'defaultValue': False, 'label': 'Campeche', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'CM'}, {'active': True, 'defaultValue': False, 'label': 'Campobasso', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'CB'}, {'active': True, 'defaultValue': False, 'label': 'Carbonia-Iglesias', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'CI'}, {'active': True, 'defaultValue': False, 'label': 'Carlow', 'validFor': 'AAAAAAAAAAAAAAAAAQAA', 'value': 'CW'}, {'active': True, 'defaultValue': False, 'label': 'Caserta', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'CE'}, {'active': True, 'defaultValue': False, 'label': 'Catania', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'CT'}, {'active': True, 'defaultValue': False, 'label': 'Catanzaro', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'CZ'}, {'active': True, 'defaultValue': False, 'label': 'Cavan', 'validFor': 'AAAAAAAAAAAAAAAAAQAA', 'value': 'CN'}, {'active': True, 'defaultValue': False, 'label': 'Ceará', 'validFor': 'AAAAAgAA', 'value': 'CE'}, {'active': True, 'defaultValue': False, 'label': 'Chandigarh', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'CH'}, {'active': True, 'defaultValue': False, 'label': 'Chhattisgarh', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'CT'}, {'active': True, 'defaultValue': False, 'label': 'Chiapas', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'CS'}, {'active': True, 'defaultValue': False, 'label': 'Chieti', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'CH'}, {'active': True, 'defaultValue': False, 'label': 'Chihuahua', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'CH'}, {'active': True, 'defaultValue': False, 'label': 'Chongqing', 'validFor': 'AAAAAAAI', 'value': '50'}, {'active': True, 'defaultValue': False, 'label': 'Clare', 'validFor': 'AAAAAAAAAAAAAAAAAQAA', 'value': 'CE'}, {'active': True, 'defaultValue': False, 'label': 'Coahuila', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'CO'}, {'active': True, 'defaultValue': False, 'label': 'Colima', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'CL'}, {'active': True, 'defaultValue': False, 'label': 'Colorado', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'CO'}, {'active': True, 'defaultValue': False, 'label': 'Como', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'CO'}, {'active': True, 'defaultValue': False, 'label': 'Connecticut', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'CT'}, {'active': True, 'defaultValue': False, 'label': 'Cork', 'validFor': 'AAAAAAAAAAAAAAAAAQAA', 'value': 'CO'}, {'active': True, 'defaultValue': False, 'label': 'Cosenza', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'CS'}, {'active': True, 'defaultValue': False, 'label': 'Cremona', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'CR'}, {'active': True, 'defaultValue': False, 'label': 'Crotone', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'KR'}, {'active': True, 'defaultValue': False, 'label': 'Cuneo', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'CN'}, {'active': True, 'defaultValue': False, 'label': 'Dadra and Nagar Haveli', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'DN'}, {'active': True, 'defaultValue': False, 'label': 'Daman and Diu', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'DD'}, {'active': True, 'defaultValue': False, 'label': 'Delaware', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'DE'}, {'active': True, 'defaultValue': False, 'label': 'Delhi', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'DL'}, {'active': True, 'defaultValue': False, 'label': 'District of Columbia', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'DC'}, {'active': True, 'defaultValue': False, 'label': 'Distrito Federal', 'validFor': 'AAAAAgAA', 'value': 'DF'}, {'active': True, 'defaultValue': False, 'label': 'Donegal', 'validFor': 'AAAAAAAAAAAAAAAAAQAA', 'value': 'DL'}, {'active': True, 'defaultValue': False, 'label': 'Dublin', 'validFor': 'AAAAAAAAAAAAAAAAAQAA', 'value': 'D'}, {'active': True, 'defaultValue': False, 'label': 'Durango', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'DG'}, {'active': True, 'defaultValue': False, 'label': 'Enna', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'EN'}, {'active': True, 'defaultValue': False, 'label': 'Espírito Santo', 'validFor': 'AAAAAgAA', 'value': 'ES'}, {'active': True, 'defaultValue': False, 'label': 'Federal District', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'DF'}, {'active': True, 'defaultValue': False, 'label': 'Fermo', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'FM'}, {'active': True, 'defaultValue': False, 'label': 'Ferrara', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'FE'}, {'active': True, 'defaultValue': False, 'label': 'Florence', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'FI'}, {'active': True, 'defaultValue': False, 'label': 'Florida', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'FL'}, {'active': True, 'defaultValue': False, 'label': 'Foggia', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'FG'}, {'active': True, 'defaultValue': False, 'label': 'Forlì-Cesena', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'FC'}, {'active': True, 'defaultValue': False, 'label': 'Frosinone', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'FR'}, {'active': True, 'defaultValue': False, 'label': 'Fujian', 'validFor': 'AAAAAAAI', 'value': '35'}, {'active': True, 'defaultValue': False, 'label': 'Galway', 'validFor': 'AAAAAAAAAAAAAAAAAQAA', 'value': 'G'}, {'active': True, 'defaultValue': False, 'label': 'Gansu', 'validFor': 'AAAAAAAI', 'value': '62'}, {'active': True, 'defaultValue': False, 'label': 'Genoa', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'GE'}, {'active': True, 'defaultValue': False, 'label': 'Georgia', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'GA'}, {'active': True, 'defaultValue': False, 'label': 'Goa', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'GA'}, {'active': True, 'defaultValue': False, 'label': 'Goiás', 'validFor': 'AAAAAgAA', 'value': 'GO'}, {'active': True, 'defaultValue': False, 'label': 'Gorizia', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'GO'}, {'active': True, 'defaultValue': False, 'label': 'Grosseto', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'GR'}, {'active': True, 'defaultValue': False, 'label': 'Guanajuato', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'GT'}, {'active': True, 'defaultValue': False, 'label': 'Guangdong', 'validFor': 'AAAAAAAI', 'value': '44'}, {'active': True, 'defaultValue': False, 'label': 'Guangxi', 'validFor': 'AAAAAAAI', 'value': '45'}, {'active': True, 'defaultValue': False, 'label': 'Guerrero', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'GR'}, {'active': True, 'defaultValue': False, 'label': 'Guizhou', 'validFor': 'AAAAAAAI', 'value': '52'}, {'active': True, 'defaultValue': False, 'label': 'Gujarat', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'GJ'}, {'active': True, 'defaultValue': False, 'label': 'Hainan', 'validFor': 'AAAAAAAI', 'value': '46'}, {'active': True, 'defaultValue': False, 'label': 'Haryana', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'HR'}, {'active': True, 'defaultValue': False, 'label': 'Hawaii', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'HI'}, {'active': True, 'defaultValue': False, 'label': 'Hebei', 'validFor': 'AAAAAAAI', 'value': '13'}, {'active': True, 'defaultValue': False, 'label': 'Heilongjiang', 'validFor': 'AAAAAAAI', 'value': '23'}, {'active': True, 'defaultValue': False, 'label': 'Henan', 'validFor': 'AAAAAAAI', 'value': '41'}, {'active': True, 'defaultValue': False, 'label': 'Hidalgo', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'HG'}, {'active': True, 'defaultValue': False, 'label': 'Himachal Pradesh', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'HP'}, {'active': True, 'defaultValue': False, 'label': 'Hong Kong', 'validFor': 'AAAAAAAI', 'value': '91'}, {'active': True, 'defaultValue': False, 'label': 'Hubei', 'validFor': 'AAAAAAAI', 'value': '42'}, {'active': True, 'defaultValue': False, 'label': 'Hunan', 'validFor': 'AAAAAAAI', 'value': '43'}, {'active': True, 'defaultValue': False, 'label': 'Idaho', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'ID'}, {'active': True, 'defaultValue': False, 'label': 'Illinois', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'IL'}, {'active': True, 'defaultValue': False, 'label': 'Imperia', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'IM'}, {'active': True, 'defaultValue': False, 'label': 'Indiana', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'IN'}, {'active': True, 'defaultValue': False, 'label': 'Iowa', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'IA'}, {'active': True, 'defaultValue': False, 'label': 'Isernia', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'IS'}, {'active': True, 'defaultValue': False, 'label': 'Jalisco', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'JA'}, {'active': True, 'defaultValue': False, 'label': 'Jammu and Kashmir', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'JK'}, {'active': True, 'defaultValue': False, 'label': 'Jharkhand', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'JH'}, {'active': True, 'defaultValue': False, 'label': 'Jiangsu', 'validFor': 'AAAAAAAI', 'value': '32'}, {'active': True, 'defaultValue': False, 'label': 'Jiangxi', 'validFor': 'AAAAAAAI', 'value': '36'}, {'active': True, 'defaultValue': False, 'label': 'Jilin', 'validFor': 'AAAAAAAI', 'value': '22'}, {'active': True, 'defaultValue': False, 'label': 'Kansas', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'KS'}, {'active': True, 'defaultValue': False, 'label': 'Karnataka', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'KA'}, {'active': True, 'defaultValue': False, 'label': 'Kentucky', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'KY'}, {'active': True, 'defaultValue': False, 'label': 'Kerala', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'KL'}, {'active': True, 'defaultValue': False, 'label': 'Kerry', 'validFor': 'AAAAAAAAAAAAAAAAAQAA', 'value': 'KY'}, {'active': True, 'defaultValue': False, 'label': 'Kildare', 'validFor': 'AAAAAAAAAAAAAAAAAQAA', 'value': 'KE'}, {'active': True, 'defaultValue': False, 'label': 'Kilkenny', 'validFor': 'AAAAAAAAAAAAAAAAAQAA', 'value': 'KK'}, {'active': True, 'defaultValue': False, 'label': "L'Aquila", 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'AQ'}, {'active': True, 'defaultValue': False, 'label': 'Lakshadweep', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'LD'}, {'active': True, 'defaultValue': False, 'label': 'Laois', 'validFor': 'AAAAAAAAAAAAAAAAAQAA', 'value': 'LS'}, {'active': True, 'defaultValue': False, 'label': 'La Spezia', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'SP'}, {'active': True, 'defaultValue': False, 'label': 'Latina', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'LT'}, {'active': True, 'defaultValue': False, 'label': 'Lecce', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'LE'}, {'active': True, 'defaultValue': False, 'label': 'Lecco', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'LC'}, {'active': True, 'defaultValue': False, 'label': 'Leitrim', 'validFor': 'AAAAAAAAAAAAAAAAAQAA', 'value': 'LM'}, {'active': True, 'defaultValue': False, 'label': 'Liaoning', 'validFor': 'AAAAAAAI', 'value': '21'}, {'active': True, 'defaultValue': False, 'label': 'Limerick', 'validFor': 'AAAAAAAAAAAAAAAAAQAA', 'value': 'LK'}, {'active': True, 'defaultValue': False, 'label': 'Livorno', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'LI'}, {'active': True, 'defaultValue': False, 'label': 'Lodi', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'LO'}, {'active': True, 'defaultValue': False, 'label': 'Longford', 'validFor': 'AAAAAAAAAAAAAAAAAQAA', 'value': 'LD'}, {'active': True, 'defaultValue': False, 'label': 'Louisiana', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'LA'}, {'active': True, 'defaultValue': False, 'label': 'Louth', 'validFor': 'AAAAAAAAAAAAAAAAAQAA', 'value': 'LH'}, {'active': True, 'defaultValue': False, 'label': 'Lucca', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'LU'}, {'active': True, 'defaultValue': False, 'label': 'Macao', 'validFor': 'AAAAAAAI', 'value': '92'}, {'active': True, 'defaultValue': False, 'label': 'Macerata', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'MC'}, {'active': True, 'defaultValue': False, 'label': 'Madhya Pradesh', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'MP'}, {'active': True, 'defaultValue': False, 'label': 'Maharashtra', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'MH'}, {'active': True, 'defaultValue': False, 'label': 'Maine', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'ME'}, {'active': True, 'defaultValue': False, 'label': 'Manipur', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'MN'}, {'active': True, 'defaultValue': False, 'label': 'Manitoba', 'validFor': 'AAAAAAIA', 'value': 'MB'}, {'active': True, 'defaultValue': False, 'label': 'Mantua', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'MN'}, {'active': True, 'defaultValue': False, 'label': 'Maranhão', 'validFor': 'AAAAAgAA', 'value': 'MA'}, {'active': True, 'defaultValue': False, 'label': 'Maryland', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'MD'}, {'active': True, 'defaultValue': False, 'label': 'Massa and Carrara', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'MS'}, {'active': True, 'defaultValue': False, 'label': 'Massachusetts', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'MA'}, {'active': True, 'defaultValue': False, 'label': 'Matera', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'MT'}, {'active': True, 'defaultValue': False, 'label': 'Mato Grosso', 'validFor': 'AAAAAgAA', 'value': 'MT'}, {'active': True, 'defaultValue': False, 'label': 'Mato Grosso do Sul', 'validFor': 'AAAAAgAA', 'value': 'MS'}, {'active': True, 'defaultValue': False, 'label': 'Mayo', 'validFor': 'AAAAAAAAAAAAAAAAAQAA', 'value': 'MO'}, {'active': True, 'defaultValue': False, 'label': 'Meath', 'validFor': 'AAAAAAAAAAAAAAAAAQAA', 'value': 'MH'}, {'active': True, 'defaultValue': False, 'label': 'Medio Campidano', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'VS'}, {'active': True, 'defaultValue': False, 'label': 'Meghalaya', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'ML'}, {'active': True, 'defaultValue': False, 'label': 'Messina', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'ME'}, {'active': True, 'defaultValue': False, 'label': 'Mexico State', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'ME'}, {'active': True, 'defaultValue': False, 'label': 'Michigan', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'MI'}, {'active': True, 'defaultValue': False, 'label': 'Michoacán', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'MI'}, {'active': True, 'defaultValue': False, 'label': 'Milan', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'MI'}, {'active': True, 'defaultValue': False, 'label': 'Minas Gerais', 'validFor': 'AAAAAgAA', 'value': 'MG'}, {'active': True, 'defaultValue': False, 'label': 'Minnesota', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'MN'}, {'active': True, 'defaultValue': False, 'label': 'Mississippi', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'MS'}, {'active': True, 'defaultValue': False, 'label': 'Missouri', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'MO'}, {'active': True, 'defaultValue': False, 'label': 'Mizoram', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'MZ'}, {'active': True, 'defaultValue': False, 'label': 'Modena', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'MO'}, {'active': True, 'defaultValue': False, 'label': 'Monaghan', 'validFor': 'AAAAAAAAAAAAAAAAAQAA', 'value': 'MN'}, {'active': True, 'defaultValue': False, 'label': 'Montana', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'MT'}, {'active': True, 'defaultValue': False, 'label': 'Monza and Brianza', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'MB'}, {'active': True, 'defaultValue': False, 'label': 'Morelos', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'MO'}, {'active': True, 'defaultValue': False, 'label': 'Nagaland', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'NL'}, {'active': True, 'defaultValue': False, 'label': 'Naples', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'NA'}, {'active': True, 'defaultValue': False, 'label': 'Nayarit', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'NA'}, {'active': True, 'defaultValue': False, 'label': 'Nebraska', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'NE'}, {'active': True, 'defaultValue': False, 'label': 'Nei Mongol', 'validFor': 'AAAAAAAI', 'value': '15'}, {'active': True, 'defaultValue': False, 'label': 'Nevada', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'NV'}, {'active': True, 'defaultValue': False, 'label': 'New Brunswick', 'validFor': 'AAAAAAIA', 'value': 'NB'}, {'active': True, 'defaultValue': False, 'label': 'Newfoundland and Labrador', 'validFor': 'AAAAAAIA', 'value': 'NL'}, {'active': True, 'defaultValue': False, 'label': 'New Hampshire', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'NH'}, {'active': True, 'defaultValue': False, 'label': 'New Jersey', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'NJ'}, {'active': True, 'defaultValue': False, 'label': 'New Mexico', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'NM'}, {'active': True, 'defaultValue': False, 'label': 'New South Wales', 'validFor': 'AAgA', 'value': 'NSW'}, {'active': True, 'defaultValue': False, 'label': 'New York', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'NY'}, {'active': True, 'defaultValue': False, 'label': 'Ningxia', 'validFor': 'AAAAAAAI', 'value': '64'}, {'active': True, 'defaultValue': False, 'label': 'North Carolina', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'NC'}, {'active': True, 'defaultValue': False, 'label': 'North Dakota', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'ND'}, {'active': True, 'defaultValue': False, 'label': 'Northern Territory', 'validFor': 'AAgA', 'value': 'NT'}, {'active': True, 'defaultValue': False, 'label': 'Northwest Territories', 'validFor': 'AAAAAAIA', 'value': 'NT'}, {'active': True, 'defaultValue': False, 'label': 'Novara', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'NO'}, {'active': True, 'defaultValue': False, 'label': 'Nova Scotia', 'validFor': 'AAAAAAIA', 'value': 'NS'}, {'active': True, 'defaultValue': False, 'label': 'Nuevo León', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'NL'}, {'active': True, 'defaultValue': False, 'label': 'Nunavut', 'validFor': 'AAAAAAIA', 'value': 'NU'}, {'active': True, 'defaultValue': False, 'label': 'Nuoro', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'NU'}, {'active': True, 'defaultValue': False, 'label': 'Oaxaca', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'OA'}, {'active': True, 'defaultValue': False, 'label': 'Odisha', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'OR'}, {'active': True, 'defaultValue': False, 'label': 'Offaly', 'validFor': 'AAAAAAAAAAAAAAAAAQAA', 'value': 'OY'}, {'active': True, 'defaultValue': False, 'label': 'Ogliastra', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'OG'}, {'active': True, 'defaultValue': False, 'label': 'Ohio', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'OH'}, {'active': True, 'defaultValue': False, 'label': 'Oklahoma', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'OK'}, {'active': True, 'defaultValue': False, 'label': 'Olbia-Tempio', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'OT'}, {'active': True, 'defaultValue': False, 'label': 'Ontario', 'validFor': 'AAAAAAIA', 'value': 'ON'}, {'active': True, 'defaultValue': False, 'label': 'Oregon', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'OR'}, {'active': True, 'defaultValue': False, 'label': 'Oristano', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'OR'}, {'active': True, 'defaultValue': False, 'label': 'Padua', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'PD'}, {'active': True, 'defaultValue': False, 'label': 'Palermo', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'PA'}, {'active': True, 'defaultValue': False, 'label': 'Pará', 'validFor': 'AAAAAgAA', 'value': 'PA'}, {'active': True, 'defaultValue': False, 'label': 'Paraíba', 'validFor': 'AAAAAgAA', 'value': 'PB'}, {'active': True, 'defaultValue': False, 'label': 'Paraná', 'validFor': 'AAAAAgAA', 'value': 'PR'}, {'active': True, 'defaultValue': False, 'label': 'Parma', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'PR'}, {'active': True, 'defaultValue': False, 'label': 'Pavia', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'PV'}, {'active': True, 'defaultValue': False, 'label': 'Pennsylvania', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'PA'}, {'active': True, 'defaultValue': False, 'label': 'Pernambuco', 'validFor': 'AAAAAgAA', 'value': 'PE'}, {'active': True, 'defaultValue': False, 'label': 'Perugia', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'PG'}, {'active': True, 'defaultValue': False, 'label': 'Pesaro and Urbino', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'PU'}, {'active': True, 'defaultValue': False, 'label': 'Pescara', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'PE'}, {'active': True, 'defaultValue': False, 'label': 'Piacenza', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'PC'}, {'active': True, 'defaultValue': False, 'label': 'Piauí', 'validFor': 'AAAAAgAA', 'value': 'PI'}, {'active': True, 'defaultValue': False, 'label': 'Pisa', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'PI'}, {'active': True, 'defaultValue': False, 'label': 'Pistoia', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'PT'}, {'active': True, 'defaultValue': False, 'label': 'Pordenone', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'PN'}, {'active': True, 'defaultValue': False, 'label': 'Potenza', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'PZ'}, {'active': True, 'defaultValue': False, 'label': 'Prato', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'PO'}, {'active': True, 'defaultValue': False, 'label': 'Prince Edward Island', 'validFor': 'AAAAAAIA', 'value': 'PE'}, {'active': True, 'defaultValue': False, 'label': 'Puducherry', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'PY'}, {'active': True, 'defaultValue': False, 'label': 'Puebla', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'PB'}, {'active': True, 'defaultValue': False, 'label': 'Punjab', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'PB'}, {'active': True, 'defaultValue': False, 'label': 'Qinghai', 'validFor': 'AAAAAAAI', 'value': '63'}, {'active': True, 'defaultValue': False, 'label': 'Quebec', 'validFor': 'AAAAAAIA', 'value': 'QC'}, {'active': True, 'defaultValue': False, 'label': 'Queensland', 'validFor': 'AAgA', 'value': 'QLD'}, {'active': True, 'defaultValue': False, 'label': 'Querétaro', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'QE'}, {'active': True, 'defaultValue': False, 'label': 'Quintana Roo', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'QR'}, {'active': True, 'defaultValue': False, 'label': 'Ragusa', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'RG'}, {'active': True, 'defaultValue': False, 'label': 'Rajasthan', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'RJ'}, {'active': True, 'defaultValue': False, 'label': 'Ravenna', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'RA'}, {'active': True, 'defaultValue': False, 'label': 'Reggio Calabria', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'RC'}, {'active': True, 'defaultValue': False, 'label': 'Reggio Emilia', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'RE'}, {'active': True, 'defaultValue': False, 'label': 'Rhode Island', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'RI'}, {'active': True, 'defaultValue': False, 'label': 'Rieti', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'RI'}, {'active': True, 'defaultValue': False, 'label': 'Rimini', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'RN'}, {'active': True, 'defaultValue': False, 'label': 'Rio de Janeiro', 'validFor': 'AAAAAgAA', 'value': 'RJ'}, {'active': True, 'defaultValue': False, 'label': 'Rio Grande do Norte', 'validFor': 'AAAAAgAA', 'value': 'RN'}, {'active': True, 'defaultValue': False, 'label': 'Rio Grande do Sul', 'validFor': 'AAAAAgAA', 'value': 'RS'}, {'active': True, 'defaultValue': False, 'label': 'Rome', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'RM'}, {'active': True, 'defaultValue': False, 'label': 'Rondônia', 'validFor': 'AAAAAgAA', 'value': 'RO'}, {'active': True, 'defaultValue': False, 'label': 'Roraima', 'validFor': 'AAAAAgAA', 'value': 'RR'}, {'active': True, 'defaultValue': False, 'label': 'Roscommon', 'validFor': 'AAAAAAAAAAAAAAAAAQAA', 'value': 'RN'}, {'active': True, 'defaultValue': False, 'label': 'Rovigo', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'RO'}, {'active': True, 'defaultValue': False, 'label': 'Salerno', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'SA'}, {'active': True, 'defaultValue': False, 'label': 'San Luis Potosí', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'SL'}, {'active': True, 'defaultValue': False, 'label': 'Santa Catarina', 'validFor': 'AAAAAgAA', 'value': 'SC'}, {'active': True, 'defaultValue': False, 'label': 'São Paulo', 'validFor': 'AAAAAgAA', 'value': 'SP'}, {'active': True, 'defaultValue': False, 'label': 'Saskatchewan', 'validFor': 'AAAAAAIA', 'value': 'SK'}, {'active': True, 'defaultValue': False, 'label': 'Sassari', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'SS'}, {'active': True, 'defaultValue': False, 'label': 'Savona', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'SV'}, {'active': True, 'defaultValue': False, 'label': 'Sergipe', 'validFor': 'AAAAAgAA', 'value': 'SE'}, {'active': True, 'defaultValue': False, 'label': 'Shaanxi', 'validFor': 'AAAAAAAI', 'value': '61'}, {'active': True, 'defaultValue': False, 'label': 'Shandong', 'validFor': 'AAAAAAAI', 'value': '37'}, {'active': True, 'defaultValue': False, 'label': 'Shanghai', 'validFor': 'AAAAAAAI', 'value': '31'}, {'active': True, 'defaultValue': False, 'label': 'Shanxi', 'validFor': 'AAAAAAAI', 'value': '14'}, {'active': True, 'defaultValue': False, 'label': 'Sichuan', 'validFor': 'AAAAAAAI', 'value': '51'}, {'active': True, 'defaultValue': False, 'label': 'Siena', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'SI'}, {'active': True, 'defaultValue': False, 'label': 'Sikkim', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'SK'}, {'active': True, 'defaultValue': False, 'label': 'Sinaloa', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'SI'}, {'active': True, 'defaultValue': False, 'label': 'Sligo', 'validFor': 'AAAAAAAAAAAAAAAAAQAA', 'value': 'SO'}, {'active': True, 'defaultValue': False, 'label': 'Sondrio', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'SO'}, {'active': True, 'defaultValue': False, 'label': 'Sonora', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'SO'}, {'active': True, 'defaultValue': False, 'label': 'South Australia', 'validFor': 'AAgA', 'value': 'SA'}, {'active': True, 'defaultValue': False, 'label': 'South Carolina', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'SC'}, {'active': True, 'defaultValue': False, 'label': 'South Dakota', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'SD'}, {'active': True, 'defaultValue': False, 'label': 'Syracuse', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'SR'}, {'active': True, 'defaultValue': False, 'label': 'Tabasco', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'TB'}, {'active': True, 'defaultValue': False, 'label': 'Taiwan', 'validFor': 'AAAAAAAI', 'value': '71'}, {'active': True, 'defaultValue': False, 'label': 'Tamaulipas', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'TM'}, {'active': True, 'defaultValue': False, 'label': 'Tamil Nadu', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'TN'}, {'active': True, 'defaultValue': False, 'label': 'Taranto', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'TA'}, {'active': True, 'defaultValue': False, 'label': 'Tasmania', 'validFor': 'AAgA', 'value': 'TAS'}, {'active': True, 'defaultValue': False, 'label': 'Telangana', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'TG'}, {'active': True, 'defaultValue': False, 'label': 'Tennessee', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'TN'}, {'active': True, 'defaultValue': False, 'label': 'Teramo', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'TE'}, {'active': True, 'defaultValue': False, 'label': 'Terni', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'TR'}, {'active': True, 'defaultValue': False, 'label': 'Texas', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'TX'}, {'active': True, 'defaultValue': False, 'label': 'Tianjin', 'validFor': 'AAAAAAAI', 'value': '12'}, {'active': True, 'defaultValue': False, 'label': 'Tipperary', 'validFor': 'AAAAAAAAAAAAAAAAAQAA', 'value': 'TA'}, {'active': True, 'defaultValue': False, 'label': 'Tlaxcala', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'TL'}, {'active': True, 'defaultValue': False, 'label': 'Tocantins', 'validFor': 'AAAAAgAA', 'value': 'TO'}, {'active': True, 'defaultValue': False, 'label': 'Trapani', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'TP'}, {'active': True, 'defaultValue': False, 'label': 'Trento', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'TN'}, {'active': True, 'defaultValue': False, 'label': 'Treviso', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'TV'}, {'active': True, 'defaultValue': False, 'label': 'Trieste', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'TS'}, {'active': True, 'defaultValue': False, 'label': 'Tripura', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'TR'}, {'active': True, 'defaultValue': False, 'label': 'Turin', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'TO'}, {'active': True, 'defaultValue': False, 'label': 'Udine', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'UD'}, {'active': True, 'defaultValue': False, 'label': 'Utah', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'UT'}, {'active': True, 'defaultValue': False, 'label': 'Uttarakhand', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'UT'}, {'active': True, 'defaultValue': False, 'label': 'Uttar Pradesh', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'UP'}, {'active': True, 'defaultValue': False, 'label': 'Varese', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'VA'}, {'active': True, 'defaultValue': False, 'label': 'Venice', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'VE'}, {'active': True, 'defaultValue': False, 'label': 'Veracruz', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'VE'}, {'active': True, 'defaultValue': False, 'label': 'Verbano-Cusio-Ossola', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'VB'}, {'active': True, 'defaultValue': False, 'label': 'Vercelli', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'VC'}, {'active': True, 'defaultValue': False, 'label': 'Vermont', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'VT'}, {'active': True, 'defaultValue': False, 'label': 'Verona', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'VR'}, {'active': True, 'defaultValue': False, 'label': 'Vibo Valentia', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'VV'}, {'active': True, 'defaultValue': False, 'label': 'Vicenza', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'VI'}, {'active': True, 'defaultValue': False, 'label': 'Victoria', 'validFor': 'AAgA', 'value': 'VIC'}, {'active': True, 'defaultValue': False, 'label': 'Virginia', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'VA'}, {'active': True, 'defaultValue': False, 'label': 'Viterbo', 'validFor': 'AAAAAAAAAAAAAAAAACAA', 'value': 'VT'}, {'active': True, 'defaultValue': False, 'label': 'Washington', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'WA'}, {'active': True, 'defaultValue': False, 'label': 'Waterford', 'validFor': 'AAAAAAAAAAAAAAAAAQAA', 'value': 'WD'}, {'active': True, 'defaultValue': False, 'label': 'West Bengal', 'validFor': 'AAAAAAAAAAAAAAAAEAAA', 'value': 'WB'}, {'active': True, 'defaultValue': False, 'label': 'Western Australia', 'validFor': 'AAgA', 'value': 'WA'}, {'active': True, 'defaultValue': False, 'label': 'Westmeath', 'validFor': 'AAAAAAAAAAAAAAAAAQAA', 'value': 'WH'}, {'active': True, 'defaultValue': False, 'label': 'West Virginia', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'WV'}, {'active': True, 'defaultValue': False, 'label': 'Wexford', 'validFor': 'AAAAAAAAAAAAAAAAAQAA', 'value': 'WX'}, {'active': True, 'defaultValue': False, 'label': 'Wicklow', 'validFor': 'AAAAAAAAAAAAAAAAAQAA', 'value': 'WW'}, {'active': True, 'defaultValue': False, 'label': 'Wisconsin', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'WI'}, {'active': True, 'defaultValue': False, 'label': 'Wyoming', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAA', 'value': 'WY'}, {'active': True, 'defaultValue': False, 'label': 'Xinjiang', 'validFor': 'AAAAAAAI', 'value': '65'}, {'active': True, 'defaultValue': False, 'label': 'Xizang', 'validFor': 'AAAAAAAI', 'value': '54'}, {'active': True, 'defaultValue': False, 'label': 'Yucatán', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'YU'}, {'active': True, 'defaultValue': False, 'label': 'Yukon Territories', 'validFor': 'AAAAAAIA', 'value': 'YT'}, {'active': True, 'defaultValue': False, 'label': 'Yunnan', 'validFor': 'AAAAAAAI', 'value': '53'}, {'active': True, 'defaultValue': False, 'label': 'Zacatecas', 'validFor': 'AAAAAAAAAAAAAAAAAAAAAAAQ', 'value': 'ZA'}, {'active': True, 'defaultValue': False, 'label': 'Zhejiang', 'validFor': 'AAAAAAAI', 'value': '33'}], 'polymorphicForeignKey': False, 'precision': 0, 'queryByDistance': False, 'referenceTargetField': None, 'referenceTo': [], 'relationshipName': None, 'relationshipOrder': None, 'restrictedDelete': False, 'restrictedPicklist': True, 'scale': 0, 'searchPrefilterable': False, 'soapType': 'xsd:string', 'sortable': True, 'type': 'picklist', 'unique': False, 'updateable': True, 'writeRequiresMasterRead': False}, {'aggregatable': True, 'aiPredictionField': False, 'autoNumber': False, 'byteLength': 30, 'calculated': False, 'calculatedFormula': None, 'cascadeDelete': False, 'caseSensitive': False, 'compoundFieldName': 'BillingAddress', 'controllerName': None, 'createable': True, 'custom': False, 'defaultValue': 'US', 'defaultValueFormula': None, 'defaultedOnCreate': True, 'dependentPicklist': False, 'deprecatedAndHidden': False, 'digits': 0, 'displayLocationInDecimal': False, 'encrypted': False, 'externalId': False, 'extraTypeInfo': None, 'filterable': True, 'filteredLookupInfo': None, 'formulaTreatNullNumberAsZero': False, 'groupable': True, 'highScaleNumber': False, 'htmlFormatted': False, 'idLookup': False, 'inlineHelpText': None, 'label': 'Billing Country Code', 'length': 10, 'mask': None, 'maskType': None, 'name': 'countryCode', 'nameField': False, 'namePointing': False, 'nillable': True, 'permissionable': True, 'picklistValues': [{'active': True, 'defaultValue': False, 'label': 'Afghanistan', 'validFor': None, 'value': 'AF'}, {'active': True, 'defaultValue': False, 'label': 'Aland Islands', 'validFor': None, 'value': 'AX'}, {'active': True, 'defaultValue': False, 'label': 'Albania', 'validFor': None, 'value': 'AL'}, {'active': True, 'defaultValue': False, 'label': 'Algeria', 'validFor': None, 'value': 'DZ'}, {'active': True, 'defaultValue': False, 'label': 'Andorra', 'validFor': None, 'value': 'AD'}, {'active': True, 'defaultValue': False, 'label': 'Angola', 'validFor': None, 'value': 'AO'}, {'active': True, 'defaultValue': False, 'label': 'Anguilla', 'validFor': None, 'value': 'AI'}, {'active': True, 'defaultValue': False, 'label': 'Antarctica', 'validFor': None, 'value': 'AQ'}, {'active': True, 'defaultValue': False, 'label': 'Antigua and Barbuda', 'validFor': None, 'value': 'AG'}, {'active': True, 'defaultValue': False, 'label': 'Argentina', 'validFor': None, 'value': 'AR'}, {'active': True, 'defaultValue': False, 'label': 'Armenia', 'validFor': None, 'value': 'AM'}, {'active': True, 'defaultValue': False, 'label': 'Aruba', 'validFor': None, 'value': 'AW'}, {'active': True, 'defaultValue': False, 'label': 'Australia', 'validFor': None, 'value': 'AU'}, {'active': True, 'defaultValue': False, 'label': 'Austria', 'validFor': None, 'value': 'AT'}, {'active': True, 'defaultValue': False, 'label': 'Azerbaijan', 'validFor': None, 'value': 'AZ'}, {'active': True, 'defaultValue': False, 'label': 'Bahamas', 'validFor': None, 'value': 'BS'}, {'active': True, 'defaultValue': False, 'label': 'Bahrain', 'validFor': None, 'value': 'BH'}, {'active': True, 'defaultValue': False, 'label': 'Bangladesh', 'validFor': None, 'value': 'BD'}, {'active': True, 'defaultValue': False, 'label': 'Barbados', 'validFor': None, 'value': 'BB'}, {'active': True, 'defaultValue': False, 'label': 'Belarus', 'validFor': None, 'value': 'BY'}, {'active': True, 'defaultValue': False, 'label': 'Belgium', 'validFor': None, 'value': 'BE'}, {'active': True, 'defaultValue': False, 'label': 'Belize', 'validFor': None, 'value': 'BZ'}, {'active': True, 'defaultValue': False, 'label': 'Benin', 'validFor': None, 'value': 'BJ'}, {'active': True, 'defaultValue': False, 'label': 'Bermuda', 'validFor': None, 'value': 'BM'}, {'active': True, 'defaultValue': False, 'label': 'Bhutan', 'validFor': None, 'value': 'BT'}, {'active': True, 'defaultValue': False, 'label': 'Bolivia, Plurinational State of', 'validFor': None, 'value': 'BO'}, {'active': True, 'defaultValue': False, 'label': 'Bonaire, Sint Eustatius and Saba', 'validFor': None, 'value': 'BQ'}, {'active': True, 'defaultValue': False, 'label': 'Bosnia and Herzegovina', 'validFor': None, 'value': 'BA'}, {'active': True, 'defaultValue': False, 'label': 'Botswana', 'validFor': None, 'value': 'BW'}, {'active': True, 'defaultValue': False, 'label': 'Bouvet Island', 'validFor': None, 'value': 'BV'}, {'active': True, 'defaultValue': False, 'label': 'Brazil', 'validFor': None, 'value': 'BR'}, {'active': True, 'defaultValue': False, 'label': 'British Indian Ocean Territory', 'validFor': None, 'value': 'IO'}, {'active': True, 'defaultValue': False, 'label': 'Brunei Darussalam', 'validFor': None, 'value': 'BN'}, {'active': True, 'defaultValue': False, 'label': 'Bulgaria', 'validFor': None, 'value': 'BG'}, {'active': True, 'defaultValue': False, 'label': 'Burkina Faso', 'validFor': None, 'value': 'BF'}, {'active': True, 'defaultValue': False, 'label': 'Burundi', 'validFor': None, 'value': 'BI'}, {'active': True, 'defaultValue': False, 'label': 'Cambodia', 'validFor': None, 'value': 'KH'}, {'active': True, 'defaultValue': False, 'label': 'Cameroon', 'validFor': None, 'value': 'CM'}, {'active': True, 'defaultValue': False, 'label': 'Canada', 'validFor': None, 'value': 'CA'}, {'active': True, 'defaultValue': False, 'label': 'Cape Verde', 'validFor': None, 'value': 'CV'}, {'active': True, 'defaultValue': False, 'label': 'Cayman Islands', 'validFor': None, 'value': 'KY'}, {'active': True, 'defaultValue': False, 'label': 'Central African Republic', 'validFor': None, 'value': 'CF'}, {'active': True, 'defaultValue': False, 'label': 'Chad', 'validFor': None, 'value': 'TD'}, {'active': True, 'defaultValue': False, 'label': 'Chile', 'validFor': None, 'value': 'CL'}, {'active': True, 'defaultValue': False, 'label': 'China', 'validFor': None, 'value': 'CN'}, {'active': True, 'defaultValue': False, 'label': 'Christmas Island', 'validFor': None, 'value': 'CX'}, {'active': True, 'defaultValue': False, 'label': 'Cocos (Keeling) Islands', 'validFor': None, 'value': 'CC'}, {'active': True, 'defaultValue': False, 'label': 'Colombia', 'validFor': None, 'value': 'CO'}, {'active': True, 'defaultValue': False, 'label': 'Comoros', 'validFor': None, 'value': 'KM'}, {'active': True, 'defaultValue': False, 'label': 'Congo', 'validFor': None, 'value': 'CG'}, {'active': True, 'defaultValue': False, 'label': 'Congo, the Democratic Republic of the', 'validFor': None, 'value': 'CD'}, {'active': True, 'defaultValue': False, 'label': 'Cook Islands', 'validFor': None, 'value': 'CK'}, {'active': True, 'defaultValue': False, 'label': 'Costa Rica', 'validFor': None, 'value': 'CR'}, {'active': True, 'defaultValue': False, 'label': "Cote d'Ivoire", 'validFor': None, 'value': 'CI'}, {'active': True, 'defaultValue': False, 'label': 'Croatia', 'validFor': None, 'value': 'HR'}, {'active': True, 'defaultValue': False, 'label': 'Cuba', 'validFor': None, 'value': 'CU'}, {'active': True, 'defaultValue': False, 'label': 'Curaçao', 'validFor': None, 'value': 'CW'}, {'active': True, 'defaultValue': False, 'label': 'Cyprus', 'validFor': None, 'value': 'CY'}, {'active': True, 'defaultValue': False, 'label': 'Czech Republic', 'validFor': None, 'value': 'CZ'}, {'active': True, 'defaultValue': False, 'label': 'Denmark', 'validFor': None, 'value': 'DK'}, {'active': True, 'defaultValue': False, 'label': 'Djibouti', 'validFor': None, 'value': 'DJ'}, {'active': True, 'defaultValue': False, 'label': 'Dominica', 'validFor': None, 'value': 'DM'}, {'active': True, 'defaultValue': False, 'label': 'Dominican Republic', 'validFor': None, 'value': 'DO'}, {'active': True, 'defaultValue': False, 'label': 'Ecuador', 'validFor': None, 'value': 'EC'}, {'active': True, 'defaultValue': False, 'label': 'Egypt', 'validFor': None, 'value': 'EG'}, {'active': True, 'defaultValue': False, 'label': 'El Salvador', 'validFor': None, 'value': 'SV'}, {'active': True, 'defaultValue': False, 'label': 'Equatorial Guinea', 'validFor': None, 'value': 'GQ'}, {'active': True, 'defaultValue': False, 'label': 'Eritrea', 'validFor': None, 'value': 'ER'}, {'active': True, 'defaultValue': False, 'label': 'Estonia', 'validFor': None, 'value': 'EE'}, {'active': True, 'defaultValue': False, 'label': 'Ethiopia', 'validFor': None, 'value': 'ET'}, {'active': True, 'defaultValue': False, 'label': 'Falkland Islands (Malvinas)', 'validFor': None, 'value': 'FK'}, {'active': True, 'defaultValue': False, 'label': 'Faroe Islands', 'validFor': None, 'value': 'FO'}, {'active': True, 'defaultValue': False, 'label': 'Fiji', 'validFor': None, 'value': 'FJ'}, {'active': True, 'defaultValue': False, 'label': 'Finland', 'validFor': None, 'value': 'FI'}, {'active': True, 'defaultValue': False, 'label': 'France', 'validFor': None, 'value': 'FR'}, {'active': True, 'defaultValue': False, 'label': 'French Guiana', 'validFor': None, 'value': 'GF'}, {'active': True, 'defaultValue': False, 'label': 'French Polynesia', 'validFor': None, 'value': 'PF'}, {'active': True, 'defaultValue': False, 'label': 'French Southern Territories', 'validFor': None, 'value': 'TF'}, {'active': True, 'defaultValue': False, 'label': 'Gabon', 'validFor': None, 'value': 'GA'}, {'active': True, 'defaultValue': False, 'label': 'Gambia', 'validFor': None, 'value': 'GM'}, {'active': True, 'defaultValue': False, 'label': 'Georgia', 'validFor': None, 'value': 'GE'}, {'active': True, 'defaultValue': False, 'label': 'Germany', 'validFor': None, 'value': 'DE'}, {'active': True, 'defaultValue': False, 'label': 'Ghana', 'validFor': None, 'value': 'GH'}, {'active': True, 'defaultValue': False, 'label': 'Gibraltar', 'validFor': None, 'value': 'GI'}, {'active': True, 'defaultValue': False, 'label': 'Greece', 'validFor': None, 'value': 'GR'}, {'active': True, 'defaultValue': False, 'label': 'Greenland', 'validFor': None, 'value': 'GL'}, {'active': True, 'defaultValue': False, 'label': 'Grenada', 'validFor': None, 'value': 'GD'}, {'active': True, 'defaultValue': False, 'label': 'Guadeloupe', 'validFor': None, 'value': 'GP'}, {'active': True, 'defaultValue': False, 'label': 'Guatemala', 'validFor': None, 'value': 'GT'}, {'active': True, 'defaultValue': False, 'label': 'Guernsey', 'validFor': None, 'value': 'GG'}, {'active': True, 'defaultValue': False, 'label': 'Guinea', 'validFor': None, 'value': 'GN'}, {'active': True, 'defaultValue': False, 'label': 'Guinea-Bissau', 'validFor': None, 'value': 'GW'}, {'active': True, 'defaultValue': False, 'label': 'Guyana', 'validFor': None, 'value': 'GY'}, {'active': True, 'defaultValue': False, 'label': 'Haiti', 'validFor': None, 'value': 'HT'}, {'active': True, 'defaultValue': False, 'label': 'Heard Island and McDonald Islands', 'validFor': None, 'value': 'HM'}, {'active': True, 'defaultValue': False, 'label': 'Holy See (Vatican City State)', 'validFor': None, 'value': 'VA'}, {'active': True, 'defaultValue': False, 'label': 'Honduras', 'validFor': None, 'value': 'HN'}, {'active': True, 'defaultValue': False, 'label': 'Hungary', 'validFor': None, 'value': 'HU'}, {'active': True, 'defaultValue': False, 'label': 'Iceland', 'validFor': None, 'value': 'IS'}, {'active': True, 'defaultValue': False, 'label': 'India', 'validFor': None, 'value': 'IN'}, {'active': True, 'defaultValue': False, 'label': 'Indonesia', 'validFor': None, 'value': 'ID'}, {'active': True, 'defaultValue': False, 'label': 'Iran, Islamic Republic of', 'validFor': None, 'value': 'IR'}, {'active': True, 'defaultValue': False, 'label': 'Iraq', 'validFor': None, 'value': 'IQ'}, {'active': True, 'defaultValue': False, 'label': 'Ireland', 'validFor': None, 'value': 'IE'}, {'active': True, 'defaultValue': False, 'label': 'Isle of Man', 'validFor': None, 'value': 'IM'}, {'active': True, 'defaultValue': False, 'label': 'Israel', 'validFor': None, 'value': 'IL'}, {'active': True, 'defaultValue': False, 'label': 'Italy', 'validFor': None, 'value': 'IT'}, {'active': True, 'defaultValue': False, 'label': 'Jamaica', 'validFor': None, 'value': 'JM'}, {'active': True, 'defaultValue': False, 'label': 'Japan', 'validFor': None, 'value': 'JP'}, {'active': True, 'defaultValue': False, 'label': 'Jersey', 'validFor': None, 'value': 'JE'}, {'active': True, 'defaultValue': False, 'label': 'Jordan', 'validFor': None, 'value': 'JO'}, {'active': True, 'defaultValue': False, 'label': 'Kazakhstan', 'validFor': None, 'value': 'KZ'}, {'active': True, 'defaultValue': False, 'label': 'Kenya', 'validFor': None, 'value': 'KE'}, {'active': True, 'defaultValue': False, 'label': 'Kiribati', 'validFor': None, 'value': 'KI'}, {'active': True, 'defaultValue': False, 'label': "Korea, Democratic People's Republic of", 'validFor': None, 'value': 'KP'}, {'active': True, 'defaultValue': False, 'label': 'Korea, Republic of', 'validFor': None, 'value': 'KR'}, {'active': True, 'defaultValue': False, 'label': 'Kuwait', 'validFor': None, 'value': 'KW'}, {'active': True, 'defaultValue': False, 'label': 'Kyrgyzstan', 'validFor': None, 'value': 'KG'}, {'active': True, 'defaultValue': False, 'label': "Lao People's Democratic Republic", 'validFor': None, 'value': 'LA'}, {'active': True, 'defaultValue': False, 'label': 'Latvia', 'validFor': None, 'value': 'LV'}, {'active': True, 'defaultValue': False, 'label': 'Lebanon', 'validFor': None, 'value': 'LB'}, {'active': True, 'defaultValue': False, 'label': 'Lesotho', 'validFor': None, 'value': 'LS'}, {'active': True, 'defaultValue': False, 'label': 'Liberia', 'validFor': None, 'value': 'LR'}, {'active': True, 'defaultValue': False, 'label': 'Libya', 'validFor': None, 'value': 'LY'}, {'active': True, 'defaultValue': False, 'label': 'Liechtenstein', 'validFor': None, 'value': 'LI'}, {'active': True, 'defaultValue': False, 'label': 'Lithuania', 'validFor': None, 'value': 'LT'}, {'active': True, 'defaultValue': False, 'label': 'Luxembourg', 'validFor': None, 'value': 'LU'}, {'active': True, 'defaultValue': False, 'label': 'Macao', 'validFor': None, 'value': 'MO'}, {'active': True, 'defaultValue': False, 'label': 'Macedonia, the former Yugoslav Republic of', 'validFor': None, 'value': 'MK'}, {'active': True, 'defaultValue': False, 'label': 'Madagascar', 'validFor': None, 'value': 'MG'}, {'active': True, 'defaultValue': False, 'label': 'Malawi', 'validFor': None, 'value': 'MW'}, {'active': True, 'defaultValue': False, 'label': 'Malaysia', 'validFor': None, 'value': 'MY'}, {'active': True, 'defaultValue': False, 'label': 'Maldives', 'validFor': None, 'value': 'MV'}, {'active': True, 'defaultValue': False, 'label': 'Mali', 'validFor': None, 'value': 'ML'}, {'active': True, 'defaultValue': False, 'label': 'Malta', 'validFor': None, 'value': 'MT'}, {'active': True, 'defaultValue': False, 'label': 'Martinique', 'validFor': None, 'value': 'MQ'}, {'active': True, 'defaultValue': False, 'label': 'Mauritania', 'validFor': None, 'value': 'MR'}, {'active': True, 'defaultValue': False, 'label': 'Mauritius', 'validFor': None, 'value': 'MU'}, {'active': True, 'defaultValue': False, 'label': 'Mayotte', 'validFor': None, 'value': 'YT'}, {'active': True, 'defaultValue': False, 'label': 'Mexico', 'validFor': None, 'value': 'MX'}, {'active': True, 'defaultValue': False, 'label': 'Moldova, Republic of', 'validFor': None, 'value': 'MD'}, {'active': True, 'defaultValue': False, 'label': 'Monaco', 'validFor': None, 'value': 'MC'}, {'active': True, 'defaultValue': False, 'label': 'Mongolia', 'validFor': None, 'value': 'MN'}, {'active': True, 'defaultValue': False, 'label': 'Montenegro', 'validFor': None, 'value': 'ME'}, {'active': True, 'defaultValue': False, 'label': 'Montserrat', 'validFor': None, 'value': 'MS'}, {'active': True, 'defaultValue': False, 'label': 'Morocco', 'validFor': None, 'value': 'MA'}, {'active': True, 'defaultValue': False, 'label': 'Mozambique', 'validFor': None, 'value': 'MZ'}, {'active': True, 'defaultValue': False, 'label': 'Myanmar', 'validFor': None, 'value': 'MM'}, {'active': True, 'defaultValue': False, 'label': 'Namibia', 'validFor': None, 'value': 'NA'}, {'active': True, 'defaultValue': False, 'label': 'Nauru', 'validFor': None, 'value': 'NR'}, {'active': True, 'defaultValue': False, 'label': 'Nepal', 'validFor': None, 'value': 'NP'}, {'active': True, 'defaultValue': False, 'label': 'Netherlands', 'validFor': None, 'value': 'NL'}, {'active': True, 'defaultValue': False, 'label': 'New Caledonia', 'validFor': None, 'value': 'NC'}, {'active': True, 'defaultValue': False, 'label': 'New Zealand', 'validFor': None, 'value': 'NZ'}, {'active': True, 'defaultValue': False, 'label': 'Nicaragua', 'validFor': None, 'value': 'NI'}, {'active': True, 'defaultValue': False, 'label': 'Niger', 'validFor': None, 'value': 'NE'}, {'active': True, 'defaultValue': False, 'label': 'Nigeria', 'validFor': None, 'value': 'NG'}, {'active': True, 'defaultValue': False, 'label': 'Niue', 'validFor': None, 'value': 'NU'}, {'active': True, 'defaultValue': False, 'label': 'Norfolk Island', 'validFor': None, 'value': 'NF'}, {'active': True, 'defaultValue': False, 'label': 'Norway', 'validFor': None, 'value': 'NO'}, {'active': True, 'defaultValue': False, 'label': 'Oman', 'validFor': None, 'value': 'OM'}, {'active': True, 'defaultValue': False, 'label': 'Pakistan', 'validFor': None, 'value': 'PK'}, {'active': True, 'defaultValue': False, 'label': 'Palestine', 'validFor': None, 'value': 'PS'}, {'active': True, 'defaultValue': False, 'label': 'Panama', 'validFor': None, 'value': 'PA'}, {'active': True, 'defaultValue': False, 'label': 'Papua New Guinea', 'validFor': None, 'value': 'PG'}, {'active': True, 'defaultValue': False, 'label': 'Paraguay', 'validFor': None, 'value': 'PY'}, {'active': True, 'defaultValue': False, 'label': 'Peru', 'validFor': None, 'value': 'PE'}, {'active': True, 'defaultValue': False, 'label': 'Philippines', 'validFor': None, 'value': 'PH'}, {'active': True, 'defaultValue': False, 'label': 'Pitcairn', 'validFor': None, 'value': 'PN'}, {'active': True, 'defaultValue': False, 'label': 'Poland', 'validFor': None, 'value': 'PL'}, {'active': True, 'defaultValue': False, 'label': 'Portugal', 'validFor': None, 'value': 'PT'}, {'active': True, 'defaultValue': False, 'label': 'Qatar', 'validFor': None, 'value': 'QA'}, {'active': True, 'defaultValue': False, 'label': 'Reunion', 'validFor': None, 'value': 'RE'}, {'active': True, 'defaultValue': False, 'label': 'Romania', 'validFor': None, 'value': 'RO'}, {'active': True, 'defaultValue': False, 'label': 'Russian Federation', 'validFor': None, 'value': 'RU'}, {'active': True, 'defaultValue': False, 'label': 'Rwanda', 'validFor': None, 'value': 'RW'}, {'active': True, 'defaultValue': False, 'label': 'Saint Barthélemy', 'validFor': None, 'value': 'BL'}, {'active': True, 'defaultValue': False, 'label': 'Saint Helena, Ascension and Tristan da Cunha', 'validFor': None, 'value': 'SH'}, {'active': True, 'defaultValue': False, 'label': 'Saint Kitts and Nevis', 'validFor': None, 'value': 'KN'}, {'active': True, 'defaultValue': False, 'label': 'Saint Lucia', 'validFor': None, 'value': 'LC'}, {'active': True, 'defaultValue': False, 'label': 'Saint Martin (French part)', 'validFor': None, 'value': 'MF'}, {'active': True, 'defaultValue': False, 'label': 'Saint Pierre and Miquelon', 'validFor': None, 'value': 'PM'}, {'active': True, 'defaultValue': False, 'label': 'Saint Vincent and the Grenadines', 'validFor': None, 'value': 'VC'}, {'active': True, 'defaultValue': False, 'label': 'Samoa', 'validFor': None, 'value': 'WS'}, {'active': True, 'defaultValue': False, 'label': 'San Marino', 'validFor': None, 'value': 'SM'}, {'active': True, 'defaultValue': False, 'label': 'Sao Tome and Principe', 'validFor': None, 'value': 'ST'}, {'active': True, 'defaultValue': False, 'label': 'Saudi Arabia', 'validFor': None, 'value': 'SA'}, {'active': True, 'defaultValue': False, 'label': 'Senegal', 'validFor': None, 'value': 'SN'}, {'active': True, 'defaultValue': False, 'label': 'Serbia', 'validFor': None, 'value': 'RS'}, {'active': True, 'defaultValue': False, 'label': 'Seychelles', 'validFor': None, 'value': 'SC'}, {'active': True, 'defaultValue': False, 'label': 'Sierra Leone', 'validFor': None, 'value': 'SL'}, {'active': True, 'defaultValue': False, 'label': 'Singapore', 'validFor': None, 'value': 'SG'}, {'active': True, 'defaultValue': False, 'label': 'Sint Maarten (Dutch part)', 'validFor': None, 'value': 'SX'}, {'active': True, 'defaultValue': False, 'label': 'Slovakia', 'validFor': None, 'value': 'SK'}, {'active': True, 'defaultValue': False, 'label': 'Slovenia', 'validFor': None, 'value': 'SI'}, {'active': True, 'defaultValue': False, 'label': 'Solomon Islands', 'validFor': None, 'value': 'SB'}, {'active': True, 'defaultValue': False, 'label': 'Somalia', 'validFor': None, 'value': 'SO'}, {'active': True, 'defaultValue': False, 'label': 'South Africa', 'validFor': None, 'value': 'ZA'}, {'active': True, 'defaultValue': False, 'label': 'South Georgia and the South Sandwich Islands', 'validFor': None, 'value': 'GS'}, {'active': True, 'defaultValue': False, 'label': 'South Sudan', 'validFor': None, 'value': 'SS'}, {'active': True, 'defaultValue': False, 'label': 'Spain', 'validFor': None, 'value': 'ES'}, {'active': True, 'defaultValue': False, 'label': 'Sri Lanka', 'validFor': None, 'value': 'LK'}, {'active': True, 'defaultValue': False, 'label': 'Sudan', 'validFor': None, 'value': 'SD'}, {'active': True, 'defaultValue': False, 'label': 'Suriname', 'validFor': None, 'value': 'SR'}, {'active': True, 'defaultValue': False, 'label': 'Svalbard and Jan Mayen', 'validFor': None, 'value': 'SJ'}, {'active': True, 'defaultValue': False, 'label': 'Swaziland', 'validFor': None, 'value': 'SZ'}, {'active': True, 'defaultValue': False, 'label': 'Sweden', 'validFor': None, 'value': 'SE'}, {'active': True, 'defaultValue': False, 'label': 'Switzerland', 'validFor': None, 'value': 'CH'}, {'active': True, 'defaultValue': False, 'label': 'Syrian Arab Republic', 'validFor': None, 'value': 'SY'}, {'active': True, 'defaultValue': False, 'label': 'Taiwan', 'validFor': None, 'value': 'TW'}, {'active': True, 'defaultValue': False, 'label': 'Tajikistan', 'validFor': None, 'value': 'TJ'}, {'active': True, 'defaultValue': False, 'label': 'Tanzania, United Republic of', 'validFor': None, 'value': 'TZ'}, {'active': True, 'defaultValue': False, 'label': 'Thailand', 'validFor': None, 'value': 'TH'}, {'active': True, 'defaultValue': False, 'label': 'Timor-Leste', 'validFor': None, 'value': 'TL'}, {'active': True, 'defaultValue': False, 'label': 'Togo', 'validFor': None, 'value': 'TG'}, {'active': True, 'defaultValue': False, 'label': 'Tokelau', 'validFor': None, 'value': 'TK'}, {'active': True, 'defaultValue': False, 'label': 'Tonga', 'validFor': None, 'value': 'TO'}, {'active': True, 'defaultValue': False, 'label': 'Trinidad and Tobago', 'validFor': None, 'value': 'TT'}, {'active': True, 'defaultValue': False, 'label': 'Tunisia', 'validFor': None, 'value': 'TN'}, {'active': True, 'defaultValue': False, 'label': 'Turkey', 'validFor': None, 'value': 'TR'}, {'active': True, 'defaultValue': False, 'label': 'Turkmenistan', 'validFor': None, 'value': 'TM'}, {'active': True, 'defaultValue': False, 'label': 'Turks and Caicos Islands', 'validFor': None, 'value': 'TC'}, {'active': True, 'defaultValue': False, 'label': 'Tuvalu', 'validFor': None, 'value': 'TV'}, {'active': True, 'defaultValue': False, 'label': 'Uganda', 'validFor': None, 'value': 'UG'}, {'active': True, 'defaultValue': False, 'label': 'Ukraine', 'validFor': None, 'value': 'UA'}, {'active': True, 'defaultValue': False, 'label': 'United Arab Emirates', 'validFor': None, 'value': 'AE'}, {'active': True, 'defaultValue': False, 'label': 'United Kingdom', 'validFor': None, 'value': 'GB'}, {'active': True, 'defaultValue': True, 'label': 'United States', 'validFor': None, 'value': 'US'}, {'active': True, 'defaultValue': False, 'label': 'Uruguay', 'validFor': None, 'value': 'UY'}, {'active': True, 'defaultValue': False, 'label': 'Uzbekistan', 'validFor': None, 'value': 'UZ'}, {'active': True, 'defaultValue': False, 'label': 'Vanuatu', 'validFor': None, 'value': 'VU'}, {'active': True, 'defaultValue': False, 'label': 'Venezuela, Bolivarian Republic of', 'validFor': None, 'value': 'VE'}, {'active': True, 'defaultValue': False, 'label': 'Vietnam', 'validFor': None, 'value': 'VN'}, {'active': True, 'defaultValue': False, 'label': 'Virgin Islands, British', 'validFor': None, 'value': 'VG'}, {'active': True, 'defaultValue': False, 'label': 'Wallis and Futuna', 'validFor': None, 'value': 'WF'}, {'active': True, 'defaultValue': False, 'label': 'Western Sahara', 'validFor': None, 'value': 'EH'}, {'active': True, 'defaultValue': False, 'label': 'Yemen', 'validFor': None, 'value': 'YE'}, {'active': True, 'defaultValue': False, 'label': 'Zambia', 'validFor': None, 'value': 'ZM'}, {'active': True, 'defaultValue': False, 'label': 'Zimbabwe', 'validFor': None, 'value': 'ZW'}], 'polymorphicForeignKey': False, 'precision': 0, 'queryByDistance': False, 'referenceTargetField': None, 'referenceTo': [], 'relationshipName': None, 'relationshipOrder': None, 'restrictedDelete': False, 'restrictedPicklist': True, 'scale': 0, 'searchPrefilterable': False, 'soapType': 'xsd:string', 'sortable': True, 'type': 'picklist', 'unique': False, 'updateable': True, 'writeRequiresMasterRead': False}, {'aggregatable': True, 'aiPredictionField': False, 'autoNumber': False, 'byteLength': 0, 'calculated': False, 'calculatedFormula': None, 'cascadeDelete': False, 'caseSensitive': False, 'compoundFieldName': 'BillingAddress', 'controllerName': None, 'createable': True, 'custom': False, 'defaultValue': None, 'defaultValueFormula': None, 'defaultedOnCreate': False, 'dependentPicklist': False, 'deprecatedAndHidden': False, 'digits': 0, 'displayLocationInDecimal': False, 'encrypted': False, 'externalId': False, 'extraTypeInfo': None, 'filterable': True, 'filteredLookupInfo': None, 'formulaTreatNullNumberAsZero': False, 'groupable': False, 'highScaleNumber': False, 'htmlFormatted': False, 'idLookup': False, 'inlineHelpText': None, 'label': 'Billing Latitude', 'length': 0, 'mask': None, 'maskType': None, 'name': 'latitude', 'nameField': False, 'namePointing': False, 'nillable': True, 'permissionable': True, 'picklistValues': [], 'polymorphicForeignKey': False, 'precision': 18, 'queryByDistance': False, 'referenceTargetField': None, 'referenceTo': [], 'relationshipName': None, 'relationshipOrder': None, 'restrictedDelete': False, 'restrictedPicklist': False, 'scale': 15, 'searchPrefilterable': False, 'soapType': 'xsd:double', 'sortable': True, 'type': 'double', 'unique': False, 'updateable': True, 'writeRequiresMasterRead': False}, {'aggregatable': True, 'aiPredictionField': False, 'autoNumber': False, 'byteLength': 0, 'calculated': False, 'calculatedFormula': None, 'cascadeDelete': False, 'caseSensitive': False, 'compoundFieldName': 'BillingAddress', 'controllerName': None, 'createable': True, 'custom': False, 'defaultValue': None, 'defaultValueFormula': None, 'defaultedOnCreate': False, 'dependentPicklist': False, 'deprecatedAndHidden': False, 'digits': 0, 'displayLocationInDecimal': False, 'encrypted': False, 'externalId': False, 'extraTypeInfo': None, 'filterable': True, 'filteredLookupInfo': None, 'formulaTreatNullNumberAsZero': False, 'groupable': False, 'highScaleNumber': False, 'htmlFormatted': False, 'idLookup': False, 'inlineHelpText': None, 'label': 'Billing Longitude', 'length': 0, 'mask': None, 'maskType': None, 'name': 'longitude', 'nameField': False, 'namePointing': False, 'nillable': True, 'permissionable': True, 'picklistValues': [], 'polymorphicForeignKey': False, 'precision': 18, 'queryByDistance': False, 'referenceTargetField': None, 'referenceTo': [], 'relationshipName': None, 'relationshipOrder': None, 'restrictedDelete': False, 'restrictedPicklist': False, 'scale': 15, 'searchPrefilterable': False, 'soapType': 'xsd:double', 'sortable': True, 'type': 'double', 'unique': False, 'updateable': True, 'writeRequiresMasterRead': False}, {'aggregatable': True, 'aiPredictionField': False, 'autoNumber': False, 'byteLength': 120, 'calculated': False, 'calculatedFormula': None, 'cascadeDelete': False, 'caseSensitive': False, 'compoundFieldName': 'BillingAddress', 'controllerName': None, 'createable': True, 'custom': False, 'defaultValue': None, 'defaultValueFormula': None, 'defaultedOnCreate': False, 'dependentPicklist': False, 'deprecatedAndHidden': False, 'digits': 0, 'displayLocationInDecimal': False, 'encrypted': False, 'externalId': False, 'extraTypeInfo': None, 'filterable': True, 'filteredLookupInfo': None, 'formulaTreatNullNumberAsZero': False, 'groupable': True, 'highScaleNumber': False, 'htmlFormatted': False, 'idLookup': False, 'inlineHelpText': None, 'label': 'Billing Geocode Accuracy', 'length': 40, 'mask': None, 'maskType': None, 'name': 'geocodeAccuracy', 'nameField': False, 'namePointing': False, 'nillable': True, 'permissionable': True, 'picklistValues': [{'active': True, 'defaultValue': False, 'label': 'Address', 'validFor': None, 'value': 'Address'}, {'active': True, 'defaultValue': False, 'label': 'NearAddress', 'validFor': None, 'value': 'NearAddress'}, {'active': True, 'defaultValue': False, 'label': 'Block', 'validFor': None, 'value': 'Block'}, {'active': True, 'defaultValue': False, 'label': 'Street', 'validFor': None, 'value': 'Street'}, {'active': True, 'defaultValue': False, 'label': 'ExtendedZip', 'validFor': None, 'value': 'ExtendedZip'}, {'active': True, 'defaultValue': False, 'label': 'Zip', 'validFor': None, 'value': 'Zip'}, {'active': True, 'defaultValue': False, 'label': 'Neighborhood', 'validFor': None, 'value': 'Neighborhood'}, {'active': True, 'defaultValue': False, 'label': 'City', 'validFor': None, 'value': 'City'}, {'active': True, 'defaultValue': False, 'label': 'County', 'validFor': None, 'value': 'County'}, {'active': True, 'defaultValue': False, 'label': 'State', 'validFor': None, 'value': 'State'}, {'active': True, 'defaultValue': False, 'label': 'Unknown', 'validFor': None, 'value': 'Unknown'}], 'polymorphicForeignKey': False, 'precision': 0, 'queryByDistance': False, 'referenceTargetField': None, 'referenceTo': [], 'relationshipName': None, 'relationshipOrder': None, 'restrictedDelete': False, 'restrictedPicklist': True, 'scale': 0, 'searchPrefilterable': False, 'soapType': 'xsd:string', 'sortable': True, 'type': 'picklist', 'unique': False, 'updateable': True, 'writeRequiresMasterRead': False}]
     type_map = {'boolean': bool, 'id': str, 'email': constr(regex=EMAIL_ADDRESS_REGEX), 'datetime': SFDateTime,
                 'textarea': str, 'int': Decimal,
                 'url': str, 'currency': Decimal, 'reference': str, 'date': date, 'picklist': str, 'string': str,
                 'double': Decimal, 'phone': str, 'address': object}
 
-    def __init__(self, sd: SalesforceServicesData):
+    def __init__(self, sd: RestAPI):
         self.sd = sd
         self.type_map['address'] = self._make_address_model(self.address_md_template)
 
     @staticmethod
     def to_snake_case(name):
         name = re.sub('(.)([A-Z][a-z]+)', r'\1_\2', name)
         name = re.sub('__([A-Z])', r'_\1', name)
```

### Comparing `salesforce-tools-0.1.9/setup.py` & `salesforce_tools-0.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['salesforce_tools']
+['salesforce_tools', 'salesforce_tools.async_sf']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Flask>=2.2.1,<3.0.0',
  'PyJWT>=2.4.0,<3.0.0',
- 'cryptography>=37.0.4,<38.0.0',
+ 'authlib>=1.1.0,<2.0.0',
+ 'cryptography>=41.0.2,<42.0.0',
  'flatten-json>=0.1.13,<0.2.0',
- 'pandas>=1.4.3,<2.0.0',
- 'pydantic>=1.9.2,<2.0.0',
+ 'httpx>=0.24.1,<0.25.0',
+ 'pydantic>=2.0,<3.0',
+ 'python-dateutil>=2.8.2,<3.0.0',
  'requests-oauthlib>=1.3.1,<2.0.0',
  'requests>=2.28.1,<3.0.0',
  'xmltodict>=0.13.0,<0.14.0']
 
 setup_kwargs = {
     'name': 'salesforce-tools',
-    'version': '0.1.9',
+    'version': '0.2.0',
     'description': 'Salesforce API tools',
-    'long_description': None,
+    'long_description': 'None',
     'author': 'David Manuel',
     'author_email': 'david@dcmanjr.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/dacmanj/salesforce-tools',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

