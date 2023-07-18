# Comparing `tmp/sap_xssec-4.0.0.tar.gz` & `tmp/sap_xssec-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sap_xssec-4.0.0.tar", last modified: Tue Jan 31 09:34:47 2023, max compression
+gzip compressed data, was "sap_xssec-4.0.1.tar", last modified: Tue Jul 18 14:42:24 2023, max compression
```

## Comparing `sap_xssec-4.0.0.tar` & `sap_xssec-4.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-01-31 09:34:47.000000 sap_xssec-4.0.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1787 2023-01-31 09:33:59.000000 sap_xssec-4.0.0/CHANGELOG.md
--rw-rw-r--   0 travis    (2000) travis    (2000)    11398 2023-01-31 09:33:59.000000 sap_xssec-4.0.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       58 2023-01-31 09:33:59.000000 sap_xssec-4.0.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     8415 2023-01-31 09:34:47.000000 sap_xssec-4.0.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     7348 2023-01-31 09:33:59.000000 sap_xssec-4.0.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-01-31 09:34:47.000000 sap_xssec-4.0.0/sap/
--rw-rw-r--   0 travis    (2000) travis    (2000)       87 2023-01-31 09:33:59.000000 sap_xssec-4.0.0/sap/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-01-31 09:34:47.000000 sap_xssec-4.0.0/sap/xssec/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1025 2023-01-31 09:33:59.000000 sap_xssec-4.0.0/sap/xssec/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      629 2023-01-31 09:33:59.000000 sap_xssec-4.0.0/sap/xssec/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3797 2023-01-31 09:33:59.000000 sap_xssec-4.0.0/sap/xssec/jwt_audience_validator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2026 2023-01-31 09:33:59.000000 sap_xssec-4.0.0/sap/xssec/jwt_validation_facade.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3513 2023-01-31 09:33:59.000000 sap_xssec-4.0.0/sap/xssec/key_cache.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2877 2023-01-31 09:33:59.000000 sap_xssec-4.0.0/sap/xssec/key_cache_v2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      379 2023-01-31 09:33:59.000000 sap_xssec-4.0.0/sap/xssec/key_tools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      315 2023-01-31 09:33:59.000000 sap_xssec-4.0.0/sap/xssec/security_context.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3631 2023-01-31 09:33:59.000000 sap_xssec-4.0.0/sap/xssec/security_context_ias.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    32226 2023-01-31 09:33:59.000000 sap_xssec-4.0.0/sap/xssec/security_context_xsuaa.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-01-31 09:34:47.000000 sap_xssec-4.0.0/sap_xssec.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8415 2023-01-31 09:34:47.000000 sap_xssec-4.0.0/sap_xssec.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      541 2023-01-31 09:34:47.000000 sap_xssec-4.0.0/sap_xssec.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-01-31 09:34:47.000000 sap_xssec-4.0.0/sap_xssec.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      105 2023-01-31 09:34:47.000000 sap_xssec-4.0.0/sap_xssec.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        4 2023-01-31 09:34:47.000000 sap_xssec-4.0.0/sap_xssec.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2023-01-31 09:34:47.000000 sap_xssec-4.0.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1962 2023-01-31 09:33:59.000000 sap_xssec-4.0.0/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2023-01-31 09:33:59.000000 sap_xssec-4.0.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:42:24.057095 sap_xssec-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-18 14:42:13.000000 sap_xssec-4.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-07-18 14:42:13.000000 sap_xssec-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-18 14:42:13.000000 sap_xssec-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-07-18 14:42:24.057095 sap_xssec-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6872 2023-07-18 14:42:13.000000 sap_xssec-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:42:24.053095 sap_xssec-4.0.1/sap/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-18 14:42:13.000000 sap_xssec-4.0.1/sap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:42:24.057095 sap_xssec-4.0.1/sap/xssec/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-18 14:42:13.000000 sap_xssec-4.0.1/sap/xssec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-18 14:42:13.000000 sap_xssec-4.0.1/sap/xssec/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-07-18 14:42:13.000000 sap_xssec-4.0.1/sap/xssec/jwt_audience_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-18 14:42:13.000000 sap_xssec-4.0.1/sap/xssec/jwt_validation_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-07-18 14:42:13.000000 sap_xssec-4.0.1/sap/xssec/key_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-18 14:42:13.000000 sap_xssec-4.0.1/sap/xssec/key_cache_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-18 14:42:13.000000 sap_xssec-4.0.1/sap/xssec/key_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-18 14:42:13.000000 sap_xssec-4.0.1/sap/xssec/security_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-07-18 14:42:13.000000 sap_xssec-4.0.1/sap/xssec/security_context_ias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32226 2023-07-18 14:42:13.000000 sap_xssec-4.0.1/sap/xssec/security_context_xsuaa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:42:24.057095 sap_xssec-4.0.1/sap_xssec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-07-18 14:42:23.000000 sap_xssec-4.0.1/sap_xssec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-18 14:42:24.000000 sap_xssec-4.0.1/sap_xssec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:42:23.000000 sap_xssec-4.0.1/sap_xssec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-18 14:42:23.000000 sap_xssec-4.0.1/sap_xssec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-18 14:42:23.000000 sap_xssec-4.0.1/sap_xssec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-18 14:42:24.057095 sap_xssec-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-18 14:42:13.000000 sap_xssec-4.0.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 14:42:13.000000 sap_xssec-4.0.1/version.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sap_xssec-4.0.0/CHANGELOG.md` & `sap_xssec-4.0.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # Change Log
 All notable changes to this project will be documented in this file.
 
 This project adheres to [Semantic Versioning](http://semver.org/).
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/).
 
+## 4.0.1
+### Fixed
+- Bug: fix `aud` validation for IAS tokens
+
 ## 4.0.0
 ### Removed
-- Removed suport for sap_py_jwt.
+- Removed suport for sap_py_jwt
 
 ## 3.3.0
 ### Added
 
 - Added IAS support
 
 ## 3.2.0
```

### Comparing `sap_xssec-4.0.0/LICENSE` & `sap_xssec-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sap_xssec-4.0.0/PKG-INFO` & `sap_xssec-4.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,161 +1,157 @@
 Metadata-Version: 2.1
 Name: sap_xssec
-Version: 4.0.0
+Version: 4.0.1
 Summary: SAP Python Security Library
 Home-page: https://github.com/SAP/cloud-pysec
 Author: SAP SE
+License: UNKNOWN
+Description: [![REUSE status](https://api.reuse.software/badge/github.com/SAP/cloud-pysec)](https://api.reuse.software/info/github.com/SAP/cloud-pysec)
+        
+        # Description
+        This project is a python client library called *sap_xssec* for validation of *OAuth access tokens* issued by the *XSUAA*. 
+        
+        ### OAuth Authorization Code Flow
+        The typical web application use the OAuth authorization code flow for authentication, which is described as follows:
+        1. A user accesses the web application using a browser.
+        2. The web application (in typical SAP Cloud Platform applications, this is an application router) acts as OAuth client and redirects
+        to the OAuth server for authorization.
+        3. Upon authentication, the web application uses the code issued by the authorization server to request an access token.
+        4. The web application uses the access token to request data from the OAuth resource server.
+        The OAuth resource server validates the token using online or offline validation.
+        For this validation libraries like sap_xssec are used.
+        
+        
+        ![alt text](https://raw.githubusercontent.com/SAP/cloud-security-xsuaa-integration/1.4.0/images/oauth.png "OAuth authorization code flow")
+        
+        
+        ### Usage
+        
+        For the usage of this library it is necessary to pass a JWT access token that should be validated to the library.
+        The examples below rely on users and credentials that you should substitute with the ones in your context.
+        
+        The typical use case for calling this API lies from within a container when an HTTP request is received and it must 
+        be checked if the requester is authorized to execute this method.
+        In this case, the access token is contained in the authorization header (with keyword `bearer`).
+        You can remove the prefix `bearer` and pass the remaining string (just as in the following example as `access_token`) to the API.
+        
+        ```python
+        from sap import xssec
+        from cfenv import AppEnv
+        
+        env = AppEnv()
+        uaa_service = env.get_service(name='<uaa_service_name>').credentials
+        
+        security_context = xssec.create_security_context(access_token, uaa_service)
+        ```
+        
+        **Note:** That the example above uses module [`cfenv`](https://pypi.python.org/pypi/cfenv) to retrieve the configuration of the uaa
+        service instance.
+        `uaa_service` is a dict that contains the necessary client information and looks like:
+        ```
+        {
+            'clientid' : 'example_clientid'               // the id of the client
+            'clientsecret': 'example_clientsecret'        // the secret of the client
+            'url': 'example_url'                          // the url of the uaa
+            'uaadomain': 'example_uaadomain'              // the domain of the uaa
+            'verificationkey': 'example_verification key' // (optional) the key used for the verfication of the token
+        }
+        
+        ```
+        If the `uaadomain` is set in the `uaa_service` and the `jku` and `kid` are set in the incomming token, the key is requested from the uaa. As a fallback, the `verificationkey` configured in `uaa_service` is used for offline validation. Requested keys are cached for 15 minutes to avoid extensive load on the uaa.
+        
+        The creation function `xssec.create_security_context` is to be used for an end-user token (e.g. for grant_type `password`
+         or grant_type `authorization_code`) where user information is expected to be available within the token and thus within the security context.
+        
+        `create_security_context` also accepts a token of grant_type `client_credentials`.
+        This leads to the creation of a limited *SecurityContext* where certain functions are not available.
+        For more details please consult the API description in the wiki.
+        
+        For example, the `security_context` object can then be used to check if a user has a required scope:
+        
+        ``` 
+        security_context.check_scope('uaa.user')
+        ```
+        
+        or to receive the client id of a user:
+        
+        ``` 
+        security_context.get_clientid()
+        ```
+        
+        More details on the API can be found in the [wiki](https://github.com/SAP/cloud-pysec/wiki).
+        ### Offline Validation
+        
+        sap_xssec offers offline validation of the access token, which requires no additional call to the UAA.
+        The trust for this offline validation is created by binding the XS UAA service instance to your application.
+        Inside the credentials section in the environment variable `VCAP_SERVICES`, the key for validation of tokens is included.
+        By default, the offline validation check will only accept tokens intended for the same OAuth2 client in the same UAA identity zone.
+        This makes sense and will cover the vast majority of use cases.
+        
+        ⚠️From version 2.1.0, the `SAP_JWT_TRUST_ACL` environment variable is no longer supported.
+        
+        If you want to enable another (foreign) application to use some of your application's scopes, you can add a ```granted-apps``` marker to your scope in the ```xs-security.json``` file (as in the following example). The value of the marker is a list of applications that is allowed to request a token with the denoted scope.
+        
+        ```JSON
+        {
+          "xsappname"     : "sample-leave-request-app",
+          "description"   : "This sample application demos leave requests",
+          "scopes"        : [ { "name"                : "$XSAPPNAME.createLR",
+                                "description"         : "create leave requests" },
+                              { "name"                : "$XSAPPNAME.approveLR",
+                                "description"         : "approve leave requests",
+                                "granted-apps"        : ["MobileApprovals"] }
+                            ],
+          "attributes"    : [ { "name"                : "costcenter",
+                                "description"         : "costcenter",
+                                "valueType"           : "string"
+                            } ],
+          "role-templates": [ { "name"                : "employee",
+                                "description"         : "Role for creating leave requests",
+                                "scope-references"    : [ "$XSAPPNAME.createLR","JobScheduler.scheduleJobs" ],
+                                "attribute-references": [ "costcenter"] },
+                              { "name"                : "manager",
+                                "description"         : "Role for creating and approving leave requests",
+                                "scope-references"    : [ "$XSAPPNAME.createLR","$XSAPPNAME.approveLR","JobScheduler.scheduleJobs" ],
+                                "attribute-references": [ "costcenter" ] }
+                            ]
+        }
+        ```
+        
+        # Configuration
+        ~~To configure whether the *sap-jwt* or the *py-jwt* library should be used for validation of the jwt token, 
+        change the `USE_SAP_PY_JWT` environment variable to `true`.~~
+        
+        ⚠️From version 4.0.0, the `USE_SAP_PY_JWT` environment variable is no longer supported and therefore *py-jwt* is installed by default.
+        
+        # Requirements
+        *sap_xssec* requires *python 3.7* or newer.
+        
+        
+        # Download and Installation
+        As this package is deployed to PyPI, you can simply add `sap_xssec` as a dependency to your python project or 
+        install this package by running `pip install sap_xssec`.
+        
+        # Known Issues
+        # How to obtain support
+        Open an issue in GitHub.
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![REUSE status](https://api.reuse.software/badge/github.com/SAP/cloud-pysec)](https://api.reuse.software/info/github.com/SAP/cloud-pysec)
-
-# Description
-This project is a python client library called *sap_xssec* for validation of *OAuth access tokens* issued by the *XSUAA*. 
-
-### OAuth Authorization Code Flow
-The typical web application use the OAuth authorization code flow for authentication, which is described as follows:
-1. A user accesses the web application using a browser.
-2. The web application (in typical SAP Cloud Platform applications, this is an application router) acts as OAuth client and redirects
-to the OAuth server for authorization.
-3. Upon authentication, the web application uses the code issued by the authorization server to request an access token.
-4. The web application uses the access token to request data from the OAuth resource server.
-The OAuth resource server validates the token using online or offline validation.
-For this validation libraries like sap_xssec are used.
-
-
-![alt text](https://raw.githubusercontent.com/SAP/cloud-security-xsuaa-integration/1.4.0/images/oauth.png "OAuth authorization code flow")
-
-
-### Usage
-
-For the usage of this library it is necessary to pass a JWT access token that should be validated to the library.
-The examples below rely on users and credentials that you should substitute with the ones in your context.
-
-The typical use case for calling this API lies from within a container when an HTTP request is received and it must 
-be checked if the requester is authorized to execute this method.
-In this case, the access token is contained in the authorization header (with keyword `bearer`).
-You can remove the prefix `bearer` and pass the remaining string (just as in the following example as `access_token`) to the API.
-
-```python
-from sap import xssec
-from cfenv import AppEnv
-
-env = AppEnv()
-uaa_service = env.get_service(name='<uaa_service_name>').credentials
-
-security_context = xssec.create_security_context(access_token, uaa_service)
-```
-
-**Note:** That the example above uses module [`cfenv`](https://pypi.python.org/pypi/cfenv) to retrieve the configuration of the uaa
-service instance.
-`uaa_service` is a dict that contains the necessary client information and looks like:
-```
-{
-    'clientid' : 'example_clientid'               // the id of the client
-    'clientsecret': 'example_clientsecret'        // the secret of the client
-    'url': 'example_url'                          // the url of the uaa
-    'uaadomain': 'example_uaadomain'              // the domain of the uaa
-    'verificationkey': 'example_verification key' // (optional) the key used for the verfication of the token
-}
-
-```
-If the `uaadomain` is set in the `uaa_service` and the `jku` and `kid` are set in the incomming token, the key is requested from the uaa. As a fallback, the `verificationkey` configured in `uaa_service` is used for offline validation. Requested keys are cached for 15 minutes to avoid extensive load on the uaa.
-
-The creation function `xssec.create_security_context` is to be used for an end-user token (e.g. for grant_type `password`
- or grant_type `authorization_code`) where user information is expected to be available within the token and thus within the security context.
-
-`create_security_context` also accepts a token of grant_type `client_credentials`.
-This leads to the creation of a limited *SecurityContext* where certain functions are not available.
-For more details please consult the API description in the wiki.
-
-For example, the `security_context` object can then be used to check if a user has a required scope:
-
-``` 
-security_context.check_scope('uaa.user')
-```
-
-or to receive the client id of a user:
-
-``` 
-security_context.get_clientid()
-```
-
-More details on the API can be found in the [wiki](https://github.com/SAP/cloud-pysec/wiki).
-### Offline Validation
-
-sap_xssec offers offline validation of the access token, which requires no additional call to the UAA.
-The trust for this offline validation is created by binding the XS UAA service instance to your application.
-Inside the credentials section in the environment variable `VCAP_SERVICES`, the key for validation of tokens is included.
-By default, the offline validation check will only accept tokens intended for the same OAuth2 client in the same UAA identity zone.
-This makes sense and will cover the vast majority of use cases.
-
-~~However, if an application absolutely wants to consume token that were issued for either different OAuth2 clients or different identity zones,
- an *Access Control List (ACL)* entry for this can be specified in an environment variable named `SAP_JWT_TRUST_ACL`.
- The name of the OAuth client has then the prefix `sb-`, the content is a JSON String, containing an array of identity zones and OAuth2 clients.
- To trust any OAuth2 client and/or identity zones, an * can be used.~~
- 
-⚠️From version 2.1.0, the `SAP_JWT_TRUST_ACL` environment variable is no longer supported.
-
-
-If you want to enable another (foreign) application to use some of your application's scopes, you can add a ```granted-apps``` marker to your scope in the ```xs-security.json``` file (as in the following example). The value of the marker is a list of applications that is allowed to request a token with the denoted scope.
-
-```JSON
-{
-  "xsappname"     : "sample-leave-request-app",
-  "description"   : "This sample application demos leave requests",
-  "scopes"        : [ { "name"                : "$XSAPPNAME.createLR",
-                        "description"         : "create leave requests" },
-                      { "name"                : "$XSAPPNAME.approveLR",
-                        "description"         : "approve leave requests",
-                        "granted-apps"        : ["MobileApprovals"] }
-                    ],
-  "attributes"    : [ { "name"                : "costcenter",
-                        "description"         : "costcenter",
-                        "valueType"           : "string"
-                    } ],
-  "role-templates": [ { "name"                : "employee",
-                        "description"         : "Role for creating leave requests",
-                        "scope-references"    : [ "$XSAPPNAME.createLR","JobScheduler.scheduleJobs" ],
-                        "attribute-references": [ "costcenter"] },
-                      { "name"                : "manager",
-                        "description"         : "Role for creating and approving leave requests",
-                        "scope-references"    : [ "$XSAPPNAME.createLR","$XSAPPNAME.approveLR","JobScheduler.scheduleJobs" ],
-                        "attribute-references": [ "costcenter" ] }
-                    ]
-}
-```
-
-# Configuration
-~~To configure whether the *sap-jwt* or the *py-jwt* library should be used for validation of the jwt token, 
-change the `USE_SAP_PY_JWT` environment variable to `true`.~~
-
-⚠️From version 4.0.0, the `USE_SAP_PY_JWT` environment variable is no longer supported and therefore only *py-jwt* is supported.
-
-# Requirements
-*sap_xssec* requires *python 3.6* or newer.
-
-
-# Download and Installation
-As this package is deployed to PyPI, you can simply add `sap_xssec` as a dependency to your python project or 
-install this package by running `pip install sap_xssec`.
-
-# Known Issues
-# How to obtain support
-Open an issue in GitHub.
```

### Comparing `sap_xssec-4.0.0/README.md` & `sap_xssec-4.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -76,22 +76,16 @@
 
 sap_xssec offers offline validation of the access token, which requires no additional call to the UAA.
 The trust for this offline validation is created by binding the XS UAA service instance to your application.
 Inside the credentials section in the environment variable `VCAP_SERVICES`, the key for validation of tokens is included.
 By default, the offline validation check will only accept tokens intended for the same OAuth2 client in the same UAA identity zone.
 This makes sense and will cover the vast majority of use cases.
 
-~~However, if an application absolutely wants to consume token that were issued for either different OAuth2 clients or different identity zones,
- an *Access Control List (ACL)* entry for this can be specified in an environment variable named `SAP_JWT_TRUST_ACL`.
- The name of the OAuth client has then the prefix `sb-`, the content is a JSON String, containing an array of identity zones and OAuth2 clients.
- To trust any OAuth2 client and/or identity zones, an * can be used.~~
- 
 ⚠️From version 2.1.0, the `SAP_JWT_TRUST_ACL` environment variable is no longer supported.
 
-
 If you want to enable another (foreign) application to use some of your application's scopes, you can add a ```granted-apps``` marker to your scope in the ```xs-security.json``` file (as in the following example). The value of the marker is a list of applications that is allowed to request a token with the denoted scope.
 
 ```JSON
 {
   "xsappname"     : "sample-leave-request-app",
   "description"   : "This sample application demos leave requests",
   "scopes"        : [ { "name"                : "$XSAPPNAME.createLR",
@@ -116,18 +110,18 @@
 }
 ```
 
 # Configuration
 ~~To configure whether the *sap-jwt* or the *py-jwt* library should be used for validation of the jwt token, 
 change the `USE_SAP_PY_JWT` environment variable to `true`.~~
 
-⚠️From version 4.0.0, the `USE_SAP_PY_JWT` environment variable is no longer supported and therefore only *py-jwt* is supported.
+⚠️From version 4.0.0, the `USE_SAP_PY_JWT` environment variable is no longer supported and therefore *py-jwt* is installed by default.
 
 # Requirements
-*sap_xssec* requires *python 3.6* or newer.
+*sap_xssec* requires *python 3.7* or newer.
 
 
 # Download and Installation
 As this package is deployed to PyPI, you can simply add `sap_xssec` as a dependency to your python project or 
 install this package by running `pip install sap_xssec`.
 
 # Known Issues
```

### Comparing `sap_xssec-4.0.0/sap/xssec/__init__.py` & `sap_xssec-4.0.1/sap/xssec/__init__.py`

 * *Files identical despite different names*

### Comparing `sap_xssec-4.0.0/sap/xssec/constants.py` & `sap_xssec-4.0.1/sap/xssec/constants.py`

 * *Files identical despite different names*

### Comparing `sap_xssec-4.0.0/sap/xssec/jwt_audience_validator.py` & `sap_xssec-4.0.1/sap/xssec/jwt_audience_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,26 +42,26 @@
     def clientid(self, clientId):
         self._clientid = clientId
 
     def configure_trusted_clientId(self, client_id):
         if client_id:
             self.trusted_clientids.add(client_id)
 
-    def validate_token(self, clientId_from_token=None, audiences_from_token= [], scopes_from_token = []):
+    def validate_token(self, clientId_from_token=None, audiences_from_token=[], scopes_from_token=[]):
         self.is_foreign_mode = False
         allowed_audiences = self.extract_audiences_from_token(audiences_from_token, scopes_from_token, clientId_from_token)
         if (self.validate_same_clientId(clientId_from_token) == True or
                 self.validate_audience_of_xsuaabrokerclone(allowed_audiences) == True or
                 self.validate_default(allowed_audiences)==True):
             return True
         else:
             return False
 
 
-    def extract_audiences_from_token(self, audiences_from_token= [], scopes_from_token= [], clientid_from_token=None):
+    def extract_audiences_from_token(self, audiences_from_token=[], scopes_from_token=[], clientid_from_token=None):
         '''
         Extracts Audience From Token
         '''
         audiences = []
         token_audiences = audiences_from_token
         for audience in token_audiences:
             if audience.find(self.DOT) > -1:
```

### Comparing `sap_xssec-4.0.0/sap/xssec/jwt_validation_facade.py` & `sap_xssec-4.0.1/sap/xssec/jwt_validation_facade.py`

 * *Files identical despite different names*

### Comparing `sap_xssec-4.0.0/sap/xssec/key_cache.py` & `sap_xssec-4.0.1/sap/xssec/key_cache.py`

 * *Files identical despite different names*

### Comparing `sap_xssec-4.0.0/sap/xssec/key_cache_v2.py` & `sap_xssec-4.0.1/sap/xssec/key_cache_v2.py`

 * *Files identical despite different names*

### Comparing `sap_xssec-4.0.0/sap/xssec/security_context_ias.py` & `sap_xssec-4.0.1/sap/xssec/security_context_ias.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,19 @@
             raise ValueError("Token has expired")
         return self
 
     def validate_audience(self):
         """
         check `aud` in jwt token
         """
-        validation_result = self.audience_validator.validate_token(audiences_from_token=self.token_payload["aud"])
+
+        # Make sure `aud` is a list
+        aud = [self.token_payload["aud"]] if isinstance(self.token_payload["aud"], str) else self.token_payload["aud"]
+        
+        validation_result = self.audience_validator.validate_token(audiences_from_token=aud)
         if validation_result is False:
             raise RuntimeError('Audience Validation Failed')
         return self
 
     def validate_signature(self):
         """
         check signature in jwt token
```

### Comparing `sap_xssec-4.0.0/sap/xssec/security_context_xsuaa.py` & `sap_xssec-4.0.1/sap/xssec/security_context_xsuaa.py`

 * *Files identical despite different names*

### Comparing `sap_xssec-4.0.0/sap_xssec.egg-info/PKG-INFO` & `sap_xssec-4.0.1/sap_xssec.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,161 +1,157 @@
 Metadata-Version: 2.1
 Name: sap-xssec
-Version: 4.0.0
+Version: 4.0.1
 Summary: SAP Python Security Library
 Home-page: https://github.com/SAP/cloud-pysec
 Author: SAP SE
+License: UNKNOWN
+Description: [![REUSE status](https://api.reuse.software/badge/github.com/SAP/cloud-pysec)](https://api.reuse.software/info/github.com/SAP/cloud-pysec)
+        
+        # Description
+        This project is a python client library called *sap_xssec* for validation of *OAuth access tokens* issued by the *XSUAA*. 
+        
+        ### OAuth Authorization Code Flow
+        The typical web application use the OAuth authorization code flow for authentication, which is described as follows:
+        1. A user accesses the web application using a browser.
+        2. The web application (in typical SAP Cloud Platform applications, this is an application router) acts as OAuth client and redirects
+        to the OAuth server for authorization.
+        3. Upon authentication, the web application uses the code issued by the authorization server to request an access token.
+        4. The web application uses the access token to request data from the OAuth resource server.
+        The OAuth resource server validates the token using online or offline validation.
+        For this validation libraries like sap_xssec are used.
+        
+        
+        ![alt text](https://raw.githubusercontent.com/SAP/cloud-security-xsuaa-integration/1.4.0/images/oauth.png "OAuth authorization code flow")
+        
+        
+        ### Usage
+        
+        For the usage of this library it is necessary to pass a JWT access token that should be validated to the library.
+        The examples below rely on users and credentials that you should substitute with the ones in your context.
+        
+        The typical use case for calling this API lies from within a container when an HTTP request is received and it must 
+        be checked if the requester is authorized to execute this method.
+        In this case, the access token is contained in the authorization header (with keyword `bearer`).
+        You can remove the prefix `bearer` and pass the remaining string (just as in the following example as `access_token`) to the API.
+        
+        ```python
+        from sap import xssec
+        from cfenv import AppEnv
+        
+        env = AppEnv()
+        uaa_service = env.get_service(name='<uaa_service_name>').credentials
+        
+        security_context = xssec.create_security_context(access_token, uaa_service)
+        ```
+        
+        **Note:** That the example above uses module [`cfenv`](https://pypi.python.org/pypi/cfenv) to retrieve the configuration of the uaa
+        service instance.
+        `uaa_service` is a dict that contains the necessary client information and looks like:
+        ```
+        {
+            'clientid' : 'example_clientid'               // the id of the client
+            'clientsecret': 'example_clientsecret'        // the secret of the client
+            'url': 'example_url'                          // the url of the uaa
+            'uaadomain': 'example_uaadomain'              // the domain of the uaa
+            'verificationkey': 'example_verification key' // (optional) the key used for the verfication of the token
+        }
+        
+        ```
+        If the `uaadomain` is set in the `uaa_service` and the `jku` and `kid` are set in the incomming token, the key is requested from the uaa. As a fallback, the `verificationkey` configured in `uaa_service` is used for offline validation. Requested keys are cached for 15 minutes to avoid extensive load on the uaa.
+        
+        The creation function `xssec.create_security_context` is to be used for an end-user token (e.g. for grant_type `password`
+         or grant_type `authorization_code`) where user information is expected to be available within the token and thus within the security context.
+        
+        `create_security_context` also accepts a token of grant_type `client_credentials`.
+        This leads to the creation of a limited *SecurityContext* where certain functions are not available.
+        For more details please consult the API description in the wiki.
+        
+        For example, the `security_context` object can then be used to check if a user has a required scope:
+        
+        ``` 
+        security_context.check_scope('uaa.user')
+        ```
+        
+        or to receive the client id of a user:
+        
+        ``` 
+        security_context.get_clientid()
+        ```
+        
+        More details on the API can be found in the [wiki](https://github.com/SAP/cloud-pysec/wiki).
+        ### Offline Validation
+        
+        sap_xssec offers offline validation of the access token, which requires no additional call to the UAA.
+        The trust for this offline validation is created by binding the XS UAA service instance to your application.
+        Inside the credentials section in the environment variable `VCAP_SERVICES`, the key for validation of tokens is included.
+        By default, the offline validation check will only accept tokens intended for the same OAuth2 client in the same UAA identity zone.
+        This makes sense and will cover the vast majority of use cases.
+        
+        ⚠️From version 2.1.0, the `SAP_JWT_TRUST_ACL` environment variable is no longer supported.
+        
+        If you want to enable another (foreign) application to use some of your application's scopes, you can add a ```granted-apps``` marker to your scope in the ```xs-security.json``` file (as in the following example). The value of the marker is a list of applications that is allowed to request a token with the denoted scope.
+        
+        ```JSON
+        {
+          "xsappname"     : "sample-leave-request-app",
+          "description"   : "This sample application demos leave requests",
+          "scopes"        : [ { "name"                : "$XSAPPNAME.createLR",
+                                "description"         : "create leave requests" },
+                              { "name"                : "$XSAPPNAME.approveLR",
+                                "description"         : "approve leave requests",
+                                "granted-apps"        : ["MobileApprovals"] }
+                            ],
+          "attributes"    : [ { "name"                : "costcenter",
+                                "description"         : "costcenter",
+                                "valueType"           : "string"
+                            } ],
+          "role-templates": [ { "name"                : "employee",
+                                "description"         : "Role for creating leave requests",
+                                "scope-references"    : [ "$XSAPPNAME.createLR","JobScheduler.scheduleJobs" ],
+                                "attribute-references": [ "costcenter"] },
+                              { "name"                : "manager",
+                                "description"         : "Role for creating and approving leave requests",
+                                "scope-references"    : [ "$XSAPPNAME.createLR","$XSAPPNAME.approveLR","JobScheduler.scheduleJobs" ],
+                                "attribute-references": [ "costcenter" ] }
+                            ]
+        }
+        ```
+        
+        # Configuration
+        ~~To configure whether the *sap-jwt* or the *py-jwt* library should be used for validation of the jwt token, 
+        change the `USE_SAP_PY_JWT` environment variable to `true`.~~
+        
+        ⚠️From version 4.0.0, the `USE_SAP_PY_JWT` environment variable is no longer supported and therefore *py-jwt* is installed by default.
+        
+        # Requirements
+        *sap_xssec* requires *python 3.7* or newer.
+        
+        
+        # Download and Installation
+        As this package is deployed to PyPI, you can simply add `sap_xssec` as a dependency to your python project or 
+        install this package by running `pip install sap_xssec`.
+        
+        # Known Issues
+        # How to obtain support
+        Open an issue in GitHub.
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![REUSE status](https://api.reuse.software/badge/github.com/SAP/cloud-pysec)](https://api.reuse.software/info/github.com/SAP/cloud-pysec)
-
-# Description
-This project is a python client library called *sap_xssec* for validation of *OAuth access tokens* issued by the *XSUAA*. 
-
-### OAuth Authorization Code Flow
-The typical web application use the OAuth authorization code flow for authentication, which is described as follows:
-1. A user accesses the web application using a browser.
-2. The web application (in typical SAP Cloud Platform applications, this is an application router) acts as OAuth client and redirects
-to the OAuth server for authorization.
-3. Upon authentication, the web application uses the code issued by the authorization server to request an access token.
-4. The web application uses the access token to request data from the OAuth resource server.
-The OAuth resource server validates the token using online or offline validation.
-For this validation libraries like sap_xssec are used.
-
-
-![alt text](https://raw.githubusercontent.com/SAP/cloud-security-xsuaa-integration/1.4.0/images/oauth.png "OAuth authorization code flow")
-
-
-### Usage
-
-For the usage of this library it is necessary to pass a JWT access token that should be validated to the library.
-The examples below rely on users and credentials that you should substitute with the ones in your context.
-
-The typical use case for calling this API lies from within a container when an HTTP request is received and it must 
-be checked if the requester is authorized to execute this method.
-In this case, the access token is contained in the authorization header (with keyword `bearer`).
-You can remove the prefix `bearer` and pass the remaining string (just as in the following example as `access_token`) to the API.
-
-```python
-from sap import xssec
-from cfenv import AppEnv
-
-env = AppEnv()
-uaa_service = env.get_service(name='<uaa_service_name>').credentials
-
-security_context = xssec.create_security_context(access_token, uaa_service)
-```
-
-**Note:** That the example above uses module [`cfenv`](https://pypi.python.org/pypi/cfenv) to retrieve the configuration of the uaa
-service instance.
-`uaa_service` is a dict that contains the necessary client information and looks like:
-```
-{
-    'clientid' : 'example_clientid'               // the id of the client
-    'clientsecret': 'example_clientsecret'        // the secret of the client
-    'url': 'example_url'                          // the url of the uaa
-    'uaadomain': 'example_uaadomain'              // the domain of the uaa
-    'verificationkey': 'example_verification key' // (optional) the key used for the verfication of the token
-}
-
-```
-If the `uaadomain` is set in the `uaa_service` and the `jku` and `kid` are set in the incomming token, the key is requested from the uaa. As a fallback, the `verificationkey` configured in `uaa_service` is used for offline validation. Requested keys are cached for 15 minutes to avoid extensive load on the uaa.
-
-The creation function `xssec.create_security_context` is to be used for an end-user token (e.g. for grant_type `password`
- or grant_type `authorization_code`) where user information is expected to be available within the token and thus within the security context.
-
-`create_security_context` also accepts a token of grant_type `client_credentials`.
-This leads to the creation of a limited *SecurityContext* where certain functions are not available.
-For more details please consult the API description in the wiki.
-
-For example, the `security_context` object can then be used to check if a user has a required scope:
-
-``` 
-security_context.check_scope('uaa.user')
-```
-
-or to receive the client id of a user:
-
-``` 
-security_context.get_clientid()
-```
-
-More details on the API can be found in the [wiki](https://github.com/SAP/cloud-pysec/wiki).
-### Offline Validation
-
-sap_xssec offers offline validation of the access token, which requires no additional call to the UAA.
-The trust for this offline validation is created by binding the XS UAA service instance to your application.
-Inside the credentials section in the environment variable `VCAP_SERVICES`, the key for validation of tokens is included.
-By default, the offline validation check will only accept tokens intended for the same OAuth2 client in the same UAA identity zone.
-This makes sense and will cover the vast majority of use cases.
-
-~~However, if an application absolutely wants to consume token that were issued for either different OAuth2 clients or different identity zones,
- an *Access Control List (ACL)* entry for this can be specified in an environment variable named `SAP_JWT_TRUST_ACL`.
- The name of the OAuth client has then the prefix `sb-`, the content is a JSON String, containing an array of identity zones and OAuth2 clients.
- To trust any OAuth2 client and/or identity zones, an * can be used.~~
- 
-⚠️From version 2.1.0, the `SAP_JWT_TRUST_ACL` environment variable is no longer supported.
-
-
-If you want to enable another (foreign) application to use some of your application's scopes, you can add a ```granted-apps``` marker to your scope in the ```xs-security.json``` file (as in the following example). The value of the marker is a list of applications that is allowed to request a token with the denoted scope.
-
-```JSON
-{
-  "xsappname"     : "sample-leave-request-app",
-  "description"   : "This sample application demos leave requests",
-  "scopes"        : [ { "name"                : "$XSAPPNAME.createLR",
-                        "description"         : "create leave requests" },
-                      { "name"                : "$XSAPPNAME.approveLR",
-                        "description"         : "approve leave requests",
-                        "granted-apps"        : ["MobileApprovals"] }
-                    ],
-  "attributes"    : [ { "name"                : "costcenter",
-                        "description"         : "costcenter",
-                        "valueType"           : "string"
-                    } ],
-  "role-templates": [ { "name"                : "employee",
-                        "description"         : "Role for creating leave requests",
-                        "scope-references"    : [ "$XSAPPNAME.createLR","JobScheduler.scheduleJobs" ],
-                        "attribute-references": [ "costcenter"] },
-                      { "name"                : "manager",
-                        "description"         : "Role for creating and approving leave requests",
-                        "scope-references"    : [ "$XSAPPNAME.createLR","$XSAPPNAME.approveLR","JobScheduler.scheduleJobs" ],
-                        "attribute-references": [ "costcenter" ] }
-                    ]
-}
-```
-
-# Configuration
-~~To configure whether the *sap-jwt* or the *py-jwt* library should be used for validation of the jwt token, 
-change the `USE_SAP_PY_JWT` environment variable to `true`.~~
-
-⚠️From version 4.0.0, the `USE_SAP_PY_JWT` environment variable is no longer supported and therefore only *py-jwt* is supported.
-
-# Requirements
-*sap_xssec* requires *python 3.6* or newer.
-
-
-# Download and Installation
-As this package is deployed to PyPI, you can simply add `sap_xssec` as a dependency to your python project or 
-install this package by running `pip install sap_xssec`.
-
-# Known Issues
-# How to obtain support
-Open an issue in GitHub.
```

### Comparing `sap_xssec-4.0.0/sap_xssec.egg-info/SOURCES.txt` & `sap_xssec-4.0.1/sap_xssec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sap_xssec-4.0.0/setup.py` & `sap_xssec-4.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,16 @@
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX",
         "Operating System :: POSIX :: BSD",
         "Operating System :: POSIX :: Linux",
         "Operating System :: Microsoft :: Windows",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
 )
```

