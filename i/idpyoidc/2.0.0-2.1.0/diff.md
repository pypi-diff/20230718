# Comparing `tmp/idpyoidc-2.0.0.tar.gz` & `tmp/idpyoidc-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idpyoidc-2.0.0.tar", last modified: Fri May  5 07:55:18 2023, max compression
+gzip compressed data, was "idpyoidc-2.1.0.tar", last modified: Tue Jul 18 08:04:12 2023, max compression
```

## Comparing `idpyoidc-2.0.0.tar` & `idpyoidc-2.1.0.tar`

### file list

```diff
@@ -1,287 +1,300 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.642208 idpyoidc-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-05-05 07:55:18.642208 idpyoidc-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:55:18.642208 idpyoidc-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.602207 idpyoidc-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.610207 idpyoidc-2.0.0/src/idpyoidc/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/claims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.610207 idpyoidc-2.0.0/src/idpyoidc/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.614207 idpyoidc-2.0.0/src/idpyoidc/client/claims/
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/claims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/claims/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/claims/oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/claims/transform.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22760 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/client_auth.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4369 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/configure.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12100 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/cookie.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/current.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/entity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1884 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.614207 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11485 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/access_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.614207 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/add_on/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/add_on/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/add_on/dpop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/add_on/identity_assurance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/add_on/pkce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/add_on/pushed_authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/add_on/status_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/client_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/refresh_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/resource_owner_password_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/server_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/token_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oauth2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.618207 idpyoidc-2.0.0/src/idpyoidc/client/oidc/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6312 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/access_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.618207 idpyoidc-2.0.0/src/idpyoidc/client/oidc/add_on/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/add_on/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14893 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/backchannel_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/check_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/check_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/end_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/provider_info_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/read_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/refresh_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/userinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/oidc/webfinger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.618207 idpyoidc-2.0.0/src/idpyoidc/client/provider/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/provider/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/provider/linkedin.py
--rw-r--r--   0 runner    (1001) docker     (123)    37660 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/rp_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    25118 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    12363 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/service_context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/state_interface.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9655 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/client/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9539 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/encrypter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/impexp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/item.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1166 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.618207 idpyoidc-2.0.0/src/idpyoidc/message/
--rw-r--r--   0 runner    (1001) docker     (123)    32638 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/message/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.618207 idpyoidc-2.0.0/src/idpyoidc/message/oauth2/
--rw-r--r--   0 runner    (1001) docker     (123)    20695 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/message/oauth2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/message/oauth2/device_authorization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.618207 idpyoidc-2.0.0/src/idpyoidc/message/oidc/
--rw-r--r--   0 runner    (1001) docker     (123)    41092 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/message/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/message/oidc/backchannel_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/message/oidc/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     8088 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.618207 idpyoidc-2.0.0/src/idpyoidc/server/
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/authn_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.618207 idpyoidc-2.0.0/src/idpyoidc/server/authz/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4191 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/authz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.622207 idpyoidc-2.0.0/src/idpyoidc/server/claims/
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/claims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/claims/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/claims/oidc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18698 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/client_authn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/client_configure.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18238 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/construct.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10319 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/cookie_handler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17179 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/endpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15939 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/endpoint_context.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1845 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/login_hint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.622207 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.622207 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/add_on/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/add_on/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/add_on/dpop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/add_on/extra_args.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    43800 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/introspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/pushed_authorization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/server_metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7650 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.622207 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token_helper/
--rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token_helper/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7566 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token_helper/access_token.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2854 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token_helper/client_credentials.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5239 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token_helper/refresh_token.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3657 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token_helper/resource_owner_password_credentials.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12739 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token_helper/token_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token_revocation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.622207 idpyoidc-2.0.0/src/idpyoidc/server/oidc/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.626207 idpyoidc-2.0.0/src/idpyoidc/server/oidc/add_on/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/add_on/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/add_on/custom_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/add_on/pkce.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/backchannel_authentication.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1154 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/discovery.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1084 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/provider_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/read_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)    18534 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/session.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1534 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.626207 idpyoidc-2.0.0/src/idpyoidc/server/oidc/token_helper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/token_helper/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7742 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/token_helper/access_token.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6452 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/token_helper/refresh_token.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/token_helper/token_exchange.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8215 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/oidc/userinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/scopes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.626207 idpyoidc-2.0.0/src/idpyoidc/server/session/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/session/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10348 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/session/claims.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/session/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    19990 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/session/grant.py
--rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/session/grant_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/session/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    18794 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/session/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/session/token.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/template_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.626207 idpyoidc-2.0.0/src/idpyoidc/server/token/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4168 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/token/exception.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5430 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/token/handler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10787 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/token/id_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/token/jwt_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.626207 idpyoidc-2.0.0/src/idpyoidc/server/user_authn/
--rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/user_authn/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5569 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/user_authn/authn_context.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11410 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/user_authn/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.626207 idpyoidc-2.0.0/src/idpyoidc/server/user_info/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2342 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/user_info/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4330 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/server/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/ssl_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.626207 idpyoidc-2.0.0/src/idpyoidc/storage/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8726 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/storage/abfile.py
--rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/time_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/src/idpyoidc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.610207 idpyoidc-2.0.0/src/idpyoidc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-05-05 07:55:18.000000 idpyoidc-2.0.0/src/idpyoidc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-05-05 07:55:18.000000 idpyoidc-2.0.0/src/idpyoidc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:55:18.000000 idpyoidc-2.0.0/src/idpyoidc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:55:18.000000 idpyoidc-2.0.0/src/idpyoidc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-05 07:55:18.000000 idpyoidc-2.0.0/src/idpyoidc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 07:55:18.000000 idpyoidc-2.0.0/src/idpyoidc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:18.642208 idpyoidc-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_01_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_03_time_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    15230 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_04_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    23147 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_05_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)    55382 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_06_oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_07_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    21649 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_08_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_09_work_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_11_impexp.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_12_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_13_dump_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_20_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_21_abfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_22_backchannel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_00_current.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_01_service_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_02_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_02b_entity_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_03_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_04_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_05_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    21456 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_06_client_authn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_10_entity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20658 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_12_client_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_14_service_context_impexp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_15_cookie.py
--rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_16_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_17_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_18_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_19_webfinger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_20_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)    50948 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_21_oidc_service.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8912 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_22_oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_23_pkce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_24_oic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_25_oauth2_cc_ropc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_26_read_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)    22154 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_27_conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)    40243 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_28_rp_handler_oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_29_pushed_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_30_rph_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_31_oauth2_persistent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5164 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_32_oidc_persistent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_40_dpop.py
--rw-r--r--   0 runner    (1001) docker     (123)    22931 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_41_rp_handler_persistent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_50_ciba.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_51_identity_assurance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_client_55_token_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_00_configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_00a_client_configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_01_claims.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_01_construct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_02_session_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_03_authz_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_04_session_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_05_token_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    18591 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_06_grant.py
--rw-r--r--   0 runner    (1001) docker     (123)     9968 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_07_sess_mngm_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    23551 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_08_id_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_09_authn_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    26303 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_10_session_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_11_session_manager_pairwise.py
--rw-r--r--   0 runner    (1001) docker     (123)    15796 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_12_session_life.py
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_13_user_authn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_14_userinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_15_login_hint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9101 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_16_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_16_endpoint_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    26790 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_17_client_authn.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5537 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_20a_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_20b_claims.py
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_20c_authz_handling.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25356 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_20d_client_authn.py
--rw-r--r--   0 runner    (1001) docker     (123)    21774 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_20e_jwt_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    18198 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_20f_userinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_20g_cookie_handler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2446 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_21_oidc_discovery_endpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3834 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_22_oidc_provider_config_endpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14660 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_23_oidc_registration_endpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28098 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_24_oauth2_authorization_endpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7926 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_24_oauth2_authorization_endpoint_jar.py
--rw-r--r--   0 runner    (1001) docker     (123)    24593 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_24_oauth2_resource_indicators.py
--rw-r--r--   0 runner    (1001) docker     (123)    39291 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_24_oauth2_token_endpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    55966 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_24_oidc_authorization_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_25_oauth2_cc_ropc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26880 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_26_oidc_userinfo_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    26745 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_30_oidc_end_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    19996 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_31_oauth2_introspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_32_oidc_read_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)    14918 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_33_oauth2_pkce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9960 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_34_oidc_sso.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    45234 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_35_oidc_token_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    61543 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_36_oauth2_token_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)    22365 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_38_oauth2_revocation_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_40_oauth2_pushed_authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)    17740 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_50_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_60_dpop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_server_61_add_on.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_tandem_08_oauth2_cc_ropc.py
--rw-r--r--   0 runner    (1001) docker     (123)    25517 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_tandem_10_oauth2_token_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:55:09.000000 idpyoidc-2.0.0/tests/test_y_actor_01.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.244511 idpyoidc-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-07-18 08:04:12.240511 idpyoidc-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 08:04:12.244511 idpyoidc-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.200510 idpyoidc-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.204511 idpyoidc-2.1.0/src/idpyoidc/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/claims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.208510 idpyoidc-2.1.0/src/idpyoidc/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.208510 idpyoidc-2.1.0/src/idpyoidc/client/claims/
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/claims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/claims/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/claims/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/claims/transform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22630 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/client_auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4302 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/configure.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12100 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/cookie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/entity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1884 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.212511 idpyoidc-2.1.0/src/idpyoidc/client/oauth2/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11816 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oauth2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oauth2/access_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.212511 idpyoidc-2.1.0/src/idpyoidc/client/oauth2/add_on/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oauth2/add_on/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oauth2/add_on/dpop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oauth2/add_on/identity_assurance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oauth2/add_on/jar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oauth2/add_on/par.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oauth2/add_on/pkce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oauth2/add_on/status_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oauth2/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oauth2/client_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oauth2/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oauth2/refresh_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oauth2/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oauth2/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oauth2/resource_owner_password_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oauth2/server_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27939 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oauth2/stand_alone_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oauth2/token_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oauth2/token_revocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oauth2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.212511 idpyoidc-2.1.0/src/idpyoidc/client/oidc/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6314 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oidc/access_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.212511 idpyoidc-2.1.0/src/idpyoidc/client/oidc/add_on/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oidc/add_on/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14653 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oidc/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oidc/backchannel_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oidc/check_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oidc/check_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oidc/end_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oidc/provider_info_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oidc/read_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oidc/refresh_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oidc/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oidc/userinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oidc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/oidc/webfinger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.212511 idpyoidc-2.1.0/src/idpyoidc/client/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/provider/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/provider/linkedin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21995 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/rp_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25685 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/service_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/state_interface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9672 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/client/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9539 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/encrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/impexp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/item.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1166 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.216511 idpyoidc-2.1.0/src/idpyoidc/message/
+-rw-r--r--   0 runner    (1001) docker     (123)    32638 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/message/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.216511 idpyoidc-2.1.0/src/idpyoidc/message/oauth2/
+-rw-r--r--   0 runner    (1001) docker     (123)    21297 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/message/oauth2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/message/oauth2/device_authorization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.216511 idpyoidc-2.1.0/src/idpyoidc/message/oidc/
+-rw-r--r--   0 runner    (1001) docker     (123)    41155 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/message/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/message/oidc/backchannel_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/message/oidc/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.216511 idpyoidc-2.1.0/src/idpyoidc/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/authn_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.216511 idpyoidc-2.1.0/src/idpyoidc/server/authz/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4169 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/authz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.216511 idpyoidc-2.1.0/src/idpyoidc/server/claims/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/claims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/claims/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/claims/oidc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18644 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/client_authn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/client_configure.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20789 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/construct.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10286 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/cookie_handler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17184 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/endpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16013 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/endpoint_context.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1902 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/login_hint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.220511 idpyoidc-2.1.0/src/idpyoidc/server/oauth2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oauth2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.220511 idpyoidc-2.1.0/src/idpyoidc/server/oauth2/add_on/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oauth2/add_on/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oauth2/add_on/dpop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oauth2/add_on/extra_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oauth2/add_on/pkce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43668 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oauth2/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oauth2/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oauth2/pushed_authorization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oauth2/server_metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7470 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oauth2/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.220511 idpyoidc-2.1.0/src/idpyoidc/server/oauth2/token_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oauth2/token_helper/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7751 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oauth2/token_helper/access_token.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2809 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oauth2/token_helper/client_credentials.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5219 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oauth2/token_helper/refresh_token.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3613 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oauth2/token_helper/resource_owner_password_credentials.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12602 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oauth2/token_helper/token_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oauth2/token_revocation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.220511 idpyoidc-2.1.0/src/idpyoidc/server/oidc/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oidc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.220511 idpyoidc-2.1.0/src/idpyoidc/server/oidc/add_on/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oidc/add_on/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oidc/add_on/custom_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oidc/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12426 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oidc/backchannel_authentication.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1154 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oidc/discovery.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1084 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oidc/provider_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oidc/read_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18736 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oidc/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15739 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oidc/session.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1534 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oidc/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.224511 idpyoidc-2.1.0/src/idpyoidc/server/oidc/token_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oidc/token_helper/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7700 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oidc/token_helper/access_token.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6398 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oidc/token_helper/refresh_token.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oidc/token_helper/token_exchange.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8193 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/oidc/userinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/scopes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.224511 idpyoidc-2.1.0/src/idpyoidc/server/session/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/session/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10510 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/session/claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/session/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19742 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/session/grant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/session/grant_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/session/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18326 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/session/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/session/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/template_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.224511 idpyoidc-2.1.0/src/idpyoidc/server/token/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4168 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/token/exception.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5382 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/token/handler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10788 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/token/id_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/token/jwt_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.224511 idpyoidc-2.1.0/src/idpyoidc/server/user_authn/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/user_authn/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5569 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/user_authn/authn_context.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11459 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/user_authn/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.224511 idpyoidc-2.1.0/src/idpyoidc/server/user_info/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2342 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/user_info/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4375 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/server/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/ssl_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.224511 idpyoidc-2.1.0/src/idpyoidc/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/storage/abfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/time_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/src/idpyoidc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.204511 idpyoidc-2.1.0/src/idpyoidc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-07-18 08:04:12.000000 idpyoidc-2.1.0/src/idpyoidc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-07-18 08:04:12.000000 idpyoidc-2.1.0/src/idpyoidc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 08:04:12.000000 idpyoidc-2.1.0/src/idpyoidc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 08:04:11.000000 idpyoidc-2.1.0/src/idpyoidc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-18 08:04:12.000000 idpyoidc-2.1.0/src/idpyoidc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 08:04:12.000000 idpyoidc-2.1.0/src/idpyoidc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:12.240511 idpyoidc-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_01_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_03_time_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15230 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_04_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23147 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_05_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55382 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_06_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_07_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17330 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_08_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_09_work_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_11_impexp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_12_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_13_dump_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_20_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_21_abfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_22_backchannel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_00_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_01_service_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_02_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_02b_entity_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_03_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_04_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_05_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21248 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_06_client_authn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_10_entity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20925 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_12_client_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_14_service_context_impexp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_15_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_16_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_17_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_18_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_19_webfinger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_20_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49595 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_21_oidc_service.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8892 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_22_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_23_pkce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_24_oic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_25_oauth2_cc_ropc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_26_read_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21072 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_27_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20299 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_28_stand_alone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_29_pushed_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40078 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_30_rp_handler_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_30_rph_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_31_oauth2_persistent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5123 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_32_oidc_persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_40_dpop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23217 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_41_rp_handler_persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_50_ciba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_51_identity_assurance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_client_55_token_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_00_configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_00a_client_configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9526 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_01_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_01_construct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_02_session_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_03_authz_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_04_session_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_05_token_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18567 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_06_grant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9875 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_07_sess_mngm_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23484 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_08_id_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_09_authn_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26484 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_10_session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_11_session_manager_pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15798 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_12_session_life.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_13_user_authn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_14_userinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_15_login_hint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9153 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_16_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_16_endpoint_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26669 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_17_client_authn.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5420 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_20a_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_20b_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_20c_authz_handling.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25252 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_20d_client_authn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21883 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_20e_jwt_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18326 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_20f_userinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_20g_cookie_handler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2446 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_21_oidc_discovery_endpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3832 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_22_oidc_provider_config_endpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14769 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_23_oidc_registration_endpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28095 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_24_oauth2_authorization_endpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7926 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_24_oauth2_authorization_endpoint_jar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24523 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_24_oauth2_resource_indicators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39072 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_24_oauth2_token_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36204 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_24_oauth2_token_endpoint_def_conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    53909 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_24_oidc_authorization_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_25_oauth2_cc_ropc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26781 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_26_oidc_userinfo_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26767 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_30_oidc_end_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20030 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_31_oauth2_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_32_oidc_read_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14853 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_33_oauth2_pkce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9850 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_34_oidc_sso.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45205 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_35_oidc_token_endpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35290 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_35_oidc_token_endpoint_def_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61177 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_36_oauth2_token_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22305 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_38_oauth2_revocation_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9308 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_40_oauth2_pushed_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17879 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_50_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_60_dpop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_server_61_add_on.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_tandem_oauth2_add_on.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_tandem_oauth2_cc_ropc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_tandem_oauth2_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25343 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_tandem_oauth2_token_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_tandem_oauth2_token_revocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10745 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_tandem_oidc_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:04:03.000000 idpyoidc-2.1.0/tests/test_y_actor_01.py
```

### Comparing `idpyoidc-2.0.0/LICENSE` & `idpyoidc-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/PKG-INFO` & `idpyoidc-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idpyoidc
-Version: 2.0.0
+Version: 2.1.0
 Summary: Python implementation of everything OAuth2 and OpenID Connect
 Home-page: https://github.com/IdentityPython/idpy-oidc/
 Author: Roland Hedberg
 Author-email: roland@catalogix.se
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `idpyoidc-2.0.0/README.md` & `idpyoidc-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/pyproject.toml` & `idpyoidc-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [metadata]
 name = "idpyoidc"
-version = "2.0.0"
+version = "2.1.0"
 author = "Roland Hedberg"
 author_email = "roland@catalogix.se"
 description = "Everything OAuth2 and OIDC"
 long_description = "file: README.md"
 long_description_content_type = "text/markdown"
 url = "https://github.com/IdentityPython/oidc-op"
 license = "Apache-2.0"
```

### Comparing `idpyoidc-2.0.0/setup.py` & `idpyoidc-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/__init__.py` & `idpyoidc-2.1.0/src/idpyoidc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Roland Hedberg"
-__version__ = "2.0.0"
+__version__ = "2.1.0"
 
 VERIFIED_CLAIM_PREFIX = "__verified"
 
 
 def verified_claim_name(claim):
     return "{}_{}".format(VERIFIED_CLAIM_PREFIX, claim)
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/claims.py` & `idpyoidc-2.1.0/src/idpyoidc/claims.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,26 +22,19 @@
     _class_name = list(item.keys())[0]  # there is only one
     _cls = importer(_class_name)
     _cls = _cls().load(item[_class_name])
     return _cls
 
 
 class Claims(ImpExp):
-    parameter = {
-        "prefer": None,
-        "use": None,
-        "callback_path": None,
-        "_local": None
-    }
+    parameter = {"prefer": None, "use": None, "callback_path": None, "_local": None}
 
     _supports = {}
 
-    def __init__(self,
-                 prefer: Optional[dict] = None,
-                 callback_path: Optional[dict] = None):
+    def __init__(self, prefer: Optional[dict] = None, callback_path: Optional[dict] = None):
 
         ImpExp.__init__(self)
         if isinstance(prefer, dict):
             self.prefer = {k: v for k, v in prefer.items() if k in self._supports}
         else:
             self.prefer = {}
 
@@ -66,58 +59,55 @@
 
     def remove_preference(self, key):
         if key in self.prefer:
             del self.prefer[key]
 
     def _callback_uris(self, base_url, hex):
         _uri = []
-        for type in self.get_usage("response_types", self._supports['response_types']):
+        for type in self.get_usage("response_types", self._supports["response_types"]):
             if "code" in type:
-                _uri.append('code')
-            elif type in ["id_token", "id_token token"]:
-                _uri.append('implicit')
+                _uri.append("code")
+            elif type in ["id_token"]:
+                _uri.append("implicit")
 
         if "form_post" in self._supports:
             _uri.append("form_post")
 
         callback_uri = {}
         for key in _uri:
             callback_uri[key] = get_uri(base_url, self.callback_path[key], hex)
         return callback_uri
 
-    def construct_redirect_uris(self,
-                                base_url: str,
-                                hex: str,
-                                callbacks: Optional[dict] = None):
+    def construct_redirect_uris(self, base_url: str, hex: str, callbacks: Optional[dict] = None):
         if not callbacks:
             callbacks = self._callback_uris(base_url, hex)
 
         if callbacks:
-            self.set_preference('callbacks', callbacks)
+            self.set_preference("callbacks", callbacks)
             self.set_preference("redirect_uris", [v for k, v in callbacks.items()])
 
         self.callback = callbacks
 
-    def verify_rules(self):
+    def verify_rules(self, supports):
         return True
 
     def locals(self, info):
         pass
 
     def _keyjar(self, keyjar=None, conf=None, entity_id=""):
-        _uri_path = ''
+        _uri_path = ""
         if keyjar is None:
             if "keys" in conf:
                 keys_args = {k: v for k, v in conf["keys"].items() if k != "uri_path"}
                 _keyjar = init_key_jar(**keys_args)
-                _uri_path = conf['keys'].get('uri_path')
+                _uri_path = conf["keys"].get("uri_path")
             elif "key_conf" in conf and conf["key_conf"]:
                 keys_args = {k: v for k, v in conf["key_conf"].items() if k != "uri_path"}
                 _keyjar = init_key_jar(**keys_args)
-                _uri_path = conf['key_conf'].get('uri_path')
+                _uri_path = conf["key_conf"].get("uri_path")
             else:
                 _keyjar = KeyJar()
                 if "jwks" in conf:
                     _keyjar.import_jwks(conf["jwks"], "")
 
             if "" in _keyjar and entity_id:
                 # make sure I have the keys under my own name too (if I know it)
@@ -125,17 +115,17 @@
 
             _httpc_params = conf.get("httpc_params")
             if _httpc_params:
                 _keyjar.httpc_params = _httpc_params
             return _keyjar, _uri_path
         else:
             if "keys" in conf:
-                _uri_path = conf['keys'].get('uri_path')
+                _uri_path = conf["keys"].get("uri_path")
             elif "key_conf" in conf and conf["key_conf"]:
-                _uri_path = conf['key_conf'].get('uri_path')
+                _uri_path = conf["key_conf"].get("uri_path")
 
         return keyjar, _uri_path
 
     def get_base_url(self, configuration: dict):
         raise NotImplementedError()
 
     def get_id(self, configuration: dict):
@@ -153,45 +143,44 @@
         keyjar, uri_path = self._keyjar(keyjar, configuration, entity_id=_id)
 
         _kj = self.add_extra_keys(keyjar, _id)
         if keyjar is None and _kj:
             keyjar = _kj
 
         # now that keys are in the Key Jar, now for how to publish it
-        if 'jwks_uri' in configuration:  # simple
-            _jwks_uri = configuration.get('jwks_uri')
+        if "jwks_uri" in configuration:  # simple
+            _jwks_uri = configuration.get("jwks_uri")
         elif uri_path:
             _base_url = self.get_base_url(configuration)
             _jwks_uri = add_path(_base_url, uri_path)
         else:  # jwks or nothing
             _jwks = self.get_jwks(keyjar)
 
-        return {'keyjar': keyjar, 'jwks': _jwks, 'jwks_uri': _jwks_uri}
+        return {"keyjar": keyjar, "jwks": _jwks, "jwks_uri": _jwks_uri}
 
-    def load_conf(self,
-                  configuration: dict,
-                  supports: dict,
-                  keyjar: Optional[KeyJar] = None) -> KeyJar:
+    def load_conf(
+        self, configuration: dict, supports: dict, keyjar: Optional[KeyJar] = None
+    ) -> KeyJar:
         for attr, val in configuration.items():
-            if attr == "preference":
+            if attr in ["preference", "capabilities"]:
                 for k, v in val.items():
                     if k in supports:
                         self.set_preference(k, v)
             elif attr in supports:
                 self.set_preference(attr, val)
 
         self.locals(configuration)
 
         for key, val in self.handle_keys(configuration, keyjar=keyjar).items():
-            if key == 'keyjar':
+            if key == "keyjar":
                 keyjar = val
             elif val:
                 self.set_preference(key, val)
 
-        self.verify_rules()
+        self.verify_rules(supports)
         return keyjar
 
     def get(self, key, default=None):
         if key in self._local:
             return self._local[key]
         else:
             return default
@@ -223,41 +212,45 @@
             _val = self.get_preference(key)
 
         if _val is None:
             return default
         else:
             return _val
 
-SIGNING_ALGORITHM_SORT_ORDER = ['RS', 'ES', 'PS', 'HS']
+
+SIGNING_ALGORITHM_SORT_ORDER = ["RS", "ES", "PS", "HS"]
 
 
 def cmp(a, b):
     return (a > b) - (a < b)
 
 
 def alg_cmp(a, b):
-    if a == 'none':
+    if a == "none":
         return 1
-    elif b == 'none':
+    elif b == "none":
         return -1
 
     _pos1 = SIGNING_ALGORITHM_SORT_ORDER.index(a[0:2])
     _pos2 = SIGNING_ALGORITHM_SORT_ORDER.index(b[0:2])
     if _pos1 == _pos2:
         return (a > b) - (a < b)
     elif _pos1 > _pos2:
         return 1
     else:
         return -1
 
 
 def get_signing_algs():
     # Assumes Cryptojwt
-    return sorted(list(SIGNER_ALGS.keys()), key=cmp_to_key(alg_cmp))
+    _list = list(SIGNER_ALGS.keys())
+    # know how to do none but should not
+    _list.remove("none")
+    return sorted(_list, key=cmp_to_key(alg_cmp))
 
 
 def get_encryption_algs():
-    return SUPPORTED['alg']
+    return SUPPORTED["alg"]
 
 
 def get_encryption_encs():
-    return SUPPORTED['enc']
+    return SUPPORTED["enc"]
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/claims/__init__.py` & `idpyoidc-2.1.0/src/idpyoidc/client/claims/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,55 +7,57 @@
 
 
 def get_client_authn_methods():
     return list(CLIENT_AUTHN_METHOD.keys())
 
 
 class Claims(claims.Claims):
-
     def get_base_url(self, configuration: dict):
-        _base = configuration.get('base_url')
+        _base = configuration.get("base_url")
         if not _base:
-            _base = configuration.get('client_id')
+            _base = configuration.get("client_id")
 
         return _base
 
     def get_id(self, configuration: dict):
-        return self.get_preference('client_id')
+        return self.get_preference("client_id")
 
     def _add_key_if_missing(self, keyjar, id, key):
         try:
             old_keys = keyjar.get_issuer_keys(id)
         except IssuerNotFound:
             old_keys = []
 
         _new_key = SYMKey(key=key)
         if _new_key not in old_keys:
             keyjar.add_symmetric(issuer_id=id, key=key)
 
     def add_extra_keys(self, keyjar, id):
-        _secret = self.get_preference('client_secret')
+        _secret = self.get_preference("client_secret")
         if _secret:
             if keyjar is None:
                 keyjar = KeyJar()
             self._add_key_if_missing(keyjar, id, _secret)
-            self._add_key_if_missing(keyjar, '', _secret)
+            self._add_key_if_missing(keyjar, "", _secret)
 
     def get_jwks(self, keyjar):
         if keyjar is None:
             return None
 
         _jwks = None
         try:
-            _own_keys = keyjar.get_issuer_keys('')
+            _own_keys = keyjar.get_issuer_keys("")
         except IssuerNotFound:
             pass
         else:
             # if only one key under the id == "", that key being a SYMKey I assume it's
             # and I have a client_secret then don't publish a JWKS
-            if len(_own_keys) == 1 and isinstance(_own_keys[0], SYMKey) and self.prefer[
-                    'client_secret']:
+            if (
+                len(_own_keys) == 1
+                and isinstance(_own_keys[0], SYMKey)
+                and self.prefer["client_secret"]
+            ):
                 pass
             else:
                 _jwks = keyjar.export_jwks()
 
         return _jwks
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/claims/oauth2.py` & `idpyoidc-2.1.0/src/idpyoidc/client/claims/oauth2.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,32 +6,30 @@
 
 class Claims(claims.Claims):
     _supports = {
         "redirect_uris": None,
         "grant_types_supported": ["authorization_code", "implicit", "refresh_token"],
         "response_types_supported": ["code"],
         "client_id": None,
-        'client_secret': None,
+        "client_secret": None,
         "client_name": None,
         "client_uri": None,
         "logo_uri": None,
         "contacts": None,
         "scopes_supported": [],
         "tos_uri": None,
         "policy_uri": None,
         "jwks_uri": None,
         "jwks": None,
         "software_id": None,
-        "software_version": None
+        "software_version": None,
     }
 
     callback_path = {}
 
     callback_uris = ["redirect_uris"]
 
-    def __init__(self,
-                 prefer: Optional[dict] = None,
-                 callback_path: Optional[dict] = None):
+    def __init__(self, prefer: Optional[dict] = None, callback_path: Optional[dict] = None):
         claims.Claims.__init__(self, prefer=prefer, callback_path=callback_path)
 
     def create_registration_request(self):
         return create_registration_request(self.prefer, self.supports())
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/claims/oidc.py` & `idpyoidc-2.1.0/src/idpyoidc/client/claims/oidc.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,32 +36,30 @@
     # 'claims_locales': 'claims_locales_supported',
     # 'ui_locales': 'ui_locales_supported',
 }
 
 PREFERRED2REGISTER = dict([(v, k) for k, v in REGISTER2PREFERRED.items()])
 
 REQUEST2REGISTER = {
-    'client_id': "client_id",
+    "client_id": "client_id",
     "client_secret": "client_secret",
     #    'acr_values': "default_acr_values" ,
     #    'max_age': "default_max_age",
-    'redirect_uri': "redirect_uris",
-    'response_type': "response_types",
-    'request_uri': "request_uris",
-    'grant_type': "grant_types",
-    "scope": 'scopes_supported',
-    'post_logout_redirect_uri': "post_logout_redirect_uris"
+    "redirect_uri": "redirect_uris",
+    "response_type": "response_types",
+    "request_uri": "request_uris",
+    "grant_type": "grant_types",
+    "scope": "scopes_supported",
+    "post_logout_redirect_uri": "post_logout_redirect_uris",
 }
 
 
 class Claims(client_claims.Claims):
     parameter = client_claims.Claims.parameter.copy()
-    parameter.update({
-        "requests_dir": None
-    })
+    parameter.update({"requests_dir": None})
 
     register2preferred = REGISTER2PREFERRED
     registration_response = RegistrationResponse
     registration_request = RegistrationRequest
 
     _supports = {
         "acr_values_supported": None,
@@ -88,40 +86,46 @@
         "require_auth_time": None,
         "sector_identifier_uri": None,
         "scopes_supported": ["openid"],
         "subject_types_supported": ["public", "pairwise", "ephemeral"],
         "tos_uri": None,
     }
 
-    def __init__(self,
-                 prefer: Optional[dict] = None,
-                 callback_path: Optional[dict] = None
-                 ):
-        client_claims.Claims.__init__(self,
-                                      prefer=prefer,
-                                      callback_path=callback_path)
+    def __init__(self, prefer: Optional[dict] = None, callback_path: Optional[dict] = None):
+        client_claims.Claims.__init__(self, prefer=prefer, callback_path=callback_path)
 
-    def verify_rules(self):
+    def verify_rules(self, supports):
         if self.get_preference("request_parameter_supported") and self.get_preference(
-                "request_uri_parameter_supported"):
+            "request_uri_parameter_supported"
+        ):
             raise ValueError(
                 "You have to chose one of 'request_parameter_supported' and "
-                "'request_uri_parameter_supported'. You can't have both.")
+                "'request_uri_parameter_supported'. You can't have both."
+            )
 
-        if not self.get_preference('encrypt_userinfo_supported'):
-            self.set_preference('userinfo_encryption_alg_values_supported', [])
-            self.set_preference('userinfo_encryption_enc_values_supported', [])
-
-        if not self.get_preference('encrypt_request_object_supported'):
-            self.set_preference('request_object_encryption_alg_values_supported', [])
-            self.set_preference('request_object_encryption_enc_values_supported', [])
-
-        if not self.get_preference('encrypt_id_token_supported'):
-            self.set_preference('id_token_encryption_alg_values_supported', [])
-            self.set_preference('id_token_encryption_enc_values_supported', [])
+        if self.get_preference("request_parameter_supported") or self.get_preference(
+            "request_uri_parameter_supported"
+        ):
+            if not self.get_preference("request_object_signing_alg_values_supported"):
+                self.set_preference(
+                    "request_object_signing_alg_values_supported",
+                    supports["request_object_signing_alg_values_supported"],
+                )
+
+        if not self.get_preference("encrypt_userinfo_supported"):
+            self.set_preference("userinfo_encryption_alg_values_supported", [])
+            self.set_preference("userinfo_encryption_enc_values_supported", [])
+
+        if not self.get_preference("encrypt_request_object_supported"):
+            self.set_preference("request_object_encryption_alg_values_supported", [])
+            self.set_preference("request_object_encryption_enc_values_supported", [])
+
+        if not self.get_preference("encrypt_id_token_supported"):
+            self.set_preference("id_token_encryption_alg_values_supported", [])
+            self.set_preference("id_token_encryption_enc_values_supported", [])
 
     def locals(self, info):
         requests_dir = info.get("requests_dir")
         if requests_dir:
             # make sure the path exists. If not, then create it.
             if not os.path.isdir(requests_dir):
                 os.makedirs(requests_dir)
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/claims/transform.py` & `idpyoidc-2.1.0/src/idpyoidc/client/claims/transform.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     "id_token_signed_response_alg": "id_token_signing_alg_values_supported",
     "id_token_encrypted_response_alg": "id_token_encryption_alg_values_supported",
     "id_token_encrypted_response_enc": "id_token_encryption_enc_values_supported",
     "default_acr_values": "acr_values_supported",
     "subject_type": "subject_types_supported",
     "token_endpoint_auth_method": "token_endpoint_auth_methods_supported",
     "response_types": "response_types_supported",
+    "response_modes": "response_modes_supported",
     "grant_types": "grant_types_supported",
     # In OAuth2 but not in OIDC
     "scope": "scopes_supported",
     "token_endpoint_auth_signing_alg": "token_endpoint_auth_signing_alg_values_supported",
     # "display": "display_values_supported",
     # "claims": "claims_supported",
     # "request": "request_parameter_supported",
@@ -32,63 +33,64 @@
     # 'claims_locales': 'claims_locales_supported',
     # 'ui_locales': 'ui_locales_supported',
 }
 
 PREFERRED2REGISTER = dict([(v, k) for k, v in REGISTER2PREFERRED.items()])
 
 REQUEST2REGISTER = {
-    'client_id': "client_id",
+    "client_id": "client_id",
     "client_secret": "client_secret",
     #    'acr_values': "default_acr_values" ,
     #    'max_age': "default_max_age",
-    'redirect_uri': "redirect_uris",
-    'response_type': "response_types",
-    'request_uri': "request_uris",
-    'grant_type': "grant_types",
-    "scope": 'scopes_supported',
-    'post_logout_redirect_uri': "post_logout_redirect_uris"
+    "redirect_uri": "redirect_uris",
+    "response_type": "response_types",
+    "request_uri": "request_uris",
+    "grant_type": "grant_types",
+    "scope": "scopes_supported",
+    "post_logout_redirect_uri": "post_logout_redirect_uris",
 }
 
 
-def supported_to_preferred(supported: dict,
-                           preference: dict,
-                           base_url: str,
-                           info: Optional[dict] = None,
-                           ):
+def supported_to_preferred(
+    supported: dict,
+    preference: dict,
+    base_url: str,
+    info: Optional[dict] = None,
+):
     if info:  # The provider info
         for key, val in supported.items():
             if key in preference:
                 _pref_val = preference.get(key)  # defined in configuration
                 _info_val = info.get(key)
                 if _info_val:
                     # Only use provider setting if less or equal to what I support
-                    if key.endswith('supported'):  # list
+                    if key.endswith("supported"):  # list
                         preference[key] = [x for x in _pref_val if x in _info_val]
                     else:
                         pass
             elif val is None:  # No default, means the RP does not have a preference
                 # if key not in ['jwks_uri', 'jwks']:
                 pass
             else:
                 # there is a default
                 _info_val = info.get(key)
                 if _info_val:  # The OP has an opinion
-                    if key.endswith('supported'):  # list
+                    if key.endswith("supported"):  # list
                         preference[key] = [x for x in val if x in _info_val]
                     else:
                         pass
                 else:
                     preference[key] = val
 
         # special case -> must have a request_uris value
-        if 'require_request_uri_registration' in info:
+        if "require_request_uri_registration" in info:
             # only makes sense if I want to use request_uri
-            if preference.get('request_parameter') == 'request_uri':
-                if 'request_uri' not in preference:
-                    preference['request_uris'] = [f'{base_url}/requests']
+            if preference.get("request_parameter") == "request_uri":
+                if "request_uri" not in preference:
+                    preference["request_uris"] = [f"{base_url}/requests"]
             else:  # just ignore
                 logger.info('Asked for "request_uri" which it did not plan to use')
     else:
         # Add defaults
         for key, val in supported.items():
             if val is None:
                 continue
@@ -117,14 +119,15 @@
         if isinstance(b, list):
             return set(a).issubset(set(b))
     elif isinstance(b, list):
         return a in b
     else:
         return a == b
 
+
 def _intersection(a, b):
     res = None
     if isinstance(a, list):
         if isinstance(b, list):
             res = list(set(a).intersection(set(b)))
         else:
             if b in a:
@@ -134,16 +137,18 @@
     elif isinstance(b, list):
         if a in b:
             res = [a]
         else:
             res = []
     return res
 
-def preferred_to_registered(prefers: dict, supported: dict,
-                            registration_response: Optional[dict] = None):
+
+def preferred_to_registered(
+    prefers: dict, supported: dict, registration_response: Optional[dict] = None
+):
     """
     The claims with values that are returned from the OP is what goes unless (!!)
     the values returned are not within the supported values.
 
     @param prefers:
     @param registration_response:
     @return:
@@ -155,21 +160,22 @@
             if key in REGISTER2PREFERRED:
                 # Is the response value with in what this instance supports
                 _supports = supported.get(REGISTER2PREFERRED[key])
                 if _is_subset(val, _supports):
                     registered[key] = val
                 else:
                     logger.warning(
-                        f'OP tells me to do something I do not support: {key} = {val} not within '
-                        f'{_supports}')
+                        f"OP tells me to do something I do not support: {key} = {val} not within "
+                        f"{_supports}"
+                    )
                     _val = _intersection(val, _supports)
                     if _val:
                         registered[key] = _val
                     else:
-                        raise ValueError(f'Not able to support the OPs choice: {key}={val}')
+                        raise ValueError(f"Not able to support the OPs choice: {key}={val}")
             else:
                 registered[key] = val  # Should I just accept with the OP says ??
 
     for key, spec in RegistrationResponse.c_param.items():
         if key in registered:
             continue
         _pref_key = REGISTER2PREFERRED.get(key, key)
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/client_auth.py` & `idpyoidc-2.1.0/src/idpyoidc/client/client_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     def _get_passwd(request, service, **kwargs):
         try:
             passwd = kwargs["password"]
         except KeyError:
             try:
                 passwd = request["client_secret"]
             except KeyError:
-                passwd = service.upstream_get("context").get_usage('client_secret')
+                passwd = service.upstream_get("context").get_usage("client_secret")
         return passwd
 
     @staticmethod
     def _get_user(service, **kwargs):
         try:
             user = kwargs["user"]
         except KeyError:
@@ -132,16 +132,16 @@
 
         If we're doing an access token request with an authorization code
         then we should add client_id to the request if it's not already there.
         :param request: A request
         :param service: A :py:class:`idpyoidc.client.service.Service` instance
         """
         if (
-                isinstance(request, AccessTokenRequest)
-                and request["grant_type"] == "authorization_code"
+            isinstance(request, AccessTokenRequest)
+            and request["grant_type"] == "authorization_code"
         ):
             if "client_id" not in request:
                 try:
                     request["client_id"] = service.upstream_get("context").get_client_id()
                 except AttributeError:
                     pass
         else:
@@ -219,15 +219,15 @@
         :param service: The service that is using this authentication method
         """
         _context = service.upstream_get("context")
         if "client_secret" not in request:
             try:
                 request["client_secret"] = kwargs["client_secret"]
             except (KeyError, TypeError):
-                request["client_secret"] = _context.get_usage('client_secret')
+                request["client_secret"] = _context.get_usage("client_secret")
                 if not request["client_secret"]:
                     raise AuthnFailure("Missing client secret")
 
         # Set the client_id in the the request
         request["client_id"] = _context.get_client_id()
 
     def construct(self, request, service=None, http_args=None, **kwargs):
@@ -438,17 +438,15 @@
     def _get_signing_key(self, algorithm, keyjar, key_types, kid=None):
         ktype = alg2keytype(algorithm)
         try:
             if kid:
                 signing_key = [self._get_key_by_kid(kid, algorithm, keyjar)]
             elif ktype in key_types:
                 try:
-                    signing_key = [
-                        self._get_key_by_kid(key_types[ktype], algorithm, keyjar)
-                    ]
+                    signing_key = [self._get_key_by_kid(key_types[ktype], algorithm, keyjar)]
                 except KeyError:
                     signing_key = self.get_signing_key_from_keyjar(algorithm, keyjar)
             else:
                 signing_key = self.get_signing_key_from_keyjar(algorithm, keyjar)
         except (MissingKey,) as err:
             LOGGER.error("%s", sanitize(err))
             raise
@@ -466,37 +464,36 @@
                 _pi = context.provider_info
                 try:
                     algs = _pi["token_endpoint_auth_signing_alg_values_supported"]
                 except KeyError:
                     algorithm = "RS256"  # default
                 else:
                     for alg in algs:  # pick the first one I support and have keys for
-                        if alg in SIGNER_ALGS and self.get_signing_key_from_keyjar(
-                                alg, keyjar
-                        ):
+                        if alg in SIGNER_ALGS and self.get_signing_key_from_keyjar(alg, keyjar):
                             algorithm = alg
                             break
 
             audience = context.provider_info.get("token_endpoint")
         else:
             audience = context.provider_info["issuer"]
 
         if not algorithm:
             algorithm = self.choose_algorithm(**kwargs)
         return audience, algorithm
 
     def _construct_client_assertion(self, service, **kwargs):
         _context = service.upstream_get("context")
         _entity = service.upstream_get("entity")
-        _keyjar = service.upstream_get('attribute', 'keyjar')
+        _keyjar = service.upstream_get("attribute", "keyjar")
         audience, algorithm = self._get_audience_and_algorithm(_context, _keyjar, **kwargs)
 
         if "kid" in kwargs:
-            signing_key = self._get_signing_key(algorithm, _keyjar, _context.kid["sig"],
-                                                kid=kwargs["kid"])
+            signing_key = self._get_signing_key(
+                algorithm, _keyjar, _context.kid["sig"], kid=kwargs["kid"]
+            )
         else:
             signing_key = self._get_signing_key(algorithm, _keyjar, _context.kid["sig"])
 
         if not signing_key:
             raise UnsupportedAlgorithm(algorithm)
 
         try:
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/configure.py` & `idpyoidc-2.1.0/src/idpyoidc/client/configure.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,24 +21,23 @@
     "backchannel_logout_uri",
     "issuer",
     "base_url",
 ]
 
 
 class RPHConfiguration(Base):
-
     def __init__(
-            self,
-            conf: Dict,
-            base_path: Optional[str] = "",
-            entity_conf: Optional[List[dict]] = None,
-            domain: Optional[str] = "127.0.0.1",
-            port: Optional[int] = 80,
-            file_attributes: Optional[List[str]] = None,
-            dir_attributes: Optional[List[str]] = None,
+        self,
+        conf: Dict,
+        base_path: Optional[str] = "",
+        entity_conf: Optional[List[dict]] = None,
+        domain: Optional[str] = "127.0.0.1",
+        port: Optional[int] = 80,
+        file_attributes: Optional[List[str]] = None,
+        dir_attributes: Optional[List[str]] = None,
     ):
 
         Base.__init__(
             self,
             conf,
             base_path=base_path,
             domain=domain,
@@ -67,15 +66,15 @@
             _val = lower_or_upper(conf, param, {})
             if _val and param not in self.default:
                 self.default[param] = _val
 
         self.clients = lower_or_upper(conf, "clients")
         if self.clients:
             for id, client in self.clients.items():
-                for param in ["services", "usage", "add_ons", 'claims']:
+                for param in ["services", "usage", "add_ons", "claims"]:
                     if param not in client:
                         if param in self.default:
                             client[param] = self.default[param]
 
         if entity_conf:
             self.extend(
                 entity_conf=entity_conf,
@@ -84,25 +83,25 @@
                 file_attributes=file_attributes,
                 domain=domain,
                 port=port,
             )
 
 
 class Configuration(Base):
-    """ Configuration for a single RP """
+    """Configuration for a single RP"""
 
     def __init__(
-            self,
-            conf: Dict,
-            base_path: str = "",
-            entity_conf: Optional[List[dict]] = None,
-            file_attributes: Optional[List[str]] = None,
-            domain: Optional[str] = "",
-            port: Optional[int] = 0,
-            dir_attributes: Optional[List[str]] = None,
+        self,
+        conf: Dict,
+        base_path: str = "",
+        entity_conf: Optional[List[dict]] = None,
+        file_attributes: Optional[List[str]] = None,
+        domain: Optional[str] = "",
+        port: Optional[int] = 0,
+        dir_attributes: Optional[List[str]] = None,
     ):
         Base.__init__(
             self,
             conf,
             base_path=base_path,
             file_attributes=file_attributes,
             dir_attributes=dir_attributes,
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/cookie.py` & `idpyoidc-2.1.0/src/idpyoidc/client/cookie.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/current.py` & `idpyoidc-2.1.0/src/idpyoidc/client/current.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,30 +47,27 @@
             self._db[key] = info.to_dict()
         else:
             self._db[key] = info
 
     def get_claim(self, key: str, claim: str) -> Union[str, None]:
         return self.get(key).get(claim)
 
-    def get_set(self,
-                key: str,
-                message: Optional[type(Message)] = None,
-                claim: Optional[list] = None) -> dict:
+    def get_set(
+        self, key: str, message: Optional[type(Message)] = None, claim: Optional[list] = None
+    ) -> dict:
         """
 
-        @param key: The key to a seet of current claims
+        @param key: The key to a set of current claims
         @param message: A message class
         @param claim: A list of claims
         @return: Dictionary
+        @raise KeyError if no such key
         """
 
-        try:
-            _current = self.get(key)
-        except KeyError:
-            return {}
+        _current = self.get(key)
 
         if message:
             _res = {k: _current[k] for k in message.c_param.keys() if k in _current}
         else:
             _res = {}
 
         if claim:
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/defaults.py` & `idpyoidc-2.1.0/src/idpyoidc/client/defaults.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,31 +27,29 @@
 }
 
 DEFAULT_CLIENT_PREFERENCES = {
     "application_type": "web",
     "response_types": [
         "code",
         "id_token",
-        "id_token token",
         "code id_token",
-        "code id_token token",
-        "code token",
     ],
     "token_endpoint_auth_method": "client_secret_basic",
     "scopes_supported": ["openid"],
 }
 
 DEFAULT_USAGE = {
     "jwks_uri": True,
     "scope": ["openid"],
 }
 
 # Using PKCE is default
 DEFAULT_CLIENT_CONFIGS = {
     "": {
+        "client_type": "oidc",
         "preference": DEFAULT_CLIENT_PREFERENCES,
         "add_ons": {
             "pkce": {
                 "function": "idpyoidc.client.oauth2.add_on.pkce.add_support",
                 "kwargs": {"code_challenge_length": 64, "code_challenge_method": "S256"},
             }
         },
@@ -67,14 +65,16 @@
     "private_path": "private/jwks.json",
     "key_defs": DEFAULT_KEY_DEFS,
     "public_path": "static/jwks.json",
     "read_only": False,
 }
 
 OIDCONF_PATTERN = "{}/.well-known/openid-configuration"
+OAUTH2_SERVER_METADATA_URL = "{}/.well-known/oauth-authorization-server"
+
 CC_METHOD = {
     "S256": hashlib.sha256,
     "S384": hashlib.sha384,
     "S512": hashlib.sha512,
 }
 
 # Map the signing context to a signing algorithm
@@ -88,7 +88,17 @@
 
 HTTP_ARGS = ["headers", "redirections", "connection_type"]
 
 JWT_BEARER = "urn:ietf:params:oauth:client-assertion-type:jwt-bearer"
 SAML2_BEARER_GRANT_TYPE = "urn:ietf:params:oauth:grant-type:saml2-bearer"
 
 BASECHR = string.ascii_letters + string.digits
+
+DEFAULT_RESPONSE_MODE = {
+    "code": "query",
+    "id_token": "fragment",
+    "token": "fragment",
+    "code token": "fragment",
+    "code id_token": "fragment",
+    "id_token token": "fragment",
+    "code id_token token": "fragment",
+}
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/entity.py` & `idpyoidc-2.1.0/src/idpyoidc/client/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 from idpyoidc.node import Unit
 
 logger = logging.getLogger(__name__)
 
 RESPONSE_TYPES2GRANT_TYPES = {
     "code": ["authorization_code"],
     "id_token": ["implicit"],
-    "id_token token": ["implicit"],
+    # "id_token token": ["implicit"],
     "code id_token": ["authorization_code", "implicit"],
-    "code token": ["authorization_code", "implicit"],
-    "code id_token token": ["authorization_code", "implicit"],
+    # "code token": ["authorization_code", "implicit"],
+    # "code id_token token": ["authorization_code", "implicit"],
 }
 
 
 def response_types_to_grant_types(response_types):
     _res = set()
 
     for response_type in response_types:
@@ -44,15 +44,15 @@
         else:
             _res.update(set(_gt))
 
     return list(_res)
 
 
 def _set_jwks(service_context, config: Configuration, keyjar: Optional[KeyJar]):
-    _key_conf = config.get("key_conf") or config.conf.get('key_conf')
+    _key_conf = config.get("key_conf") or config.conf.get("key_conf")
 
     if _key_conf:
         keys_args = {k: v for k, v in _key_conf.items() if k != "uri_path"}
         _keyjar = init_key_jar(**keys_args)
         service_context.set_preference("jwks", _keyjar.export_jwks())
     elif keyjar:
         service_context.set_preference("jwks", keyjar.export_jwks())
@@ -67,73 +67,85 @@
             service_context.set_preference("jwks_uri", jwks_uri)
         else:
             _set_jwks(service_context, config, keyjar)
 
 
 def redirect_uris_from_callback_uris(callback_uris):
     res = []
-    for k, v in callback_uris['redirect_uris'].items():
+    for k, v in callback_uris["redirect_uris"].items():
         res.extend(v)
     return res
 
 
 class Entity(Unit):  # This is a Client. What type is undefined here.
     parameter = {
-        'entity_id': None,
-        'jwks_uri': None,
-        'httpc_params': None,
-        'key_conf': None,
-        'keyjar': KeyJar,
-        'context': None
+        "entity_id": None,
+        "jwks_uri": None,
+        "httpc_params": None,
+        "key_conf": None,
+        "keyjar": KeyJar,
+        "context": None,
     }
 
     def __init__(
-            self,
-            keyjar: Optional[KeyJar] = None,
-            config: Optional[Union[dict, Configuration]] = None,
-            services: Optional[dict] = None,
-            jwks_uri: Optional[str] = "",
-            httpc: Optional[Callable] = None,
-            httpc_params: Optional[dict] = None,
-            client_type: Optional[str] = "oauth2",
-            context: Optional[OidcContext] = None,
-            upstream_get: Optional[Callable] = None,
-            key_conf: Optional[dict] = None,
-            entity_id: Optional[str] = ''
+        self,
+        keyjar: Optional[KeyJar] = None,
+        config: Optional[Union[dict, Configuration]] = None,
+        services: Optional[dict] = None,
+        jwks_uri: Optional[str] = "",
+        httpc: Optional[Callable] = None,
+        httpc_params: Optional[dict] = None,
+        client_type: Optional[str] = "oauth2",
+        context: Optional[OidcContext] = None,
+        upstream_get: Optional[Callable] = None,
+        key_conf: Optional[dict] = None,
+        entity_id: Optional[str] = "",
     ):
         if config is None:
             config = {}
 
-        _id = config.get('client_id')
-        self.client_id = self.entity_id = entity_id or config.get('entity_id', _id)
+        _id = config.get("client_id")
+        self.client_id = self.entity_id = entity_id or config.get("entity_id", _id)
 
-        Unit.__init__(self, upstream_get=upstream_get, keyjar=keyjar, httpc=httpc,
-                      httpc_params=httpc_params, config=config, key_conf=key_conf,
-                      client_id=self.client_id)
+        Unit.__init__(
+            self,
+            upstream_get=upstream_get,
+            keyjar=keyjar,
+            httpc=httpc,
+            httpc_params=httpc_params,
+            config=config,
+            key_conf=key_conf,
+            client_id=self.client_id,
+        )
 
         if services:
             _srvs = services
         elif config:
             _srvs = config.get("services")
         else:
             _srvs = None
 
         if not _srvs:
-            if client_type == 'oauth2':
+            if client_type == "oauth2":
                 _srvs = DEFAULT_OAUTH2_SERVICES
             else:
                 _srvs = DEFAULT_OIDC_SERVICES
 
         self._service = init_services(service_definitions=_srvs, upstream_get=self.unit_get)
 
         if context:
             self.context = context
         else:
-            self.context = ServiceContext(config=config, jwks_uri=jwks_uri, keyjar=self.keyjar,
-                                          upstream_get=self.unit_get, client_type=client_type)
+            self.context = ServiceContext(
+                config=config,
+                jwks_uri=jwks_uri,
+                keyjar=self.keyjar,
+                upstream_get=self.unit_get,
+                client_type=client_type,
+            )
 
         self.setup_client_authn_methods(config)
 
         self.upstream_get = upstream_get
 
     def get_services(self, *arg):
         return self._service
@@ -157,19 +169,19 @@
 
         return None
 
     def get_entity(self):
         return self
 
     def get_client_id(self):
-        _val = self.context.claims.get_usage('client_id')
+        _val = self.context.claims.get_usage("client_id")
         if _val:
             return _val
         else:
-            return self.context.claims.get_preference('client_id')
+            return self.context.claims.get_preference("client_id")
 
     def setup_client_authn_methods(self, config):
         if config and "client_authn_methods" in config:
             _methods = config.get("client_authn_methods")
             self.context.client_authn_methods = client_auth_setup(method_to_item(_methods))
         else:
             self.context.client_authn_methods = {}
@@ -179,25 +191,24 @@
         The client needs its own set of keys. It can either dynamically
         create them or load them from local storage.
         This method can also fetch other entities keys provided the
         URL points to a JWKS.
 
         :param keyspec:
         """
-        _keyjar = self.get_attribute('keyjar')
+        _keyjar = self.get_attribute("keyjar")
         if _keyjar is None:
             _keyjar = KeyJar()
 
         for where, spec in keyspec.items():
             if where == "file":
                 for typ, files in spec.items():
                     if typ == "rsa":
                         for fil in files:
-                            _key = RSAKey(priv_key=import_private_rsa_key_from_file(fil),
-                                          use="sig")
+                            _key = RSAKey(priv_key=import_private_rsa_key_from_file(fil), use="sig")
                             _bundle = KeyBundle()
                             _bundle.append(_key)
                             _keyjar.add_kb("", _bundle)
             elif where == "url":
                 for iss, url in spec.items():
                     _bundle = KeyBundle(source=url)
                     _keyjar.add_kb(iss, _bundle)
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/exception.py` & `idpyoidc-2.1.0/src/idpyoidc/client/exception.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/http.py` & `idpyoidc-2.1.0/src/idpyoidc/client/http.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/oauth2/__init__.py` & `idpyoidc-2.1.0/src/idpyoidc/client/oauth2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,58 +1,57 @@
-from json import JSONDecodeError
 import logging
+from json import JSONDecodeError
 from typing import Callable
 from typing import Optional
 from typing import Union
 
 from cryptojwt.key_jar import KeyJar
 from requests import request
 
 from idpyoidc.client.entity import Entity
 from idpyoidc.client.exception import ConfigurationError
 from idpyoidc.client.exception import OidcServiceError
 from idpyoidc.client.exception import ParseError
 from idpyoidc.client.service import REQUEST_INFO
-from idpyoidc.client.service import SUCCESSFUL
 from idpyoidc.client.service import Service
+from idpyoidc.client.service import SUCCESSFUL
 from idpyoidc.client.util import do_add_ons
 from idpyoidc.client.util import get_deserialization_method
 from idpyoidc.configure import Configuration
 from idpyoidc.context import OidcContext
 from idpyoidc.exception import FormatError
 from idpyoidc.message import Message
 from idpyoidc.message.oauth2 import is_error_message
 
 __author__ = "Roland Hedberg"
 
 logger = logging.getLogger(__name__)
 
-Version = "2.0"
-
 
 class ExpiredToken(Exception):
     pass
 
 
 # =============================================================================
 
 
 class Client(Entity):
-    client_type = 'oauth2'
+    client_type = "oauth2"
+
     def __init__(
             self,
             keyjar: Optional[KeyJar] = None,
             config: Optional[Union[dict, Configuration]] = None,
             services: Optional[dict] = None,
             httpc: Optional[Callable] = None,
             httpc_params: Optional[dict] = None,
             context: Optional[OidcContext] = None,
             upstream_get: Optional[Callable] = None,
             key_conf: Optional[dict] = None,
-            entity_id: Optional[str] = '',
+            entity_id: Optional[str] = "",
             verify_ssl: Optional[bool] = True,
             jwks_uri: Optional[str] = "",
             client_type: Optional[str] = "",
             **kwargs
     ):
         """
 
@@ -65,37 +64,43 @@
         :param httpc: A HTTP client to use
         :param httpc_params: HTTP request arguments
         :param services: A list of service definitions
         :param jwks_uri: A jwks_uri
         :return: Client instance
         """
 
-        if not client_type:
+        if client_type:
+            self.client_type = client_type
+        elif config and 'client_type' in config:
+            client_type = self.client_type = config["client_type"]
+        else:
             client_type = self.client_type
 
         if verify_ssl is False:
             # just ignore verify_ssl until it goes away
             if httpc_params:
-                httpc_params['verify'] = False
+                httpc_params["verify"] = False
             else:
-                httpc_params = {'verify': False}
+                httpc_params = {"verify": False}
+
+        jwks_uri = jwks_uri or config.get('jwks_uri', '')
 
         Entity.__init__(
             self,
             keyjar=keyjar,
             config=config,
             services=services,
             jwks_uri=jwks_uri,
             httpc=httpc,
             httpc_params=httpc_params,
             client_type=client_type,
             context=context,
             upstream_get=upstream_get,
             key_conf=key_conf,
-            entity_id=entity_id
+            entity_id=entity_id,
         )
 
         self.httpc = httpc or request
 
         if isinstance(config, Configuration):
             _add_ons = config.conf.get("add_ons")
         else:
@@ -159,15 +164,15 @@
             raise
 
         if 300 <= resp.status_code < 400:
             return {"http_response": resp}
 
         if resp.status_code < 300:
             if "keyjar" not in kwargs:
-                kwargs["keyjar"] = self.get_attribute('keyjar')
+                kwargs["keyjar"] = self.get_attribute("keyjar")
             if not response_body_type:
                 response_body_type = service.response_body_type
 
             if response_body_type == "html":
                 return resp.text
 
             if body:
@@ -213,15 +218,15 @@
             response = self.get_response(
                 service, url, method, body, response_body_type, headers, **kwargs
             )
 
         if "error" in response:
             pass
         else:
-            service.update_service_context(response, key=kwargs.get('state'), **kwargs)
+            service.update_service_context(response, key=kwargs.get("state"), **kwargs)
         return response
 
     def parse_request_response(self, service, reqresp, response_body_type="", state="", **kwargs):
         """
         Deal with a self.httpc response. The response are expected to
         follow a special pattern, having the attributes:
 
@@ -307,21 +312,24 @@
 def dynamic_provider_info_discovery(client: Client, behaviour_args: Optional[dict] = None):
     """
     This is about performing dynamic Provider Info discovery
 
     :param behaviour_args:
     :param client: A :py:class:`idpyoidc.client.oidc.Client` instance
     """
+
+    if client.client_type == 'oidc' and client.get_service("provider_info"):
+        service = 'provider_info'
+    elif client.client_type == 'oauth2' and client.get_service('server_metadata'):
+        service = 'server_metadata'
+    else:
+        raise ConfigurationError("Can not do dynamic provider info discovery")
+
+    _context = client.get_context()
     try:
-        client.get_service("provider_info")
+        _context.set("issuer", _context.config["srv_discovery_url"])
     except KeyError:
-        raise ConfigurationError("Can not do dynamic provider info discovery")
-    else:
-        _context = client.get_context()
-        try:
-            _context.set("issuer", _context.config["srv_discovery_url"])
-        except KeyError:
-            pass
+        pass
 
-        response = client.do_request("provider_info", behaviour_args=behaviour_args)
-        if is_error_message(response):
-            raise OidcServiceError(response["error"])
+    response = client.do_request(service, behaviour_args=behaviour_args)
+    if is_error_message(response):
+        raise OidcServiceError(response["error"])
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/oauth2/access_token.py` & `idpyoidc-2.1.0/src/idpyoidc/client/oauth2/access_token.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,26 +23,26 @@
     synchronous = True
     service_name = "accesstoken"
     default_authn_method = "client_secret_basic"
     http_method = "POST"
     request_body_type = "urlencoded"
     response_body_type = "json"
 
-    _include = {"grant_types_supported": ['authorization_code']}
+    _include = {"grant_types_supported": ["authorization_code"]}
 
     _supports = {
         "token_endpoint_auth_methods_supported": get_client_authn_methods,
         "token_endpoint_auth_signing_alg": get_signing_algs,
     }
 
     def __init__(self, upstream_get, conf=None):
         Service.__init__(self, upstream_get, conf=conf)
         self.pre_construct.append(self.oauth_pre_construct)
 
-    def update_service_context(self, resp, key: Optional[str] = '', **kwargs):
+    def update_service_context(self, resp, key: Optional[str] = "", **kwargs):
         if "expires_in" in resp:
             resp["__expires_at"] = time_sans_frac() + int(resp["expires_in"])
         if key:
             self.upstream_get("context").cstate.update(key, resp)
 
     def oauth_pre_construct(self, request_args=None, post_args=None, **kwargs):
         """
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/oauth2/add_on/dpop.py` & `idpyoidc-2.1.0/src/idpyoidc/client/oauth2/add_on/dpop.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,46 @@
+import logging
 import uuid
+from hashlib import sha256
 from typing import Optional
 
+from cryptography.hazmat.primitives import hashes
 from cryptojwt.jwk.jwk import key_from_jwk_dict
 from cryptojwt.jws.jws import JWS
 from cryptojwt.jws.jws import factory
+from cryptojwt.jws.jws import SIGNER_ALGS
 from cryptojwt.key_bundle import key_by_alg
 
+from idpyoidc.claims import get_signing_algs
 from idpyoidc.client.service_context import ServiceContext
+from idpyoidc.message import SINGLE_OPTIONAL_STRING
 from idpyoidc.message import SINGLE_REQUIRED_INT
 from idpyoidc.message import SINGLE_REQUIRED_JSON
 from idpyoidc.message import SINGLE_REQUIRED_STRING
 from idpyoidc.message import Message
 from idpyoidc.time_util import utc_time_sans_frac
 
+logger = logging.getLogger(__name__)
+
 
 class DPoPProof(Message):
     c_param = {
         # header
         "typ": SINGLE_REQUIRED_STRING,
         "alg": SINGLE_REQUIRED_STRING,
         "jwk": SINGLE_REQUIRED_JSON,
         # body
         "jti": SINGLE_REQUIRED_STRING,
         "htm": SINGLE_REQUIRED_STRING,
         "htu": SINGLE_REQUIRED_STRING,
         "iat": SINGLE_REQUIRED_INT,
+        "ath": SINGLE_OPTIONAL_STRING,
     }
     header_params = {"typ", "alg", "jwk"}
-    body_params = {"jti", "htm", "htu", "iat"}
+    body_params = {"jti", "htm", "htu", "iat", "ath"}
 
     def __init__(self, set_defaults=True, **kwargs):
         self.key = None
         Message.__init__(self, set_defaults=set_defaults, **kwargs)
 
         if self.key:
             pass
@@ -52,15 +61,15 @@
         Message.verify(self, **kwargs)
         if self["typ"] != "dpop+jwt":
             raise ValueError("Wrong type")
         if self["alg"] == "none":
             raise ValueError("'none' is not allowed as signing algorithm")
 
     def create_header(self) -> str:
-        payload = {k: self[k] for k in self.body_params}
+        payload = {k: self[k] for k in self.body_params if k in self}
         _jws = JWS(payload, alg=self["alg"])
         _jws_headers = {k: self[k] for k in self.header_params}
         _signed_jwt = _jws.sign_compact(keys=[self.key], **_jws_headers)
         return _signed_jwt
 
     def verify_header(self, dpop_header) -> Optional["DPoPProof"]:
         _jws = factory(dpop_header)
@@ -84,58 +93,66 @@
 
 
 def dpop_header(
     service_context: ServiceContext,
     service_endpoint: str,
     http_method: str,
     headers: Optional[dict] = None,
+    token: Optional[str] = "",
+    nonce: Optional[str] = "",
     **kwargs
 ) -> dict:
     """
 
     :param service_context:
     :param service_endpoint:
     :param http_method:
-    :param headers:
+    :param headers: The HTTP headers to which the DPoP header should be added.
+    :param token: If the DPoP Proof is sent together with an access token this should lead to
+        the addition of the ath claim (hash of the token as value)
+    :param nonce: AS or RS provided nonce.
     :param kwargs:
     :return:
     """
 
     provider_info = service_context.provider_info
-    dpop_key = service_context.add_on["dpop"].get("key")
+    _dpop_conf = service_context.add_on.get("dpop")
+    if not _dpop_conf:
+        logger.warning("Asked to do dpop when I do not support it")
+        return headers
 
-    if not dpop_key:
-        algs_supported = provider_info["dpop_signing_alg_values_supported"]
-        if not algs_supported:  # does not support DPoP
-            return headers
+    dpop_key = _dpop_conf.get("key")
 
-        chosen_alg = ""
-        for alg in service_context.add_on["dpop"]["sign_algs"]:
-            if alg in algs_supported:
-                chosen_alg = alg
-                break
+    if not dpop_key:
+        chosen_alg = _dpop_conf.get("algs_supported", [])[0]
 
         if not chosen_alg:
             return headers
 
         # Mint a new key
         dpop_key = key_by_alg(chosen_alg)
-        service_context.add_on["dpop"]["key"] = dpop_key
-        service_context.add_on["dpop"]["alg"] = chosen_alg
+        _dpop_conf["key"] = dpop_key
+        _dpop_conf["alg"] = chosen_alg
 
     header_dict = {
         "typ": "dpop+jwt",
-        "alg": service_context.add_on["dpop"]["alg"],
+        "alg": _dpop_conf["alg"],
         "jwk": dpop_key.serialize(),
         "jti": uuid.uuid4().hex,
         "htm": http_method,
         "htu": provider_info[service_endpoint],
         "iat": utc_time_sans_frac(),
     }
 
+    if token:
+        header_dict["ath"] = sha256(token.encode("utf8")).hexdigest()
+
+    if nonce:
+        header_dict["nonce"] = nonce
+
     _dpop = DPoPProof(**header_dict)
     _dpop.key = dpop_key
     jws = _dpop.create_header()
 
     if headers is None:
         headers = {"dpop": jws}
     else:
@@ -151,17 +168,22 @@
     :param services: A dictionary with all the services the client has access to.
     :param signing_algorithms: Allowed signing algorithms, there is no default algorithms
     """
 
     # Access token request should use DPoP header
     _service = services["accesstoken"]
     _context = _service.upstream_get("context")
+    _algs_supported = [
+        alg for alg in dpop_signing_alg_values_supported if alg in get_signing_algs()
+    ]
     _context.add_on["dpop"] = {
         # "key": key_by_alg(signing_algorithm),
-        "sign_algs": dpop_signing_alg_values_supported
+        "algs_supported": _algs_supported
     }
+    _context.set_preference("dpop_signing_alg_values_supported", _algs_supported)
+
     _service.construct_extra_headers.append(dpop_header)
 
     # The same for userinfo requests
     _userinfo_service = services.get("userinfo")
     if _userinfo_service:
         _userinfo_service.construct_extra_headers.append(dpop_header)
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/oauth2/add_on/identity_assurance.py` & `idpyoidc-2.1.0/src/idpyoidc/client/oauth2/add_on/identity_assurance.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,15 @@
             else:
                 _resp[json.dumps(vr["verification"])] = vr["claims"]
 
     return _resp
 
 
 def identity_assurance_process(response, service_context, state):
-    auth_request = service_context.cstate.get_set(state,
-                                                  message=AuthorizationRequest)
+    auth_request = service_context.cstate.get_set(state, message=AuthorizationRequest)
     claims_request = auth_request.get("claims")
     if claims_request and "userinfo" in claims_request:
         vc = VerifiedClaims(**response["verified_claims"])
 
         # find the claims request in the authorization request
         verified_response = match_verified_claims(vc, claims_request["userinfo"]["verified_claims"])
         _response_format = service_context.add_on["identity_assurance"]["response_format"]
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/oauth2/add_on/pkce.py` & `idpyoidc-2.1.0/src/idpyoidc/client/oauth2/add_on/pkce.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     :param service: The service that uses this function
     :param request_args: Set of request arguments
     :return: updated set of request arguments
     """
     _state = request_args.get("state")
     if _state is None:
         _state = kwargs.get("state")
-    _item = service.upstream_get("context").cstate.get_set(_state, claim=['code_verifier'])
+    _item = service.upstream_get("context").cstate.get_set(_state, claim=["code_verifier"])
     request_args.update(_item)
     return request_args
 
 
 def put_state_in_post_args(request_args, **kwargs):
     state = get_state_parameter(request_args, kwargs)
     return request_args, {"state": state}
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/oauth2/add_on/status_check.py` & `idpyoidc-2.1.0/src/idpyoidc/client/oauth2/add_on/status_check.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/oauth2/authorization.py` & `idpyoidc-2.1.0/src/idpyoidc/client/oauth2/authorization.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """The service that talks to the OAuth2 Authorization endpoint."""
 import logging
 from typing import List
 from typing import Optional
 
-from idpyoidc import claims
 from idpyoidc.client.oauth2.utils import get_state_parameter
 from idpyoidc.client.oauth2.utils import pre_construct_pick_redirect_uri
 from idpyoidc.client.oauth2.utils import set_state_parameter
 from idpyoidc.client.service import Service
 from idpyoidc.client.service_context import ServiceContext
+from idpyoidc.client.util import IMPLICIT_RESPONSE_TYPES
 from idpyoidc.client.util import implicit_response_types
 from idpyoidc.exception import MissingParameter
 from idpyoidc.message import oauth2
 from idpyoidc.message.oauth2 import ResponseMessage
 from idpyoidc.time_util import time_sans_frac
 
 LOGGER = logging.getLogger(__name__)
@@ -26,27 +26,27 @@
     error_msg = ResponseMessage
     endpoint_name = "authorization_endpoint"
     synchronous = False
     service_name = "authorization"
     response_body_type = "urlencoded"
 
     _supports = {
-        "response_types_supported": ["code", 'token'],
-        "response_modes_supported": ['query', 'fragment'],
+        "response_types_supported": ["code"],
+        "response_modes_supported": ["query", "fragment"],
         # Below not OAuth2 functionality
         # "request_object_signing_alg_values_supported": claims.get_signing_algs,
         # "request_object_encryption_alg_values_supported": claims.get_encryption_algs,
         # "request_object_encryption_enc_values_supported": claims.get_encryption_encs,
         # "encrypt_request_object_supported": False,
     }
 
     _callback_path = {
-        "redirect_uris": {  # based on response_types
-            "code": "authz_cb",
-            "implicit": "authz_im_cb",
+        "redirect_uris": {  # based on response_mode
+            "query": "authz_cb",
+            "fragment": "authz_im_cb",
             # "form_post": "form"
         }
     }
 
     def __init__(self, upstream_get, conf=None):
         Service.__init__(self, upstream_get, conf=conf)
         self.pre_construct.extend([pre_construct_pick_redirect_uri, set_state_parameter])
@@ -64,16 +64,15 @@
         return request_args
 
     def gather_request_args(self, **kwargs):
         ar_args = Service.gather_request_args(self, **kwargs)
 
         if "redirect_uri" not in ar_args:
             try:
-                ar_args["redirect_uri"] = self.upstream_get("context").get_usage(
-                    "redirect_uris")[0]
+                ar_args["redirect_uri"] = self.upstream_get("context").get_usage("redirect_uris")[0]
             except (KeyError, AttributeError):
                 raise MissingParameter("redirect_uri")
 
         return ar_args
 
     def post_parse_response(self, response, **kwargs):
         """
@@ -89,68 +88,86 @@
             try:
                 _key = kwargs["state"]
             except KeyError:
                 pass
             else:
                 if _key:
                     item = self.upstream_get("context").cstate.get_set(
-                        _key, message=oauth2.AuthorizationRequest)
+                        _key, message=oauth2.AuthorizationRequest
+                    )
                     try:
                         response["scope"] = item["scope"]
                     except KeyError:
                         pass
         return response
 
-    def _do_flow(self, flow_type, response_types):
-        if flow_type == 'code' and 'code' in response_types:
-            return True
-        elif flow_type == 'implicit':
+    def _do_flow(self, flow_type, response_types, context) -> str:
+        if flow_type == "query":
+            if "code" in response_types:
+                return "query"
+        elif flow_type == "fragment":
             if implicit_response_types(response_types):
-                return True
-        return False
+                return "fragment"
+        elif flow_type == 'form_post':
+            rm = context.get_preference('response_modes_supported')
+            if rm and 'form_post' in rm:
+                if context.config.conf.get("separate_form_post_cb", True):
+                    return "form_post"
+                else:
+                    return "query"
+        return ''
 
     def _do_redirect_uris(self, base_url, hex, context, callback_uris, response_types):
-        _redirect_uris = context.get_preference('redirect_uris', [])
+        _redirect_uris = context.get_preference("redirect_uris", [])
         if _redirect_uris:
-            if not callback_uris or 'redirect_uris' not in callback_uris:
+            if not callback_uris or "redirect_uris" not in callback_uris:
                 # the same redirect_uris for all flow types
-                callback_uris['redirect_uris'] = {}
-                for flow_type in self._callback_path['redirect_uris'].keys():
-                    if self._do_flow(flow_type, response_types):
-                        callback_uris['redirect_uris'][flow_type] = _redirect_uris
+                callback_uris["redirect_uris"] = {}
+                for flow_type in self._callback_path["redirect_uris"].keys():
+                    if self._do_flow(flow_type, response_types, context):
+                        callback_uris["redirect_uris"][flow_type] = _redirect_uris
         elif callback_uris:
-            if 'redirect_uris' in callback_uris:
+            if "redirect_uris" in callback_uris:
                 pass
             else:
-                callback_uris['redirect_uris'] = {}
-                for flow_type, path in self._callback_path['redirect_uris'].items():
-                    if self._do_flow(flow_type, response_types):
-                        callback_uris['redirect_uris'][flow_type] = [
-                            self.get_uri(base_url, path, hex)]
+                callback_uris["redirect_uris"] = {}
+                for flow_type in self._callback_path["redirect_uris"].keys():
+                    _var = self._do_flow(flow_type, response_types, context)
+                    if _var:
+                        _path = self._callback_path["redirect_uris"][_var]
+                        callback_uris["redirect_uris"][flow_type] = [
+                            self.get_uri(base_url, _path, hex)
+                        ]
         else:
-            callback_uris['redirect_uris'] = {}
-            for flow_type, path in self._callback_path['redirect_uris'].items():
-                if self._do_flow(flow_type, response_types):
-                    callback_uris['redirect_uris'][flow_type] = [self.get_uri(base_url, path, hex)]
+            callback_uris["redirect_uris"] = {}
+            for flow_type in self._callback_path["redirect_uris"].keys():
+                _var = self._do_flow(flow_type, response_types, context)
+                if _var:
+                    _path = self._callback_path["redirect_uris"][_var]
+                    callback_uris["redirect_uris"][flow_type] = [self.get_uri(base_url, _path, hex)]
         return callback_uris
 
-    def construct_uris(self,
-                       base_url: str,
-                       hex: bytes,
-                       context: ServiceContext,
-                       targets: Optional[List[str]] = None,
-                       response_types: Optional[List[str]] = None):
-        _callback_uris = context.get_preference('callback_uris', {})
+    def construct_uris(
+        self,
+        base_url: str,
+        hex: bytes,
+        context: ServiceContext,
+        targets: Optional[List[str]] = None,
+        response_types: Optional[List[str]] = None,
+    ):
+        _callback_uris = context.get_preference("callback_uris", {})
 
         for uri_name in self._callback_path.keys():
-            if uri_name == 'redirect_uris':
-                _callback_uris = self._do_redirect_uris(base_url, hex, context, _callback_uris,
-                                                        response_types)
+            if uri_name == "redirect_uris":
+                _callback_uris = self._do_redirect_uris(
+                    base_url, hex, context, _callback_uris, response_types
+                )
                 _redirect_uris = set()
-                for flow, _uris in _callback_uris['redirect_uris'].items():
+                for flow, _uris in _callback_uris["redirect_uris"].items():
                     _redirect_uris.update(set(_uris))
-                context.set_preference('redirect_uris', list(_redirect_uris))
+                context.set_preference("redirect_uris", list(_redirect_uris))
             else:
-                _callback_uris[uri_name] = self.get_uri(base_url, self._callback_path[uri_name],
-                                                        hex)
+                _callback_uris[uri_name] = self.get_uri(
+                    base_url, self._callback_path[uri_name], hex
+                )
 
         return _callback_uris
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/oauth2/client_credentials.py` & `idpyoidc-2.1.0/src/idpyoidc/client/oauth2/client_credentials.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,24 +20,22 @@
     default_authn_method = ""
     http_method = "POST"
 
     def __init__(self, upstream_get, conf=None):
         Service.__init__(self, upstream_get, conf=conf)
         self.pre_construct.append(self.cc_pre_construct)
 
-    def cc_pre_construct(self,
-                         request: Union[Message, dict],
-                         service: Service,
-                         post_args: Optional[dict],
-                         **_args):
-        _grant_type = request.get('grant_type')
+    def cc_pre_construct(
+        self, request: Union[Message, dict], service: Service, post_args: Optional[dict], **_args
+    ):
+        _grant_type = request.get("grant_type")
         if not _grant_type:
-            request['grant_type'] = 'client_credentials'
-        elif _grant_type != 'client_credentials':
-            logging.error('Wrong grant_type')
+            request["grant_type"] = "client_credentials"
+        elif _grant_type != "client_credentials":
+            logging.error("Wrong grant_type")
 
         return request, post_args
 
     def update_service_context(self, resp, key: Optional[str] = "", **kwargs):
         if "expires_in" in resp:
             resp["__expires_at"] = time_sans_frac() + int(resp["expires_in"])
         self.upstream_get("context").cstate.update(key, resp)
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/oauth2/refresh_access_token.py` & `idpyoidc-2.1.0/src/idpyoidc/client/oauth2/refresh_access_token.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 
     msg_type = oauth2.RefreshAccessTokenRequest
     response_cls = oauth2.AccessTokenResponse
     error_msg = ResponseMessage
     endpoint_name = "token_endpoint"
     synchronous = True
     service_name = "refresh_token"
-    default_authn_method = "bearer_header"
+    default_authn_method = "client_secret_post"
     http_method = "POST"
 
-    _include = {"grant_types_supported": ['refresh_token']}
+    _include = {"grant_types_supported": ["refresh_token"]}
 
     def __init__(self, upstream_get, conf=None):
         Service.__init__(self, upstream_get, conf=conf)
         self.pre_construct.append(self.oauth_pre_construct)
 
     def update_service_context(self, resp, key: Optional[str] = "", **kwargs):
         if "expires_in" in resp:
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/oauth2/resource_owner_password_credentials.py` & `idpyoidc-2.1.0/src/idpyoidc/client/oauth2/resource_owner_password_credentials.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,24 +20,22 @@
     default_authn_method = ""
     http_method = "POST"
 
     def __init__(self, upstream_get, conf=None):
         Service.__init__(self, upstream_get, conf=conf)
         self.pre_construct.append(self.ropc_pre_construct)
 
-    def ropc_pre_construct(self,
-                           request: Union[Message, dict],
-                           service: Service,
-                           post_args: Optional[dict],
-                           **_args):
-        _grant_type = request.get('grant_type')
+    def ropc_pre_construct(
+        self, request: Union[Message, dict], service: Service, post_args: Optional[dict], **_args
+    ):
+        _grant_type = request.get("grant_type")
         if not _grant_type:
-            request['grant_type'] = 'password'
-        elif _grant_type != 'password':
-            logging.error('Wrong grant_type')
+            request["grant_type"] = "password"
+        elif _grant_type != "password":
+            logging.error("Wrong grant_type")
 
         return request, post_args
 
     def update_service_context(self, resp, key: Optional[str] = "", **kwargs):
         if "expires_in" in resp:
             resp["__expires_at"] = time_sans_frac() + int(resp["expires_in"])
         self.upstream_get("context").cstate.update(key, resp)
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/oauth2/server_metadata.py` & `idpyoidc-2.1.0/src/idpyoidc/client/oauth2/server_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """The service that talks to the OAuth2 provider info discovery endpoint."""
 import logging
 from typing import Optional
 
 from cryptojwt.key_jar import KeyJar
 
+from idpyoidc.client.defaults import OAUTH2_SERVER_METADATA_URL
 from idpyoidc.client.defaults import OIDCONF_PATTERN
 from idpyoidc.client.exception import OidcServiceError
 from idpyoidc.client.service import Service
 from idpyoidc.message import Message
 from idpyoidc.message import oauth2
 from idpyoidc.message.oauth2 import ResponseMessage
 
@@ -19,14 +20,15 @@
 
     msg_type = oauth2.Message
     response_cls = oauth2.ASConfigurationResponse
     error_msg = ResponseMessage
     synchronous = True
     service_name = "server_metadata"
     http_method = "GET"
+    url_pattern = OAUTH2_SERVER_METADATA_URL
 
     _supports = {}
 
     def __init__(self, upstream_get, conf=None):
         Service.__init__(self, upstream_get, conf=conf)
 
     def get_endpoint(self):
@@ -37,17 +39,17 @@
         """
         try:
             _iss = self.upstream_get("context").issuer
         except AttributeError:
             _iss = self.endpoint
 
         if _iss.endswith("/"):
-            return OIDCONF_PATTERN.format(_iss[:-1])
+            return self.url_pattern.format(_iss[:-1])
 
-        return OIDCONF_PATTERN.format(_iss)
+        return self.url_pattern.format(_iss)
 
     def get_request_parameters(self, method="GET", **kwargs):
         """
         The Provider info discovery version of get_request_parameters()
 
         :param method:
         :param kwargs:
@@ -113,15 +115,15 @@
         _context.provider_info = resp
 
         self._set_endpoints(resp)
 
         # If I already have a Key Jar then I'll add then provider keys to
         # that. Otherwise, a new Key Jar is minted
         try:
-            _keyjar = self.upstream_get('attribute', 'keyjar')
+            _keyjar = self.upstream_get("attribute", "keyjar")
             if _keyjar is None:
                 _keyjar = KeyJar()
         except KeyError:
             _keyjar = KeyJar()
 
         # Load the keys. Note that this only means that the key specification
         # is loaded not necessarily that any keys are fetched.
@@ -131,11 +133,11 @@
             _keyjar.load_keys(_pcr_issuer, jwks=resp["jwks"])
 
         # Combine what I prefer/supports with what the Provider supports
         if isinstance(resp, Message):
             _info = resp.to_dict()
         else:
             _info = resp
-        _context.map_supported_to_preferred(_info)
+        _context.map_service_against_endpoint(_info)
 
     def update_service_context(self, resp, key: Optional[str] = "", **kwargs):
         return self._update_service_context(resp)
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/oauth2/token_exchange.py` & `idpyoidc-2.1.0/src/idpyoidc/client/oauth2/token_exchange.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     synchronous = True
     service_name = "token_exchange"
     default_authn_method = "client_secret_basic"
     http_method = "POST"
     request_body_type = "urlencoded"
     response_body_type = "json"
 
-    _include = {'grant_types_supported': ['urn:ietf:params:oauth:grant-type:token-exchange']}
+    _include = {"grant_types_supported": ["urn:ietf:params:oauth:grant-type:token-exchange"]}
 
     def __init__(self, upstream_get, conf=None):
         Service.__init__(self, upstream_get, conf=conf)
         self.pre_construct.append(self.oauth_pre_construct)
 
     def update_service_context(self, resp, key: Optional[str] = "", **kwargs):
         if "expires_in" in resp:
@@ -44,25 +44,25 @@
         :param request_args: Initial set of request arguments
         :param kwargs: Extra keyword arguments
         :return: Request arguments
         """
         if request_args is None:
             request_args = {}
 
-        if 'subject_token' not in request_args:
+        if "subject_token" not in request_args:
             try:
                 _key = get_state_parameter(request_args, kwargs)
             except MissingParameter:
                 raise MissingRequiredAttribute("subject_token")
 
-            parameters = {'access_token', 'scope'}
+            parameters = {"access_token", "scope"}
 
             _current = self.upstream_get("service_context").cstate
 
             _args = _current.get_set(_key, claim=parameters)
 
             request_args["subject_token"] = _args["access_token"]
-            request_args["subject_token_type"] = 'urn:ietf:params:oauth:token-type:access_token'
-            if 'scope' not in request_args and "scope" in _args:
+            request_args["subject_token_type"] = "urn:ietf:params:oauth:token-type:access_token"
+            if "scope" not in request_args and "scope" in _args:
                 request_args["scope"] = _args["scope"]
 
         return request_args, post_args
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/oauth2/utils.py` & `idpyoidc-2.1.0/src/idpyoidc/client/oauth2/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 from typing import Optional
 from typing import Union
 
+from idpyoidc.client.defaults import DEFAULT_RESPONSE_MODE
 from idpyoidc.client.service import Service
 from idpyoidc.exception import MissingParameter
 from idpyoidc.exception import MissingRequiredAttribute
 from idpyoidc.message import Message
 
 logger = logging.getLogger(__name__)
 
@@ -20,49 +21,55 @@
         except KeyError:
             raise MissingParameter("state")
 
     return _state
 
 
 def pick_redirect_uri(
-        context,
-        request_args: Optional[Union[Message, dict]] = None,
-        response_type: Optional[str] = "",
+    context,
+    request_args: Optional[Union[Message, dict]] = None,
+    response_type: Optional[str] = "",
+    response_mode: Optional[str] = ""
 ):
     if request_args is None:
         request_args = {}
 
     if "redirect_uri" in request_args:
         return request_args["redirect_uri"]
 
     _callback_uris = context.get_preference("callback_uris")
     if _callback_uris:
-        _callback_uris = _callback_uris.get("redirect_uris")
-
-    if _callback_uris:
-        if not response_type:
-            _conf_resp_types = context.get_usage("response_types", [])
-            response_type = request_args.get("response_type")
-            if not response_type and _conf_resp_types:
-                response_type = _conf_resp_types[0]
-
-        _response_mode = request_args.get("response_mode")
+        _redirect_uris = _callback_uris.get("redirect_uris")
+        _response_mode = request_args.get("response_mode") or response_mode
 
         if _response_mode:
             if _response_mode == "form_post":
-                redirect_uri = _callback_uris["form_post"][0]
-            elif response_type == "code" or response_type == ["code"]:
-                redirect_uri = _callback_uris["code"][0]
+                try:
+                    redirect_uri = _redirect_uris["form_post"][0]
+                except KeyError:
+                    redirect_uri = _redirect_uris["query"][0]
             else:
-                redirect_uri = _callback_uris["implicit"][0]
+                redirect_uri = _redirect_uris[_response_mode]
         else:
-            if 'code' == response_type:
-                redirect_uri = _callback_uris["code"][0]
-            else:
-                redirect_uri = _callback_uris["implicit"][0]
+            if not response_type:
+                _conf_resp_types = context.get_usage("response_types", [])
+                response_type = request_args.get("response_type")
+                if not response_type and _conf_resp_types:
+                    response_type = _conf_resp_types[0]
+
+            if isinstance(response_type, list):
+                response_type.sort()
+                response_type = " ".join(response_type)
+
+            try:
+                _response_mode = DEFAULT_RESPONSE_MODE[response_type]
+            except KeyError:
+                raise ValueError(f"Unknown response_type: {response_type}")
+
+            redirect_uri = _redirect_uris[_response_mode][0]
 
         logger.debug(
             f"pick_redirect_uris: response_type={response_type}, response_mode={_response_mode}, "
             f"redirect_uri={redirect_uri}"
         )
     else:
         redirect_uris = context.get_usage("redirect_uris", [])
@@ -72,19 +79,19 @@
             logger.error("No redirect_uri")
             raise MissingRequiredAttribute("redirect_uri")
 
     return redirect_uri
 
 
 def pre_construct_pick_redirect_uri(
-        request_args: Optional[Union[Message, dict]] = None, service: Optional[Service] = None,
-        **kwargs
+    request_args: Optional[Union[Message, dict]] = None, service: Optional[Service] = None, **kwargs
 ):
-    request_args["redirect_uri"] = pick_redirect_uri(service.upstream_get("context"),
-                                                     request_args=request_args)
+    request_args["redirect_uri"] = pick_redirect_uri(
+        service.upstream_get("context"), request_args=request_args
+    )
     return request_args, {}
 
 
 def set_state_parameter(request_args=None, **kwargs):
     """Assigned a state value."""
     request_args["state"] = get_state_parameter(request_args, kwargs)
     return request_args, {"state": request_args["state"]}
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/oidc/__init__.py` & `idpyoidc-2.1.0/src/idpyoidc/client/oidc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     "id_token_encrypted_response_alg": "id_token_encryption_alg_values_supported",
     "id_token_encrypted_response_enc": "id_token_encryption_enc_values_supported",
     "default_acr_values": "acr_values_supported",
     "subject_type": "subject_types_supported",
     "token_endpoint_auth_method": "token_endpoint_auth_methods_supported",
     "token_endpoint_auth_signing_alg": "token_endpoint_auth_signing_alg_values_supported",
     "response_types": "response_types_supported",
+    "response_modes": "response_modes_supported",
     "grant_types": "grant_types_supported",
 }
 
 PROVIDER2PREFERENCE = dict([(v, k) for k, v in PREFERENCE2PROVIDER.items()])
 
 PROVIDER_DEFAULT = {
     "token_endpoint_auth_method": "client_secret_basic",
@@ -73,29 +74,29 @@
 
 
 class FetchException(Exception):
     pass
 
 
 class RP(oauth2.Client):
-    client_type = 'oidc'
+    client_type = "oidc"
 
     def __init__(
-            self,
-            keyjar: Optional[KeyJar] = None,
-            config: Optional[Union[dict, Configuration]] = None,
-            services: Optional[dict] = None,
-            httpc: Optional[Callable] = None,
-            httpc_params: Optional[dict] = None,
-            upstream_get: Optional[Callable] = None,
-            key_conf: Optional[dict] = None,
-            entity_id: Optional[str] = '',
-            verify_ssl: Optional[bool] = True,
-            jwks_uri: Optional[str] = "",
-            **kwargs
+        self,
+        keyjar: Optional[KeyJar] = None,
+        config: Optional[Union[dict, Configuration]] = None,
+        services: Optional[dict] = None,
+        httpc: Optional[Callable] = None,
+        httpc_params: Optional[dict] = None,
+        upstream_get: Optional[Callable] = None,
+        key_conf: Optional[dict] = None,
+        entity_id: Optional[str] = "",
+        verify_ssl: Optional[bool] = True,
+        jwks_uri: Optional[str] = "",
+        **kwargs
     ):
         self.upstream_get = upstream_get
         if services:
             _srvs = services
         else:
             _srvs = config.get("services", DEFAULT_OIDC_SERVICES)
 
@@ -107,21 +108,21 @@
             httpc=httpc,
             httpc_params=httpc_params,
             upstream_get=upstream_get,
             key_conf=key_conf,
             entity_id=entity_id,
             verify_ssl=verify_ssl,
             jwks_uri=jwks_uri,
-            client_type='oidc',
+            client_type="oidc",
             **kwargs
         )
 
         _context = self.get_service_context()
-        if _context.get_preference('callback_uris') is None:
-            _context.set_preference('callback_uris', {})
+        if _context.get_preference("callback_uris") is None:
+            _context.set_preference("callback_uris", {})
 
     def fetch_distributed_claims(self, userinfo, callback=None):
         """
 
         :param userinfo: A :py:class:`idpyoidc.message.Message` sub class
             instance
         :param callback: A function that can be used to fetch things
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/oidc/access_token.py` & `idpyoidc-2.1.0/src/idpyoidc/client/oidc/access_token.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,40 +19,39 @@
 
 class AccessToken(access_token.AccessToken):
     msg_type = oidc.AccessTokenRequest
     response_cls = oidc.AccessTokenResponse
     error_msg = oidc.ResponseMessage
     default_authn_method = "client_secret_basic"
 
-    _include = {"grant_types_supported": ['authorization_code']}
+    _include = {"grant_types_supported": ["authorization_code"]}
 
     _supports = {
         "token_endpoint_auth_methods_supported": get_client_authn_methods,
-        "token_endpoint_auth_signing_alg_values_supported": get_signing_algs
+        "token_endpoint_auth_signing_alg_values_supported": get_signing_algs,
     }
 
     def __init__(self, upstream_get, conf: Optional[dict] = None):
         access_token.AccessToken.__init__(self, upstream_get, conf=conf)
 
     def gather_verify_arguments(
-            self, response: Optional[Union[dict, Message]] = None,
-            behaviour_args: Optional[dict] = None
+        self, response: Optional[Union[dict, Message]] = None, behaviour_args: Optional[dict] = None
     ):
         """
         Need to add some information before running verify()
 
         :return: dictionary with arguments to the verify call
         """
         _context = self.upstream_get("context")
         _entity = self.upstream_get("entity")
 
         kwargs = {
             "client_id": _entity.get_client_id(),
             "iss": _context.issuer,
-            "keyjar": self.upstream_get('attribute', 'keyjar'),
+            "keyjar": self.upstream_get("attribute", "keyjar"),
             "verify": True,
             "skew": _context.clock_skew,
         }
 
         _reg_resp = _context.registration_response
         if _reg_resp:
             for attr, param in IDT2REG.items():
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/oidc/authorization.py` & `idpyoidc-2.1.0/src/idpyoidc/client/oidc/authorization.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,60 +31,59 @@
     response_cls = oidc.AuthorizationResponse
     error_msg = oidc.ResponseMessage
 
     _supports = {
         "request_object_signing_alg_values_supported": claims.get_signing_algs,
         "request_object_encryption_alg_values_supported": claims.get_encryption_algs,
         "request_object_encryption_enc_values_supported": claims.get_encryption_encs,
-        "response_types_supported": ["code", "token", "code token", 'id_token', 'id_token token',
-                                     'code id_token', 'code idtoken token'],
-        'request_parameter_supported': None,
-        'request_uri_parameter_supported': None,
+        "response_types_supported": ["code", "id_token", "code id_token"],
+        "request_parameter_supported": None,
+        "request_uri_parameter_supported": None,
         "request_uris": None,
         "request_parameter": None,
         "encrypt_request_object_supported": False,
         "redirect_uris": None,
-        "response_modes_supported": ['query', 'fragment', 'form_post']
+        "response_modes_supported": ["query", "fragment", "form_post"],
     }
 
     _callback_path = {
         "request_uris": ["req"],
-        "redirect_uris": {  # based on response_types
-            "code": "authz_cb",
-            "token": "authz_tok_cb",
-            "form_post": "form"
-        }
+        "redirect_uris": {  # based on response_mode
+            "query": "authz_cb",
+            "fragment": "authz_tok_cb",
+            "form_post": "authz_cb_form",
+        },
     }
 
     def __init__(self, upstream_get, conf=None, request_args: Optional[dict] = None):
         authorization.Authorization.__init__(self, upstream_get, conf=conf)
         self.default_request_args.update({"scope": ["openid"]})
         if request_args:
             self.default_request_args.update(request_args)
         self.pre_construct = [
             self.set_state,
             pre_construct_pick_redirect_uri,
             self.oidc_pre_construct,
         ]
         self.post_construct = [self.oidc_post_construct]
-        if 'scope' not in self.default_request_args:
-            self.default_request_args['scope'] = ['openid']
+        if "scope" not in self.default_request_args:
+            self.default_request_args["scope"] = ["openid"]
 
     def set_state(self, request_args, **kwargs):
         _context = self.upstream_get("context")
         try:
             _state = kwargs["state"]
         except KeyError:
             try:
                 _state = request_args["state"]
             except KeyError:
                 _state = _context.cstate.create_key()
 
         request_args["state"] = _state
-        _context.cstate.set(_state, {'iss': _context.issuer})
+        _context.cstate.set(_state, {"iss": _context.issuer})
         return request_args, {}
 
     def update_service_context(self, resp, key="", **kwargs):
         _context = self.upstream_get("context")
 
         if "expires_in" in resp:
             resp["__expires_at"] = time_sans_frac() + int(resp["expires_in"])
@@ -97,16 +96,19 @@
     def post_parse_response(self, response, **kwargs):
         response = authorization.Authorization.post_parse_response(self, response, **kwargs)
 
         _idt = response.get(verified_claim_name("id_token"))
         if _idt:
             # If there is a verified ID Token then we have to do nonce
             # verification.
-            _req_nonce = self.upstream_get("context").cstate.get_set(
-                response["state"], claim=['nonce']).get('nonce')
+            _req_nonce = (
+                self.upstream_get("context")
+                .cstate.get_set(response["state"], claim=["nonce"])
+                .get("nonce")
+            )
             if _req_nonce:
                 _id_token_nonce = _idt.get("nonce")
                 if not _id_token_nonce:
                     raise MissingRequiredAttribute("nonce")
                 elif _req_nonce != _id_token_nonce:
                     raise ValueError("Invalid nonce")
         return response
@@ -119,25 +121,26 @@
         try:
             _response_types = [request_args["response_type"]]
         except KeyError:
             _response_types = _context.get_usage("response_types")
             if _response_types:
                 request_args["response_type"] = _response_types[0]
             else:
+                _response_types = ["code"]
                 request_args["response_type"] = "code"
 
         # For OIDC 'openid' is required in scope
         if "scope" not in request_args:
             _scope = _context.get_usage("scope")
             if _scope:
                 request_args["scope"] = _scope
             else:
                 _scope = _context.get_preference("scopes_supported")
                 if _scope:
-                    request_args['scope'] = _scope
+                    request_args["scope"] = _scope
                 else:
                     request_args["scope"] = "openid"
         elif "openid" not in request_args["scope"]:
             request_args["scope"].append("openid")
 
         # 'code' and/or 'id_token' in response_type means an ID Roken
         # will eventually be returned, hence the need for a nonce
@@ -206,23 +209,23 @@
 
         fid = open(filename, mode="w")
         fid.write(req)
         fid.close()
         return _webname
 
     def construct_request_parameter(
-            self, req, request_param, audience=None, expires_in=0, **kwargs
+        self, req, request_param, audience=None, expires_in=0, **kwargs
     ):
         """Construct a request parameter"""
         alg = self.get_request_object_signing_alg(**kwargs)
         kwargs["request_object_signing_alg"] = alg
 
         _context = self.upstream_get("context")
         if "keys" not in kwargs and alg and alg != "none":
-            kwargs["keys"] = self.upstream_get('attribute', 'keyjar')
+            kwargs["keys"] = self.upstream_get("attribute", "keyjar")
 
         if alg == "none":
             kwargs["keys"] = []
 
         # This is the issuer of the JWT, that is me !
         _issuer = kwargs.get("issuer")
         if _issuer is None:
@@ -253,21 +256,21 @@
                 "lifetime",
             ]
             if k in kwargs
         }
 
         _req_jwt = make_openid_request(req, **_mor_args)
 
-        if 'target' not in kwargs:
-            kwargs['target'] = _context.provider_info.get("issuer", _context.issuer)
+        if "target" not in kwargs:
+            kwargs["target"] = _context.provider_info.get("issuer", _context.issuer)
 
         # Should the request be encrypted
-        _req_jwte = request_object_encryption(_req_jwt, _context,
-                                              self.upstream_get('attribute', 'keyjar'),
-                                              **kwargs)
+        _req_jwte = request_object_encryption(
+            _req_jwt, _context, self.upstream_get("attribute", "keyjar"), **kwargs
+        )
         return _req_jwte
 
     def oidc_post_construct(self, req, **kwargs):
         """
         Modify the request arguments.
 
         :param req: The request
@@ -312,26 +315,25 @@
             _keys = [k for k in req.keys() if k not in _leave]
             for k in _keys:
                 del req[k]
 
         return req
 
     def gather_verify_arguments(
-            self, response: Optional[Union[dict, Message]] = None,
-            behaviour_args: Optional[dict] = None
+        self, response: Optional[Union[dict, Message]] = None, behaviour_args: Optional[dict] = None
     ):
         """
         Need to add some information before running verify()
 
         :return: dictionary with arguments to the verify call
         """
         _context = self.upstream_get("context")
         kwargs = {
             "iss": _context.issuer,
-            "keyjar": self.upstream_get('attribute', 'keyjar'),
+            "keyjar": self.upstream_get("attribute", "keyjar"),
             "verify": True,
             "skew": _context.clock_skew,
         }
 
         _client_id = _context.get_client_id()
         if _client_id:
             kwargs["client_id"] = _client_id
@@ -351,47 +353,51 @@
         _verify_args = _context.get_usage("verify_args")
         if _verify_args:
             kwargs.update(_verify_args)
 
         return kwargs
 
     def _do_request_uris(self, base_url, hex, context, callback_uris):
-        _uri_name = 'request_uris'
-        if context.get_preference('request_parameter') == _uri_name:
+        _uri_name = "request_uris"
+        if context.get_preference("request_parameter") == _uri_name:
             if _uri_name not in callback_uris:
-                callback_uris[_uri_name] = self.get_uri(base_url,
-                                                        self._callback_path[_uri_name],
-                                                        hex)
+                callback_uris[_uri_name] = self.get_uri(
+                    base_url, self._callback_path[_uri_name], hex
+                )
         return callback_uris
 
     def _do_type(self, context, typ, response_types):
-        if typ == 'code' and 'code' in response_types:
-            if typ in context.get_preference('response_modes_supported'):
-                return True
-        elif typ == 'implicit':
-            if typ in context.get_preference('response_modes_supported'):
+        if typ == "code" and "code" in response_types:
+            if typ in context.get_preference("response_modes_supported"):
+                return "query"
+        elif typ == "implicit":
+            if typ in context.get_preference("response_modes_supported"):
                 if implicit_response_types(response_types):
-                    return True
-        elif typ == 'form_post':
-            if typ in context.get_preference('response_modes_supported'):
-                return True
-        return False
-
-    def construct_uris(self,
-                       base_url: str,
-                       hex: bytes,
-                       context: ServiceContext,
-                       targets: Optional[List[str]] = None,
-                       response_types: Optional[List[str]] = None):
-        _callback_uris = context.get_preference('callback_uris', {})
+                    return "fragment"
+        elif typ == "form_post":
+            if typ in context.get_preference("response_modes_supported"):
+                return "form_post"
+        return ''
+
+    def construct_uris(
+        self,
+        base_url: str,
+        hex: bytes,
+        context: ServiceContext,
+        targets: Optional[List[str]] = None,
+        response_types: Optional[List[str]] = None,
+    ):
+        _callback_uris = context.get_preference("callback_uris", {})
 
         for uri_name in self._callback_path.keys():
-            if uri_name == 'redirect_uris':
-                _callback_uris = self._do_redirect_uris(base_url, hex, context, _callback_uris,
-                                                        response_types)
-            elif uri_name == 'request_uris':
+            if uri_name == "redirect_uris":
+                _callback_uris = self._do_redirect_uris(
+                    base_url, hex, context, _callback_uris, response_types
+                )
+            elif uri_name == "request_uris":
                 _callback_uris = self._do_request_uris(base_url, hex, context, _callback_uris)
             else:
-                _callback_uris[uri_name] = self.get_uri(base_url, self._callback_path[uri_name],
-                                                        hex)
+                _callback_uris[uri_name] = self.get_uri(
+                    base_url, self._callback_path[uri_name], hex
+                )
 
         return _callback_uris
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/oidc/backchannel_authentication.py` & `idpyoidc-2.1.0/src/idpyoidc/client/oidc/backchannel_authentication.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/oidc/check_id.py` & `idpyoidc-2.1.0/src/idpyoidc/client/oidc/check_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,14 @@
     service_name = "check_id"
 
     def __init__(self, upstream_get, conf=None):
         Service.__init__(self, upstream_get, conf=conf)
         self.pre_construct = [self.oidc_pre_construct]
 
     def oidc_pre_construct(self, request_args: Optional[dict] = None, **kwargs):
-        _args = self.upstream_get("context").cstate.get_set(
-            kwargs["state"],
-            claim=["id_token"]
-        )
+        _args = self.upstream_get("context").cstate.get_set(kwargs["state"], claim=["id_token"])
         if request_args:
             request_args.update()
         else:
             request_args = _args
 
         return request_args, {}
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/oidc/check_session.py` & `idpyoidc-2.1.0/src/idpyoidc/client/oidc/check_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     service_name = "check_session"
 
     def __init__(self, upstream_get, conf=None):
         Service.__init__(self, upstream_get, conf=conf)
         self.pre_construct = [self.oidc_pre_construct]
 
     def oidc_pre_construct(self, request_args=None, **kwargs):
-        _args = self.upstream_get("context").cstate.get_set(kwargs["state"],
-                                                            claim=["id_token"])
+        _args = self.upstream_get("context").cstate.get_set(kwargs["state"], claim=["id_token"])
         if request_args:
             request_args.update(_args)
         else:
             request_args = _args
 
         return request_args, {}
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/oidc/end_session.py` & `idpyoidc-2.1.0/src/idpyoidc/client/oidc/end_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,26 +18,26 @@
     endpoint_name = "end_session_endpoint"
     synchronous = True
     service_name = "end_session"
     response_body_type = "html"
 
     _supports = {
         "post_logout_redirect_uris": None,
-        'frontchannel_logout_supported': None,
+        "frontchannel_logout_supported": None,
         "frontchannel_logout_uri": None,
         "frontchannel_logout_session_required": None,
-        'backchannel_logout_supported': None,
+        "backchannel_logout_supported": None,
         "backchannel_logout_uri": None,
-        "backchannel_logout_session_required": None
+        "backchannel_logout_session_required": None,
     }
 
     _callback_path = {
         "frontchannel_logout_uri": "fc_logout",
         "backchannel_logout_uri": "bc_logout",
-        "post_logout_redirect_uris": ["session_logout"]
+        "post_logout_redirect_uris": ["session_logout"],
     }
 
     def __init__(self, upstream_get, conf=None):
         Service.__init__(self, upstream_get, conf=conf)
         self.pre_construct = [
             self.get_id_token_hint,
             self.add_post_logout_redirect_uri,
@@ -49,15 +49,15 @@
         Add id_token_hint to request
 
         :param request_args:
         :param kwargs:
         :return:
         """
 
-        _id_token = self.upstream_get("context").cstate.get_claim(kwargs["state"], claim='id_token')
+        _id_token = self.upstream_get("context").cstate.get_claim(kwargs["state"], claim="id_token")
         if _id_token:
             request_args["id_token_hint"] = _id_token
 
         return request_args, {}
 
     def add_post_logout_redirect_uri(self, request_args=None, **kwargs):
         if "post_logout_redirect_uri" not in request_args:
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/oidc/provider_info_discovery.py` & `idpyoidc-2.1.0/src/idpyoidc/client/oidc/provider_info_discovery.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 from typing import Optional
 
+from idpyoidc.client.defaults import OIDCONF_PATTERN
 from idpyoidc.client.oauth2 import server_metadata
 from idpyoidc.message import oidc
 from idpyoidc.message.oauth2 import ResponseMessage
 
 __author__ = "Roland Hedberg"
 
 logger = logging.getLogger(__name__)
@@ -24,45 +25,48 @@
     :param kwargs: Possible extra keyword arguments
     :return: A possibly augmented set of request arguments.
     """
     _work_environment = service.upstream_get("context").claims
     if "redirect_uris" not in request_args:
         # Callbacks is a dictionary with callback type 'code', 'implicit',
         # 'form_post' as keys.
-        _callback = _work_environment.get_preference('callback')
+        _callback = _work_environment.get_preference("callback")
         if _callback:
             # Filter out local additions.
             _uris = [v for k, v in _callback.items() if not k.startswith("__")]
             request_args["redirect_uris"] = _uris
         else:
             request_args["redirect_uris"] = _work_environment.get_preference(
-                "redirect_uris", _work_environment.supports.get('redirect_uris'))
+                "redirect_uris", _work_environment.supports.get("redirect_uris")
+            )
 
     return request_args, {}
 
 
 class ProviderInfoDiscovery(server_metadata.ServerMetadata):
     msg_type = oidc.Message
     response_cls = oidc.ProviderConfigurationResponse
     error_msg = ResponseMessage
     service_name = "provider_info"
+    url_pattern = OIDCONF_PATTERN
 
     _include = {}
     _supports = {}
 
     def __init__(self, upstream_get, conf=None):
         server_metadata.ServerMetadata.__init__(self, upstream_get, conf=conf)
 
-    def update_service_context(self, resp, key: Optional[str] = '', **kwargs):
+    def update_service_context(self, resp, key: Optional[str] = "", **kwargs):
         _context = self.upstream_get("context")
         self._update_service_context(resp)
         _context.map_supported_to_preferred(resp)
         if "pre_load_keys" in self.conf and self.conf["pre_load_keys"]:
-            _jwks = self.upstream_get('attribute', 'keyjar').export_jwks_as_json(
-                issuer=resp["issuer"])
+            _jwks = self.upstream_get("attribute", "keyjar").export_jwks_as_json(
+                issuer=resp["issuer"]
+            )
             logger.info("Preloaded keys for {}: {}".format(resp["issuer"], _jwks))
 
     def match_preferences(self, pcr=None, issuer=None):
         """
         Match the clients supports against what the provider can do.
         This is to prepare for later client registration and/or what
         functionality the client actually will use.
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/oidc/read_registration.py` & `idpyoidc-2.1.0/src/idpyoidc/client/oidc/read_registration.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,17 +15,15 @@
     synchronous = True
     service_name = "registration_read"
     http_method = "GET"
     default_authn_method = "client_secret_basic"
 
     def get_endpoint(self):
         try:
-            return self.upstream_get("context").registration_response[
-                "registration_client_uri"
-            ]
+            return self.upstream_get("context").registration_response["registration_client_uri"]
         except KeyError:
             return ""
 
     def get_authn_header(self, request, authn_method, **kwargs):
         """
         Construct an authorization specification to be sent in the
         HTTP header.
@@ -36,13 +34,11 @@
         :return: A set of keyword arguments to be sent in the HTTP header.
         """
         headers = {}
 
         if authn_method == "client_secret_basic":
             LOGGER.debug("Client authn method: %s", authn_method)
             headers["Authorization"] = "Bearer {}".format(
-                self.upstream_get("context").registration_response[
-                    "registration_access_token"
-                ]
+                self.upstream_get("context").registration_response["registration_access_token"]
             )
 
         return headers
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/oidc/refresh_access_token.py` & `idpyoidc-2.1.0/src/idpyoidc/client/oidc/refresh_access_token.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/oidc/registration.py` & `idpyoidc-2.1.0/src/idpyoidc/client/oidc/registration.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,30 +68,29 @@
         _context = self.upstream_get("context")
         _context.map_preferred_to_registered(resp)
 
         _context.registration_response = resp
         _client_id = _context.get_usage("client_id")
         if _client_id:
             _context.client_id = _client_id
-            _keyjar = self.upstream_get('attribute', 'keyjar')
+            _keyjar = self.upstream_get("attribute", "keyjar")
             if _keyjar:
                 if _client_id not in _keyjar:
                     _keyjar.import_jwks(_keyjar.export_jwks(True, ""), issuer_id=_client_id)
             _client_secret = _context.get_usage("client_secret")
             if _client_secret:
                 if not _keyjar:
-                    _entity = self.upstream_get('unit')
+                    _entity = self.upstream_get("unit")
                     _keyjar = _entity.keyjar = KeyJar()
 
                 _context.client_secret = _client_secret
                 _keyjar.add_symmetric("", _client_secret)
                 _keyjar.add_symmetric(_client_id, _client_secret)
                 try:
-                    _context.set_usage("client_secret_expires_at",
-                                       resp["client_secret_expires_at"])
+                    _context.set_usage("client_secret_expires_at", resp["client_secret_expires_at"])
                 except KeyError:
                     pass
 
         try:
             _context.set_usage("registration_access_token", resp["registration_access_token"])
         except KeyError:
             pass
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/oidc/userinfo.py` & `idpyoidc-2.1.0/src/idpyoidc/client/oidc/userinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,36 +35,36 @@
 class UserInfo(Service):
     msg_type = Message
     response_cls = oidc.OpenIDSchema
     error_msg = oidc.ResponseMessage
     endpoint_name = "userinfo_endpoint"
     service_name = "userinfo"
     default_authn_method = "bearer_header"
+    response_body_type = "jose"
 
     _supports = {
         "userinfo_signing_alg_values_supported": get_signing_algs,
         "userinfo_encryption_alg_values_supported": get_encryption_algs,
         "userinfo_encryption_enc_values_supported": get_encryption_encs,
-        "encrypt_userinfo_supported": False
+        "encrypt_userinfo_supported": False,
     }
 
     def __init__(self, upstream_get, conf=None):
         Service.__init__(self, upstream_get, conf=conf)
         self.pre_construct = [self.oidc_pre_construct, carry_state]
 
     def oidc_pre_construct(self, request_args=None, **kwargs):
         if request_args is None:
             request_args = {}
 
         if "access_token" in request_args:
             pass
         else:
             request_args = self.upstream_get("context").cstate.get_set(
-                kwargs["state"],
-                claim=["access_token"]
+                kwargs["state"], claim=["access_token"]
             )
 
         return request_args, {}
 
     def post_parse_response(self, response, **kwargs):
         _context = self.upstream_get("context")
         _current = _context.cstate
@@ -84,15 +84,15 @@
             pass
         else:
             for csrc, spec in _csrc.items():
                 if "JWT" in spec:
                     try:
                         aggregated_claims = Message().from_jwt(
                             spec["JWT"].encode("utf-8"),
-                            keyjar=self.upstream_get('attribute', 'keyjar')
+                            keyjar=self.upstream_get("attribute", "keyjar"),
                         )
                     except MissingSigningKey as err:
                         logger.warning(
                             f"Error encountered while unpacking aggregated claims: {err}"
                         )
                     else:
                         claims = [
@@ -106,27 +106,26 @@
         for meth in self.post_parse_process:
             response = meth(response, _current, kwargs["state"])
 
         _current.update(kwargs["state"], response)
         return response
 
     def gather_verify_arguments(
-            self, response: Optional[Union[dict, Message]] = None,
-            behaviour_args: Optional[dict] = None
+        self, response: Optional[Union[dict, Message]] = None, behaviour_args: Optional[dict] = None
     ):
         """
         Need to add some information before running verify()
 
         :return: dictionary with arguments to the verify call
         """
         _context = self.upstream_get("context")
         kwargs = {
             "client_id": _context.get_client_id(),
             "iss": _context.issuer,
-            "keyjar": self.upstream_get('attribute', 'keyjar'),
+            "keyjar": self.upstream_get("attribute", "keyjar"),
             "verify": True,
             "skew": _context.clock_skew,
         }
 
         _reg_resp = _context.registration_response
         if _reg_resp:
             for attr, param in UI2REG.items():
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/oidc/utils.py` & `idpyoidc-2.1.0/src/idpyoidc/client/oidc/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     _kty = alg2keytype(encalg)
 
     try:
         _kid = kwargs["enc_kid"]
     except KeyError:
         _kid = ""
 
-    _target = kwargs.get('target', kwargs.get('recv', None))
+    _target = kwargs.get("target", kwargs.get("recv", None))
     if _target is None:
         raise MissingRequiredAttribute("No target specified")
 
     if _kid:
         _keys = keyjar.get_encrypt_key(_kty, issuer_id=_target, kid=_kid)
         _jwe["kid"] = _kid
     else:
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/oidc/webfinger.py` & `idpyoidc-2.1.0/src/idpyoidc/client/oidc/webfinger.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,16 +45,16 @@
             links = resp["links"]
         except KeyError:
             raise MissingRequiredAttribute("links")
         else:
             for link in links:
                 if link["rel"] == self.rel:
                     _href = link["href"]
-                    _context = self.upstream_get('service_context')
-                    _http_allowed = 'http_links' in _context.get("allow", default={})
+                    _context = self.upstream_get("service_context")
+                    _http_allowed = "http_links" in _context.get("allow", default={})
 
                     if _href.startswith("http://") and not _http_allowed:
                         raise ValueError("http link not allowed ({})".format(_href))
 
                     self.upstream_get("context").issuer = link["href"]
                     break
         return resp
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/provider/github.py` & `idpyoidc-2.1.0/src/idpyoidc/client/provider/github.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     msg_type = oauth2.AccessTokenRequest
     response_cls = AccessTokenResponse
     error_msg = oauth2.TokenErrorResponse
     response_body_type = "urlencoded"
 
     _supports = {
         "token_endpoint_auth_methods_supported": get_client_authn_methods,
-        "token_endpoint_auth_signing_alg_values_supported": get_signing_algs
+        "token_endpoint_auth_signing_alg_values_supported": get_signing_algs,
     }
 
 
 class UserInfo(userinfo.UserInfo):
     response_cls = Message
     error_msg = ResponseMessage
     default_authn_method = ""
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/provider/linkedin.py` & `idpyoidc-2.1.0/src/idpyoidc/client/provider/linkedin.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,13 +31,13 @@
 class AccessToken(access_token.AccessToken):
     msg_type = oauth2.AccessTokenRequest
     response_cls = AccessTokenResponse
     error_msg = oauth2.TokenErrorResponse
 
     _supports = {
         "token_endpoint_auth_methods_supported": get_client_authn_methods,
-        "token_endpoint_auth_signing_alg_values_supported": get_signing_algs
+        "token_endpoint_auth_signing_alg_values_supported": get_signing_algs,
     }
 
 
 class UserInfo(userinfo.UserInfo):
     response_cls = UserSchema
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/rp_handler.py` & `idpyoidc-2.1.0/src/idpyoidc/server/oauth2/authorization.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1055 +1,1183 @@
+import json
 import logging
-import sys
-import traceback
+from typing import List
 from typing import Optional
+from typing import Union
+from urllib.parse import unquote
+from urllib.parse import urlencode
+from urllib.parse import urlparse
 
 from cryptojwt import as_unicode
-from cryptojwt import KeyJar
-from cryptojwt.key_bundle import keybundle_from_local_file
-from cryptojwt.key_jar import init_key_jar
+from cryptojwt import b64d
+from cryptojwt.jwe.exception import JWEException
+from cryptojwt.jws.exception import NoSuitableSigningKeys
 from cryptojwt.utils import as_bytes
+from cryptojwt.utils import b64e
 
-from idpyoidc import verified_claim_name
-from idpyoidc.client.defaults import DEFAULT_CLIENT_CONFIGS
-from idpyoidc.client.defaults import DEFAULT_OIDC_SERVICES
-from idpyoidc.client.defaults import DEFAULT_RP_KEY_DEFS
-from idpyoidc.client.exception import ConfigurationError
-from idpyoidc.client.exception import OidcServiceError
-from idpyoidc.exception import MessageException
-from idpyoidc.exception import MissingRequiredAttribute
-from idpyoidc.exception import NotForMe
-from idpyoidc.message.oauth2 import is_error_message
-from idpyoidc.message.oidc import AuthorizationRequest
+from idpyoidc import claims
+from idpyoidc.exception import ImproperlyConfigured
+from idpyoidc.exception import ParameterError
+from idpyoidc.exception import URIError
+from idpyoidc.message import Message
+from idpyoidc.message import oauth2
+from idpyoidc.message.oauth2 import AuthorizationRequest
 from idpyoidc.message.oidc import AuthorizationResponse
-from idpyoidc.message.oidc import Claims
-from idpyoidc.message.oidc import OpenIDSchema
-from idpyoidc.message.oidc import RegistrationRequest
-from idpyoidc.message.oidc.session import BackChannelLogoutRequest
+from idpyoidc.message.oidc import verified_claim_name
+from idpyoidc.server.authn_event import create_authn_event
+from idpyoidc.server.cookie_handler import compute_session_state
+from idpyoidc.server.endpoint import Endpoint
+from idpyoidc.server.endpoint_context import EndpointContext
+from idpyoidc.server.exception import InvalidRequest
+from idpyoidc.server.exception import NoSuchAuthentication
+from idpyoidc.server.exception import RedirectURIError
+from idpyoidc.server.exception import ServiceError
+from idpyoidc.server.exception import TamperAllert
+from idpyoidc.server.exception import ToOld
+from idpyoidc.server.exception import UnAuthorizedClientScope
+from idpyoidc.server.exception import UnknownClient
+from idpyoidc.server.session import Revoked
+from idpyoidc.server.token.exception import UnknownToken
+from idpyoidc.server.user_authn.authn_context import pick_auth
 from idpyoidc.time_util import utc_time_sans_frac
-from idpyoidc.util import add_path
 from idpyoidc.util import rndstr
-from . import oidc
-from .oauth2 import Client
-from .oauth2 import dynamic_provider_info_discovery
-from .oauth2.utils import pick_redirect_uri
-from ..message.oauth2 import ResponseMessage
-
-logger = logging.getLogger(__name__)
+from idpyoidc.util import split_uri
+from idpyoidc.util import importer
 
 
-class RPHandler(object):
-
-    def __init__(
-            self,
-            base_url: Optional[str] = "",
-            client_configs=None,
-            services=None,
-            keyjar=None,
-            hash_seed="",
-            verify_ssl=True,
-            client_cls=None,
-            state_db=None,
-            httpc=None,
-            httpc_params=None,
-            config=None,
-            **kwargs,
-    ):
-        self.base_url = base_url
-        _jwks_path = kwargs.get("jwks_path")
+logger = logging.getLogger(__name__)
 
-        if config:
-            if not hash_seed:
-                self.hash_seed = config.hash_seed
-            if not keyjar:
-                self.keyjar = init_key_jar(**config.key_conf, issuer_id="")
-            if not client_configs:
-                self.client_configs = config.clients
-        else:
-            if hash_seed:
-                self.hash_seed = as_bytes(hash_seed)
-            else:
-                self.hash_seed = as_bytes(rndstr(32))
+# For the time being. This is JAR specific and should probably be configurable.
+ALG_PARAMS = {
+    "sign": [
+        "request_object_signing_alg",
+        "request_object_signing_alg_values_supported",
+    ],
+    "enc_alg": [
+        "request_object_encryption_alg",
+        "request_object_encryption_alg_values_supported",
+    ],
+    "enc_enc": [
+        "request_object_encryption_enc",
+        "request_object_encryption_enc_values_supported",
+    ],
+}
+
+FORM_POST = """<html>
+  <head>
+    <title>Submit This Form</title>
+  </head>
+  <body onload="javascript:document.forms[0].submit()">
+    <form method="post" action="{action}">
+        {inputs}
+    </form>
+  </body>
+</html>"""
 
-            if keyjar is None:
-                self.keyjar = init_key_jar(**DEFAULT_RP_KEY_DEFS, issuer_id="")
-                self.keyjar.import_jwks_as_json(self.keyjar.export_jwks_as_json(True, ""), base_url)
-                if _jwks_path is None:
-                    _jwks_path = DEFAULT_RP_KEY_DEFS["public_path"]
-            else:
-                self.keyjar = keyjar
 
-            if client_configs is None:
-                self.client_configs = DEFAULT_CLIENT_CONFIGS
-            else:
-                self.client_configs = client_configs
+def inputs(form_args):
+    """
+    Creates list of input elements
+    """
+    element = []
+    html_field = '<input type="hidden" name="{}" value="{}"/>'
+    for name, value in form_args.items():
+        if name == "scope" and isinstance(value, list):
+            value = " ".join(value)
+        element.append(html_field.format(name, value))
+    return "\n".join(element)
+
+
+def max_age(request):
+    verified_request = verified_claim_name("request")
+    return request.get(verified_request, {}).get("max_age") or request.get("max_age", 0)
+
+
+def verify_uri(
+    context: EndpointContext,
+    request: Union[dict, Message],
+    uri_type: str,
+    client_id: Optional[str] = None,
+):
+    """
+    A redirect URI
+    MUST NOT contain a fragment
+    MAY contain query component
+
+    :param context: An EndpointContext instance
+    :param request: The authorization request
+    :param uri_type: redirect_uri or post_logout_redirect_uri
+    :return: An error response if the redirect URI is faulty otherwise
+        None
+    """
+    _cid = request.get("client_id", client_id)
 
-        if _jwks_path:
-            self.jwks_uri = add_path(base_url, _jwks_path)
-        else:
-            self.jwks_uri = ""
-            if len(self.keyjar):
-                self.jwks = self.keyjar.export_jwks()
-            else:
-                self.jwks = {}
+    if not _cid:
+        logger.error("No client id found")
+        raise UnknownClient("No client_id provided")
 
-        if state_db:
-            self.state_db = state_db
-        else:
-            self.state_db = {}
+    _uri = request.get(uri_type)
+    if _uri is None:
+        raise ValueError(f"Wrong uri_type: {uri_type}")
 
-        self.extra = kwargs
+    _redirect_uri = unquote(_uri)
 
-        self.client_cls = client_cls or oidc.RP
-        if services is None:
-            self.services = DEFAULT_OIDC_SERVICES
-        else:
-            self.services = services
+    part = urlparse(_redirect_uri)
+    if part.fragment:
+        raise URIError("Contains fragment")
 
-        # keep track on which RP instance that serves which OP
-        self.issuer2rp = {}
-        self.hash2issuer = {}
-        self.httpc = httpc
+    (_base, _query) = split_uri(_redirect_uri)
 
-        if not httpc_params:
-            self.httpc_params = {"verify": verify_ssl}
-        else:
-            self.httpc_params = httpc_params
+    # Get the clients registered redirect uris
+    client_info = context.cdb.get(_cid)
+    if client_info is None:
+        raise KeyError("No such client")
 
-        if not self.keyjar.httpc_params:
-            self.keyjar.httpc_params = self.httpc_params
+    if uri_type == "redirect_uri":
+        redirect_uris = client_info.get(f"{uri_type}s")
+    else:
+        redirect_uris = client_info.get(f"{uri_type}")
 
-    def state2issuer(self, state):
-        """
-        Given the state value find the Issuer ID of the OP/AS that state value
-        was used against.
-        Will raise a KeyError if the state is unknown.
+    if redirect_uris is None:
+        raise RedirectURIError(f"No registered {uri_type} for {_cid}")
+    else:
+        match = False
+        for _item in redirect_uris:
+            if isinstance(_item, str):
+                regbase = _item
+                rquery = {}
+            else:
+                regbase, rquery = _item
 
-        :param state: The state value
-        :return: An Issuer ID
-        """
-        for _rp in self.issuer2rp.values():
-            _iss = _rp.get_context().cstate.get_set(
-                state, claim=['iss']).get('iss')
-            if _iss:
-                return _iss
-        return None
+            # The URI MUST exactly match one of the Redirection URI
+            if _base == regbase:
+                # every registered query component must exist in the uri
+                if rquery:
+                    if not _query:
+                        raise ValueError("Missing query part")
+
+                    for key, vals in rquery.items():
+                        if key not in _query:
+                            raise ValueError('"{}" not in query part'.format(key))
+
+                        for val in vals:
+                            if val not in _query[key]:
+                                raise ValueError("{}={} value not in query part".format(key, val))
+
+                # and vice versa, every query component in the uri
+                # must be registered
+                if _query:
+                    if not rquery:
+                        raise ValueError("No registered query part")
+
+                    for key, vals in _query.items():
+                        if key not in rquery:
+                            raise ValueError('"{}" extra in query part'.format(key))
+                        for val in vals:
+                            if val not in rquery[key]:
+                                raise ValueError("Extra {}={} value in query part".format(key, val))
+                match = True
+                break
+        if not match:
+            raise RedirectURIError("Doesn't match any registered uris")
 
-    def pick_config(self, issuer):
-        """
-        From the set of client configurations pick one based on the issuer ID.
-        Will raise a KeyError if issuer is unknown.
 
-        :param issuer: Issuer ID
-        :return: A client configuration
-        """
-        return self.client_configs[issuer]
+def join_query(base, query):
+    """
 
-    def get_session_information(self, key, client=None):
-        """
-        This is the second of the methods users of this class should know about.
-        It will return the complete session information as an
-        :py:class:`idpyoidc.client.current.Current` instance.
+    :param base: URL base
+    :param query: query part as a dictionary
+    :return:
+    """
+    if query:
+        return "{}?{}".format(base, urlencode(query, doseq=True))
+    else:
+        return base
 
-        :param key: The session key (state)
-        :return: A State instance
-        """
-        if not client:
-            client = self.get_client_from_session_key(key)
 
-        return client.get_context().cstate.get(key)
+def get_uri(context, request, uri_type):
+    """verify that the redirect URI is reasonable.
 
-    def init_client(self, issuer):
-        """
-        Initiate a Client instance. Specifically which Client class is used
-        is decided by configuration.
+    :param context: An EndpointContext instance
+    :param request: The Authorization request
+    :param uri_type: 'redirect_uri' or 'post_logout_redirect_uri'
+    :return: redirect_uri
+    """
+    uri = ""
 
-        :param issuer: An issuer ID
-        :return: A Client instance
-        """
+    if uri_type in request:
+        verify_uri(context, request, uri_type)
+        uri = request[uri_type]
+    else:
+        uris = f"{uri_type}s"
+        client_id = str(request["client_id"])
+        if client_id in context.cdb:
+            _specs = context.cdb[client_id].get(uris)
+            if not _specs:
+                raise ParameterError(f"Missing '{uri_type}' and none registered")
 
-        logger.debug(20 * "*" + " init_client " + 20 * "*")
+            if len(_specs) > 1:
+                raise ParameterError(f"Missing '{uri_type}' and more than one registered")
 
-        try:
-            _cnf = self.pick_config(issuer)
-        except KeyError:
-            _cnf = self.pick_config("")
-            _cnf["issuer"] = issuer
+            uri = join_query(*_specs[0])
+        else:
+            raise UnknownClient(client_id)
 
-        try:
-            _services = _cnf["services"]
-        except KeyError:
-            _services = self.services
+    return uri
 
-        if 'base_url' not in _cnf:
-            _cnf['base_url'] = self.base_url
 
-        if self.jwks_uri:
-            _cnf['jwks_uri'] = self.jwks_uri
+def authn_args_gather(
+    request: Union[AuthorizationRequest, dict],
+    authn_class_ref: str,
+    cinfo: dict,
+    **kwargs,
+):
+    """
+    Gather information to be used by the authentication method
 
-        try:
-            client = self.client_cls(
-                services=_services,
-                config=_cnf,
-                httpc=self.httpc,
-                httpc_params=self.httpc_params,
-            )
-        except Exception as err:
-            logger.error("Failed initiating client: {}".format(err))
-            message = traceback.format_exception(*sys.exc_info())
-            logger.error(message)
-            raise
-
-        _context = client.get_context()
-        if _context.iss_hash:
-            self.hash2issuer[_context.iss_hash] = issuer
-        # If non persistent
-        _keyjar = client.keyjar
-        if not _keyjar:
-            _keyjar = KeyJar()
-            _keyjar.httpc_params.update(self.httpc_params)
-
-        for iss in self.keyjar.owners():
-            _keyjar.import_jwks(self.keyjar.export_jwks(issuer_id=iss, private=True), iss)
-
-        client.keyjar = _keyjar
-        # If persistent nothing has to be copied
-
-        _context.base_url = self.base_url
-        _context.jwks_uri = self.jwks_uri
-        return client
-
-    def do_provider_info(
-            self,
-            client: Optional[Client] = None,
-            state: Optional[str] = "",
-            behaviour_args: Optional[dict] = None,
-    ) -> str:
-        """
-        Either get the provider info from configuration or through dynamic
-        discovery.
+    :param request: The request either as a dictionary or as a Message instance
+    :param authn_class_ref: Authentication class reference
+    :param cinfo: Client information
+    :param kwargs: Extra keyword arguments
+    :return: Authentication arguments
+    """
+    authn_args = {}
 
-        :param behaviour_args:
-        :param client: A Client instance
-        :param state: A key by which the state of the session can be
-            retrieved
-        :return: issuer ID
-        """
-        logger.debug(20 * "*" + " do_provider_info " + 20 * "*")
+    if isinstance(request, Message):
+        authn_args["query"] = request.to_urlencoded()
+    elif isinstance(request, dict):
+        authn_args["query"] = urlencode(request)
+    else:
+        raise ValueError("Wrong request format")
 
-        if not client:
-            if state:
-                client = self.get_client_from_session_key(state)
-            else:
-                raise ValueError("Missing state/session key")
+    authn_args.update({"authn_class_ref": authn_class_ref, "return_uri": request["redirect_uri"]})
 
-        _context = client.get_context()
-        if not _context.get("provider_info"):
-            dynamic_provider_info_discovery(client, behaviour_args=behaviour_args)
-            return _context.get("provider_info")["issuer"]
-        else:
-            _pi = _context.get("provider_info")
-            for key, val in _pi.items():
-                # All service endpoint parameters in the provider info has
-                # a name ending in '_endpoint' so I can look specifically
-                # for those
-                if key.endswith("_endpoint"):
-                    for _srv in client.get_services().values():
-                        # Every service has an endpoint_name assigned
-                        # when initiated. This name *MUST* match the
-                        # endpoint names used in the provider info
-                        if _srv.endpoint_name == key:
-                            _srv.endpoint = val
-
-            if "keys" in _pi:
-                _kj = client.get_attribute('keyjar')
-                for typ, _spec in _pi["keys"].items():
-                    if typ == "url":
-                        for _iss, _url in _spec.items():
-                            _kj.add_url(_iss, _url)
-                    elif typ == "file":
-                        for kty, _name in _spec.items():
-                            if kty == "jwks":
-                                _kj.import_jwks_from_file(_name, _context.get("issuer"))
-                            elif kty == "rsa":  # PEM file
-                                _kb = keybundle_from_local_file(_name, "der", ["sig"])
-                                _kj.add_kb(_context.get("issuer"), _kb)
-                    else:
-                        raise ValueError("Unknown provider JWKS type: {}".format(typ))
+    if "req_user" in kwargs:
+        authn_args["as_user"] = (kwargs["req_user"],)
 
-            _context.map_supported_to_preferred(info=_pi)
+    # Below are OIDC specific. Just ignore if OAuth2
+    if cinfo:
+        for attr in ["policy_uri", "logo_uri", "tos_uri"]:
+            if cinfo.get(attr):
+                authn_args[attr] = cinfo[attr]
 
-            try:
-                return _context.get("provider_info")["issuer"]
-            except KeyError:
-                return _context.get("issuer")
+    for attr in ["ui_locales", "acr_values", "login_hint"]:
+        if request.get(attr):
+            authn_args[attr] = request[attr]
 
-    def do_client_registration(
-            self,
-            client=None,
-            iss_id: Optional[str] = "",
-            state: Optional[str] = "",
-            request_args: Optional[dict] = None,
-            behaviour_args: Optional[dict] = None,
-    ):
-        """
-        Prepare for and do client registration if configured to do so
+    return authn_args
 
-        :param iss_id: Issuer ID
-        :param behaviour_args: To fine tune behaviour
-        :param client: A Client instance
-        :param state: A key by which the state of the session can be
-            retrieved
-        """
 
-        logger.debug(20 * "*" + " do_client_registration " + 20 * "*")
+def check_unknown_scopes_policy(request_info, client_id, context):
+    if not context.get_preference("deny_unknown_scopes"):
+        return
 
-        if not client:
-            if state:
-                client = self.get_client_from_session_key(state)
-            else:
-                raise ValueError("Missing state/session key")
+    scope = request_info["scope"]
+    filtered_scopes = set(context.scopes_handler.filter_scopes(scope, client_id=client_id))
+    scopes = set(scope)
+    # this prevents that authz would be released for unavailable scopes
+    if scopes != filtered_scopes:
+        diff = " ".join(scopes - filtered_scopes)
+        logger.warning(f"{client_id} requested unauthorized scopes: {diff}")
+        raise UnAuthorizedClientScope()
 
-        _context = client.get_context()
-        _iss = _context.get("issuer")
-        self.hash2issuer[iss_id] = _iss
 
-        # This should only be interesting if the client supports Single Log Out
-        # if _context.callback.get("post_logout_redirect_uri") is None:
-        #     _context.callback["post_logout_redirect_uri"] = [self.base_url]
+def validate_resource_indicators_policy(request, context, **kwargs):
+    if "resource" not in request:
+        return oauth2.AuthorizationErrorResponse(
+            error="invalid_target",
+            error_description="Missing resource parameter",
+        )
 
-        if not client.get_client_id():  # means I have to do dynamic client registration
-            if request_args is None:
-                request_args = {}
+    resource_servers_per_client = kwargs["resource_servers_per_client"]
+    client_id = request["client_id"]
 
-            if behaviour_args:
-                _params = RegistrationRequest().parameters()
-                request_args.update({k: v for k, v in behaviour_args.items() if k in _params})
+    if (
+        isinstance(resource_servers_per_client, dict)
+        and client_id not in resource_servers_per_client
+    ):
+        return oauth2.AuthorizationErrorResponse(
+            error="invalid_target",
+            error_description=f"Resources for client {client_id} not found",
+        )
 
-            load_registration_response(client, request_args=request_args)
-        else:
-            _context.map_preferred_to_registered()
+    if isinstance(resource_servers_per_client, dict):
+        permitted_resources = [res for res in resource_servers_per_client[client_id]]
+    else:
+        permitted_resources = [res for res in resource_servers_per_client]
 
-    def do_webfinger(self, user: str) -> Client:
-        """
-        Does OpenID Provider Issuer discovery using webfinger.
+    common_resources = list(set(request["resource"]).intersection(set(permitted_resources)))
+    if not common_resources:
+        return oauth2.AuthorizationErrorResponse(
+            error="invalid_target",
+            error_description=f"Invalid resource requested by client {client_id}",
+        )
 
-        :param user: Identifier for the target End-User that is the subject of the discovery
-            request.
-        :return: A Client instance
-        """
+    common_resources = [r for r in common_resources if r in context.cdb.keys()]
+    if not common_resources:
+        return oauth2.AuthorizationErrorResponse(
+            error="invalid_target",
+            error_description=f"Invalid resource requested by client {client_id}",
+        )
 
-        logger.debug(20 * "*" + " do_webfinger " + 20 * "*")
+    if client_id not in common_resources:
+        common_resources.append(client_id)
 
-        temporary_client = self.init_client("")
-        temporary_client.do_request("webfinger", resource=user)
-        return temporary_client
-
-    def client_setup(
-            self,
-            iss_id: Optional[str] = "",
-            user: Optional[str] = "",
-            behaviour_args: Optional[dict] = None,
-    ) -> Client:
-        """
-        First if no issuer ID is given then the identifier for the user is
-        used by the webfinger service to try to find the issuer ID.
-        Once the method has an issuer ID if no client is bound to this issuer
-        one is created and initiated with
-        the necessary information for the client to be able to communicate
-        with the OP/AS that has the provided issuer ID.
-
-        :param behaviour_args: To fine tune behaviour
-        :param iss_id: The issuer ID
-        :param user: A user identifier
-        :return: A :py:class:`idpyoidc.client.oidc.Client` instance
-        """
+    request["resource"] = common_resources
 
-        logger.debug(20 * "*" + " client_setup " + 20 * "*")
+    permitted_scopes = [context.cdb[r]["allowed_scopes"] for r in common_resources]
+    permitted_scopes = [r for res in permitted_scopes for r in res]
+    scopes = list(set(request.get("scope", [])).intersection(set(permitted_scopes)))
+    request["scope"] = scopes
+    return request
+
+
+class Authorization(Endpoint):
+    request_cls = oauth2.AuthorizationRequest
+    response_cls = oauth2.AuthorizationResponse
+    error_cls = oauth2.AuthorizationErrorResponse
+    request_format = "urlencoded"
+    response_format = "urlencoded"
+    response_placement = "url"
+    endpoint_name = "authorization_endpoint"
+    name = "authorization"
+
+    _supports = {
+        "claims_parameter_supported": True,
+        "request_parameter_supported": True,
+        "request_uri_parameter_supported": True,
+        "response_types_supported": ["code"],
+        "response_modes_supported": ["query", "fragment", "form_post"],
+        "request_object_signing_alg_values_supported": claims.get_signing_algs,
+        "request_object_encryption_alg_values_supported": claims.get_encryption_algs,
+        "request_object_encryption_enc_values_supported": claims.get_encryption_encs,
+        # "grant_types_supported": ["authorization_code", "implicit"],
+        "code_challenge_methods_supported": ["S256"],
+        "scopes_supported": [],
+    }
+    default_capabilities = {
+        "client_authn_method": ["request_param", "public"],
+    }
 
-        logger.info("client_setup: iss_id={}, user={}".format(iss_id, user))
+    def __init__(self, upstream_get, **kwargs):
+        Endpoint.__init__(self, upstream_get, **kwargs)
+        self.post_parse_request.append(self._do_request_uri)
+        self.post_parse_request.append(self._post_parse_request)
+        self.allowed_request_algorithms = AllowedAlgorithms(ALG_PARAMS)
+        self.resource_indicators_config = kwargs.get("resource_indicators", None)
+
+    def filter_request(self, context, req):
+        return req
+
+    def extra_response_args(self, aresp):
+        return aresp
+
+    def authentication_error_response(self, request, error, error_description, **kwargs):
+        _error_msg = self.error_cls(error=error, error_description=error_description)
+        _state = request.get("state")
+        if _state:
+            _error_msg["state"] = _state
+        return _error_msg
+
+    def verify_response_type(self, request: Union[Message, dict], cinfo: dict) -> bool:
+        # Checking response types
+        _registered = [set(rt.split(" ")) for rt in cinfo.get("response_types_supported", [])]
+        if not _registered:
+            # If no response_type is registered by the client then we'll use code.
+            _registered = [{"code"}]
+
+        # Is the asked for response_type among those that are permitted
+        return set(request["response_type"]) in _registered
+
+    def mint_token(self, token_class, grant, session_id, based_on=None, **kwargs):
+        usage_rules = grant.usage_rules.get(token_class, {})
+        token = grant.mint_token(
+            session_id=session_id,
+            context=self.upstream_get("context"),
+            token_class=token_class,
+            based_on=based_on,
+            usage_rules=usage_rules,
+            **kwargs,
+        )
 
-        if not iss_id:
-            if not user:
-                raise ValueError("Need issuer or user")
+        _exp_in = usage_rules.get("expires_in")
+        if isinstance(_exp_in, str):
+            _exp_in = int(_exp_in)
+        if _exp_in:
+            token.expires_at = utc_time_sans_frac() + _exp_in
+
+        _mngr = self.upstream_get("context").session_manager
+        _mngr.set(_mngr.unpack_session_key(session_id), grant)
+
+        return token
+
+    def _do_request_uri(self, request, client_id, context, **kwargs):
+        _request_uri = request.get("request_uri")
+        if _request_uri:
+            # Do I do pushed authorization requests ?
+            _endp = self.upstream_get("endpoint", "pushed_authorization")
+            if _endp:
+                # Is it a UUID urn
+                if _request_uri.startswith("urn:uuid:"):
+                    _req = context.par_db.get(_request_uri)
+                    if _req:
+                        # One time usage
+                        del context.par_db[_request_uri]
+                        return _req
+                    else:
+                        raise ValueError("Got a request_uri I can not resolve")
 
-            logger.debug("Connecting to previously unknown OP")
-            temporary_client = self.do_webfinger(user)
-        else:
-            temporary_client = None
+            # Do I support request_uri ?
+            if context.provider_info.get("request_uri_parameter_supported", True) is False:
+                raise ServiceError("Someone is using request_uri which I'm not supporting")
+
+            _registered = context.cdb[client_id].get("request_uris")
+            # Not registered should be handled else where
+            if _registered:
+                # Before matching remove a possible fragment
+                _p = _request_uri.split("#")
+                # ignore registered fragments for now.
+                if _p[0] not in [base for base, qp in _registered]:
+                    raise ValueError("A request_uri outside the registered")
+
+            # Fetch the request
+            _resp = context.httpc("GET", _request_uri, **context.httpc_params)
+            if _resp.status_code == 200:
+                args = {"keyjar": self.upstream_get("attribute", "keyjar"), "issuer": client_id}
+                _ver_request = self.request_cls().from_jwt(_resp.text, **args)
+                self.allowed_request_algorithms(
+                    client_id,
+                    context,
+                    _ver_request.jws_header.get("alg", "RS256"),
+                    "sign",
+                )
+                if _ver_request.jwe_header is not None:
+                    self.allowed_request_algorithms(
+                        client_id,
+                        context,
+                        _ver_request.jws_header.get("alg"),
+                        "enc_alg",
+                    )
+                    self.allowed_request_algorithms(
+                        client_id,
+                        context,
+                        _ver_request.jws_header.get("enc"),
+                        "enc_enc",
+                    )
+                # The protected info overwrites the non-protected
+                for k, v in _ver_request.items():
+                    request[k] = v
 
-        try:
-            client = self.issuer2rp[iss_id]
-        except KeyError:
-            if temporary_client:
-                client = temporary_client
+                request[verified_claim_name("request")] = _ver_request
             else:
-                logger.debug("Creating new client: %s", iss_id)
-                client = self.init_client(iss_id)
-        else:
-            return client
-
-        logger.debug("Get provider info")
-        issuer = self.do_provider_info(client, behaviour_args=behaviour_args)
-
-        logger.debug("Do client registration")
-        self.do_client_registration(client, iss_id, behaviour_args=behaviour_args)
+                raise ServiceError("Got a %s response", _resp.status)
 
-        self.issuer2rp[issuer] = client
-        return client
+        return request
 
-    def _get_response_type(self, context, req_args: Optional[dict] = None):
-        if req_args:
-            return req_args.get("response_type",
-                                context.claims.get_usage("response_types")[0])
-        else:
-            return context.claims.get_usage("response_types")[0]
-
-    def init_authorization(
-            self,
-            client: Optional[Client] = None,
-            state: Optional[str] = "",
-            req_args: Optional[dict] = None,
-            behaviour_args: Optional[dict] = None,
-    ) -> dict:
+    def _post_parse_request(self, request, client_id, context, **kwargs):
         """
-        Constructs the URL that will redirect the user to the authorization
-        endpoint of the OP/AS.
+        Verify the authorization request.
 
-        :param behaviour_args:
-        :param state:
-        :param client: A Client instance
-        :param req_args: Non-default Request arguments
-        :return: A dictionary with 2 keys: **url** The authorization redirect
-            URL and **state** the key to the session information in the
-            state data store.
+        :param context:
+        :param request:
+        :param client_id:
+        :param kwargs:
+        :return:
         """
+        if not request:
+            logger.debug("No AuthzRequest")
+            return self.authentication_error_response(
+                request, error="invalid_request", error_description="Can not parse AuthzRequest"
+            )
 
-        logger.debug(20 * "*" + " init_authorization " + 20 * "*")
-        if not client:
-            if state:
-                client = self.get_client_from_session_key(state)
-            else:
-                raise ValueError("Missing state/session key")
-
-        _context = client.get_context()
-        # _entity = client.upstream_get("entity")
-        _nonce = rndstr(24)
-        _response_type = self._get_response_type(_context, req_args)
-        request_args = {
-            "redirect_uri": pick_redirect_uri(
-                _context, request_args=req_args, response_type=_response_type
-            ),
-            "response_type": _response_type,
-            "nonce": _nonce,
-        }
-
-        _scope = _context.claims.get_usage("scope")
-        if _scope:
-            request_args['scope'] = _scope
-
-        _req_args = _context.config.get("request_args")
-        if _req_args:
-            if "claims" in _req_args:
-                _req_args["claims"] = Claims(**_req_args["claims"])
-            request_args.update(_req_args)
-
-        if req_args is not None:
-            request_args.update(req_args)
-
-        # Need a new state for a new authorization request
-        _current = _context.cstate
-        _state = _current.create_key()
-        request_args["state"] = _state
-        _current.bind_key(_nonce, _state)
-        _current.set(_state, {'iss': _context.get("issuer")})
-
-        logger.debug("Authorization request args: {}".format(request_args))
-
-        # if behaviour_args and "request_param" not in behaviour_args:
-        #     _pi = _context.get("provider_info")
-
-        _srv = client.get_service("authorization")
-        _info = _srv.get_request_parameters(
-            request_args=request_args, behaviour_args=behaviour_args
-        )
-        logger.debug("Authorization info: {}".format(_info))
-        return {"url": _info["url"], "state": _state}
+        request = self.filter_request(context, request)
 
-    def begin(self, issuer_id="", user_id="", req_args=None, behaviour_args=None):
-        """
-        This is the first of the 3 high level methods that most users of this
-        library should confine them self to use.
-        If will use client_setup to produce a Client instance ready to be used
-        against the OP/AS the user wants to use.
-        Once it has the client it will construct an Authorization
-        request.
-
-        :param behaviour_args:
-        :param req_args:
-        :param issuer_id: Issuer ID
-        :param user_id: A user identifier
-        :return: A dictionary containing **url** the URL that will redirect the
-            user to the OP/AS and **state** the session key which will
-            allow higher level code to access session information.
-        """
+        _cinfo = context.cdb.get(client_id)
+        if not _cinfo:
+            logger.error("Client ID ({}) not in client database".format(request["client_id"]))
+            return self.authentication_error_response(
+                request, error="unauthorized_client", error_description="unknown client"
+            )
 
-        # Get the client instance that has been assigned to this issuer
-        client = self.client_setup(issuer_id, user_id, behaviour_args=behaviour_args)
+        # Is the asked for response_type among those that are permitted
+        if not self.verify_response_type(request, _cinfo):
+            return self.authentication_error_response(
+                request,
+                error="invalid_request",
+                error_description="Trying to use unregistered response_type",
+            )
 
+        # Get a verified redirect URI
         try:
-            res = self.init_authorization(client, req_args=req_args, behaviour_args=behaviour_args)
-        except Exception:
-            message = traceback.format_exception(*sys.exc_info())
-            logger.error(message)
-            raise
+            redirect_uri = get_uri(context, request, "redirect_uri")
+        except (RedirectURIError, ParameterError) as err:
+            return self.authentication_error_response(
+                request,
+                error="invalid_request",
+                error_description="{}:{}".format(err.__class__.__name__, err),
+            )
         else:
-            return res
+            request["redirect_uri"] = redirect_uri
 
-    # ----------------------------------------------------------------------
+        if (
+            "resource_indicators" in _cinfo
+            and "authorization_code" in _cinfo["resource_indicators"]
+        ):
+            resource_indicators_config = _cinfo["resource_indicators"]["authorization_code"]
+        else:
+            resource_indicators_config = self.resource_indicators_config
 
-    def get_client_from_session_key(self, state):
-        return self.issuer2rp[self.state2issuer(state)]
+        if resource_indicators_config is not None:
+            if "policy" not in resource_indicators_config:
+                policy = {"policy": {"function": validate_resource_indicators_policy}}
+                resource_indicators_config.update(policy)
+            request = self._enforce_resource_indicators_policy(request, resource_indicators_config)
 
-    @staticmethod
-    def get_response_type(client):
-        """
-        Return the response_type a specific client wants to use.
+        return request
 
-        :param client: A Client instance
-        :return: The response_type
-        """
-        return client.service_context.claims.get_usage("response_types")[0]
+    def _enforce_resource_indicators_policy(self, request, config):
+        _context = self.upstream_get("context")
 
-    @staticmethod
-    def get_client_authn_method(client, endpoint):
-        """
-        Return the client authentication method a client wants to use a
-        specific endpoint
+        policy = config["policy"]
+        function = policy["function"]
+        kwargs = policy.get("kwargs", {})
 
-        :param client: A Client instance
-        :param endpoint: The endpoint at which the client has to authenticate
-        :return: The client authentication method
-        """
-        if endpoint == "token_endpoint":
-            am = client.get_context().get_usage("token_endpoint_auth_method")
-            if not am:
-                return ""
-            else:
-                if isinstance(am, str):
-                    return am
-                else:  # a list
-                    return am[0]
+        if kwargs.get("resource_servers_per_client", None) is None:
+            kwargs["resource_servers_per_client"] = {request["client_id"]: request["client_id"]}
 
-    def get_tokens(self, state, client: Optional[Client] = None):
-        """
-        Use the 'accesstoken' service to get an access token from the OP/AS.
-
-        :param state: The state key (the state parameter in the
-            authorization request)
-        :param client: A Client instance
-        :return: A :py:class:`idpyoidc.message.oidc.AccessTokenResponse` or
-            :py:class:`idpyoidc.message.oauth2.AuthorizationResponse`
-        """
-        logger.debug(20 * "*" + " get_tokens " + 20 * "*")
-
-        if client is None:
-            client = self.get_client_from_session_key(state)
+        if isinstance(function, str):
+            try:
+                fn = importer(function)
+            except Exception:
+                raise ImproperlyConfigured(f"Error importing {function} policy function")
+        else:
+            fn = function
+        try:
+            return fn(request, context=_context, **kwargs)
+        except Exception as e:
+            logger.error(f"Error while executing the {fn} policy function: {e}")
+            return self.error_cls(error="server_error", error_description="Internal server error")
+
+    def pick_authn_method(self, request, redirect_uri, acr=None, **kwargs):
+        _context = self.upstream_get("context")
+        auth_id = kwargs.get("auth_method_id")
+        if auth_id:
+            return _context.authn_broker[auth_id]
+
+        res = None
+        if acr:
+            res = _context.authn_broker.pick(acr)
+        else:
+            try:
+                res = pick_auth(_context, request)
+            except Exception as exc:
+                logger.exception(f"An error occurred while picking the authN broker: {exc}")
+        if res:
+            return res
+        else:
+            return {
+                "error": "access_denied",
+                "error_description": "ACR I do not support",
+                "return_uri": redirect_uri,
+                "return_type": request["response_type"],
+            }
 
-        _context = client.get_context()
-        _claims = _context.cstate.get_set(state, claim=['code', 'redirect_uri'])
+    def create_session(self, request, user_id, acr, time_stamp, authn_method):
+        _context = self.upstream_get("context")
+        _mngr = _context.session_manager
+        authn_event = create_authn_event(
+            user_id,
+            authn_info=acr,
+            time_stamp=time_stamp,
+        )
+        _exp_in = authn_method.kwargs.get("expires_in")
+        if _exp_in and "valid_until" in authn_event:
+            authn_event["valid_until"] = utc_time_sans_frac() + _exp_in
+
+        _token_usage_rules = _context.authz.usage_rules(request["client_id"])
+        return _mngr.create_session(
+            authn_event=authn_event,
+            auth_req=request,
+            user_id=user_id,
+            client_id=request["client_id"],
+            token_usage_rules=_token_usage_rules,
+        )
 
-        req_args = {
-            "code": _claims["code"],
-            "state": state,
-            "redirect_uri": _claims["redirect_uri"],
-            "grant_type": "authorization_code",
-            "client_id": client.get_client_id(),
-            "client_secret": _context.get("client_secret"),
+    def _login_required_error(self, redirect_uri, request):
+        _res = {
+            "error": "login_required",
+            "return_uri": redirect_uri,
+            "return_type": request["response_type"],
         }
-        logger.debug("request_args: {}".format(req_args))
-        try:
-            tokenresp = client.do_request(
-                "accesstoken",
-                request_args=req_args,
-                authn_method=self.get_client_authn_method(client, "token_endpoint"),
-                state=state,
-            )
-        except Exception:
-            message = traceback.format_exception(*sys.exc_info())
-            logger.error(message)
-            raise
+        _state = request.get("state")
+        if _state:
+            _res["state"] = _state
+        logger.debug("Login required error: {}".format(_res))
+        return _res
+
+    def _unwrap_identity(self, identity):
+        # identity is a dict or a json object
+        # the value of 'uid' in the dictionary might be a base64 encoded (b64e) json object
+        if isinstance(identity, dict):
+            _uid = as_unicode(identity["uid"])
+            try:
+                _id = b64d(as_bytes(_uid))
+            except Exception:
+                return identity
         else:
-            if is_error_message(tokenresp):
-                raise OidcServiceError(tokenresp["error"])
-
-        return tokenresp
+            try:
+                _id = b64d(as_bytes(identity))
+            except Exception:
+                return identity
 
-    def refresh_access_token(self, state, client=None, scope=""):
+        try:
+            return json.loads(as_unicode(_id))
+        except UnicodeDecodeError:
+            return identity
+
+    def setup_auth(
+        self,
+        request: Optional[Union[Message, dict]],
+        redirect_uri: str,
+        cinfo: dict,
+        cookie: List[dict] = None,
+        acr: str = None,
+        **kwargs,
+    ) -> dict:
         """
-        Refresh an access token using a refresh_token. When asking for a new
-        access token the RP can ask for another scope for the new token.
 
-        :param client: A Client instance
-        :param state: The state key (the state parameter in the
-            authorization request)
-        :param scope: What the returned token should be valid for.
-        :return: A :py:class:`idpyoidc.message.oidc.AccessTokenResponse` instance
+        :param request: The authorization/authentication request
+        :param redirect_uri:
+        :param cinfo: client info
+        :param cookie: List of cookies
+        :param acr: Default ACR, if nothing else is specified
+        :param kwargs:
+        :return:
         """
 
-        logger.debug(20 * "*" + " refresh_access_token " + 20 * "*")
-
-        if scope:
-            req_args = {"scope": scope}
-        else:
-            req_args = {}
+        res = self.pick_authn_method(request, redirect_uri, acr, **kwargs)
 
-        if client is None:
-            client = self.get_client_from_session_key(state)
+        authn = res["method"]
+        authn_class_ref = res["acr"]
 
+        client_id = request.get("client_id")
+        _context = self.upstream_get("context")
         try:
-            tokenresp = client.do_request(
-                "refresh_token",
-                authn_method=self.get_client_authn_method(client, "token_endpoint"),
-                state=state,
-                request_args=req_args,
+            _auth_info = kwargs.get("authn", "")
+            if "upm_answer" in request and request["upm_answer"] == "true":
+                _max_age = 0
+            else:
+                _max_age = max_age(request)
+            logger.debug(f"Max age: {_max_age}")
+            identity, _ts = authn.authenticated_as(
+                client_id, cookie, authorization=_auth_info, max_age=_max_age
             )
-        except Exception:
-            message = traceback.format_exception(*sys.exc_info())
-            logger.error(message)
-            raise
+        except (NoSuchAuthentication, TamperAllert):
+            identity = None
+            _ts = 0
+        except ToOld:
+            logger.info("Too old authentication")
+            identity = None
+            _ts = 0
+        except UnknownToken:
+            logger.info("Unknown Token")
+            identity = None
+            _ts = 0
+        else:
+            if identity:
+                identity = self._unwrap_identity(identity)
+                _sid = identity.get("sid")
+                if _sid:
+                    try:
+                        _csi = _context.session_manager[_sid]
+                    except Revoked:
+                        logger.debug("Authentication session revoked!!")
+                        identity = None
+                    else:
+                        logger.debug(f"Session info type: {_csi.__class__.__name__}")
+                        if _csi.is_active() is False:
+                            identity = None
+
+        _mngr = _context.session_manager
+        _session_id = ""
+
+        # To authenticate or Not
+        if not identity:  # No!
+            logger.info("No active authentication")
+            # logger.debug("Known clients: {}".format(list(_context.cdb.keys())))
+
+            if "prompt" in request and "none" in request["prompt"]:
+                # Need to authenticate but not allowed
+                return self._login_required_error(redirect_uri, request)
+            else:
+                authn_args = authn_args_gather(request, authn_class_ref, cinfo, **kwargs)
+                return {"function": authn, "args": authn_args}
         else:
-            if is_error_message(tokenresp):
-                raise OidcServiceError(tokenresp["error"])
-
-        return tokenresp
-
-    def get_user_info(self, state, client=None, access_token="", **kwargs):
-        """
-        use the access token previously acquired to get some userinfo
-
-        :param client: A Client instance
-        :param state: The state value, this is the key into the session
-            data store
-        :param access_token: An access token
-        :param kwargs: Extra keyword arguments
-        :return: A :py:class:`idpyoidc.message.oidc.OpenIDSchema` instance
-        """
+            authn_args = authn_args_gather(request, authn_class_ref, cinfo, **kwargs)
+            logger.info(f"Active authentication: {identity}")
+            if re_authenticate(request, authn):
+                # demand re-authentication
+                return {"function": authn, "args": authn_args}
+            else:
+                # I got back a dictionary
+                user = identity["uid"]
+                if "req_user" in kwargs:
+                    if user != kwargs["req_user"]:
+                        logger.debug("Wanted to be someone else!")
+                        if "prompt" in request and "none" in request["prompt"]:
+                            return self._login_required_error(redirect_uri, request)
+                        else:
+                            return {"function": authn, "args": authn_args}
+
+                if "sid" in identity:
+                    _session_id = identity["sid"]
+
+                    # make sure the client is the same
+                    _uid, _cid, _gid = _mngr.decrypt_session_id(_session_id)
+                    if request["client_id"] != _cid:
+                        return {"function": authn, "args": authn_args}
+
+                    grant = _mngr[_session_id]
+                    if grant.is_active() is False:
+                        return {"function": authn, "args": authn_args}
+                    elif request != grant.authorization_request:
+                        authn_event = _mngr.get_authentication_event(session_id=_session_id)
+                        if authn_event.is_valid() is False:  # if not valid, do new login
+                            return {"function": authn, "args": authn_args}
+
+                        # create new grant
+                        _session_id = _mngr.create_grant(
+                            authn_event=authn_event,
+                            auth_req=request,
+                            user_id=user,
+                            client_id=request["client_id"],
+                        )
+
+        if _session_id:
+            authn_event = _mngr.get_authentication_event(session_id=_session_id)
+            if authn_event.is_valid() is False:  # if not valid, do new login
+                return {"function": authn, "args": authn_args}
+        else:
+            _session_id = self.create_session(request, identity["uid"], authn_class_ref, _ts, authn)
+
+        return {"session_id": _session_id, "identity": identity, "user": user}
+
+    def aresp_check(self, aresp, request):
+        return ""
+
+    def response_mode(
+        self,
+        request: Union[dict, AuthorizationRequest],
+        response_args: Optional[Union[dict, AuthorizationResponse]] = None,
+        return_uri: Optional[str] = "",
+        fragment_enc: Optional[bool] = None,
+        **kwargs,
+    ) -> dict:
+        resp_mode = request["response_mode"]
+        if resp_mode == "form_post":
+            if isinstance(response_args, AuthorizationRequest):
+                _args = response_args.to_dict()
+            else:
+                _args = response_args
 
-        logger.debug(20 * "*" + " get_user_info " + 20 * "*")
+            if "error" in _args:
+                if not return_uri:
+                    return_uri = _args["return_uri"]
+                    del _args["return_uri"]
+                if "return_type" in _args:
+                    del _args["return_type"]
+
+            msg = FORM_POST.format(inputs=inputs(_args), action=return_uri)
+            kwargs.update(
+                {
+                    "response_msg": msg,
+                    "content_type": "text/html",
+                    "response_placement": "body",
+                }
+            )
+        elif resp_mode == "fragment":
+            if fragment_enc is False:
+                # Can't be done
+                raise InvalidRequest("wrong response_mode")
+            else:
+                kwargs["fragment_enc"] = True
+        elif resp_mode == "query":
+            if fragment_enc is True:
+                # Can't be done
+                raise InvalidRequest("wrong response_mode")
+        else:
+            raise InvalidRequest("Unknown response_mode")
+
+        if resp_mode in ["fragment", "query"]:
+            kwargs.update({"response_args": response_args, "return_uri": return_uri})
+
+        return kwargs
+
+    def error_response(self, response_info, request, error, error_description):
+        resp = self.authentication_error_response(
+            request, error=error, error_description=str(error_description)
+        )
+        response_info["response_args"] = resp
+        return response_info
 
-        if client is None:
-            client = self.get_client_from_session_key(state)
+    def error_by_response_mode(self, response_info, request, error, error_description):
+        response_info = self.error_response(response_info, request, error, error_description)
+        if "return_uri" not in response_info:
+            response_info["return_uri"] = request["redirect_uri"]
+        response_info = self.response_mode(request, **response_info)
+        return response_info
+
+    def create_authn_response(self, request: Union[dict, Message], sid: str) -> dict:
+        """
+        :param request:
+        :param sid:
+        :return:
+        """
+        # create the response
+        aresp = self.response_cls()
+        if request.get("state"):
+            aresp["state"] = request["state"]
+
+        if "response_type" in request and request["response_type"] == ["none"]:
+            fragment_enc = False
+        else:
+            _context = self.upstream_get("context")
+            _mngr = _context.session_manager
+            _sinfo = _mngr.get_session_info(sid, grant=True)
+
+            scope = []
+            resource_scopes = []
+            if request.get("scope"):
+                scope = request.get("scope")
+            if request.get("resource"):
+                resource_scopes = [
+                    _context.cdb[s]["scope"]
+                    for s in request.get("resource")
+                    if s in _context.cdb.keys() and _context.cdb[s].get("scope")
+                ]
+                resource_scopes = [item for sublist in resource_scopes for item in sublist]
 
-        if not access_token:
-            _arg = client.get_context().cstate.get_set(state, claim=["access_token"])
-            access_token = _arg["access_token"]
+            aresp["scope"] = _context.scopes_handler.filter_scopes(
+                list(set(scope + resource_scopes)), _sinfo["client_id"]
+            )
 
-        request_args = {"access_token": access_token}
+            rtype = set(request["response_type"][:])
+            handled_response_type = []
 
-        resp = client.do_request("userinfo", state=state, request_args=request_args, **kwargs)
-        if is_error_message(resp):
-            raise OidcServiceError(resp["error"])
+            fragment_enc = True
+            if len(rtype) == 1 and "code" in rtype:
+                fragment_enc = False
+
+            grant = _sinfo["grant"]
+
+            if "code" in rtype:
+                _code = self.mint_token(
+                    token_class="authorization_code",
+                    grant=grant,
+                    session_id=_sinfo["branch_id"],
+                )
+                aresp["code"] = _code.value
+                handled_response_type.append("code")
+            else:
+                _code = None
 
-        return resp
+            if "token" in rtype:
+                _access_token = self.mint_token(
+                    token_class="access_token",
+                    grant=grant,
+                    session_id=_sinfo["branch_id"],
+                )
+                aresp["access_token"] = _access_token.value
+                aresp["token_type"] = "Bearer"
+                if _access_token.expires_at:
+                    aresp["expires_in"] = _access_token.expires_at - utc_time_sans_frac()
+                handled_response_type.append("token")
+            else:
+                _access_token = None
 
-    @staticmethod
-    def userinfo_in_id_token(id_token):
-        """
-        Given an verified ID token return all the claims that may been user
-        information.
+            if "id_token" in rtype:
+                kwargs = {}
+                if {"code", "id_token", "token"}.issubset(rtype):
+                    kwargs = {"code": _code.value, "access_token": _access_token.value}
+                elif {"code", "id_token"}.issubset(rtype):
+                    kwargs = {"code": _code.value}
+                elif {"id_token", "token"}.issubset(rtype):
+                    kwargs = {"access_token": _access_token.value}
+
+                if rtype == {"id_token"}:
+                    kwargs["as_if"] = "userinfo"
+
+                try:
+                    id_token = self.mint_token(
+                        token_class="id_token",
+                        grant=grant,
+                        session_id=_sinfo["branch_id"],
+                        scope=request["scope"],
+                        **kwargs,
+                    )
+                    # id_token = _context.idtoken.make(sid, **kwargs)
+                except (JWEException, NoSuitableSigningKeys) as err:
+                    logger.warning(str(err))
+                    resp = self.authentication_error_response(
+                        request,
+                        error="invalid_request",
+                        error_description="Could not sign/encrypt id_token",
+                    )
+                    return {"response_args": resp, "fragment_enc": fragment_enc}
+
+                aresp["id_token"] = id_token.value
+                handled_response_type.append("id_token")
+
+            not_handled = rtype.difference(handled_response_type)
+            if not_handled:
+                resp = self.authentication_error_response(
+                    request,
+                    error="invalid_request",
+                    error_description="unsupported_response_type",
+                )
+                return {"response_args": resp, "fragment_enc": fragment_enc}
+
+        aresp = self.extra_response_args(aresp)
+
+        return {"response_args": aresp, "fragment_enc": fragment_enc}
+
+    def post_authentication(self, request: Union[dict, Message], session_id: str, **kwargs) -> dict:
+        """
+        Things that are done after a successful authentication.
+
+        :param request: The authorization request
+        :param session_id: Session identifier
+        :param kwargs:
+        :return: A dictionary with 'response_args'
+        """
+
+        response_info = {}
+        _context = self.upstream_get("context")
+        _mngr = _context.session_manager
+
+        # Do the authorization
+
+        grant = _context.authz(session_id, request=request)
+        if grant.is_active() is False:
+            return self.error_response(response_info, request, "server_error", "Grant not usable")
 
-        :param id_token: An :py:class:`idpyoidc.message.oidc.IDToken` instance
-        :return: A dictionary with user information
-        """
-        res = dict([(k, id_token[k]) for k in OpenIDSchema.c_param.keys() if k in id_token])
-        res.update(id_token.extra())
-        return res
+        user_id, client_id, grant_id = _mngr.decrypt_session_id(session_id)
+        try:
+            _mngr.set([user_id, client_id, grant_id], grant)
+        except Exception as err:
+            return self.error_response(
+                response_info, request, "server_error", "{}".format(err.args)
+            )
 
-    def finalize_auth(
-            self, client, issuer: str, response: dict, behaviour_args: Optional[dict] = None
-    ):
-        """
-        Given the response returned to the redirect_uri, parse and verify it.
+        logger.debug("response type: %s" % request["response_type"])
 
-        :param behaviour_args: For fine tuning behaviour
-        :param client: A Client instance
-        :param issuer: An Issuer ID
-        :param response: The authorization response as a dictionary
-        :return: An :py:class:`idpyoidc.message.oidc.AuthorizationResponse` or
-            :py:class:`idpyoidc.message.oauth2.AuthorizationResponse` instance.
-        """
+        response_info = self.create_authn_response(request, session_id)
+        response_info["session_id"] = session_id
 
-        logger.debug(20 * "*" + " finalize_auth " + 20 * "*")
+        logger.debug("Known clients: {}".format(list(_context.cdb.keys())))
 
-        _srv = client.get_service("authorization")
         try:
-            authorization_response = _srv.parse_response(
-                response, sformat="dict", behaviour_args=behaviour_args
+            redirect_uri = get_uri(_context, request, "redirect_uri")
+        except (RedirectURIError, ParameterError) as err:
+            return self.error_response(
+                response_info, request, "invalid_request", "{}".format(err.args)
             )
-        except Exception as err:
-            logger.error("Parsing authorization_response: {}".format(err))
-            message = traceback.format_exception(*sys.exc_info())
-            logger.error(message)
-            raise
         else:
-            logger.debug("Authz response: {}".format(authorization_response.to_dict()))
-
-        if is_error_message(authorization_response):
-            return authorization_response
+            response_info["return_uri"] = redirect_uri
 
-        _context = client.get_context()
-        try:
-            _iss = _context.cstate.get_set(
-                authorization_response["state"], claim=['iss']).get('iss')
-        except KeyError:
-            raise KeyError("Unknown state value")
-
-        if _iss != issuer:
-            logger.error("Issuer problem: {} != {}".format(_iss, issuer))
-            # got it from the wrong bloke
-            raise ValueError("Impersonator {}".format(issuer))
-
-        _srv.update_service_context(authorization_response, key=authorization_response["state"])
-        return authorization_response
-
-    def get_access_and_id_token(
-            self,
-            authorization_response=None,
-            state: Optional[str] = "",
-            client: Optional[object] = None,
-            behaviour_args: Optional[dict] = None,
-    ):
-        """
-        There are a number of services where access tokens and ID tokens can
-        occur in the response. This method goes through the possible places
-        based on the response_type the client uses.
-
-        :param behaviour_args: For fine tuning behaviour
-        :param authorization_response: The Authorization response
-        :param state: The state key (the state parameter in the
-            authorization request)
-        :return: A dictionary with 2 keys: **access_token** with the access
-            token as value and **id_token** with a verified ID Token if one
-            was returned otherwise None.
-        """
+        # Now about the response_mode. Should not be set if it's obvious
+        # from the response_type. Knows about 'query', 'fragment' and
+        # 'form_post'.
 
-        logger.debug(20 * "*" + " get_access_and_id_token " + 20 * "*")
-
-        if client is None:
-            client = self.get_client_from_session_key(state)
-
-        _context = client.get_context()
+        if "response_mode" in request:
+            try:
+                response_info = self.response_mode(request, **response_info)
+            except InvalidRequest as err:
+                return self.error_response(
+                    response_info, request, "invalid_request", "{}".format(err.args)
+                )
+
+        _cookie_info = _context.new_cookie(
+            name=_context.cookie_handler.name["session"],
+            sid=session_id,
+            state=request.get("state"),
+        )
 
-        resp_attr = authorization_response or _context.cstate.get_set(state,
-                                                                      message=AuthorizationResponse)
-        if resp_attr is None:
-            raise ValueError("One of authorization_response or state must be provided")
-
-        if not state:
-            state = authorization_response["state"]
-
-        _req_attr = _context.cstate.get_set(state, AuthorizationRequest)
-        _resp_type = set(_req_attr["response_type"].split(' '))
-
-        access_token = None
-        id_token = None
-        if _resp_type in [{"id_token"}, {"id_token", "token"}, {"code", "id_token", "token"}]:
-            id_token = authorization_response["__verified_id_token"]
-
-        if _resp_type in [
-            {"token"},
-            {"id_token", "token"},
-            {"code", "token"},
-            {"code", "id_token", "token"},
-        ]:
-            access_token = authorization_response["access_token"]
-            if behaviour_args:
-                if behaviour_args.get("collect_tokens", False):
-                    # get what you can from the token endpoint
-                    token_resp = self.get_tokens(state, client=client)
-                    if is_error_message(token_resp):
-                        return False, "Invalid response %s." % token_resp["error"]
-                    # Now which access_token should I use
-                    access_token = token_resp["access_token"]
-                    # May or may not get an ID Token
-                    id_token = token_resp.get("__verified_id_token")
-
-        elif _resp_type in [{"code"}, {"code", "id_token"}]:
-            # get the access token
-            token_resp = self.get_tokens(state, client=client)
-            if is_error_message(token_resp):
-                return False, "Invalid response %s." % token_resp["error"]
-
-            access_token = token_resp["access_token"]
-            # May or may not get an ID Token
-            id_token = token_resp.get("__verified_id_token")
+        response_info["cookie"] = [_cookie_info]
 
-        return {"access_token": access_token, "id_token": id_token}
+        return response_info
 
-    # noinspection PyUnusedLocal
-    def finalize(self, issuer, response, behaviour_args: Optional[dict] = None):
-        """
-        The third of the high level methods that a user of this Class should
-        know about.
-        Once the consumer has redirected the user back to the
-        callback URL there might be a number of services that the client should
-        use. Which one those are defined by the client configuration.
-
-        :param behaviour_args: For finetuning
-        :param issuer: Who sent the response
-        :param response: The Authorization response as a dictionary
-        :returns: A dictionary with two claims:
-            **state** The key under which the session information is
-            stored in the data store and
-            **error** and encountered error or
-            **userinfo** The collected user information
+    def authz_part2(self, request, session_id, **kwargs):
         """
+        After the authentication this is where you should end up
 
-        client = self.issuer2rp[issuer]
+        :param request: The Authorization Request
+        :param session_id: Session identifier
+        :param kwargs: possible other parameters
+        :return: A redirect to the redirect_uri of the client
+        """
+        try:
+            resp_info = self.post_authentication(request, session_id, **kwargs)
+        except Exception as err:
+            return self.error_by_response_mode({}, request, "server_error", err)
 
-        if behaviour_args:
-            logger.debug(f"Finalize behaviour args: {behaviour_args}")
+        _context = self.upstream_get("context")
 
-        authorization_response = self.finalize_auth(client, issuer, response)
-        if is_error_message(authorization_response):
-            return {
-                "state": authorization_response["state"],
-                "error": authorization_response["error"],
-            }
+        logger.debug(f"resp_info: {resp_info}")
 
-        _state = authorization_response["state"]
-        token = self.get_access_and_id_token(
-            authorization_response, state=_state, client=client, behaviour_args=behaviour_args
-        )
-        _id_token = token.get("id_token")
-        logger.debug(f"ID Token: {_id_token}")
-
-        if client.get_service("userinfo") and token["access_token"]:
-            inforesp = self.get_user_info(
-                state=authorization_response["state"],
-                client=client,
-                access_token=token["access_token"],
+        if "check_session_iframe" in _context.provider_info:
+            salt = rndstr()
+            try:
+                authn_event = _context.session_manager.get_authentication_event(session_id)
+            except KeyError:
+                return self.error_by_response_mode({}, request, "server_error", "No such session")
+            else:
+                if authn_event.is_valid() is False:
+                    return self.error_by_response_mode(
+                        {}, request, "server_error", "Authentication has timed out"
+                    )
+
+            _state = b64e(as_bytes(json.dumps({"authn_time": authn_event["authn_time"]})))
+
+            _session_cookie_content = _context.new_cookie(
+                name=_context.cookie_handler.name["session_management"],
+                state=as_unicode(_state),
             )
 
-            if isinstance(inforesp, ResponseMessage) and "error" in inforesp:
-                return {"error": "Invalid response %s." % inforesp["error"], "state": _state}
-
-        elif _id_token:  # look for it in the ID Token
-            inforesp = self.userinfo_in_id_token(_id_token)
-        else:
-            inforesp = {}
-
-        logger.debug("UserInfo: %s", inforesp)
+            opbs_value = _session_cookie_content["value"]
 
-        _context = client.get_context()
-        try:
-            _sid_support = _context.get("provider_info")["backchannel_logout_session_required"]
-        except KeyError:
-            try:
-                _sid_support = _context.get("provider_info")[
-                    "frontchannel_logout_session_required"
-                ]
-            except Exception:
-                _sid_support = False
-
-        if _sid_support and _id_token:
-            try:
-                sid = _id_token["sid"]
-            except KeyError:
-                pass
+            if "return_uri" in resp_info:
+                re_uri = resp_info["return_uri"]
             else:
-                _context.cstate.bind_key(sid, _state)
+                re_uri = request["redirect_uri"]
 
-        if _id_token:
-            _context.cstate.bind_key(_id_token["sub"], _state)
-        else:
-            _context.cstate.bind_key(inforesp["sub"], _state)
+            logger.debug(
+                "compute_session_state: client_id=%s, origin=%s, opbs=%s, salt=%s",
+                request["client_id"],
+                re_uri,
+                opbs_value,
+                salt,
+            )
 
-        return {
-            "userinfo": inforesp,
-            "state": authorization_response["state"],
-            "token": token["access_token"],
-            "id_token": _id_token,
-            "session_state": authorization_response.get("session_state", ""),
-        }
+            _session_state = compute_session_state(opbs_value, salt, request["client_id"], re_uri)
 
-    def has_active_authentication(self, state):
-        """
-        Find out if the user has an active authentication
+            if _session_cookie_content:
+                if "cookie" in resp_info:
+                    resp_info["cookie"].append(_session_cookie_content)
+                else:
+                    resp_info["cookie"] = [_session_cookie_content]
+
+            if "response_args" in resp_info:
+                resp_info["response_args"]["session_state"] = _session_state
+
+        # Mix-Up mitigation
+        if "response_args" in resp_info:
+            resp_info["response_args"]["iss"] = _context.issuer
+            resp_info["response_args"]["client_id"] = request["client_id"]
+
+        return resp_info
+
+    def do_request_user(self, request_info, **kwargs):
+        return kwargs
+
+    def process_request(
+        self,
+        request: Optional[Union[Message, dict]] = None,
+        http_info: Optional[dict] = None,
+        **kwargs,
+    ):
+        """The AuthorizationRequest endpoint
 
-        :param state:
-        :return: True/False
+        :param http_info: Information on the HTTP request
+        :param request: The authorization request as a Message instance
+        :return: dictionary
         """
 
-        client = self.get_client_from_session_key(state)
-
-        # Look for an IdToken
-        _arg = client.get_context().cstate.get_set(state,
-                                                   claim=["__verified_id_token"])
-
-        if _arg:
-            _now = utc_time_sans_frac()
-            exp = _arg["__verified_id_token"]["exp"]
-            return _now < exp
-        else:
-            return False
+        if "error" in request:
+            return request
 
-    def get_valid_access_token(self, state):
-        """
-        Find a valid access token.
+        _cid = request["client_id"]
+        _context = self.upstream_get("context")
+        cinfo = _context.cdb[_cid]
+        # logger.debug("client {}: {}".format(_cid, cinfo))
 
-        :param state:
-        :return: An access token if a valid one exists and when it
-            expires. Otherwise raise exception.
-        """
+        # this applies the default option deny_unknown_scopes policy
+        check_unknown_scopes_policy(request, _cid, _context)
 
-        token = None
-        indefinite = []
-        now = utc_time_sans_frac()
-
-        client = self.get_client_from_session_key(state)
-        _context = client.get_context()
-        _args = _context.cstate.get_set(state, claim=["access_token", "__expires_at"])
-        if "access_token" in _args:
-            access_token = _args["access_token"]
-            _exp = _args.get("__expires_at", 0)
-            if not _exp:  # No expiry date, lives for ever
-                indefinite.append((access_token, 0))
-            else:
-                if _exp > now:  # expires sometime in the future
-                    token = (access_token, _exp)
+        if http_info is None:
+            http_info = {}
 
-        if indefinite:
-            return indefinite[0]
+        _cookies = http_info.get("cookie")
+        if _cookies:
+            logger.debug("parse_cookie@process_request")
+            _session_cookie_name = _context.cookie_handler.name["session"]
+            try:
+                _my_cookies = _context.cookie_handler.parse_cookie(_session_cookie_name, _cookies)
+            except Exception as err:
+                logger.info(f"Parse cookie failed due to: {err}")
+                _my_cookies = {}
         else:
-            if token:
-                return token
-            else:
-                raise OidcServiceError("No valid access token")
+            _my_cookies = {}
 
-    def logout(
-            self,
-            state: str,
-            client: Optional[Client] = None,
-            post_logout_redirect_uri: Optional[str] = "",
-    ) -> dict:
-        """
-        Does an RP initiated logout from an OP. After logout the user will be
-        redirected by the OP to a URL of choice (post_logout_redirect_uri).
+        kwargs = self.do_request_user(request_info=request, **kwargs)
 
-        :param state: Key to an active session
-        :param client: Which client to use
-        :param post_logout_redirect_uri: If a special post_logout_redirect_uri
-            should be used
-        :return: Request arguments
-        """
+        info = self.setup_auth(request, request["redirect_uri"], cinfo, _my_cookies, **kwargs)
 
-        logger.debug(20 * "*" + " logout " + 20 * "*")
+        if "error" in info:
+            if "response_mode" in request:
+                return self.response_mode(request, info)
+            else:
+                return info
 
-        if client is None:
-            client = self.get_client_from_session_key(state)
+        _function = info.get("function")
+        if not _function:
+            logger.debug("- authenticated -")
+            logger.debug("AREQ keys: %s" % request.keys())
+            return self.authz_part2(request=request, cookie=_my_cookies, **info)
 
         try:
-            srv = client.get_service("end_session")
-        except KeyError:
-            raise OidcServiceError("Does not know how to logout")
-
-        if post_logout_redirect_uri:
-            request_args = {"post_logout_redirect_uri": post_logout_redirect_uri}
-        else:
-            request_args = {}
-
-        resp = srv.get_request_parameters(state=state, request_args=request_args)
-
-        logger.debug(f"EndSession Request: {resp}")
-        return resp
+            # Run the authentication function
+            return {
+                "http_response": _function(**info["args"]),
+                "return_uri": request["redirect_uri"],
+            }
+        except Exception as err:
+            logger.exception(err)
+            return {"http_response": "Internal error: {}".format(err)}
 
-    def close(
-            self, state: str, issuer: Optional[str] = "",
-            post_logout_redirect_uri: Optional[str] = ""
-    ) -> dict:
 
-        logger.debug(20 * "*" + " close " + 20 * "*")
+class AllowedAlgorithms:
+    def __init__(self, algorithm_parameters):
+        self.algorithm_parameters = algorithm_parameters
 
-        if issuer:
-            client = self.issuer2rp[issuer]
-        else:
-            client = self.get_client_from_session_key(state)
+    def __call__(self, client_id, context, alg, alg_type):
+        _cinfo = context.cdb[client_id]
+        _pinfo = context.provider_info
 
-        return self.logout(
-            state=state, client=client, post_logout_redirect_uri=post_logout_redirect_uri
-        )
+        _reg, _sup = self.algorithm_parameters[alg_type]
+        _allowed = _cinfo.get(_reg)
+        if _allowed is None:
+            _allowed = _pinfo.get(_sup)
 
-    def clear_session(self, state):
-        client = self.get_client_from_session_key(state)
-        client.get_context().cstate.remove_state(state)
+        if alg not in _allowed:
+            logger.error("Signing alg user: {} not among allowed: {}".format(alg, _allowed))
+            raise ValueError("Not allowed '%s' algorithm used", alg)
 
 
-def backchannel_logout(client, request="", request_args=None):
+def re_authenticate(request, authn) -> bool:
     """
+    This is where you can demand re-authentication even though the authentication in use
+    is still valid.
 
-    :param request: URL encoded logout request
+    :param request:
+    :param authn:
     :return:
     """
-    if request:
-        req = BackChannelLogoutRequest().from_urlencoded(as_unicode(request))
-    elif request_args:
-        req = BackChannelLogoutRequest(**request_args)
-    else:
-        raise MissingRequiredAttribute("logout_token")
-
-    _context = client.get_context()
-    kwargs = {
-        "aud": client.get_client_id(),
-        "iss": _context.get("issuer"),
-        "keyjar": client.get_attribute('keyjar'),
-        "allowed_sign_alg": _context.get("registration_response").get(
-            "id_token_signed_response_alg", "RS256"
-        ),
-    }
-
-    logger.debug(f"(backchannel_logout) Verifying request using: {kwargs}")
-    try:
-        req.verify(**kwargs)
-    except (MessageException, ValueError, NotForMe) as err:
-        raise MessageException("Bogus logout request: {}".format(err))
-    else:
-        logger.debug("Request verified OK")
-
-    # Find the subject through 'sid' or 'sub'
-    sub = req[verified_claim_name("logout_token")].get("sub")
-    sid = None
-    if not sub:
-        sid = req[verified_claim_name("logout_token")].get("sid")
-
-    if not sub and not sid:
-        raise MessageException('Neither "sid" nor "sub"')
-    elif sub:
-        _state = _context.cstate.get_base_key(sub)
-    elif sid:
-        _state = _context.cstate.get_base_key(sid)
-    else:
-        _state = None
-
-    return _state
+    logger.debug("Re-authenticate ??: {}".format(request))
 
+    _prompt = request.get("prompt", [])
+    logger.debug(f"Prompt={_prompt}")
+    if "login" in _prompt:
+        logger.debug("Reauthenticate due to prompt=login")
+        return True
 
-def load_registration_response(client, request_args=None):
-    """
-    If the client has been statically registered that information
-    must be provided during the configuration. If expected to be
-    done dynamically this method will do dynamic client registration.
-
-    :param client: A :py:class:`idpyoidc.client.oidc.Client` instance
-    """
-    if not client.get_context().get_client_id():
-        try:
-            response = client.do_request("registration", request_args=request_args)
-        except KeyError:
-            raise ConfigurationError("No registration info")
-        except Exception as err:
-            logger.error(err)
-            raise
-        else:
-            if "error" in response:
-                raise OidcServiceError(response.to_json())
+    return False
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/service.py` & `idpyoidc-2.1.0/src/idpyoidc/client/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 import logging
 from typing import Callable
 from typing import List
 from typing import Optional
 from typing import Union
 from urllib.parse import urlparse
 
+from cryptojwt.jwe.jwe import factory as jwe_factory
+from cryptojwt.jws.jws import factory as jws_factory
 from cryptojwt.jwt import JWT
 
 from idpyoidc.client.exception import Unsupported
 from idpyoidc.impexp import ImpExp
 from idpyoidc.item import DLDict
 from idpyoidc.message import Message
-from idpyoidc.message.oauth2 import is_error_message
 from idpyoidc.message.oauth2 import ResponseMessage
+from idpyoidc.message.oauth2 import is_error_message
 from idpyoidc.util import importer
 from .client_auth import client_auth_setup
 from .client_auth import method_to_item
 from .client_auth import single_authn_setup
 from .configure import Configuration
 from .exception import ResponseError
 from .util import get_http_body
@@ -70,18 +72,15 @@
     init_args = ["upstream_get"]
 
     _include = {}
     _supports = {}
     _callback_path = {}
 
     def __init__(
-            self,
-            upstream_get: Callable,
-            conf: Optional[Union[dict, Configuration]] = None,
-            **kwargs
+        self, upstream_get: Callable, conf: Optional[Union[dict, Configuration]] = None, **kwargs
     ):
         ImpExp.__init__(self)
 
         self.upstream_get = upstream_get
         self.default_request_args = {}
         self.client_authn_methods = {}
 
@@ -90,15 +89,15 @@
             for param in [
                 "msg_type",
                 "response_cls",
                 "error_msg",
                 "http_method",
                 "request_body_type",
                 "response_body_type",
-                "default_authn_method"
+                "default_authn_method",
             ]:
                 if param in conf:
                     setattr(self, param, conf[param])
 
             _default_request_args = conf.get("request_args", {})
             if _default_request_args:
                 self.default_request_args = _default_request_args
@@ -107,21 +106,23 @@
             _client_authn_methods = conf.get("client_authn_methods", None)
             if _client_authn_methods:
                 self.client_authn_methods = client_auth_setup(method_to_item(_client_authn_methods))
 
             if self.default_authn_method:
                 if self.default_authn_method not in self.client_authn_methods:
                     self.client_authn_methods[self.default_authn_method] = single_authn_setup(
-                        self.default_authn_method, None)
+                        self.default_authn_method, None
+                    )
 
         else:
             self.conf = {}
             if self.default_authn_method:
                 self.client_authn_methods[self.default_authn_method] = single_authn_setup(
-                    self.default_authn_method, None)
+                    self.default_authn_method, None
+                )
 
         # pull in all the modifiers
         self.pre_construct = []
         self.post_construct = []
         self.construct_extra_headers = []
         self.post_parse_process = []
 
@@ -217,15 +218,15 @@
         _args = self.method_args("post_construct", **kwargs)
 
         for meth in self.post_construct:
             request_args = meth(request_args, service=self, **_args)
 
         return request_args
 
-    def update_service_context(self, resp: Message, key: Optional[str] = '', **kwargs):
+    def update_service_context(self, resp: Message, key: Optional[str] = "", **kwargs):
         """
         A method run after the response has been parsed and verified.
 
         :param resp: The response as a :py:class:`idpyoidc.Message` instance
         :param key: The key under which the response should be stored
         :param kwargs: Extra key word arguments
         """
@@ -293,15 +294,15 @@
                 _context = self.upstream_get("context")
                 try:
                     _func = _context.client_authn_methods[authn_method]
                 except KeyError:  # not one of the common
                     LOGGER.error(f"Unknown client authentication method: {authn_method}")
                     raise Unsupported(f"Unknown client authentication method: {authn_method}")
 
-            return _func.construct(request, self, http_args=http_args, **kwargs)
+            return _func.construct(request=request, service=self, http_args=http_args, **kwargs)
 
         return http_args
 
     def construct_request(self, request_args=None, **kwargs):
         """
         The method where everything is setup for sending the request.
         The request information is gathered and the where and how of sending the
@@ -325,15 +326,15 @@
         """
         if self.endpoint:
             return self.endpoint
 
         return self.upstream_get("context").provider_info[self.endpoint_name]
 
     def get_authn_header(
-            self, request: Union[dict, Message], authn_method: Optional[str] = "", **kwargs
+        self, request: Union[dict, Message], authn_method: Optional[str] = "", **kwargs
     ) -> dict:
         """
         Construct an authorization specification to be sent in the
         HTTP header.
 
         :param request: The service request
         :param authn_method: Which authentication/authorization method to use
@@ -357,19 +358,19 @@
         service.
 
         :return: The authn/authz method
         """
         return self.default_authn_method
 
     def get_headers(
-            self,
-            request: Union[dict, Message],
-            http_method: str,
-            authn_method: Optional[str] = "",
-            **kwargs,
+        self,
+        request: Union[dict, Message],
+        http_method: str,
+        authn_method: Optional[str] = "",
+        **kwargs,
     ) -> dict:
         """
 
         :param request:
         :param authn_method:
         :param kwargs:
         :return:
@@ -377,29 +378,33 @@
         if not authn_method:
             authn_method = self.get_authn_method()
 
         _headers = self.get_authn_header(
             request, authn_method=authn_method, authn_endpoint=self.endpoint_name, **kwargs
         )
 
+        _authz = _headers.get("Authorization")
+        if _authz and _authz.startswith("Bearer"):
+            kwargs["token"] = _authz.split(" ")[1]
+
         for meth in self.construct_extra_headers:
             _headers = meth(
                 self.upstream_get("context"),
                 headers=_headers,
                 request=request,
                 authn_method=authn_method,
                 service_endpoint=self.endpoint_name,
                 http_method=http_method,
                 **kwargs,
             )
 
         return _headers
 
     def get_request_parameters(
-            self, request_args=None, method="", request_body_type="", authn_method="", **kwargs
+        self, request_args=None, method="", request_body_type="", authn_method="", **kwargs
     ) -> dict:
         """
         Builds the request message and constructs the HTTP headers.
 
         This is the starting point for a pipeline that will:
 
         - construct the request message
@@ -493,27 +498,26 @@
         :param response: The service response
         :param kwargs: A set of keyword arguments
         :return: The possibly modified response
         """
         return response
 
     def gather_verify_arguments(
-            self, response: Optional[Union[dict, Message]] = None,
-            behaviour_args: Optional[dict] = None
+        self, response: Optional[Union[dict, Message]] = None, behaviour_args: Optional[dict] = None
     ):
         """
         Need to add some information before running verify()
 
         :return: dictionary with arguments to the verify call
         """
 
         _context = self.upstream_get("context")
         kwargs = {
             "iss": _context.issuer,
-            "keyjar": self.upstream_get('attribute', 'keyjar'),
+            "keyjar": self.upstream_get("attribute", "keyjar"),
             "verify": True,
             "client_id": _context.get_client_id(),
         }
 
         if self.service_name == "provider_info":
             if _context.issuer.startswith("http://"):
                 kwargs["allow_http"] = True
@@ -523,15 +527,15 @@
     def _do_jwt(self, info):
         _context = self.upstream_get("context")
         args = {"allowed_sign_algs": _context.get_sign_alg(self.service_name)}
         enc_algs = _context.get_enc_alg_enc(self.service_name)
         args["allowed_enc_algs"] = enc_algs["alg"]
         args["allowed_enc_encs"] = enc_algs["enc"]
 
-        _jwt = JWT(key_jar=self.upstream_get('attribute', 'keyjar'), **args)
+        _jwt = JWT(key_jar=self.upstream_get("attribute", "keyjar"), **args)
         _jwt.iss = _context.get_client_id()
         return _jwt.unpack(info)
 
     def _do_response(self, info, sformat, **kwargs):
         _context = self.upstream_get("context")
 
         try:
@@ -551,20 +555,20 @@
                     raise
 
             if resp is None:
                 raise ValueError(f"Incorrect message type: {sformat}")
         return resp
 
     def parse_response(
-            self,
-            info,
-            sformat: Optional[str] = "",
-            state: Optional[str] = "",
-            behaviour_args: Optional[dict] = None,
-            **kwargs,
+        self,
+        info,
+        sformat: Optional[str] = "",
+        state: Optional[str] = "",
+        behaviour_args: Optional[dict] = None,
+        **kwargs,
     ):
         """
         This the start of a pipeline that will:
 
             1 Deserializes a response into it's response message class.
               Or :py:class:`idpyoidc.message.oauth2.ErrorResponse` if it's an error
               message
@@ -583,24 +587,31 @@
 
         if not sformat:
             sformat = self.response_body_type
 
         LOGGER.debug("response format: %s", sformat)
 
         resp = None
-        if sformat == "jose":
+        if sformat == "jose":  # can be jwe, jws or json
+            # the checks for JWS and JWE will be replaced with functions from cryptojwt
             try:
-                self._do_jwt(info)
-                sformat = "dict"
-            except Exception:
-                _keyjar = self.upstream_get("attribute", 'keyjar')
-                resp = self.response_cls().from_jwe(info, keys=_keyjar)
+                if jws_factory(info):
+                    info = self._do_jwt(info)
+            except:
+                try:
+                    if jwe_factory(info):
+                        info = self._do_jwt(info)
+                except:
+                    LOGGER.debug('jwe detected')
+            if info and isinstance(info, str):
+                info = json.loads(info)
+            sformat = "dict"
         elif sformat == "jwe":
-            _keyjar = self.upstream_get("attribute", 'keyjar')
-            _client_id = self.upstream_get("attribute", 'client_id')
+            _keyjar = self.upstream_get("attribute", "keyjar")
+            _client_id = self.upstream_get("attribute", "client_id")
             resp = self.response_cls().from_jwe(info, keys=_keyjar.get_issuer_keys(_client_id))
         # If format is urlencoded 'info' may be a URL
         # in which case I have to get at the query/fragment part
         elif sformat == "urlencoded":
             info = self.get_urlinfo(info)
         elif sformat in ["jwt", "jws"]:
             info = self._do_jwt(info)
@@ -612,20 +623,24 @@
         LOGGER.debug("response_cls: %s", self.response_cls.__name__)
 
         if resp is None:
             if not info:
                 LOGGER.error("Missing or faulty response")
                 raise ResponseError("Missing or faulty response")
 
-            resp = self._do_response(info, sformat, **kwargs)
-
-        LOGGER.debug('Initial response parsing => "%s"', resp.to_dict())
+            if sformat == "text":
+                resp = info
+            else:
+                resp = self._do_response(info, sformat, **kwargs)
+                LOGGER.debug('Initial response parsing => "%s"', resp.to_dict())
 
         # is this an error message
-        if is_error_message(resp):
+        if sformat == "text":
+            pass
+        elif is_error_message(resp):
             LOGGER.debug("Error response: %s", resp)
         else:
             vargs = self.gather_verify_arguments(response=resp, behaviour_args=behaviour_args)
             LOGGER.debug("Verify response with %s", vargs)
             try:
                 # verify the message. If something is wrong an exception is thrown
                 resp.verify(**vargs)
@@ -661,27 +676,29 @@
     def get_callback_path(self, callback):
         return self._callback_path.get(callback)
 
     @staticmethod
     def get_uri(base_url, path, hex):
         return f"{base_url}/{path}/{hex}"
 
-    def construct_uris(self,
-                       base_url: str,
-                       hex: bytes,
-                       context: OidcContext,
-                       targets: Optional[List[str]] = None,
-                       response_types: Optional[list] = None):
+    def construct_uris(
+        self,
+        base_url: str,
+        hex: bytes,
+        context: OidcContext,
+        targets: Optional[List[str]] = None,
+        response_types: Optional[list] = None,
+    ):
         if not targets:
             targets = self._callback_path.keys()
 
         if not targets:
             return {}
 
-        _callback_uris = context.get_preference('callback_uris', {})
+        _callback_uris = context.get_preference("callback_uris", {})
         for uri in targets:
             if uri in _callback_uris:
                 pass
             else:
                 _path = self._callback_path.get(uri)
                 if isinstance(_path, str):
                     _callback_uris[uri] = self.get_uri(base_url, _path, hex)
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/service_context.py` & `idpyoidc-2.1.0/src/idpyoidc/client/service_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
 DEFAULT_VALUE = {
     "client_secret": "",
     "client_id": "",
     "redirect_uris": [],
     "provider_info": {},
     "callback": {},
-    "issuer": ""
+    "issuer": "",
 }
 
 
 class ServiceContext(ImpExp):
     """
     This class keeps information that a client needs to be able to talk
     to a server. Some of this information comes from configuration and some
@@ -93,38 +93,40 @@
         # "client_secret_expires_at": 0,
         "clock_skew": None,
         "config": None,
         "hash_seed": b"",
         "httpc_params": None,
         "iss_hash": None,
         "issuer": None,
-        'keyjar': KeyJar,
+        "keyjar": KeyJar,
         "claims": Claims,
         "provider_info": None,
         "requests_dir": None,
         "registration_response": None,
         "cstate": Current,
         # 'usage': None,
         "verify_args": None,
     }
 
     special_load_dump = {
         "specs": {"load": claims_load, "dump": claims_dump},
     }
 
-    init_args = ['upstream_get']
+    init_args = ["upstream_get"]
 
-    def __init__(self,
-                 upstream_get: Optional[Callable] = None,
-                 base_url: Optional[str] = "",
-                 keyjar: Optional[KeyJar] = None,
-                 config: Optional[Union[dict, Configuration]] = None,
-                 cstate: Optional[Current] = None,
-                 client_type: Optional[str] = 'oauth2',
-                 **kwargs):
+    def __init__(
+        self,
+        upstream_get: Optional[Callable] = None,
+        base_url: Optional[str] = "",
+        keyjar: Optional[KeyJar] = None,
+        config: Optional[Union[dict, Configuration]] = None,
+        cstate: Optional[Current] = None,
+        client_type: Optional[str] = "oauth2",
+        **kwargs,
+    ):
         ImpExp.__init__(self)
         config = get_configuration(config)
         self.config = config
         self.upstream_get = upstream_get
 
         if not client_type or client_type == "oidc":
             self.claims = OIDC_Specs()
@@ -134,15 +136,15 @@
             raise ValueError(f"Unknown client type: {client_type}")
 
         self.entity_id = config.conf.get("client_id", "")
         self.cstate = cstate or Current()
 
         self.kid = {"sig": {}, "enc": {}}
 
-        self.allow = config.conf.get('allow', {})
+        self.allow = config.conf.get("allow", {})
         self.base_url = base_url or config.conf.get("base_url", "")
         self.provider_info = config.conf.get("provider_info", {})
 
         # Below so my IDE won't complain
         self.args = {}
         self.add_on = {}
         self.iss_hash = ""
@@ -163,20 +165,23 @@
 
         _seed = config.get("hash_seed", rndstr(32))
         self.hash_seed = as_bytes(_seed)
 
         for key, val in kwargs.items():
             setattr(self, key, val)
 
-        self.keyjar = self.claims.load_conf(config.conf, supports=self.supports(),
-                                            keyjar=keyjar)
+        self.keyjar = self.claims.load_conf(config.conf, supports=self.supports(), keyjar=keyjar)
+
+        _jwks_uri = self.provider_info.get('jwks_uri')
+        if _jwks_uri:
+            self.keyjar.load_keys(self.provider_info.get('issuer'), jwks_uri=_jwks_uri)
 
         _response_types = self.get_preference(
-            'response_types_supported',
-            self.supports().get('response_types_supported', []))
+            "response_types_supported", self.supports().get("response_types_supported", [])
+        )
 
         self.construct_uris(response_types=_response_types)
 
     def __setitem__(self, key, value):
         setattr(self, key, value)
 
     def filename_from_webname(self, webname):
@@ -191,30 +196,30 @@
 
         :param webname: The published URL
         :return: local filename
         """
         if not webname.startswith(self.base_url):
             raise ValueError("Webname doesn't match base_url")
 
-        _name = webname[len(self.base_url):]
+        _name = webname[len(self.base_url) :]
         if _name.startswith("/"):
             return _name[1:]
 
         return _name
 
     def import_keys(self, keyspec):
         """
         The client needs its own set of keys. It can either dynamically
         create them or load them from local storage.
         This method can also fetch other entities keys provided the
         URL points to a JWKS.
 
         :param keyspec:
         """
-        _keyjar = self.upstream_get('attribute', 'keyjar')
+        _keyjar = self.upstream_get("attribute", "keyjar")
         if _keyjar is None:
             _keyjar = KeyJar()
             new = True
         else:
             new = False
 
         for where, spec in keyspec.items():
@@ -228,20 +233,20 @@
                             _keyjar.add_kb("", _bundle)
             elif where == "url":
                 for iss, url in spec.items():
                     _bundle = KeyBundle(source=url)
                     _keyjar.add_kb(iss, _bundle)
 
         if new:
-            _unit = self.upstream_get('unit')
-            _unit.setattribute('keyjar', _keyjar)
+            _unit = self.upstream_get("unit")
+            _unit.setattribute("keyjar", _keyjar)
 
     def _get_crypt(self, typ, attr):
         _item_typ = CLI_REG_MAP.get(typ)
-        _alg = ''
+        _alg = ""
         if _item_typ:
             _alg = self.claims.get_usage(_item_typ[attr])
             if not _alg:
                 _alg = self.claims.get_preference(_item_typ[attr])
 
         if not _alg:
             _item_typ = PROVIDER_INFO_MAP.get(typ)
@@ -252,15 +257,15 @@
 
     def get_sign_alg(self, typ):
         """
 
         :param typ: ['id_token', 'userinfo', 'request_object']
         :return: signing algorithm
         """
-        return self._get_crypt(typ, 'sign')
+        return self._get_crypt(typ, "sign")
 
     def get_enc_alg_enc(self, typ):
         """
 
         :param typ:
         :return:
         """
@@ -282,15 +287,15 @@
 
     def collect_usage(self):
         return self.claims.use
 
     def supports(self):
         res = {}
         if self.upstream_get:
-            services = self.upstream_get('services')
+            services = self.upstream_get("services")
             if not services:
                 pass
             else:
                 for service in services.values():
                     res.update(service.supports())
                     res = service.extends(res)
         res.update(self.claims.supports())
@@ -309,15 +314,15 @@
         return self.claims.get_usage(claim, default)
 
     def set_usage(self, claim, value):
         return self.claims.set_usage(claim, value)
 
     def _callback_per_service(self):
         _cb = {}
-        for service in self.upstream_get('services').values():
+        for service in self.upstream_get("services").values():
             _cbs = service._callback_path.keys()
             if _cbs:
                 _cb[service.service_name] = _cbs
         return _cb
 
     def construct_uris(self, response_types: Optional[list] = None):
         _hash = hashlib.sha256()
@@ -325,49 +330,70 @@
         _hash.update(as_bytes(self.issuer))
         _hex = _hash.hexdigest()
 
         self.iss_hash = _hex
 
         _base_url = self.get("base_url")
 
-        _callback_uris = self.get_preference('callback_uris', {})
+        _callback_uris = self.get_preference("callback_uris", {})
         if self.upstream_get:
-            services = self.upstream_get('services')
+            services = self.upstream_get("services")
             if services:
                 for service in services.values():
-                    _callback_uris.update(service.construct_uris(base_url=_base_url, hex=_hex,
-                                                                 context=self,
-                                                                 response_types=response_types))
+                    _callback_uris.update(
+                        service.construct_uris(
+                            base_url=_base_url,
+                            hex=_hex,
+                            context=self,
+                            response_types=response_types,
+                        )
+                    )
 
-        self.set_preference('callback_uris', _callback_uris)
-        if 'redirect_uris' in _callback_uris:
+        self.set_preference("callback_uris", _callback_uris)
+        if "redirect_uris" in _callback_uris:
             _redirect_uris = set()
-            for flow, _uris in _callback_uris['redirect_uris'].items():
+            for flow, _uris in _callback_uris["redirect_uris"].items():
                 _redirect_uris.update(set(_uris))
-            self.set_preference('redirect_uris', list(_redirect_uris))
+            self.set_preference("redirect_uris", list(_redirect_uris))
 
     def prefer_or_support(self, claim):
         if claim in self.claims.prefer:
-            return 'prefer'
+            return "prefer"
         else:
-            for service in self.upstream_get('services').values():
+            for service in self.upstream_get("services").values():
                 _res = service.prefer_or_support(claim)
                 if _res:
                     return _res
 
         if claim in self.claims.supported(claim):
-            return 'support'
+            return "support"
         return None
 
     def map_supported_to_preferred(self, info: Optional[dict] = None):
-        self.claims.prefer = supported_to_preferred(self.supports(),
-                                                    self.claims.prefer,
-                                                    base_url=self.base_url,
-                                                    info=info)
+        self.claims.prefer = supported_to_preferred(
+            self.supports(), self.claims.prefer, base_url=self.base_url, info=info
+        )
         return self.claims.prefer
 
+    def map_service_against_endpoint(self, provider_config):
+        # Check endpoints against services
+        remove = []
+        for srv_name, srv in self.upstream_get("services").items():
+            if srv.endpoint_name:
+                _match = provider_config.get(srv.endpoint_name)
+                if _match is None:
+                    for key in srv._supports.keys():
+                        if key in self.claims.prefer:
+                            del self.claims.prefer[key]
+                    remove.append(srv_name)
+
+        for item in remove:
+            del self.upstream_get("services")[item]
+
     def map_preferred_to_registered(self, registration_response: Optional[dict] = None):
         self.claims.use = preferred_to_registered(
             self.claims.prefer,
             supported=self.supports(),
-            registration_response=registration_response)
+            registration_response=registration_response,
+        )
+
         return self.claims.use
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/client/util.py` & `idpyoidc-2.1.0/src/idpyoidc/client/util.py`

 * *Files 15% similar despite different names*

```diff
@@ -306,22 +306,26 @@
     res = config.get(param.lower(), default)
     if not res:
         res = config.get(param.upper(), default)
     return res
 
 
 IMPLICIT_RESPONSE_TYPES = [
-    {'id_token'}, {'id_token', 'token'}, {'code', 'token'}, ['code', 'id_token'],
-    {'code', 'id_token', 'token'}, {'token'}
+    {"id_token"},
+    {"id_token", "token"},
+    {"code", "token"},
+    {"code", "id_token"},
+    {"code", "id_token", "token"},
+    {"token"},
 ]
 
 
 def implicit_response_types(a):
     res = []
     for typ in a:
-        if set(typ.split(' ')) in IMPLICIT_RESPONSE_TYPES:
+        if set(typ.split(" ")) in IMPLICIT_RESPONSE_TYPES:
             res.append(typ)
     return res
 
 
 def get_uri(base_url, path, hex):
     return f"{base_url}/{path}/{hex}"
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/configure.py` & `idpyoidc-2.1.0/src/idpyoidc/configure.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/context.py` & `idpyoidc-2.1.0/src/idpyoidc/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     def __init__(self, config=None, entity_id=""):
         ImpExp.__init__(self)
         if entity_id:
             self.entity_id = entity_id
         else:
             if config:
-                val = ''
-                for alt in ['client_id', 'issuer', 'entity_id']:
+                val = ""
+                for alt in ["client_id", "issuer", "entity_id"]:
                     val = config.get(alt)
                     if val:
                         break
                 self.entity_id = val
             else:
-                self.entity_id = ''
+                self.entity_id = ""
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/converter.py` & `idpyoidc-2.1.0/src/idpyoidc/converter.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/encrypter.py` & `idpyoidc-2.1.0/src/idpyoidc/encrypter.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/exception.py` & `idpyoidc-2.1.0/src/idpyoidc/exception.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/impexp.py` & `idpyoidc-2.1.0/src/idpyoidc/impexp.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,19 +74,19 @@
 
         return info
 
     def local_load_adjustments(self, **kwargs):
         pass
 
     def load_attr(
-            self,
-            cls: Any,
-            item: dict,
-            init_args: Optional[dict] = None,
-            load_args: Optional[dict] = None,
+        self,
+        cls: Any,
+        item: dict,
+        init_args: Optional[dict] = None,
+        load_args: Optional[dict] = None,
     ) -> Any:
         if load_args:
             _kwargs = {"load_args": load_args}
         else:
             _kwargs = {}
 
         if init_args:
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/item.py` & `idpyoidc-2.1.0/src/idpyoidc/item.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/logging.py` & `idpyoidc-2.1.0/src/idpyoidc/logging.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/message/__init__.py` & `idpyoidc-2.1.0/src/idpyoidc/message/__init__.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/message/oauth2/__init__.py` & `idpyoidc-2.1.0/src/idpyoidc/message/oauth2/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,14 +133,15 @@
     c_param = {
         "response_type": REQUIRED_LIST_OF_SP_SEP_STRINGS,
         "client_id": SINGLE_REQUIRED_STRING,
         "scope": OPTIONAL_LIST_OF_SP_SEP_STRINGS,
         "redirect_uri": SINGLE_OPTIONAL_STRING,
         "state": SINGLE_OPTIONAL_STRING,
         "request": SINGLE_OPTIONAL_STRING,
+        "resource": OPTIONAL_LIST_OF_STRINGS,  # From RFC8707
     }
 
     def merge(self, request_object, treatement="strict", whitelist=None):
         """
         How to combine parameter that appear in the request with parameters that
         appear in the request object.
 
@@ -223,15 +224,15 @@
     """
 
     c_param = ResponseMessage.c_param.copy()
     c_param.update(
         {
             "code": SINGLE_REQUIRED_STRING,
             "state": SINGLE_OPTIONAL_STRING,
-            "iss": SINGLE_OPTIONAL_STRING,
+            "iss": SINGLE_OPTIONAL_STRING,  # RFC 9207
             "client_id": SINGLE_OPTIONAL_STRING,
         }
     )
 
     def verify(self, **kwargs):
         super(AuthorizationResponse, self).verify(**kwargs)
 
@@ -297,20 +298,20 @@
     Client Credential grant flow access token request
     """
 
     c_param = {
         "client_id": SINGLE_OPTIONAL_STRING,
         "client_secret": SINGLE_OPTIONAL_STRING,
         "grant_type": SINGLE_REQUIRED_STRING,
-        "scope": OPTIONAL_LIST_OF_SP_SEP_STRINGS
+        "scope": OPTIONAL_LIST_OF_SP_SEP_STRINGS,
     }
 
     def verify(self, **kwargs):
-        if self['grant_type'] != 'client_credentials':
-            raise ValueError('Grant type MUST be client_credentials')
+        if self["grant_type"] != "client_credentials":
+            raise ValueError("Grant type MUST be client_credentials")
 
 
 class RefreshAccessTokenRequest(Message):
     """
     Access token refresh request
     """
 
@@ -341,15 +342,15 @@
             "authorization_endpoint": SINGLE_OPTIONAL_STRING,
             "token_endpoint": SINGLE_OPTIONAL_STRING,
             "jwks_uri": SINGLE_OPTIONAL_STRING,
             "registration_endpoint": SINGLE_OPTIONAL_STRING,
             "scopes_supported": OPTIONAL_LIST_OF_STRINGS,
             "response_types_supported": REQUIRED_LIST_OF_STRINGS,
             "response_modes_supported": OPTIONAL_LIST_OF_STRINGS,
-            "grant_types_supported": REQUIRED_LIST_OF_STRINGS,
+            "grant_types_supported": OPTIONAL_LIST_OF_STRINGS,
             "token_endpoint_auth_methods_supported": OPTIONAL_LIST_OF_STRINGS,
             "token_endpoint_auth_signing_alg_values_supported": OPTIONAL_LIST_OF_STRINGS,
             "service_documentation": SINGLE_OPTIONAL_STRING,
             "ui_locales_supported": OPTIONAL_LIST_OF_STRINGS,
             "op_policy_uri": SINGLE_OPTIONAL_STRING,
             "op_tos_uri": SINGLE_OPTIONAL_STRING,
             "code_challenge_methods_supported": OPTIONAL_LIST_OF_STRINGS,
@@ -374,14 +375,15 @@
         except FormatError:
             pass
     raise FormatError("Unexpected format")
 
 
 class OauthClientMetadata(Message):
     """Metadata for an OAuth2 Client."""
+
     c_param = {
         "redirect_uris": OPTIONAL_LIST_OF_STRINGS,
         "token_endpoint_auth_method": SINGLE_OPTIONAL_STRING,
         "grant_type": OPTIONAL_LIST_OF_STRINGS,
         "response_types": OPTIONAL_LIST_OF_STRINGS,
         "client_name": SINGLE_OPTIONAL_STRING,
         "client_uri": SINGLE_OPTIONAL_STRING,
@@ -389,53 +391,73 @@
         "scope": OPTIONAL_LIST_OF_SP_SEP_STRINGS,
         "contacts": OPTIONAL_LIST_OF_STRINGS,
         "tos_uri": SINGLE_OPTIONAL_STRING,
         "policy_uri": SINGLE_OPTIONAL_STRING,
         "jwks_uri": SINGLE_OPTIONAL_STRING,
         "jwks": SINGLE_OPTIONAL_JSON,
         "software_id": SINGLE_OPTIONAL_STRING,
-        "software_version": SINGLE_OPTIONAL_STRING
+        "software_version": SINGLE_OPTIONAL_STRING,
+        "software_statement": SINGLE_OPTIONAL_JSON,
     }
 
+    def verify(self, **kwargs):
+        super(OauthClientMetadata, self).verify(**kwargs)
+
+        # if grant type is present and if contains the values authorization_code or
+        # implicit then redirect_uris must be present
+
+        _grant_types = self.get("grant_types", [])
+        if set(_grant_types).intersection({"authorization_code", "implicit"}):
+            if "redirect_uris" not in self:
+                raise ValueError("Missing redirect_uris claim")
+
 
 def oauth_client_metadata_deser(val, sformat="json"):
     """Deserializes a JSON object (most likely) into a OauthClientMetadata."""
     return deserialize_from_one_of(val, OauthClientMetadata, sformat)
 
 
-OPTIONAL_OAUTH_CLIENT_METADATA = (Message, False, msg_ser,
-                                  oauth_client_metadata_deser, False)
+OPTIONAL_OAUTH_CLIENT_METADATA = (Message, False, msg_ser, oauth_client_metadata_deser, False)
 
 
 class OauthClientInformationResponse(OauthClientMetadata):
     """The information returned by a OAuth2 Server about an OAuth2 client."""
+
     c_param = OauthClientMetadata.c_param.copy()
-    c_param.update({
-        "client_id": SINGLE_REQUIRED_STRING,
-        "client_secret": SINGLE_OPTIONAL_STRING,
-        "client_id_issued_at": SINGLE_OPTIONAL_INT,
-        "client_secret_expires_at": SINGLE_OPTIONAL_INT
-    })
+    c_param.update(
+        {
+            "client_id": SINGLE_REQUIRED_STRING,
+            "client_secret": SINGLE_OPTIONAL_STRING,
+            "client_id_issued_at": SINGLE_OPTIONAL_INT,
+            "client_secret_expires_at": SINGLE_OPTIONAL_INT,
+        }
+    )
 
     def verify(self, **kwargs):
         super(OauthClientInformationResponse, self).verify(**kwargs)
 
         if "client_secret" in self:
             if "client_secret_expires_at" not in self:
                 raise MissingRequiredAttribute(
-                    "client_secret_expires_at is a MUST if client_secret is present")
+                    "client_secret_expires_at is a MUST if client_secret is present"
+                )
 
 
 def oauth_client_registration_response_deser(val, sformat="json"):
     """Deserializes a JSON object (most likely) into a OauthClientInformationResponse."""
     return deserialize_from_one_of(val, OauthClientInformationResponse, sformat)
 
 
 OPTIONAL_OAUTH_CLIENT_REGISTRATION_RESPONSE = (
-    Message, False, msg_ser, oauth_client_registration_response_deser, False)
+    Message,
+    False,
+    msg_ser,
+    oauth_client_registration_response_deser,
+    False,
+)
 
 
 # RFC 7662
 class TokenIntrospectionRequest(Message):
     c_param = {
         "token": SINGLE_REQUIRED_STRING,
         "token_type_hint": SINGLE_OPTIONAL_STRING,
@@ -561,38 +583,38 @@
         "sub": SINGLE_REQUIRED_STRING,
         "client_id": SINGLE_REQUIRED_STRING,
         "iat": SINGLE_REQUIRED_INT,
         "jti": SINGLE_REQUIRED_STRING,
         "auth_time": SINGLE_OPTIONAL_INT,
         "acr": SINGLE_OPTIONAL_STRING,
         "amr": OPTIONAL_LIST_OF_STRINGS,
-        'scope': OPTIONAL_LIST_OF_SP_SEP_STRINGS,
-        'groups': OPTIONAL_LIST_OF_STRINGS,
-        'roles': OPTIONAL_LIST_OF_STRINGS,
-        'entitlements': OPTIONAL_LIST_OF_STRINGS
+        "scope": OPTIONAL_LIST_OF_SP_SEP_STRINGS,
+        "groups": OPTIONAL_LIST_OF_STRINGS,
+        "roles": OPTIONAL_LIST_OF_STRINGS,
+        "entitlements": OPTIONAL_LIST_OF_STRINGS,
     }
 
 
 class JSONWebToken(Message):
     # implements RFC 9068
     c_param = {
-        'iss': SINGLE_REQUIRED_STRING,
-        'exp': SINGLE_REQUIRED_STRING,
-        'aud': SINGLE_REQUIRED_STRING,
-        'sub': SINGLE_REQUIRED_STRING,
+        "iss": SINGLE_REQUIRED_STRING,
+        "exp": SINGLE_REQUIRED_STRING,
+        "aud": SINGLE_REQUIRED_STRING,
+        "sub": SINGLE_REQUIRED_STRING,
         "client_id": SINGLE_REQUIRED_STRING,
-        'iat': SINGLE_REQUIRED_STRING,
-        'jti': SINGLE_REQUIRED_STRING,
-        'auth_time': SINGLE_OPTIONAL_INT,
-        'acr': SINGLE_OPTIONAL_STRING,
-        'amr': OPTIONAL_LIST_OF_STRINGS,
-        'scope': OPTIONAL_LIST_OF_SP_SEP_STRINGS,
-        'groups': OPTIONAL_LIST_OF_STRINGS,
-        'roles': OPTIONAL_LIST_OF_STRINGS,
-        'entitlements': OPTIONAL_LIST_OF_STRINGS
+        "iat": SINGLE_REQUIRED_STRING,
+        "jti": SINGLE_REQUIRED_STRING,
+        "auth_time": SINGLE_OPTIONAL_INT,
+        "acr": SINGLE_OPTIONAL_STRING,
+        "amr": OPTIONAL_LIST_OF_STRINGS,
+        "scope": OPTIONAL_LIST_OF_SP_SEP_STRINGS,
+        "groups": OPTIONAL_LIST_OF_STRINGS,
+        "roles": OPTIONAL_LIST_OF_STRINGS,
+        "entitlements": OPTIONAL_LIST_OF_STRINGS,
     }
 
 
 # RFC 7009
 class TokenRevocationRequest(Message):
     c_param = {
         "token": SINGLE_REQUIRED_STRING,
@@ -607,20 +629,17 @@
     pass
 
 
 class TokenRevocationErrorResponse(ResponseMessage):
     """
     Error response from the revocation endpoint
     """
+
     c_allowed_values = ResponseMessage.c_allowed_values.copy()
-    c_allowed_values.update({
-        "error": [
-            "unsupported_token_type"
-        ]
-    })
+    c_allowed_values.update({"error": ["unsupported_token_type"]})
 
 
 def factory(msgtype, **kwargs):
     """
     Factory method that can be used to easily instansiate a class instance
 
     :param msgtype: The name of the class
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/message/oauth2/device_authorization.py` & `idpyoidc-2.1.0/src/idpyoidc/message/oauth2/device_authorization.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/message/oidc/__init__.py` & `idpyoidc-2.1.0/src/idpyoidc/message/oidc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,14 +236,15 @@
 ID_TOKEN_VERIFY_ARGS = [
     "keyjar",
     "verify",
     "encalg",
     "encenc",
     "sigalg",
     "issuer",
+    "iss",
     "allow_missing_kid",
     "no_kid_issuer",
     "trusting",
     "skew",
     "nonce_storage_time",
     "client_id",
     "allow_sign_alg_none",
@@ -631,14 +632,15 @@
         "post_logout_redirect_uri": SINGLE_OPTIONAL_STRING,
         "frontchannel_logout_uri": SINGLE_OPTIONAL_STRING,
         "frontchannel_logout_session_required": SINGLE_OPTIONAL_BOOLEAN,
         "backchannel_logout_uri": SINGLE_OPTIONAL_STRING,
         "backchannel_logout_session_required": SINGLE_OPTIONAL_BOOLEAN,
         # "federation_type": OPTIONAL_LIST_OF_STRINGS,
         # "organization_name": SINGLE_OPTIONAL_STRING,
+        "response_modes": OPTIONAL_LIST_OF_STRINGS,
     }
     c_default = {"application_type": "web", "response_types": ["code"]}
     c_allowed_values = {
         "application_type": ["native", "web"],
         "subject_type": ["public", "pairwise"],
     }
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/message/oidc/backchannel_authentication.py` & `idpyoidc-2.1.0/src/idpyoidc/message/oidc/backchannel_authentication.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/message/oidc/session.py` & `idpyoidc-2.1.0/src/idpyoidc/message/oidc/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         _now = utc_time_sans_frac()
 
         try:
             _skew = kwargs["skew"]
         except KeyError:
             _skew = 0
 
-        if 'iat' in self and self["iat"] > (_now + _skew):
+        if "iat" in self and self["iat"] > (_now + _skew):
             raise ValueError("Invalid issued_at time")
 
         _allowed = kwargs.get("allowed_sign_alg")
         if _allowed and self.jws_header["alg"] != _allowed:
             _msg = "Wrong token signing algorithm, {} != {}".format(
                 self.jws_header["alg"], kwargs["allowed_sign_alg"]
             )
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/metadata.py` & `idpyoidc-2.1.0/src/idpyoidc/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,26 +25,19 @@
     _class_name = list(item.keys())[0]  # there is only one
     _cls = importer(_class_name)
     _cls = _cls().load(item[_class_name])
     return _cls
 
 
 class Metadata(ImpExp):
-    parameter = {
-        "prefer": None,
-        "use": None,
-        "callback_path": None,
-        "_local": None
-    }
+    parameter = {"prefer": None, "use": None, "callback_path": None, "_local": None}
 
     _supports = {}
 
-    def __init__(self,
-                 prefer: Optional[dict] = None,
-                 callback_path: Optional[dict] = None):
+    def __init__(self, prefer: Optional[dict] = None, callback_path: Optional[dict] = None):
 
         ImpExp.__init__(self)
         if isinstance(prefer, dict):
             self.prefer = {k: v for k, v in prefer.items() if k in self._supports}
         else:
             self.prefer = {}
 
@@ -69,58 +62,55 @@
 
     def remove_preference(self, key):
         if key in self.prefer:
             del self.prefer[key]
 
     def _callback_uris(self, base_url, hex):
         _uri = []
-        for type in self.get_usage("response_types", self._supports['response_types']):
+        for type in self.get_usage("response_types", self._supports["response_types"]):
             if "code" in type:
-                _uri.append('code')
+                _uri.append("code")
             elif type in ["id_token", "id_token token"]:
-                _uri.append('implicit')
+                _uri.append("implicit")
 
         if "form_post" in self.supports:
             _uri.append("form_post")
 
         callback_uri = {}
         for key in _uri:
             callback_uri[key] = get_uri(base_url, self.callback_path[key], hex)
         return callback_uri
 
-    def construct_redirect_uris(self,
-                                base_url: str,
-                                hex: str,
-                                callbacks: Optional[dict] = None):
+    def construct_redirect_uris(self, base_url: str, hex: str, callbacks: Optional[dict] = None):
         if not callbacks:
             callbacks = self._callback_uris(base_url, hex)
 
         if callbacks:
-            self.set_preference('callbacks', callbacks)
+            self.set_preference("callbacks", callbacks)
             self.set_preference("redirect_uris", [v for k, v in callbacks.items()])
 
         self.callback = callbacks
 
-    def verify_rules(self):
+    def verify_rules(self, supports):
         return True
 
     def locals(self, info):
         pass
 
     def _keyjar(self, keyjar=None, conf=None, entity_id=""):
-        _uri_path = ''
+        _uri_path = ""
         if keyjar is None:
             if "keys" in conf:
                 keys_args = {k: v for k, v in conf["keys"].items() if k != "uri_path"}
                 _keyjar = init_key_jar(**keys_args)
-                _uri_path = conf['keys'].get('uri_path')
+                _uri_path = conf["keys"].get("uri_path")
             elif "key_conf" in conf and conf["key_conf"]:
                 keys_args = {k: v for k, v in conf["key_conf"].items() if k != "uri_path"}
                 _keyjar = init_key_jar(**keys_args)
-                _uri_path = conf['key_conf'].get('uri_path')
+                _uri_path = conf["key_conf"].get("uri_path")
             else:
                 _keyjar = KeyJar()
                 if "jwks" in conf:
                     _keyjar.import_jwks(conf["jwks"], "")
 
             if "" in _keyjar and entity_id:
                 # make sure I have the keys under my own name too (if I know it)
@@ -129,70 +119,72 @@
             _httpc_params = conf.get("httpc_params")
             if _httpc_params:
                 _keyjar.httpc_params = _httpc_params
 
             return _keyjar, _uri_path
         else:
             if "keys" in conf:
-                _uri_path = conf['keys'].get('uri_path')
+                _uri_path = conf["keys"].get("uri_path")
             elif "key_conf" in conf and conf["key_conf"]:
-                _uri_path = conf['key_conf'].get('uri_path')
+                _uri_path = conf["key_conf"].get("uri_path")
             return keyjar, _uri_path
 
     def get_base_url(self, configuration: dict):
         raise NotImplementedError()
 
     def get_id(self, configuration: dict):
         raise NotImplementedError()
 
     def add_extra_keys(self, keyjar, id):
         return None
 
     def get_jwks(self, keyjar):
         return None
 
-    def handle_keys(self, configuration: dict, keyjar: Optional[KeyJar] = None,
-                    base_url: Optional[str] = ''):
+    def handle_keys(
+        self, configuration: dict, keyjar: Optional[KeyJar] = None, base_url: Optional[str] = ""
+    ):
         _jwks = _jwks_uri = None
         _id = self.get_id(configuration)
         keyjar, uri_path = self._keyjar(keyjar, configuration, entity_id=_id)
 
         self.add_extra_keys(keyjar, _id)
 
         # now that keys are in the Key Jar, now for how to publish it
-        if 'jwks_uri' in configuration:  # simple
-            _jwks_uri = configuration.get('jwks_uri')
+        if "jwks_uri" in configuration:  # simple
+            _jwks_uri = configuration.get("jwks_uri")
         elif uri_path:
             if not base_url:
                 base_url = self.get_base_url(configuration)
             _jwks_uri = add_path(base_url, uri_path)
         else:  # jwks or nothing
             _jwks = self.get_jwks(keyjar)
 
-        return {'keyjar': keyjar, 'jwks': _jwks, 'jwks_uri': _jwks_uri}
+        return {"keyjar": keyjar, "jwks": _jwks, "jwks_uri": _jwks_uri}
 
-    def load_conf(self, configuration, supports, keyjar: Optional[KeyJar] = None,
-                  base_url: Optional[str] = ''):
+    def load_conf(
+        self, configuration, supports, keyjar: Optional[KeyJar] = None, base_url: Optional[str] = ""
+    ):
         for attr, val in configuration.items():
             if attr == "preference":
                 for k, v in val.items():
                     if k in supports:
                         self.set_preference(k, v)
             elif attr in supports:
                 self.set_preference(attr, val)
 
         self.locals(configuration)
 
         for key, val in self.handle_keys(configuration, keyjar=keyjar, base_url=base_url).items():
-            if key == 'keyjar':
+            if key == "keyjar":
                 keyjar = val
             elif val:
                 self.set_preference(key, val)
 
-        self.verify_rules()
+        self.verify_rules(supports)
         return keyjar
 
     def get(self, key, default=None):
         if key in self._local:
             return self._local[key]
         else:
             return default
@@ -215,49 +207,49 @@
     def supported(self, claim):
         return claim in self._supports
 
     def prefers(self):
         return self.prefer
 
 
-SIGNING_ALGORITHM_SORT_ORDER = ['RS', 'ES', 'PS', 'HS']
+SIGNING_ALGORITHM_SORT_ORDER = ["RS", "ES", "PS", "HS"]
 
 
 def cmp(a, b):
     return (a > b) - (a < b)
 
 
 def alg_cmp(a, b):
-    if a == 'none':
+    if a == "none":
         return 1
-    elif b == 'none':
+    elif b == "none":
         return -1
 
     _pos1 = SIGNING_ALGORITHM_SORT_ORDER.index(a[0:2])
     _pos2 = SIGNING_ALGORITHM_SORT_ORDER.index(b[0:2])
     if _pos1 == _pos2:
         return (a > b) - (a < b)
     elif _pos1 > _pos2:
         return 1
     else:
         return -1
 
 
 def get_signing_algs():
     # Assumes Cryptojwt
-    _algs = [name for name in list(SIGNER_ALGS.keys()) if name != 'none']
+    _algs = [name for name in list(SIGNER_ALGS.keys()) if name != "none"]
     return sorted(_algs, key=cmp_to_key(alg_cmp))
 
 
 def get_encryption_algs():
-    return SUPPORTED['alg']
+    return SUPPORTED["alg"]
 
 
 def get_encryption_encs():
-    return SUPPORTED['enc']
+    return SUPPORTED["enc"]
 
 
 def array_or_singleton(claim_spec, values):
     if isinstance(claim_spec[0], list):
         if isinstance(values, list):
             return values
         else:
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/node.py` & `idpyoidc-2.1.0/src/idpyoidc/node.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import Callable
 from typing import Optional
 from typing import Union
 
 from cryptojwt import KeyJar
+from cryptojwt.key_jar import build_keyjar
 from cryptojwt.key_jar import init_key_jar
 
+from idpyoidc.client.defaults import DEFAULT_KEY_DEFS
 from idpyoidc.configure import Configuration
 from idpyoidc.impexp import ImpExp
 from idpyoidc.util import instantiate
 
 
 def create_keyjar(
         keyjar: Optional[KeyJar] = None,
@@ -39,16 +41,58 @@
             _keyjar.import_jwks_as_json(_keyjar.export_jwks_as_json(True, ""), id)
 
         return _keyjar
     else:
         return keyjar
 
 
-class Node:
+def make_keyjar(
+        keyjar: Optional[Union[KeyJar, bool]] = None,
+        config: Optional[Union[Configuration, dict]] = None,
+        key_conf: Optional[dict] = None,
+        issuer_id: Optional[str] = "",
+        client_id: Optional[str] = "",
+    ):
+    if keyjar is False:
+        return None
+
+    keyjar = keyjar or config.get("keyjar")
+    key_conf = key_conf or config.get("key_conf", config.get("keys"))
+
+    if not keyjar and not key_conf:
+        keyjar = KeyJar()
+        _jwks = config.get("jwks")
+        if _jwks:
+            keyjar.import_jwks_as_json(_jwks, client_id)
+
+    if keyjar or key_conf:
+        # Should be either one
+        id = issuer_id or client_id
+        keyjar = create_keyjar(keyjar, conf=config, key_conf=key_conf, id=id)
+        if client_id:
+            _key = config.get("client_secret")
+            if _key:
+                keyjar.add_symmetric(client_id, _key)
+                keyjar.add_symmetric("", _key)
+    else:
+        if client_id:
+            _key = config.get("client_secret")
+            if _key:
+                keyjar = KeyJar()
+                keyjar.add_symmetric(client_id, _key)
+                keyjar.add_symmetric("", _key)
+        else:
+            keyjar = build_keyjar(DEFAULT_KEY_DEFS)
+            if issuer_id:
+                keyjar.import_jwks(keyjar.export_jwks(private=True), issuer_id)
+
+    return keyjar
 
+
+class Node:
     def __init__(self, upstream_get: Callable = None):
         self.upstream_get = upstream_get
 
     def unit_get(self, what, *arg):
         _func = getattr(self, f"get_{what}", None)
         if _func:
             return _func(*arg)
@@ -72,59 +116,37 @@
         setattr(self, attr, val)
 
     def get_unit(self, *args):
         return self
 
 
 class Unit(ImpExp):
-    name = ''
+    name = ""
 
-    init_args = ['upstream_get']
+    init_args = ["upstream_get"]
 
-    def __init__(self,
-                 upstream_get: Callable = None,
-                 keyjar: Optional[KeyJar] = None,
-                 httpc: Optional[object] = None,
-                 httpc_params: Optional[dict] = None,
-                 config: Optional[Union[Configuration, dict]] = None,
-                 key_conf: Optional[dict] = None,
-                 issuer_id: Optional[str] = '',
-                 client_id: Optional[str] = ''
-                 ):
+    def __init__(
+            self,
+            upstream_get: Callable = None,
+            keyjar: Optional[Union[KeyJar, bool]] = None,
+            httpc: Optional[object] = None,
+            httpc_params: Optional[dict] = None,
+            config: Optional[Union[Configuration, dict]] = None,
+            key_conf: Optional[dict] = None,
+            issuer_id: Optional[str] = "",
+            client_id: Optional[str] = "",
+    ):
         ImpExp.__init__(self)
         self.upstream_get = upstream_get
         self.httpc = httpc
 
         if config is None:
             config = {}
 
-        keyjar = keyjar or config.get('keyjar')
-        key_conf = key_conf or config.get('key_conf', config.get('keys'))
-
-        if not keyjar and not key_conf:
-            _jwks = config.get('jwks')
-            if _jwks:
-                keyjar = KeyJar()
-                keyjar.import_jwks_as_json(_jwks, client_id)
-
-        if keyjar or key_conf:
-            # Should be either one
-            id = issuer_id or client_id
-            self.keyjar = create_keyjar(keyjar, conf=config, key_conf=key_conf, id=id)
-            if client_id:
-                self.keyjar.add_symmetric('', client_id)
-        else:
-            if client_id:
-                _key = config.get("client_secret")
-                if _key:
-                    self.keyjar = KeyJar()
-                    self.keyjar.add_symmetric(client_id, _key)
-                    self.keyjar.add_symmetric('', _key)
-            else:
-                self.keyjar = None
+        self.keyjar = make_keyjar(keyjar, config, key_conf, issuer_id, client_id)
 
         self.httpc_params = httpc_params or config.get("httpc_params", {})
 
         if self.keyjar:
             self.keyjar.httpc = self.httpc
             self.keyjar.httpc_params = self.httpc_params
 
@@ -152,107 +174,121 @@
         setattr(self, attr, val)
 
     def get_unit(self, *args):
         return self
 
 
 def topmost_unit(unit):
-    if hasattr(unit, 'upstream_get'):
+    if hasattr(unit, "upstream_get"):
         if unit.upstream_get:
-            next_unit = unit.upstream_get('unit')
+            next_unit = unit.upstream_get("unit")
             if next_unit:
                 unit = topmost_unit(next_unit)
 
     return unit
 
 
 class ClientUnit(Unit):
-    name = ''
+    name = ""
 
-    def __init__(self,
-                 upstream_get: Callable = None,
-                 httpc: Optional[object] = None,
-                 httpc_params: Optional[dict] = None,
-                 keyjar: Optional[KeyJar] = None,
-                 context: Optional[ImpExp] = None,
-                 config: Optional[Union[Configuration, dict]] = None,
-                 # jwks_uri: Optional[str] = "",
-                 entity_id: Optional[str] = "",
-                 key_conf: Optional[dict] = None
-                 ):
+    def __init__(
+            self,
+            upstream_get: Callable = None,
+            httpc: Optional[object] = None,
+            httpc_params: Optional[dict] = None,
+            keyjar: Optional[KeyJar] = None,
+            context: Optional[ImpExp] = None,
+            config: Optional[Union[Configuration, dict]] = None,
+            # jwks_uri: Optional[str] = "",
+            entity_id: Optional[str] = "",
+            key_conf: Optional[dict] = None,
+    ):
         if config is None:
             config = {}
 
-        self.entity_id = entity_id or config.get('entity_id')
-        self.client_id = config.get('client_id', entity_id)
+        self.entity_id = entity_id or config.get("entity_id")
+        self.client_id = config.get("client_id", entity_id)
 
-        Unit.__init__(self, upstream_get=upstream_get, keyjar=keyjar, httpc=httpc,
-                      httpc_params=httpc_params, config=config, client_id=self.client_id,
-                      key_conf=key_conf)
+        Unit.__init__(
+            self,
+            upstream_get=upstream_get,
+            keyjar=keyjar,
+            httpc=httpc,
+            httpc_params=httpc_params,
+            config=config,
+            client_id=self.client_id,
+            key_conf=key_conf,
+        )
 
         self.context = context or None
 
     def get_context_attribute(self, attr, *args):
         _val = getattr(self.context, attr)
         if not _val and self.upstream_get:
-            return self.upstream_get('context_attribute', attr)
+            return self.upstream_get("context_attribute", attr)
         else:
             return _val
 
 
 # Neither client nor Server
 class Collection(Unit):
-
-    def __init__(self,
-                 upstream_get: Callable = None,
-                 keyjar: Optional[KeyJar] = None,
-                 httpc: Optional[object] = None,
-                 httpc_params: Optional[dict] = None,
-                 config: Optional[Union[Configuration, dict]] = None,
-                 entity_id: Optional[str] = "",
-                 key_conf: Optional[dict] = None,
-                 functions: Optional[dict] = None,
-                 claims: Optional[dict] = None
-                 ):
+    def __init__(
+            self,
+            upstream_get: Callable = None,
+            keyjar: Optional[KeyJar] = None,
+            httpc: Optional[object] = None,
+            httpc_params: Optional[dict] = None,
+            config: Optional[Union[Configuration, dict]] = None,
+            entity_id: Optional[str] = "",
+            key_conf: Optional[dict] = None,
+            functions: Optional[dict] = None,
+            claims: Optional[dict] = None,
+    ):
         if config is None:
             config = {}
 
-        self.entity_id = entity_id or config.get('entity_id')
+        self.entity_id = entity_id or config.get("entity_id")
 
-        Unit.__init__(self, upstream_get, keyjar, httpc, httpc_params, config,
-                      issuer_id=self.entity_id, key_conf=key_conf)
+        Unit.__init__(
+            self,
+            upstream_get,
+            keyjar,
+            httpc,
+            httpc_params,
+            config,
+            issuer_id=self.entity_id,
+            key_conf=key_conf,
+        )
 
-        _args = {
-            'upstream_get': self.unit_get
-        }
+        _args = {"upstream_get": self.unit_get}
 
         self.claims = claims or {}
         self.upstream_get = upstream_get
         # self.context = {}
 
         if functions:
             for key, val in functions.items():
                 _kwargs = val["kwargs"].copy()
                 _kwargs.update(_args)
                 setattr(self, key, instantiate(val["class"], **_kwargs))
 
     def get_context_attribute(self, attr, *args):
-        _cntx = getattr(self, 'context', None)
+        _cntx = getattr(self, "context", None)
         if _cntx:
             _val = getattr(_cntx, attr, None)
             if _val:
                 return _val
 
         if self.upstream_get:
-            return self.upstream_get('context_attribute', attr)
+            return self.upstream_get("context_attribute", attr)
         else:
             return None
 
     def get_attribute(self, attr, *args):
         val = getattr(self, attr, None)
         if val:
             return val
 
         if self.upstream_get:
-            return self.upstream_get('attribute', attr)
+            return self.upstream_get("attribute", attr)
         else:
             return None
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/__init__.py` & `idpyoidc-2.1.0/src/idpyoidc/server/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 from typing import Callable
 from typing import Optional
 from typing import Union
 
 from cryptojwt import KeyJar
 
 from idpyoidc.node import Unit
+
 # from idpyoidc.server import authz
 # from idpyoidc.server.client_authn import client_auth_setup
 from idpyoidc.server.configure import ASConfiguration
 from idpyoidc.server.configure import OPConfiguration
 from idpyoidc.server.endpoint import Endpoint
 from idpyoidc.server.endpoint_context import EndpointContext
+
 # from idpyoidc.server.session.manager import create_session_manager
 # from idpyoidc.server.user_authn.authn_context import populate_authn_broker
 from idpyoidc.server.util import allow_refresh_token
 from idpyoidc.server.util import build_endpoints
 
 logger = logging.getLogger(__name__)
 
@@ -30,59 +32,66 @@
         return {}
 
 
 class Server(Unit):
     parameter = {"endpoint": [Endpoint], "context": EndpointContext}
 
     def __init__(
-            self,
-            conf: Union[dict, OPConfiguration, ASConfiguration],
-            keyjar: Optional[KeyJar] = None,
-            cwd: Optional[str] = "",
-            cookie_handler: Optional[Any] = None,
-            httpc: Optional[Callable] = None,
-            upstream_get: Optional[Callable] = None,
-            httpc_params: Optional[dict] = None,
-            entity_id: Optional[str] = "",
-            key_conf: Optional[dict] = None
+        self,
+        conf: Union[dict, OPConfiguration, ASConfiguration],
+        keyjar: Optional[KeyJar] = None,
+        cwd: Optional[str] = "",
+        cookie_handler: Optional[Any] = None,
+        httpc: Optional[Callable] = None,
+        upstream_get: Optional[Callable] = None,
+        httpc_params: Optional[dict] = None,
+        entity_id: Optional[str] = "",
+        key_conf: Optional[dict] = None,
     ):
-        self.entity_id = entity_id or conf.get('entity_id')
-        self.issuer = conf.get('issuer', self.entity_id)
+        self.entity_id = entity_id or conf.get("entity_id")
+        self.issuer = conf.get("issuer", self.entity_id)
 
-        Unit.__init__(self, config=conf, keyjar=keyjar, httpc=httpc, upstream_get=upstream_get,
-                      httpc_params=httpc_params, key_conf=key_conf,
-                      issuer_id=self.issuer)
+        Unit.__init__(
+            self,
+            config=conf,
+            keyjar=keyjar,
+            httpc=httpc,
+            upstream_get=upstream_get,
+            httpc_params=httpc_params,
+            key_conf=key_conf,
+            issuer_id=self.issuer,
+        )
 
         self.upstream_get = upstream_get
         if isinstance(conf, OPConfiguration) or isinstance(conf, ASConfiguration):
             self.conf = conf
         else:
             self.conf = OPConfiguration(conf)
 
         self.endpoint = do_endpoints(self.conf, self.unit_get)
 
         self.context = EndpointContext(
             conf=self.conf,
             upstream_get=self.unit_get,  # points to me
             cwd=cwd,
             cookie_handler=cookie_handler,
-            keyjar=self.keyjar
+            keyjar=self.keyjar,
         )
 
         # Need to have context in place before doing this
         self.context.do_add_on(endpoints=self.endpoint)
 
         for endpoint_name, _ in self.endpoint.items():
             self.endpoint[endpoint_name].upstream_get = self.unit_get
 
         _token_endp = self.endpoint.get("token")
-        if _token_endp:
-            _token_endp.allow_refresh = allow_refresh_token(self.context)
 
         self.context.map_supported_to_preferred()
+        if _token_endp:
+            _token_endp.allow_refresh = allow_refresh_token(self.context)
 
     def get_endpoints(self, *arg):
         return self.endpoint
 
     def get_endpoint(self, endpoint_name, *arg):
         try:
             return self.endpoint[endpoint_name]
@@ -100,8 +109,8 @@
 
     def get_entity(self, *args):
         return self
 
     def get_context_attribute(self, attr, *args):
         _val = getattr(self.context, attr)
         if not _val and self.upstream_get:
-            return self.upstream_get('context_attribute', attr)
+            return self.upstream_get("context_attribute", attr)
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/authn_event.py` & `idpyoidc-2.1.0/src/idpyoidc/server/authn_event.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/authz/__init__.py` & `idpyoidc-2.1.0/src/idpyoidc/server/authz/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,19 +58,17 @@
     def __call__(
         self,
         session_id: str,
         request: Union[dict, Message],
         resources: Optional[list] = None,
     ) -> Grant:
         _context = self.upstream_get("context")
-        session_info = _context.session_manager.get_session_info(
-            session_id=session_id, grant=True
-        )
+        session_info = _context.session_manager.get_session_info(session_id=session_id, grant=True)
         grant = session_info["grant"]
-        _client_id = session_info['client_id']
+        _client_id = session_info["client_id"]
 
         args = self.grant_config.copy()
 
         for key, val in args.items():
             if key == "expires_in":
                 grant.set_expires_at(val)
             elif key == "usage_rules":
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/claims/__init__.py` & `idpyoidc-2.1.0/src/idpyoidc/server/claims/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from typing import Optional
 
 from idpyoidc import claims
 
 
 class Claims(claims.Claims):
-
     def get_base_url(self, configuration: dict):
-        _base = configuration.get('base_url')
+        _base = configuration.get("base_url")
         if not _base:
-            _base = configuration.get('issuer')
+            _base = configuration.get("issuer")
 
         return _base
 
     def get_id(self, configuration: dict):
-        return configuration.get('issuer')
+        return configuration.get("issuer")
 
-    def supported_to_preferred(self,
-                               supported: dict,
-                               base_url: Optional[str] = '',
-                               info: Optional[dict] = None):
+    def supported_to_preferred(
+        self, supported: dict, base_url: Optional[str] = "", info: Optional[dict] = None
+    ):
         # Add defaults
         for key, val in supported.items():
             if val is None:
                 continue
             if key not in self.prefer:
                 self.prefer[key] = val
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/claims/oauth2.py` & `idpyoidc-2.1.0/src/idpyoidc/server/claims/oauth2.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,17 +31,15 @@
         "op_policy_uri": None,
     }
 
     callback_path = {}
 
     callback_uris = ["redirect_uris"]
 
-    def __init__(self,
-                 prefer: Optional[dict] = None,
-                 callback_path: Optional[dict] = None):
+    def __init__(self, prefer: Optional[dict] = None, callback_path: Optional[dict] = None):
         claims.Claims.__init__(self, prefer=prefer, callback_path=callback_path)
 
     def provider_info(self, supports):
         _info = {}
         for key in ASConfigurationResponse.c_param.keys():
             _val = self.get_preference(key, supports.get(key, None))
             if _val and _val != []:
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/claims/oidc.py` & `idpyoidc-2.1.0/src/idpyoidc/server/claims/oidc.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     "id_token_signed_response_alg": "id_token_signing_alg_values_supported",
     "id_token_encrypted_response_alg": "id_token_encryption_alg_values_supported",
     "id_token_encrypted_response_enc": "id_token_encryption_enc_values_supported",
     "default_acr_values": "acr_values_supported",
     "subject_type": "subject_types_supported",
     "token_endpoint_auth_method": "token_endpoint_auth_methods_supported",
     "response_types": "response_types_supported",
+    "response_modes": "response_modes_supported",
     "grant_types": "grant_types_supported",
     # In OAuth2 but not in OIDC
     "scope": "scopes_supported",
     "token_endpoint_auth_signing_alg": "token_endpoint_auth_signing_alg_values_supported",
 }
 
 
@@ -53,47 +54,46 @@
         "initiate_login_uri": None,
         "jwks": None,
         "jwks_uri": None,
         "op_policy_uri": None,
         "require_auth_time": None,
         "scopes_supported": ["openid"],
         "service_documentation": None,
-        'subject_types_supported': ['public', 'pairwise', 'ephemeral'],
+        "subject_types_supported": ["public", "pairwise", "ephemeral"],
         "op_tos_uri": None,
         "ui_locales_supported": None,
         # "version": '3.0'
         #  "verify_args": None,
     }
 
     register2preferred = REGISTER2PREFERRED
 
-    def __init__(self,
-                 prefer: Optional[dict] = None,
-                 callback_path: Optional[dict] = None
-                 ):
+    def __init__(self, prefer: Optional[dict] = None, callback_path: Optional[dict] = None):
         server_claims.Claims.__init__(self, prefer=prefer, callback_path=callback_path)
 
-    def verify_rules(self):
+    def verify_rules(self, supports):
         if self.get_preference("request_parameter_supported") and self.get_preference(
-                "request_uri_parameter_supported"):
+            "request_uri_parameter_supported"
+        ):
             raise ValueError(
                 "You have to chose one of 'request_parameter_supported' and "
-                "'request_uri_parameter_supported'. You can't have both.")
+                "'request_uri_parameter_supported'. You can't have both."
+            )
 
-        if not self.get_preference('encrypt_userinfo_supported'):
-            self.set_preference('userinfo_encryption_alg_values_supported', [])
-            self.set_preference('userinfo_encryption_enc_values_supported', [])
-
-        if not self.get_preference('encrypt_request_object_supported'):
-            self.set_preference('request_object_encryption_alg_values_supported', [])
-            self.set_preference('request_object_encryption_enc_values_supported', [])
-
-        if not self.get_preference('encrypt_id_token_supported'):
-            self.set_preference('id_token_encryption_alg_values_supported', [])
-            self.set_preference('id_token_encryption_enc_values_supported', [])
+        if not self.get_preference("encrypt_userinfo_supported"):
+            self.set_preference("userinfo_encryption_alg_values_supported", [])
+            self.set_preference("userinfo_encryption_enc_values_supported", [])
+
+        if not self.get_preference("encrypt_request_object_supported"):
+            self.set_preference("request_object_encryption_alg_values_supported", [])
+            self.set_preference("request_object_encryption_enc_values_supported", [])
+
+        if not self.get_preference("encrypt_id_token_supported"):
+            self.set_preference("id_token_encryption_alg_values_supported", [])
+            self.set_preference("id_token_encryption_enc_values_supported", [])
 
     def provider_info(self, supports):
         _info = {}
         for key in ProviderConfigurationResponse.c_param.keys():
             _val = self.get_preference(key, supports.get(key, None))
             if _val not in [None, []]:
                 _info[key] = _val
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/client_authn.py` & `idpyoidc-2.1.0/src/idpyoidc/server/client_authn.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,34 +37,34 @@
     def __init__(self, upstream_get):
         """
         :param upstream_get: A method that can be used to get general server information.
         """
         self.upstream_get = upstream_get
 
     def _verify(
-            self,
-            request: Optional[Union[dict, Message]] = None,
-            authorization_token: Optional[str] = None,
-            endpoint=None,  # Optional[Endpoint]
-            **kwargs,
+        self,
+        request: Optional[Union[dict, Message]] = None,
+        authorization_token: Optional[str] = None,
+        endpoint=None,  # Optional[Endpoint]
+        **kwargs,
     ):
         """
         Verify authentication information in a request
         :param kwargs:
         :return:
         """
         raise NotImplementedError()
 
     def verify(
-            self,
-            request: Optional[Union[dict, Message]] = None,
-            authorization_token: Optional[str] = None,
-            endpoint=None,  # Optional[Endpoint]
-            get_client_id_from_token: Optional[Callable] = None,
-            **kwargs,
+        self,
+        request: Optional[Union[dict, Message]] = None,
+        authorization_token: Optional[str] = None,
+        endpoint=None,  # Optional[Endpoint]
+        get_client_id_from_token: Optional[Callable] = None,
+        **kwargs,
     ):
         """
         Verify authentication information in a request
         :param kwargs:
         :return:
         """
         res = self._verify(
@@ -74,17 +74,17 @@
             get_client_id_from_token=get_client_id_from_token,
             **kwargs,
         )
         res["method"] = self.tag
         return res
 
     def is_usable(
-            self,
-            request: Optional[Union[dict, Message]] = None,
-            authorization_token: Optional[str] = None,
+        self,
+        request: Optional[Union[dict, Message]] = None,
+        authorization_token: Optional[str] = None,
     ):
         """
         Verify that this authentication method is applicable.
 
         :param request: The request
         :param authorization_token: The authorization token
         :return: True/False
@@ -113,19 +113,19 @@
 
     tag = "none"
 
     def is_usable(self, request=None, authorization_token=None):
         return request is not None
 
     def _verify(
-            self,
-            request: Optional[Union[dict, Message]] = None,
-            authorization_token: Optional[str] = None,
-            endpoint=None,  # Optional[Endpoint]
-            **kwargs,
+        self,
+        request: Optional[Union[dict, Message]] = None,
+        authorization_token: Optional[str] = None,
+        endpoint=None,  # Optional[Endpoint]
+        **kwargs,
     ):
         return {"client_id": request.get("client_id")}
 
 
 class PublicAuthn(ClientAuthnMethod):
     """
     Used for public clients, that don't require any form of authentication other
@@ -134,19 +134,19 @@
 
     tag = "public"
 
     def is_usable(self, request=None, authorization_token=None):
         return request and "client_id" in request
 
     def _verify(
-            self,
-            request: Optional[Union[dict, Message]] = None,
-            authorization_token: Optional[str] = None,
-            endpoint=None,  # Optional[Endpoint]
-            **kwargs,
+        self,
+        request: Optional[Union[dict, Message]] = None,
+        authorization_token: Optional[str] = None,
+        endpoint=None,  # Optional[Endpoint]
+        **kwargs,
     ):
         return {"client_id": request["client_id"]}
 
 
 class ClientSecretBasic(ClientAuthnMethod):
     """
     Clients that have received a client_secret value from the Authorization
@@ -158,22 +158,22 @@
 
     def is_usable(self, request=None, authorization_token=None):
         if authorization_token is not None and authorization_token.startswith("Basic "):
             return True
         return False
 
     def _verify(
-            self,
-            request: Optional[Union[dict, Message]] = None,
-            authorization_token: Optional[str] = None,
-            endpoint=None,  # Optional[Endpoint]
-            **kwargs,
+        self,
+        request: Optional[Union[dict, Message]] = None,
+        authorization_token: Optional[str] = None,
+        endpoint=None,  # Optional[Endpoint]
+        **kwargs,
     ):
         client_info = basic_authn(authorization_token)
-        _context = self.upstream_get('context')
+        _context = self.upstream_get("context")
         if _context.cdb[client_info["id"]]["client_secret"] == client_info["secret"]:
             return {"client_id": client_info["id"]}
         else:
             raise ClientAuthenticationError()
 
 
 class ClientSecretPost(ClientSecretBasic):
@@ -190,21 +190,21 @@
         if request is None:
             return False
         if "client_id" in request and "client_secret" in request:
             return True
         return False
 
     def _verify(
-            self,
-            request: Optional[Union[dict, Message]] = None,
-            authorization_token: Optional[str] = None,
-            endpoint=None,  # Optional[Endpoint]
-            **kwargs,
+        self,
+        request: Optional[Union[dict, Message]] = None,
+        authorization_token: Optional[str] = None,
+        endpoint=None,  # Optional[Endpoint]
+        **kwargs,
     ):
-        _context = self.upstream_get('context')
+        _context = self.upstream_get("context")
         if _context.cdb[request["client_id"]]["client_secret"] == request["client_secret"]:
             return {"client_id": request["client_id"]}
         else:
             raise ClientAuthenticationError("secrets doesn't match")
 
 
 class BearerHeader(ClientSecretBasic):
@@ -214,23 +214,23 @@
 
     def is_usable(self, request=None, authorization_token=None):
         if authorization_token is not None and authorization_token.startswith("Bearer "):
             return True
         return False
 
     def _verify(
-            self,
-            request: Optional[Union[dict, Message]] = None,
-            authorization_token: Optional[str] = None,
-            endpoint=None,  # Optional[Endpoint]
-            get_client_id_from_token: Optional[Callable] = None,
-            **kwargs,
+        self,
+        request: Optional[Union[dict, Message]] = None,
+        authorization_token: Optional[str] = None,
+        endpoint=None,  # Optional[Endpoint]
+        get_client_id_from_token: Optional[Callable] = None,
+        **kwargs,
     ):
         token = authorization_token.split(" ", 1)[1]
-        _context = self.upstream_get('context')
+        _context = self.upstream_get("context")
         try:
             client_id = get_client_id_from_token(_context, token, request)
         except ToOld:
             raise BearerTokenAuthenticationError("Expired token")
         except KeyError:
             raise BearerTokenAuthenticationError("Unknown token")
         return {"token": token, "client_id": client_id}
@@ -245,66 +245,63 @@
 
     def is_usable(self, request=None, authorization_token=None):
         if request is not None and "access_token" in request:
             return True
         return False
 
     def _verify(
-            self,
-            request: Optional[Union[dict, Message]] = None,
-            authorization_token: Optional[str] = None,
-            endpoint=None,  # Optional[Endpoint]
-            get_client_id_from_token: Optional[Callable] = None,
-            **kwargs,
+        self,
+        request: Optional[Union[dict, Message]] = None,
+        authorization_token: Optional[str] = None,
+        endpoint=None,  # Optional[Endpoint]
+        get_client_id_from_token: Optional[Callable] = None,
+        **kwargs,
     ):
         _token = request.get("access_token")
         if _token is None:
             raise ClientAuthenticationError("No access token")
 
         res = {"token": _token}
-        _context = self.upstream_get('context')
+        _context = self.upstream_get("context")
         _client_id = get_client_id_from_token(_context, _token, request)
         if _client_id:
             res["client_id"] = _client_id
         return res
 
 
 class JWSAuthnMethod(ClientAuthnMethod):
-
     def is_usable(self, request=None, authorization_token=None):
         if request is None:
             return False
         if "client_assertion" in request:
             return True
         return False
 
     def _verify(
-            self,
-            request: Optional[Union[dict, Message]] = None,
-            authorization_token: Optional[str] = None,
-            endpoint=None,  # Optional[Endpoint]
-            key_type: Optional[str] = None,
-            **kwargs,
+        self,
+        request: Optional[Union[dict, Message]] = None,
+        authorization_token: Optional[str] = None,
+        endpoint=None,  # Optional[Endpoint]
+        key_type: Optional[str] = None,
+        **kwargs,
     ):
-        _context = self.upstream_get('context')
-        _keyjar = self.upstream_get('attribute', 'keyjar')
+        _context = self.upstream_get("context")
+        _keyjar = self.upstream_get("attribute", "keyjar")
         _jwt = JWT(_keyjar, msg_cls=JsonWebToken)
         try:
             ca_jwt = _jwt.unpack(request["client_assertion"])
         except (Invalid, MissingKey, BadSignature) as err:
             logger.info("%s" % sanitize(err))
             raise ClientAuthenticationError("Could not verify client_assertion.")
 
         _sign_alg = ca_jwt.jws_header.get("alg")
         if _sign_alg and _sign_alg.startswith("HS"):
             if key_type == "private_key":
                 raise AttributeError("Wrong key type")
-            keys = _keyjar.get(
-                "sig", "oct", ca_jwt["iss"], ca_jwt.jws_header.get("kid")
-            )
+            keys = _keyjar.get("sig", "oct", ca_jwt["iss"], ca_jwt.jws_header.get("kid"))
             _secret = _context.cdb[ca_jwt["iss"]].get("client_secret")
             if _secret and keys[0].key != as_bytes(_secret):
                 raise AttributeError("Oct key used for signing not client_secret")
         else:
             if key_type == "client_secret":
                 raise AttributeError("Wrong key type")
 
@@ -344,19 +341,19 @@
     The HMAC (Hash-based Message Authentication Code) is calculated using the
     bytes of the UTF-8 representation of the client_secret as the shared key.
     """
 
     tag = "client_secret_jwt"
 
     def _verify(
-            self,
-            request: Optional[Union[dict, Message]] = None,
-            authorization_token: Optional[str] = None,
-            endpoint=None,  # Optional[Endpoint]
-            **kwargs,
+        self,
+        request: Optional[Union[dict, Message]] = None,
+        authorization_token: Optional[str] = None,
+        endpoint=None,  # Optional[Endpoint]
+        **kwargs,
     ):
         res = super()._verify(
             request=request, key_type="client_secret", endpoint=endpoint, **kwargs
         )
         # Verify that a HS alg was used
         return res
 
@@ -365,19 +362,19 @@
     """
     Clients that have registered a public key sign a JWT using that key.
     """
 
     tag = "private_key_jwt"
 
     def _verify(
-            self,
-            request: Optional[Union[dict, Message]] = None,
-            authorization_token: Optional[str] = None,
-            endpoint=None,  # Optional[Endpoint]
-            **kwargs,
+        self,
+        request: Optional[Union[dict, Message]] = None,
+        authorization_token: Optional[str] = None,
+        endpoint=None,  # Optional[Endpoint]
+        **kwargs,
     ):
         res = super()._verify(
             request=request,
             authorization_token=authorization_token,
             endpoint=endpoint,
             **kwargs,
             key_type="private_key",
@@ -390,22 +387,22 @@
     tag = "request_param"
 
     def is_usable(self, request=None, authorization_token=None):
         if request and "request" in request:
             return True
 
     def _verify(
-            self,
-            request: Optional[Union[dict, Message]] = None,
-            authorization_token: Optional[str] = None,
-            endpoint=None,  # Optional[Endpoint]
-            **kwargs,
+        self,
+        request: Optional[Union[dict, Message]] = None,
+        authorization_token: Optional[str] = None,
+        endpoint=None,  # Optional[Endpoint]
+        **kwargs,
     ):
-        _context = self.upstream_get('context')
-        _jwt = JWT(self.upstream_get('attribute', 'keyjar'), msg_cls=JsonWebToken)
+        _context = self.upstream_get("context")
+        _jwt = JWT(self.upstream_get("attribute", "keyjar"), msg_cls=JsonWebToken)
         try:
             _jwt = _jwt.unpack(request["request"])
         except (Invalid, MissingKey, BadSignature) as err:
             logger.info("%s" % sanitize(err))
             raise ClientAuthenticationError("Could not verify client_assertion.")
 
         # If there is a jti use it to make sure one-time usage is true
@@ -442,19 +439,20 @@
     eta = cinfo.get("client_secret_expires_at", 0)
     if eta != 0 and eta < utc_time_sans_frac():
         return False
     return True
 
 
 def verify_client(
-        request: Union[dict, Message],
-        http_info: Optional[dict] = None,
-        get_client_id_from_token: Optional[Callable] = None,
-        endpoint=None,  # Optional[Endpoint]
-        also_known_as: Optional[Dict[str, str]] = None,
+    request: Union[dict, Message],
+    http_info: Optional[dict] = None,
+    get_client_id_from_token: Optional[Callable] = None,
+    endpoint=None,  # Optional[Endpoint]
+    also_known_as: Optional[Dict[str, str]] = None,
+    **kwargs,
 ) -> dict:
     """
     Initiated Guessing !
 
     :param also_known_as:
     :param endpoint: Endpoint instance
     :param context: EndpointContext instance
@@ -469,29 +467,29 @@
         authorization_token = http_info["headers"].get("authorization")
         if not authorization_token:
             authorization_token = http_info["headers"].get("Authorization")
     else:
         authorization_token = None
 
     auth_info = {}
-    _context = endpoint.upstream_get('context')
+    _context = endpoint.upstream_get("context")
     methods = _context.client_authn_methods
     client_id = None
     allowed_methods = getattr(endpoint, "client_authn_method")
     if not allowed_methods:
         allowed_methods = list(methods.keys())  # If not specific for this endpoint then all
 
     _method = None
     for _method in (methods[meth] for meth in allowed_methods):
         if not _method.is_usable(request=request, authorization_token=authorization_token):
             continue
         try:
             logger.info(f"Verifying client authentication using {_method.tag}")
             auth_info = _method.verify(
-                keyjar=endpoint.upstream_get('attribute', 'keyjar'),
+                keyjar=endpoint.upstream_get("attribute", "keyjar"),
                 request=request,
                 authorization_token=authorization_token,
                 endpoint=endpoint,
                 get_client_id_from_token=get_client_id_from_token,
             )
         except (BearerTokenAuthenticationError, ClientAuthenticationError):
             raise
@@ -506,18 +504,25 @@
         if client_id is None:
             raise ClientAuthenticationError("Failed to verify client")
 
         if also_known_as:
             client_id = also_known_as[client_id]
             auth_info["client_id"] = client_id
 
-        if client_id not in _context.cdb:
-            raise UnknownClient("Unknown Client ID")
+        _get_client_info = kwargs.get("get_client_info")
+        if _get_client_info:
+            _cinfo = _get_client_info(client_id, _context)
+        else:
+            try:
+                _cinfo = _context.cdb[client_id]
+            except KeyError:
+                raise UnknownClient("Unknown Client ID")
 
-        _cinfo = _context.cdb[client_id]
+        if not _cinfo:
+            raise UnknownClient("Unknown Client ID")
 
         if not valid_client_info(_cinfo):
             logger.warning("Client registration has timed out or " "client secret is expired.")
             raise InvalidClient("Not valid client")
 
         # Validate that the used method is allowed for this client/endpoint
         client_allowed_methods = _cinfo.get(
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/client_configure.py` & `idpyoidc-2.1.0/src/idpyoidc/server/client_configure.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/configure.py` & `idpyoidc-2.1.0/src/idpyoidc/server/configure.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,24 +3,22 @@
 import logging
 import os
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 
+from idpyoidc.client.defaults import OAUTH2_SERVER_METADATA_URL
 from idpyoidc.configure import Base
 from idpyoidc.server.client_configure import verify_oidc_client_information
 from idpyoidc.server.scopes import SCOPE2CLAIMS
 
 logger = logging.getLogger(__name__)
 
-OP_DEFAULT_CONFIG = {
-    "preference": {
-        "subject_types_supported": ["public", "pairwise"],
-    },
+_DEFAULT_CONFIG = {
     "cookie_handler": {
         "class": "idpyoidc.server.cookie_handler.CookieHandler",
         "kwargs": {
             "encrypter": {
                 "kwargs": {
                     "keys": {
                         "private_path": "private/cookie_jwks.json",
@@ -35,39 +33,119 @@
             "name": {
                 "session": "oidc_op",
                 "register": "oidc_op_rp",
                 "session_management": "sman",
             },
         },
     },
-    "claims_interface": {"class": "idpyoidc.server.session.claims.ClaimsInterface", "kwargs": {}},
+    "claims_interface": {
+        "class": "idpyoidc.server.session.claims.ClaimsInterface",
+        "kwargs": {}
+    },
+    "httpc_params": {"verify": False, "timeout": 4},
+    "issuer": "https://{domain}:{port}",
+    "template_dir": "templates"
+}
+
+AS_DEFAULT_CONFIG = copy.deepcopy(_DEFAULT_CONFIG)
+_C = {
+    "authz": {
+        "class": "idpyoidc.server.authz.AuthzHandling",
+        "kwargs": {
+            "grant_config": {
+                "usage_rules": {
+                    "authorization_code": {
+                        "supports_minting": ["access_token", "refresh_token"],
+                        "max_usage": 1,
+                        "expires_in": 120  # 2 minutes
+                    },
+                    "access_token": {"expires_in": 3600},  # An hour
+                    "refresh_token": {
+                        "supports_minting": ["access_token", "refresh_token"],
+                        "expires_in": 86400,  # One day
+                    },
+                },
+                "expires_in": 2592000,  # a month, 30 days
+            }
+        }
+    },
+    "claims_interface": {
+        "class": "idpyoidc.server.session.claims.ClaimsInterface",
+        "kwargs": {
+            "claims_release_points": ["introspection", "access_token"]
+        }
+    },
+    "endpoint": {
+        "provider_info": {
+            "path": OAUTH2_SERVER_METADATA_URL[3:],
+            "class": "idpyoidc.server.oauth2.server_metadata.ServerMetadata",
+            "kwargs": {"client_authn_method": None},
+        },
+        "authorization": {
+            "path": "authorization",
+            "class": "idpyoidc.server.oauth2.authorization.Authorization",
+            "kwargs": {
+                "client_authn_method": None,
+                "claims_parameter_supported": True,
+                "request_parameter_supported": True,
+                "request_uri_parameter_supported": True,
+                "response_types_supported": ["code"],
+                "response_modes_supported": ["query", "fragment", "form_post"],
+            },
+        },
+        "token": {
+            "path": "token",
+            "class": "idpyoidc.server.oauth2.token.Token",
+            "kwargs": {
+                "client_authn_method": [
+                    "client_secret_post",
+                    "client_secret_basic",
+                    "client_secret_jwt",
+                    "private_key_jwt",
+                ]
+            }
+        }
+    }
+}
+
+AS_DEFAULT_CONFIG.update(_C)
+
+OP_DEFAULT_CONFIG = copy.deepcopy(_DEFAULT_CONFIG)
+OP_DEFAULT_CONFIG.update({
+    "preference": {
+        "subject_types_supported": ["public", "pairwise"],
+    },
     "authz": {
         "class": "idpyoidc.server.authz.AuthzHandling",
         "kwargs": {
             "grant_config": {
                 "usage_rules": {
                     "authorization_code": {
                         "supports_minting": [
                             "access_token",
                             "refresh_token",
                             "id_token",
                         ],
                         "max_usage": 1,
+                        'expires_in': 120  # 2 minutes
                     },
-                    "access_token": {},
+                    "access_token": {'expires_in': 3600},  # An hour
                     "refresh_token": {
-                        "supports_minting": ["access_token", "refresh_token"],
-                        "expires_in": -1,
+                        "supports_minting": ["access_token", "refresh_token", "id_token"],
+                        "expires_in": 86400,  # One day
                     },
                 },
-                "expires_in": 43200,
+                "expires_in": 2592000,  # a month, 30 days
             }
         },
     },
-    "httpc_params": {"verify": False, "timeout": 4},
+    "claims_interface": {
+        "class": "idpyoidc.server.session.claims.ClaimsInterface",
+        "kwargs": {}
+    },
     "endpoint": {
         "provider_info": {
             "path": ".well-known/openid-configuration",
             "class": "idpyoidc.server.oidc.provider_config.ProviderConfiguration",
             "kwargs": {"client_authn_method": None},
         },
         "authorization": {
@@ -76,20 +154,20 @@
             "kwargs": {
                 "client_authn_method": None,
                 "claims_parameter_supported": True,
                 "request_parameter_supported": True,
                 "request_uri_parameter_supported": True,
                 "response_types_supported": [
                     "code",
-                    "token",
+                    # "token",
                     "id_token",
-                    "code token",
+                    # "code token",
                     "code id_token",
-                    "id_token token",
-                    "code id_token token",
+                    # "id_token token",
+                    # "code id_token token",
                     # "none"
                 ],
                 "response_modes_supported": ["query", "fragment", "form_post"],
             },
         },
         "token": {
             "path": "token",
@@ -105,37 +183,30 @@
         },
         "userinfo": {
             "path": "userinfo",
             "class": "idpyoidc.server.oidc.userinfo.UserInfo",
             "kwargs": {"claim_types_supported": ["normal", "aggregated", "distributed"]},
         },
     },
-    "issuer": "https://{domain}:{port}",
-    "template_dir": "templates",
     "token_handler_args": {
         "jwks_file": "private/token_jwks.json",
         "code": {"kwargs": {"lifetime": 600}},
         "token": {
             "class": "idpyoidc.server.token.jwt_token.JWTToken",
             "kwargs": {"lifetime": 3600},
         },
         "refresh": {
             "class": "idpyoidc.server.token.jwt_token.JWTToken",
             "kwargs": {"lifetime": 86400},
         },
         "id_token": {"class": "idpyoidc.server.token.id_token.IDToken", "kwargs": {}},
     },
     "scopes_to_claims": SCOPE2CLAIMS,
-}
+})
 
-AS_DEFAULT_CONFIG = copy.deepcopy(OP_DEFAULT_CONFIG)
-AS_DEFAULT_CONFIG["claims_interface"] = {
-    "class": "idpyoidc.server.session.claims.OAuth2ClaimsInterface",
-    "kwargs": {},
-}
 
 
 class EntityConfiguration(Base):
     default_config = AS_DEFAULT_CONFIG
     uris = ["issuer", "base_url"]
     parameter = {
         "add_on": None,
@@ -147,32 +218,32 @@
         "client_db": None,
         "client_authn_methods": {},
         "cookie_handler": None,
         "endpoint": {},
         "httpc_params": {},
         "issuer": "",
         "key_conf": None,
-        'preference': {},
+        "preference": {},
         "session_params": None,
         "template_dir": None,
         "token_handler_args": {},
         "userinfo": None,
-        "scopes_handler": None
+        "scopes_handler": None,
     }
 
     def __init__(
-        self,
-        conf: Dict,
-        base_path: Optional[str] = "",
-        entity_conf: Optional[List[dict]] = None,
-        domain: Optional[str] = "",
-        port: Optional[int] = 0,
-        file_attributes: Optional[List[str]] = None,
-        dir_attributes: Optional[List[str]] = None,
-        upstream_get: Optional[Callable] = None
+            self,
+            conf: Dict,
+            base_path: Optional[str] = "",
+            entity_conf: Optional[List[dict]] = None,
+            domain: Optional[str] = "",
+            port: Optional[int] = 0,
+            file_attributes: Optional[List[str]] = None,
+            dir_attributes: Optional[List[str]] = None,
+            upstream_get: Optional[Callable] = None,
     ):
 
         conf = copy.deepcopy(conf)
         Base.__init__(
             self,
             conf,
             base_path,
@@ -228,22 +299,22 @@
             "oidc_clients": {},
             "sub_func": {},
             "scopes_to_claims": {},
         }
     )
 
     def __init__(
-        self,
-        conf: Dict,
-        base_path: Optional[str] = "",
-        entity_conf: Optional[List[dict]] = None,
-        domain: Optional[str] = "",
-        port: Optional[int] = 0,
-        file_attributes: Optional[List[str]] = None,
-        dir_attributes: Optional[List[str]] = None,
+            self,
+            conf: Dict,
+            base_path: Optional[str] = "",
+            entity_conf: Optional[List[dict]] = None,
+            domain: Optional[str] = "",
+            port: Optional[int] = 0,
+            file_attributes: Optional[List[str]] = None,
+            dir_attributes: Optional[List[str]] = None,
     ):
         super().__init__(
             conf=conf,
             base_path=base_path,
             entity_conf=entity_conf,
             domain=domain,
             port=port,
@@ -252,22 +323,22 @@
         )
 
 
 class ASConfiguration(EntityConfiguration):
     "Authorization server configuration"
 
     def __init__(
-        self,
-        conf: Dict,
-        base_path: Optional[str] = "",
-        entity_conf: Optional[List[dict]] = None,
-        domain: Optional[str] = "",
-        port: Optional[int] = 0,
-        file_attributes: Optional[List[str]] = None,
-        dir_attributes: Optional[List[str]] = None,
+            self,
+            conf: Dict,
+            base_path: Optional[str] = "",
+            entity_conf: Optional[List[dict]] = None,
+            domain: Optional[str] = "",
+            port: Optional[int] = 0,
+            file_attributes: Optional[List[str]] = None,
+            dir_attributes: Optional[List[str]] = None,
     ):
         EntityConfiguration.__init__(
             self,
             conf=conf,
             base_path=base_path,
             entity_conf=entity_conf,
             domain=domain,
@@ -276,15 +347,15 @@
             dir_attributes=dir_attributes,
         )
 
 
 DEFAULT_EXTENDED_CONF = {
     "add_on": {
         "pkce": {
-            "function": "idpyoidc.server.oidc.add_on.pkce.add_pkce_support",
+            "function": "idpyoidc.server.oauth2.add_on.pkce.add_support",
             "kwargs": {"essential": False, "code_challenge_method": "S256 S384 S512"},
         },
         "claims": {
             "function": "idpyoidc.server.oidc.add_on.custom_scopes.add_custom_scopes",
             "kwargs": {
                 "research_and_scholarship": [
                     "name",
@@ -345,17 +416,15 @@
         "grant_types_supported": [
             "authorization_code",
             # "implicit",
             "urn:ietf:params:oauth:grant-type:jwt-bearer",
             "refresh_token",
         ],
     },
-    "scopes_handler": {
-        "class": "idpyoidc.server.scopes.Scopes"
-    },
+    "scopes_handler": {"class": "idpyoidc.server.scopes.Scopes"},
     "claims_interface": {"class": "idpyoidc.server.session.claims.ClaimsInterface", "kwargs": {}},
     "cookie_handler": {
         "class": "idpyoidc.server.cookie_handler.CookieHandler",
         "kwargs": {
             "encrypter": {
                 "kwargs": {
                     "keys": {
@@ -413,20 +482,20 @@
             "kwargs": {
                 "client_authn_method": None,
                 "claims_parameter_supported": True,
                 "request_parameter_supported": True,
                 "request_uri_parameter_supported": True,
                 "response_types_supported": [
                     "code",
-                    "token",
+                    # "token",
                     "id_token",
-                    "code token",
+                    # "code token",
                     "code id_token",
-                    "id_token token",
-                    "code id_token token",
+                    # "id_token token",
+                    # "code id_token token",
                     # "none"
                 ],
                 "response_modes_supported": ["query", "fragment", "form_post"],
             },
         },
         "token": {
             "path": "token",
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/construct.py` & `idpyoidc-2.1.0/src/idpyoidc/server/construct.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/cookie_handler.py` & `idpyoidc-2.1.0/src/idpyoidc/server/cookie_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,17 +140,15 @@
                 bytes_timestamp,
                 base64.b64encode(iv),
                 base64.b64encode(ctx),
                 base64.b64encode(tag),
             ]
         elif self.crypt:
             msg = lv_pack(timestamp, payload)
-            cookie_payload = [
-                bytes_timestamp,
-                base64.b64encode(self.crypt.encrypt(msg.encode()))]
+            cookie_payload = [bytes_timestamp, base64.b64encode(self.crypt.encrypt(msg.encode()))]
         else:
             cookie_payload = [bytes_timestamp, bytes_load, base64.b64encode(mac)]
 
         return (b"|".join(cookie_payload)).decode("utf-8")
 
     def _ver_dec_content(self, parts):
         """
@@ -165,15 +163,15 @@
         elif len(parts) == 2:
             t0, enc_payload = parts
             if not self.crypt:
                 raise VerificationError("Can not decrypt")
             msg = self.crypt.decrypt(base64.b64decode(as_bytes(enc_payload)))
             t1, payload = lv_unpack(msg.decode("utf-8"))
             if t0 != t1:
-                raise VerificationError('Suspicious timestamp')
+                raise VerificationError("Suspicious timestamp")
             return payload, t1
         elif len(parts) == 3:
             # verify the cookie signature
             timestamp, payload, b64_mac = parts
             mac = base64.b64decode(b64_mac)
             verifier = HMACSigner(algorithm=self.sign_alg)
             if verifier.verify(
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/endpoint.py` & `idpyoidc-2.1.0/src/idpyoidc/server/endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,38 +166,43 @@
             if lap:
                 return self.error_cls(error=err)
             client_id = self.find_client_keys(err.args[0])
             if not client_id:
                 return self.error_cls(error=err)
             else:
                 # Fund a client ID I believe will work
-                self.verify_request(request=request, keyjar=keyjar, client_id=client_id,
-                                    verify_args=verify_args, lap=1)
+                self.verify_request(
+                    request=request,
+                    keyjar=keyjar,
+                    client_id=client_id,
+                    verify_args=verify_args,
+                    lap=1,
+                )
         return None
 
     def parse_request(
-            self,
-            request: Union[Message, dict, str],
-            http_info: Optional[dict] = None,
-            verify_args: Optional[dict] = None,
-            **kwargs
+        self,
+        request: Union[Message, dict, str],
+        http_info: Optional[dict] = None,
+        verify_args: Optional[dict] = None,
+        **kwargs
     ):
         """
 
         :param request: The request the server got
         :param http_info: HTTP information in connection with the request.
             This is a dictionary with keys: headers, url, cookies.
         :param kwargs: extra keyword arguments
         :return:
         """
         LOGGER.debug("- {} -".format(self.endpoint_name))
         LOGGER.info("Request: %s" % sanitize(request))
 
         _context = self.upstream_get("context")
-        _keyjar = self.upstream_get('attribute', 'keyjar')
+        _keyjar = self.upstream_get("attribute", "keyjar")
 
         if http_info is None:
             http_info = {}
 
         if request:
             if isinstance(request, (dict, Message)):
                 req = self.request_cls(**request)
@@ -222,25 +227,26 @@
 
         # Verify that the client is allowed to do this
         auth_info = self.client_authentication(req, http_info, endpoint=self, **kwargs)
 
         if "client_id" in auth_info:
             req["client_id"] = auth_info["client_id"]
 
-            _auth_method = auth_info.get('method')
-            if _auth_method and _auth_method not in ['public', 'none']:
-                req['authenticated'] = True
+            _auth_method = auth_info.get("method")
+            if _auth_method and _auth_method not in ["public", "none"]:
+                req["authenticated"] = True
 
             _client_id = auth_info["client_id"]
         else:
             _client_id = req.get("client_id")
 
         # verify that the request message is correct, may have to do it twice
-        err_response = self.verify_request(request=req, keyjar=_keyjar, client_id=_client_id,
-                                           verify_args=verify_args)
+        err_response = self.verify_request(
+            request=req, keyjar=_keyjar, client_id=_client_id, verify_args=verify_args
+        )
         if err_response:
             return err_response
 
         LOGGER.info("Parsed and verified request: %s" % sanitize(req))
 
         # Do any endpoint specific parsing
         return self.do_post_parse_request(
@@ -259,78 +265,74 @@
         if "endpoint" not in kwargs:
             kwargs["endpoint"] = self
 
         get_client_id_from_token = kwargs.get("get_client_id_from_token")
         if not get_client_id_from_token:
             kwargs["get_client_id_from_token"] = getattr(self, "get_client_id_from_token", None)
 
-        authn_info = verify_client(
-            request=request,
-            http_info=http_info,
-            **kwargs
-        )
+        authn_info = verify_client(request=request, http_info=http_info, **kwargs)
 
         LOGGER.debug("authn_info: %s", authn_info)
         if authn_info == {} and self.client_authn_method and len(self.client_authn_method):
             LOGGER.debug("client_authn_method: %s", self.client_authn_method)
             raise UnAuthorizedClient("Authorization failed")
         if "client_id" not in authn_info and authn_info.get("method") != "none":
             raise UnAuthorizedClient("Authorization failed")
         return authn_info
 
     def do_post_parse_request(
-            self, request: Message, client_id: Optional[str] = "", **kwargs
+        self, request: Message, client_id: Optional[str] = "", **kwargs
     ) -> Message:
         _context = self.upstream_get("context")
         for meth in self.post_parse_request:
             if isinstance(request, self.error_cls):
                 break
             request = meth(request, client_id, context=_context, **kwargs)
         return request
 
     def do_pre_construct(
-            self, response_args: dict, request: Optional[Union[Message, dict]] = None, **kwargs
+        self, response_args: dict, request: Optional[Union[Message, dict]] = None, **kwargs
     ) -> dict:
         _context = self.upstream_get("context")
         for meth in self.pre_construct:
             response_args = meth(response_args, request, context=_context, **kwargs)
 
         return response_args
 
     def do_post_construct(
-            self,
-            response_args: Union[Message, dict],
-            request: Optional[Union[Message, dict]] = None,
-            **kwargs
+        self,
+        response_args: Union[Message, dict],
+        request: Optional[Union[Message, dict]] = None,
+        **kwargs
     ) -> dict:
         _context = self.upstream_get("context")
         for meth in self.post_construct:
             response_args = meth(response_args, request, context=_context, **kwargs)
 
         return response_args
 
     def process_request(
-            self,
-            request: Optional[Union[Message, dict]] = None,
-            http_info: Optional[dict] = None,
-            **kwargs
+        self,
+        request: Optional[Union[Message, dict]] = None,
+        http_info: Optional[dict] = None,
+        **kwargs
     ) -> Union[Message, dict]:
         """
 
         :param http_info: Information on the HTTP request
         :param request: The request, can be in a number of formats
         :return: Arguments for the do_response method
         """
         return {}
 
     def construct(
-            self,
-            response_args: Optional[dict] = None,
-            request: Optional[Union[Message, dict]] = None,
-            **kwargs
+        self,
+        response_args: Optional[dict] = None,
+        request: Optional[Union[Message, dict]] = None,
+        **kwargs
     ):
         """
         Construct the response
 
         :param response_args: response arguments
         :param request: The parsed request, a self.request_cls class instance
         :param kwargs: Extra keyword arguments
@@ -340,27 +342,27 @@
 
         # LOGGER.debug("kwargs: %s" % sanitize(kwargs))
         response = self.response_cls(**response_args)
 
         return self.do_post_construct(response, request, **kwargs)
 
     def response_info(
-            self,
-            response_args: Optional[dict] = None,
-            request: Optional[Union[Message, dict]] = None,
-            **kwargs
+        self,
+        response_args: Optional[dict] = None,
+        request: Optional[Union[Message, dict]] = None,
+        **kwargs
     ) -> dict:
         return self.construct(response_args, request, **kwargs)
 
     def do_response(
-            self,
-            response_args: Optional[dict] = None,
-            request: Optional[Union[Message, dict]] = None,
-            error: Optional[str] = "",
-            **kwargs
+        self,
+        response_args: Optional[dict] = None,
+        request: Optional[Union[Message, dict]] = None,
+        error: Optional[str] = "",
+        **kwargs
     ) -> dict:
         """
         :param response_args: Information to use when constructing the response
         :param request: The original request
         :param error: Possible error encountered while processing the request
         """
         do_placement = True
@@ -387,14 +389,16 @@
             if content_type is None:
                 if self.response_content_type:
                     content_type = self.response_content_type
                 elif self.response_format == "json":
                     content_type = "application/json"
                 elif self.response_format in ["jws", "jwe", "jose"]:
                     content_type = "application/jose"
+                elif self.response_format == "text":
+                    content_type = "text/plain"
                 else:
                     content_type = "application/x-www-form-urlencoded"
         else:
             _response = self.response_info(response_args, request, **kwargs)
 
         if do_placement:
             content_type = kwargs.get("content_type")
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/endpoint_context.py` & `idpyoidc-2.1.0/src/idpyoidc/server/endpoint_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,27 +98,27 @@
         "sso_ttl": None,
         "symkey": "",
         "token_args_methods": [],
         # "userinfo": UserInfo,
         "client_authn_method": {},
     }
 
-    init_args = ['upstream_get', 'handler']
+    init_args = ["upstream_get", "handler"]
 
     def __init__(
-            self,
-            conf: Union[dict, OPConfiguration],
-            upstream_get: Callable,
-            cwd: Optional[str] = "",
-            cookie_handler: Optional[Any] = None,
-            httpc: Optional[Any] = None,
-            server_type: Optional[str] = '',
-            entity_id: Optional[str] = "",
-            keyjar: Optional[KeyJar] = None,
-            claims_class: Optional[Claims] = None
+        self,
+        conf: Union[dict, OPConfiguration],
+        upstream_get: Callable,
+        cwd: Optional[str] = "",
+        cookie_handler: Optional[Any] = None,
+        httpc: Optional[Any] = None,
+        server_type: Optional[str] = "",
+        entity_id: Optional[str] = "",
+        keyjar: Optional[KeyJar] = None,
+        claims_class: Optional[Claims] = None,
     ):
         _id = entity_id or conf.get("issuer", "")
         OidcContext.__init__(self, conf, entity_id=_id)
         self.conf = conf
         self.upstream_get = upstream_get
 
         if claims_class:
@@ -236,15 +236,15 @@
             self.claims_interface = init_service(_interface, self.upstream_get)
 
         if isinstance(conf, OPConfiguration):
             conf = conf.conf
         _supports = self.supports()
         self.keyjar = self.claims.load_conf(conf, supports=_supports, keyjar=keyjar)
         self.provider_info = self.claims.provider_info(_supports)
-        self.provider_info['issuer'] = self.issuer
+        self.provider_info["issuer"] = self.issuer
         self.provider_info.update(self._get_endpoint_info())
 
         # INTERFACES
 
         self.authz = self.setup_authz()
 
         self.setup_authentication()
@@ -312,15 +312,18 @@
             self.scopes_handler = Scopes(
                 self.upstream_get,
                 allowed_scopes=self.conf.get("allowed_scopes"),
                 scopes_to_claims=self.conf.get("scopes_to_claims"),
             )
 
     def do_add_on(self, endpoints):
-        _add_on_conf = self.conf.get("add_on")
+        _add_on_conf = self.conf.get("add_ons", self.conf.get("add_on"))
+        if not _add_on_conf:
+            _add_on_conf = self.conf.conf.get("add_ons")
+
         if _add_on_conf:
             for spec in _add_on_conf.values():
                 if isinstance(spec["function"], str):
                     _func = importer(spec["function"])
                 else:
                     _func = spec["function"]
                 _func(endpoints, **spec["kwargs"])
@@ -395,29 +398,29 @@
 
             self.login_hint_lookup = init_service(_conf)
             self.login_hint_lookup.userinfo = _userinfo
 
     def supports(self):
         res = {}
         if self.upstream_get:
-            for endpoint in self.upstream_get('endpoints').values():
+            for endpoint in self.upstream_get("endpoints").values():
                 res.update(endpoint.supports())
         res.update(self.claims.supports())
         return res
 
     def set_provider_info(self):
         _info = self.claims.provider_info(self.supports())
-        _info.update({'issuer': self.issuer, 'version': "3.0"})
+        _info.update({"issuer": self.issuer, "version": "3.0"})
 
-        for endp in self.upstream_get('endpoints').values():
+        for endp in self.upstream_get("endpoints").values():
             if endp.endpoint_name:
                 _info[endp.endpoint_name] = endp.full_path
 
         # acr_values
-        if 'acr_values_supported' not in _info:
+        if "acr_values_supported" not in _info:
             if self.authn_broker:
                 acr_values = self.authn_broker.get_acr_values()
                 if acr_values is not None:
                     _info["acr_values_supported"] = acr_values
 
         self.provider_info = _info
 
@@ -480,11 +483,11 @@
 
     def map_supported_to_preferred(self):
         self.claims.supported_to_preferred(self.supports())
         return self.claims.prefer
 
     def _get_endpoint_info(self):
         _res = {}
-        for name, endp in self.upstream_get('endpoints').items():
+        for name, endp in self.upstream_get("endpoints").items():
             if endp.endpoint_name:
                 _res[endp.endpoint_name] = endp.full_path
         return _res
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/exception.py` & `idpyoidc-2.1.0/src/idpyoidc/server/exception.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,7 +124,11 @@
 
 class MultipleCodeUsage(OidcEndpointError):
     pass
 
 
 class InvalidBranchID(OidcEndpointError):
     pass
+
+
+class ClientGrantMismatch(OidcEndpointError):
+    pass
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/login_hint.py` & `idpyoidc-2.1.0/src/idpyoidc/server/login_hint.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/oauth2/add_on/dpop.py` & `idpyoidc-2.1.0/src/idpyoidc/server/oauth2/add_on/dpop.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,41 @@
+import logging
+from hashlib import sha256
+from typing import Callable
 from typing import Optional
+from typing import Union
 
-from cryptojwt import JWS
 from cryptojwt import as_unicode
+from cryptojwt import JWS
 from cryptojwt.jwk.jwk import key_from_jwk_dict
 from cryptojwt.jws.jws import factory
 
+from idpyoidc.claims import get_signing_algs
+from idpyoidc.message import Message
+from idpyoidc.message import SINGLE_OPTIONAL_STRING
 from idpyoidc.message import SINGLE_REQUIRED_INT
 from idpyoidc.message import SINGLE_REQUIRED_JSON
 from idpyoidc.message import SINGLE_REQUIRED_STRING
-from idpyoidc.message import Message
-from idpyoidc.server.client_authn import ClientAuthnMethod
-from idpyoidc.server.client_authn import basic_authn
-from idpyoidc.server.exception import ClientAuthenticationError
+from idpyoidc.server.client_authn import BearerHeader
+
+logger = logging.getLogger(__name__)
 
 
 class DPoPProof(Message):
     c_param = {
         # header
         "typ": SINGLE_REQUIRED_STRING,
         "alg": SINGLE_REQUIRED_STRING,
         "jwk": SINGLE_REQUIRED_JSON,
         # body
         "jti": SINGLE_REQUIRED_STRING,
         "htm": SINGLE_REQUIRED_STRING,
         "htu": SINGLE_REQUIRED_STRING,
         "iat": SINGLE_REQUIRED_INT,
+        "ath": SINGLE_OPTIONAL_STRING,
     }
     header_params = {"typ", "alg", "jwk"}
     body_params = {"jti", "htm", "htu", "iat"}
 
     def __init__(self, set_defaults=True, **kwargs):
         self.key = None
         Message.__init__(self, set_defaults=set_defaults, **kwargs)
@@ -80,15 +87,15 @@
                 raise Exception()
 
             return self
         else:
             return None
 
 
-def post_parse_request(request, client_id, context, **kwargs):
+def token_post_parse_request(request, client_id, context, **kwargs):
     """
     Expect http_info attribute in kwargs. http_info should be a dictionary
     containing HTTP information.
 
     :param request:
     :param client_id:
     :param context:
@@ -115,14 +122,55 @@
         _dpop.key = key_from_jwk_dict(_dpop["jwk"])
 
     # Need something I can add as a reference when minting tokens
     request["dpop_jkt"] = as_unicode(_dpop.key.thumbprint("SHA-256"))
     return request
 
 
+def userinfo_post_parse_request(request, client_id, context, auth_info, **kwargs):
+    """
+    Expect http_info attribute in kwargs. http_info should be a dictionary
+    containing HTTP information.
+
+    :param request:
+    :param client_id:
+    :param context:
+    :param kwargs:
+    :return:
+    """
+
+    _http_info = kwargs.get("http_info")
+    if not _http_info:
+        return request
+
+    _dpop = DPoPProof().verify_header(_http_info["headers"]["dpop"])
+
+    # The signature of the JWS is verified, now for checking the
+    # content
+
+    if _dpop["htu"] != _http_info["url"]:
+        raise ValueError("htu in DPoP does not match the HTTP URI")
+
+    if _dpop["htm"] != _http_info["method"]:
+        raise ValueError("htm in DPoP does not match the HTTP method")
+
+    if not _dpop.key:
+        _dpop.key = key_from_jwk_dict(_dpop["jwk"])
+
+    ath = sha256(auth_info["token"].encode("utf8")).hexdigest()
+
+    if _dpop["ath"] != ath:
+        raise ValueError("'ath' in DPoP does not match the token hash")
+
+    # Need something I can add as a reference when minting tokens
+    request["dpop_jkt"] = as_unicode(_dpop.key.thumbprint("SHA-256"))
+    logger.debug("DPoP verified")
+    return request
+
+
 def token_args(context, client_id, token_args: Optional[dict] = None):
     dpop_jkt = context.cdb[client_id]["dpop_jkt"]
     _jkt = list(dpop_jkt.keys())[0]
     if "dpop_jkt" in context.cdb[client_id]:
         if token_args is None:
             token_args = {"cnf": {"jkt": _jkt}}
         else:
@@ -130,39 +178,57 @@
 
     return token_args
 
 
 def add_support(endpoint: dict, **kwargs):
     #
     _token_endp = endpoint["token"]
-    _token_endp.post_parse_request.append(post_parse_request)
+    _token_endp.post_parse_request.append(token_post_parse_request)
 
     _algs_supported = kwargs.get("dpop_signing_alg_values_supported")
     if not _algs_supported:
         _algs_supported = ["RS256"]
+    else:
+        _algs_supported = [alg for alg in _algs_supported if alg in get_signing_algs()]
 
     _token_endp.upstream_get("context").provider_info[
         "dpop_signing_alg_values_supported"
     ] = _algs_supported
 
     _context = _token_endp.upstream_get("context")
-    _context.dpop_enabled = True
+    _context.add_on["dpop"] = {"algs_supported": _algs_supported}
+    _context.client_authn_methods["dpop"] = DPoPClientAuth
+
+    _userinfo_endpoint = endpoint.get("userinfo")
+    if _userinfo_endpoint:
+        _userinfo_endpoint.post_parse_request.append(userinfo_post_parse_request)
 
 
 # DPoP-bound access token in the "Authorization" header and the DPoP proof in the "DPoP" header
 
 
-class DPoPClientAuth(ClientAuthnMethod):
+class DPoPClientAuth(BearerHeader):
     tag = "dpop_client_auth"
 
     def is_usable(self, request=None, authorization_info=None, http_headers=None):
         if authorization_info is not None and authorization_info.startswith("DPoP "):
             return True
         return False
 
-    def verify(self, authorization_info, **kwargs):
-        client_info = basic_authn(authorization_info)
+    def verify(
+        self,
+        request: Optional[Union[dict, Message]] = None,
+        authorization_token: Optional[str] = None,
+        endpoint=None,  # Optional[Endpoint]
+        get_client_id_from_token: Optional[Callable] = None,
+        **kwargs,
+    ):
+        # info contains token and client_id
+        info = BearerHeader._verify(
+            self, request, authorization_token, endpoint, get_client_id_from_token, **kwargs
+        )
         _context = self.upstream_get("context")
-        if _context.cdb[client_info["id"]]["client_secret"] == client_info["secret"]:
-            return {"client_id": client_info["id"]}
-        else:
-            raise ClientAuthenticationError()
+        return {"client_id": ""}
+        # if _context.cdb[client_info["id"]]["client_secret"] == client_info["secret"]:
+        #     return {"client_id": client_info["id"]}
+        # else:
+        #     raise ClientAuthenticationError()
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/oauth2/add_on/extra_args.py` & `idpyoidc-2.1.0/src/idpyoidc/server/oauth2/add_on/extra_args.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/oauth2/introspection.py` & `idpyoidc-2.1.0/src/idpyoidc/server/oauth2/introspection.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
             "private_key_jwt",
         ]
     }
 
     def __init__(self, upstream_get, **kwargs):
         Endpoint.__init__(self, upstream_get, **kwargs)
         self.offset = kwargs.get("offset", 0)
+        self.enforce_aud_restriction = kwargs.get("enforce_audience_restriction", True)
 
     def _introspect(self, token, client_id, grant):
         # Make sure that the token is an access_token or a refresh_token
         if token.token_class not in ["access_token", "refresh_token"]:
             return None
 
         if not token.is_active():
@@ -109,17 +110,26 @@
 
         grant = _session_info["grant"]
         _token = grant.get_token(request_token)
 
         aud = _token.resources
         if not aud:
             aud = grant.resources
-        
-        if request["client_id"] not in aud:
-            return {"response_args": _resp}
+
+        client_id = request["client_id"]
+        try:
+            _cinfo = _context.cdb[client_id]
+            enforce_aud_restriction = _cinfo.get(
+                "enforce_audience_restriction", self.enforce_aud_restriction
+            )
+        except:
+            enforce_aud_restriction = self.enforce_aud_restriction
+        if enforce_aud_restriction:
+            if request["client_id"] not in aud:
+                return {"response_args": _resp}
 
         _info = self._introspect(_token, _session_info["client_id"], _session_info["grant"])
         if _info is None:
             return {"response_args": _resp}
 
         if release:
             if "username" in release:
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/oauth2/pushed_authorization.py` & `idpyoidc-2.1.0/src/idpyoidc/server/oauth2/pushed_authorization.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+from typing import Optional
+from typing import Union
 import uuid
 
+from idpyoidc.message import Message
 from idpyoidc.message import oauth2
+from idpyoidc.message.oauth2 import AuthorizationRequest
 from idpyoidc.server.oauth2.authorization import Authorization
 
 
 class PushedAuthorization(Authorization):
     request_cls = oauth2.PushedAuthorizationRequest
     response_cls = oauth2.Message
     endpoint_name = "pushed_authorization_request_endpoint"
@@ -16,22 +20,30 @@
 
     def __init__(self, upstream_get, **kwargs):
         Authorization.__init__(self, upstream_get, **kwargs)
         # self.pre_construct.append(self._pre_construct)
         self.post_parse_request.append(self._post_parse_request)
         self.ttl = kwargs.get("ttl", 3600)
 
-    def process_request(self, request=None, **kwargs):
+    def process_request(self, request: Optional[Union[Message, str]] = None, **kwargs):
         """
         Store the request and return a URI.
 
         :param request:
         """
         # create URN
 
+        if isinstance(request, str):
+            _request = AuthorizationRequest().from_urlencoded(request)
+        else:
+            _request = AuthorizationRequest(**request)
+
+        _request.verify(keyjar=self.upstream_get("attribute", "keyjar"))
+
         _urn = "urn:uuid:{}".format(uuid.uuid4())
-        self.upstream_get("context").par_db[_urn] = request
+        # Store the parsed and verified request
+        self.upstream_get("context").par_db[_urn] = _request
 
         return {
             "http_response": {"request_uri": _urn, "expires_in": self.ttl},
-            "return_uri": request["redirect_uri"],
+            "return_uri": _request["redirect_uri"],
         }
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/oauth2/server_metadata.py` & `idpyoidc-2.1.0/src/idpyoidc/server/oauth2/server_metadata.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token.py` & `idpyoidc-2.1.0/src/idpyoidc/server/oauth2/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from .token_helper.refresh_token import RefreshTokenHelper
 from .token_helper.resource_owner_password_credentials import ResourceOwnerPasswordCredentials
 from .token_helper.token_exchange import TokenExchangeHelper
 
 logger = logging.getLogger(__name__)
 
 
-
 class Token(Endpoint):
     request_cls = Message
     response_cls = AccessTokenResponse
     error_cls = TokenErrorResponse
     request_format = "json"
     request_placement = "body"
     response_format = "json"
@@ -40,29 +39,28 @@
         "authorization_code": AccessTokenHelper,
         "refresh_token": RefreshTokenHelper,
         "urn:ietf:params:oauth:grant-type:token-exchange": TokenExchangeHelper,
         "client_credentials": ClientCredentials,
         "password": ResourceOwnerPasswordCredentials,
     }
 
-    _supports = {
-        "grant_types_supported": list(helper_by_grant_type.keys())
-    }
+    _supports = {"grant_types_supported": list(helper_by_grant_type.keys())}
 
     def __init__(self, upstream_get, new_refresh_token=False, **kwargs):
         Endpoint.__init__(self, upstream_get, **kwargs)
         self.post_parse_request.append(self._post_parse_request)
         self.allow_refresh = False
         self.new_refresh_token = new_refresh_token
-        self.grant_type_helper = self.configure_types(kwargs.get("grant_types_helpers"),
-                                                      self.helper_by_grant_type)
+        self.grant_type_helper = self.configure_types(
+            kwargs.get("grant_types_helpers"), self.helper_by_grant_type
+        )
         # self.grant_types_supported = kwargs.get("grant_types_supported",
         #                                         list(self.grant_type_helper.keys()))
         self.revoke_refresh_on_issue = kwargs.get("revoke_refresh_on_issue", False)
-        self.resource_indicators_config = kwargs.get('resource_indicators', None)
+        self.resource_indicators_config = kwargs.get("resource_indicators", None)
 
     def configure_types(self, helpers, default_helpers):
         if helpers is None:
             return {k: v(self) for k, v in default_helpers.items()}
 
         _helper = {}
         for type, args in helpers.items():
@@ -89,41 +87,41 @@
             try:
                 _helper[type] = _class(self, _kwargs)
             except Exception as e:
                 raise ProcessError(f"Failed to initialize class {_class}: {e}")
 
         return _helper
 
-    def _get_helper(self,
-                    request: Union[Message, dict],
-                    client_id: Optional[str] = "") -> Optional[Union[Message, TokenEndpointHelper]]:
-        grant_type = request.get('grant_type')
+    def _get_helper(
+        self, request: Union[Message, dict], client_id: Optional[str] = ""
+    ) -> Optional[Union[Message, TokenEndpointHelper]]:
+        grant_type = request.get("grant_type")
         if grant_type:
-            _client_id = client_id or request.get('client_id')
+            _client_id = client_id or request.get("client_id")
             if client_id:
-                client = self.upstream_get('context').cdb[client_id]
-                _grant_types_supported = client.get("grant_types_supported",
-                                                    self.upstream_get('context').claims.get_claim(
-                                                        "grant_types_supported", [])
-                                                    )
+                client = self.upstream_get("context").cdb[client_id]
+                _grant_types_supported = client.get(
+                    "grant_types_supported",
+                    self.upstream_get("context").claims.get_claim("grant_types_supported", []),
+                )
                 if grant_type not in _grant_types_supported:
                     return self.error_cls(
                         error="invalid_request",
                         error_description=f"Unsupported grant_type: {grant_type}",
                     )
 
             return self.grant_type_helper.get(grant_type)
         else:
             return self.error_cls(
                 error="invalid_request",
                 error_description=f"Do not know how to handle this type of request",
             )
 
     def _post_parse_request(
-            self, request: Union[Message, dict], client_id: Optional[str] = "", **kwargs
+        self, request: Union[Message, dict], client_id: Optional[str] = "", **kwargs
     ):
         _resp = self._get_helper(request, client_id)
         if isinstance(_resp, TokenEndpointHelper):
             return _resp.post_parse_request(request, client_id, **kwargs)
         elif _resp:
             return _resp
         else:
@@ -187,8 +185,8 @@
         _headers = [("Content-type", "application/json")]
         resp = {"response_args": response_args, "http_headers": _headers}
         if _cookie:
             resp["cookie"] = [_cookie]
         return resp
 
     def supports(self):
-        return {'grant_types_supported': list(self.grant_type_helper.keys())}
+        return {"grant_types_supported": list(self.grant_type_helper.keys())}
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token_helper/__init__.py` & `idpyoidc-2.1.0/src/idpyoidc/server/oauth2/token_helper/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,51 +9,51 @@
 from idpyoidc.server.session.token import SessionToken
 from idpyoidc.time_util import utc_time_sans_frac
 
 logger = logging.getLogger(__name__)
 
 
 class TokenEndpointHelper(object):
-
     def __init__(self, endpoint, config=None):
         self.endpoint = endpoint
         self.config = config
         self.error_cls = self.endpoint.error_cls
 
     def post_parse_request(
-            self, request: Union[Message, dict], client_id: Optional[str] = "", **kwargs
+        self, request: Union[Message, dict], client_id: Optional[str] = "", **kwargs
     ):
         """Context specific parsing of the request.
         This is done after general request parsing and before processing
         the request.
         """
         raise NotImplementedError
 
     def process_request(self, req: Union[Message, dict], **kwargs):
         """Acts on a process request."""
         raise NotImplementedError
 
     def _mint_token(
-            self,
-            token_class: str,
-            grant: Grant,
-            session_id: str,
-            client_id: str,
-            based_on: Optional[SessionToken] = None,
-            scope: Optional[list] = None,
-            token_args: Optional[dict] = None,
-            token_type: Optional[str] = "",
+        self,
+        token_class: str,
+        grant: Grant,
+        session_id: str,
+        client_id: str,
+        based_on: Optional[SessionToken] = None,
+        scope: Optional[list] = None,
+        token_args: Optional[dict] = None,
+        token_type: Optional[str] = "",
     ) -> SessionToken:
         _context = self.endpoint.upstream_get("context")
         _mngr = _context.session_manager
         usage_rules = grant.usage_rules.get(token_class)
         if usage_rules:
             _exp_in = usage_rules.get("expires_in")
         else:
-            _exp_in = DEFAULT_TOKEN_LIFETIME
+            _token_handler = _mngr.token_handler[token_class]
+            _exp_in = _token_handler.lifetime
 
         token_args = token_args or {}
         for meth in _context.token_args_methods:
             token_args = meth(_context, client_id, token_args)
 
         if token_args:
             _args = token_args
@@ -91,16 +91,18 @@
             error_description="Missing resource parameter",
         )
 
     client_id = request["client_id"]
 
     resource_servers_per_client = kwargs.get("resource_servers_per_client", [])
 
-    if isinstance(resource_servers_per_client,
-                  dict) and client_id not in resource_servers_per_client:
+    if (
+        isinstance(resource_servers_per_client, dict)
+        and client_id not in resource_servers_per_client
+    ):
         return TokenErrorResponse(
             error="invalid_target",
             error_description=f"Resources for client {client_id} not found",
         )
 
     if isinstance(resource_servers_per_client, dict):
         permitted_resources = [res for res in resource_servers_per_client[client_id]]
@@ -150,27 +152,27 @@
 
     if "actor_token" in request or "actor_token_type" in request:
         return TokenErrorResponse(
             error="invalid_request", error_description="Actor token not supported"
         )
 
     if (
-            "requested_token_type" in request
-            and request["requested_token_type"] == "urn:ietf:params:oauth:token-type:refresh_token"
+        "requested_token_type" in request
+        and request["requested_token_type"] == "urn:ietf:params:oauth:token-type:refresh_token"
     ):
         if "offline_access" not in subject_token.scope:
             return TokenErrorResponse(
                 error="invalid_request",
                 error_description=f"Exchange {request['subject_token_type']} to refresh token "
-                                  f"forbidden",
+                f"forbidden",
             )
 
     scopes = request.get("scope", subject_token.scope)
     scopes = list(set(scopes).intersection(subject_token.scope))
     if kwargs.get("scope"):
         scopes = list(set(scopes).intersection(kwargs.get("scope")))
     if scopes:
         request["scope"] = scopes
-    else:
-        request.pop("scope")
+    elif "scope" in request:
+        del request["scope"]
 
     return request
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token_helper/access_token.py` & `idpyoidc-2.1.0/src/idpyoidc/server/oauth2/token_helper/access_token.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from ...session.token import AuthorizationCode
 from ...token import UnknownToken
 
 logger = logging.getLogger(__name__)
 
 
 class AccessTokenHelper(TokenEndpointHelper):
-
     def process_request(self, req: Union[Message, dict], **kwargs):
         """
 
         :param req:
         :param kwargs:
         :return:
         """
@@ -46,36 +45,43 @@
         if client_id != req["client_id"]:
             logger.debug("{} owner of token".format(client_id))
             logger.warning("Client using token it was not given")
             return self.error_cls(error="invalid_grant", error_description="Wrong client")
 
         _cinfo = self.endpoint.upstream_get("context").cdb.get(client_id)
 
-        if ("resource_indicators" in _cinfo
-                and "access_token" in _cinfo["resource_indicators"]):
+        if "resource_indicators" in _cinfo and "access_token" in _cinfo["resource_indicators"]:
             resource_indicators_config = _cinfo["resource_indicators"]["access_token"]
         else:
             resource_indicators_config = self.endpoint.kwargs.get("resource_indicators", None)
 
         if resource_indicators_config is not None:
             if "policy" not in resource_indicators_config:
                 policy = {"policy": {"function": validate_resource_indicators_policy}}
                 resource_indicators_config.update(policy)
 
             req = self._enforce_resource_indicators_policy(req, resource_indicators_config)
 
             if isinstance(req, TokenErrorResponse):
                 return req
 
-        # if "grant_types_supported" in _context.cdb[client_id]:
-        #     grant_types_supported = _context.cdb[client_id].get("grant_types_supported")
-        # else:
-        #     grant_types_supported = _context.provider_info["grant_types_supported"]
-
         grant = _session_info["grant"]
+        token_type = "Bearer"
+
+        # Is DPOP supported
+        try:
+            _dpop_enabled = _context.add_on.get("dpop")
+        except AttributeError:
+            _dpop_enabled = False
+
+        if _dpop_enabled:
+            _dpop_jkt = req.get("dpop_jkt")
+            if _dpop_jkt:
+                grant.extra["dpop_jkt"] = _dpop_jkt
+                token_type = "DPoP"
 
         _based_on = grant.get_token(_access_code)
         _supports_minting = _based_on.usage_rules.get("supports_minting", [])
 
         _authn_req = grant.authorization_request
 
         # If redirect_uri was in the initial authorization request
@@ -84,23 +90,26 @@
             if req["redirect_uri"] != _authn_req["redirect_uri"]:
                 return self.error_cls(
                     error="invalid_request", error_description="redirect_uri mismatch"
                 )
 
         logger.debug("All checks OK")
 
-        issue_refresh = kwargs.get("issue_refresh", False)
-
         if resource_indicators_config is not None:
             scope = req["scope"]
         else:
             scope = grant.scope
 
+        if "offline_access" in scope and "refresh_token" in _supports_minting:
+            issue_refresh = True
+        else:
+            issue_refresh = kwargs.get("issue_refresh", False)
+
         _response = {
-            "token_type": "Bearer",
+            "token_type": token_type,
             "scope": scope,
         }
 
         if "access_token" in _supports_minting:
 
             resources = req.get("resource", None)
             if resources:
@@ -111,27 +120,24 @@
             try:
                 token = self._mint_token(
                     token_class="access_token",
                     grant=grant,
                     session_id=_session_info["branch_id"],
                     client_id=_session_info["client_id"],
                     based_on=_based_on,
-                    token_args=token_args
+                    token_args=token_args,
                 )
             except MintingNotAllowed as err:
                 logger.warning(err)
             else:
                 _response["access_token"] = token.value
                 if token.expires_at:
                     _response["expires_in"] = token.expires_at - utc_time_sans_frac()
 
-        if (
-                issue_refresh
-                and "refresh_token" in _supports_minting
-        ):
+        if issue_refresh and "refresh_token" in _supports_minting:
             try:
                 refresh_token = self._mint_token(
                     token_class="refresh_token",
                     grant=grant,
                     session_id=_session_info["branch_id"],
                     client_id=_session_info["client_id"],
                     based_on=_based_on,
@@ -145,15 +151,15 @@
         _mngr[_session_info["branch_id"]] = grant
 
         _based_on.register_usage()
 
         return _response
 
     def _enforce_resource_indicators_policy(self, request, config):
-        _context = self.endpoint.upstream_get('context')
+        _context = self.endpoint.upstream_get("context")
 
         policy = config["policy"]
         function = policy["function"]
         kwargs = policy.get("kwargs", {})
 
         if isinstance(function, str):
             try:
@@ -165,15 +171,15 @@
         try:
             return fn(request, context=_context, **kwargs)
         except Exception as e:
             logger.error(f"Error while executing the {fn} policy function: {e}")
             return self.error_cls(error="server_error", error_description="Internal server error")
 
     def post_parse_request(
-            self, request: Union[Message, dict], client_id: Optional[str] = "", **kwargs
+        self, request: Union[Message, dict], client_id: Optional[str] = "", **kwargs
     ):
         """
         This is where clients come to get their access tokens
 
         :param request: The request
         :param client_id: Client identifier
         :returns:
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token_helper/client_credentials.py` & `idpyoidc-2.1.0/src/idpyoidc/server/oauth2/token_helper/client_credentials.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,51 +8,51 @@
 from idpyoidc.util import sanitize
 from . import TokenEndpointHelper
 
 logger = logging.getLogger(__name__)
 
 
 class ClientCredentials(TokenEndpointHelper):
-
     def __init__(self, endpoint, config=None):
         TokenEndpointHelper.__init__(self, endpoint, config)
 
     def process_request(self, req: Union[Message, dict], **kwargs):
         _context = self.endpoint.upstream_get("context")
         _mngr = _context.session_manager
         logger.debug("Client credentials flow")
 
         # verify the client and the user
 
-        client_id = req['client_id']
+        client_id = req["client_id"]
         _authenticated = req.get("authenticated", False)
         if not _authenticated:
-            if _context.cdb[client_id] != req['client_secret']:
+            if _context.cdb[client_id] != req["client_secret"]:
                 logger.warning("Client authentication failed")
                 return self.error_cls(error="invalid_request", error_description="Wrong client")
 
-        _grant_types_supported = _context.cdb[client_id].get('grant_types_supported')
-        if _grant_types_supported and 'client_credentials' not in _grant_types_supported:
-            return self.error_cls(error="invalid_request",
-                                  error_description="Unsupported grant type")
+        _grant_types_supported = _context.cdb[client_id].get("grant_types_supported")
+        if _grant_types_supported and "client_credentials" not in _grant_types_supported:
+            return self.error_cls(
+                error="invalid_request", error_description="Unsupported grant type"
+            )
 
         # Is there a previous session ?
         try:
-            _session_info = _mngr.get(['client_credentials', client_id])
+            _session_info = _mngr.get(["client_credentials", client_id])
             _grant = _session_info["grant"]
         except KeyError:
-            logger.debug('No previous session')
-            branch_id = _mngr.add_grant(['client_credentials', client_id])
+            logger.debug("No previous session")
+            branch_id = _mngr.add_grant(["client_credentials", client_id])
             _session_info = _mngr.get_session_info(branch_id)
 
         _grant = _session_info["grant"]
 
         token_type = "Bearer"
 
-        _allowed = _context.cdb[client_id].get('allowed_scopes', [])
+        _allowed = _context.cdb[client_id].get("allowed_scopes", [])
         access_token = self._mint_token(
             token_class="access_token",
             grant=_grant,
             session_id=_session_info["branch_id"],
             client_id=_session_info["client_id"],
             based_on=None,
             scope=_allowed,
@@ -67,15 +67,12 @@
 
         if access_token.expires_at:
             _resp["expires_in"] = access_token.expires_at - utc_time_sans_frac()
 
         return _resp
 
     def post_parse_request(
-            self,
-            request: Union[Message, dict],
-            client_id: Optional[str] = "",
-            **kwargs
+        self, request: Union[Message, dict], client_id: Optional[str] = "", **kwargs
     ):
         request = CCAccessTokenRequest(**request.to_dict())
         logger.debug("%s: %s" % (request.__class__.__name__, sanitize(request)))
         return request
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token_helper/refresh_token.py` & `idpyoidc-2.1.0/src/idpyoidc/server/oauth2/token_helper/refresh_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from idpyoidc.time_util import utc_time_sans_frac
 from . import TokenEndpointHelper
 
 logger = logging.getLogger(__name__)
 
 
 class RefreshTokenHelper(TokenEndpointHelper):
-
     def process_request(self, req: Union[Message, dict], **kwargs):
         _context = self.endpoint.upstream_get("context")
         _mngr = _context.session_manager
         logger.debug("Refresh Token")
 
         if req["grant_type"] != "refresh_token":
             return self.error_cls(error="invalid_request", error_description="Wrong grant_type")
@@ -80,44 +79,44 @@
             )
             refresh_token.usage_rules = token.usage_rules.copy()
             _resp["refresh_token"] = refresh_token.value
 
         token.register_usage()
 
         if (
-                "client_id" in req
-                and req["client_id"] in _context.cdb
-                and "revoke_refresh_on_issue" in _context.cdb[req["client_id"]]
+            "client_id" in req
+            and req["client_id"] in _context.cdb
+            and "revoke_refresh_on_issue" in _context.cdb[req["client_id"]]
         ):
             revoke_refresh = _context.cdb[req["client_id"]].get("revoke_refresh_on_issue")
         else:
             revoke_refresh = self.endpoint.revoke_refresh_on_issue
 
         if revoke_refresh:
             token.revoke()
 
         return _resp
 
     def post_parse_request(
-            self, request: Union[Message, dict], client_id: Optional[str] = "", **kwargs
+        self, request: Union[Message, dict], client_id: Optional[str] = "", **kwargs
     ):
         """
         This is where clients come to refresh their access tokens
 
         :param request: The request
         :param client_id: Client identifier
         :returns:
         """
 
         request = RefreshAccessTokenRequest(**request.to_dict())
         _context = self.endpoint.upstream_get("context")
 
         request.verify(
-            keyjar=self.endpoint.upstream_get('sttribute', 'keyjar'),
-            opponent_id=client_id)
+            keyjar=self.endpoint.upstream_get("sttribute", "keyjar"), opponent_id=client_id
+        )
 
         _mngr = _context.session_manager
         try:
             _session_info = _mngr.get_session_info_by_token(
                 request["refresh_token"], grant=True, handler_key="refresh_token"
             )
         except (KeyError, UnknownToken):
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token_helper/resource_owner_password_credentials.py` & `idpyoidc-2.1.0/src/idpyoidc/server/oauth2/token_helper/resource_owner_password_credentials.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,99 +9,96 @@
 from . import TokenEndpointHelper
 from ...user_authn.authn_context import pick_auth
 
 logger = logging.getLogger(__name__)
 
 
 class ResourceOwnerPasswordCredentials(TokenEndpointHelper):
-
     def __init__(self, endpoint, config=None):
         TokenEndpointHelper.__init__(self, endpoint, config)
         self.user_db = {}
         if config:
-            _db = config.get('db')
+            _db = config.get("db")
             if _db:
                 _db_kwargs = _db.get("kwargs", {})
                 self.user_db = instantiate(_db["class"], **_db_kwargs)
 
     def process_request(self, req: Union[Message, dict], **kwargs):
         _context = self.endpoint.upstream_get("context")
         _mngr = _context.session_manager
         logger.debug("Client credentials flow")
 
         # verify the client and the user
 
-        client_id = req['client_id']
+        client_id = req["client_id"]
         _cinfo = _context.cdb.get(client_id)
         if not _cinfo:
-            logger.error('Unknown client')
+            logger.error("Unknown client")
             return self.error_cls(error="invalid_grant", error_description="Unknown client")
 
-        if _cinfo['client_secret'] != req['client_secret']:
+        if _cinfo["client_secret"] != req["client_secret"]:
             logger.warning("Client secret mismatch")
             return self.error_cls(error="invalid_grant", error_description="Wrong client")
 
         _auth_method = None
-        _acr = kwargs.get('acr')
+        _acr = kwargs.get("acr")
         if _acr:
             _auth_method = _context.authn_broker.pick(_acr)
         else:
             try:
                 _auth_method = pick_auth(_context, req)
             except Exception as exc:
                 logger.exception(f"An error occurred while picking the authN broker: {exc}")
 
         if not _auth_method:
-            return self.error_cls(error="invalid_request",
-                                  error_description="Can't authenticate user")
+            return self.error_cls(
+                error="invalid_request", error_description="Can't authenticate user"
+            )
 
         authn = _auth_method["method"]
         # authn_class_ref = _auth_method["acr"]
 
         try:
-            _username = authn.verify(username=req['username'], password=req['password'])
+            _username = authn.verify(username=req["username"], password=req["password"])
         except FailedAuthentication:
             logger.warning("User password did not match")
             return self.error_cls(error="invalid_grant", error_description="Wrong user")
 
         # Is there a previous session ?
         try:
             _session_info = _mngr.get([_username, client_id])
             _grant = _session_info["grant"]
         except KeyError:
-            logger.debug('No previous session')
+            logger.debug("No previous session")
             branch_id = _mngr.add_grant([_username, client_id])
             _session_info = _mngr.get_session_info(branch_id)
 
         _grant = _session_info["grant"]
 
         token_type = "Bearer"
 
-        _allowed = _context.cdb[client_id].get('allowed_scopes', [])
+        _allowed = _context.cdb[client_id].get("allowed_scopes", [])
         access_token = self._mint_token(
             token_class="access_token",
             grant=_grant,
             session_id=_session_info["branch_id"],
             client_id=_session_info["client_id"],
             based_on=None,
             scope=_allowed,
             token_type=token_type,
         )
 
         _resp = {
             "access_token": access_token.value,
             "token_type": access_token.token_class,
-            "scope": _allowed
+            "scope": _allowed,
         }
 
         if access_token.expires_at:
             _resp["expires_in"] = access_token.expires_at - utc_time_sans_frac()
 
         return _resp
 
     def post_parse_request(
-            self,
-            request: Union[Message, dict],
-            client_id: Optional[str] = "",
-            **kwargs
+        self, request: Union[Message, dict], client_id: Optional[str] = "", **kwargs
     ):
         return request
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token_helper/token_exchange.py` & `idpyoidc-2.1.0/src/idpyoidc/server/oauth2/token_helper/token_exchange.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,22 +53,21 @@
         if "token_exchange" in _context.cdb[request["client_id"]]:
             config = _context.cdb[request["client_id"]]["token_exchange"]
         else:
             config = self.config
 
         try:
             request.verify(
-                keyjar=self.endpoint.upstream_get('attribute', 'keyjar'),
-                opponent_id=client_id
+                keyjar=self.endpoint.upstream_get("attribute", "keyjar"), opponent_id=client_id
             )
         except (
-                MissingRequiredAttribute,
-                ValueError,
-                MissingRequiredValue,
-                JWKESTException,
+            MissingRequiredAttribute,
+            ValueError,
+            MissingRequiredValue,
+            JWKESTException,
         ) as err:
             return self.endpoint.error_cls(error="invalid_request", error_description="%s" % err)
 
         self._validate_configuration(config)
 
         _mngr = _context.session_manager
         try:
@@ -129,16 +128,16 @@
         if self.token_types_mapping[subject_token_type] != token.token_class:
             return TokenErrorResponse(
                 error="invalid_request",
                 error_description="Wrong token type",
             )
 
         if (
-                "requested_token_type" in request
-                and request["requested_token_type"] not in config["requested_token_types_supported"]
+            "requested_token_type" in request
+            and request["requested_token_type"] not in config["requested_token_types_supported"]
         ):
             return TokenErrorResponse(
                 error="invalid_request",
                 error_description="Unsupported requested token type",
             )
 
         request_info = dict(scope=request.get("scope", token.scope))
@@ -278,33 +277,30 @@
         if "requested_token_types_supported" not in config:
             raise ImproperlyConfigured(
                 "Missing 'requested_token_types_supported' from Token Exchange configuration"
             )
         if "policy" not in config:
             raise ImproperlyConfigured("Missing 'policy' from Token Exchange configuration")
         if "" not in config["policy"]:
-            raise ImproperlyConfigured(
-                "Default Token Exchange policy configuration is not defined"
-            )
+            raise ImproperlyConfigured("Default Token Exchange policy configuration is not defined")
         if "function" not in config["policy"][""]:
             raise ImproperlyConfigured(
                 "Missing 'function' from default Token Exchange policy configuration"
             )
 
-        _default_requested_token_type = config.get("default_requested_token_type",
-                                                   DEFAULT_REQUESTED_TOKEN_TYPE)
+        _default_requested_token_type = config.get(
+            "default_requested_token_type", DEFAULT_REQUESTED_TOKEN_TYPE
+        )
         if _default_requested_token_type not in config["requested_token_types_supported"]:
             raise ImproperlyConfigured(
                 f"Unsupported default requested_token_type {_default_requested_token_type}"
             )
 
     def get_handler_key(self, request, endpoint_context):
         client_info = endpoint_context.cdb.get(request["client_id"], {})
 
-        default_requested_token_type = (
-                client_info.get("token_exchange", {}).get("default_requested_token_type", None)
-                or
-                self.config.get("default_requested_token_type", DEFAULT_REQUESTED_TOKEN_TYPE)
-        )
+        default_requested_token_type = client_info.get("token_exchange", {}).get(
+            "default_requested_token_type", None
+        ) or self.config.get("default_requested_token_type", DEFAULT_REQUESTED_TOKEN_TYPE)
 
         requested_token_type = request.get("requested_token_type", default_requested_token_type)
         return TOKEN_TYPES_MAPPING[requested_token_type]
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/oauth2/token_revocation.py` & `idpyoidc-2.1.0/src/idpyoidc/server/oauth2/token_revocation.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 class TokenRevocation(Endpoint):
     """Implements RFC7009"""
 
     request_cls = oauth2.TokenRevocationRequest
     response_cls = oauth2.TokenRevocationResponse
     error_cls = oauth2.TokenRevocationErrorResponse
     request_format = "urlencoded"
-    response_format = "json"
+    response_format = "text"
+    response_body_type = "text"
     endpoint_name = "revocation_endpoint"
     name = "token_revocation"
     default_capabilities = {
         "client_authn_method": [
             "client_secret_basic",
             "client_secret_post",
             "client_secret_jwt",
@@ -73,24 +74,27 @@
             return self.error_cls(error="invalid_grant", error_description="Wrong client")
 
         grant = _session_info["grant"]
         _token = grant.get_token(request_token)
 
         try:
             self.token_types_supported = _context.cdb[client_id]["token_revocation"][
-                "token_types_supported"]
+                "token_types_supported"
+            ]
         except Exception:
-            self.token_types_supported = self.token_revocation_kwargs.get("token_types_supported",
-                                                                          self.token_types_supported)
+            self.token_types_supported = self.token_revocation_kwargs.get(
+                "token_types_supported", self.token_types_supported
+            )
 
         try:
             self.policy = _context.cdb[client_id]["token_revocation"]["policy"]
         except Exception:
-            self.policy = self.token_revocation_kwargs.get("policy", {
-                "": {"function": validate_token_revocation_policy}})
+            self.policy = self.token_revocation_kwargs.get(
+                "policy", {"": {"function": validate_token_revocation_policy}}
+            )
 
         if _token.token_class not in self.token_types_supported:
             desc = (
                 "The authorization server does not support the revocation of "
                 "the presented token type. That is, the client tried to revoke an access "
                 "token on a server not supporting this feature."
             )
@@ -126,9 +130,9 @@
             return self.error_cls(error="server_error", error_description="Internal server error")
 
 
 def validate_token_revocation_policy(token, session_info, **kwargs):
     _token = token
     _token.revoke()
 
-    response_args = {"response_args": {}}
-    return oauth2.TokenRevocationResponse(**response_args)
+    response_args = {"response_msg": "OK"}
+    return response_args
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/oidc/add_on/custom_scopes.py` & `idpyoidc-2.1.0/src/idpyoidc/server/oidc/add_on/custom_scopes.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/oidc/add_on/pkce.py` & `idpyoidc-2.1.0/src/idpyoidc/server/oauth2/add_on/pkce.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import hashlib
 import logging
 from typing import Dict
+from typing import Optional
 
 from cryptojwt.utils import b64e
 
 from idpyoidc.message.oauth2 import AuthorizationErrorResponse
 from idpyoidc.message.oauth2 import RefreshAccessTokenRequest
 from idpyoidc.message.oauth2 import TokenExchangeRequest
 from idpyoidc.message.oauth2 import CCAccessTokenRequest
@@ -40,27 +41,26 @@
     :param kwargs:
     :return:
     """
     client = context.cdb[client_id]
     if "pkce_essential" in client:
         essential = client["pkce_essential"]
     else:
-        essential = context.args["pkce"].get("essential", False)
+        essential = context.add_on["pkce"].get("essential", False)
     if essential and "code_challenge" not in request:
         return AuthorizationErrorResponse(
             error="invalid_request",
             error_description="Missing required code_challenge",
         )
 
     if "code_challenge_method" not in request:
-        request["code_challenge_method"] = "S256"
+        request["code_challenge_method"] = "plain"
 
     if "code_challenge" in request and (
-        request["code_challenge_method"]
-        not in context.args["pkce"]["code_challenge_methods"]
+        request["code_challenge_method"] not in context.add_on["pkce"]["code_challenge_methods"]
     ):
         return AuthorizationErrorResponse(
             error="invalid_request",
             error_description="Unsupported code_challenge_method={}".format(
                 request["code_challenge_method"]
             ),
         )
@@ -122,40 +122,39 @@
             _method,
         ):
             return TokenErrorResponse(error="invalid_grant", error_description="PKCE check failed")
 
     return request
 
 
-def add_pkce_support(endpoint: Dict[str, Endpoint], **kwargs):
+def add_support(
+    endpoint: Dict[str, Endpoint],
+    code_challenge_methods: Optional[dict] = None,
+    essential: Optional[bool] = False,
+    **kwargs
+):
     authn_endpoint = endpoint.get("authorization")
     if authn_endpoint is None:
         LOGGER.warning("No authorization endpoint found, skipping PKCE configuration")
         return
 
     token_endpoint = endpoint.get("token")
     if token_endpoint is None:
         LOGGER.warning("No token endpoint found, skipping PKCE configuration")
         return
 
     authn_endpoint.post_parse_request.append(post_authn_parse)
     token_endpoint.post_parse_request.append(post_token_parse)
 
-    code_challenge_methods = kwargs.get("code_challenge_methods", CC_METHOD.keys())
-    code_challenge_methods = list(
-        set(code_challenge_methods).intersection(
-            authn_endpoint._supports["code_challenge_methods_supported"]
-        )
-    )
-    if not code_challenge_methods:
-        raise ValueError(
-            "Unsupported method: {}".format(
-                ", ".join(kwargs.get("code_challenge_methods", CC_METHOD.keys()))
-            )
-        )
-    kwargs["code_challenge_methods"] = {}
-    for method in code_challenge_methods:
-        if method not in CC_METHOD:
-            raise ValueError("Unsupported method: {}".format(method))
-        kwargs["code_challenge_methods"][method] = CC_METHOD[method]
-
-    authn_endpoint.upstream_get("context").args["pkce"] = kwargs
+    if code_challenge_methods is None:
+        code_challenge_methods = CC_METHOD
+    else:
+        for method in code_challenge_methods:
+            if method not in CC_METHOD:
+                raise ValueError("Unsupported method: {}".format(method))
+
+    _context = authn_endpoint.upstream_get("context")
+    _context.add_on["pkce"] = {
+        "code_challenge_methods": code_challenge_methods,
+        "essential": essential,
+    }
+    _context.set_preference("code_challenge_methods_supported", list(code_challenge_methods.keys()))
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/oidc/authorization.py` & `idpyoidc-2.1.0/src/idpyoidc/server/oidc/authorization.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,19 +83,18 @@
             "encrypt_request_object_supported": False,
             "request_object_signing_alg_values_supported": claims.get_signing_algs,
             "request_object_encryption_alg_values_supported": claims.get_encryption_algs,
             "request_object_encryption_enc_values_supported": claims.get_encryption_encs,
             "request_parameter_supported": True,
             "request_uri_parameter_supported": True,
             "require_request_uri_registration": False,
-            "response_types_supported": ["code", "token", "code token", 'id_token', 'id_token token',
-                                     'code id_token', 'code id_token token'],
-            "response_modes_supported": ['query', 'fragment', 'form_post'],
+            "response_types_supported": ["code", "id_token", "code id_token"],
+            "response_modes_supported": ["query", "fragment", "form_post"],
             "subject_types_supported": ["public", "pairwise", "ephemeral"],
-          },
+        },
     }
 
     def __init__(self, upstream_get: Callable, **kwargs):
         authorization.Authorization.__init__(self, upstream_get, **kwargs)
         self.post_parse_request.append(self._do_request_uri)
         self.post_parse_request.append(self._post_parse_request)
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/oidc/backchannel_authentication.py` & `idpyoidc-2.1.0/src/idpyoidc/server/oidc/backchannel_authentication.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
                 _context = self.upstream_get("context")
                 if _context.login_hint_lookup:
                     _request_user = _context.login_hint_lookup(_login_hint)
         elif request.get("login_hint_token"):
             _context = self.upstream_get("context")
             _request_user = execute(
                 self.parse_login_hint_token,
-                keyjar=self.upstream_get('attribute', 'keyjar'),
+                keyjar=self.upstream_get("attribute", "keyjar"),
                 login_hint_token=request.get("login_hint_token"),
                 context=_context,
             )
 
         return _request_user
 
     def allowed_target_uris(self):
@@ -81,18 +81,18 @@
         _context = self.upstream_get("context")
         res = [_context.issuer]
         res.append(self.full_path)
         res.append(self.upstream_get("endpoint", "token").full_path)
         return set(res)
 
     def process_request(
-            self,
-            request: Optional[Union[Message, dict]] = None,
-            http_info: Optional[dict] = None,
-            **kwargs,
+        self,
+        request: Optional[Union[Message, dict]] = None,
+        http_info: Optional[dict] = None,
+        **kwargs,
     ):
         try:
             request_user = self.do_request_user(request)
         except KeyError:
             logger.error("Login hint didn't lead to a known user")
             _error_msg = self.error_cls(
                 error="invalid_request", error_description="Login hint didn't lead to a known user"
@@ -132,15 +132,15 @@
             "client_id": _path[1],
             "grant_id": _path[2],
             "session_id": request["_session_id"],
         }
         return session_info, _grant
 
     def post_parse_request(
-            self, request: Union[Message, dict], client_id: Optional[str] = "", **kwargs
+        self, request: Union[Message, dict], client_id: Optional[str] = "", **kwargs
     ) -> Union[Message, dict]:
         _context = self.endpoint.upstream_get("context")
         _mngr = _context.session_manager
         _session_id = _mngr.auth_req_id_map[request["auth_req_id"]]
         _info = _mngr.get_session_info(_session_id)
         # There should be 2 grants for the user_id, client_id combination
         # one without authentication information, the other one with
@@ -298,18 +298,18 @@
         "backchannel_client_notification_endpoint": None,
     }
 
     def __init__(self, upstream_get: Callable, **kwargs):
         Endpoint.__init__(self, upstream_get, **kwargs)
 
     def process_request(
-            self,
-            request: Optional[Union[Message, dict]] = None,
-            http_info: Optional[dict] = None,
-            **kwargs,
+        self,
+        request: Optional[Union[Message, dict]] = None,
+        http_info: Optional[dict] = None,
+        **kwargs,
     ) -> Union[Message, dict]:
         return {}
 
 
 class ClientNotificationAuthn(ClientSecretBasic):
     """The authentication method used at the notification endpoint."""
 
@@ -317,19 +317,19 @@
 
     def is_usable(self, request=None, authorization_token=None):
         if authorization_token is not None and authorization_token.startswith("Bearer "):
             return True
         return False
 
     def _verify(
-            self,
-            authorization_token: Optional[str] = None,
-            endpoint=None,  # Optional[Endpoint]
-            get_client_id_from_token: Optional[Callable] = None,
-            **kwargs,
+        self,
+        authorization_token: Optional[str] = None,
+        endpoint=None,  # Optional[Endpoint]
+        get_client_id_from_token: Optional[Callable] = None,
+        **kwargs,
     ):
         ttype, token = authorization_token.split(" ", 1)
         if ttype != "Bearer":
             raise NoSuchAuthentication(f"No support for {ttype}")
         if get_client_id_from_token:
             client_id = get_client_id_from_token(token)
         else:
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/oidc/discovery.py` & `idpyoidc-2.1.0/src/idpyoidc/server/oidc/discovery.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/oidc/provider_config.py` & `idpyoidc-2.1.0/src/idpyoidc/server/oidc/provider_config.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/oidc/read_registration.py` & `idpyoidc-2.1.0/src/idpyoidc/server/oidc/read_registration.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/oidc/registration.py` & `idpyoidc-2.1.0/src/idpyoidc/server/oidc/registration.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,29 +149,28 @@
             return None
 
         if _val:
             if isinstance(_claim_spec[0], list):
                 if isinstance(val, str):
                     if val in _val:
                         return val
-                    else:
-                        return None
                 else:
                     _ret = list(set(_val).intersection(set(val)))
                     if len(_ret) > 0:
                         return _ret
                     else:
                         raise CapabilitiesMisMatch(_my_key)
             else:
-                if val == _val:
+                if isinstance(_val, list):
+                    if val in _val:
+                        return val
+                elif val == _val:
                     return val
-                else:
-                    return None
-        else:
-            return None
+
+        return None
 
     def filter_client_request(self, request: dict) -> dict:
         _args = {}
         _context = self.upstream_get("context")
         for key, val in request.items():
             if key not in _context.claims.register2preferred:
                 _args[key] = val
@@ -246,20 +245,26 @@
                     _cinfo[item] = request[item]
                 else:
                     return ResponseMessage(
                         error="invalid_configuration_parameter",
                         error_description="%s pointed to illegal URL" % item,
                     )
 
-        _keyjar = self.upstream_get('attribute', 'keyjar')
+        _keyjar = self.upstream_get("attribute", "keyjar")
         # Do I have the necessary keys
         for item in ["id_token_signed_response_alg", "userinfo_signed_response_alg"]:
             if item in request:
-                if request[item] in _context.provider_info[
-                        _context.claims.register2preferred[item]]:
+                _claim = _context.claims.register2preferred[item]
+                _support = _context.provider_info.get(_claim)
+                if _support is None:
+                    logger.warning(f'Lacking support for "{item}"')
+                    del _cinfo[item]
+                    continue
+
+                if request[item] in _support:
                     ktyp = alg2keytype(request[item])
                     # do I have this ktyp and for EC type keys the curve
                     if ktyp not in ["none", "oct"]:
                         _k = []
                         for iss in ["", _context.issuer]:
                             _k.extend(
                                 _keyjar.get_signing_key(ktyp, alg=request[item], issuer_id=iss)
@@ -461,15 +466,15 @@
         args = dict([(k, v) for k, v in _cinfo.items() if k in self.response_cls.c_param])
 
         comb_uri(args)
         response = self.response_cls(**args)
 
         # Add the client_secret as a symmetric key to the key jar
         if client_secret:
-            self.upstream_get('attribute', 'keyjar').add_symmetric(client_id, str(client_secret))
+            self.upstream_get("attribute", "keyjar").add_symmetric(client_id, str(client_secret))
 
         logger.debug("Stored updated client info in CDB under cid={}".format(client_id))
         logger.debug("ClientInfo: {}".format(_cinfo))
         _context.cdb[client_id] = _cinfo
 
         # Not all databases can be sync'ed
         if hasattr(_context.cdb, "sync") and callable(_context.cdb.sync):
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/oidc/session.py` & `idpyoidc-2.1.0/src/idpyoidc/server/oidc/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,18 +132,20 @@
         payload = {"sid": sid, "events": {BACK_CHANNEL_LOGOUT_EVENT: {}}}
 
         try:
             alg = cinfo["id_token_signed_response_alg"]
         except KeyError:
             alg = _context.provider_info["id_token_signing_alg_values_supported"][0]
 
-        _jws = JWT(self.upstream_get('attribute', 'keyjar'),
-                   iss=_context.issuer,
-                   lifetime=86400,
-                   sign_alg=alg)
+        _jws = JWT(
+            self.upstream_get("attribute", "keyjar"),
+            iss=_context.issuer,
+            lifetime=86400,
+            sign_alg=alg,
+        )
         _jws.with_jti = True
         _logout_token = _jws.pack(payload=payload, recv=cinfo["client_id"])
 
         return back_channel_logout_uri, _logout_token
 
     def clean_sessions(self, usids):
         # Revoke all sessions
@@ -217,15 +219,15 @@
         _jwt = factory(sjwt)
         if _jwt:
             if sig_alg:
                 alg = sig_alg
             else:
                 alg = self.kwargs["signing_alg"]
 
-            sign_keys = self.upstream_get('attribute', 'keyjar').get_signing_key(alg2keytype(alg))
+            sign_keys = self.upstream_get("attribute", "keyjar").get_signing_key(alg2keytype(alg))
             _info = _jwt.verify_compact(keys=sign_keys, sigalg=alg)
             return _info
         else:
             raise ValueError("Not a signed JWT")
 
     def logout_from_client(self, sid):
         _context = self.upstream_get("context")
@@ -338,15 +340,15 @@
             payload["state"] = request["state"]
 
         payload["redirect_uri"] = _uri
 
         logger.debug("JWS payload: {}".format(payload))
         # From me to me
         _jws = JWT(
-            self.upstream_get('attribute', 'keyjar'),
+            self.upstream_get("attribute", "keyjar"),
             iss=_context.issuer,
             lifetime=86400,
             sign_alg=self.kwargs["signing_alg"],
         )
         sjwt = _jws.pack(payload=payload, recv=_context.issuer)
 
         location = "{}?{}".format(self.kwargs["logout_verify_url"], urlencode({"sjwt": sjwt}))
@@ -373,15 +375,15 @@
         else:
             request["client_id"] = auth_info["client_id"]
             request["access_token"] = auth_info["token"]
 
         if isinstance(request, dict):
             _context = self.upstream_get("context")
             request = self.request_cls(**request)
-            if not request.verify(keyjar=self.upstream_get('attribute', 'keyjar'), sigalg=""):
+            if not request.verify(keyjar=self.upstream_get("attribute", "keyjar"), sigalg=""):
                 raise InvalidRequest("Request didn't verify")
             # id_token_signing_alg_values_supported
             try:
                 _ith = request[verified_claim_name("id_token_hint")]
             except KeyError:
                 pass
             else:
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/oidc/token.py` & `idpyoidc-2.1.0/src/idpyoidc/server/oidc/token.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/oidc/token_helper/access_token.py` & `idpyoidc-2.1.0/src/idpyoidc/server/oidc/token_helper/access_token.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from idpyoidc.server.token.exception import UnknownToken
 from idpyoidc.util import sanitize
 
 logger = logging.getLogger(__name__)
 
 
 class AccessTokenHelper(TokenEndpointHelper):
-
     def _get_session_info(self, request, session_manager):
         if request["grant_type"] != "authorization_code":
             return self.error_cls(error="invalid_request", error_description="Unknown grant_type")
 
         try:
             _access_code = request["code"].replace(" ", "+")
         except KeyError:  # Missing code parameter - absolutely fatal
@@ -59,18 +58,18 @@
         else:
             grant_types_supported = _context.provider_info["grant_types_supported"]
         grant = _session_info["grant"]
 
         token_type = "Bearer"
 
         # Is DPOP supported
-        try:
-            _dpop_enabled = _context.dpop_enabled
-        except AttributeError:
-            _dpop_enabled = False
+        _dpop_enabled = False
+        _dpop_args = _context.add_on.get("dpop")
+        if _dpop_args:
+            _dpop_enabled = True
 
         if _dpop_enabled:
             _dpop_jkt = req.get("dpop_jkt")
             if _dpop_jkt:
                 grant.extra["dpop_jkt"] = _dpop_jkt
                 token_type = "DPoP"
 
@@ -112,18 +111,15 @@
             except MintingNotAllowed as err:
                 logger.warning(err)
             else:
                 _response["access_token"] = token.value
                 if token.expires_at:
                     _response["expires_in"] = token.expires_at - utc_time_sans_frac()
 
-        if (
-                issue_refresh
-                and "refresh_token" in _supports_minting
-        ):
+        if issue_refresh and "refresh_token" in _supports_minting:
             try:
                 refresh_token = self._mint_token(
                     token_class="refresh_token",
                     grant=grant,
                     session_id=_session_info["branch_id"],
                     client_id=_session_info["client_id"],
                     based_on=_based_on,
@@ -157,15 +153,15 @@
                 _response["id_token"] = _idtoken.value
 
         _based_on.register_usage()
 
         return _response
 
     def post_parse_request(
-            self, request: Union[Message, dict], client_id: Optional[str] = "", **kwargs
+        self, request: Union[Message, dict], client_id: Optional[str] = "", **kwargs
     ) -> Union[Message, dict]:
         """
         This is where clients come to get their access tokens
 
         :param request: The request
         :param client_id: Client identifier
         :returns:
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/oidc/token_helper/refresh_token.py` & `idpyoidc-2.1.0/src/idpyoidc/server/oidc/token_helper/refresh_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 from idpyoidc.server.session.token import MintingNotAllowed
 from idpyoidc.server.session.token import RefreshToken
 from idpyoidc.server.token.exception import UnknownToken
 from idpyoidc.util import sanitize
 
 logger = logging.getLogger(__name__)
 
-class RefreshTokenHelper(TokenEndpointHelper):
 
+class RefreshTokenHelper(TokenEndpointHelper):
     def process_request(self, req: Union[Message, dict], **kwargs):
         _context = self.endpoint.upstream_get("context")
         _mngr = _context.session_manager
 
         if req["grant_type"] != "refresh_token":
             return self.error_cls(error="invalid_request", error_description="Wrong grant_type")
 
@@ -109,46 +109,44 @@
                 return resp
 
             _resp["id_token"] = _idtoken.value
 
         token.register_usage()
 
         if (
-                "client_id" in req
-                and req["client_id"] in _context.cdb
-                and "revoke_refresh_on_issue" in _context.cdb[req["client_id"]]
+            "client_id" in req
+            and req["client_id"] in _context.cdb
+            and "revoke_refresh_on_issue" in _context.cdb[req["client_id"]]
         ):
             revoke_refresh = _context.cdb[req["client_id"]].get("revoke_refresh_on_issue")
         else:
             revoke_refresh = self.endpoint.revoke_refresh_on_issue
 
         if revoke_refresh:
             token.revoke()
 
         return _resp
 
     def post_parse_request(
-            self,
-            request: Union[Message, dict],
-            client_id: Optional[str] = "",
-            **kwargs
+        self, request: Union[Message, dict], client_id: Optional[str] = "", **kwargs
     ):
         """
         This is where clients come to refresh their access tokens
 
         :param request: The request
         :param client_id: Client identifier
         :returns:
         """
 
         request = RefreshAccessTokenRequest(**request.to_dict())
         _context = self.endpoint.upstream_get("context")
 
-        request.verify(keyjar=self.endpoint.upstream_get('attribute', 'keyjar'),
-                       opponent_id=client_id)
+        request.verify(
+            keyjar=self.endpoint.upstream_get("attribute", "keyjar"), opponent_id=client_id
+        )
 
         _mngr = _context.session_manager
         try:
             _session_info = _mngr.get_session_info_by_token(
                 request["refresh_token"], handler_key="refresh_token", grant=True
             )
         except (KeyError, UnknownToken, BadSyntax):
@@ -172,8 +170,7 @@
             if not req_scopes.issubset(scopes):
                 return self.error_cls(
                     error="invalid_request",
                     error_description="Invalid refresh scopes",
                 )
 
         return request
-
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/oidc/userinfo.py` & `idpyoidc-2.1.0/src/idpyoidc/server/oidc/userinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,58 +22,49 @@
 logger = logging.getLogger(__name__)
 
 
 class UserInfo(Endpoint):
     request_cls = Message
     response_cls = oidc.OpenIDSchema
     request_format = "json"
-    response_format = "json"
+    response_format = "jose"
     response_placement = "body"
     endpoint_name = "userinfo_endpoint"
     name = "userinfo"
     _supports = {
         "claim_types_supported": ["normal", "aggregated", "distributed"],
         "encrypt_userinfo_supported": True,
         "userinfo_signing_alg_values_supported": claims.get_signing_algs,
         "userinfo_encryption_alg_values_supported": claims.get_encryption_algs,
         "userinfo_encryption_enc_values_supported": claims.get_encryption_encs,
     }
 
-    def __init__(self, upstream_get: Callable, add_claims_by_scope: Optional[bool] = True, **kwargs):
+    def __init__(
+        self, upstream_get: Callable, add_claims_by_scope: Optional[bool] = True, **kwargs
+    ):
         Endpoint.__init__(
             self,
             upstream_get,
             add_claims_by_scope=add_claims_by_scope,
             **kwargs,
         )
         # Add the issuer ID as an allowed JWT target
         self.allowed_targets.append("")
+        self.config = kwargs or {}
 
-        if kwargs is None:
-            self.config = {
-                "policy": {
-                    "function": "/path/to/callable",
-                    "kwargs": {}
-                },
-            }
-        else:
-            self.config = kwargs
-
-    def get_client_id_from_token(self, endpoint_context, token, request=None):
-        _info = endpoint_context.session_manager.get_session_info_by_token(
-            token, handler_key="access_token"
-        )
+    def get_client_id_from_token(self, context, token, request=None):
+        _info = context.session_manager.get_session_info_by_token(token, handler_key="access_token")
         return _info["client_id"]
 
     def do_response(
-            self,
-            response_args: Optional[Union[Message, dict]] = None,
-            request: Optional[Union[Message, dict]] = None,
-            client_id: Optional[str] = "",
-            **kwargs
+        self,
+        response_args: Optional[Union[Message, dict]] = None,
+        request: Optional[Union[Message, dict]] = None,
+        client_id: Optional[str] = "",
+        **kwargs,
     ) -> dict:
 
         if "error" in kwargs and kwargs["error"]:
             return Endpoint.do_response(self, response_args, request, **kwargs)
 
         _context = self.upstream_get("context")
         if not client_id:
@@ -96,15 +87,15 @@
             encrypt = True
         except KeyError:
             encrypt = False
             enc_alg = enc_enc = ""
 
         if encrypt or sign:
             _jwt = JWT(
-                self.upstream_get('attribute', 'keyjar'),
+                self.upstream_get("attribute", "keyjar"),
                 iss=_context.issuer,
                 sign=sign,
                 sign_alg=sign_alg,
                 encrypt=encrypt,
                 enc_enc=enc_enc,
                 enc_alg=enc_alg,
             )
@@ -140,15 +131,15 @@
 
         # And it should be valid
         if token.is_active() is False:
             return self.error_cls(error="invalid_token", error_description="Invalid Token")
 
         allowed = True
         _auth_event = _grant.authentication_event
-        # if the authenticate is still active or offline_access is granted.
+        # if the authentication is still active or offline_access is granted.
         if not _auth_event["valid_until"] >= utc_time_sans_frac():
             logger.debug(
                 "authentication not valid: {} > {}".format(
                     datetime.fromtimestamp(_auth_event["valid_until"]),
                     datetime.fromtimestamp(utc_time_sans_frac()),
                 )
             )
@@ -203,15 +194,22 @@
 
         if isinstance(auth_info, ResponseMessage):
             return auth_info
         else:
             request["client_id"] = auth_info["client_id"]
             request["access_token"] = auth_info["token"]
 
-        return request
+        # Do any endpoint specific parsing
+        return self.do_post_parse_request(
+            request=request,
+            client_id=auth_info["client_id"],
+            http_info=http_info,
+            auth_info=auth_info,
+            **kwargs,
+        )
 
     def _enforce_policy(self, request, response_info, token, config):
         policy = config["policy"]
         callable = policy["function"]
         kwargs = policy.get("kwargs", {})
 
         if isinstance(callable, str):
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/scopes.py` & `idpyoidc-2.1.0/src/idpyoidc/server/scopes.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/session/claims.py` & `idpyoidc-2.1.0/src/idpyoidc/server/session/claims.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from typing import List
 from typing import Optional
 from typing import Union
 
 from idpyoidc.message.oidc import OpenIDSchema
 from idpyoidc.server.exception import ImproperlyConfigured
 from idpyoidc.server.exception import ServiceError
 
@@ -22,16 +23,18 @@
         return STANDARD_CLAIMS
 
 
 class ClaimsInterface:
     init_args = {"add_claims_by_scope": False, "enable_claims_per_client": False}
     claims_release_points = ["userinfo", "introspection", "id_token", "access_token"]
 
-    def __init__(self, upstream_get):
+    def __init__(self, upstream_get, claims_release_points:List[str] = None):
         self.upstream_get = upstream_get
+        if claims_release_points:
+            self.claims_release_points = claims_release_points
 
     def authorization_request_claims(
         self,
         authorization_request: dict,
         claims_release_point: Optional[str] = "",
     ) -> dict:
         if authorization_request and "claims" in authorization_request:
@@ -164,14 +167,15 @@
         client_id = session_info["client_id"]
         grant = session_info["grant"]
 
         if grant.authorization_request:
             auth_req = grant.authorization_request
         else:
             auth_req = {}
+
         claims = self.get_claims_from_request(
             auth_req=auth_req,
             claims_release_point=claims_release_point,
             scopes=scopes,
             client_id=client_id,
             secondary_identifier=secondary_identifier,
         )
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/session/database.py` & `idpyoidc-2.1.0/src/idpyoidc/server/session/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,33 +40,33 @@
 
         session_params = kwargs.get("session_params", {})
         self.node_type = session_params.get("node_type")
         self.node_info_class = session_params.get("node_info_class")
 
     @staticmethod
     def branch_key(*args):
-        """ Construct a key using a list of names """
+        """Construct a key using a list of names"""
         return DIVIDER.join(args)
 
     @staticmethod
     def unpack_branch_key(key):
-        """ Translate a key into an ordered list of names """
+        """Translate a key into an ordered list of names"""
         return key.split(DIVIDER)
 
     def encrypted_branch_id(self, *args) -> str:
-        """ Provided an ordered list of names construct a key and then encrypt it. """
+        """Provided an ordered list of names construct a key and then encrypt it."""
         rnd = rndstr(32)
         return base64.b64encode(
             self.crypt.encrypt(lv_pack(rnd, self.branch_key(*args)).encode())
         ).decode("utf-8")
 
     def decrypt_branch_id(self, key: str) -> List[str]:
         """
-            Given an encrypted key, decrypt it and then unpack the key to return an ordered list
-            of names.
+        Given an encrypted key, decrypt it and then unpack the key to return an ordered list
+        of names.
         """
         try:
             plain = self.crypt.decrypt(base64.b64decode(key))
         except cryptography.fernet.InvalidToken as err:
             logger.error(f"cryptography.fernet.InvalidToken: {key}")
             raise ValueError(err)
         except Exception as err:
@@ -84,15 +84,15 @@
         :param value: Class instance to be stored
         """
 
         _len = len(path)
 
         _superior = None
         for i in range(_len):
-            _key = self.branch_key(*path[0:i + 1])
+            _key = self.branch_key(*path[0 : i + 1])
             # _key = path[i]
             _info = self.db.get(_key)
             if _info is None:
                 if i == _len - 1:
                     _info = value
                 else:
                     if self.node_type:
@@ -111,15 +111,15 @@
                 if _key not in getattr(_superior, "subordinate", {}):
                     _superior.add_subordinate(_key)
 
             self.db[_key] = _info
             _superior = _info
 
     def get(self, path: List[str]) -> Union[NodeInfo, Grant]:
-        """ Given a path return the node that matches the path. """
+        """Given a path return the node that matches the path."""
         _key = self.branch_key(*path)
         return self.db[_key]
 
     def delete_sub_tree(self, key: str):
         """
         Removes all a node and all its subordinates
 
@@ -152,15 +152,15 @@
         # start at leaf and work our way upwards
         _inv_path = path[:]
         _inv_path.reverse()
         _len = len(path)
 
         _sub = None
         for i in range(0, len(path)):
-            _key = self.branch_key(*path[0:_len - i])
+            _key = self.branch_key(*path[0 : _len - i])
             if _key in self.db:
                 _node = self.db[_key]
                 if _sub:
                     if _sub in _node.subordinate:
                         _node.subordinate.remove(_sub)
                         if _node.subordinate == []:
                             self.db.__delitem__(_key)
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/session/grant.py` & `idpyoidc-2.1.0/src/idpyoidc/server/session/grant.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,19 @@
         "authorization_details": {},  # As defined in draft-lodderstedt-oauth-rar
         "claims": {},  # As defined in OIDC core
         "resources": [],  # As defined in RFC8707
         "scope": "",  # As defined in RFC6749
     }
 
     def __init__(
-            self,
-            scope: Optional[str] = "",
-            authorization_details: Optional[dict] = None,
-            claims: Optional[list] = None,
-            resources: Optional[list] = None,
+        self,
+        scope: Optional[str] = "",
+        authorization_details: Optional[dict] = None,
+        claims: Optional[list] = None,
+        resources: Optional[list] = None,
     ):
         ImpExp.__init__(self)
         self.scope = scope
         self.authorization_details = authorization_details
         self.claims = claims
         self.resources = resources
 
@@ -100,32 +100,32 @@
     type = "grant"
     special_load_dump = {
         "issued_token": {"load": issued_token_load, "dump": issued_token_dump},
         "token_map": {"load": token_map_load, "dump": token_map_dump},
     }
 
     def __init__(
-            self,
-            scope: Optional[list] = None,
-            claims: Optional[dict] = None,
-            resources: Optional[list] = None,
-            authorization_details: Optional[dict] = None,
-            authorization_request: Optional[Message] = None,
-            authentication_event: Optional[AuthnEvent] = None,
-            issued_token: Optional[list] = None,
-            usage_rules: Optional[dict] = None,
-            issued_at: int = 0,
-            expires_in: int = 0,
-            expires_at: int = 0,
-            revoked: bool = False,
-            token_map: Optional[dict] = None,
-            sub: Optional[str] = "",
-            extra: Optional[Dict[str, str]] = None,
-            remember_token: Optional[Callable] = None,
-            remove_inactive_token: Optional[bool] = False,
+        self,
+        scope: Optional[list] = None,
+        claims: Optional[dict] = None,
+        resources: Optional[list] = None,
+        authorization_details: Optional[dict] = None,
+        authorization_request: Optional[Message] = None,
+        authentication_event: Optional[AuthnEvent] = None,
+        issued_token: Optional[list] = None,
+        usage_rules: Optional[dict] = None,
+        issued_at: int = 0,
+        expires_in: int = 0,
+        expires_at: int = 0,
+        revoked: bool = False,
+        token_map: Optional[dict] = None,
+        sub: Optional[str] = "",
+        extra: Optional[Dict[str, str]] = None,
+        remember_token: Optional[Callable] = None,
+        remove_inactive_token: Optional[bool] = False,
     ):
         Item.__init__(
             self,
             usage_rules=usage_rules,
             issued_at=issued_at,
             expires_in=expires_in,
             expires_at=expires_at,
@@ -167,30 +167,33 @@
 
             if based_on.based_on:
                 return self.find_scope(based_on.based_on)
 
         return self.scope
 
     def add_acr_value(self, claims_release_point):
+        # if claims_release_point == "userinfo":
+        #     return False
+
         _release = self.claims.get(claims_release_point)
         if _release:
             _acr_request = _release.get("acr")
             _used_acr = self.authentication_event.get("authn_info")
             return claims_match(_used_acr, _acr_request)
         return False
 
     def payload_arguments(
-            self,
-            session_id: str,
-            context: object,
-            item: SessionToken,
-            claims_release_point: str,
-            scope: Optional[dict] = None,
-            extra_payload: Optional[dict] = None,
-            secondary_identifier: str = "",
+        self,
+        session_id: str,
+        context: object,
+        item: SessionToken,
+        claims_release_point: str,
+        scope: Optional[dict] = None,
+        extra_payload: Optional[dict] = None,
+        secondary_identifier: str = "",
     ) -> dict:
         """
 
         :param session_id: Session ID
         :param context: EndPoint Context
         :param item: A SessionToken instance
         :param claims_release_point: One of "userinfo", "introspection", "id_token", "access_token"
@@ -234,42 +237,41 @@
             _claims_restriction = context.claims_interface.get_claims(
                 session_id,
                 scopes=payload["scope"],
                 claims_release_point=claims_release_point,
                 secondary_identifier=secondary_identifier,
             )
 
-        if context.session_manager.node_type[0] == "user":
+        if _claims_restriction and context.session_manager.node_type[0] == "user":
             user_id, _, _ = context.session_manager.decrypt_branch_id(session_id)
-            user_info = context.claims_interface.get_user_claims(user_id,
-                                                                 _claims_restriction)
+            user_info = context.claims_interface.get_user_claims(user_id, _claims_restriction)
             payload.update(user_info)
 
         # Should I add the acr value
         if self.add_acr_value(claims_release_point):
             payload["acr"] = self.authentication_event["authn_info"]
         elif self.add_acr_value(secondary_identifier):
             payload["acr"] = self.authentication_event["authn_info"]
 
         return payload
 
     def mint_token(
-            self,
-            session_id: str,
-            context: object,
-            token_class: str,
-            token_handler: TokenHandler = None,
-            based_on: Optional[SessionToken] = None,
-            usage_rules: Optional[dict] = None,
-            scope: Optional[list] = None,
-            token_type: Optional[str] = "",
-            expires_in: Optional[int] = 0,
-            not_before: Optional[int] = 0,
-            claims: Optional[List[str]] = None,
-            **kwargs,
+        self,
+        session_id: str,
+        context: object,
+        token_class: str,
+        token_handler: TokenHandler = None,
+        based_on: Optional[SessionToken] = None,
+        usage_rules: Optional[dict] = None,
+        scope: Optional[list] = None,
+        token_type: Optional[str] = "",
+        expires_in: Optional[int] = 0,
+        not_before: Optional[int] = 0,
+        claims: Optional[List[str]] = None,
+        **kwargs,
     ) -> Optional[SessionToken]:
         """
 
         :param session_id:
         :param context:
         :param token_type:
         :param token_handler:
@@ -385,15 +387,15 @@
     def get_token(self, value: str) -> Optional[SessionToken]:
         for t in self.issued_token:
             if t.value == value:
                 return t
         return None
 
     def revoke_token(
-            self, value: Optional[str] = "", based_on: Optional[str] = "", recursive: bool = True
+        self, value: Optional[str] = "", based_on: Optional[str] = "", recursive: bool = True
     ):
         remain = []
         for t in self.issued_token:
             if not value and not based_on:
                 t.revoked = True
             elif value and based_on:
                 if value == t.value and based_on == t.based_on:
@@ -480,32 +482,32 @@
 
 class ExchangeGrant(Grant):
     parameter = Grant.parameter.copy()
     parameter.update({"exchange_request": TokenExchangeRequest, "original_session_id": ""})
     type = "exchange_grant"
 
     def __init__(
-            self,
-            scope: Optional[list] = None,
-            claims: Optional[dict] = None,
-            resources: Optional[list] = None,
-            authorization_details: Optional[dict] = None,
-            authorization_request: Optional[Message] = None,
-            authentication_event: Optional[AuthnEvent] = None,
-            issued_token: Optional[list] = None,
-            usage_rules: Optional[dict] = None,
-            exchange_request: Optional[TokenExchangeRequest] = None,
-            original_branch_id: str = "",
-            issued_at: int = 0,
-            expires_in: int = 0,
-            expires_at: int = 0,
-            revoked: bool = False,
-            token_map: Optional[dict] = None,
-            users: list = None,
-            sub: Optional[str] = "",
+        self,
+        scope: Optional[list] = None,
+        claims: Optional[dict] = None,
+        resources: Optional[list] = None,
+        authorization_details: Optional[dict] = None,
+        authorization_request: Optional[Message] = None,
+        authentication_event: Optional[AuthnEvent] = None,
+        issued_token: Optional[list] = None,
+        usage_rules: Optional[dict] = None,
+        exchange_request: Optional[TokenExchangeRequest] = None,
+        original_branch_id: str = "",
+        issued_at: int = 0,
+        expires_in: int = 0,
+        expires_at: int = 0,
+        revoked: bool = False,
+        token_map: Optional[dict] = None,
+        users: list = None,
+        sub: Optional[str] = "",
     ):
         Grant.__init__(
             self,
             scope=scope,
             claims=claims,
             resources=resources,
             authorization_details=authorization_details,
@@ -525,22 +527,22 @@
         self.usage_rules = {
             "access_token": {"supports_minting": ["access_token"], "expires_in": 60}
         }
         self.exchange_request = exchange_request
         self.original_branch_id = original_branch_id
 
     def payload_arguments(
-            self,
-            session_id: str,
-            endpoint_context,
-            item: SessionToken,
-            claims_release_point: str,
-            scope: Optional[dict] = None,
-            extra_payload: Optional[dict] = None,
-            secondary_identifier: str = "",
+        self,
+        session_id: str,
+        endpoint_context,
+        item: SessionToken,
+        claims_release_point: str,
+        scope: Optional[dict] = None,
+        extra_payload: Optional[dict] = None,
+        secondary_identifier: str = "",
     ) -> dict:
         """
         :param session_id: Session ID
         :param endpoint_context: EndPoint Context
         :param claims_release_point: One of "userinfo", "introspection", "id_token", "access_token"
         :param scope: scope from the request
         :param extra_payload:
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/session/grant_manager.py` & `idpyoidc-2.1.0/src/idpyoidc/server/session/grant_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,25 +24,25 @@
 
 
 class GrantManager(Database):
     parameter = Database.parameter.copy()
     init_args = ["handler"]
 
     def __init__(
-            self,
-            handler: TokenHandler,
-            conf: Optional[dict] = None,
-            remember_token: Optional[Callable] = None,
-            remove_inactive_token: Optional[bool] = False,
+        self,
+        handler: TokenHandler,
+        conf: Optional[dict] = None,
+        remember_token: Optional[Callable] = None,
+        remove_inactive_token: Optional[bool] = False,
     ):
         self.conf = conf or {
             "session_params": {
                 "encrypter": default_crypt_config(),
                 "node_type": ["client", "grant"],
-                "node_info_class": {"client": ClientSessionInfo, "grant": Grant}
+                "node_info_class": {"client": ClientSessionInfo, "grant": Grant},
             }
         }
 
         session_params = self.conf.get("session_params") or {}
         _crypt_config = get_crypt_config(session_params)
         super(GrantManager, self).__init__(_crypt_config, **self.conf)
 
@@ -65,36 +65,36 @@
         return self.get(self.decrypt_branch_id(branch_id))
 
     def __setitem__(self, branch_id: str, value):
         return self.set(self.decrypt_branch_id(branch_id), value)
 
     def _setup_branch(self, path):
         for i in range(len(path)):
-            _id = path[0:i + 1]
+            _id = path[0 : i + 1]
 
             try:
                 _si = self.get(_id)
             except KeyError:
                 _info_class = self.node_info_class[self.node_type[i]]
                 _si = _info_class(id=_id[i])
                 self.set(_id, _si)
 
     def _get_nodes(self, path):
         res = []
         for i in range(len(path)):
-            _id = path[0:i + 1]
+            _id = path[0 : i + 1]
             res.append(self.get(_id))
         return res
 
     def add_grant(
-            self,
-            path: List[str],
-            token_usage_rules: Optional[dict] = None,
-            scope: Optional[list] = None,
-            **kwargs
+        self,
+        path: List[str],
+        token_usage_rules: Optional[dict] = None,
+        scope: Optional[list] = None,
+        **kwargs,
     ) -> str:
         """
         Creates a Grant instance and adds it as a leaf to a branch
 
         :param path: The nodes in a branch
         :param token_usage_rules:
         :return: A branch ID
@@ -107,30 +107,30 @@
         if "usage_rules" not in grant_args and token_usage_rules:
             grant_args["usage_rules"] = token_usage_rules
 
         grant = Grant(
             remember_token=self.remember_token,
             remove_inactive_token=self.remove_inactive_token,
             scope=scope,
-            **grant_args
+            **grant_args,
         )
 
         _id = path[:]
         _id.append(grant.id)
         self.set(_id, grant)
 
         return self.encrypted_branch_id(*_id)
 
     def add_exchange_grant(
-            self,
-            exchange_request: TokenExchangeRequest,
-            original_branch_id: str,
-            path: List[str],
-            token_usage_rules: Optional[dict] = None,
-            **grant_args
+        self,
+        exchange_request: TokenExchangeRequest,
+        original_branch_id: str,
+        path: List[str],
+        token_usage_rules: Optional[dict] = None,
+        **grant_args,
     ) -> str:
         """
 
         :param scopes: Scopes
         :param exchange_request:
         :param original_branch_id:
         :param path: list of strings identifying the nodes in the branch
@@ -152,16 +152,17 @@
 
         _id = path[:]
         _id.append(grant.id)
         self.set(_id, grant)
 
         return self.encrypted_branch_id(*_id)
 
-    def get_node_info(self, branch_id: str, level: Optional[int] = None,
-                      node_type: Optional[str] = None) -> (str, NodeInfo):
+    def get_node_info(
+        self, branch_id: str, level: Optional[int] = None, node_type: Optional[str] = None
+    ) -> (str, NodeInfo):
         """
         Return session information for a specific node in the grant path.
 
         :param branch_id: Session identifier
         :param level:
         :param node_type: Type of node, MUST appear in the node_type
         :return: NodeInfo instance
@@ -169,15 +170,15 @@
         _path = self.decrypt_branch_id(branch_id)
         if level is None:
             if node_type:
                 level = self.node_type.index(node_type)
             else:
                 raise ValueError("One of level or node_type MUST be defined")
 
-        return _path[level], self.get(_path[0:level + 1])
+        return _path[level], self.get(_path[0 : level + 1])
 
     def branch_info(self, branch_id: str, *args) -> dict:
         """
         Returns information about the branch
 
         :param branch_id: Session identifier
         :return: dict with node identifiers as keys and NodeInfo instances as values
@@ -226,30 +227,30 @@
         """
         _path = self.decrypt_branch_id(branch_id)
         if level is None:
             _node = self.get(_path)
         else:
             if level > len(_path):
                 raise ValueError("Looking for level beyond what is available")
-            _node = self.get(_path[0:level + 1])
+            _node = self.get(_path[0 : level + 1])
         self._revoke_tree(_node)
 
     def _grants(self, path):
         _res = []
         for s in self.get_subordinates(path):
             if isinstance(s, Grant):
                 _res.append(s)
             else:
                 _res.extend(self._grants(self.unpack_branch_key(s)))
         return _res
 
     def grants(
-            self,
-            branch_id: Optional[str] = "",
-            path: Optional[List[str]] = "",
+        self,
+        branch_id: Optional[str] = "",
+        path: Optional[List[str]] = "",
     ) -> List[Grant]:
         """
         Find all grants connected to a branch
 
         :param path:
         :param branch_id: A session identifier
         :return: A list of grants
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/session/info.py` & `idpyoidc-2.1.0/src/idpyoidc/server/session/info.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/session/manager.py` & `idpyoidc-2.1.0/src/idpyoidc/server/session/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     def __init__(self, salt: Optional[str] = "", filename: Optional[str] = ""):
         if salt:
             self.salt = salt
         elif filename:
             if os.path.isfile(filename):
                 self.salt = open(filename).read()
             elif not os.path.isfile(filename) and os.path.exists(
-                    filename
+                filename
             ):  # Not a file, Something else
                 raise ConfigurationError("Salt filename points to something that is not a file")
             else:
                 self.salt = rndstr(24)
                 # May raise an exception
                 fp = open(filename, "w")
                 fp.write(self.salt)
@@ -79,39 +79,37 @@
 
 class SessionManager(GrantManager):
     parameter = Database.parameter.copy()
     # parameter.update({"salt": ""})
     init_args = ["handler"]
 
     def __init__(
-            self,
-            handler: TokenHandler,
-            conf: Optional[dict] = None,
-            sub_func: Optional[dict] = None,
-            remember_token: Optional[Callable] = None,
-            remove_inactive_token: Optional[bool] = False,
+        self,
+        handler: TokenHandler,
+        conf: Optional[dict] = None,
+        sub_func: Optional[dict] = None,
+        remember_token: Optional[Callable] = None,
+        remove_inactive_token: Optional[bool] = False,
     ):
         self.conf = conf or {"session_params": {"encrypter": default_crypt_config()}}
 
         session_params = self.conf.get("session_params") or {}
         super(SessionManager, self).__init__(handler, self.conf)
 
         self.node_type = session_params.get("node_type", ["user", "client", "grant"])
         # Make sure node_type is a list and must contain at least one element.
         if not isinstance(self.node_type, list):
             raise ValueError("Wrong type of value for SessionManager node_type")
         if len(self.node_type) == 0:
             raise ValueError("SessionManager node_type must at least contain one value")
 
-        self.node_info_class = session_params.get("node_info_class",
-                                                  {
-                                                      "user": UserSessionInfo,
-                                                      "client": ClientSessionInfo,
-                                                      "grant": Grant
-                                                  })
+        self.node_info_class = session_params.get(
+            "node_info_class",
+            {"user": UserSessionInfo, "client": ClientSessionInfo, "grant": Grant},
+        )
 
         self.token_handler = handler
         self.remember_token = remember_token
         self.remove_inactive_token = remove_inactive_token
 
         # this allows the subject identifier minters to be defined by someone
         # else then me.
@@ -157,22 +155,22 @@
         _path = []
         for typ in self.node_type[:-1]:
             _id_type = f"{typ}_id"
             _path.append(kwargs[_id_type])
         return _path
 
     def create_grant(
-            self,
-            authn_event: AuthnEvent,
-            auth_req: AuthorizationRequest,
-            user_id: Optional[str] = "",
-            client_id: Optional[str] = "",
-            sub_type: Optional[str] = "public",
-            token_usage_rules: Optional[dict] = None,
-            scopes: Optional[list] = None,
+        self,
+        authn_event: AuthnEvent,
+        auth_req: AuthorizationRequest,
+        user_id: Optional[str] = "",
+        client_id: Optional[str] = "",
+        sub_type: Optional[str] = "public",
+        token_usage_rules: Optional[dict] = None,
+        scopes: Optional[list] = None,
     ) -> str:
         """
 
         :param scopes: Scopes
         :param authn_event: AuthnEvent instance
         :param auth_req:
         :param user_id:
@@ -207,23 +205,23 @@
             claims=_claims,
             remember_token=self.remember_token,
             remove_inactive_token=self.remove_inactive_token,
             resources=resources,
         )
 
     def create_exchange_grant(
-            self,
-            exchange_request: TokenExchangeRequest,
-            original_grant: Grant,
-            original_session_id: str,
-            user_id: str,
-            client_id: Optional[str] = "",
-            sub_type: Optional[str] = "public",
-            token_usage_rules: Optional[dict] = None,
-            scopes: Optional[list] = None,
+        self,
+        exchange_request: TokenExchangeRequest,
+        original_grant: Grant,
+        original_session_id: str,
+        user_id: str,
+        client_id: Optional[str] = "",
+        sub_type: Optional[str] = "public",
+        token_usage_rules: Optional[dict] = None,
+        scopes: Optional[list] = None,
     ) -> str:
         """
 
         :param scopes: Scopes
         :param exchange_req:
         :param user_id:
         :param client_id:
@@ -235,26 +233,26 @@
             authentication_event=original_grant.authentication_event,
             authorization_request=original_grant.authorization_request,
             exchange_request=exchange_request,
             original_branch_id=original_session_id,
             path=self.make_path(user_id=user_id, client_id=client_id),
             sub=original_grant.sub,
             token_usage_rules=token_usage_rules,
-            scope=scopes
+            scope=scopes,
         )
 
     def create_session(
-            self,
-            authn_event: AuthnEvent,
-            auth_req: AuthorizationRequest,
-            user_id: Optional[str] = "",
-            client_id: Optional[str] = "",
-            sub_type: Optional[str] = "public",
-            token_usage_rules: Optional[dict] = None,
-            scopes: Optional[list] = None,
+        self,
+        authn_event: AuthnEvent,
+        auth_req: AuthorizationRequest,
+        user_id: Optional[str] = "",
+        client_id: Optional[str] = "",
+        sub_type: Optional[str] = "public",
+        token_usage_rules: Optional[dict] = None,
+        scopes: Optional[list] = None,
     ) -> str:
         """
         Create part of a user session. The parts added are user- and client
         information and a grant.
 
         :param scopes:
         :param authn_event: Authentication Event information
@@ -273,23 +271,23 @@
             client_id=client_id,
             sub_type=sub_type,
             token_usage_rules=token_usage_rules,
             scopes=scopes,
         )
 
     def create_exchange_session(
-            self,
-            exchange_request: TokenExchangeRequest,
-            original_grant: Grant,
-            original_session_id: str,
-            user_id: str,
-            client_id: Optional[str] = "",
-            sub_type: Optional[str] = "public",
-            token_usage_rules: Optional[dict] = None,
-            scopes: Optional[list] = None,
+        self,
+        exchange_request: TokenExchangeRequest,
+        original_grant: Grant,
+        original_session_id: str,
+        user_id: str,
+        client_id: Optional[str] = "",
+        sub_type: Optional[str] = "public",
+        token_usage_rules: Optional[dict] = None,
+        scopes: Optional[list] = None,
     ) -> str:
         """
         Create part of a user session. The parts added are user- and client
         information and a grant.
 
         :param scopes:
         :param authn_event: Authentication Event information
@@ -315,43 +313,43 @@
     def get_client_session_info(self, session_id: str) -> ClientSessionInfo:
         """
         Return client connected information for a user session.
 
         :param session_id: Session identifier
         :return: ClientSessionInfo instance
         """
-        _id, csi = self.get_node_info(session_id, node_type='client')
+        _id, csi = self.get_node_info(session_id, node_type="client")
 
         if isinstance(csi, ClientSessionInfo):
             return csi
         else:  # pragma: no cover
             raise ValueError("Wrong type of session info")
 
     def get_user_session_info(self, session_id: str) -> UserSessionInfo:
         """
         Return client connected information for a user session.
 
         :param session_id: Session identifier
         :return: ClientSessionInfo instance
         """
-        _id, usi = self.get_node_info(session_id, node_type='user')
+        _id, usi = self.get_node_info(session_id, node_type="user")
 
         if isinstance(usi, UserSessionInfo):
             return usi
         else:  # pragma: no cover
             raise ValueError("Wrong type of session info")
 
     def get_grant(self, session_id: str) -> Grant:
         """
         Return client connected information for a user session.
 
         :param session_id: Session identifier
         :return: ClientSessionInfo instance
         """
-        _id, grant = self.get_node_info(session_id, node_type='grant')
+        _id, grant = self.get_node_info(session_id, node_type="grant")
 
         if isinstance(grant, Grant):
             return grant
         else:  # pragma: no cover
             raise ValueError("Wrong type of item")
 
     def revoke_token(self, session_id: str, token_value: str, recursive: bool = False):
@@ -369,29 +367,29 @@
 
         token.revoked = True
         if recursive:  # TODO: not covered yet!
             grant = self[session_id]
             grant.revoke_token(value=token.value)
 
     def get_authentication_events(
-            self,
-            session_id: Optional[str] = "",
-            user_id: Optional[str] = "",
-            client_id: Optional[str] = "",
+        self,
+        session_id: Optional[str] = "",
+        user_id: Optional[str] = "",
+        client_id: Optional[str] = "",
     ) -> List[AuthnEvent]:
         """
         Return the authentication events that exists for a user/client combination.
 
         :param client_id:
         :param user_id:
         :param session_id: A session identifier
         :return: None if no authentication event could be found or an AuthnEvent instance.
         """
         if session_id:
-            cid, c_info = self.get_node_info(session_id, node_type='client')
+            cid, c_info = self.get_node_info(session_id, node_type="client")
         elif user_id and client_id:
             c_info = self.get([user_id, client_id])
         else:
             raise AttributeError("Must have session_id or user_id and client_id")
 
         _grants = [self.get(self.unpack_branch_key(gid)) for gid in c_info.subordinate]
         return [g.authentication_event for g in _grants]
@@ -446,21 +444,21 @@
     #     else:
     #         raise AttributeError("Must have session_id or user_id and client_id")
     #
     #     _csi = self.get([user_id, client_id])
     #     return [self.get([user_id, client_id, gid]) for gid in _csi.subordinate]
 
     def get_session_info(
-            self,
-            session_id: str,
-            user_session_info: bool = False,
-            client_session_info: bool = False,
-            grant: bool = False,
-            authentication_event: bool = False,
-            authorization_request: bool = False,
+        self,
+        session_id: str,
+        user_session_info: bool = False,
+        client_session_info: bool = False,
+        grant: bool = False,
+        authentication_event: bool = False,
+        authorization_request: bool = False,
     ) -> dict:
         """
         Returns information connected to a session.
 
         :param session_id: The identifier of the session
         :param user_session_info: Whether user session info should part of the response
         :param client_session_info: Whether client session info should part of the response
@@ -477,22 +475,22 @@
 
         if authorization_request:
             res["authorization_request"] = res["grant"].authorization_request
 
         return res
 
     def get_session_info_by_token(
-            self,
-            token_value: str,
-            user_session_info: Optional[bool] = False,
-            client_session_info: Optional[bool] = False,
-            grant: Optional[bool] = False,
-            authentication_event: Optional[bool] = False,
-            authorization_request: Optional[bool] = False,
-            handler_key: Optional[str] = "",
+        self,
+        token_value: str,
+        user_session_info: Optional[bool] = False,
+        client_session_info: Optional[bool] = False,
+        grant: Optional[bool] = False,
+        authentication_event: Optional[bool] = False,
+        authorization_request: Optional[bool] = False,
+        handler_key: Optional[str] = "",
     ) -> dict:
 
         if handler_key:
             _token_info = self.token_handler.handler[handler_key].info(token_value)
         else:
             _token_info = self.token_handler.info(token_value)
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/session/token.py` & `idpyoidc-2.1.0/src/idpyoidc/server/session/token.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/token/__init__.py` & `idpyoidc-2.1.0/src/idpyoidc/server/token/__init__.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/token/handler.py` & `idpyoidc-2.1.0/src/idpyoidc/server/token/handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 logger = logging.getLogger(__name__)
 
 
 class TokenHandler(ImpExp):
     parameter = {"handler": DLDict, "handler_order": [""]}
 
     def __init__(
-            self,
-            access_token: Optional[Token] = None,
-            authorization_code: Optional[Token] = None,
-            refresh_token: Optional[Token] = None,
-            id_token: Optional[Token] = None,
+        self,
+        access_token: Optional[Token] = None,
+        authorization_code: Optional[Token] = None,
+        refresh_token: Optional[Token] = None,
+        id_token: Optional[Token] = None,
     ):
         ImpExp.__init__(self)
         self.handler = {"authorization_code": authorization_code, "access_token": access_token}
 
         self.handler_order = ["authorization_code", "access_token"]
 
         if refresh_token:
@@ -137,21 +137,21 @@
         return False
 
 
 JWKS_FILE = "private/token_jwks.json"
 
 
 def factory(
-        upstream_get,
-        code: Optional[dict] = None,
-        token: Optional[dict] = None,
-        refresh: Optional[dict] = None,
-        id_token: Optional[dict] = None,
-        jwks_file: Optional[str] = "",
-        **kwargs
+    upstream_get,
+    code: Optional[dict] = None,
+    token: Optional[dict] = None,
+    refresh: Optional[dict] = None,
+    id_token: Optional[dict] = None,
+    jwks_file: Optional[str] = "",
+    **kwargs
 ) -> TokenHandler:
     """
     Create a token handler
 
     :param code:
     :param token:
     :param refresh:
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/token/id_token.py` & `idpyoidc-2.1.0/src/idpyoidc/server/token/id_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,17 +53,15 @@
         context.cdb[client_id]["{}channel_logout_uri".format(where)]
     except KeyError:
         return False
 
     return True
 
 
-def get_sign_and_encrypt_algorithms(
-    context, client_info, payload_type, sign=False, encrypt=False
-):
+def get_sign_and_encrypt_algorithms(context, client_info, payload_type, sign=False, encrypt=False):
     args = {"sign": sign, "encrypt": encrypt}
     if sign:
         try:
             args["sign_alg"] = client_info["{}_signed_response_alg".format(payload_type)]
         except KeyError:  # Fall back to default
             try:
                 args["sign_alg"] = context.jwx_def["signing_alg"][payload_type]
@@ -253,18 +251,19 @@
             user_info=user_info,
         )
 
         if lifetime is None:
             lifetime = self.lifetime
 
         _jwt = JWT(
-            self.upstream_get('attribute', 'keyjar'),
+            self.upstream_get("attribute", "keyjar"),
             iss=_context.issuer,
             lifetime=lifetime,
-            **alg_dict)
+            **alg_dict,
+        )
 
         return _jwt.pack(_payload, recv=client_id)
 
     def __call__(
         self,
         session_id: Optional[str] = "",
         ttype: Optional[str] = "",
@@ -320,16 +319,16 @@
 
         _payload = _jwt.jwt.payload()
         client_id = _payload["aud"][0]
         client_info = _context.cdb[client_id]
         alg_dict = get_sign_and_encrypt_algorithms(_context, client_info, "id_token", sign=True)
 
         verifier = JWT(
-            key_jar=self.upstream_get('attribute', 'keyjar'),
-            allowed_sign_algs=alg_dict["sign_alg"])
+            key_jar=self.upstream_get("attribute", "keyjar"), allowed_sign_algs=alg_dict["sign_alg"]
+        )
         try:
             _payload = verifier.unpack(token)
         except JWSException:
             raise UnknownToken()
 
         logger.debug(f"Received ID Token payload: {_payload}")
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/token/jwt_token.py` & `idpyoidc-2.1.0/src/idpyoidc/server/token/jwt_token.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,28 +13,27 @@
 from .exception import WrongTokenClass
 from ..constant import DEFAULT_TOKEN_LIFETIME
 from ...message import Message
 from ...message.oauth2 import JWTAccessToken
 
 
 class JWTToken(Token):
-
     def __init__(
-            self,
-            token_class,
-            # keyjar: KeyJar = None,
-            issuer: str = None,
-            aud: Optional[list] = None,
-            alg: str = "ES256",
-            lifetime: int = DEFAULT_TOKEN_LIFETIME,
-            upstream_get: Callable = None,
-            token_type: str = "Bearer",
-            profile: Optional[Union[Message, str]] = JWTAccessToken,
-            with_jti: Optional[bool] = False,
-            **kwargs
+        self,
+        token_class,
+        # keyjar: KeyJar = None,
+        issuer: str = None,
+        aud: Optional[list] = None,
+        alg: str = "ES256",
+        lifetime: int = DEFAULT_TOKEN_LIFETIME,
+        upstream_get: Callable = None,
+        token_type: str = "Bearer",
+        profile: Optional[Union[Message, str]] = JWTAccessToken,
+        with_jti: Optional[bool] = False,
+        **kwargs
     ):
         Token.__init__(self, token_class, **kwargs)
         self.token_type = token_type
         self.lifetime = lifetime
 
         self.kwargs = kwargs
         _context = upstream_get("context")
@@ -55,21 +54,21 @@
             self.with_jti = True
 
     def load_custom_claims(self, payload: dict = None):
         # inherit me and do your things here
         return payload
 
     def __call__(
-            self,
-            session_id: Optional[str] = "",
-            token_class: Optional[str] = "",
-            usage_rules: Optional[dict] = None,
-            profile: Optional[Message] = None,
-            with_jti: Optional[bool] = None,
-            **payload
+        self,
+        session_id: Optional[str] = "",
+        token_class: Optional[str] = "",
+        usage_rules: Optional[dict] = None,
+        profile: Optional[Message] = None,
+        with_jti: Optional[bool] = None,
+        **payload
     ) -> str:
         """
         Return a token.
 
         :param session_id: Session id
         :param token_class: Token class
         :param payload: A dictionary with information that is part of the payload of the JWT.
@@ -86,15 +85,15 @@
 
         # payload.update(kwargs)
         if usage_rules and "expires_in" in usage_rules:
             lifetime = usage_rules.get("expires_in")
         else:
             lifetime = self.lifetime
         signer = JWT(
-            key_jar=self.upstream_get('attribute', 'keyjar'),
+            key_jar=self.upstream_get("attribute", "keyjar"),
             iss=self.issuer,
             lifetime=lifetime,
             sign_alg=self.alg,
         )
         if isinstance(payload, Message):  # don't mess with it.
             pass
         else:
@@ -107,16 +106,17 @@
             signer.with_jti = True
         elif with_jti is None:
             signer.with_jti = self.with_jti
 
         return signer.pack(payload)
 
     def get_payload(self, token):
-        verifier = JWT(key_jar=self.upstream_get('attribute', 'keyjar'),
-                       allowed_sign_algs=[self.alg])
+        verifier = JWT(
+            key_jar=self.upstream_get("attribute", "keyjar"), allowed_sign_algs=[self.alg]
+        )
         try:
             _payload = verifier.unpack(token)
         except JWSException:
             raise UnknownToken()
 
         return _payload
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/user_authn/authn_context.py` & `idpyoidc-2.1.0/src/idpyoidc/server/user_authn/authn_context.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/user_authn/user.py` & `idpyoidc-2.1.0/src/idpyoidc/server/user_authn/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,16 +115,21 @@
             for val in cookie:
                 _info = json.loads(val["value"])
                 _info["timestamp"] = int(val["timestamp"])
 
                 # verify session ID
                 try:
                     _context.session_manager[_info["sid"]]
-                except (KeyError, ValueError, InconsistentDatabase,
-                        NoSuchClientSession, NoSuchGrant) as err:
+                except (
+                    KeyError,
+                    ValueError,
+                    InconsistentDatabase,
+                    NoSuchClientSession,
+                    NoSuchGrant,
+                ) as err:
                     logger.info(f"Verifying session ID fail due to {err}")
                     return {}
 
                 session_id = _context.session_manager.decrypt_session_id(_info["sid"])
                 logger.debug("cookie_info: session id={}".format(session_id))
 
                 if session_id[1] != client_id:
@@ -149,21 +154,21 @@
 LABELS = {"tos_uri": "Terms of Service", "policy_uri": "Service policy", "logo_uri": ""}
 
 
 class UserPassJinja2(UserAuthnMethod):
     url_endpoint = "/verify/user_pass_jinja"
 
     def __init__(
-            self,
-            db,
-            template_handler,
-            template="user_pass.jinja2",
-            upstream_get=None,
-            verify_endpoint="",
-            **kwargs,
+        self,
+        db,
+        template_handler,
+        template="user_pass.jinja2",
+        upstream_get=None,
+        verify_endpoint="",
+        **kwargs,
     ):
 
         super(UserPassJinja2, self).__init__(upstream_get=upstream_get)
         self.template_handler = template_handler
         self.template = template
 
         self.action = verify_endpoint or self.url_endpoint
@@ -189,15 +194,15 @@
                 "production environment"
             ),
             OnlyForTestingWarning,
         )
         if not self.upstream_get:
             raise Exception(f"{self.__class__.__name__} doesn't have a working upstream_get")
         _context = self.upstream_get("context")
-        _keyjar = self.upstream_get("attribute", 'keyjar')
+        _keyjar = self.upstream_get("attribute", "keyjar")
         # Stores information need afterwards in a signed JWT that then
         # appears as a hidden input in the form
         jws = create_signed_jwt(_context.issuer, _keyjar, **kwargs)
         _kwargs = self.kwargs.copy()
         for attr in ["policy", "tos", "logo"]:
             _uri = "{}_uri".format(attr)
             try:
@@ -215,20 +220,19 @@
         if username in self.user_db and self.user_db[username] == kwargs["password"]:
             return username
         else:
             raise FailedAuthentication()
 
 
 class UserPass(UserAuthnMethod):
-
     def __init__(
-            self,
-            db_conf,
-            upstream_get=None,
-            **kwargs,
+        self,
+        db_conf,
+        upstream_get=None,
+        **kwargs,
     ):
 
         super(UserPass, self).__init__(upstream_get=upstream_get)
         self.user_db = instantiate(db_conf["class"], **db_conf["kwargs"])
 
     def __call__(self, **kwargs):
         pass
@@ -238,15 +242,14 @@
         if username in self.user_db and self.user_db[username] == kwargs["password"]:
             return username
         else:
             raise FailedAuthentication()
 
 
 class BasicAuthn(UserAuthnMethod):
-
     def __init__(self, pwd, ttl=5, upstream_get=None):
         UserAuthnMethod.__init__(self, upstream_get=upstream_get)
         self.passwd = pwd
         self.ttl = ttl
 
     def verify_password(self, user, password):
         if password != self.passwd[user]:
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/user_info/__init__.py` & `idpyoidc-2.1.0/src/idpyoidc/server/user_info/__init__.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/server/util.py` & `idpyoidc-2.1.0/src/idpyoidc/server/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 
         endpoint[_instance.name] = _instance
 
     return endpoint
 
 
 class JSONDictDB(object):
-
     def __init__(self, filename):
         with open(filename, "r") as f:
             self._db = json.load(f)
 
     def __getitem__(self, item):
         return self._db[item]
 
@@ -90,15 +89,15 @@
     :return: a list og values
     """
     txt = txt.strip()
     res = []
     while txt:
         l, v = txt.split(":", 1)
         res.append(v[: int(l)])
-        txt = v[int(l):]
+        txt = v[int(l) :]
     return res
 
 
 def get_http_params(config):
     _verify_ssl = config.get("verify")
     if _verify_ssl is None:
         _verify_ssl = config.get("verify_ssl")
@@ -119,17 +118,17 @@
         raise ValueError("Key without cert is no good")
 
     return params
 
 
 def allow_refresh_token(context):
     # Are there a refresh_token handler
-    refresh_token_handler = context.session_manager.token_handler.handler.get(
-        "refresh_token"
-    )
+    refresh_token_handler = context.session_manager.token_handler.handler.get("refresh_token")
+    if refresh_token_handler is None:
+        return False
 
     # Is refresh_token grant type supported
     _token_supported = False
     _supported = context.get_preference("grant_types_supported")
     if _supported:
         if "refresh_token" in _supported:
             # self.allow_refresh = kwargs.get("allow_refresh", True)
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/ssl_context.py` & `idpyoidc-2.1.0/src/idpyoidc/ssl_context.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/src/idpyoidc/storage/abfile.py` & `idpyoidc-2.1.0/src/idpyoidc/storage/abfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,18 +20,19 @@
     Each key maps one-to-one to a file on disc, where the content of the
     file is the value.
     ONLY goes one level deep.
     Not directories in directories.
     """
 
     def __init__(
-        self, fdir: Optional[str] = "",
-            key_conv: Optional[str] = "",
-            value_conv: Optional[str] = "",
-            **kwargs
+        self,
+        fdir: Optional[str] = "",
+        key_conv: Optional[str] = "",
+        value_conv: Optional[str] = "",
+        **kwargs
     ):
         """
         items = FileSystem(
             {
                 'fdir': fdir,
                 'key_conv':{'to': quote_plus, 'from': unquote_plus},
                 'value_conv':{'to': keyjar_to_jwks, 'from': jwks_to_keyjar}
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/time_util.py` & `idpyoidc-2.1.0/src/idpyoidc/time_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,19 +100,19 @@
                     raise TimeUtilError("Not allowed to end with 'T'")
             else:
                 raise TimeUtilError("Missing T")
         else:
             try:
                 mod = duration[index:].index(code)
                 try:
-                    dic[typ] = int(duration[index: index + mod])
+                    dic[typ] = int(duration[index : index + mod])
                 except ValueError:
                     if code == "S":
                         try:
-                            dic[typ] = float(duration[index: index + mod])
+                            dic[typ] = float(duration[index : index + mod])
                         except ValueError:
                             raise TimeUtilError("Not a float")
                     else:
                         raise TimeUtilError("Fractions not allow on anything byt seconds")
                 index = mod + index + 1
             except ValueError:
                 dic[typ] = 0
@@ -181,15 +181,15 @@
     """
     delta = timedelta(days, seconds, microseconds, milliseconds, minutes, hours, weeks)
     res = datetime.now(timezone.utc) + delta
     return res.replace(tzinfo=None)
 
 
 def time_a_while_ago(
-        days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=0, weeks=0
+    days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=0, weeks=0
 ):
     """
     Will return a time specification for a time sometime in the past.
 
     :param days:
     :param seconds:
     :param microseconds:
@@ -201,22 +201,22 @@
     """
     delta = timedelta(days, seconds, microseconds, milliseconds, minutes, hours, weeks)
     res = datetime.now(timezone.utc) - delta
     return res.replace(tzinfo=None)
 
 
 def in_a_while(
-        days=0,
-        seconds=0,
-        microseconds=0,
-        milliseconds=0,
-        minutes=0,
-        hours=0,
-        weeks=0,
-        time_format=TIME_FORMAT,
+    days=0,
+    seconds=0,
+    microseconds=0,
+    milliseconds=0,
+    minutes=0,
+    hours=0,
+    weeks=0,
+    time_format=TIME_FORMAT,
 ):
     """
     :param days:
     :param seconds:
     :param microseconds:
     :param milliseconds:
     :param minutes:
@@ -230,22 +230,22 @@
 
     return time_in_a_while(
         days, seconds, microseconds, milliseconds, minutes, hours, weeks
     ).strftime(time_format)
 
 
 def a_while_ago(
-        days=0,
-        seconds=0,
-        microseconds=0,
-        milliseconds=0,
-        minutes=0,
-        hours=0,
-        weeks=0,
-        time_format=TIME_FORMAT,
+    days=0,
+    seconds=0,
+    microseconds=0,
+    milliseconds=0,
+    minutes=0,
+    hours=0,
+    weeks=0,
+    time_format=TIME_FORMAT,
 ):
     """
 
     :param days:
     :param seconds:
     :param microseconds:
     :param milliseconds:
@@ -357,15 +357,15 @@
 
 
 def time_sans_frac():
     return int("%d" % time.time())
 
 
 def epoch_in_a_while(
-        days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=0, weeks=0
+    days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=0, weeks=0
 ):
     """
     Return the number of seconds since epoch a while from now.
 
     :param days:
     :param seconds:
     :param microseconds:
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc/util.py` & `idpyoidc-2.1.0/src/idpyoidc/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,33 +80,30 @@
         return [base, None]
 
 
 # Converters
 
 
 class QPKey:
-
     def serialize(self, str):
         return quote_plus(str)
 
     def deserialize(self, str):
         return unquote_plus(str)
 
 
 class JSON:
-
     def serialize(self, str):
         return json.dumps(str)
 
     def deserialize(self, str):
         return json.loads(str)
 
 
 class PassThru:
-
     def serialize(self, str):
         return str
 
     def deserialize(self, str):
         return str
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc.egg-info/PKG-INFO` & `idpyoidc-2.1.0/src/idpyoidc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idpyoidc
-Version: 2.0.0
+Version: 2.1.0
 Summary: Python implementation of everything OAuth2 and OpenID Connect
 Home-page: https://github.com/IdentityPython/idpy-oidc/
 Author: Roland Hedberg
 Author-email: roland@catalogix.se
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `idpyoidc-2.0.0/src/idpyoidc.egg-info/SOURCES.txt` & `idpyoidc-2.1.0/src/idpyoidc.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,24 +43,30 @@
 src/idpyoidc/client/claims/oauth2.py
 src/idpyoidc/client/claims/oidc.py
 src/idpyoidc/client/claims/transform.py
 src/idpyoidc/client/oauth2/__init__.py
 src/idpyoidc/client/oauth2/access_token.py
 src/idpyoidc/client/oauth2/authorization.py
 src/idpyoidc/client/oauth2/client_credentials.py
+src/idpyoidc/client/oauth2/introspection.py
 src/idpyoidc/client/oauth2/refresh_access_token.py
+src/idpyoidc/client/oauth2/registration.py
+src/idpyoidc/client/oauth2/resource.py
 src/idpyoidc/client/oauth2/resource_owner_password_credentials.py
 src/idpyoidc/client/oauth2/server_metadata.py
+src/idpyoidc/client/oauth2/stand_alone_client.py
 src/idpyoidc/client/oauth2/token_exchange.py
+src/idpyoidc/client/oauth2/token_revocation.py
 src/idpyoidc/client/oauth2/utils.py
 src/idpyoidc/client/oauth2/add_on/__init__.py
 src/idpyoidc/client/oauth2/add_on/dpop.py
 src/idpyoidc/client/oauth2/add_on/identity_assurance.py
+src/idpyoidc/client/oauth2/add_on/jar.py
+src/idpyoidc/client/oauth2/add_on/par.py
 src/idpyoidc/client/oauth2/add_on/pkce.py
-src/idpyoidc/client/oauth2/add_on/pushed_authorization.py
 src/idpyoidc/client/oauth2/add_on/status_check.py
 src/idpyoidc/client/oidc/__init__.py
 src/idpyoidc/client/oidc/access_token.py
 src/idpyoidc/client/oidc/authorization.py
 src/idpyoidc/client/oidc/backchannel_authentication.py
 src/idpyoidc/client/oidc/check_id.py
 src/idpyoidc/client/oidc/check_session.py
@@ -107,14 +113,15 @@
 src/idpyoidc/server/oauth2/pushed_authorization.py
 src/idpyoidc/server/oauth2/server_metadata.py
 src/idpyoidc/server/oauth2/token.py
 src/idpyoidc/server/oauth2/token_revocation.py
 src/idpyoidc/server/oauth2/add_on/__init__.py
 src/idpyoidc/server/oauth2/add_on/dpop.py
 src/idpyoidc/server/oauth2/add_on/extra_args.py
+src/idpyoidc/server/oauth2/add_on/pkce.py
 src/idpyoidc/server/oauth2/token_helper/__init__.py
 src/idpyoidc/server/oauth2/token_helper/access_token.py
 src/idpyoidc/server/oauth2/token_helper/client_credentials.py
 src/idpyoidc/server/oauth2/token_helper/refresh_token.py
 src/idpyoidc/server/oauth2/token_helper/resource_owner_password_credentials.py
 src/idpyoidc/server/oauth2/token_helper/token_exchange.py
 src/idpyoidc/server/oidc/__init__.py
@@ -125,15 +132,14 @@
 src/idpyoidc/server/oidc/read_registration.py
 src/idpyoidc/server/oidc/registration.py
 src/idpyoidc/server/oidc/session.py
 src/idpyoidc/server/oidc/token.py
 src/idpyoidc/server/oidc/userinfo.py
 src/idpyoidc/server/oidc/add_on/__init__.py
 src/idpyoidc/server/oidc/add_on/custom_scopes.py
-src/idpyoidc/server/oidc/add_on/pkce.py
 src/idpyoidc/server/oidc/token_helper/__init__.py
 src/idpyoidc/server/oidc/token_helper/access_token.py
 src/idpyoidc/server/oidc/token_helper/refresh_token.py
 src/idpyoidc/server/oidc/token_helper/token_exchange.py
 src/idpyoidc/server/session/__init__.py
 src/idpyoidc/server/session/claims.py
 src/idpyoidc/server/session/database.py
@@ -187,16 +193,17 @@
 tests/test_client_21_oidc_service.py
 tests/test_client_22_oidc.py
 tests/test_client_23_pkce.py
 tests/test_client_24_oic_utils.py
 tests/test_client_25_oauth2_cc_ropc.py
 tests/test_client_26_read_registration.py
 tests/test_client_27_conversation.py
-tests/test_client_28_rp_handler_oidc.py
+tests/test_client_28_stand_alone.py
 tests/test_client_29_pushed_auth.py
+tests/test_client_30_rp_handler_oidc.py
 tests/test_client_30_rph_defaults.py
 tests/test_client_31_oauth2_persistent.py
 tests/test_client_32_oidc_persistent.py
 tests/test_client_40_dpop.py
 tests/test_client_41_rp_handler_persistent.py
 tests/test_client_50_ciba.py
 tests/test_client_51_identity_assurance.py
@@ -232,25 +239,31 @@
 tests/test_server_21_oidc_discovery_endpoint.py
 tests/test_server_22_oidc_provider_config_endpoint.py
 tests/test_server_23_oidc_registration_endpoint.py
 tests/test_server_24_oauth2_authorization_endpoint.py
 tests/test_server_24_oauth2_authorization_endpoint_jar.py
 tests/test_server_24_oauth2_resource_indicators.py
 tests/test_server_24_oauth2_token_endpoint.py
+tests/test_server_24_oauth2_token_endpoint_def_conf.py
 tests/test_server_24_oidc_authorization_endpoint.py
 tests/test_server_25_oauth2_cc_ropc.py
 tests/test_server_26_oidc_userinfo_endpoint.py
 tests/test_server_30_oidc_end_session.py
 tests/test_server_31_oauth2_introspection.py
 tests/test_server_32_oidc_read_registration.py
 tests/test_server_33_oauth2_pkce.py
 tests/test_server_34_oidc_sso.py
 tests/test_server_35_oidc_token_endpoint.py
+tests/test_server_35_oidc_token_endpoint_def_conf.py
 tests/test_server_36_oauth2_token_exchange.py
 tests/test_server_38_oauth2_revocation_endpoint.py
 tests/test_server_40_oauth2_pushed_authorization.py
 tests/test_server_50_persistence.py
 tests/test_server_60_dpop.py
 tests/test_server_61_add_on.py
-tests/test_tandem_08_oauth2_cc_ropc.py
-tests/test_tandem_10_oauth2_token_exchange.py
+tests/test_tandem_oauth2_add_on.py
+tests/test_tandem_oauth2_cc_ropc.py
+tests/test_tandem_oauth2_code.py
+tests/test_tandem_oauth2_token_exchange.py
+tests/test_tandem_oauth2_token_revocation.py
+tests/test_tandem_oidc_code.py
 tests/test_y_actor_01.py
```

### Comparing `idpyoidc-2.0.0/tests/test_01_util.py` & `idpyoidc-2.1.0/tests/test_01_util.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_03_time_util.py` & `idpyoidc-2.1.0/tests/test_03_time_util.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_04_message.py` & `idpyoidc-2.1.0/tests/test_04_message.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_05_oauth2.py` & `idpyoidc-2.1.0/tests/test_05_oauth2.py`

 * *Files 0% similar despite different names*

```diff
@@ -574,15 +574,15 @@
         ropc.verify()
         assert ropc["username"] == "johndoe"
         assert ropc["password"] == "A3ddj3w"
 
 
 class TestCCAccessTokenRequest(object):
     def test_init(self):
-        cc = CCAccessTokenRequest(scope="/foo", grant_type='client_credentials')
+        cc = CCAccessTokenRequest(scope="/foo", grant_type="client_credentials")
         cc.verify()
         assert cc["scope"] == ["/foo"]
 
 
 class TestRefreshAccessTokenRequest(object):
     def test_init(self):
         ratr = RefreshAccessTokenRequest(refresh_token="ababababab", client_id="Client_id")
```

### Comparing `idpyoidc-2.0.0/tests/test_06_oidc.py` & `idpyoidc-2.1.0/tests/test_06_oidc.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_07_session.py` & `idpyoidc-2.1.0/tests/test_07_session.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_08_transform.py` & `idpyoidc-2.1.0/tests/test_08_transform.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,203 +9,214 @@
 from idpyoidc.client.claims.transform import preferred_to_registered
 from idpyoidc.client.claims.transform import supported_to_preferred
 from idpyoidc.message.oidc import ProviderConfigurationResponse
 from idpyoidc.message.oidc import RegistrationRequest
 
 
 class TestTransform:
-
     @pytest.fixture(autouse=True)
     def setup(self):
         supported = OIDC_Claims._supports.copy()
         for service in [
-            'idpyoidc.client.oidc.access_token.AccessToken',
-            'idpyoidc.client.oidc.authorization.Authorization',
-            'idpyoidc.client.oidc.backchannel_authentication.BackChannelAuthentication',
-            'idpyoidc.client.oidc.backchannel_authentication.ClientNotification',
-            'idpyoidc.client.oidc.check_id.CheckID',
-            'idpyoidc.client.oidc.check_session.CheckSession',
-            'idpyoidc.client.oidc.end_session.EndSession',
-            'idpyoidc.client.oidc.provider_info_discovery.ProviderInfoDiscovery',
-            'idpyoidc.client.oidc.read_registration.RegistrationRead',
-            'idpyoidc.client.oidc.refresh_access_token.RefreshAccessToken',
-            'idpyoidc.client.oidc.registration.Registration',
-            'idpyoidc.client.oidc.userinfo.UserInfo',
-            'idpyoidc.client.oidc.webfinger.WebFinger'
+            "idpyoidc.client.oidc.access_token.AccessToken",
+            "idpyoidc.client.oidc.authorization.Authorization",
+            "idpyoidc.client.oidc.backchannel_authentication.BackChannelAuthentication",
+            "idpyoidc.client.oidc.backchannel_authentication.ClientNotification",
+            "idpyoidc.client.oidc.check_id.CheckID",
+            "idpyoidc.client.oidc.check_session.CheckSession",
+            "idpyoidc.client.oidc.end_session.EndSession",
+            "idpyoidc.client.oidc.provider_info_discovery.ProviderInfoDiscovery",
+            "idpyoidc.client.oidc.read_registration.RegistrationRead",
+            "idpyoidc.client.oidc.refresh_access_token.RefreshAccessToken",
+            "idpyoidc.client.oidc.registration.Registration",
+            "idpyoidc.client.oidc.userinfo.UserInfo",
+            "idpyoidc.client.oidc.webfinger.WebFinger",
         ]:
             cls = importer(service)
             supported.update(cls._supports)
 
         for key, val in supported.items():
             if isinstance(val, Callable):
                 supported[key] = val()
         # NOTE! Not checking rules
         self.supported = supported
 
     def test_supported(self):
         # These are all the available configuration parameters
         assert set(self.supported.keys()) == {
-            'acr_values_supported',
-            'application_type',
-            'backchannel_logout_session_required',
-            'backchannel_logout_supported',
-            'backchannel_logout_uri',
-            'callback_uris',
-            'client_id',
-            'client_name',
-            'client_secret',
-            'client_uri',
-            'contacts',
-            'default_max_age',
-            'encrypt_id_token_supported',
-            'encrypt_request_object_supported',
-            'encrypt_userinfo_supported',
-            'frontchannel_logout_session_required',
-            'frontchannel_logout_supported',
-            'frontchannel_logout_uri',
-            'id_token_encryption_alg_values_supported',
-            'id_token_encryption_enc_values_supported',
-            'id_token_signing_alg_values_supported',
-            'initiate_login_uri',
-            'jwks',
-            'jwks_uri',
-            'logo_uri',
-            'policy_uri',
-            'post_logout_redirect_uris',
-            'redirect_uris',
-            'request_object_encryption_alg_values_supported',
-            'request_object_encryption_enc_values_supported',
-            'request_object_signing_alg_values_supported',
-            'request_parameter',
-            'request_parameter_supported',
-            'request_uri_parameter_supported',
-            'request_uris',
-            'requests_dir',
-            'require_auth_time',
-            'response_modes_supported',
-            'response_types_supported',
-            'scopes_supported',
-            'sector_identifier_uri',
-            'subject_types_supported',
+            "acr_values_supported",
+            "application_type",
+            "backchannel_logout_session_required",
+            "backchannel_logout_supported",
+            "backchannel_logout_uri",
+            "callback_uris",
+            "client_id",
+            "client_name",
+            "client_secret",
+            "client_uri",
+            "contacts",
+            "default_max_age",
+            "encrypt_id_token_supported",
+            "encrypt_request_object_supported",
+            "encrypt_userinfo_supported",
+            "frontchannel_logout_session_required",
+            "frontchannel_logout_supported",
+            "frontchannel_logout_uri",
+            "id_token_encryption_alg_values_supported",
+            "id_token_encryption_enc_values_supported",
+            "id_token_signing_alg_values_supported",
+            "initiate_login_uri",
+            "jwks",
+            "jwks_uri",
+            "logo_uri",
+            "policy_uri",
+            "post_logout_redirect_uris",
+            "redirect_uris",
+            "request_object_encryption_alg_values_supported",
+            "request_object_encryption_enc_values_supported",
+            "request_object_signing_alg_values_supported",
+            "request_parameter",
+            "request_parameter_supported",
+            "request_uri_parameter_supported",
+            "request_uris",
+            "requests_dir",
+            "require_auth_time",
+            "response_modes_supported",
+            "response_types_supported",
+            "scopes_supported",
+            "sector_identifier_uri",
+            "subject_types_supported",
             # 'token_endpoint_auth_method',
-            'token_endpoint_auth_methods_supported',
-            'token_endpoint_auth_signing_alg_values_supported',
-            'tos_uri',
-            'userinfo_encryption_alg_values_supported',
-            'userinfo_encryption_enc_values_supported',
-            'userinfo_signing_alg_values_supported'}
+            "token_endpoint_auth_methods_supported",
+            "token_endpoint_auth_signing_alg_values_supported",
+            "tos_uri",
+            "userinfo_encryption_alg_values_supported",
+            "userinfo_encryption_enc_values_supported",
+            "userinfo_signing_alg_values_supported",
+        }
 
     def test_oidc_setup(self):
         # This is OP specified stuff
         assert set(ProviderConfigurationResponse.c_param.keys()).difference(
-            set(self.supported)) == {'authorization_endpoint',
-                                     'check_session_iframe',
-                                     'claim_types_supported',
-                                     'claims_locales_supported',
-                                     'claims_parameter_supported',
-                                     'claims_supported',
-                                     'display_values_supported',
-                                     'end_session_endpoint',
-                                     'error',
-                                     'error_description',
-                                     'error_uri',
-                                     'grant_types_supported',
-                                     'issuer',
-                                     'op_policy_uri',
-                                     'op_tos_uri',
-                                     'registration_endpoint',
-                                     'require_request_uri_registration',
-                                     'service_documentation',
-                                     'token_endpoint',
-                                     'ui_locales_supported',
-                                     'userinfo_endpoint',
-                                     'code_challenge_methods_supported'}
+            set(self.supported)
+        ) == {
+            "authorization_endpoint",
+            "check_session_iframe",
+            "claim_types_supported",
+            "claims_locales_supported",
+            "claims_parameter_supported",
+            "claims_supported",
+            "display_values_supported",
+            "end_session_endpoint",
+            "error",
+            "error_description",
+            "error_uri",
+            "grant_types_supported",
+            "issuer",
+            "op_policy_uri",
+            "op_tos_uri",
+            "registration_endpoint",
+            "require_request_uri_registration",
+            "service_documentation",
+            "token_endpoint",
+            "ui_locales_supported",
+            "userinfo_endpoint",
+            "code_challenge_methods_supported",
+        }
 
         # parameters that are not mapped against what the OP's provider info says
         assert set(self.supported).difference(
-            set(ProviderConfigurationResponse.c_param.keys())) == {'application_type',
-                                                                   'backchannel_logout_uri',
-                                                                   'callback_uris',
-                                                                   'client_id',
-                                                                   'client_name',
-                                                                   'client_secret',
-                                                                   'client_uri',
-                                                                   'contacts',
-                                                                   'default_max_age',
-                                                                   'encrypt_id_token_supported',
-                                                                   'encrypt_request_object_supported',
-                                                                   'encrypt_userinfo_supported',
-                                                                   'frontchannel_logout_uri',
-                                                                   'initiate_login_uri',
-                                                                   'jwks',
-                                                                   'logo_uri',
-                                                                   'policy_uri',
-                                                                   'post_logout_redirect_uris',
-                                                                   'redirect_uris',
-                                                                   'request_parameter',
-                                                                   'request_uris',
-                                                                   'requests_dir',
-                                                                   'require_auth_time',
-                                                                   'sector_identifier_uri',
-                                                                   'tos_uri'}
+            set(ProviderConfigurationResponse.c_param.keys())
+        ) == {
+            "application_type",
+            "backchannel_logout_uri",
+            "callback_uris",
+            "client_id",
+            "client_name",
+            "client_secret",
+            "client_uri",
+            "contacts",
+            "default_max_age",
+            "encrypt_id_token_supported",
+            "encrypt_request_object_supported",
+            "encrypt_userinfo_supported",
+            "frontchannel_logout_uri",
+            "initiate_login_uri",
+            "jwks",
+            "logo_uri",
+            "policy_uri",
+            "post_logout_redirect_uris",
+            "redirect_uris",
+            "request_parameter",
+            "request_uris",
+            "requests_dir",
+            "require_auth_time",
+            "sector_identifier_uri",
+            "tos_uri",
+        }
 
         claims = OIDC_Claims()
         # No input from the IDP so info is absent
-        claims.prefer = supported_to_preferred(supported=self.supported,
-                                                    preference=claims.prefer,
-                                                    base_url='https://example.com')
+        claims.prefer = supported_to_preferred(
+            supported=self.supported, preference=claims.prefer, base_url="https://example.com"
+        )
 
         # These are the claims that has default values. A default value may be an empty list.
         # This is the case for claims like id_token_encryption_enc_values_supported.
-        assert set(claims.prefer.keys()) == {'application_type',
-                                                  'default_max_age',
-                                                  'encrypt_request_object_supported',
-                                                  'encrypt_userinfo_supported',
-                                                  'id_token_encryption_alg_values_supported',
-                                                  'id_token_encryption_enc_values_supported',
-                                                  'id_token_signing_alg_values_supported',
-                                                  'request_object_encryption_alg_values_supported',
-                                                  'request_object_encryption_enc_values_supported',
-                                                  'request_object_signing_alg_values_supported',
-                                                  'response_modes_supported',
-                                                  'response_types_supported',
-                                                  'scopes_supported',
-                                                  'subject_types_supported',
-                                                  'token_endpoint_auth_methods_supported',
-                                                  'token_endpoint_auth_signing_alg_values_supported',
-                                                  'userinfo_encryption_alg_values_supported',
-                                                  'userinfo_encryption_enc_values_supported',
-                                                  'userinfo_signing_alg_values_supported'}
+        assert set(claims.prefer.keys()) == {
+            "application_type",
+            "default_max_age",
+            "encrypt_request_object_supported",
+            "encrypt_userinfo_supported",
+            "id_token_encryption_alg_values_supported",
+            "id_token_encryption_enc_values_supported",
+            "id_token_signing_alg_values_supported",
+            "request_object_encryption_alg_values_supported",
+            "request_object_encryption_enc_values_supported",
+            "request_object_signing_alg_values_supported",
+            "response_modes_supported",
+            "response_types_supported",
+            "scopes_supported",
+            "subject_types_supported",
+            "token_endpoint_auth_methods_supported",
+            "token_endpoint_auth_signing_alg_values_supported",
+            "userinfo_encryption_alg_values_supported",
+            "userinfo_encryption_enc_values_supported",
+            "userinfo_signing_alg_values_supported",
+        }
 
         # To verify that I have all the necessary claims to do client registration
         reg_claim = []
         for key, spec in OIDC_Claims.registration_request.c_param.items():
             _pref_key = OIDC_Claims.register2preferred.get(key, key)
             if _pref_key in self.supported:
                 reg_claim.append(key)
 
         assert set(RegistrationRequest.c_param.keys()).difference(set(reg_claim)) == {
-            'post_logout_redirect_uri', 'grant_types'}
+            "post_logout_redirect_uri",
+            "grant_types",
+            "response_modes" # Extra item
+        }
 
         # Which ones are list -> singletons
 
         l_to_s = []
         non_oidc = []
         for key, pref_key in OIDC_Claims.register2preferred.items():
             spec = RegistrationRequest.c_param.get(key)
             if spec is None:
                 non_oidc.append(pref_key)
             elif isinstance(spec[0], list):
                 l_to_s.append(key)
 
-        assert set(non_oidc) == {'scopes_supported'}
-        assert set(l_to_s) == {'response_types', 'grant_types', 'default_acr_values'}
+        assert set(non_oidc) == {"scopes_supported"}
+        assert set(l_to_s) == {"response_types", "grant_types", "default_acr_values"}
 
     def test_provider_info(self):
-        OP_BASEURL = 'https://example.com'
+        OP_BASEURL = "https://example.com"
         provider_info_response = {
             "version": "3.0",
             "token_endpoint_auth_methods_supported": [
                 "client_secret_post",
                 "client_secret_basic",
                 "client_secret_jwt",
                 "private_key_jwt",
@@ -214,100 +225,108 @@
             "jwks_uri": f"{OP_BASEURL}/static/jwks_tE2iLbOAqXhe8bqh.json",
             "authorization_endpoint": f"{OP_BASEURL}/authorization",
             "token_endpoint": f"{OP_BASEURL}/token",
             "userinfo_endpoint": f"{OP_BASEURL}/userinfo",
             "registration_endpoint": f"{OP_BASEURL}/registration",
             "end_session_endpoint": f"{OP_BASEURL}/end_session",
             # below are a set which the RP has default values but the OP overwrites
-            "scopes_supported": ['openid', 'fee', 'faa', 'foo', 'fum'],
-            "response_types_supported": ['code', 'id_token', 'code id_token'],
-            "response_modes_supported": ['query', 'form_post', 'new_fangled'],
+            "scopes_supported": ["openid", "fee", "faa", "foo", "fum"],
+            "response_types_supported": ["code", "id_token", "code id_token"],
+            "response_modes_supported": ["query", "form_post", "new_fangled"],
             # this does not have a default value
-            "acr_values_supported": ['mfa'],
+            "acr_values_supported": ["mfa"],
         }
 
         claims = OIDC_Claims()
-        claims.prefer = supported_to_preferred(supported=self.supported,
-                                                    preference=claims.prefer,
-                                                    base_url='https://example.com',
-                                                    info=provider_info_response)
+        claims.prefer = supported_to_preferred(
+            supported=self.supported,
+            preference=claims.prefer,
+            base_url="https://example.com",
+            info=provider_info_response,
+        )
 
         # These are the claims that has default values
-        assert set(claims.prefer.keys()) == {'application_type',
-                                                  'default_max_age',
-                                                  'encrypt_request_object_supported',
-                                                  'encrypt_userinfo_supported',
-                                                  'id_token_encryption_alg_values_supported',
-                                                  'id_token_encryption_enc_values_supported',
-                                                  'id_token_signing_alg_values_supported',
-                                                  'request_object_encryption_alg_values_supported',
-                                                  'request_object_encryption_enc_values_supported',
-                                                  'request_object_signing_alg_values_supported',
-                                                  'response_modes_supported',
-                                                  'response_types_supported',
-                                                  'scopes_supported',
-                                                  'subject_types_supported',
-                                                  'token_endpoint_auth_methods_supported',
-                                                  'token_endpoint_auth_signing_alg_values_supported',
-                                                  'userinfo_encryption_alg_values_supported',
-                                                  'userinfo_encryption_enc_values_supported',
-                                                  'userinfo_signing_alg_values_supported'}
+        assert set(claims.prefer.keys()) == {
+            "application_type",
+            "default_max_age",
+            "encrypt_request_object_supported",
+            "encrypt_userinfo_supported",
+            "id_token_encryption_alg_values_supported",
+            "id_token_encryption_enc_values_supported",
+            "id_token_signing_alg_values_supported",
+            "request_object_encryption_alg_values_supported",
+            "request_object_encryption_enc_values_supported",
+            "request_object_signing_alg_values_supported",
+            "response_modes_supported",
+            "response_types_supported",
+            "scopes_supported",
+            "subject_types_supported",
+            "token_endpoint_auth_methods_supported",
+            "token_endpoint_auth_signing_alg_values_supported",
+            "userinfo_encryption_alg_values_supported",
+            "userinfo_encryption_enc_values_supported",
+            "userinfo_signing_alg_values_supported",
+        }
 
         # least common denominator
         # The RP supports less than the OP
-        assert claims.get_preference('scopes_supported') == ['openid']
-        assert claims.get_preference("response_modes_supported") == ['query', 'form_post']
+        assert claims.get_preference("scopes_supported") == ["openid"]
+        assert claims.get_preference("response_modes_supported") == ["query", "form_post"]
         # The OP supports less than the RP
-        assert claims.get_preference("response_types_supported") == ['code', 'id_token',
-                                                                          'code id_token']
+        assert claims.get_preference("response_types_supported") == [
+            "code",
+            "id_token",
+            "code id_token",
+        ]
 
 
 class TestTransform2:
-
     @pytest.fixture(autouse=True)
     def setup(self):
         self.claims = OIDC_Claims()
         supported = self.claims._supports.copy()
         for service in [
-            'idpyoidc.client.oidc.access_token.AccessToken',
-            'idpyoidc.client.oidc.authorization.Authorization',
-            'idpyoidc.client.oidc.backchannel_authentication.BackChannelAuthentication',
-            'idpyoidc.client.oidc.backchannel_authentication.ClientNotification',
-            'idpyoidc.client.oidc.check_id.CheckID',
-            'idpyoidc.client.oidc.check_session.CheckSession',
-            'idpyoidc.client.oidc.end_session.EndSession',
-            'idpyoidc.client.oidc.provider_info_discovery.ProviderInfoDiscovery',
-            'idpyoidc.client.oidc.read_registration.RegistrationRead',
-            'idpyoidc.client.oidc.refresh_access_token.RefreshAccessToken',
-            'idpyoidc.client.oidc.registration.Registration',
-            'idpyoidc.client.oidc.userinfo.UserInfo',
-            'idpyoidc.client.oidc.webfinger.WebFinger'
+            "idpyoidc.client.oidc.access_token.AccessToken",
+            "idpyoidc.client.oidc.authorization.Authorization",
+            "idpyoidc.client.oidc.backchannel_authentication.BackChannelAuthentication",
+            "idpyoidc.client.oidc.backchannel_authentication.ClientNotification",
+            "idpyoidc.client.oidc.check_id.CheckID",
+            "idpyoidc.client.oidc.check_session.CheckSession",
+            "idpyoidc.client.oidc.end_session.EndSession",
+            "idpyoidc.client.oidc.provider_info_discovery.ProviderInfoDiscovery",
+            "idpyoidc.client.oidc.read_registration.RegistrationRead",
+            "idpyoidc.client.oidc.refresh_access_token.RefreshAccessToken",
+            "idpyoidc.client.oidc.registration.Registration",
+            "idpyoidc.client.oidc.userinfo.UserInfo",
+            "idpyoidc.client.oidc.webfinger.WebFinger",
         ]:
             cls = importer(service)
             supported.update(cls._supports)
 
         for key, val in supported.items():
             if isinstance(val, Callable):
                 supported[key] = val()
 
         self.supported = supported
         preference = {
             "application_type": "web",
-            "redirect_uris": ["https://client.example.org/callback",
-                              "https://client.example.org/callback2"],
+            "redirect_uris": [
+                "https://client.example.org/callback",
+                "https://client.example.org/callback2",
+            ],
             "client_name": "My Example",
             # "client_name#ja-Jpan-JP": "クライアント名",
             "logo_uri": "https://client.example.org/logo.png",
-            'contacts': ["ve7jtb@example.org", "mary@example.org"]
+            "contacts": ["ve7jtb@example.org", "mary@example.org"],
         }
 
         self.claims.load_conf(preference, self.supported)
 
     def test_registration_response(self):
-        OP_BASEURL = 'https://example.com'
+        OP_BASEURL = "https://example.com"
         provider_info_response = {
             "version": "3.0",
             "token_endpoint_auth_methods_supported": [
                 "client_secret_post",
                 "client_secret_basic",
                 "client_secret_jwt",
                 "private_key_jwt",
@@ -316,85 +335,96 @@
             "jwks_uri": f"{OP_BASEURL}/static/jwks_tE2iLbOAqXhe8bqh.json",
             "authorization_endpoint": f"{OP_BASEURL}/authorization",
             "token_endpoint": f"{OP_BASEURL}/token",
             "userinfo_endpoint": f"{OP_BASEURL}/userinfo",
             "registration_endpoint": f"{OP_BASEURL}/registration",
             "end_session_endpoint": f"{OP_BASEURL}/end_session",
             # below are a set which the RP has default values but the OP overwrites
-            "scopes_supported": ['openid', 'fee', 'faa', 'foo', 'fum'],
-            "response_types_supported": ['code', 'id_token', 'code id_token'],
-            "response_modes_supported": ['query', 'form_post', 'new_fangled'],
+            "scopes_supported": ["openid", "fee", "faa", "foo", "fum"],
+            "response_types_supported": ["code", "id_token", "code id_token"],
+            "response_modes_supported": ["query", "form_post", "new_fangled"],
             # this does not have a default value
-            "acr_values_supported": ['mfa'],
+            "acr_values_supported": ["mfa"],
         }
 
-        self.claims.prefer = supported_to_preferred(supported=self.supported,
-                                                         preference=self.claims.prefer,
-                                                         base_url='https://example.com',
-                                                         info=provider_info_response)
-
-        registration_request = create_registration_request(prefers=self.claims.prefer,
-                                                           supported=self.supported)
-
-        assert set(registration_request.keys()) == {'application_type',
-                                                    'client_name',
-                                                    'contacts',
-                                                    'default_max_age',
-                                                    'id_token_signed_response_alg',
-                                                    'logo_uri',
-                                                    'redirect_uris',
-                                                    'request_object_signing_alg',
-                                                    'response_types',
-                                                    'subject_type',
-                                                    'token_endpoint_auth_method',
-                                                    'token_endpoint_auth_signing_alg',
-                                                    'userinfo_signed_response_alg'}
+        self.claims.prefer = supported_to_preferred(
+            supported=self.supported,
+            preference=self.claims.prefer,
+            base_url="https://example.com",
+            info=provider_info_response,
+        )
+
+        registration_request = create_registration_request(
+            prefers=self.claims.prefer, supported=self.supported
+        )
+
+        assert set(registration_request.keys()) == {
+            "application_type",
+            "client_name",
+            "contacts",
+            "default_max_age",
+            "id_token_signed_response_alg",
+            "logo_uri",
+            "redirect_uris",
+            "request_object_signing_alg",
+            "response_types",
+            "response_modes", # non-standard
+            "subject_type",
+            "token_endpoint_auth_method",
+            "token_endpoint_auth_signing_alg",
+            "userinfo_signed_response_alg",
+        }
 
-        assert registration_request["subject_type"] == 'public'
+        assert registration_request["subject_type"] == "public"
 
         registration_response = {
             "application_type": "web",
-            "redirect_uris":
-                ["https://client.example.org/callback",
-                 "https://client.example.org/callback2"],
+            "redirect_uris": [
+                "https://client.example.org/callback",
+                "https://client.example.org/callback2",
+            ],
             "client_name": "My Example",
             "logo_uri": "https://client.example.org/logo.png",
             "subject_type": "pairwise",
-            "sector_identifier_uri":
-                "https://other.example.net/file_of_redirect_uris.json",
+            "sector_identifier_uri": "https://other.example.net/file_of_redirect_uris.json",
             "token_endpoint_auth_method": "client_secret_basic",
             "jwks_uri": "https://client.example.org/my_public_keys.jwks",
             "userinfo_encrypted_response_alg": "RSA1_5",
             "userinfo_encrypted_response_enc": "A128CBC-HS256",
             "contacts": ["ve7jtb@example.org", "mary@example.org"],
             "request_uris": [
-                "https://client.example.org/rf.txt#qpXaRLh_n93TTR9F252ValdatUQvQiJi5BDub2BeznA"]
+                "https://client.example.org/rf.txt#qpXaRLh_n93TTR9F252ValdatUQvQiJi5BDub2BeznA"
+            ],
         }
 
-        to_use = preferred_to_registered(supported=self.supported,
-                                         prefers=self.claims.prefer,
-                                         registration_response=registration_response)
-
-        assert set(to_use.keys()) == {'application_type',
-                                      'client_name',
-                                      'contacts',
-                                      'default_max_age',
-                                      'encrypt_request_object_supported',
-                                      'encrypt_userinfo_supported',
-                                      'id_token_signed_response_alg',
-                                      'jwks_uri',
-                                      'logo_uri',
-                                      'redirect_uris',
-                                      'request_object_signing_alg',
-                                      'request_uris',
-                                      'response_modes_supported',
-                                      'response_types',
-                                      'scope',
-                                      'sector_identifier_uri',
-                                      'subject_type',
-                                      'token_endpoint_auth_method',
-                                      'token_endpoint_auth_signing_alg',
-                                      'userinfo_encrypted_response_alg',
-                                      'userinfo_encrypted_response_enc',
-                                      'userinfo_signed_response_alg'}
+        to_use = preferred_to_registered(
+            supported=self.supported,
+            prefers=self.claims.prefer,
+            registration_response=registration_response,
+        )
+
+        assert set(to_use.keys()) == {
+            "application_type",
+            "client_name",
+            "contacts",
+            "default_max_age",
+            "encrypt_request_object_supported",
+            "encrypt_userinfo_supported",
+            "id_token_signed_response_alg",
+            "jwks_uri",
+            "logo_uri",
+            "redirect_uris",
+            "request_object_signing_alg",
+            "request_uris",
+            "response_types",
+            "response_modes", # non-standard
+            "scope",
+            "sector_identifier_uri",
+            "subject_type",
+            "token_endpoint_auth_method",
+            "token_endpoint_auth_signing_alg",
+            "userinfo_encrypted_response_alg",
+            "userinfo_encrypted_response_enc",
+            "userinfo_signed_response_alg",
+        }
 
-        assert to_use["subject_type"] == 'pairwise'
+        assert to_use["subject_type"] == "pairwise"
```

### Comparing `idpyoidc-2.0.0/tests/test_11_impexp.py` & `idpyoidc-2.1.0/tests/test_11_impexp.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_13_dump_item.py` & `idpyoidc-2.1.0/tests/test_13_dump_item.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_20_config.py` & `idpyoidc-2.1.0/tests/test_20_config.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_21_abfile.py` & `idpyoidc-2.1.0/tests/test_21_abfile.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_22_backchannel.py` & `idpyoidc-2.1.0/tests/test_22_backchannel.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_client_00_current.py` & `idpyoidc-2.1.0/tests/test_client_00_current.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 class TestCurrent:
     @pytest.fixture(autouse=True)
     def test_setup(self):
         self.current = Current()
 
     def test_create_key_no_key(self):
         state_key = self.current.create_key()
-        self.current.set(state_key, {'iss': ISSUER})
-        _iss = self.current.get(state_key)['iss']
+        self.current.set(state_key, {"iss": ISSUER})
+        _iss = self.current.get(state_key)["iss"]
         assert _iss == ISSUER
-        _item = self.current.get_set(state_key, claim=['iss'])
-        assert _item['iss'] == ISSUER
+        _item = self.current.get_set(state_key, claim=["iss"])
+        assert _item["iss"] == ISSUER
 
     def test_store_and_retrieve_state_item(self):
         state_key = self.current.create_key()
         item = Message(foo="bar", issuer=ISSUER)
         self.current.set(state_key, item)
         _state = self.current.get(state_key)
         assert set(_state.keys()) == {"issuer", "foo"}
@@ -47,15 +47,15 @@
         assert _state_key == state_key
         _state_key = self.current.get_base_key("session_id")
         assert _state_key == state_key
         _state_key = self.current.get_base_key("logout_id")
         assert _state_key == state_key
 
     def test_remove(self):
-        state_key = self.current.create_state(iss='foo')
+        state_key = self.current.create_state(iss="foo")
         self.current.bind_key("subject_id", state_key)
         self.current.bind_key("nonce", state_key)
         self.current.bind_key("session_id", state_key)
         self.current.bind_key("logout_id", state_key)
 
         _state_key = self.current.get_base_key("nonce")
         assert _state_key == state_key
```

### Comparing `idpyoidc-2.0.0/tests/test_client_01_service_context.py` & `idpyoidc-2.1.0/tests/test_client_01_service_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,34 +11,32 @@
 
 KEYJAR = build_keyjar(KEYDEFS)
 
 MINI_CONFIG = {
     "base_url": "https://example.com/cli",
     "key_conf": {"key_defs": KEYDEFS},
     "issuer": "https://op.example.com",
-    "preference": {
-        "response_types": ["code"]
-    }
+    "preference": {"response_types": ["code"]},
 }
 
 
 class TestServiceContext:
-
     @pytest.fixture(autouse=True)
     def setup(self):
         self.unit = Unit()
-        self.service_context = ServiceContext(config=MINI_CONFIG, upstream_get=self.unit.unit_get,
-                                              base_url="https://example.com/cli")
+        self.service_context = ServiceContext(
+            config=MINI_CONFIG, upstream_get=self.unit.unit_get, base_url="https://example.com/cli"
+        )
 
     def test_init(self):
         assert self.service_context
 
     def test_filename_from_webname(self):
         _filename = self.service_context.filename_from_webname("https://example.com/cli/jwks.json")
-        assert _filename == 'jwks.json'
+        assert _filename == "jwks.json"
 
     def test_get_sign_alg(self):
         _alg = self.service_context.get_sign_alg("id_token")
         assert _alg is None
 
         self.service_context.claims.set_preference("id_token_signed_response_alg", "RS384")
         _alg = self.service_context.get_sign_alg("id_token")
@@ -53,16 +51,17 @@
         assert _alg == ["RS256", "ES256"]
 
     def test_get_enc_alg_enc(self):
         _alg_enc = self.service_context.get_enc_alg_enc("userinfo")
         assert _alg_enc == {"alg": None, "enc": None}
 
         self.service_context.claims.set_preference("userinfo_encrypted_response_alg", "RSA1_5")
-        self.service_context.claims.set_preference("userinfo_encrypted_response_enc",
-                                                     "A128CBC+HS256")
+        self.service_context.claims.set_preference(
+            "userinfo_encrypted_response_enc", "A128CBC+HS256"
+        )
 
         _alg_enc = self.service_context.get_enc_alg_enc("userinfo")
         assert _alg_enc == {"alg": "RSA1_5", "enc": "A128CBC+HS256"}
 
         self.service_context.claims.prefer = {}
         self.service_context.provider_info["userinfo_encryption_alg_values_supported"] = [
             "RSA1_5",
```

### Comparing `idpyoidc-2.0.0/tests/test_client_02_entity.py` & `idpyoidc-2.1.0/tests/test_client_02_entity.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 }
 
 
 class TestEntity:
     @pytest.fixture(autouse=True)
     def setup(self):
         self.entity = Entity(
-            config=MINI_CONFIG.copy(), services={"xyz": {"class": "idpyoidc.client.service.Service"}}
+            config=MINI_CONFIG.copy(),
+            services={"xyz": {"class": "idpyoidc.client.service.Service"}},
         )
 
     def test_1(self):
         assert self.entity
 
     def test_get_service(self):
         _srv = self.entity.get_service("")
@@ -62,32 +63,34 @@
     config = {
         "application_type": "web",
         "contacts": ["ops@example.org"],
         "redirect_uris": [f"{RP_BASEURL}/authz_cb"],
         "keys": {"key_defs": KEYSPEC, "read_only": True},
     }
 
-    entity = Entity(config=config, client_type='oidc')
+    entity = Entity(config=config, client_type="oidc")
 
     assert entity.get_context().client_authn_methods == {}
 
 
 def test_client_authn_by_names():
     config = {
         "application_type": "web",
         "contacts": ["ops@example.org"],
         "redirect_uris": [f"{RP_BASEURL}/authz_cb"],
         "keys": {"key_defs": KEYSPEC, "read_only": True},
-        "client_authn_methods": ['client_secret_basic', 'client_secret_post']
+        "client_authn_methods": ["client_secret_basic", "client_secret_post"],
     }
 
-    entity = Entity(config=config, client_type='oidc')
+    entity = Entity(config=config, client_type="oidc")
 
-    assert set(entity.get_context().client_authn_methods.keys()) == {'client_secret_basic',
-                                                                     'client_secret_post'}
+    assert set(entity.get_context().client_authn_methods.keys()) == {
+        "client_secret_basic",
+        "client_secret_post",
+    }
 
 
 class FooBar(ClientAuthnMethod):
     def __init__(self, **kwargs):
         self.kwargs = kwargs
 
     def modify_request(self, request, service, **kwargs):
@@ -97,78 +100,82 @@
 def test_client_authn_full():
     config = {
         "application_type": "web",
         "contacts": ["ops@example.org"],
         "redirect_uris": [f"{RP_BASEURL}/authz_cb"],
         "keys": {"key_defs": KEYSPEC, "read_only": True},
         "client_authn_methods": {
-            'client_secret_basic': {},
-            'client_secret_post': None,
-            'home_brew': {
-                'class': FooBar,
-                'kwargs': {'one': 'bar'}
-            }
-        }
+            "client_secret_basic": {},
+            "client_secret_post": None,
+            "home_brew": {"class": FooBar, "kwargs": {"one": "bar"}},
+        },
     }
 
-    entity = Entity(config=config, client_type='oidc')
+    entity = Entity(config=config, client_type="oidc")
 
-    assert set(entity.get_context().client_authn_methods.keys()) == {'client_secret_basic',
-                                                                    'client_secret_post',
-                                                                    'home_brew'}
+    assert set(entity.get_context().client_authn_methods.keys()) == {
+        "client_secret_basic",
+        "client_secret_post",
+        "home_brew",
+    }
 
 
 def test_service_specific():
     config = {
         "application_type": "web",
         "contacts": ["ops@example.org"],
         "redirect_uris": [f"{RP_BASEURL}/authz_cb"],
         "keys": {"key_defs": KEYSPEC, "read_only": True},
-        "client_authn_methods": ['client_secret_basic', 'client_secret_post']
+        "client_authn_methods": ["client_secret_basic", "client_secret_post"],
     }
 
-    entity = Entity(config=config, client_type='oidc',
-                    services={
-                        "xyz": {
-                            "class": "idpyoidc.client.service.Service",
-                            "kwargs": {
-                                "client_authn_methods": ['private_key_jwt']
-                            }
-                        }
-                    })
+    entity = Entity(
+        config=config,
+        client_type="oidc",
+        services={
+            "xyz": {
+                "class": "idpyoidc.client.service.Service",
+                "kwargs": {"client_authn_methods": ["private_key_jwt"]},
+            }
+        },
+    )
 
     # A specific does not change the general
-    assert set(entity.get_context().client_authn_methods.keys()) == {'client_secret_basic',
-                                                                    'client_secret_post'}
+    assert set(entity.get_context().client_authn_methods.keys()) == {
+        "client_secret_basic",
+        "client_secret_post",
+    }
 
-    assert set(entity.get_service('').client_authn_methods.keys()) == {'private_key_jwt'}
+    assert set(entity.get_service("").client_authn_methods.keys()) == {"private_key_jwt"}
 
 
 def test_service_specific2():
     config = {
         "application_type": "web",
         "contacts": ["ops@example.org"],
         "redirect_uris": [f"{RP_BASEURL}/authz_cb"],
         "keys": {"key_defs": KEYSPEC, "read_only": True},
-        "client_authn_methods": ['client_secret_basic', 'client_secret_post']
+        "client_authn_methods": ["client_secret_basic", "client_secret_post"],
     }
 
-    entity = Entity(config=config, client_type='oidc',
-                    services={
-                        "xyz": {
-                            "class": "idpyoidc.client.service.Service",
-                            "kwargs": {
-                                "client_authn_methods": {
-                                    'home_brew': {
-                                        'class': FooBar,
-                                        'kwargs': {'one': 'bar'}
-                                    }
-                                }
-                            }
-                        }
-                    })
+    entity = Entity(
+        config=config,
+        client_type="oidc",
+        services={
+            "xyz": {
+                "class": "idpyoidc.client.service.Service",
+                "kwargs": {
+                    "client_authn_methods": {
+                        "home_brew": {"class": FooBar, "kwargs": {"one": "bar"}}
+                    }
+                },
+            }
+        },
+    )
 
     # A specific does not change the general
-    assert set(entity.get_context().client_authn_methods.keys()) == {'client_secret_basic',
-                                                                    'client_secret_post'}
+    assert set(entity.get_context().client_authn_methods.keys()) == {
+        "client_secret_basic",
+        "client_secret_post",
+    }
 
-    assert set(entity.get_service('').client_authn_methods.keys()) == {'home_brew'}
+    assert set(entity.get_service("").client_authn_methods.keys()) == {"home_brew"}
```

### Comparing `idpyoidc-2.0.0/tests/test_client_02b_entity_metadata.py` & `idpyoidc-2.1.0/tests/test_client_02b_entity_metadata.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,147 +11,137 @@
     "redirect_uris": ["https://example.com/cli/authz_cb"],
     "issuer": ISS,
     "application_name": "rphandler",
     "preference": {
         "application_type": "web",
         "contacts": "support@example.com",
         "response_types_supported": ["code"],
-        'request_parameter': "request_uri",
+        "request_parameter": "request_uri",
         "request_object_signing_alg_values_supported": ["ES256"],
         "scope": ["openid", "profile", "email", "address", "phone"],
         "token_endpoint_auth_methods_supported": ["private_key_jwt"],
         "token_endpoint_auth_signing_alg_values_supported": ["ES256"],
         "userinfo_signing_alg_values_supported": ["ES256"],
         "post_logout_redirect_uris": ["https://rp.example.com/post"],
         "backchannel_logout_uri": "https://rp.example.com/back",
         "backchannel_logout_session_required": True,
-        "client_authn_methods": ['bearer_header']
+        "client_authn_methods": ["bearer_header"],
     },
-
     "services": {
         "discovery": {
             "class": "idpyoidc.client.oidc.provider_info_discovery.ProviderInfoDiscovery",
-            "kwargs": {}
-        },
-        "registration": {
-            "class": "idpyoidc.client.oidc.registration.Registration",
-            "kwargs": {}
+            "kwargs": {},
         },
+        "registration": {"class": "idpyoidc.client.oidc.registration.Registration", "kwargs": {}},
         "authorization": {
             "class": "idpyoidc.client.oidc.authorization.Authorization",
-            "kwargs": {}
-        },
-        "accesstoken": {
-            "class": "idpyoidc.client.oidc.access_token.AccessToken",
-            "kwargs": {}
-        },
-        "userinfo": {
-            "class": "idpyoidc.client.oidc.userinfo.UserInfo",
-            "kwargs": {}
+            "kwargs": {},
         },
-        "end_session": {
-            "class": "idpyoidc.client.oidc.end_session.EndSession",
-            "kwargs": {}
-        }
-    }
+        "accesstoken": {"class": "idpyoidc.client.oidc.access_token.AccessToken", "kwargs": {}},
+        "userinfo": {"class": "idpyoidc.client.oidc.userinfo.UserInfo", "kwargs": {}},
+        "end_session": {"class": "idpyoidc.client.oidc.end_session.EndSession", "kwargs": {}},
+    },
 }
 
 KEY_CONF = {
     "private_path": "private/jwks.json",
-    "key_defs": [{"type": "RSA", "key": "", "use": ["sig"]},
-                 {"type": "EC", "crv": "P-256", "use": ["sig"]}],
-    "read_only": False
+    "key_defs": [
+        {"type": "RSA", "key": "", "use": ["sig"]},
+        {"type": "EC", "crv": "P-256", "use": ["sig"]},
+    ],
+    "read_only": False,
 }
 
 
 def test_create_client():
-    client = Entity(config=CLIENT_CONFIG, client_type='oidc')
+    client = Entity(config=CLIENT_CONFIG, client_type="oidc")
     _context = client.get_context()
     _context.map_supported_to_preferred()
     _pref = _context.prefers()
     _pref_with_values = [k for k, v in _pref.items() if v]
-    assert set(_pref_with_values) == {'application_type',
-                                      'backchannel_logout_session_required',
-                                      'backchannel_logout_uri',
-                                      'callback_uris',
-                                      'client_id',
-                                      'client_secret',
-                                      'contacts',
-                                      'default_max_age',
-                                      'grant_types_supported',
-                                      'id_token_signing_alg_values_supported',
-                                      'post_logout_redirect_uris',
-                                      'redirect_uris',
-                                      'request_object_signing_alg_values_supported',
-                                      'request_parameter',
-                                      'response_modes_supported',
-                                      'response_types_supported',
-                                      'scopes_supported',
-                                      'subject_types_supported',
-                                      'token_endpoint_auth_methods_supported',
-                                      'token_endpoint_auth_signing_alg_values_supported',
-                                      'userinfo_signing_alg_values_supported'}
+    assert set(_pref_with_values) == {
+        "application_type",
+        "backchannel_logout_session_required",
+        "backchannel_logout_uri",
+        "callback_uris",
+        "client_id",
+        "client_secret",
+        "contacts",
+        "default_max_age",
+        "grant_types_supported",
+        "id_token_signing_alg_values_supported",
+        "post_logout_redirect_uris",
+        "redirect_uris",
+        "request_object_signing_alg_values_supported",
+        "request_parameter",
+        "response_modes_supported",
+        "response_types_supported",
+        "scopes_supported",
+        "subject_types_supported",
+        "token_endpoint_auth_methods_supported",
+        "token_endpoint_auth_signing_alg_values_supported",
+        "userinfo_signing_alg_values_supported",
+    }
 
     # What's in service configuration has higher priority then what's just supported.
     _context = client.get_service_context()
-    assert _context.get_preference("contacts") == 'support@example.com'
+    assert _context.get_preference("contacts") == "support@example.com"
     #
-    assert _context.get_preference("userinfo_signing_alg_values_supported") == ['ES256']
+    assert _context.get_preference("userinfo_signing_alg_values_supported") == ["ES256"]
     # How to act
     _context.map_preferred_to_registered()
 
     assert _context.get_usage("request_uris") is None
 
     _conf_args = list(_context.collect_usage().keys())
     assert _conf_args
     assert len(_conf_args) == 23
     rr = set(RegistrationRequest.c_param.keys())
     # The ones that are not defined and will therefore not appear in a registration request
     d = rr.difference(set(_conf_args))
-    assert d == {'client_name',
-                 'client_uri',
-                 'default_acr_values',
-                 'frontchannel_logout_session_required',
-                 'frontchannel_logout_uri',
-                 'id_token_encrypted_response_alg',
-                 'id_token_encrypted_response_enc',
-                 'initiate_login_uri',
-                 'logo_uri',
-                 'jwks',
-                 'jwks_uri',
-                 'policy_uri',
-                 'post_logout_redirect_uri',
-                 'request_object_encryption_alg',
-                 'request_object_encryption_enc',
-                 'request_uris',
-                 'require_auth_time',
-                 'sector_identifier_uri',
-                 'tos_uri',
-                 'userinfo_encrypted_response_alg',
-                 'userinfo_encrypted_response_enc'}
+    assert d == {
+        "client_name",
+        "client_uri",
+        "default_acr_values",
+        "frontchannel_logout_session_required",
+        "frontchannel_logout_uri",
+        "id_token_encrypted_response_alg",
+        "id_token_encrypted_response_enc",
+        "initiate_login_uri",
+        "logo_uri",
+        "jwks",
+        "jwks_uri",
+        "policy_uri",
+        "post_logout_redirect_uri",
+        "request_object_encryption_alg",
+        "request_object_encryption_enc",
+        "request_uris",
+        "require_auth_time",
+        "sector_identifier_uri",
+        "tos_uri",
+        "userinfo_encrypted_response_alg",
+        "userinfo_encrypted_response_enc",
+    }
 
 
 def test_create_client_key_conf():
     client_config = CLIENT_CONFIG.copy()
-    client_config.update({
-        "key_conf": KEY_CONF,
-        "jwks_uri": "https://example.com/keys/jwks.json"
-    })
+    client_config.update({"key_conf": KEY_CONF, "jwks_uri": "https://example.com/keys/jwks.json"})
 
-    client = Entity(config=client_config, client_type='oidc')
+    client = Entity(config=client_config, client_type="oidc")
     assert client.get_service_context().get_preference("jwks_uri")
 
 
 def test_create_client_keyjar():
     _keyjar = init_key_jar(**KEY_CONF)
     client_config = CLIENT_CONFIG.copy()
 
-    client = Entity(config=client_config, keyjar=_keyjar, client_type='oidc')
+    client = Entity(config=client_config, keyjar=_keyjar, client_type="oidc")
     _jwks = client.get_service_context().get_preference("jwks")
     assert _jwks
 
 
 def test_create_client_jwks_uri():
     client_config = CLIENT_CONFIG.copy()
-    client_config['jwks_uri'] = "https://rp.example.com/jwks_uri.json"
+    client_config["jwks_uri"] = "https://rp.example.com/jwks_uri.json"
     client = Entity(config=client_config)
     assert client.get_service_context().get_preference("jwks_uri")
```

### Comparing `idpyoidc-2.0.0/tests/test_client_03_config.py` & `idpyoidc-2.1.0/tests/test_client_03_config.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_client_04_service.py` & `idpyoidc-2.1.0/tests/test_client_04_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from idpyoidc.client.entity import Entity
 from idpyoidc.message.oauth2 import AuthorizationResponse
 from idpyoidc.message.oauth2 import Message
 
 
 class Response(object):
-
     def __init__(self, status_code, text, headers=None):
         self.status_code = status_code
         self.text = text
         self.headers = headers or {"content-type": "text/plain"}
 
 
 KEYDEFS = [
@@ -18,79 +17,90 @@
     {"type": "EC", "crv": "P-256", "use": ["sig"]},
 ]
 
 CLIENT_CONF = {
     "redirect_uris": ["https://example.com/cli/authz_cb"],
     "preference": {"response_types_supported": ["code"]},
     "key_conf": {"key_defs": KEYDEFS},
-    "client_id": 'CLIENT',
-    'base_url': "https://example.com/cli"
+    "client_id": "CLIENT",
+    "base_url": "https://example.com/cli",
 }
 
 
 class TestService:
-
     @pytest.fixture(autouse=True)
     def create_service(self):
         self.entity = Entity(
             config=CLIENT_CONF.copy(),
             services={"authz": {"class": "idpyoidc.client.oidc.authorization.Authorization"}},
-            client_type='oidc',
-            jwks_uri='https://example.com/cli/jwks.json'
+            client_type="oidc",
+            jwks_uri="https://example.com/cli/jwks.json",
         )
 
         self.service = self.entity.get_service("authorization")
         self.service_context = self.entity.get_service_context()
         self.service_context.map_supported_to_preferred()
 
     def upstream_get(self, *args):
         if args[0] == "context":
             return self.service_context
-        elif args[0] == 'attribute' and args[1] == 'keyjar':
-            return self.upstream_get('attribute', 'keyjar')
+        elif args[0] == "attribute" and args[1] == "keyjar":
+            return self.upstream_get("attribute", "keyjar")
 
     def test_1(self):
         assert self.service
 
     def test_use(self):
         use = self.service_context.map_preferred_to_registered()
 
-        assert set(use.keys()) == {'application_type',
-                                   'callback_uris',
-                                   'client_id',
-                                   'default_max_age',
-                                   'encrypt_request_object_supported',
-                                   'id_token_signed_response_alg',
-                                   'jwks',
-                                   'redirect_uris',
-                                   'request_object_signing_alg',
-                                   'response_modes_supported',
-                                   'response_types',
-                                   'scope',
-                                   'subject_type'}
+        assert set(use.keys()) == {
+            "application_type",
+            "callback_uris",
+            "client_id",
+            "default_max_age",
+            "encrypt_request_object_supported",
+            "id_token_signed_response_alg",
+            "jwks",
+            "redirect_uris",
+            "request_object_signing_alg",
+            "response_modes",
+            "response_types",
+            "scope",
+            "subject_type",
+        }
 
     def test_gather_request_args(self):
         self.service.conf["request_args"] = {"response_type": "code"}
         args = self.service.gather_request_args(state="state")
-        assert args == {"response_type": "code", "state": "state", 'client_id': 'CLIENT',
-                        'redirect_uri': 'https://example.com/cli/authz_cb', 'scope': ['openid']}
+        assert args == {
+            "response_type": "code",
+            "state": "state",
+            "client_id": "CLIENT",
+            "redirect_uri": "https://example.com/cli/authz_cb",
+            "scope": ["openid"],
+        }
 
         self.service_context.set_usage("client_id", "client")
         args = self.service.gather_request_args(state="state")
-        assert args == {"client_id": "client", "response_type": "code", "state": "state",
-                        'redirect_uri': 'https://example.com/cli/authz_cb', 'scope': ['openid']}
+        assert args == {
+            "client_id": "client",
+            "response_type": "code",
+            "state": "state",
+            "redirect_uri": "https://example.com/cli/authz_cb",
+            "scope": ["openid"],
+        }
 
         self.service_context.set_usage("scope", ["openid", "foo"])
         args = self.service.gather_request_args(state="state")
         assert args == {
             "client_id": "client",
             "response_type": "code",
             "scope": ["openid", "foo"],
             "state": "state",
-            'redirect_uri': 'https://example.com/cli/authz_cb',
+            "redirect_uri": "https://example.com/cli/authz_cb",
         }
 
         self.service_context.set_usage("redirect_uri", "https://rp.example.com")
         args = self.service.gather_request_args(state="state")
         assert args == {
             "client_id": "client",
             "redirect_uri": "https://rp.example.com",
@@ -111,54 +121,54 @@
 
     def test_parse_response_json(self):
         self.service.response_body_type = "json"
         self.service.response_cls = AuthorizationResponse
         self.service_context.issuer = "https://op.example.com/"
         self.service_context.client_id = "client"
 
-        _sign_key = self.service.upstream_get('attribute', 'keyjar').get_signing_key()
+        _sign_key = self.service.upstream_get("attribute", "keyjar").get_signing_key()
         resp1 = AuthorizationResponse(code="auth_grant", state="state").to_json()
         arg = self.service.parse_response(resp1)
         assert isinstance(arg, AuthorizationResponse)
         assert arg.to_dict() == {"code": "auth_grant", "state": "state"}
 
     def test_parse_response_jwt(self):
         self.service.response_body_type = "jwt"
         self.service.response_cls = AuthorizationResponse
         self.service_context.issuer = "https://op.example.com/"
         self.service_context.client_id = "client"
 
-        _sign_key = self.service.upstream_get('attribute', 'keyjar').get_signing_key()
+        _sign_key = self.service.upstream_get("attribute", "keyjar").get_signing_key()
         resp1 = AuthorizationResponse(code="auth_grant", state="state").to_jwt(
             key=_sign_key, algorithm="RS256"
         )
         arg = self.service.parse_response(resp1)
         assert isinstance(arg, AuthorizationResponse)
         assert arg.to_dict() == {"code": "auth_grant", "state": "state"}
 
     def test_parse_response_err(self):
         self.service.response_body_type = "urlencoded"
         self.service.response_cls = AuthorizationResponse
         self.service_context.issuer = "https://op.example.com/"
         self.service_context.client_id = "client"
 
-        _sign_key = self.service.upstream_get('attribute', 'keyjar').get_signing_key()
+        _sign_key = self.service.upstream_get("attribute", "keyjar").get_signing_key()
         resp1 = AuthorizationResponse(code="auth_grant", state="state").to_jwt(
             key=_sign_key, algorithm="RS256"
         )
         with pytest.raises(ValueError):
             arg = self.service.parse_response(resp1)
 
 
 class TestAuthorization(object):
-
     @pytest.fixture(autouse=True)
     def create_service(self):
         self.entity = Entity(
-            config=CLIENT_CONF.copy(), services={"base": {"class": "idpyoidc.client.service.Service"}}
+            config=CLIENT_CONF.copy(),
+            services={"base": {"class": "idpyoidc.client.service.Service"}},
         )
         self.service = self.entity.get_service("")
 
     def test_construct(self):
         req_args = {"foo": "bar"}
         _req = self.service.construct(request_args=req_args, state="state")
         assert isinstance(_req, Message)
```

### Comparing `idpyoidc-2.0.0/tests/test_client_05_util.py` & `idpyoidc-2.1.0/tests/test_client_05_util.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_client_06_client_authn.py` & `idpyoidc-2.1.0/tests/test_client_12_client_auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,118 +1,99 @@
 import base64
 import os
 
+import pytest
 from cryptojwt.exception import MissingKey
-from cryptojwt.jws.jws import JWS
+from cryptojwt.jwk.rsa import new_rsa_key
 from cryptojwt.jws.jws import factory
+from cryptojwt.jws.jws import JWS
 from cryptojwt.jwt import JWT
 from cryptojwt.key_bundle import KeyBundle
 from cryptojwt.key_jar import KeyJar
-from cryptojwt.key_jar import init_key_jar
-import pytest
 
+from idpyoidc.client.client_auth import assertion_jwt
 from idpyoidc.client.client_auth import AuthnFailure
+from idpyoidc.client.client_auth import bearer_auth
 from idpyoidc.client.client_auth import BearerBody
 from idpyoidc.client.client_auth import BearerHeader
 from idpyoidc.client.client_auth import ClientSecretBasic
 from idpyoidc.client.client_auth import ClientSecretJWT
 from idpyoidc.client.client_auth import ClientSecretPost
 from idpyoidc.client.client_auth import PrivateKeyJWT
-from idpyoidc.client.client_auth import assertion_jwt
-from idpyoidc.client.client_auth import bearer_auth
 from idpyoidc.client.client_auth import valid_service_context
 from idpyoidc.client.entity import Entity
-from idpyoidc.claims import Claims
 from idpyoidc.defaults import JWT_BEARER
 from idpyoidc.message import Message
 from idpyoidc.message.oauth2 import AccessTokenRequest
 from idpyoidc.message.oauth2 import AccessTokenResponse
 from idpyoidc.message.oauth2 import AuthorizationRequest
 from idpyoidc.message.oauth2 import AuthorizationResponse
 from idpyoidc.message.oauth2 import CCAccessTokenRequest
 from idpyoidc.message.oauth2 import ResourceRequest
 
 BASE_PATH = os.path.abspath(os.path.dirname(__file__))
 CLIENT_ID = "A"
 
-KEYSPEC = [
-    {"type": "RSA", "use": ["sig"]},
-    {"type": "EC", "crv": "P-256", "use": ["sig"]},
-]
-
 CLIENT_CONF = {
     "issuer": "https://example.com/as",
-    # "redirect_uris": ["https://example.com/cli/authz_cb"],
+    "redirect_uris": ["https://example.com/cli/authz_cb"],
     "client_secret": "white boarding pass",
     "client_id": CLIENT_ID,
-    "key_conf": {'key_defs': KEYSPEC}
-}
-
-KEY_CONF = {
-    "key_defs": [{"type": "RSA", "key": "", "use": ["sig"]},
-                 {"type": "EC", "crv": "P-256", "use": ["sig"]}],
-    "read_only": False
 }
 
 
 def _eq(l1, l2):
     return set(l1) == set(l2)
 
 
 @pytest.fixture
 def entity():
-    keyjar = init_key_jar(**KEY_CONF)
-    _entity = Entity(
-        config=CLIENT_CONF,
-        services={
-            "base": {"class": "idpyoidc.client.service.Service"},
-            "accesstoken": {
-                "class": "idpyoidc.client.oidc.access_token.AccessToken",
-                "kwargs": {
-                }
-            }
-        },
-        keyjar=keyjar,
-        client_type='oidc'
-    )
+    entity = Entity(config=CLIENT_CONF, client_type="oidc")
     # The following two lines is necessary since they replace provider info collection and
     # client registration.
-    _entity.get_service_context().map_supported_to_preferred()
-    _entity.get_service_context().map_preferred_to_registered()
-    return _entity
+    entity.get_service_context().map_supported_to_preferred()
+    entity.get_service_context().map_preferred_to_registered()
+    return entity
 
 
 def test_quote():
     csb = ClientSecretBasic()
     http_args = csb.construct(
         Message(),
         password="MKEM/A7Pkn7JuU0LAcxyHVKvwdczsugaPU0BieLb4CbQAgQj+ypcanFOCb0/FA5h",
         user="796d8fae-a42f-4e4f-ab25-d6205b6d4fa2",
     )
 
     assert (
-            http_args["headers"]["Authorization"] == "Basic "
-                                                     'Nzk2ZDhmYWUtYTQyZi00ZTRmLWFiMjUtZDYyMDViNmQ0ZmEyOk1LRU0vQTdQa243SnVVMExBY3h5SFZLdndkY3pzdWdhUFUwQmllTGI0Q2JRQWdRait5cGNhbkZPQ2IwL0ZBNWg='
+        http_args["headers"]["Authorization"] == "Basic "
+        "Nzk2ZDhmYWUtYTQyZi00ZTRmLWFiMjUtZDYyMDViNmQ0ZmEyOk1LRU0vQTdQa243SnVVMExBY3h5SFZLdndkY3pzdWdhUFUwQmllTGI0Q2JRQWdRait5cGNhbkZPQ2IwL0ZBNWg="
     )
 
 
 class TestClientSecretBasic(object):
-
     def test_construct(self, entity):
-        _service = entity.get_service("")
-        request = _service.construct(
-            request_args={'redirect_uri': "http://example.com", 'state': "ABCDE"})
+        entity.context.cstate.update("ABCDE", {'code': 'abcdefghijklmnopqrst'})
+
+        _token_service = entity.get_service("accesstoken")
+        request = _token_service.construct(
+            request_args={"redirect_uri": "http://example.com", "state": "ABCDE"}
+        )
 
         csb = ClientSecretBasic()
-        http_args = csb.construct(request, _service)
+        http_args = csb.construct(request, _token_service)
 
-        _authz = http_args["headers"]["Authorization"]
-        assert _authz.startswith("Basic ")
-        _token = _authz.split(" ", 1)[1]
-        assert base64.urlsafe_b64decode(_token) == b'A:white boarding pass'
+        credentials = "{}:{}".format("A", "white boarding pass")
+
+        assert http_args == {
+            "headers": {
+                "Authorization": "Basic {}".format(
+                    base64.urlsafe_b64encode(credentials.encode("utf-8")).decode("utf-8")
+                )
+            }
+        }
 
     def test_does_not_remove_padding(self):
         request = AccessTokenRequest(code="foo", redirect_uri="http://example.com")
 
         csb = ClientSecretBasic()
         http_args = csb.construct(request, user="ab", password="c")
 
@@ -125,100 +106,97 @@
         csb = ClientSecretBasic()
         http_args = csb.construct(request, user="service1", password="secret")
 
         assert http_args["headers"]["Authorization"].startswith("Basic ")
 
 
 class TestBearerHeader(object):
-
     def test_construct(self, entity):
         request = ResourceRequest(access_token="Sesame")
         bh = BearerHeader()
-        http_args = bh.construct(request, service=entity.get_service(""))
+        http_args = bh.construct(request, service=entity.get_service("accesstoken"))
 
         assert http_args == {"headers": {"Authorization": "Bearer Sesame"}}
 
     def test_construct_with_http_args(self, entity):
         request = ResourceRequest(access_token="Sesame")
         bh = BearerHeader()
         # Any HTTP args should just be passed on
         http_args = bh.construct(
-            request, service=entity.get_service(""), http_args={"foo": "bar"}
+            request, service=entity.get_service("accesstoken"), http_args={"foo": "bar"}
         )
 
         assert _eq(http_args.keys(), ["foo", "headers"])
         assert http_args["headers"] == {"Authorization": "Bearer Sesame"}
 
     def test_construct_with_headers_in_http_args(self, entity):
         request = ResourceRequest(access_token="Sesame")
 
         bh = BearerHeader()
         http_args = bh.construct(
             request,
-            service=entity.get_service(""),
+            service=entity.get_service("accesstoken"),
             http_args={"headers": {"x-foo": "bar"}},
         )
 
         assert _eq(http_args.keys(), ["headers"])
         assert _eq(http_args["headers"].keys(), ["Authorization", "x-foo"])
         assert http_args["headers"]["Authorization"] == "Bearer Sesame"
 
     def test_construct_with_resource_request(self, entity):
         bh = BearerHeader()
         request = ResourceRequest(access_token="Sesame")
 
-        http_args = bh.construct(request, service=entity.get_service(""))
+        http_args = bh.construct(request, service=entity.get_service("accesstoken"))
 
         assert "access_token" not in request
         assert http_args == {"headers": {"Authorization": "Bearer Sesame"}}
 
     def test_construct_with_token(self, entity):
-        _service = entity.get_service("")
-        srv_cntx = _service.upstream_get("context")
-        _state = srv_cntx.cstate.create_key()
-        srv_cntx.cstate.set(_state, {'iss': "Issuer"})
+        authz_service = entity.get_service("authorization")
+        srv_cntx = authz_service.upstream_get("context")
+        _state = srv_cntx.cstate.create_state(iss="Issuer")
         req = AuthorizationRequest(
             state=_state, response_type="code", redirect_uri="https://example.com", scope=["openid"]
         )
         srv_cntx.cstate.update(_state, req)
 
         # Add a state and bind a code to it
         resp1 = AuthorizationResponse(code="auth_grant", state=_state)
-        response = _service.parse_response(resp1.to_urlencoded(), "urlencoded")
-        _service.update_service_context(response, key=_state)
+        response = authz_service.parse_response(resp1.to_urlencoded(), "urlencoded")
+        authz_service.update_service_context(response, key=_state)
 
         # based on state find the code and then get an access token
         resp2 = AccessTokenResponse(
             access_token="token1", token_type="Bearer", expires_in=0, state=_state
         )
+        _token_service = entity.get_service("accesstoken")
+        response = _token_service.parse_response(resp2.to_urlencoded(), "urlencoded")
 
-        response = _service.parse_response(resp2.to_urlencoded(), "urlencoded")
-        _service.upstream_get("service_context").cstate.update(_state, response)
+        _token_service.update_service_context(response, key=_state)
 
         # and finally use the access token, bound to a state, to
         # construct the authorization header
-        http_args = BearerHeader().construct(ResourceRequest(), _service, key=_state)
+        http_args = BearerHeader().construct(ResourceRequest(), _token_service, key=_state)
         assert http_args == {"headers": {"Authorization": "Bearer token1"}}
 
 
 class TestBearerBody(object):
-
     def test_construct(self, entity):
-        _token_service = entity.get_service("")
+        _token_service = entity.get_service("accesstoken")
         request = ResourceRequest(access_token="Sesame")
         http_args = BearerBody().construct(request, service=_token_service)
 
         assert request["access_token"] == "Sesame"
         assert http_args is None
 
     def test_construct_with_state(self, entity):
-        _auth_service = entity.get_service("accesstoken")
+        _auth_service = entity.get_service("authorization")
         _cntx = _auth_service.upstream_get("context")
-        _key = _cntx.cstate.create_key()
-        _cntx.cstate.set(_key, {'iss': "Issuer"})
+        _key = _cntx.cstate.create_state(iss="Issuer")
 
         resp = AuthorizationResponse(code="code", state=_key)
         _cntx.cstate.update(_key, resp)
 
         atr = AccessTokenResponse(
             access_token="2YotnFZFEjr1zCsicMWpAA",
             token_type="example",
@@ -230,167 +208,172 @@
 
         request = ResourceRequest()
         http_args = BearerBody().construct(request, service=_auth_service, key=_key)
         assert request["access_token"] == "2YotnFZFEjr1zCsicMWpAA"
         assert http_args is None
 
     def test_construct_with_request(self, entity):
-        authz_service = entity.get_service("")
-        _cntx = authz_service.upstream_get('context')
+        authz_service = entity.get_service("authorization")
+        _cntx = authz_service.upstream_get("context")
 
-        _key = _cntx.cstate.create_key()
-        _cntx.cstate.set(_key, {'iss': "Issuer"})
+        _key = _cntx.cstate.create_state(iss="Issuer")
         resp1 = AuthorizationResponse(code="auth_grant", state=_key)
         response = authz_service.parse_response(resp1.to_urlencoded(), "urlencoded")
         authz_service.update_service_context(response, key=_key)
 
         resp2 = AccessTokenResponse(
             access_token="token1", token_type="Bearer", expires_in=0, state=_key
         )
-        _service2 = entity.get_service("")
-        response = _service2.parse_response(resp2.to_urlencoded(), "urlencoded")
-        _service2.upstream_get("service_context").cstate.update(_key, response)
+        _token_service = entity.get_service("accesstoken")
+        response = _token_service.parse_response(resp2.to_urlencoded(), "urlencoded")
+        _token_service.update_service_context(response, key=_key)
 
         request = ResourceRequest()
         BearerBody().construct(request, service=authz_service, key=_key)
 
         assert "access_token" in request
         assert request["access_token"] == "token1"
 
 
 class TestClientSecretPost(object):
-
     def test_construct(self, entity):
-        _token_service = entity.get_service("")
-        request = _token_service.construct(request_args={'redirect_uri': "http://example.com",
-                                                         'state': "ABCDE"})
+        entity.context.cstate.update("ABCDE", {'code': 'abcdefghijklmnopqrst'})
+
+        _token_service = entity.get_service("accesstoken")
+        request = _token_service.construct(redirect_uri="http://example.com", state="ABCDE")
         csp = ClientSecretPost()
         http_args = csp.construct(request, service=_token_service)
 
         assert request["client_id"] == "A"
         assert request["client_secret"] == "white boarding pass"
         assert http_args is None
 
         request = AccessTokenRequest(code="foo", redirect_uri="http://example.com")
         http_args = csp.construct(request, service=_token_service, client_secret="another")
         assert request["client_id"] == "A"
         assert request["client_secret"] == "another"
         assert http_args is None
 
     def test_modify_1(self, entity):
-        token_service = entity.get_service("")
-        request = token_service.construct(request_args={'redirect_uri': "http://example.com",
-                                                        'state': "ABCDE"})
+        entity.context.cstate.update("ABCDE", {'code': 'abcdefghijklmnopqrst'})
+
+        token_service = entity.get_service("accesstoken")
+        request = token_service.construct(redirect_uri="http://example.com", state="ABCDE")
         csp = ClientSecretPost()
+        # client secret not in request or kwargs
+        del request["client_secret"]
         http_args = csp.construct(request, service=token_service)
         assert "client_secret" in request
 
     def test_modify_2(self, entity):
-        _service = entity.get_service("")
-        request = _service.construct(request_args={'redirect_uri': "http://example.com",
-                                                   'state': "ABCDE"})
+        entity.context.cstate.update("ABCDE", {'code': 'abcdefghijklmnopqrst'})
+
+        token_service = entity.get_service("accesstoken")
+        request = token_service.construct(redirect_uri="http://example.com", state="ABCDE")
         csp = ClientSecretPost()
-        _service.upstream_get("context").set_usage('client_secret', "")
+        # client secret not in request or kwargs
+        del request["client_secret"]
+        token_service.upstream_get("context").set_usage("client_secret", "")
         # this will fail
         with pytest.raises(AuthnFailure):
-            http_args = csp.construct(request, service=_service)
+            csp.construct(request, service=token_service)
 
 
 class TestPrivateKeyJWT(object):
-
     def test_construct(self, entity):
-        token_service = entity.get_service("")
+        token_service = entity.get_service("accesstoken")
         kb_rsa = KeyBundle(
             source="file://{}".format(os.path.join(BASE_PATH, "data/keys/rsa.key")),
             fileformat="der",
         )
 
         for key in kb_rsa:
             key.add_kid()
 
-        _context = token_service.upstream_get('context')
-        _keyjar = token_service.upstream_get('attribute', 'keyjar')
+        _keyjar = token_service.upstream_get("attribute", "keyjar")
         _keyjar.add_kb("", kb_rsa)
+
+        _context = token_service.upstream_get("context")
         _context.provider_info = {
             "issuer": "https://example.com/",
             "token_endpoint": "https://example.com/token",
         }
         _context.registration_response = {"token_endpoint_auth_signing_alg": "RS256"}
         token_service.endpoint = "https://example.com/token"
 
         request = AccessTokenRequest()
         pkj = PrivateKeyJWT()
         http_args = pkj.construct(request, service=token_service, authn_endpoint="token_endpoint")
         assert http_args == {}
         cas = request["client_assertion"]
 
-        # Receiver
         _kj = KeyJar()
-        _kj.import_jwks(_keyjar.export_jwks(), issuer_id=_context.get_client_id())
         _kj.add_kb(_context.get_client_id(), kb_rsa)
         jso = JWT(key_jar=_kj).unpack(cas)
         assert _eq(jso.keys(), ["aud", "iss", "sub", "jti", "exp", "iat"])
         # assert _jwt.headers == {'alg': 'RS256'}
         assert jso["aud"] == [_context.provider_info["token_endpoint"]]
 
     def test_construct_client_assertion(self, entity):
-        token_service = entity.get_service("")
+        token_service = entity.get_service("accesstoken")
 
         kb_rsa = KeyBundle(
             source="file://{}".format(os.path.join(BASE_PATH, "data/keys/rsa.key")),
             fileformat="der",
         )
 
         request = AccessTokenRequest()
         pkj = PrivateKeyJWT()
         _ca = assertion_jwt(
-            token_service.upstream_get('context').get_client_id(),
+            token_service.upstream_get("context").get_client_id(),
             kb_rsa.get("RSA"),
             "https://example.com/token",
             "RS256",
         )
         http_args = pkj.construct(request, client_assertion=_ca)
         assert http_args == {}
         assert request["client_assertion"] == _ca
         assert request["client_assertion_type"] == JWT_BEARER
 
 
 class TestClientSecretJWT_TE(object):
-
     def test_client_secret_jwt(self, entity):
         _service_context = entity.get_context()
         _service_context.token_endpoint = "https://example.com/token"
 
         _service_context.provider_info = {
             "issuer": "https://example.com/",
             "token_endpoint": "https://example.com/token",
         }
 
-        # This is not the default
         _service_context.set_usage("token_endpoint_auth_signing_alg", "HS256")
 
         csj = ClientSecretJWT()
         request = AccessTokenRequest()
 
         csj.construct(
-            request, service=entity.get_service(""), authn_endpoint="token_endpoint"
+            request,
+            service=entity.get_service("accesstoken"),
+            authn_endpoint="token_endpoint",
         )
         assert request["client_assertion_type"] == JWT_BEARER
         assert "client_assertion" in request
         cas = request["client_assertion"]
 
         _kj = KeyJar()
-        _kj.add_symmetric(_service_context.get_client_id(),
-                          _service_context.get_usage('client_secret'), ["sig"])
+        _kj.add_symmetric(
+            _service_context.get_client_id(), _service_context.get_usage("client_secret"), ["sig"]
+        )
         jso = JWT(key_jar=_kj, sign_alg="HS256").unpack(cas)
         assert _eq(jso.keys(), ["aud", "iss", "sub", "exp", "iat", "jti"])
 
         _rj = JWS(alg="HS256")
-        info = _rj.verify_compact(cas, _kj.get_signing_key(
-            issuer_id=_service_context.get_client_id()))
+        info = _rj.verify_compact(
+            cas, _kj.get_signing_key(issuer_id=_service_context.get_client_id())
+        )
 
         assert _eq(info.keys(), ["aud", "iss", "sub", "jti", "exp", "iat"])
         assert info["aud"] == [_service_context.provider_info["token_endpoint"]]
 
     def test_get_key_by_kid(self, entity):
         _service_context = entity.get_context()
         _service_context.token_endpoint = "https://example.com/token"
@@ -401,29 +384,24 @@
         }
 
         _service_context.set_usage("token_endpoint_auth_signing_alg", "HS256")
 
         csj = ClientSecretJWT()
         request = AccessTokenRequest()
 
-        # get a kid for a symmetric key
-        kid = ''
-        for _key in entity.get_attribute('keyjar').get_issuer_keys(""):
-            if _key.kty == 'oct':
-                kid = _key.kid
-                break
-
-        # token_service = entity.get_service("")
+        # get a kid
+        _keys = entity.keyjar.get_issuer_keys("")
+        kid = _keys[0].kid
         token_service = entity.get_service("accesstoken")
         csj.construct(request, service=token_service, authn_endpoint="token_endpoint", kid=kid)
         assert "client_assertion" in request
 
     def test_get_key_by_kid_fail(self, entity):
-        token_service = entity.get_service("")
-        _service_context = token_service.upstream_get('context')
+        token_service = entity.get_service("accesstoken")
+        _service_context = token_service.upstream_get("context")
         _service_context.token_endpoint = "https://example.com/token"
 
         _service_context.provider_info = {
             "issuer": "https://example.com/",
             "token_endpoint": "https://example.com/token",
         }
 
@@ -442,66 +420,65 @@
         _service_context.token_endpoint = "https://example.com/token"
 
         _service_context.provider_info = {
             "issuer": "https://example.com/",
             "token_endpoint": "https://example.com/token",
         }
 
-        # This is the default so this line is unnecessary
-        # _service_context.set_usage("token_endpoint_auth_signing_alg", "RS256")
+        _service_context.set_usage("token_endpoint_auth_signing_alg", "RS256")
 
         csj = ClientSecretJWT()
         request = AccessTokenRequest()
 
-        # No preference -> default == RS256
         _service_context.registration_response = {}
 
-        token_service = entity.get_service("")
+        token_service = entity.get_service("accesstoken")
 
-        # Since I have an RSA key this doesn't fail
+        # Add a RSA key to be able to handle default
+        _kb = KeyBundle()
+        _rsa_key = new_rsa_key()
+        _kb.append(_rsa_key)
+        entity.keyjar.add_kb("", _kb)
+        # Since I have a RSA key this doesn't fail
         csj.construct(request, service=token_service, authn_endpoint="token_endpoint")
 
-        _rsa_key = entity.keyjar.get(key_use='sig', key_type='rsa', issuer_id='')[0]
         _jws = factory(request["client_assertion"])
         assert _jws.jwt.headers["alg"] == "RS256"
-        _rsa_key = entity.keyjar.get_signing_key(key_type="RSA")[0]
         assert _jws.jwt.headers["kid"] == _rsa_key.kid
 
         # By client preferences
         request = AccessTokenRequest()
         _service_context.set_usage("token_endpoint_auth_signing_alg", "RS512")
         csj.construct(request, service=token_service, authn_endpoint="token_endpoint")
 
         _jws = factory(request["client_assertion"])
         assert _jws.jwt.headers["alg"] == "RS512"
         assert _jws.jwt.headers["kid"] == _rsa_key.kid
 
         # Use provider information is everything else fails
         request = AccessTokenRequest()
-        _service_context.claims = Claims()
+        # Can't use set_metadata_value since it won't allow me to overwrite a non-default value
+        _service_context.set_usage("token_endpoint_auth_signing_alg", None)
         _service_context.provider_info["token_endpoint_auth_signing_alg_values_supported"] = [
             "ES256",
             "RS256",
         ]
         csj.construct(request, service=token_service, authn_endpoint="token_endpoint")
 
-        _ec_key = entity.keyjar.get(key_use='sig', key_type='ec', issuer_id='')[0]
         _jws = factory(request["client_assertion"])
-        # Should be ES256 since I have a key for ES256
-        assert _jws.jwt.headers["alg"] == "ES256"
-        _ec_key = entity.keyjar.get_signing_key(key_type="EC")[0]
-        assert _jws.jwt.headers["kid"] == _ec_key.kid
+        # Should be RS256 since I have no key for ES256
+        assert _jws.jwt.headers["alg"] == "RS256"
+        assert _jws.jwt.headers["kid"] == _rsa_key.kid
 
 
 class TestClientSecretJWT_UI(object):
-
     def test_client_secret_jwt(self, entity):
-        access_token_service = entity.get_service("")
+        access_token_service = entity.get_service("accesstoken")
 
-        _service_context = access_token_service.upstream_get('context')
+        _service_context = access_token_service.upstream_get("context")
         _service_context.token_endpoint = "https://example.com/token"
         _service_context.provider_info = {
             "issuer": "https://example.com/",
             "token_endpoint": "https://example.com/token",
         }
 
         csj = ClientSecretJWT()
@@ -511,29 +488,32 @@
             request, service=access_token_service, algorithm="HS256", authn_endpoint="userinfo"
         )
         assert request["client_assertion_type"] == JWT_BEARER
         assert "client_assertion" in request
         cas = request["client_assertion"]
 
         _kj = KeyJar()
-        _kj.add_symmetric(_service_context.get_client_id(),
-                          _service_context.get_usage('client_secret'), usage=["sig"])
+        _kj.add_symmetric(
+            _service_context.get_client_id(),
+            _service_context.get_usage("client_secret"),
+            usage=["sig"],
+        )
         jso = JWT(key_jar=_kj, sign_alg="HS256").unpack(cas)
         assert _eq(jso.keys(), ["aud", "iss", "sub", "jti", "exp", "iat"])
 
         _rj = JWS(alg="HS256")
-        info = _rj.verify_compact(cas, _kj.get_signing_key(
-            issuer_id=_service_context.get_client_id()))
+        info = _rj.verify_compact(
+            cas, _kj.get_signing_key(issuer_id=_service_context.get_client_id())
+        )
 
         assert _eq(info.keys(), ["aud", "iss", "sub", "jti", "exp", "iat"])
         assert info["aud"] == [_service_context.provider_info["issuer"]]
 
 
 class TestValidClientInfo(object):
-
     def test_valid_service_context(self, entity):
         _service_context = entity.get_context()
 
         _now = 123456  # At some time
         # Expiration time missing or 0, client_secret never expires
         # service_context.client_secret_expires_at
         assert valid_service_context(_service_context, _now)
```

### Comparing `idpyoidc-2.0.0/tests/test_client_10_entity.py` & `idpyoidc-2.1.0/tests/test_client_10_entity.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,24 +38,25 @@
         assert len(self.entity.keyjar.get_issuer_keys("")) == 1
 
         with responses.RequestsMock() as rsps:
             _jwks_url = "https://foobar.com/jwks.json"
             rsps.add(
                 "GET",
                 _jwks_url,
-                body=self.entity.get_attribute('keyjar').export_jwks_as_json(),
+                body=self.entity.get_attribute("keyjar").export_jwks_as_json(),
                 status=200,
                 adding_headers={"Content-Type": "application/json"},
             )
             keyspec = {"url": {"https://foobar.com": _jwks_url}}
             self.entity.import_keys(keyspec)
 
             # Now there should be one belonging to https://example.com
-            assert len(self.entity.get_attribute('keyjar').get_issuer_keys(
-                "https://foobar.com")) == 1
+            assert (
+                len(self.entity.get_attribute("keyjar").get_issuer_keys("https://foobar.com")) == 1
+            )
 
     def test_import_keys_file_json(self):
         # Should only be one and that a symmetric key (client_secret) usable
         # for signing and encryption
         assert len(self.entity.keyjar.get_issuer_keys("")) == 1
 
         file_path = os.path.abspath(os.path.join(os.path.dirname(__file__), "salesforce.key"))
```

### Comparing `idpyoidc-2.0.0/tests/test_client_12_client_auth.py` & `idpyoidc-2.1.0/tests/test_client_06_client_authn.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,97 +1,116 @@
 import base64
 import os
 
-import pytest
 from cryptojwt.exception import MissingKey
-from cryptojwt.jwk.rsa import new_rsa_key
-from cryptojwt.jws.jws import factory
 from cryptojwt.jws.jws import JWS
+from cryptojwt.jws.jws import factory
 from cryptojwt.jwt import JWT
 from cryptojwt.key_bundle import KeyBundle
 from cryptojwt.key_jar import KeyJar
+from cryptojwt.key_jar import init_key_jar
+import pytest
 
-from idpyoidc.client.client_auth import assertion_jwt
 from idpyoidc.client.client_auth import AuthnFailure
-from idpyoidc.client.client_auth import bearer_auth
 from idpyoidc.client.client_auth import BearerBody
 from idpyoidc.client.client_auth import BearerHeader
 from idpyoidc.client.client_auth import ClientSecretBasic
 from idpyoidc.client.client_auth import ClientSecretJWT
 from idpyoidc.client.client_auth import ClientSecretPost
 from idpyoidc.client.client_auth import PrivateKeyJWT
+from idpyoidc.client.client_auth import assertion_jwt
+from idpyoidc.client.client_auth import bearer_auth
 from idpyoidc.client.client_auth import valid_service_context
 from idpyoidc.client.entity import Entity
+from idpyoidc.claims import Claims
 from idpyoidc.defaults import JWT_BEARER
 from idpyoidc.message import Message
 from idpyoidc.message.oauth2 import AccessTokenRequest
 from idpyoidc.message.oauth2 import AccessTokenResponse
 from idpyoidc.message.oauth2 import AuthorizationRequest
 from idpyoidc.message.oauth2 import AuthorizationResponse
 from idpyoidc.message.oauth2 import CCAccessTokenRequest
 from idpyoidc.message.oauth2 import ResourceRequest
 
 BASE_PATH = os.path.abspath(os.path.dirname(__file__))
 CLIENT_ID = "A"
 
+KEYSPEC = [
+    {"type": "RSA", "use": ["sig"]},
+    {"type": "EC", "crv": "P-256", "use": ["sig"]},
+]
+
 CLIENT_CONF = {
     "issuer": "https://example.com/as",
-    "redirect_uris": ["https://example.com/cli/authz_cb"],
+    # "redirect_uris": ["https://example.com/cli/authz_cb"],
     "client_secret": "white boarding pass",
     "client_id": CLIENT_ID,
+    "key_conf": {"key_defs": KEYSPEC},
+}
+
+KEY_CONF = {
+    "key_defs": [
+        {"type": "RSA", "key": "", "use": ["sig"]},
+        {"type": "EC", "crv": "P-256", "use": ["sig"]},
+    ],
+    "read_only": False,
 }
 
 
 def _eq(l1, l2):
     return set(l1) == set(l2)
 
 
 @pytest.fixture
 def entity():
-    entity = Entity(config=CLIENT_CONF, client_type='oidc')
+    keyjar = init_key_jar(**KEY_CONF)
+    _entity = Entity(
+        config=CLIENT_CONF,
+        services={
+            "base": {"class": "idpyoidc.client.service.Service"},
+            "accesstoken": {"class": "idpyoidc.client.oidc.access_token.AccessToken", "kwargs": {}},
+        },
+        keyjar=keyjar,
+        client_type="oidc",
+    )
     # The following two lines is necessary since they replace provider info collection and
     # client registration.
-    entity.get_service_context().map_supported_to_preferred()
-    entity.get_service_context().map_preferred_to_registered()
-    return entity
+    _entity.get_service_context().map_supported_to_preferred()
+    _entity.get_service_context().map_preferred_to_registered()
+    return _entity
 
 
 def test_quote():
     csb = ClientSecretBasic()
     http_args = csb.construct(
         Message(),
         password="MKEM/A7Pkn7JuU0LAcxyHVKvwdczsugaPU0BieLb4CbQAgQj+ypcanFOCb0/FA5h",
         user="796d8fae-a42f-4e4f-ab25-d6205b6d4fa2",
     )
 
     assert (
-            http_args["headers"]["Authorization"] == "Basic "
-                                                     'Nzk2ZDhmYWUtYTQyZi00ZTRmLWFiMjUtZDYyMDViNmQ0ZmEyOk1LRU0vQTdQa243SnVVMExBY3h5SFZLdndkY3pzdWdhUFUwQmllTGI0Q2JRQWdRait5cGNhbkZPQ2IwL0ZBNWg='
+        http_args["headers"]["Authorization"] == "Basic "
+        "Nzk2ZDhmYWUtYTQyZi00ZTRmLWFiMjUtZDYyMDViNmQ0ZmEyOk1LRU0vQTdQa243SnVVMExBY3h5SFZLdndkY3pzdWdhUFUwQmllTGI0Q2JRQWdRait5cGNhbkZPQ2IwL0ZBNWg="
     )
 
 
 class TestClientSecretBasic(object):
-
     def test_construct(self, entity):
-        _token_service = entity.get_service("accesstoken")
-        request = _token_service.construct(request_args={'redirect_uri': "http://example.com",
-                                                         'state': "ABCDE"})
+        _service = entity.get_service("")
+        request = _service.construct(
+            request_args={"redirect_uri": "http://example.com", "state": "ABCDE"}
+        )
 
         csb = ClientSecretBasic()
-        http_args = csb.construct(request, _token_service)
-
-        credentials = "{}:{}".format("A", "white boarding pass")
+        http_args = csb.construct(request, _service)
 
-        assert http_args == {
-            "headers": {
-                "Authorization": "Basic {}".format(
-                    base64.urlsafe_b64encode(credentials.encode("utf-8")).decode("utf-8")
-                )
-            }
-        }
+        _authz = http_args["headers"]["Authorization"]
+        assert _authz.startswith("Basic ")
+        _token = _authz.split(" ", 1)[1]
+        assert base64.urlsafe_b64decode(_token) == b"A:white boarding pass"
 
     def test_does_not_remove_padding(self):
         request = AccessTokenRequest(code="foo", redirect_uri="http://example.com")
 
         csb = ClientSecretBasic()
         http_args = csb.construct(request, user="ab", password="c")
 
@@ -104,99 +123,96 @@
         csb = ClientSecretBasic()
         http_args = csb.construct(request, user="service1", password="secret")
 
         assert http_args["headers"]["Authorization"].startswith("Basic ")
 
 
 class TestBearerHeader(object):
-
     def test_construct(self, entity):
         request = ResourceRequest(access_token="Sesame")
         bh = BearerHeader()
-        http_args = bh.construct(request, service=entity.get_service("accesstoken"))
+        http_args = bh.construct(request, service=entity.get_service(""))
 
         assert http_args == {"headers": {"Authorization": "Bearer Sesame"}}
 
     def test_construct_with_http_args(self, entity):
         request = ResourceRequest(access_token="Sesame")
         bh = BearerHeader()
         # Any HTTP args should just be passed on
-        http_args = bh.construct(
-            request, service=entity.get_service("accesstoken"), http_args={"foo": "bar"}
-        )
+        http_args = bh.construct(request, service=entity.get_service(""), http_args={"foo": "bar"})
 
         assert _eq(http_args.keys(), ["foo", "headers"])
         assert http_args["headers"] == {"Authorization": "Bearer Sesame"}
 
     def test_construct_with_headers_in_http_args(self, entity):
         request = ResourceRequest(access_token="Sesame")
 
         bh = BearerHeader()
         http_args = bh.construct(
             request,
-            service=entity.get_service("accesstoken"),
+            service=entity.get_service(""),
             http_args={"headers": {"x-foo": "bar"}},
         )
 
         assert _eq(http_args.keys(), ["headers"])
         assert _eq(http_args["headers"].keys(), ["Authorization", "x-foo"])
         assert http_args["headers"]["Authorization"] == "Bearer Sesame"
 
     def test_construct_with_resource_request(self, entity):
         bh = BearerHeader()
         request = ResourceRequest(access_token="Sesame")
 
-        http_args = bh.construct(request, service=entity.get_service("accesstoken"))
+        http_args = bh.construct(request, service=entity.get_service(""))
 
         assert "access_token" not in request
         assert http_args == {"headers": {"Authorization": "Bearer Sesame"}}
 
     def test_construct_with_token(self, entity):
-        authz_service = entity.get_service("authorization")
-        srv_cntx = authz_service.upstream_get("context")
-        _state = srv_cntx.cstate.create_state(iss="Issuer")
+        _service = entity.get_service("")
+        srv_cntx = _service.upstream_get("context")
+        _state = srv_cntx.cstate.create_key()
+        srv_cntx.cstate.set(_state, {"iss": "Issuer"})
         req = AuthorizationRequest(
             state=_state, response_type="code", redirect_uri="https://example.com", scope=["openid"]
         )
         srv_cntx.cstate.update(_state, req)
 
         # Add a state and bind a code to it
         resp1 = AuthorizationResponse(code="auth_grant", state=_state)
-        response = authz_service.parse_response(resp1.to_urlencoded(), "urlencoded")
-        authz_service.update_service_context(response, key=_state)
+        response = _service.parse_response(resp1.to_urlencoded(), "urlencoded")
+        _service.update_service_context(response, key=_state)
 
         # based on state find the code and then get an access token
         resp2 = AccessTokenResponse(
             access_token="token1", token_type="Bearer", expires_in=0, state=_state
         )
-        _token_service = entity.get_service("accesstoken")
-        response = _token_service.parse_response(resp2.to_urlencoded(), "urlencoded")
 
-        _token_service.update_service_context(response, key=_state)
+        response = _service.parse_response(resp2.to_urlencoded(), "urlencoded")
+        _service.upstream_get("service_context").cstate.update(_state, response)
 
         # and finally use the access token, bound to a state, to
         # construct the authorization header
-        http_args = BearerHeader().construct(ResourceRequest(), _token_service, key=_state)
+        http_args = BearerHeader().construct(ResourceRequest(), _service, key=_state)
         assert http_args == {"headers": {"Authorization": "Bearer token1"}}
 
 
 class TestBearerBody(object):
-
     def test_construct(self, entity):
-        _token_service = entity.get_service("accesstoken")
+        _token_service = entity.get_service("")
         request = ResourceRequest(access_token="Sesame")
         http_args = BearerBody().construct(request, service=_token_service)
 
         assert request["access_token"] == "Sesame"
         assert http_args is None
 
     def test_construct_with_state(self, entity):
-        _auth_service = entity.get_service("authorization")
+        _auth_service = entity.get_service("accesstoken")
         _cntx = _auth_service.upstream_get("context")
-        _key = _cntx.cstate.create_state(iss="Issuer")
+        _key = _cntx.cstate.create_key()
+        _cntx.cstate.set(_key, {"iss": "Issuer"})
 
         resp = AuthorizationResponse(code="code", state=_key)
         _cntx.cstate.update(_key, resp)
 
         atr = AccessTokenResponse(
             access_token="2YotnFZFEjr1zCsicMWpAA",
             token_type="example",
@@ -208,113 +224,115 @@
 
         request = ResourceRequest()
         http_args = BearerBody().construct(request, service=_auth_service, key=_key)
         assert request["access_token"] == "2YotnFZFEjr1zCsicMWpAA"
         assert http_args is None
 
     def test_construct_with_request(self, entity):
-        authz_service = entity.get_service("authorization")
+        authz_service = entity.get_service("")
         _cntx = authz_service.upstream_get("context")
 
-        _key = _cntx.cstate.create_state(iss="Issuer")
+        _key = _cntx.cstate.create_key()
+        _cntx.cstate.set(_key, {"iss": "Issuer"})
         resp1 = AuthorizationResponse(code="auth_grant", state=_key)
         response = authz_service.parse_response(resp1.to_urlencoded(), "urlencoded")
         authz_service.update_service_context(response, key=_key)
 
         resp2 = AccessTokenResponse(
             access_token="token1", token_type="Bearer", expires_in=0, state=_key
         )
-        _token_service = entity.get_service("accesstoken")
-        response = _token_service.parse_response(resp2.to_urlencoded(), "urlencoded")
-        _token_service.update_service_context(response, key=_key)
+        _service2 = entity.get_service("")
+        response = _service2.parse_response(resp2.to_urlencoded(), "urlencoded")
+        _service2.upstream_get("service_context").cstate.update(_key, response)
 
         request = ResourceRequest()
         BearerBody().construct(request, service=authz_service, key=_key)
 
         assert "access_token" in request
         assert request["access_token"] == "token1"
 
 
 class TestClientSecretPost(object):
-
     def test_construct(self, entity):
-        _token_service = entity.get_service("accesstoken")
-        request = _token_service.construct(redirect_uri="http://example.com", state="ABCDE")
+        _token_service = entity.get_service("")
+        request = _token_service.construct(
+            request_args={"redirect_uri": "http://example.com", "state": "ABCDE"}
+        )
         csp = ClientSecretPost()
         http_args = csp.construct(request, service=_token_service)
 
         assert request["client_id"] == "A"
         assert request["client_secret"] == "white boarding pass"
         assert http_args is None
 
         request = AccessTokenRequest(code="foo", redirect_uri="http://example.com")
         http_args = csp.construct(request, service=_token_service, client_secret="another")
         assert request["client_id"] == "A"
         assert request["client_secret"] == "another"
         assert http_args is None
 
     def test_modify_1(self, entity):
-        token_service = entity.get_service("accesstoken")
-        request = token_service.construct(redirect_uri="http://example.com", state="ABCDE")
+        token_service = entity.get_service("")
+        request = token_service.construct(
+            request_args={"redirect_uri": "http://example.com", "state": "ABCDE"}
+        )
         csp = ClientSecretPost()
-        # client secret not in request or kwargs
-        del request["client_secret"]
         http_args = csp.construct(request, service=token_service)
         assert "client_secret" in request
 
     def test_modify_2(self, entity):
-        token_service = entity.get_service("accesstoken")
-        request = token_service.construct(redirect_uri="http://example.com", state="ABCDE")
+        _service = entity.get_service("")
+        request = _service.construct(
+            request_args={"redirect_uri": "http://example.com", "state": "ABCDE"}
+        )
         csp = ClientSecretPost()
-        # client secret not in request or kwargs
-        del request["client_secret"]
-        token_service.upstream_get("context").set_usage('client_secret', "")
+        _service.upstream_get("context").set_usage("client_secret", "")
         # this will fail
         with pytest.raises(AuthnFailure):
-            csp.construct(request, service=token_service)
+            http_args = csp.construct(request, service=_service)
 
 
 class TestPrivateKeyJWT(object):
-
     def test_construct(self, entity):
-        token_service = entity.get_service("accesstoken")
+        token_service = entity.get_service("")
         kb_rsa = KeyBundle(
             source="file://{}".format(os.path.join(BASE_PATH, "data/keys/rsa.key")),
             fileformat="der",
         )
 
         for key in kb_rsa:
             key.add_kid()
 
+        _context = token_service.upstream_get("context")
         _keyjar = token_service.upstream_get("attribute", "keyjar")
         _keyjar.add_kb("", kb_rsa)
-
-        _context = token_service.upstream_get("context")
         _context.provider_info = {
             "issuer": "https://example.com/",
             "token_endpoint": "https://example.com/token",
         }
         _context.registration_response = {"token_endpoint_auth_signing_alg": "RS256"}
         token_service.endpoint = "https://example.com/token"
 
         request = AccessTokenRequest()
         pkj = PrivateKeyJWT()
         http_args = pkj.construct(request, service=token_service, authn_endpoint="token_endpoint")
         assert http_args == {}
         cas = request["client_assertion"]
 
+        # Receiver
         _kj = KeyJar()
+        _kj.import_jwks(_keyjar.export_jwks(), issuer_id=_context.get_client_id())
         _kj.add_kb(_context.get_client_id(), kb_rsa)
         jso = JWT(key_jar=_kj).unpack(cas)
         assert _eq(jso.keys(), ["aud", "iss", "sub", "jti", "exp", "iat"])
         # assert _jwt.headers == {'alg': 'RS256'}
         assert jso["aud"] == [_context.provider_info["token_endpoint"]]
 
     def test_construct_client_assertion(self, entity):
-        token_service = entity.get_service("accesstoken")
+        token_service = entity.get_service("")
 
         kb_rsa = KeyBundle(
             source="file://{}".format(os.path.join(BASE_PATH, "data/keys/rsa.key")),
             fileformat="der",
         )
 
         request = AccessTokenRequest()
@@ -328,47 +346,45 @@
         http_args = pkj.construct(request, client_assertion=_ca)
         assert http_args == {}
         assert request["client_assertion"] == _ca
         assert request["client_assertion_type"] == JWT_BEARER
 
 
 class TestClientSecretJWT_TE(object):
-
     def test_client_secret_jwt(self, entity):
         _service_context = entity.get_context()
         _service_context.token_endpoint = "https://example.com/token"
 
         _service_context.provider_info = {
             "issuer": "https://example.com/",
             "token_endpoint": "https://example.com/token",
         }
 
+        # This is not the default
         _service_context.set_usage("token_endpoint_auth_signing_alg", "HS256")
 
         csj = ClientSecretJWT()
         request = AccessTokenRequest()
 
-        csj.construct(
-            request,
-            service=entity.get_service("accesstoken"),
-            authn_endpoint="token_endpoint",
-        )
+        csj.construct(request, service=entity.get_service(""), authn_endpoint="token_endpoint")
         assert request["client_assertion_type"] == JWT_BEARER
         assert "client_assertion" in request
         cas = request["client_assertion"]
 
         _kj = KeyJar()
-        _kj.add_symmetric(_service_context.get_client_id(),
-                          _service_context.get_usage('client_secret'), ["sig"])
+        _kj.add_symmetric(
+            _service_context.get_client_id(), _service_context.get_usage("client_secret"), ["sig"]
+        )
         jso = JWT(key_jar=_kj, sign_alg="HS256").unpack(cas)
         assert _eq(jso.keys(), ["aud", "iss", "sub", "exp", "iat", "jti"])
 
         _rj = JWS(alg="HS256")
         info = _rj.verify_compact(
-            cas, _kj.get_signing_key(issuer_id=_service_context.get_client_id()))
+            cas, _kj.get_signing_key(issuer_id=_service_context.get_client_id())
+        )
 
         assert _eq(info.keys(), ["aud", "iss", "sub", "jti", "exp", "iat"])
         assert info["aud"] == [_service_context.provider_info["token_endpoint"]]
 
     def test_get_key_by_kid(self, entity):
         _service_context = entity.get_context()
         _service_context.token_endpoint = "https://example.com/token"
@@ -379,23 +395,28 @@
         }
 
         _service_context.set_usage("token_endpoint_auth_signing_alg", "HS256")
 
         csj = ClientSecretJWT()
         request = AccessTokenRequest()
 
-        # get a kid
-        _keys = entity.keyjar.get_issuer_keys("")
-        kid = _keys[0].kid
+        # get a kid for a symmetric key
+        kid = ""
+        for _key in entity.get_attribute("keyjar").get_issuer_keys(""):
+            if _key.kty == "oct":
+                kid = _key.kid
+                break
+
+        # token_service = entity.get_service("")
         token_service = entity.get_service("accesstoken")
         csj.construct(request, service=token_service, authn_endpoint="token_endpoint", kid=kid)
         assert "client_assertion" in request
 
     def test_get_key_by_kid_fail(self, entity):
-        token_service = entity.get_service("accesstoken")
+        token_service = entity.get_service("")
         _service_context = token_service.upstream_get("context")
         _service_context.token_endpoint = "https://example.com/token"
 
         _service_context.provider_info = {
             "issuer": "https://example.com/",
             "token_endpoint": "https://example.com/token",
         }
@@ -415,64 +436,63 @@
         _service_context.token_endpoint = "https://example.com/token"
 
         _service_context.provider_info = {
             "issuer": "https://example.com/",
             "token_endpoint": "https://example.com/token",
         }
 
-        _service_context.set_usage("token_endpoint_auth_signing_alg", "RS256")
+        # This is the default so this line is unnecessary
+        # _service_context.set_usage("token_endpoint_auth_signing_alg", "RS256")
 
         csj = ClientSecretJWT()
         request = AccessTokenRequest()
 
+        # No preference -> default == RS256
         _service_context.registration_response = {}
 
-        token_service = entity.get_service("accesstoken")
+        token_service = entity.get_service("")
 
-        # Add a RSA key to be able to handle default
-        _kb = KeyBundle()
-        _rsa_key = new_rsa_key()
-        _kb.append(_rsa_key)
-        entity.keyjar.add_kb("", _kb)
-        # Since I have a RSA key this doesn't fail
+        # Since I have an RSA key this doesn't fail
         csj.construct(request, service=token_service, authn_endpoint="token_endpoint")
 
+        _rsa_key = entity.keyjar.get(key_use="sig", key_type="rsa", issuer_id="")[0]
         _jws = factory(request["client_assertion"])
         assert _jws.jwt.headers["alg"] == "RS256"
+        _rsa_key = entity.keyjar.get_signing_key(key_type="RSA")[0]
         assert _jws.jwt.headers["kid"] == _rsa_key.kid
 
         # By client preferences
         request = AccessTokenRequest()
         _service_context.set_usage("token_endpoint_auth_signing_alg", "RS512")
         csj.construct(request, service=token_service, authn_endpoint="token_endpoint")
 
         _jws = factory(request["client_assertion"])
         assert _jws.jwt.headers["alg"] == "RS512"
         assert _jws.jwt.headers["kid"] == _rsa_key.kid
 
         # Use provider information is everything else fails
         request = AccessTokenRequest()
-        # Can't use set_metadata_value since it won't allow me to overwrite a non-default value
-        _service_context.set_usage("token_endpoint_auth_signing_alg", None)
+        _service_context.claims = Claims()
         _service_context.provider_info["token_endpoint_auth_signing_alg_values_supported"] = [
             "ES256",
             "RS256",
         ]
         csj.construct(request, service=token_service, authn_endpoint="token_endpoint")
 
+        _ec_key = entity.keyjar.get(key_use="sig", key_type="ec", issuer_id="")[0]
         _jws = factory(request["client_assertion"])
-        # Should be RS256 since I have no key for ES256
-        assert _jws.jwt.headers["alg"] == "RS256"
-        assert _jws.jwt.headers["kid"] == _rsa_key.kid
+        # Should be ES256 since I have a key for ES256
+        assert _jws.jwt.headers["alg"] == "ES256"
+        _ec_key = entity.keyjar.get_signing_key(key_type="EC")[0]
+        assert _jws.jwt.headers["kid"] == _ec_key.kid
 
 
 class TestClientSecretJWT_UI(object):
-
     def test_client_secret_jwt(self, entity):
-        access_token_service = entity.get_service("accesstoken")
+        access_token_service = entity.get_service("")
 
         _service_context = access_token_service.upstream_get("context")
         _service_context.token_endpoint = "https://example.com/token"
         _service_context.provider_info = {
             "issuer": "https://example.com/",
             "token_endpoint": "https://example.com/token",
         }
@@ -484,29 +504,32 @@
             request, service=access_token_service, algorithm="HS256", authn_endpoint="userinfo"
         )
         assert request["client_assertion_type"] == JWT_BEARER
         assert "client_assertion" in request
         cas = request["client_assertion"]
 
         _kj = KeyJar()
-        _kj.add_symmetric(_service_context.get_client_id(),
-                          _service_context.get_usage('client_secret'), usage=["sig"])
+        _kj.add_symmetric(
+            _service_context.get_client_id(),
+            _service_context.get_usage("client_secret"),
+            usage=["sig"],
+        )
         jso = JWT(key_jar=_kj, sign_alg="HS256").unpack(cas)
         assert _eq(jso.keys(), ["aud", "iss", "sub", "jti", "exp", "iat"])
 
         _rj = JWS(alg="HS256")
         info = _rj.verify_compact(
-            cas, _kj.get_signing_key(issuer_id=_service_context.get_client_id()))
+            cas, _kj.get_signing_key(issuer_id=_service_context.get_client_id())
+        )
 
         assert _eq(info.keys(), ["aud", "iss", "sub", "jti", "exp", "iat"])
         assert info["aud"] == [_service_context.provider_info["issuer"]]
 
 
 class TestValidClientInfo(object):
-
     def test_valid_service_context(self, entity):
         _service_context = entity.get_context()
 
         _now = 123456  # At some time
         # Expiration time missing or 0, client_secret never expires
         # service_context.client_secret_expires_at
         assert valid_service_context(_service_context, _now)
```

### Comparing `idpyoidc-2.0.0/tests/test_client_14_service_context_impexp.py` & `idpyoidc-2.1.0/tests/test_client_14_service_context_impexp.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     config = {
         "client_id": "client_id",
         "issuer": "issuer",
         "client_secret": "client_secret_wordplay",
         "base_url": BASE_URL,
         "requests_dir": "requests",
     }
-    ci = ServiceContext(config=config, client_type='oidc', base_url=BASE_URL)
+    ci = ServiceContext(config=config, client_type="oidc", base_url=BASE_URL)
     ci.claims.load_conf(config, supports=ci.supports())
     ci.map_supported_to_preferred()
     ci.map_preferred_to_registered()
 
     srvcnx = ServiceContext().load(ci.dump())
 
     for attr in config.keys():
@@ -36,19 +36,19 @@
                 val = srvcnx.get_usage(attr)
 
             assert val == config[attr]
 
 
 def test_set_and_get_client_secret():
     service_context = ServiceContext(base_url=BASE_URL)
-    service_context.set_usage('client_secret', "longenoughsupersecret")
+    service_context.set_usage("client_secret", "longenoughsupersecret")
 
     srvcnx2 = ServiceContext(base_url=BASE_URL).load(service_context.dump())
 
-    assert srvcnx2.get_usage('client_secret') == "longenoughsupersecret"
+    assert srvcnx2.get_usage("client_secret") == "longenoughsupersecret"
 
 
 def test_set_and_get_client_id():
     service_context = ServiceContext(base_url=BASE_URL)
     service_context.set_usage("client_id", "myself")
     srvcnx2 = ServiceContext(base_url=BASE_URL).load(service_context.dump())
     assert srvcnx2.get_client_id() == "myself"
@@ -93,15 +93,14 @@
     if alg in supported:
         return True
     else:
         return False
 
 
 class TestClientInfo(object):
-
     @pytest.fixture(autouse=True)
     def create_client_info_instance(self):
         config = {
             "client_id": "client_id",
             "issuer": "issuer",
             "client_secret": "longenoughsupersecret",
             "base_url": "https://example.com",
@@ -272,25 +271,26 @@
         assert len(_keyjar.get_issuer_keys("")) == 1
 
         file_path = os.path.abspath(os.path.join(os.path.dirname(__file__), "salesforce.key"))
 
         keyspec = {"file": {"rsa": [file_path]}}
         self.service_context.import_keys(keyspec)
 
-        _sc_state = self.service_context.dump(exclude_attributes=["context", 'upstream_get'])
+        _sc_state = self.service_context.dump(exclude_attributes=["context", "upstream_get"])
         _jsc_state = json.dumps(_sc_state)
         _o_state = json.loads(_jsc_state)
-        srvcntx = ServiceContext(base_url=BASE_URL).load(_o_state, init_args={
-            'upstream_get': self.service_context.upstream_get})
+        srvcntx = ServiceContext(base_url=BASE_URL).load(
+            _o_state, init_args={"upstream_get": self.service_context.upstream_get}
+        )
 
         # Now there should be 2, the second a RSA key for signing
-        assert len(srvcntx.upstream_get('attribute', 'keyjar').get_issuer_keys("")) == 2
+        assert len(srvcntx.upstream_get("attribute", "keyjar").get_issuer_keys("")) == 2
 
     def test_import_keys_url(self):
-        _keyjar = self.service_context.upstream_get('attribute', 'keyjar')
+        _keyjar = self.service_context.upstream_get("attribute", "keyjar")
         assert len(_keyjar.get_issuer_keys("")) == 1
 
         # One EC key for signing
         key_def = [{"type": "EC", "crv": "P-256", "use": ["sig"]}]
 
         keyjar = build_keyjar(key_def)
 
@@ -305,13 +305,19 @@
             )
             keyspec = {"url": {"https://foobar.com": _jwks_url}}
             self.service_context.import_keys(keyspec)
             _keyjar.update()
 
             srvcntx = ServiceContext(base_url=BASE_URL).load(
                 self.service_context.dump(exclude_attributes=["context"]),
-                init_args={'upstream_get': self.service_context.upstream_get}
+                init_args={"upstream_get": self.service_context.upstream_get},
             )
 
             # Now there should be one belonging to https://example.com
-            assert len(srvcntx.upstream_get('attribute', 'keyjar').get_issuer_keys(
-                "https://foobar.com")) == 1
+            assert (
+                len(
+                    srvcntx.upstream_get("attribute", "keyjar").get_issuer_keys(
+                        "https://foobar.com"
+                    )
+                )
+                == 1
+            )
```

### Comparing `idpyoidc-2.0.0/tests/test_client_15_cookie.py` & `idpyoidc-2.1.0/tests/test_client_15_cookie.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_client_16_util.py` & `idpyoidc-2.1.0/tests/test_client_16_util.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_client_17_http.py` & `idpyoidc-2.1.0/tests/test_client_17_http.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_client_18_service.py` & `idpyoidc-2.1.0/tests/test_client_18_service.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_client_19_webfinger.py` & `idpyoidc-2.1.0/tests/test_client_19_webfinger.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_client_20_oauth2.py` & `idpyoidc-2.1.0/tests/test_client_20_oauth2.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     def test_construct_authorization_request(self):
         req_args = {
             "state": "ABCDE",
             "redirect_uri": "https://example.com/auth_cb",
             "response_type": ["code"],
         }
 
-        self.client.get_context().cstate.set("ABCDE", {"iss": 'issuer'})
+        self.client.get_context().cstate.set("ABCDE", {"iss": "issuer"})
         msg = self.client.get_service("authorization").construct(request_args=req_args)
         assert isinstance(msg, AuthorizationRequest)
         assert msg["client_id"] == "client_1"
         assert msg["redirect_uri"] == "https://example.com/auth_cb"
 
     def test_construct_accesstoken_request(self):
         # Bind access code to state
@@ -83,32 +83,30 @@
 
         _context.cstate.update("ABCDE", auth_request)
 
         auth_response = AuthorizationResponse(code="access_code")
 
         self.client.get_context().cstate.update("ABCDE", auth_response)
 
-        msg = self.client.get_service("accesstoken").construct(
-            request_args=req_args, state="ABCDE"
-        )
+        msg = self.client.get_service("accesstoken").construct(request_args=req_args, state="ABCDE")
 
         assert isinstance(msg, AccessTokenRequest)
         assert msg.to_dict() == {
             "client_id": "client_1",
             "client_secret": "abcdefghijklmnop",
             "grant_type": "authorization_code",
             "state": "ABCDE",
             "code": "access_code",
             "redirect_uri": "https://example.com/cli/authz_cb",
         }
 
     def test_construct_refresh_token_request(self):
         _context = self.client.get_context()
         _state = "ABCDE"
-        _context.cstate.set(_state, {'iss': "issuer"})
+        _context.cstate.set(_state, {"iss": "issuer"})
 
         auth_request = AuthorizationRequest(
             redirect_uri="https://example.com/cli/authz_cb", state="state"
         )
 
         _context.cstate.update(_state, auth_request)
 
@@ -142,28 +140,24 @@
         assert resp["error"] == "Illegal"
         assert resp["status_code"] == 400
 
     def test_error_response_500(self):
         err = ResponseMessage(error="Illegal")
         http_resp = MockResponse(500, err.to_urlencoded())
         with pytest.raises(ParseError):
-            self.client.parse_request_response(
-                self.client.get_service("authorization"), http_resp
-            )
+            self.client.parse_request_response(self.client.get_service("authorization"), http_resp)
 
     def test_error_response_2(self):
         err = ResponseMessage(error="Illegal")
         http_resp = MockResponse(
             400, err.to_json(), headers={"content-type": "application/x-www-form-urlencoded"}
         )
 
         with pytest.raises(OidcServiceError):
-            self.client.parse_request_response(
-                self.client.get_service("authorization"), http_resp
-            )
+            self.client.parse_request_response(self.client.get_service("authorization"), http_resp)
 
 
 BASE_URL = "https://example.com"
 
 
 class TestClient2(object):
     @pytest.fixture(autouse=True)
@@ -192,11 +186,11 @@
         }
         rp_conf = RPHConfiguration(conf)
         rp_handler = RPHandler(base_url=BASE_URL, config=rp_conf)
         self.client = rp_handler.init_client(issuer="service_1")
         assert self.client
 
     def test_keyjar(self):
-        _keyjar = self.client.get_attribute('keyjar')
+        _keyjar = self.client.get_attribute("keyjar")
         assert len(_keyjar) == 2  # one issuer
         assert len(_keyjar[""]) == 3
         assert len(_keyjar.get("sig")) == 3
```

### Comparing `idpyoidc-2.0.0/tests/test_client_21_oidc_service.py` & `idpyoidc-2.1.0/tests/test_client_21_oidc_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from idpyoidc.message.oidc import verified_claim_name
 from idpyoidc.message.oidc.session import CheckIDRequest
 from idpyoidc.message.oidc.session import CheckSessionRequest
 from idpyoidc.message.oidc.session import EndSessionRequest
 
 
 class Response(object):
-
     def __init__(self, status_code, text, headers=None):
         self.status_code = status_code
         self.text = text
         self.headers = headers or {"content-type": "text/plain"}
 
 
 KEYSPEC = [
@@ -66,31 +65,34 @@
     )
     _keyjar.import_jwks(_keyjar.export_jwks(private=True, issuer_id="client_id"), issuer_id="")
     _keyjar.import_jwks_as_json(open("{}/pub_iss.jwks".format(_dirname)).read(), ISS)
     return _keyjar
 
 
 class TestAuthorization(object):
-
     @pytest.fixture(autouse=True)
     def create_request(self):
         client_config = {
             "client_id": "client_id",
             "client_secret": "a longesh password",
             "callback_uris": {
                 "redirect_uris": {  # different flows
-                    "code": ["https://example.com/cli/authz_cb"],
-                    "implicit": ["https://example.com/cli/imp_cb"],
-                    "form_post": ["https://example.com/cli/form"]
+                    "query": ["https://example.com/cli/authz_cb"],
+                    "fragment": ["https://example.com/cli/imp_cb"],
+                    "form_post": ["https://example.com/cli/form"],
                 }
             },
-            "response_types_supported": ['code', 'token']
+            "response_types_supported": ["code", "token"],
         }
-        entity = Entity(services=DEFAULT_OIDC_SERVICES, keyjar=make_keyjar(), config=client_config,
-                        client_type='oidc')
+        entity = Entity(
+            services=DEFAULT_OIDC_SERVICES,
+            keyjar=make_keyjar(),
+            config=client_config,
+            client_type="oidc",
+        )
         _context = entity.get_context()
         _context.issuer = "https://example.com"
         _context.map_supported_to_preferred()
         _context.map_preferred_to_registered()
         self.context = _context
         self.service = entity.get_service("authorization")
 
@@ -180,15 +182,15 @@
             "redirect_uri",
             "nonce",
         }
 
     def test_request_init_request_method(self):
         req_args = {"response_type": "code", "state": "state"}
         self.service.endpoint = "https://example.com/authorize"
-        self.context.set_usage('request_object_encryption_alg', None)
+        self.context.set_usage("request_object_encryption_alg", None)
         _info = self.service.get_request_parameters(request_args=req_args, request_method="value")
         assert set(_info.keys()) == {"url", "method", "request"}
         msg = AuthorizationRequest().from_urlencoded(self.service.get_urlinfo(_info["url"]))
         assert set(msg.to_dict()) == {
             "client_id",
             "redirect_uri",
             "request",
@@ -293,42 +295,45 @@
         req_args = {"response_type": "code", "state": "state", "nonce": "nonce"}
         self.service.endpoint = "https://example.com/authorize"
         self.service.get_request_parameters(request_args=req_args)
         # Build an ID Token
         idt = JWT(ISS_KEY, iss=ISS, lifetime=3600, sign_alg="none")
         payload = {"sub": "123456789", "aud": ["client_id"], "nonce": req_args["nonce"]}
         _idt = idt.pack(payload)
-        self.service.upstream_get("context").claims.set_usage("verify_args", {
-            "allow_sign_alg_none": allow_sign_alg_none
-        })
+        self.service.upstream_get("context").claims.set_usage(
+            "verify_args", {"allow_sign_alg_none": allow_sign_alg_none}
+        )
         resp = AuthorizationResponse(state="state", code="code", id_token=_idt)
         if allow_sign_alg_none:
             self.service.parse_response(resp.to_urlencoded())
         else:
             with pytest.raises(UnsupportedAlgorithm):
                 self.service.parse_response(resp.to_urlencoded())
 
 
 class TestAuthorizationCallback(object):
-
     @pytest.fixture(autouse=True)
     def create_request(self):
         client_config = {
             "client_id": "client_id",
             "client_secret": "a longesh password",
             "callback_uris": {
                 "redirect_uris": {
-                    "code": ["https://example.com/cli/authz_cb"],
-                    "implicit": ["https://example.com/cli/authz_im_cb"],
-                    "form_post": ["https://example.com/cli/authz_fp_cb"]
+                    "query": ["https://example.com/cli/authz_cb"],
+                    "fragment": ["https://example.com/cli/authz_im_cb"],
+                    "form_post": ["https://example.com/cli/authz_fp_cb"],
                 },
             },
         }
-        entity = Entity(keyjar=make_keyjar(), config=client_config, services=DEFAULT_OIDC_SERVICES,
-                        client_type='oidc')
+        entity = Entity(
+            keyjar=make_keyjar(),
+            config=client_config,
+            services=DEFAULT_OIDC_SERVICES,
+            client_type="oidc",
+        )
         _context = entity.get_context()
         _context.issuer = "https://example.com"
         _context.map_supported_to_preferred()
         _context.map_preferred_to_registered()
 
         self.service = entity.get_service("authorization")
 
@@ -387,27 +392,26 @@
             "nonce",
             "response_mode",
         }
         assert _req["redirect_uri"] == "https://example.com/cli/authz_fp_cb"
 
 
 class TestAccessTokenRequest(object):
-
     @pytest.fixture(autouse=True)
     def create_request(self):
         client_config = {
             "client_id": "client_id",
             "client_secret": "a longesh password",
             "redirect_uris": ["https://example.com/cli/authz_cb"],
-            'client_authn_methods': ['client_secret_basic']
+            "client_authn_methods": ["client_secret_basic"],
         }
         entity = Entity(keyjar=make_keyjar(), config=client_config, services=DEFAULT_OIDC_SERVICES)
         _context = entity.get_context()
         _context.issuer = "https://example.com"
-        _context.provider_info = {'token_endpoint': f'{_context.issuer}/token'}
+        _context.provider_info = {"token_endpoint": f"{_context.issuer}/token"}
         self.service = entity.get_service("accesstoken")
 
         # add some history
         auth_request = AuthorizationRequest(
             redirect_uri="https://example.com/cli/authz_cb", state="state", response_type="code"
         )
 
@@ -453,28 +457,27 @@
         req_args = {"redirect_uri": "https://example.com/cli/authz_cb", "code": "access_code"}
         self.service.endpoint = "https://example.com/authorize"
 
         _info = self.service.get_request_parameters(request_args=req_args, state="state")
         assert set(_info.keys()) == {"body", "url", "headers", "method", "request"}
         assert _info["url"] == "https://example.com/authorize"
         msg = AccessTokenRequest().from_urlencoded(self.service.get_urlinfo(_info["body"]))
-        assert set(msg.keys()) == {'redirect_uri', 'grant_type', 'state', 'code', 'client_id'}
+        assert set(msg.keys()) == {"redirect_uri", "grant_type", "state", "code", "client_id"}
 
     def test_id_token_nonce_match(self):
         _cstate = self.service.upstream_get("context").cstate
         _cstate.bind_key("nonce", "state")
         resp = AccessTokenResponse()
         resp[verified_claim_name("id_token")] = {"nonce": "nonce"}
         _cstate.bind_key("nonce2", "state2")
         with pytest.raises(ParameterError):
             self.service.update_service_context(resp, key="state2")
 
 
 class TestProviderInfo(object):
-
     @pytest.fixture(autouse=True)
     def create_service(self):
         self._iss = ISS
         client_config = {
             "client_id": "client_id",
             "client_secret": "a longesh password",
             "redirect_uris": ["https://example.com/cli/authz_cb"],
@@ -488,44 +491,41 @@
                 "request_object_signing_alg_values_supported": ["ES256"],
                 "encrypt_id_token_supported": False,  # default
                 "token_endpoint_auth_methods_supported": ["private_key_jwt"],
                 "token_endpoint_auth_signing_alg_values_supported": ["ES256"],
                 "userinfo_signing_alg_values_supported": ["ES256"],
                 "post_logout_redirect_uris": ["https://rp.example.com/post"],
                 "backchannel_logout_uri": "https://rp.example.com/back",
-                "backchannel_logout_session_required": True
+                "backchannel_logout_session_required": True,
             },
             "services": {
                 "web_finger": {"class": "idpyoidc.client.oidc.webfinger.WebFinger"},
                 "discovery": {
                     "class": "idpyoidc.client.oidc.provider_info_discovery.ProviderInfoDiscovery"
                 },
                 "registration": {
                     "class": "idpyoidc.client.oidc.registration.Registration",
-                    "kwargs": {}
+                    "kwargs": {},
                 },
                 "authorization": {
                     "class": "idpyoidc.client.oidc.authorization.Authorization",
-                    "kwargs": {}
+                    "kwargs": {},
                 },
                 "accesstoken": {
                     "class": "idpyoidc.client.oidc.access_token.AccessToken",
-                    "kwargs": {}
-                },
-                "userinfo": {
-                    "class": "idpyoidc.client.oidc.userinfo.UserInfo",
-                    "kwargs": {}
+                    "kwargs": {},
                 },
+                "userinfo": {"class": "idpyoidc.client.oidc.userinfo.UserInfo", "kwargs": {}},
                 "end_session": {
                     "class": "idpyoidc.client.oidc.end_session.EndSession",
-                    "kwargs": {}
-                }
-            }
+                    "kwargs": {},
+                },
+            },
         }
-        entity = Entity(keyjar=make_keyjar(), config=client_config, client_type='oidc')
+        entity = Entity(keyjar=make_keyjar(), config=client_config, client_type="oidc")
         entity.get_context().issuer = "https://example.com"
         self.service = entity.get_service("provider_info")
 
     def test_construct(self):
         _req = self.service.construct()
         assert isinstance(_req, Message)
         assert len(_req) == 0
@@ -728,47 +728,49 @@
         assert _context.claims.use == {}
         resp = self.service.post_parse_response(provider_info_response)
 
         iss_jwks = ISS_KEY.export_jwks_as_json(issuer_id=ISS)
         with responses.RequestsMock() as rsps:
             rsps.add("GET", resp["jwks_uri"], body=iss_jwks, status=200)
 
-            self.service.update_service_context(resp, '')
+            self.service.update_service_context(resp, "")
 
         # static client registration
         _context.map_preferred_to_registered()
 
         use_copy = self.service.upstream_get("context").claims.use.copy()
         # jwks content will change dynamically between runs
-        assert 'jwks' in use_copy
-        del use_copy['jwks']
-        del use_copy['callback_uris']
-
-        assert use_copy == {'application_type': 'web',
-                            'backchannel_logout_session_required': True,
-                            'backchannel_logout_uri': 'https://rp.example.com/back',
-                            'client_id': 'client_id',
-                            'client_secret': 'a longesh password',
-                            'contacts': ['ops@example.org'],
-                            'default_max_age': 86400,
-                            'encrypt_id_token_supported': False,
-                            'encrypt_request_object_supported': False,
-                            'encrypt_userinfo_supported': False,
-                            'grant_types': ['authorization_code'],
-                            'id_token_signed_response_alg': 'RS256',
-                            'post_logout_redirect_uris': ['https://rp.example.com/post'],
-                            'redirect_uris': ['https://example.com/cli/authz_cb'],
-                            'request_object_signing_alg': 'ES256',
-                            'response_modes_supported': ['query', 'fragment', 'form_post'],
-                            'response_types': ['code'],
-                            'scope': ['openid'],
-                            'subject_type': 'public',
-                            'token_endpoint_auth_method': 'private_key_jwt',
-                            'token_endpoint_auth_signing_alg': 'ES256',
-                            'userinfo_signed_response_alg': 'ES256'}
+        assert "jwks" in use_copy
+        del use_copy["jwks"]
+        del use_copy["callback_uris"]
+
+        assert use_copy == {
+            "application_type": "web",
+            "backchannel_logout_session_required": True,
+            "backchannel_logout_uri": "https://rp.example.com/back",
+            "client_id": "client_id",
+            "client_secret": "a longesh password",
+            "contacts": ["ops@example.org"],
+            "default_max_age": 86400,
+            "encrypt_id_token_supported": False,
+            "encrypt_request_object_supported": False,
+            "encrypt_userinfo_supported": False,
+            "grant_types": ["authorization_code"],
+            "id_token_signed_response_alg": "RS256",
+            "post_logout_redirect_uris": ["https://rp.example.com/post"],
+            "redirect_uris": ["https://example.com/cli/authz_cb"],
+            "request_object_signing_alg": "ES256",
+            "response_modes": ["query", "fragment", "form_post"],
+            "response_types": ["code"],
+            "scope": ["openid"],
+            "subject_type": "public",
+            "token_endpoint_auth_method": "private_key_jwt",
+            "token_endpoint_auth_signing_alg": "ES256",
+            "userinfo_signed_response_alg": "ES256",
+        }
 
     def test_post_parse_2(self):
         OP_BASEURL = ISS
 
         provider_info_response = {
             "version": "3.0",
             "token_endpoint_auth_methods_supported": [
@@ -789,47 +791,49 @@
         assert _context.claims.use == {}
         resp = self.service.post_parse_response(provider_info_response)
 
         iss_jwks = ISS_KEY.export_jwks_as_json(issuer_id=ISS)
         with responses.RequestsMock() as rsps:
             rsps.add("GET", resp["jwks_uri"], body=iss_jwks, status=200)
 
-            self.service.update_service_context(resp, '')
+            self.service.update_service_context(resp, "")
 
         # static client registration
         _context.map_preferred_to_registered()
 
         use_copy = self.service.upstream_get("context").claims.use.copy()
         # jwks content will change dynamically between runs
-        assert 'jwks' in use_copy
-        del use_copy['jwks']
-        del use_copy['callback_uris']
-
-        assert use_copy == {'application_type': 'web',
-                            'backchannel_logout_session_required': True,
-                            'backchannel_logout_uri': 'https://rp.example.com/back',
-                            'client_id': 'client_id',
-                            'client_secret': 'a longesh password',
-                            'contacts': ['ops@example.org'],
-                            'default_max_age': 86400,
-                            'encrypt_id_token_supported': False,
-                            'encrypt_request_object_supported': False,
-                            'encrypt_userinfo_supported': False,
-                            'grant_types': ['authorization_code'],
-                            'id_token_signed_response_alg': 'RS256',
-                            'post_logout_redirect_uris': ['https://rp.example.com/post'],
-                            'redirect_uris': ['https://example.com/cli/authz_cb'],
-                            'request_object_signing_alg': 'ES256',
-                            'response_modes_supported': ['query', 'fragment', 'form_post'],
-                            'response_types': ['code'],
-                            'scope': ['openid'],
-                            'subject_type': 'public',
-                            'token_endpoint_auth_method': 'private_key_jwt',
-                            'token_endpoint_auth_signing_alg': 'ES256',
-                            'userinfo_signed_response_alg': 'ES256'}
+        assert "jwks" in use_copy
+        del use_copy["jwks"]
+        del use_copy["callback_uris"]
+
+        assert use_copy == {
+            "application_type": "web",
+            "backchannel_logout_session_required": True,
+            "backchannel_logout_uri": "https://rp.example.com/back",
+            "client_id": "client_id",
+            "client_secret": "a longesh password",
+            "contacts": ["ops@example.org"],
+            "default_max_age": 86400,
+            "encrypt_id_token_supported": False,
+            "encrypt_request_object_supported": False,
+            "encrypt_userinfo_supported": False,
+            "grant_types": ["authorization_code"],
+            "id_token_signed_response_alg": "RS256",
+            "post_logout_redirect_uris": ["https://rp.example.com/post"],
+            "redirect_uris": ["https://example.com/cli/authz_cb"],
+            "request_object_signing_alg": "ES256",
+            "response_modes": ["query", "fragment", "form_post"],
+            "response_types": ["code"],
+            "scope": ["openid"],
+            "subject_type": "public",
+            "token_endpoint_auth_method": "private_key_jwt",
+            "token_endpoint_auth_signing_alg": "ES256",
+            "userinfo_signed_response_alg": "ES256",
+        }
 
 
 def test_response_types_to_grant_types():
     req_args = ["code"]
     assert set(response_types_to_grant_types(req_args)) == {"authorization_code"}
     req_args = ["code", "code id_token"]
     assert set(response_types_to_grant_types(req_args)) == {"authorization_code", "implicit"}
@@ -844,96 +848,119 @@
 
     return idts.to_jwt(
         key=ISS_KEY.get_signing_key("ec", issuer_id=ISS), algorithm="ES256", lifetime=lifetime
     )
 
 
 class TestRegistration(object):
-
     @pytest.fixture(autouse=True)
     def create_request(self):
         self._iss = ISS
         client_config = {
             "redirect_uris": ["https://example.com/cli/authz_cb"],
             "issuer": self._iss,
             "requests_dir": "requests",
             "base_url": "https://example.com/cli/",
         }
-        entity = Entity(keyjar=make_keyjar(),
-                        config=client_config,
-                        services=DEFAULT_OIDC_SERVICES,
-                        client_type='oidc')
+        entity = Entity(
+            keyjar=make_keyjar(),
+            config=client_config,
+            services=DEFAULT_OIDC_SERVICES,
+            client_type="oidc",
+        )
         entity.get_context().issuer = "https://example.com"
         entity.get_context().map_supported_to_preferred()
         self.service = entity.get_service("registration")
 
     def test_construct(self):
         _req = self.service.construct()
         assert isinstance(_req, RegistrationRequest)
-        assert set(_req.keys()) == {'application_type',
-                                    'default_max_age',
-                                    'grant_types',
-                                    'id_token_signed_response_alg',
-                                    'jwks',
-                                    'redirect_uris',
-                                    'request_object_signing_alg',
-                                    'response_types',
-                                    'subject_type',
-                                    'token_endpoint_auth_method',
-                                    'token_endpoint_auth_signing_alg',
-                                    'userinfo_signed_response_alg'}
+        assert set(_req.keys()) == {
+            "application_type",
+            "default_max_age",
+            "grant_types",
+            "id_token_signed_response_alg",
+            "jwks",
+            "redirect_uris",
+            "request_object_signing_alg",
+            "response_modes",
+            "response_types",
+            "subject_type",
+            "token_endpoint_auth_method",
+            "token_endpoint_auth_signing_alg",
+            "userinfo_signed_response_alg",
+        }
 
     def test_config_with_post_logout(self):
         self.service.upstream_get("context").claims.set_preference(
-            "post_logout_redirect_uri", "https://example.com/post_logout")
+            "post_logout_redirect_uri", "https://example.com/post_logout"
+        )
 
         _req = self.service.construct()
         assert isinstance(_req, RegistrationRequest)
-        assert set(_req.keys()) == {'application_type',
-                                    'default_max_age',
-                                    'grant_types',
-                                    'id_token_signed_response_alg',
-                                    'jwks',
-                                    'post_logout_redirect_uri',
-                                    'redirect_uris',
-                                    'request_object_signing_alg',
-                                    'response_types',
-                                    'subject_type',
-                                    'token_endpoint_auth_method',
-                                    'token_endpoint_auth_signing_alg',
-                                    'userinfo_signed_response_alg'}
+        assert set(_req.keys()) == {
+            "application_type",
+            "default_max_age",
+            "grant_types",
+            "id_token_signed_response_alg",
+            "jwks",
+            "post_logout_redirect_uri",
+            "redirect_uris",
+            "request_object_signing_alg",
+            "response_modes",
+            "response_types",
+            "subject_type",
+            "token_endpoint_auth_method",
+            "token_endpoint_auth_signing_alg",
+            "userinfo_signed_response_alg",
+        }
         assert "post_logout_redirect_uri" in _req.keys()
 
 
 def test_config_with_required_request_uri():
     client_config = {
         "client_id": "client_id",
         "client_secret": "a longesh password",
         "redirect_uris": ["https://example.com/cli/authz_cb"],
         "issuer": ISS,
         "requests_dir": "requests",
-        "request_parameter": 'request_uri',
-        'request_uris': ["https://example.com/cli/requests"],
+        "request_parameter": "request_uri",
+        "request_uris": ["https://example.com/cli/requests"],
         "base_url": "https://example.com/cli",
     }
-    entity = Entity(keyjar=make_keyjar(), config=client_config, services=DEFAULT_OIDC_SERVICES,
-                    client_type='oidc')
+    entity = Entity(
+        keyjar=make_keyjar(),
+        config=client_config,
+        services=DEFAULT_OIDC_SERVICES,
+        client_type="oidc",
+    )
     entity.get_context().issuer = "https://example.com"
 
     pi_service = entity.get_service("provider_info")
     pi_service.match_preferences({"require_request_uri_registration": True})
 
     reg_service = entity.get_service("registration")
     _req = reg_service.construct()
     assert isinstance(_req, RegistrationRequest)
-    assert set(_req.keys()) == {"application_type", "response_types", "jwks",
-                                "redirect_uris", "grant_types", "id_token_signed_response_alg",
-                                "request_uris", 'default_max_age', 'request_object_signing_alg',
-                                'subject_type', 'token_endpoint_auth_method',
-                                'token_endpoint_auth_signing_alg', 'userinfo_signed_response_alg'}
+    assert set(_req.keys()) == {
+        "application_type",
+        "response_modes",
+        "response_types",
+        "jwks",
+        "redirect_uris",
+        "grant_types",
+        "id_token_signed_response_alg",
+        "request_uris",
+        "default_max_age",
+        "request_object_signing_alg",
+        "subject_type",
+        "token_endpoint_auth_method",
+        "token_endpoint_auth_signing_alg",
+        "userinfo_signed_response_alg",
+    }
 
 
 def test_config_logout_uri():
     client_config = {
         "client_id": "client_id",
         "client_secret": "a longesh password",
         "redirect_uris": ["https://example.com/cli/authz_cb"],
@@ -946,59 +973,69 @@
             "request_object_signing_alg": "ES256",
             "token_endpoint_auth_method": "private_key_jwt",
             "token_endpoint_auth_signing_alg": "ES256",
             "userinfo_signed_response_alg": "ES256",
             "post_logout_redirect_uri": "https://rp.example.com/post",
             "backchannel_logout_uri": "https://rp.example.com/back",
             "backchannel_logout_session_required": True,
-            'backchannel_logout_supported': True
-        }
+            "backchannel_logout_supported": True,
+        },
     }
-    entity = Entity(keyjar=make_keyjar(), config=client_config, services=DEFAULT_OIDC_SERVICES,
-                    client_type='oidc')
+    entity = Entity(
+        keyjar=make_keyjar(),
+        config=client_config,
+        services=DEFAULT_OIDC_SERVICES,
+        client_type="oidc",
+    )
     _context = entity.get_context()
     _context.issuer = "https://example.com"
 
     pi_service = entity.get_service("provider_info")
     _pi = {"require_request_uri_registration": True, "backchannel_logout_supported": True}
     pi_service.match_preferences(_pi)
 
     reg_service = entity.get_service("registration")
     _req = reg_service.construct()
     assert isinstance(_req, RegistrationRequest)
-    assert set(_req.keys()) == {'application_type',
-                                'default_max_age',
-                                'grant_types',
-                                'id_token_signed_response_alg',
-                                'jwks',
-                                'redirect_uris',
-                                'request_object_signing_alg',
-                                'request_uris',
-                                'response_types',
-                                'subject_type',
-                                'token_endpoint_auth_method',
-                                'token_endpoint_auth_signing_alg',
-                                'userinfo_signed_response_alg'}
+    assert set(_req.keys()) == {
+        "application_type",
+        "default_max_age",
+        "grant_types",
+        "id_token_signed_response_alg",
+        "jwks",
+        "redirect_uris",
+        "request_object_signing_alg",
+        "request_uris",
+        "response_modes",
+        "response_types",
+        "subject_type",
+        "token_endpoint_auth_method",
+        "token_endpoint_auth_signing_alg",
+        "userinfo_signed_response_alg",
+    }
 
 
 class TestUserInfo(object):
-
     @pytest.fixture(autouse=True)
     def create_request(self):
         self._iss = ISS
         client_config = {
             "client_id": "client_id",
             "client_secret": "a longesh password",
             "redirect_uris": ["https://example.com/cli/authz_cb"],
             "issuer": self._iss,
             "requests_dir": "requests",
             "base_url": "https://example.com/cli/",
         }
-        entity = Entity(keyjar=make_keyjar(), config=client_config, services=DEFAULT_OIDC_SERVICES,
-                        client_type='oidc')
+        entity = Entity(
+            keyjar=make_keyjar(),
+            config=client_config,
+            services=DEFAULT_OIDC_SERVICES,
+            client_type="oidc",
+        )
         entity.get_context().issuer = "https://example.com"
         self.service = entity.get_service("userinfo")
 
         entity.get_context().claims.use = {
             "userinfo_signed_response_alg": "RS256",
             "userinfo_encrypted_response_alg": "RSA-OAEP",
             "userinfo_encrypted_response_enc": "A256GCM",
@@ -1102,35 +1139,32 @@
         )
         assert _resp
 
     def test_unpack_encrypted_response(self):
         # Add encryption key
         _kj = build_keyjar([{"type": "RSA", "use": ["enc"]}], issuer_id="")
         # Own key jar gets the private key
-        self.service.upstream_get("attribute", 'keyjar').import_jwks(
+        self.service.upstream_get("attribute", "keyjar").import_jwks(
             _kj.export_jwks(private=True), issuer_id="client_id"
         )
         # opponent gets the public key
         ISS_KEY.import_jwks(_kj.export_jwks(), issuer_id="client_id")
 
         resp = OpenIDSchema(
             sub="diana", given_name="Diana", family_name="krall", iss=ISS, aud="client_id"
         )
         enckey = ISS_KEY.get_encrypt_key("rsa", issuer_id="client_id")
-        algspec = self.service.upstream_get("context").get_enc_alg_enc(
-            self.service.service_name
-        )
+        algspec = self.service.upstream_get("context").get_enc_alg_enc(self.service.service_name)
 
         enc_resp = resp.to_jwe(enckey, **algspec)
         _resp = self.service.parse_response(enc_resp, state="abcde", sformat="jwe")
         assert _resp
 
 
 class TestCheckSession(object):
-
     @pytest.fixture(autouse=True)
     def create_request(self):
         self._iss = ISS
         client_config = {
             "client_id": "client_id",
             "client_secret": "a longesh password",
             "redirect_uris": ["https://example.com/cli/authz_cb"],
@@ -1150,15 +1184,14 @@
         assert isinstance(_req, CheckSessionRequest)
         assert len(_req) == 1
         assert "id_token" in _req
         assert _req["id_token"] == "a.signed.jwt"
 
 
 class TestCheckID(object):
-
     @pytest.fixture(autouse=True)
     def create_request(self):
         self._iss = ISS
         client_config = {
             "client_id": "client_id",
             "client_secret": "a longesh password",
             "redirect_uris": ["https://example.com/cli/authz_cb"],
@@ -1178,50 +1211,50 @@
         assert isinstance(_req, CheckIDRequest)
         assert len(_req) == 1
         assert "id_token" in _req
         assert _req["id_token"] == "a.signed.jwt"
 
 
 class TestEndSession(object):
-
     @pytest.fixture(autouse=True)
     def create_request(self):
         self._iss = ISS
         client_config = {
             "client_id": "client_id",
             "client_secret": "a longesh password",
             "redirect_uris": ["https://example.com/cli/authz_cb"],
             "issuer": self._iss,
             "requests_dir": "requests",
             "base_url": "https://example.com/cli/",
-            "post_logout_redirect_uris": ["https://example.com/post_logout"]
+            "post_logout_redirect_uris": ["https://example.com/post_logout"],
         }
         services = {"checksession": {"class": "idpyoidc.client.oidc.end_session.EndSession"}}
         entity = Entity(keyjar=make_keyjar(), config=client_config, services=services)
         _context = entity.get_context()
         _context.issuer = "https://example.com"
         _context.map_supported_to_preferred()
         _context.map_preferred_to_registered()
         self.service = entity.get_service("end_session")
 
     def test_construct(self):
         self.service.upstream_get("service_context").cstate.update(
-            "abcde", {"id_token": "a.signed.jwt"})
+            "abcde", {"id_token": "a.signed.jwt"}
+        )
         _req = self.service.construct(state="abcde")
         assert isinstance(_req, EndSessionRequest)
         assert len(_req) == 3
         assert set(_req.keys()) == {"state", "id_token_hint", "post_logout_redirect_uri"}
 
 
 def test_authz_service_conf():
     client_config = {
         "client_id": "client_id",
         "client_secret": "a longesh password",
         "redirect_uris": ["https://example.com/cli/authz_cb"],
-        "response_types": ["code"],
+        "response_types": ["code", "id_token"],
     }
 
     services = {
         "authz": {
             "class": "idpyoidc.client.oidc.authorization.Authorization",
             "kwargs": {
                 "request_args": {
@@ -1231,46 +1264,53 @@
                             "acr": {"values": ["urn:mace:incommon:iap:silver"]},
                         }
                     }
                 }
             },
         }
     }
-    entity = Entity(keyjar=make_keyjar(), config=client_config, services=services,
-                    client_type='oidc')
+    entity = Entity(
+        keyjar=make_keyjar(), config=client_config, services=services, client_type="oidc"
+    )
     _context = entity.get_context()
     _context.issuer = "https://example.com"
     _context.map_supported_to_preferred()
     _context.map_preferred_to_registered()
     service = entity.get_service("authorization")
 
     req = service.construct()
-    assert set(req.keys()) == {'claims',
-                               'client_id',
-                               'nonce',
-                               'redirect_uri',
-                               'response_type',
-                               'scope',
-                               'state'}
+    assert set(req.keys()) == {
+        "claims",
+        "client_id",
+        "nonce",
+        "redirect_uri",
+        "response_type",
+        "scope",
+        "state",
+    }
 
     assert set(req["claims"].keys()) == {"id_token"}
 
 
 def test_jwks_uri_conf():
     client_config = {
         "client_secret": "a longesh password",
         "issuer": ISS,
         "client_id": "client_id",
         "jwks_uri": "https://example.com/jwks/jwks.json",
         "redirect_uris": ["https://example.com/cli/authz_cb"],
         "id_token_signed_response_alg": "RS384",
         "userinfo_signed_response_alg": "RS384",
     }
-    entity = Entity(keyjar=make_keyjar(), config=client_config, services=DEFAULT_OIDC_SERVICES,
-                    client_type='oidc')
+    entity = Entity(
+        keyjar=make_keyjar(),
+        config=client_config,
+        services=DEFAULT_OIDC_SERVICES,
+        client_type="oidc",
+    )
     _context = entity.get_context()
     _context.issuer = "https://example.com"
     _context.map_supported_to_preferred()
     _context.map_preferred_to_registered()
 
     assert _context.get_usage("jwks_uri")
 
@@ -1287,15 +1327,15 @@
             "userinfo_signed_response_alg": "RS384",
         },
     }
     entity = Entity(
         keyjar=make_keyjar(),
         config=client_config,
         services=DEFAULT_OIDC_SERVICES,
-        client_type='oidc'
+        client_type="oidc",
     )
     _context = entity.get_context()
     _context.issuer = "https://example.com"
     _context.map_supported_to_preferred()
     _context.map_preferred_to_registered()
 
     assert _context.get_usage("jwks_uri")
```

### Comparing `idpyoidc-2.0.0/tests/test_client_22_oidc.py` & `idpyoidc-2.1.0/tests/test_client_22_oidc.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,64 +46,62 @@
     @pytest.fixture(autouse=True)
     def create_client(self):
         self.redirect_uri = "http://example.com/redirect"
         conf = {
             "redirect_uris": ["https://example.com/cli/authz_cb"],
             "client_id": "client_1",
             "client_secret": "abcdefghijklmnop",
-            'client_authn_methods': ['bearer_header']
+            "client_authn_methods": ["bearer_header"],
         }
         self.client = RP(config=conf)
 
     def test_construct_authorization_request(self):
         req_args = {
             "state": "ABCDE",
             "redirect_uri": "https://example.com/auth_cb",
             "response_type": ["code"],
             "nonce": "nonce",
         }
 
-        self.client.get_context().cstate.set("ABCDE", {'iss': "issuer"})
+        self.client.get_context().cstate.set("ABCDE", {"iss": "issuer"})
 
         msg = self.client.get_service("authorization").construct(request_args=req_args)
         assert isinstance(msg, AuthorizationRequest)
         assert msg["redirect_uri"] == "https://example.com/auth_cb"
 
     def test_construct_accesstoken_request(self):
         _context = self.client.get_context()
         auth_request = AuthorizationRequest(redirect_uri="https://example.com/cli/authz_cb")
 
         _state = _context.cstate.create_key()
-        _context.cstate.set(_state, {'iss': "issuer"})
+        _context.cstate.set(_state, {"iss": "issuer"})
         auth_request["state"] = _state
 
         _context.cstate.update(_state, auth_request)
 
         auth_response = AuthorizationResponse(code="access_code")
 
         _context.cstate.update(_state, auth_response)
 
         # Bind access code to state
         req_args = {}
-        msg = self.client.get_service("accesstoken").construct(
-            request_args=req_args, state=_state
-        )
+        msg = self.client.get_service("accesstoken").construct(request_args=req_args, state=_state)
         assert isinstance(msg, AccessTokenRequest)
         assert msg.to_dict() == {
             "client_id": "client_1",
             "client_secret": "abcdefghijklmnop",
             "grant_type": "authorization_code",
             "state": _state,
             "code": "access_code",
             "redirect_uri": "https://example.com/cli/authz_cb",
         }
 
     def test_construct_refresh_token_request(self):
         _context = self.client.get_context()
-        _context.cstate.set("ABCDE", {'iss':"issuer"})
+        _context.cstate.set("ABCDE", {"iss": "issuer"})
 
         auth_request = AuthorizationRequest(
             redirect_uri="https://example.com/cli/authz_cb", state="state"
         )
 
         _context.cstate.update("ABCDE", auth_request)
 
@@ -124,15 +122,15 @@
             "grant_type": "refresh_token",
             "refresh_token": "refresh_with_me",
         }
 
     def test_do_userinfo_request_init(self):
         _context = self.client.get_context()
         _state = _context.cstate.create_key()
-        _context.cstate.set(_state, {'iss': "issuer"})
+        _context.cstate.set(_state, {"iss": "issuer"})
 
         auth_request = AuthorizationRequest(
             redirect_uri="https://example.com/cli/authz_cb", state="state"
         )
 
         _context.cstate.update(_state, auth_request)
```

### Comparing `idpyoidc-2.0.0/tests/test_client_23_pkce.py` & `idpyoidc-2.1.0/tests/test_client_23_pkce.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,31 +44,25 @@
 class TestPKCE256:
     @pytest.fixture(autouse=True)
     def create_client(self):
         config = {
             "client_id": "client_id",
             "client_secret": "a longesh password",
             "redirect_uris": ["https://example.com/cli/authz_cb"],
-            "preference": {
-                "response_types": ["code"]
-            },
+            "preference": {"response_types": ["code"]},
             "add_ons": {
                 "pkce": {
                     "function": "idpyoidc.client.oauth2.add_on.pkce.add_support",
-                    "kwargs": {
-                        "code_challenge_length": 64,
-                        "code_challenge_method": "S256"
-                    },
+                    "kwargs": {"code_challenge_length": 64, "code_challenge_method": "S256"},
                 }
             },
         }
-        self.entity = Entity(keyjar=CLI_KEY,
-                             config=config,
-                             services=DEFAULT_OAUTH2_SERVICES,
-                             client_type='oauth2')
+        self.entity = Entity(
+            keyjar=CLI_KEY, config=config, services=DEFAULT_OAUTH2_SERVICES, client_type="oauth2"
+        )
 
         if "add_ons" in config:
             do_add_ons(config["add_ons"], self.entity.get_services())
         _context = self.entity.get_context()
         _context.map_supported_to_preferred()
         _context.map_preferred_to_registered()
 
@@ -101,16 +95,16 @@
     def test_access_token_and_pkce(self):
         authz_service = self.entity.get_service("authorization")
         request = authz_service.construct_request({"state": "state", "response_type": "code"})
         _state = request["state"]
         auth_response = AuthorizationResponse(code="access code")
         _context = self.entity.get_context()
         _context.cstate.update(_state, auth_response)
-        #auth_serv = self.entity.get_service("authorization")
-        #_state = _context.cstate.create_state(iss="Issuer")
+        # auth_serv = self.entity.get_service("authorization")
+        # _state = _context.cstate.create_state(iss="Issuer")
 
         token_service = self.entity.get_service("accesstoken")
         request = token_service.construct_request(state=_state)
         assert set(request.keys()) == {
             "client_id",
             "redirect_uri",
             "grant_type",
```

### Comparing `idpyoidc-2.0.0/tests/test_client_24_oic_utils.py` & `idpyoidc-2.1.0/tests/test_client_24_oic_utils.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_client_25_oauth2_cc_ropc.py` & `idpyoidc-2.1.0/tests/test_client_25_oauth2_cc_ropc.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,20 @@
 
 KEYDEF = [{"type": "EC", "crv": "P-256", "use": ["sig"]}]
 
 BASE_URL = "https://example.com"
 
 
 class TestCC:
-
     @pytest.fixture(autouse=True)
     def create_service(self):
         client_config = {
             "client_id": "client_id",
             "client_secret": "another password",
-            "base_url": BASE_URL
+            "base_url": BASE_URL,
         }
         services = {
             "client_credentials": {
                 "class": "idpyoidc.client.oauth2.client_credentials.CCAccessTokenRequest"
             }
         }
 
@@ -30,16 +29,18 @@
         self.entity.get_service("client_credentials").endpoint = "https://example.com/token"
 
     def test_token_get_request(self):
         _srv = self.entity.get_service("client_credentials")
         _info = _srv.get_request_parameters()
         assert _info["method"] == "POST"
         assert _info["url"] == "https://example.com/token"
-        assert _info[
-                   "body"] == "grant_type=client_credentials&client_id=client_id&client_secret=another+password"
+        assert (
+            _info["body"]
+            == "grant_type=client_credentials&client_id=client_id&client_secret=another+password"
+        )
 
         assert _info["headers"] == {
             "Content-Type": "application/x-www-form-urlencoded",
         }
 
     def test_token_parse_response(self):
         _srv = self.entity.get_service("client_credentials")
@@ -59,46 +60,46 @@
         _key = rndstr(16)
         _srv.update_service_context(_response, key=_key)
         info = _srv.upstream_get("context").cstate.get(_key)
         assert "__expires_at" in info
 
 
 class TestROPC:
-
     @pytest.fixture(autouse=True)
     def create_service(self):
         client_config = {
             "client_id": "client_id",
             "client_secret": "another password",
-            "base_url": BASE_URL
+            "base_url": BASE_URL,
         }
         services = {
             "resource_owner_password_credentials": {
-                "class":
-                    "idpyoidc.client.oauth2.resource_owner_password_credentials"
-                    ".ROPCAccessTokenRequest"
+                "class": "idpyoidc.client.oauth2.resource_owner_password_credentials"
+                ".ROPCAccessTokenRequest"
             }
         }
 
         self.entity = Entity(config=client_config, services=services)
 
         self.entity.get_service(
-            "resource_owner_password_credentials").endpoint = "https://example.com/token"
+            "resource_owner_password_credentials"
+        ).endpoint = "https://example.com/token"
 
     def test_token_get_request(self):
         _srv = self.entity.get_service("resource_owner_password_credentials")
-        _info = _srv.get_request_parameters({'username': 'diana', 'password': 'krall'})
+        _info = _srv.get_request_parameters({"username": "diana", "password": "krall"})
         assert _info["method"] == "POST"
         assert _info["url"] == "https://example.com/token"
         assert _info["body"] == (
             "username=diana&"
             "password=krall&"
             "grant_type=password&"
             "client_id=client_id&"
-            "client_secret=another+password")
+            "client_secret=another+password"
+        )
 
         assert _info["headers"] == {
             "Content-Type": "application/x-www-form-urlencoded",
         }
 
     def test_token_parse_response(self):
         _srv = self.entity.get_service("resource_owner_password_credentials")
```

### Comparing `idpyoidc-2.0.0/tests/test_client_26_read_registration.py` & `idpyoidc-2.1.0/tests/test_client_26_read_registration.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,16 +30,16 @@
             "grant_types_supported": ["authorization_code"],
         }
         services = {
             "registration": {"class": "idpyoidc.client.oidc.registration.Registration"},
             "read_registration": {
                 "class": "idpyoidc.client.oidc.read_registration.RegistrationRead"
             },
-            'authorization': {'class': 'idpyoidc.client.oidc.authorization.Authorization'},
-            'accesstoken': {'class': 'idpyoidc.client.oidc.access_token.AccessToken'}
+            "authorization": {"class": "idpyoidc.client.oidc.authorization.Authorization"},
+            "accesstoken": {"class": "idpyoidc.client.oidc.access_token.AccessToken"},
         }
 
         self.entity = Entity(config=client_config, services=services)
         _context = self.entity.get_service_context()
         _context.map_supported_to_preferred()
         _context.map_preferred_to_registered()
```

### Comparing `idpyoidc-2.0.0/tests/test_client_27_conversation.py` & `idpyoidc-2.1.0/tests/test_client_27_conversation.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,30 +23,29 @@
     {"type": "EC", "crv": "P-256", "use": ["sig"]},
 ]
 
 JWKS_OP = {
     "keys": [
         {
             "d": "mcAW1xeNsjzyV1M7F7_cUHz0MIR"
-                 "-tcnKFJnbbo5UXxMRUPu17qwRHr8ttep1Ie64r2L9QlphcT9BjYd0KQ8ll3flIzLtiJv__MNPQVjk5bsYzb_erQRzSwLJU-aCcNFB8dIyQECzu-p44UVEPQUGzykImsSShvMQhcvrKiqqg7NlijJuEKHaKynV9voPsjwKYSqk6lH8kMloCaVS-dOkK-r7bZtbODUxx9GJWnxhX0JWXcdrPZRb29y9cdthrMcEaCXG23AxnMEfp-enDqarLHYTQrCBJXs_b-9k2d8v9zLm7E-Pf-0YGmaoJtX89lwQkO_SmFF3sXsnI2cFreqU3Q",
+            "-tcnKFJnbbo5UXxMRUPu17qwRHr8ttep1Ie64r2L9QlphcT9BjYd0KQ8ll3flIzLtiJv__MNPQVjk5bsYzb_erQRzSwLJU-aCcNFB8dIyQECzu-p44UVEPQUGzykImsSShvMQhcvrKiqqg7NlijJuEKHaKynV9voPsjwKYSqk6lH8kMloCaVS-dOkK-r7bZtbODUxx9GJWnxhX0JWXcdrPZRb29y9cdthrMcEaCXG23AxnMEfp-enDqarLHYTQrCBJXs_b-9k2d8v9zLm7E-Pf-0YGmaoJtX89lwQkO_SmFF3sXsnI2cFreqU3Q",
             "e": "AQAB",
             "kid": "c19uYlBJXzVfNjNZeGVnYmxncHZwUzZTZDVwUFdxdVJLU3AxQXdwaFdfbw",
             "kty": "RSA",
             "n": "3ZblhNL2CjRktLM9vyDn8jnA4G1B1HCpPh"
-                 "-gv2AK4m9qDBZPYZGOGqzeW3vanvLTBlqnPm0GHg4rOrfMEwwLrfMcgmg1y4GD0vVU8G9HP1"
-                 "-oUPtKUqaKOp313tFKzFh9_OHGQ6EmhxG7gegPR9kQXduTDXqBFi81MzRplIQ8DHLM3-n2CyDW1V"
-                 "-dhRVh"
-                 "-AM0ZcJyzR_DvZ3mhG44DysPdHQOSeWnpdn1d81"
-                 "-PriqZfhAF9tn1ihgtjXd5swf1HTSjLd7xv1hitGf2245Xmr"
-                 "-V2pQFzeMukLM3JKbTYbElsB7Zm0wZx49hZMtgx35XMoO04bifdbO3yLtTA5ovXN3fQ",
+            "-gv2AK4m9qDBZPYZGOGqzeW3vanvLTBlqnPm0GHg4rOrfMEwwLrfMcgmg1y4GD0vVU8G9HP1"
+            "-oUPtKUqaKOp313tFKzFh9_OHGQ6EmhxG7gegPR9kQXduTDXqBFi81MzRplIQ8DHLM3-n2CyDW1V"
+            "-dhRVh"
+            "-AM0ZcJyzR_DvZ3mhG44DysPdHQOSeWnpdn1d81"
+            "-PriqZfhAF9tn1ihgtjXd5swf1HTSjLd7xv1hitGf2245Xmr"
+            "-V2pQFzeMukLM3JKbTYbElsB7Zm0wZx49hZMtgx35XMoO04bifdbO3yLtTA5ovXN3fQ",
             "p": "88aNu59aBn0elksaVznzoVKkdbT5B4euhOIEqJoFvFbEocw9mC4k"
-                 "-yozIAQSV5FEakoSPOl8lrymCoM3Q1fVHfaM9Rbb9RCRlsV1JOeVVZOE05HUdz8zOIqLBDEGM_oQqDwF_kp"
-                 "-4nDTZ1-dtnGdTo4Cf7QRuApzE_dwVabUCTc",
-            "q":
-                "6LOHuM7H_0kDrMTwUEX7Aubzr792GoJ6EgTKIQY25SAFTZpYwuC3NnqlAdy8foIa3d7eGU2yICRbBG0S_ITcooDFrOa7nZ6enMUclMTxW8FwwvBXeIHo9cIsrKYtOThGplz43Cvl73MK5M58ZRmuhaNYa6Mk4PL4UokARfEiDus",
+            "-yozIAQSV5FEakoSPOl8lrymCoM3Q1fVHfaM9Rbb9RCRlsV1JOeVVZOE05HUdz8zOIqLBDEGM_oQqDwF_kp"
+            "-4nDTZ1-dtnGdTo4Cf7QRuApzE_dwVabUCTc",
+            "q": "6LOHuM7H_0kDrMTwUEX7Aubzr792GoJ6EgTKIQY25SAFTZpYwuC3NnqlAdy8foIa3d7eGU2yICRbBG0S_ITcooDFrOa7nZ6enMUclMTxW8FwwvBXeIHo9cIsrKYtOThGplz43Cvl73MK5M58ZRmuhaNYa6Mk4PL4UokARfEiDus",
             "use": "sig",
         },
         {
             "crv": "P-256",
             "d": "N2dg0-DAROBF8owQA4-uY5s0Ab-Fep_42kEFQG4BNVQ",
             "kid": "UnpYbi0tWC1HaEtyRFMtSmkyZDVHUHZVNDF0d21KTVk1dzEwYmhpNlVtQQ",
             "kty": "EC",
@@ -66,23 +65,21 @@
     "keys": [
         {
             "kty": "RSA",
             "use": "sig",
             "kid": "Mk0yN2w0N3BZLWtyOEpQWGFmNDZvQi1hbDl2azR3ai1WNElGdGZQSFd6MA",
             "e": "AQAB",
             "n": "yPrOADZtGoa9jxFCmDsJ1nAYmzgznUxCtUlb_ty33"
-                 "-AFNEqzW_pSLr5g6RQAPGsvVQqbsb9AB18QNgz"
-                 "-eG7cnvKIIR7JXWCuGv_Q9MwoRD0-zaYGRbRvFoTZokZMB6euBfMo6kijJ"
-                 "-gdKuSaxIE84X_Fcf1ESAKJ0EX6Cxdm8hKkBelGIDPMW5z7EHQ8OuLCQtTJnDvbjEOk9sKzkKqVj53XFs5vjd4WUhxS6xIDcWE-lTafUpm0BsobklLePidHxyAMGOunL_Pt3RCLZGlWeWOO9fZhLtydiDWiZlcNR0FQEX_mfV1kCOHHBFN1VKOY2pyJpjp9djdtHxPZ9fP35w",
-            "d":
-                "aRBTqGDLYFaXuba4LYSPe_5Vnq8erFg1dzfGU9Fmfi5KCjAS2z5cv_reBnpiNTODJt3Izn7AJhpYCyl3zdWGl8EJ0OabNalY2txoi9A-LI4nyrHEDaRpfkgszVwaWtYZbxrShMc8I5x_wvCGx7sX7Hoy6YgQreRFzw8Fy86MDncpmcUwQTnXVUMLgioeYz5gW6rwXkqj_NVyuHPiheykJG026cXFNBWplCk4ET1bvf_6ZB9QmLwO16Pu2O-dtu1HHDOqI7y6-YgKIC6mcLrQrF9-FO7NkilcOB7zODNiYzhDBQ2YJAbcdn_3M_lkhaFwR-n4WB7vCM0vNqz7lEg6QQ",
-            "p":
-                "_STNoJFkX9_uw8whytVmTrHP5K7vcZBIH9nuCTvj137lC48ZpR1UARx4qShxHLfK7DrufHd7TYnJkEMNUHFmdKvkaVQMY0_BsBSvCrUl10gzxsI08hg53L17E1Pe73iZp3f5nA4eB-1YB-km1Cc-Xs10OPWedJHf9brlCPDLAb8",
+            "-AFNEqzW_pSLr5g6RQAPGsvVQqbsb9AB18QNgz"
+            "-eG7cnvKIIR7JXWCuGv_Q9MwoRD0-zaYGRbRvFoTZokZMB6euBfMo6kijJ"
+            "-gdKuSaxIE84X_Fcf1ESAKJ0EX6Cxdm8hKkBelGIDPMW5z7EHQ8OuLCQtTJnDvbjEOk9sKzkKqVj53XFs5vjd4WUhxS6xIDcWE-lTafUpm0BsobklLePidHxyAMGOunL_Pt3RCLZGlWeWOO9fZhLtydiDWiZlcNR0FQEX_mfV1kCOHHBFN1VKOY2pyJpjp9djdtHxPZ9fP35w",
+            "d": "aRBTqGDLYFaXuba4LYSPe_5Vnq8erFg1dzfGU9Fmfi5KCjAS2z5cv_reBnpiNTODJt3Izn7AJhpYCyl3zdWGl8EJ0OabNalY2txoi9A-LI4nyrHEDaRpfkgszVwaWtYZbxrShMc8I5x_wvCGx7sX7Hoy6YgQreRFzw8Fy86MDncpmcUwQTnXVUMLgioeYz5gW6rwXkqj_NVyuHPiheykJG026cXFNBWplCk4ET1bvf_6ZB9QmLwO16Pu2O-dtu1HHDOqI7y6-YgKIC6mcLrQrF9-FO7NkilcOB7zODNiYzhDBQ2YJAbcdn_3M_lkhaFwR-n4WB7vCM0vNqz7lEg6QQ",
+            "p": "_STNoJFkX9_uw8whytVmTrHP5K7vcZBIH9nuCTvj137lC48ZpR1UARx4qShxHLfK7DrufHd7TYnJkEMNUHFmdKvkaVQMY0_BsBSvCrUl10gzxsI08hg53L17E1Pe73iZp3f5nA4eB-1YB-km1Cc-Xs10OPWedJHf9brlCPDLAb8",
             "q": "yz9T0rPEc0ZPjSi45gsYiQL2KJ3UsPHmLrgOHq0D4UvsB6UFtUtOWh7A1UpQdmBuHjIJz"
-                 "-Iq7VH4kzlI6VxoXhwE69oxBXr4I7fBudZRvlLuIJS9M2wvsTVouj0DBYSR6ZlAQHCCou89P2P6zQCEaqu7bWXNcpyTixbbvOU1w9k",
+            "-Iq7VH4kzlI6VxoXhwE69oxBXr4I7fBudZRvlLuIJS9M2wvsTVouj0DBYSR6ZlAQHCCou89P2P6zQCEaqu7bWXNcpyTixbbvOU1w9k",
         },
         {
             "kty": "EC",
             "use": "sig",
             "kid": "ME9NV3VQV292OTA4T1pNLXZoVjd2TldVSjNrNEkycjU2ZjkycldQOTcyUQ",
             "crv": "P-256",
             "x": "WWoO_Exim-LOD1k8QPi_CdU8M_VUSF7DkJCKR7PFWhQ",
@@ -102,39 +99,22 @@
 
 # ---------------------------------------------------
 
 SERVICES = {
     "WebFinger": {"class": WebFinger},
     "discovery": {
         "class": "idpyoidc.client.oidc.provider_info_discovery.ProviderInfoDiscovery",
-        "kwargs": {}
+        "kwargs": {},
     },
-    "registration": {
-        "class": "idpyoidc.client.oidc.registration.Registration",
-        "kwargs": {}
-    },
-    "authorization": {
-        "class": "idpyoidc.client.oidc.authorization.Authorization",
-        "kwargs": {}
-    },
-    "accesstoken": {
-        "class": "idpyoidc.client.oidc.access_token.AccessToken",
-        "kwargs": {}
-    },
-    "refresh_token": {
-        "class": "idpyoidc.client.oidc.refresh_access_token.RefreshAccessToken"
-    },
-    "userinfo": {
-        "class": "idpyoidc.client.oidc.userinfo.UserInfo",
-        "kwargs": {}
-    },
-    "end_session": {
-        "class": "idpyoidc.client.oidc.end_session.EndSession",
-        "kwargs": {}
-    }
+    "registration": {"class": "idpyoidc.client.oidc.registration.Registration", "kwargs": {}},
+    "authorization": {"class": "idpyoidc.client.oidc.authorization.Authorization", "kwargs": {}},
+    "accesstoken": {"class": "idpyoidc.client.oidc.access_token.AccessToken", "kwargs": {}},
+    "refresh_token": {"class": "idpyoidc.client.oidc.refresh_access_token.RefreshAccessToken"},
+    "userinfo": {"class": "idpyoidc.client.oidc.userinfo.UserInfo", "kwargs": {}},
+    "end_session": {"class": "idpyoidc.client.oidc.end_session.EndSession", "kwargs": {}},
 }
 
 
 def test_conversation():
     config = {
         "application_type": "web",
         "contacts": ["ops@example.org"],
@@ -145,44 +125,44 @@
         "request_uris": [f"{RP_BASEURL}/requests"],
         "token_endpoint_auth_methods_supported": ["private_key_jwt"],
         "token_endpoint_auth_signing_alg_values_supported": ["ES256"],
         "userinfo_signing_alg_values_supported": ["ES256"],
         "post_logout_redirect_uri": "https://rp.example.com/post",
         "backchannel_logout_uri": "https://rp.example.com/back",
         "backchannel_logout_session_required": True,
-        'allow': {'missing_kid': True},
-        "client_authn_methods": ['bearer_header'],
-        "services": SERVICES
+        "allow": {"missing_kid": True},
+        "client_authn_methods": ["bearer_header"],
+        "services": SERVICES,
     }
 
-    entity = Entity(config=config, keyjar=RP_KEYJAR, client_type='oidc')
+    entity = Entity(config=config, keyjar=RP_KEYJAR, client_type="oidc")
 
     assert set(entity.get_services().keys()) == {
         "accesstoken",
         "authorization",
         "webfinger",
         "registration",
         "refresh_token",
         "userinfo",
         "provider_info",
-        'end_session',
+        "end_session",
     }
     service_context = entity.get_context()
 
     # ======================== WebFinger ========================
 
     webfinger_service = entity.get_service("webfinger")
     info = webfinger_service.get_request_parameters(request_args={"resource": "foobar@example.org"})
 
     assert (
-            info["url"] == "https://example.org/.well-known/webfinger?rel=http"
-                           "%3A%2F"
-                           "%2Fopenid.net%2Fspecs%2Fconnect%2F1.0%2Fissuer"
-                           "&resource"
-                           "=acct%3Afoobar%40example.org"
+        info["url"] == "https://example.org/.well-known/webfinger?rel=http"
+        "%3A%2F"
+        "%2Fopenid.net%2Fspecs%2Fconnect%2F1.0%2Fissuer"
+        "&resource"
+        "=acct%3Afoobar%40example.org"
     )
 
     webfinger_response = json.dumps(
         {
             "subject": "acct:foobar@example.org",
             "links": [
                 {
@@ -401,43 +381,46 @@
             "end_session_endpoint": "{}/end_session".format(OP_BASEURL),
         }
     )
 
     resp = provider_info_service.parse_response(provider_info_response)
 
     assert isinstance(resp, ProviderConfigurationResponse)
-    provider_info_service.update_service_context(resp, '')
+    provider_info_service.update_service_context(resp, "")
 
     _pi = entity.get_context().provider_info
     assert _pi["issuer"] == OP_BASEURL
     assert _pi["authorization_endpoint"] == "https://example.org/op/authorization"
     assert _pi["registration_endpoint"] == "https://example.org/op/registration"
 
     # =================== Client registration ====================
     registration_service = entity.get_service("registration")
     info = registration_service.get_request_parameters()
 
     assert info["url"] == "https://example.org/op/registration"
     _body = json.loads(info["body"])
-    assert set(_body.keys()) == {'application_type',
-                                 'backchannel_logout_session_required',
-                                 'backchannel_logout_uri',
-                                 'contacts',
-                                 'default_max_age',
-                                 'grant_types',
-                                 'id_token_signed_response_alg',
-                                 'jwks',
-                                 'redirect_uris',
-                                 'request_object_signing_alg',
-                                 'request_uris',
-                                 'response_types',
-                                 'subject_type',
-                                 'token_endpoint_auth_method',
-                                 'token_endpoint_auth_signing_alg',
-                                 'userinfo_signed_response_alg'}
+    assert set(_body.keys()) == {
+        "application_type",
+        "backchannel_logout_session_required",
+        "backchannel_logout_uri",
+        "contacts",
+        "default_max_age",
+        "grant_types",
+        "id_token_signed_response_alg",
+        "jwks",
+        "redirect_uris",
+        "request_object_signing_alg",
+        "request_uris",
+        "response_modes",
+        "response_types",
+        "subject_type",
+        "token_endpoint_auth_method",
+        "token_endpoint_auth_signing_alg",
+        "userinfo_signed_response_alg",
+    }
     assert info["headers"] == {"Content-Type": "application/json"}
 
     now = int(time.time())
 
     op_client_registration_response = json.dumps(
         {
             "client_id": "zls2qhN1jO6A",
@@ -456,15 +439,15 @@
     )
 
     response = registration_service.parse_response(op_client_registration_response)
 
     registration_service.update_service_context(response)
 
     assert service_context.get_client_id() == "zls2qhN1jO6A"
-    assert service_context.get_usage('client_secret') == "c8434f28cf9375d9a7"
+    assert service_context.get_usage("client_secret") == "c8434f28cf9375d9a7"
     assert set(service_context.registration_response.keys()) == {
         "client_secret_expires_at",
         "contacts",
         "client_id",
         "token_endpoint_auth_method",
         "redirect_uris",
         "response_types",
@@ -521,19 +504,15 @@
     request_args = {"state": STATE, "redirect_uri": service_context.get_usage("redirect_uris")[0]}
 
     info = token_service.get_request_parameters(request_args=request_args)
 
     assert info["url"] == "https://example.org/op/token"
     _qp = parse_qs(info["body"])
     # since the default is private_key_jwt !!!
-    assert set(_qp.keys()) == {'client_id',
-                               'code',
-                               'grant_type',
-                               'redirect_uri',
-                               'state'}
+    assert set(_qp.keys()) == {"client_id", "code", "grant_type", "redirect_uri", "state"}
     assert info["headers"]["Content-Type"] == "application/x-www-form-urlencoded"
 
     # create the IdToken
     _jwt = JWT(OP_KEYJAR, OP_BASEURL, lifetime=3600, sign=True, sign_alg="RS256")
     payload = {
         "sub": "1b2fc9341a16ae4e30082965d537",
         "acr": "PASSWORD",
@@ -566,28 +545,30 @@
         "sub",
     }
 
     token_service.update_service_context(_resp, key=STATE)
 
     _item = _cstate.get(STATE)
 
-    assert set(_item.keys()) == {'__expires_at',
-                                 '__verified_id_token',
-                                 'access_token',
-                                 'client_id',
-                                 'code',
-                                 'expires_in',
-                                 'id_token',
-                                 'iss',
-                                 'nonce',
-                                 'redirect_uri',
-                                 'response_type',
-                                 'scope',
-                                 'state',
-                                 'token_type'}
+    assert set(_item.keys()) == {
+        "__expires_at",
+        "__verified_id_token",
+        "access_token",
+        "client_id",
+        "code",
+        "expires_in",
+        "id_token",
+        "iss",
+        "nonce",
+        "redirect_uri",
+        "response_type",
+        "scope",
+        "state",
+        "token_type",
+    }
 
     assert _item["token_type"] == "Bearer"
     assert _item["access_token"] == "Z0FBQUFBQmFkdFF"
 
     # =================== User info ====================
 
     userinfo_service = entity.get_service("userinfo")
```

### Comparing `idpyoidc-2.0.0/tests/test_client_28_rp_handler_oidc.py` & `idpyoidc-2.1.0/tests/test_client_30_rp_handler_oidc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import os
 from urllib.parse import parse_qs
 from urllib.parse import urlparse
 from urllib.parse import urlsplit
 
-from cryptojwt.key_jar import init_key_jar
 import pytest
 import responses
+from cryptojwt.key_jar import init_key_jar
 
 from idpyoidc.client.entity import Entity
 from idpyoidc.client.rp_handler import RPHandler
 from idpyoidc.message.oidc import AccessTokenResponse
 from idpyoidc.message.oidc import AuthorizationResponse
 from idpyoidc.message.oidc import IdToken
 from idpyoidc.message.oidc import JRD
@@ -24,30 +24,28 @@
 
 PREF = {
     "application_type": "web",
     "contacts": ["ops@example.com"],
     "response_types_supported": [
         "code",
         "id_token",
-        "id_token token",
         "code id_token",
-        "code id_token token",
-        "code token",
     ],
     "token_endpoint_auth_methods_supported": ["client_secret_basic"],
     "scopes_supported": ["openid", "profile", "email", "address", "phone"],
     "verify_args": {"allow_sign_alg_none": True},
 }
 
 CLIENT_CONFIG = {
     "": {
         "preference": PREF,
         "redirect_uris": None,
         "base_url": BASE_URL,
         "request_parameter": "request_uris",
+        "client_type": "oidc",
         "services": {
             "web_finger": {"class": "idpyoidc.client.oidc.webfinger.WebFinger"},
             "discovery": {
                 "class": "idpyoidc.client.oidc.provider_info_discovery.ProviderInfoDiscovery"
             },
             "registration": {"class": "idpyoidc.client.oidc.registration.Registration"},
             "authorization": {"class": "idpyoidc.client.oidc.authorization.Authorization"},
@@ -107,18 +105,19 @@
             },
         },
     },
     "github": {
         "issuer": "https://github.com/login/oauth/authorize",
         "client_id": "eeeeeeeee",
         "client_secret": "aaaaaaaaaaaaaaaaaaaa",
+        "client_type": "oidc",
         "redirect_uris": ["{}/authz_cb/github".format(BASE_URL)],
         "preference": {
             "response_types_supported": ["code"],
-            "scopes_supported": ["user", "public_repo", 'openid'],
+            "scopes_supported": ["user", "public_repo", "openid"],
             "token_endpoint_auth_methods_supported": [],
             "verify_args": {"allow_sign_alg_none": True},
         },
         "provider_info": {
             "authorization_endpoint": "https://github.com/login/oauth/authorize",
             "token_endpoint": "https://github.com/login/oauth/access_token",
             "userinfo_endpoint": "https://api.github.com/user",
@@ -134,21 +133,22 @@
             },
         },
     },
     "github2": {
         "issuer": "https://github.com/login/oauth/authorize",
         "client_id": "eeeeeeeee",
         "client_secret": "aaaaaaaaaaaaaaaaaaaa",
+        "client_type": "oidc",
         "redirect_uris": ["{}/authz_cb/github".format(BASE_URL)],
         "preference": {
             "response_types_supported": ["code"],
             "scopes_supported": ["user", "public_repo"],
             "token_endpoint_auth_methods_supported": [],
             "verify_args": {"allow_sign_alg_none": True},
-            'encrypt_request_object': False
+            "encrypt_request_object": False,
         },
         "provider_info": {
             "authorization_endpoint": "https://github.com/login/oauth/authorize",
             "token_endpoint": "https://github.com/login/oauth/access_token",
             "userinfo_endpoint": "https://api.github.com/user",
             "request_parameter_supported": True,
             "request_uri_parameter_supported": True,
@@ -201,19 +201,26 @@
     public_path="{}/pub_github.jwks".format(_dirname),
     private_path="{}/priv_github.jwks".format(_dirname),
     key_defs=KEYDEFS,
     issuer_id=CLIENT_CONFIG["github"]["issuer"],
 )
 
 
+def get_state_from_url(url):
+    p = urlsplit(url)
+    qp = parse_qs(p.query)
+    return qp["state"][0]
+
+
 def iss_id(iss):
     return CLIENT_CONFIG[iss]["issuer"]
 
 
 class TestRPHandler(object):
+
     @pytest.fixture(autouse=True)
     def rphandler_setup(self):
         self.rph = RPHandler(
             BASE_URL, client_configs=CLIENT_CONFIG, keyjar=CLI_KEY, module_dirs=["oidc"]
         )
 
     def test_pick_config(self):
@@ -238,38 +245,44 @@
             "refresh_token",
         }
 
         _context = client.get_context()
 
         # Neither provider info discovery not client registration has been done
         # So only preferences so far.
-        assert _context.get_preference('client_id') == "eeeeeeeee"
+        assert _context.get_preference("client_id") == "eeeeeeeee"
         assert _context.get_preference("client_secret") == "aaaaaaaaaaaaaaaaaaaa"
         assert _context.issuer == "https://github.com/login/oauth/authorize"
 
         assert _context.get("provider_info") is not None
         assert set(_context.get("provider_info").keys()) == {
             "authorization_endpoint",
             "token_endpoint",
             "userinfo_endpoint",
         }
 
         _pref = [k for k, v in _context.prefers().items() if v]
-        assert set(_pref) == {'client_id', 'client_secret', 'redirect_uris',
-                              'response_types_supported', 'callback_uris', 'scopes_supported'}
+        assert set(_pref) == {
+            "client_id",
+            "client_secret",
+            "redirect_uris",
+            "response_types_supported",
+            "callback_uris",
+            "scopes_supported",
+        }
 
         _github_id = iss_id("github")
-        _keyjar = _context.upstream_get('attribute', 'keyjar')
+        _keyjar = _context.upstream_get("attribute", "keyjar")
         _keyjar.import_jwks(GITHUB_KEY.export_jwks(issuer_id=_github_id), _github_id)
 
         # The key jar should only contain a symmetric key that is the clients
         # secret. 2 because one is marked for encryption and the other signing
         # usage.
 
-        assert set(_keyjar.owners()) == {"", 'eeeeeeeee', _github_id}
+        assert set(_keyjar.owners()) == {"", "eeeeeeeee", _github_id}
         keys = _keyjar.get_issuer_keys("")
         assert len(keys) == 3
 
         assert _context.base_url == BASE_URL
 
     def test_do_provider_info(self):
         client = self.rph.init_client("github")
@@ -288,69 +301,67 @@
         issuer = self.rph.do_provider_info(client)
         self.rph.do_client_registration(client, "github")
 
         # only 2 things should have happened
 
         assert self.rph.hash2issuer["github"] == issuer
         assert (
-                client.get_context().get_preference('callback_uris').get(
-                    "post_logout_redirect_uris") is None
+                client.get_context().get_preference("callback_uris").get(
+                    "post_logout_redirect_uris")
+                is None
         )
 
     def test_do_client_setup(self):
         client = self.rph.client_setup("github")
         _github_id = iss_id("github")
         _context = client.get_context()
 
         # Neither provider info discovery not client registration has been done
         # So only preferences so far.
-        assert _context.get_preference('client_id') == "eeeeeeeee"
+        assert _context.get_preference("client_id") == "eeeeeeeee"
         assert _context.get_preference("client_secret") == "aaaaaaaaaaaaaaaaaaaa"
         assert _context.issuer == _github_id
 
-        _keyjar = _context.upstream_get('attribute', 'keyjar')
+        _keyjar = _context.upstream_get("attribute", "keyjar")
         _keyjar.import_jwks(GITHUB_KEY.export_jwks(issuer_id=_github_id), _github_id)
 
         assert set(_keyjar.owners()) == {"", "eeeeeeeee", _github_id}
         keys = _keyjar.get_issuer_keys("")
         assert len(keys) == 3
 
         for service_type in ["authorization", "accesstoken", "userinfo"]:
             _srv = client.get_service(service_type)
             _endp = _srv.upstream_get("context").get("provider_info")[_srv.endpoint_name]
             assert _srv.endpoint == _endp
 
-        assert self.rph.hash2issuer["github"] == _context.get("issuer")
-
     def test_create_callbacks(self):
         client = self.rph.init_client("https://op.example.com/")
         _srv = client.get_service("registration")
         _context = _srv.upstream_get("context")
-        cb = _context.get_preference('callback_uris')
+        cb = _context.get_preference("callback_uris")
 
         assert set(cb.keys()) == {"request_uris", "redirect_uris"}
-        assert set(cb['redirect_uris'].keys()) == {'code'}
+        assert set(cb["redirect_uris"].keys()) == {"query", "fragment"}
         _hash = _context.iss_hash
 
-        assert cb['redirect_uris']["code"] == [f"https://example.com/rp/authz_cb/{_hash}"]
+        assert cb["redirect_uris"]["query"] == [f"https://example.com/rp/authz_cb/{_hash}"]
 
         assert list(self.rph.hash2issuer.keys()) == [_hash]
 
         assert self.rph.hash2issuer[_hash] == "https://op.example.com/"
 
     def test_begin(self):
-        res = self.rph.begin(issuer_id="github")
-        assert set(res.keys()) == {"url", "state"}
+        url = self.rph.begin(issuer_id="github")
         _github_id = iss_id("github")
 
         client = self.rph.issuer2rp[_github_id]
 
         assert client.get_context().issuer == _github_id
 
-        part = urlsplit(res["url"])
+        part = urlsplit(url)
         assert part.scheme == "https"
         assert part.netloc == "github.com"
         assert part.path == "/login/oauth/authorize"
         query = parse_qs(part.query)
 
         assert set(query.keys()) == {
             "nonce",
@@ -362,78 +373,85 @@
         }
 
         # nonce and state are created on the fly so can't check for those
         # that all values are lists is a parse_qs artifact.
         assert query["client_id"] == ["eeeeeeeee"]
         assert query["redirect_uri"] == ["https://example.com/rp/authz_cb/github"]
         assert query["response_type"] == ["code"]
-        assert set(query["scope"][0].split(' ')) == {"openid", "user", "public_repo"}
+        assert set(query["scope"][0].split(" ")) == {"openid", "user", "public_repo"}
 
     def test_get_session_information(self):
-        res = self.rph.begin(issuer_id="github")
-        _session = self.rph.get_session_information(res["state"])
+        url = self.rph.begin(issuer_id="github")
+        _session = self.rph.get_session_information(get_state_from_url(url))
         assert self.rph.client_configs["github"]["issuer"] == _session["iss"]
 
     def test_get_client_from_session_key(self):
-        res = self.rph.begin(issuer_id="linkedin")
-        cli1 = self.rph.get_client_from_session_key(state=res["state"])
-        _session = self.rph.get_session_information(res["state"])
-        cli2 = self.rph.issuer2rp[_session['iss']]
+        url = self.rph.begin(issuer_id="linkedin")
+        _state = get_state_from_url(url)
+        cli1 = self.rph.get_client_from_session_key(state=_state)
+        _session = self.rph.get_session_information(_state)
+        cli2 = self.rph.issuer2rp[_session["iss"]]
         assert cli1 == cli2
         # redo
-        self.rph.do_provider_info(state=res["state"])
+        self.rph.do_provider_info(state=_state)
         # get new redirect_uris
         cli2.get_context().set_preference("redirect_uris", [])
-        self.rph.do_client_registration(state=res["state"])
+        self.rph.do_client_registration(state=_state)
 
     def test_finalize_auth(self):
-        res = self.rph.begin(issuer_id="linkedin")
-        _session = self.rph.get_session_information(res["state"])
-        client = self.rph.issuer2rp[_session['iss']]
+        url = self.rph.begin(issuer_id="linkedin")
+        _state = get_state_from_url(url)
+        _session = self.rph.get_session_information(_state)
+        client = self.rph.issuer2rp[_session["iss"]]
 
-        auth_response = AuthorizationResponse(code="access_code", state=res["state"])
-        resp = self.rph.finalize_auth(client, _session['iss'], auth_response.to_dict())
+        auth_response = AuthorizationResponse(code="access_code", state=_state)
+        resp = self.rph.finalize_auth(client, _session["iss"], auth_response.to_dict())
         assert set(resp.keys()) == {"state", "code"}
-        _state = client.get_context().cstate.get(res["state"])
-        assert set(_state.keys()) == {'client_id',
-                                      'code',
-                                      'iss',
-                                      'nonce',
-                                      'redirect_uri',
-                                      'response_type',
-                                      'scope',
-                                      'state'}
+        _state = client.get_context().cstate.get(_state)
+        assert set(_state.keys()) == {
+            "client_id",
+            "code",
+            "iss",
+            "nonce",
+            "redirect_uri",
+            "response_type",
+            "scope",
+            "state",
+        }
 
     def test_get_client_authn_method(self):
-        res = self.rph.begin(issuer_id="github")
-        _session = self.rph.get_session_information(res["state"])
-        client = self.rph.issuer2rp[_session['iss']]
+        url = self.rph.begin(issuer_id="github")
+        _state = get_state_from_url(url)
+        _session = self.rph.get_session_information(_state)
+        client = self.rph.issuer2rp[_session["iss"]]
         authn_method = self.rph.get_client_authn_method(client, "token_endpoint")
-        assert authn_method == ''
+        assert authn_method == ""
 
-        res = self.rph.begin(issuer_id="linkedin")
-        _session = self.rph.get_session_information(res["state"])
-        client = self.rph.issuer2rp[_session['iss']]
+        url = self.rph.begin(issuer_id="linkedin")
+        _state = get_state_from_url(url)
+        _session = self.rph.get_session_information(_state)
+        client = self.rph.issuer2rp[_session["iss"]]
         authn_method = self.rph.get_client_authn_method(client, "token_endpoint")
         assert authn_method == "client_secret_post"
 
     def test_get_tokens(self):
-        res = self.rph.begin(issuer_id="github")
-        _session = self.rph.get_session_information(res["state"])
-        client = self.rph.issuer2rp[_session['iss']]
+        url = self.rph.begin(issuer_id="github")
+        _state = get_state_from_url(url)
+        _session = self.rph.get_session_information(_state)
+        client = self.rph.issuer2rp[_session["iss"]]
 
         _github_id = iss_id("github")
         _context = client.get_context()
-        _keyjar = _context.upstream_get('attribute', 'keyjar')
+        _keyjar = _context.upstream_get("attribute", "keyjar")
         _keyjar.import_jwks(GITHUB_KEY.export_jwks(issuer_id=_github_id), _github_id)
 
         _nonce = _session["nonce"]
-        _iss = _session['iss']
+        _iss = _session["iss"]
         _aud = _context.get_client_id()
-        idval = {"nonce": _nonce, "sub": "EndUserSubject", 'iss': _iss, "aud": _aud}
+        idval = {"nonce": _nonce, "sub": "EndUserSubject", "iss": _iss, "aud": _aud}
 
         idts = IdToken(**idval)
         _signed_jwt = idts.to_jwt(
             key=GITHUB_KEY.get_signing_key(issuer_id=_github_id), algorithm="RS256", lifetime=300
         )
 
         _info = {
@@ -451,55 +469,58 @@
                 _url,
                 body=at.to_json(),
                 adding_headers={"Content-Type": "application/json"},
                 status=200,
             )
             client.get_service("accesstoken").endpoint = _url
 
-            auth_response = AuthorizationResponse(code="access_code", state=res["state"])
-            resp = self.rph.finalize_auth(client, _session['iss'], auth_response.to_dict())
+            auth_response = AuthorizationResponse(code="access_code", state=_state)
+            resp = self.rph.finalize_auth(client, _session["iss"], auth_response.to_dict())
 
-            resp = self.rph.get_tokens(res["state"], client)
+            resp = self.rph.get_tokens(_state, client)
             assert set(resp.keys()) == {
                 "access_token",
                 "expires_in",
                 "id_token",
                 "token_type",
                 "__verified_id_token",
                 "__expires_at",
             }
 
-            _curr = client.get_context().cstate.get(res["state"])
-            assert set(_curr.keys()) == {'__expires_at',
-                                         '__verified_id_token',
-                                         'access_token',
-                                         'client_id',
-                                         'code',
-                                         'expires_in',
-                                         'id_token',
-                                         'iss',
-                                         'nonce',
-                                         'redirect_uri',
-                                         'response_type',
-                                         'scope',
-                                         'state',
-                                         'token_type'}
+            _curr = client.get_context().cstate.get(_state)
+            assert set(_curr.keys()) == {
+                "__expires_at",
+                "__verified_id_token",
+                "access_token",
+                "client_id",
+                "code",
+                "expires_in",
+                "id_token",
+                "iss",
+                "nonce",
+                "redirect_uri",
+                "response_type",
+                "scope",
+                "state",
+                "token_type",
+            }
 
     def test_access_and_id_token(self):
-        res = self.rph.begin(issuer_id="github")
-        _session = self.rph.get_session_information(res["state"])
-        client = self.rph.issuer2rp[_session['iss']]
+        url = self.rph.begin(issuer_id="github")
+        _state = get_state_from_url(url)
+        _session = self.rph.get_session_information(_state)
+        client = self.rph.issuer2rp[_session["iss"]]
         _context = client.get_context()
         _nonce = _session["nonce"]
-        _iss = _session['iss']
+        _iss = _session["iss"]
         _aud = _context.get_client_id()
-        idval = {"nonce": _nonce, "sub": "EndUserSubject", 'iss': _iss, "aud": _aud}
+        idval = {"nonce": _nonce, "sub": "EndUserSubject", "iss": _iss, "aud": _aud}
 
         _github_id = iss_id("github")
-        _keyjar = _context.upstream_get('attribute', 'keyjar')
+        _keyjar = _context.upstream_get("attribute", "keyjar")
         _keyjar.import_jwks(GITHUB_KEY.export_jwks(issuer_id=_github_id), _github_id)
 
         idts = IdToken(**idval)
         _signed_jwt = idts.to_jwt(
             key=GITHUB_KEY.get_signing_key("rsa", issuer_id=_github_id),
             algorithm="RS256",
             lifetime=300,
@@ -520,32 +541,33 @@
                 _url,
                 body=at.to_json(),
                 adding_headers={"Content-Type": "application/json"},
                 status=200,
             )
             client.get_service("accesstoken").endpoint = _url
 
-            _response = AuthorizationResponse(code="access_code", state=res["state"])
-            auth_response = self.rph.finalize_auth(client, _session['iss'], _response.to_dict())
+            _response = AuthorizationResponse(code="access_code", state=_state)
+            auth_response = self.rph.finalize_auth(client, _session["iss"], _response.to_dict())
             resp = self.rph.get_access_and_id_token(auth_response, client=client)
             assert resp["access_token"] == "accessTok"
             assert isinstance(resp["id_token"], IdToken)
 
     def test_access_and_id_token_by_reference(self):
-        res = self.rph.begin(issuer_id="github")
-        _session = self.rph.get_session_information(res["state"])
-        client = self.rph.issuer2rp[_session['iss']]
+        url = self.rph.begin(issuer_id="github")
+        _state = get_state_from_url(url)
+        _session = self.rph.get_session_information(_state)
+        client = self.rph.issuer2rp[_session["iss"]]
         _context = client.get_context()
         _nonce = _session["nonce"]
-        _iss = _session['iss']
+        _iss = _session["iss"]
         _aud = _context.get_client_id()
-        idval = {"nonce": _nonce, "sub": "EndUserSubject", 'iss': _iss, "aud": _aud}
+        idval = {"nonce": _nonce, "sub": "EndUserSubject", "iss": _iss, "aud": _aud}
 
         _github_id = iss_id("github")
-        _keyjar = _context.upstream_get('attribute', 'keyjar')
+        _keyjar = _context.upstream_get("attribute", "keyjar")
         _keyjar.import_jwks(GITHUB_KEY.export_jwks(issuer_id=_github_id), _github_id)
 
         idts = IdToken(**idval)
         _signed_jwt = idts.to_jwt(
             key=GITHUB_KEY.get_signing_key("rsa", issuer_id=_github_id),
             algorithm="RS256",
             lifetime=300,
@@ -566,32 +588,33 @@
                 _url,
                 body=at.to_json(),
                 adding_headers={"Content-Type": "application/json"},
                 status=200,
             )
             client.get_service("accesstoken").endpoint = _url
 
-            _response = AuthorizationResponse(code="access_code", state=res["state"])
-            _ = self.rph.finalize_auth(client, _session['iss'], _response.to_dict())
-            resp = self.rph.get_access_and_id_token(state=res["state"])
+            _response = AuthorizationResponse(code="access_code", state=_state)
+            _ = self.rph.finalize_auth(client, _session["iss"], _response.to_dict())
+            resp = self.rph.get_access_and_id_token(state=_state)
             assert resp["access_token"] == "accessTok"
             assert isinstance(resp["id_token"], IdToken)
 
     def test_get_user_info(self):
-        res = self.rph.begin(issuer_id="github")
-        _session = self.rph.get_session_information(res["state"])
-        client = self.rph.issuer2rp[_session['iss']]
+        url = self.rph.begin(issuer_id="github")
+        _state = get_state_from_url(url)
+        _session = self.rph.get_session_information(_state)
+        client = self.rph.issuer2rp[_session["iss"]]
         _context = client.get_context()
         _nonce = _session["nonce"]
-        _iss = _session['iss']
+        _iss = _session["iss"]
         _aud = _context.get_client_id()
-        idval = {"nonce": _nonce, "sub": "EndUserSubject", 'iss': _iss, "aud": _aud}
+        idval = {"nonce": _nonce, "sub": "EndUserSubject", "iss": _iss, "aud": _aud}
 
         _github_id = iss_id("github")
-        _keyjar = _context.upstream_get('attribute', 'keyjar')
+        _keyjar = _context.upstream_get("attribute", "keyjar")
         _keyjar.import_jwks(GITHUB_KEY.export_jwks(issuer_id=_github_id), _github_id)
 
         idts = IdToken(**idval)
         _signed_jwt = idts.to_jwt(
             key=GITHUB_KEY.get_signing_key("rsa", issuer_id=_github_id),
             algorithm="RS256",
             lifetime=300,
@@ -612,45 +635,46 @@
                 _url,
                 body=at.to_json(),
                 adding_headers={"Content-Type": "application/json"},
                 status=200,
             )
             client.get_service("accesstoken").endpoint = _url
 
-            _response = AuthorizationResponse(code="access_code", state=res["state"])
-            auth_response = self.rph.finalize_auth(client, _session['iss'], _response.to_dict())
+            _response = AuthorizationResponse(code="access_code", state=_state)
+            auth_response = self.rph.finalize_auth(client, _session["iss"], _response.to_dict())
 
             token_resp = self.rph.get_access_and_id_token(auth_response, client=client)
 
         _url = "https://github.com/user_info"
         with responses.RequestsMock() as rsps:
             rsps.add(
                 "GET",
                 _url,
                 body='{"sub":"EndUserSubject"}',
                 adding_headers={"Content-Type": "application/json"},
                 status=200,
             )
             client.get_service("userinfo").endpoint = _url
 
-            userinfo_resp = self.rph.get_user_info(res["state"], client, token_resp["access_token"])
+            userinfo_resp = self.rph.get_user_info(_state, client, token_resp["access_token"])
             assert userinfo_resp
 
     def test_userinfo_in_id_token(self):
-        res = self.rph.begin(issuer_id="github")
-        _session = self.rph.get_session_information(res["state"])
-        client = self.rph.issuer2rp[_session['iss']]
+        url = self.rph.begin(issuer_id="github")
+        _state = get_state_from_url(url)
+        _session = self.rph.get_session_information(_state)
+        client = self.rph.issuer2rp[_session["iss"]]
         _context = client.get_context()
         _nonce = _session["nonce"]
-        _iss = _session['iss']
+        _iss = _session["iss"]
         _aud = _context.get_client_id()
         idval = {
             "nonce": _nonce,
             "sub": "EndUserSubject",
-            'iss': _iss,
+            "iss": _iss,
             "aud": _aud,
             "given_name": "Diana",
             "family_name": "Krall",
             "occupation": "Jazz pianist",
         }
 
         idts = IdToken(**idval)
@@ -662,28 +686,30 @@
 def test_get_provider_specific_service():
     srv_desc = {"access_token": {"class": "idpyoidc.client.provider.github.AccessToken"}}
     entity = Entity(services=srv_desc, config={})
     assert entity.get_service("accesstoken").response_body_type == "urlencoded"
 
 
 class TestRPHandlerTier2(object):
+
     @pytest.fixture(autouse=True)
     def rphandler_setup(self):
         self.rph = RPHandler(BASE_URL, CLIENT_CONFIG, keyjar=CLI_KEY)
-        res = self.rph.begin(issuer_id="github")
-        _session = self.rph.get_session_information(res["state"])
-        client = self.rph.issuer2rp[_session['iss']]
+        url = self.rph.begin(issuer_id="github")
+        _state = get_state_from_url(url)
+        _session = self.rph.get_session_information(_state)
+        client = self.rph.issuer2rp[_session["iss"]]
         _context = client.get_context()
         _nonce = _session["nonce"]
-        _iss = _session['iss']
+        _iss = _session["iss"]
         _aud = _context.get_client_id()
-        idval = {"nonce": _nonce, "sub": "EndUserSubject", 'iss': _iss, "aud": _aud}
+        idval = {"nonce": _nonce, "sub": "EndUserSubject", "iss": _iss, "aud": _aud}
 
         _github_id = iss_id("github")
-        _keyjar = _context.upstream_get('attribute', 'keyjar')
+        _keyjar = _context.upstream_get("attribute", "keyjar")
         _keyjar.import_jwks(GITHUB_KEY.export_jwks(issuer_id=_github_id), _github_id)
 
         idts = IdToken(**idval)
         _signed_jwt = idts.to_jwt(
             key=GITHUB_KEY.get_signing_key("rsa", issuer_id=_github_id),
             algorithm="RS256",
             lifetime=300,
@@ -706,44 +732,44 @@
                 body=at.to_json(),
                 adding_headers={"Content-Type": "application/json"},
                 status=200,
             )
 
             client.get_service("accesstoken").endpoint = _url
 
-            _response = AuthorizationResponse(code="access_code", state=res["state"])
-            auth_response = self.rph.finalize_auth(client, _session['iss'], _response.to_dict())
+            _response = AuthorizationResponse(code="access_code", state=_state)
+            auth_response = self.rph.finalize_auth(client, _session["iss"], _response.to_dict())
 
             token_resp = self.rph.get_access_and_id_token(auth_response, client=client)
 
         _url = "https://github.com/token"
         with responses.RequestsMock() as rsps:
             rsps.add(
                 "GET",
                 _url,
                 body='{"sub":"EndUserSubject"}',
                 adding_headers={"Content-Type": "application/json"},
                 status=200,
             )
 
             client.get_service("userinfo").endpoint = _url
-            self.rph.get_user_info(res["state"], client, token_resp["access_token"])
-            self.state = res["state"]
+            self.rph.get_user_info(_state, client, token_resp["access_token"])
+            self.state = _state
 
     def test_init_authorization(self):
         _session = self.rph.get_session_information(self.state)
-        client = self.rph.issuer2rp[_session['iss']]
-        res = self.rph.init_authorization(client, req_args={"scope": ["openid", "email"]})
-        part = urlsplit(res["url"])
+        client = self.rph.issuer2rp[_session["iss"]]
+        _url = self.rph.init_authorization(client, req_args={"scope": ["openid", "email"]})
+        part = urlsplit(_url)
         _qp = parse_qs(part.query)
         assert _qp["scope"] == ["openid email"]
 
     def test_refresh_access_token(self):
         _session = self.rph.get_session_information(self.state)
-        client = self.rph.issuer2rp[_session['iss']]
+        client = self.rph.issuer2rp[_session["iss"]]
 
         _info = {"access_token": "2nd_accessTok", "token_type": "Bearer", "expires_in": 3600}
         at = AccessTokenResponse(**_info)
         _url = "https://github.com/token"
         with responses.RequestsMock() as rsps:
             rsps.add(
                 "POST",
@@ -755,15 +781,15 @@
 
             client.get_service("refresh_token").endpoint = _url
             res = self.rph.refresh_access_token(self.state, client, "openid email")
             assert res["access_token"] == "2nd_accessTok"
 
     def test_get_user_info(self):
         _session = self.rph.get_session_information(self.state)
-        client = self.rph.issuer2rp[_session['iss']]
+        client = self.rph.issuer2rp[_session["iss"]]
 
         _url = "https://github.com/userinfo"
         with responses.RequestsMock() as rsps:
             rsps.add(
                 "GET",
                 _url,
                 body='{"sub":"EndUserSubject", "mail":"foo@example.com"}',
@@ -782,21 +808,23 @@
     def test_get_valid_access_token(self):
         (token, expires_at) = self.rph.get_valid_access_token(self.state)
         assert token == "accessTok"
         assert expires_at > 0
 
 
 class MockResponse:
+
     def __init__(self, status_code, text, headers=None):
         self.status_code = status_code
         self.text = text
         self.headers = headers or {}
 
 
 class MockOP(object):
+
     def __init__(self, issuer, keyjar=None):
         self.keyjar = keyjar
         self.issuer = issuer
         self.state = ""
         self.nonce = ""
         self.get_response = {}
         self.register_get_response("default", "OK", 200)
@@ -837,15 +865,15 @@
 
             return _resp
 
 
 def construct_access_token_response(nonce, issuer, client_id, key_jar):
     _aud = client_id
 
-    idval = {"nonce": nonce, "sub": "EndUserSubject", 'iss': issuer, "aud": _aud}
+    idval = {"nonce": nonce, "sub": "EndUserSubject", "iss": issuer, "aud": _aud}
 
     idts = IdToken(**idval)
     _signed_jwt = idts.to_jwt(
         key=key_jar.get_signing_key("rsa", issuer_id=issuer), algorithm="RS256", lifetime=300
     )
 
     _info = {
@@ -864,53 +892,51 @@
     _req["client_id"] = "client1"
     _req["client_secret"] = "ClientSecretString"
     return json.dumps(_req)
 
 
 def test_rphandler_request_uri():
     rph = RPHandler(BASE_URL, CLIENT_CONFIG, keyjar=CLI_KEY)
-    res = rph.begin(issuer_id="github2", behaviour_args={"request_param": "request_uri"})
-    _session = rph.get_session_information(res["state"])
-    _url = res["url"]
+    _url = rph.begin(issuer_id="github2", behaviour_args={"request_param": "request_uri"})
     _qp = parse_qs(urlparse(_url).query)
     assert "request_uri" in _qp
 
 
 def test_rphandler_request():
     rph = RPHandler(BASE_URL, CLIENT_CONFIG, keyjar=CLI_KEY)
-    res = rph.begin(issuer_id="github2", behaviour_args={"request_param": "request"})
-    _session = rph.get_session_information(res["state"])
-    _url = res["url"]
+    _url = rph.begin(issuer_id="github2", behaviour_args={"request_param": "request"})
     _qp = parse_qs(urlparse(_url).query)
     assert "request" in _qp
 
 
 class TestRPHandlerWithMockOP(object):
+
     @pytest.fixture(autouse=True)
     def rphandler_setup(self):
         self.issuer = "https://github.com/login/oauth/authorize"
         # self.mock_op = MockOP(issuer=self.issuer)
         self.rph = RPHandler(BASE_URL, client_configs=CLIENT_CONFIG, keyjar=CLI_KEY)
 
     def test_finalize(self):
-        auth_query = self.rph.begin(issuer_id="github")
+        url = self.rph.begin(issuer_id="github")
+        _state = get_state_from_url(url)
         #  The authorization query is sent and after successful authentication
-        client = self.rph.get_client_from_session_key(state=auth_query["state"])
+        client = self.rph.get_client_from_session_key(state=_state)
         # register a response
         _url = CLIENT_CONFIG["github"]["provider_info"]["authorization_endpoint"]
         with responses.RequestsMock() as rsps:
             rsps.add(
                 "GET",
                 _url,
                 status=302,
             )
-            _ = client.httpc("GET", auth_query["url"])
+            _ = client.httpc("GET", url)
 
         #  the user is redirected back to the RP with a positive response
-        auth_response = AuthorizationResponse(code="access_code", state=auth_query["state"])
+        auth_response = AuthorizationResponse(code="access_code", state=_state)
 
         # need session information and the client instance
         _session = self.rph.get_session_information(auth_response["state"])
         client = self.rph.get_client_from_session_key(state=auth_response["state"])
 
         # Faking
         resp = construct_access_token_response(
@@ -922,15 +948,15 @@
 
         _token_url = CLIENT_CONFIG["github"]["provider_info"]["token_endpoint"]
         _user_url = CLIENT_CONFIG["github"]["provider_info"]["userinfo_endpoint"]
         _user_info = OpenIDSchema(
             sub="EndUserSubject", given_name="Diana", family_name="Krall", occupation="Jazz pianist"
         )
         _github_id = iss_id("github")
-        _keyjar = client.get_attribute('keyjar')
+        _keyjar = client.get_attribute("keyjar")
         _keyjar.import_jwks(GITHUB_KEY.export_jwks(issuer_id=_github_id), _github_id)
         with responses.RequestsMock() as rsps:
             rsps.add(
                 "POST",
                 _token_url,
                 body=resp.to_json(),
                 adding_headers={"Content-Type": "application/json"},
@@ -942,17 +968,18 @@
                 body=_user_info.to_json(),
                 adding_headers={"Content-Type": "application/json"},
                 status=200,
             )
 
             # do the rest (= get access token and user info)
             # assume code flow
-            resp = self.rph.finalize(_session['iss'], auth_response.to_dict())
+            resp = self.rph.finalize(_session["iss"], auth_response.to_dict())
 
-        assert set(resp.keys()) == {"userinfo", "state", "token", "id_token", "session_state"}
+        assert set(resp.keys()) == {'token', 'session_state', 'userinfo', 'state', 'issuer',
+                                    'id_token'}
 
     def test_dynamic_setup(self):
         user_id = "acct:foobar@example.com"
         _link = Link(
             rel="http://openid.net/specs/connect/1.0/issuer", href="https://server.example.com"
         )
         webfinger_response = JRD(subject=user_id, links=[_link])
@@ -979,24 +1006,32 @@
                 "A128CBC",
                 "A128KW",
                 "RSA1_5",
             ],
             "request_object_algs_supported": ["HS256", "RS256", "A128CBC", "A128KW", "RSA1_5"],
         }
         pcr = ProviderConfigurationResponse(**resp)
-        _crr = {"application_type": "web", "response_types": ["code", "code id_token"],
-                "redirect_uris": [
-                    "https://example.com/rp/authz_cb"
-                    "/7b7308fecf10c90b29303b6ae35ad1ef0f1914e49187f163335ae0b26a769e4f"],
-                "grant_types": ["authorization_code", "implicit"], "contacts": ["ops@example.com"],
-                "subject_type": "public", "id_token_signed_response_alg": "RS256",
-                "userinfo_signed_response_alg": "RS256", "request_object_signing_alg": "RS256",
-                "token_endpoint_auth_signing_alg": "RS256", "default_max_age": 86400,
-                "token_endpoint_auth_method": "client_secret_basic"}
-        _crr.update({'client_id':'abcdefghijkl', 'client_secret':rndstr(32)})
+        _crr = {
+            "application_type": "web",
+            "response_types": ["code", "code id_token"],
+            "redirect_uris": [
+                "https://example.com/rp/authz_cb"
+                "/7b7308fecf10c90b29303b6ae35ad1ef0f1914e49187f163335ae0b26a769e4f"
+            ],
+            "grant_types": ["authorization_code", "implicit"],
+            "contacts": ["ops@example.com"],
+            "subject_type": "public",
+            "id_token_signed_response_alg": "RS256",
+            "userinfo_signed_response_alg": "RS256",
+            "request_object_signing_alg": "RS256",
+            "token_endpoint_auth_signing_alg": "RS256",
+            "default_max_age": 86400,
+            "token_endpoint_auth_method": "client_secret_basic",
+        }
+        _crr.update({"client_id": "abcdefghijkl", "client_secret": rndstr(32)})
         cli_reg_resp = RegistrationResponse(**_crr)
         with responses.RequestsMock() as rsps:
             rsps.add(
                 "GET",
                 "https://example.com/.well-known/webfinger",
                 body=webfinger_response.to_json(),
                 adding_headers={"Content-Type": "application/json"},
```

### Comparing `idpyoidc-2.0.0/tests/test_client_29_pushed_auth.py` & `idpyoidc-2.1.0/tests/test_client_29_pushed_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         config = {
             "client_id": "client_id",
             "client_secret": "a longesh password",
             "redirect_uris": ["https://example.com/cli/authz_cb"],
             "preference": {"response_types": ["code"]},
             "add_ons": {
                 "pushed_authorization": {
-                    "function": "idpyoidc.client.oauth2.add_on.pushed_authorization.add_support",
+                    "function": "idpyoidc.client.oauth2.add_on.par.add_support",
                     "kwargs": {
                         "body_format": "jws",
                         "signing_algorithm": "RS256",
                         "http_client": None,
                         "merge_rule": "lax",
                     },
                 }
```

### Comparing `idpyoidc-2.0.0/tests/test_client_30_rph_defaults.py` & `idpyoidc-2.1.0/tests/test_client_30_rph_defaults.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,18 +45,18 @@
             'redirect_uris',
             'request_object_encryption_alg_values_supported',
             'request_object_encryption_enc_values_supported',
             'scopes_supported',
             'userinfo_encryption_alg_values_supported',
             'userinfo_encryption_enc_values_supported'}
 
-        _keyjar = client.get_attribute('keyjar')
+        _keyjar = client.get_attribute("keyjar")
         assert list(_keyjar.owners()) == ["", BASE_URL]
         keys = _keyjar.get_issuer_keys("")
-        assert len(keys) == 2
+        assert len(keys) == 4
 
         assert _context.base_url == BASE_URL
 
     def test_begin(self):
         ISS_ID = "https://op.example.org"
         OP_KEYS = build_keyjar(DEFAULT_KEY_DEFS)
         # The 4 steps of client_setup
@@ -92,44 +92,42 @@
                 client_id="client uno", client_secret="VerySecretAndLongEnough", **_req.to_dict()
             ).to_json()
             rsps.add("POST", request_uri, body=_jws, status=200)
             self.rph.do_client_registration(client, ISS_ID)
 
         self.rph.issuer2rp[issuer] = client
 
-        assert set(_context.claims.use.keys()) == {'application_type',
-                                                   'callback_uris',
-                                                   'client_id',
-                                                   'client_secret',
-                                                   'default_max_age',
-                                                   'encrypt_request_object_supported',
-                                                   'encrypt_userinfo_supported',
-                                                   'grant_types',
-                                                   'id_token_signed_response_alg',
-                                                   'jwks_uri',
-                                                   'redirect_uris',
-                                                   'request_object_signing_alg',
-                                                   'response_modes_supported',
-                                                   'response_types',
-                                                   'scope',
-                                                   'subject_type',
-                                                   'token_endpoint_auth_method',
-                                                   'token_endpoint_auth_signing_alg',
-                                                   'userinfo_signed_response_alg'}
+        assert set(_context.claims.use.keys()) == {
+            "application_type",
+            "callback_uris",
+            "client_id",
+            "client_secret",
+            "default_max_age",
+            "encrypt_request_object_supported",
+            "grant_types",
+            "id_token_signed_response_alg",
+            "jwks_uri",
+            "redirect_uris",
+            "request_object_signing_alg",
+            "response_modes",
+            "response_types",
+            "scope",
+            "subject_type",
+            "token_endpoint_auth_method",
+            "token_endpoint_auth_signing_alg",
+        }
         assert _context.get_client_id() == "client uno"
         assert _context.get_usage("client_secret") == "VerySecretAndLongEnough"
         assert _context.get("issuer") == ISS_ID
 
-        res = self.rph.init_authorization(client)
-        assert set(res.keys()) == {"url", "state"}
-        p = urlparse(res["url"])
+        url = self.rph.init_authorization(client)
+        p = urlparse(url)
         assert p.hostname == "op.example.org"
         assert p.path == "/authorization"
         qs = parse_qs(p.query)
-        assert qs["state"] == [res["state"]]
         # PKCE stuff
         assert "code_challenge" in qs
         assert qs["code_challenge_method"] == ["S256"]
 
     def test_begin_2(self):
         ISS_ID = "https://op.example.org"
         OP_KEYS = build_keyjar(DEFAULT_KEY_DEFS)
```

### Comparing `idpyoidc-2.0.0/tests/test_client_31_oauth2_persistent.py` & `idpyoidc-2.1.0/tests/test_client_31_oauth2_persistent.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,17 +107,15 @@
         client_2.get_context().cstate.update(_state, token_response)
 
         # Next up is Client 1
         _state_dump = client_2.get_context().dump()
         client_1.get_context().load(_state_dump)
 
         req_args = {}
-        msg = client_1.get_service("refresh_token").construct(
-            request_args=req_args, state=_state
-        )
+        msg = client_1.get_service("refresh_token").construct(request_args=req_args, state=_state)
         assert isinstance(msg, RefreshAccessTokenRequest)
         assert msg.to_dict() == {
             "client_id": "client_1",
             "client_secret": "abcdefghijklmnop",
             "grant_type": "refresh_token",
             "refresh_token": "refresh_with_me",
         }
```

### Comparing `idpyoidc-2.0.0/tests/test_client_32_oidc_persistent.py` & `idpyoidc-2.1.0/tests/test_client_32_oidc_persistent.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,17 +63,15 @@
         client_2.get_context().load(_state_dump)
 
         auth_response = AuthorizationResponse(code="access_code")
         client_2.get_context().cstate.update(_state, auth_response)
 
         # Bind access code to state
         req_args = {}
-        msg = client_2.get_service("accesstoken").construct(
-            request_args=req_args, state=_state
-        )
+        msg = client_2.get_service("accesstoken").construct(request_args=req_args, state=_state)
         assert isinstance(msg, AccessTokenRequest)
         assert msg.to_dict() == {
             "client_id": "client_1",
             "code": "access_code",
             "client_secret": "abcdefghijklmnop",
             "grant_type": "authorization_code",
             "redirect_uri": "https://example.com/cli/authz_cb",
@@ -85,35 +83,33 @@
         client_1 = RP(config=CONF)
         _state = client_1.get_context().cstate.create_state(iss=ISSUER)
 
         auth_request = AuthorizationRequest(
             redirect_uri="https://example.com/cli/authz_cb", state=_state
         )
 
-        client_1.get_context().cstate.update(_state,auth_request)
+        client_1.get_context().cstate.update(_state, auth_request)
 
         # Client 2 carries on
         client_2 = RP(config=CONF)
         _state_dump = client_1.get_context().dump()
         client_2.get_context().load(_state_dump)
 
         auth_response = AuthorizationResponse(code="access_code")
         client_2.get_context().cstate.update(_state, auth_response)
 
         token_response = AccessTokenResponse(refresh_token="refresh_with_me", access_token="access")
-        client_2.get_context().cstate.update(_state,token_response )
+        client_2.get_context().cstate.update(_state, token_response)
 
         # Back to Client 1
         _state_dump = client_2.get_context().dump()
         client_1.get_context().load(_state_dump)
 
         req_args = {}
-        msg = client_1.get_service("refresh_token").construct(
-            request_args=req_args, state=_state
-        )
+        msg = client_1.get_service("refresh_token").construct(request_args=req_args, state=_state)
         assert isinstance(msg, RefreshAccessTokenRequest)
         assert msg.to_dict() == {
             "client_id": "client_1",
             "client_secret": "abcdefghijklmnop",
             "grant_type": "refresh_token",
             "refresh_token": "refresh_with_me",
         }
@@ -129,18 +125,18 @@
 
         # Client 2 carries on
         client_2 = RP(config=CONF)
         _state_dump = client_1.get_context().dump()
         client_2.get_context().load(_state_dump)
 
         auth_response = AuthorizationResponse(code="access_code")
-        client_2.get_context().cstate.update(_state,auth_response)
+        client_2.get_context().cstate.update(_state, auth_response)
 
         token_response = AccessTokenResponse(refresh_token="refresh_with_me", access_token="access")
-        client_2.get_context().cstate.update(_state,token_response)
+        client_2.get_context().cstate.update(_state, token_response)
 
         # Back to Client 1
         _state_dump = client_2.get_context().dump()
         client_1.get_context().load(_state_dump)
 
         _srv = client_1.get_service("userinfo")
         _srv.endpoint = "https://example.com/userinfo"
```

### Comparing `idpyoidc-2.0.0/tests/test_client_40_dpop.py` & `idpyoidc-2.1.0/tests/test_client_40_dpop.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,17 +83,15 @@
                     "function": "idpyoidc.client.oauth2.add_on.dpop.add_support",
                     "kwargs": {"dpop_signing_alg_values_supported": ["ES256", "ES512"]},
                 }
             },
         }
 
         services = {
-            "discovery": {
-                "class": "idpyoidc.client.oauth2.server_metadata.ServerMetadata"
-            },
+            "discovery": {"class": "idpyoidc.client.oauth2.server_metadata.ServerMetadata"},
             "authorization": {"class": "idpyoidc.client.oauth2.authorization.Authorization"},
             "access_token": {"class": "idpyoidc.client.oauth2.access_token.AccessToken"},
             "refresh_access_token": {
                 "class": "idpyoidc.client.oauth2.refresh_access_token.RefreshAccessToken"
             },
             "userinfo": {"class": "idpyoidc.client.oidc.userinfo.UserInfo"},
         }
```

### Comparing `idpyoidc-2.0.0/tests/test_client_41_rp_handler_persistent.py` & `idpyoidc-2.1.0/tests/test_client_41_rp_handler_persistent.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from urllib.parse import parse_qs
 from urllib.parse import urlsplit
 
-from cryptojwt.key_jar import init_key_jar
 import responses
+from cryptojwt.key_jar import init_key_jar
 
 from idpyoidc.client.rp_handler import RPHandler
 from idpyoidc.message.oidc import AccessTokenResponse
 from idpyoidc.message.oidc import AuthorizationResponse
 from idpyoidc.message.oidc import IdToken
 
 BASE_URL = "https://example.com/rp"
@@ -47,15 +47,15 @@
         },
     },
     "linkedin": {
         "issuer": "https://www.linkedin.com/oauth/v2/",
         "client_id": "xxxxxxx",
         "client_secret": "yyyyyyyyyyyyyyyyyyyy",
         "redirect_uris": ["{}/authz_cb/linkedin".format(BASE_URL)],
-        'client_type': 'oauth2',
+        "client_type": "oauth2",
         "preference": {
             "response_types": ["code"],
             "scope": ["r_basicprofile", "r_emailaddress"],
             "token_endpoint_auth_methods_supported": ["client_secret_post"],
         },
         "provider_info": {
             "authorization_endpoint": "https://www.linkedin.com/oauth/v2/authorization",
@@ -164,15 +164,22 @@
 )
 
 
 def iss_id(iss):
     return CLIENT_CONFIG[iss]["issuer"]
 
 
+def get_state_from_url(url):
+    p = urlsplit(url)
+    qp = parse_qs(p.query)
+    return qp["state"][0]
+
+
 class TestRPHandler(object):
+
     def test_pick_config(self):
         rph_1 = RPHandler(
             BASE_URL, client_configs=CLIENT_CONFIG, keyjar=CLI_KEY, module_dirs=["oidc"]
         )
         cnf = rph_1.pick_config("facebook")
         assert cnf["issuer"] == "https://www.facebook.com/v2.11/dialog/oauth"
 
@@ -237,42 +244,39 @@
         _github_id = iss_id("github")
         _context = client.get_context()
 
         assert _context.get_client_id() == "eeeeeeeee"
         assert _context.get_usage("client_secret") == "aaaaaaaaaaaaaaaaaaaa"
         assert _context.get("issuer") == _github_id
 
-        _keyjar = _context.upstream_get('attribute', 'keyjar')
+        _keyjar = _context.upstream_get("attribute", "keyjar")
         _keyjar.import_jwks(GITHUB_KEY.export_jwks(issuer_id=_github_id), _github_id)
 
-        assert set(_keyjar.owners()) == {"", 'eeeeeeeee', _github_id}
+        assert set(_keyjar.owners()) == {"", "eeeeeeeee", _github_id}
         keys = _keyjar.get_issuer_keys("")
         assert len(keys) == 3  # one symmetric, one RSA and one EC
 
         for service_type in ["authorization", "accesstoken", "userinfo"]:
             _srv = client.get_service(service_type)
             _endp = client.get_context().get("provider_info")[_srv.endpoint_name]
             assert _srv.endpoint == _endp
 
-        assert rph_1.hash2issuer["github"] == _context.get("issuer")
-
     def test_begin(self):
         rph_1 = RPHandler(
             BASE_URL, client_configs=CLIENT_CONFIG, keyjar=CLI_KEY, module_dirs=["oidc"]
         )
 
-        res = rph_1.begin(issuer_id="github")
-        assert set(res.keys()) == {"url", "state"}
+        url = rph_1.begin(issuer_id="github")
         _github_id = iss_id("github")
 
         client = rph_1.issuer2rp[_github_id]
 
         assert client.get_context().get("issuer") == _github_id
 
-        part = urlsplit(res["url"])
+        part = urlsplit(url)
         assert part.scheme == "https"
         assert part.netloc == "github.com"
         assert part.path == "/login/oauth/authorize"
         query = parse_qs(part.query)
 
         assert set(query.keys()) == {
             "nonce",
@@ -290,82 +294,92 @@
         assert query["scope"] == ["user public_repo openid"]
 
     def test_get_session_information(self):
         rph_1 = RPHandler(
             BASE_URL, client_configs=CLIENT_CONFIG, keyjar=CLI_KEY, module_dirs=["oidc"]
         )
 
-        res = rph_1.begin(issuer_id="github")
-        _session = rph_1.get_session_information(res["state"])
+        url = rph_1.begin(issuer_id="github")
+        _session = rph_1.get_session_information(get_state_from_url(url))
         assert rph_1.client_configs["github"]["issuer"] == _session["iss"]
 
     def test_get_client_from_session_key(self):
         rph_1 = RPHandler(
             BASE_URL, client_configs=CLIENT_CONFIG, keyjar=CLI_KEY, module_dirs=["oidc"]
         )
 
-        res = rph_1.begin(issuer_id="linkedin")
-        cli1 = rph_1.get_client_from_session_key(state=res["state"])
-        _session = rph_1.get_session_information(res["state"])
+        url = rph_1.begin(issuer_id="linkedin")
+        _state = get_state_from_url(url)
+        cli1 = rph_1.get_client_from_session_key(state=_state)
+        _session = rph_1.get_session_information(_state)
         cli2 = rph_1.issuer2rp[_session["iss"]]
         assert cli1 == cli2
         # redo
-        rph_1.do_provider_info(state=res["state"])
+        rph_1.do_provider_info(state=_state)
         # get new redirect_uris
         cli2.get_context().set_usage("redirect_uris", [])
-        rph_1.do_client_registration(state=res["state"])
+        rph_1.do_client_registration(state=_state)
 
     def test_finalize_auth(self):
         rph_1 = RPHandler(
             BASE_URL, client_configs=CLIENT_CONFIG, keyjar=CLI_KEY, module_dirs=["oidc"]
         )
 
-        res = rph_1.begin(issuer_id="linkedin")
-        _session = rph_1.get_session_information(res["state"])
+        url = rph_1.begin(issuer_id="linkedin")
+        _state = get_state_from_url(url)
+        _session = rph_1.get_session_information(_state)
         client = rph_1.issuer2rp[_session["iss"]]
 
-        auth_response = AuthorizationResponse(code="access_code", state=res["state"])
+        auth_response = AuthorizationResponse(code="access_code", state=_state)
         resp = rph_1.finalize_auth(client, _session["iss"], auth_response.to_dict())
         assert set(resp.keys()) == {"state", "code"}
-        aresp = (
-            client.get_service("authorization").upstream_get("context").cstate.get(res["state"])
-        )
+        aresp = client.get_service("authorization").upstream_get("context").cstate.get(_state)
         assert set(aresp.keys()) == {
-            "state", "code", 'iss', 'client_id',
-            'scope', 'nonce', 'response_type', 'redirect_uri'}
+            "state",
+            "code",
+            "iss",
+            "client_id",
+            "scope",
+            "nonce",
+            "response_type",
+            "redirect_uri",
+        }
 
     def test_get_client_authn_method(self):
         rph_1 = RPHandler(
             BASE_URL, client_configs=CLIENT_CONFIG, keyjar=CLI_KEY, module_dirs=["oidc"]
         )
 
-        res = rph_1.begin(issuer_id="github")
-        _session = rph_1.get_session_information(res["state"])
+        url = rph_1.begin(issuer_id="github")
+        _state = get_state_from_url(url)
+        _session = rph_1.get_session_information(_state)
         client = rph_1.issuer2rp[_session["iss"]]
         authn_method = rph_1.get_client_authn_method(client, "token_endpoint")
         assert authn_method == ""
 
-        res = rph_1.begin(issuer_id="linkedin")
-        _session = rph_1.get_session_information(res["state"])
+        url = rph_1.begin(issuer_id="linkedin")
+        _state = get_state_from_url(url)
+        _session = rph_1.get_session_information(_state)
         client = rph_1.issuer2rp[_session["iss"]]
         authn_method = rph_1.get_client_authn_method(client, "token_endpoint")
         assert authn_method == "client_secret_post"
 
     def test_get_tokens(self):
         rph_1 = RPHandler(
             BASE_URL, client_configs=CLIENT_CONFIG, keyjar=CLI_KEY, module_dirs=["oidc"]
         )
 
-        res = rph_1.begin(issuer_id="github")
-        _session = rph_1.get_session_information(res["state"])
+        url = rph_1.begin(issuer_id="github")
+        _state = get_state_from_url(url)
+        _session = rph_1.get_session_information(_state)
         client = rph_1.issuer2rp[_session["iss"]]
 
         _github_id = iss_id("github")
         _context = client.get_context()
-        _keyjar = _context.upstream_get('attribute', 'keyjar')
+        _keyjar = _context.upstream_get("attribute", "keyjar")
         _keyjar.import_jwks(GITHUB_KEY.export_jwks(issuer_id=_github_id), _github_id)
 
         _nonce = _session["nonce"]
         _iss = _session["iss"]
         _aud = _context.get_client_id()
         idval = {"nonce": _nonce, "sub": "EndUserSubject", "iss": _iss, "aud": _aud}
 
@@ -389,65 +403,66 @@
                 _url,
                 body=at.to_json(),
                 adding_headers={"Content-Type": "application/json"},
                 status=200,
             )
             client.get_service("accesstoken").endpoint = _url
 
-            auth_response = AuthorizationResponse(code="access_code", state=res["state"])
+            auth_response = AuthorizationResponse(code="access_code", state=_state)
             resp = rph_1.finalize_auth(client, _session["iss"], auth_response.to_dict())
 
-            resp = rph_1.get_tokens(res["state"], client)
+            resp = rph_1.get_tokens(_state, client)
             assert set(resp.keys()) == {
                 "access_token",
                 "expires_in",
                 "id_token",
                 "token_type",
                 "__verified_id_token",
                 "__expires_at",
             }
 
             atresp = (
                 client.get_service("accesstoken")
                 .upstream_get("service_context")
-                .cstate.get(res["state"])
+                .cstate.get(_state)
             )
             assert set(atresp.keys()) == {
                 "__expires_at",
                 "__verified_id_token",
                 "access_token",
-                'client_id',
-                'code',
+                "client_id",
+                "code",
                 "expires_in",
                 "id_token",
-                'iss',
-                'nonce',
-                'redirect_uri',
-                'response_type',
-                'scope',
-                'state',
-                "token_type"
+                "iss",
+                "nonce",
+                "redirect_uri",
+                "response_type",
+                "scope",
+                "state",
+                "token_type",
             }
 
     def test_access_and_id_token(self):
         rph_1 = RPHandler(
             BASE_URL, client_configs=CLIENT_CONFIG, keyjar=CLI_KEY, module_dirs=["oidc"]
         )
 
-        res = rph_1.begin(issuer_id="github")
-        _session = rph_1.get_session_information(res["state"])
+        url = rph_1.begin(issuer_id="github")
+        _state = get_state_from_url(url)
+        _session = rph_1.get_session_information(_state)
         client = rph_1.issuer2rp[_session["iss"]]
         _context = client.get_context()
         _nonce = _session["nonce"]
         _iss = _session["iss"]
         _aud = _context.get_client_id()
         idval = {"nonce": _nonce, "sub": "EndUserSubject", "iss": _iss, "aud": _aud}
 
         _github_id = iss_id("github")
-        _keyjar = _context.upstream_get('attribute', 'keyjar')
+        _keyjar = _context.upstream_get("attribute", "keyjar")
         _keyjar.import_jwks(GITHUB_KEY.export_jwks(issuer_id=_github_id), _github_id)
 
         idts = IdToken(**idval)
         _signed_jwt = idts.to_jwt(
             key=GITHUB_KEY.get_signing_key("rsa", issuer_id=_github_id),
             algorithm="RS256",
             lifetime=300,
@@ -468,36 +483,37 @@
                 _url,
                 body=at.to_json(),
                 adding_headers={"Content-Type": "application/json"},
                 status=200,
             )
             client.get_service("accesstoken").endpoint = _url
 
-            _response = AuthorizationResponse(code="access_code", state=res["state"])
+            _response = AuthorizationResponse(code="access_code", state=_state)
             auth_response = rph_1.finalize_auth(client, _session["iss"], _response.to_dict())
             resp = rph_1.get_access_and_id_token(auth_response, client=client)
             assert resp["access_token"] == "accessTok"
             assert isinstance(resp["id_token"], IdToken)
 
     def test_access_and_id_token_by_reference(self):
         rph_1 = RPHandler(
             BASE_URL, client_configs=CLIENT_CONFIG, keyjar=CLI_KEY, module_dirs=["oidc"]
         )
 
-        res = rph_1.begin(issuer_id="github")
-        _session = rph_1.get_session_information(res["state"])
+        url = rph_1.begin(issuer_id="github")
+        _state = get_state_from_url(url)
+        _session = rph_1.get_session_information(_state)
         client = rph_1.issuer2rp[_session["iss"]]
         _context = client.get_context()
         _nonce = _session["nonce"]
         _iss = _session["iss"]
         _aud = _context.get_client_id()
         idval = {"nonce": _nonce, "sub": "EndUserSubject", "iss": _iss, "aud": _aud}
 
         _github_id = iss_id("github")
-        _keyjar = _context.upstream_get('attribute', 'keyjar')
+        _keyjar = _context.upstream_get("attribute", "keyjar")
         _keyjar.import_jwks(GITHUB_KEY.export_jwks(issuer_id=_github_id), _github_id)
 
         idts = IdToken(**idval)
         _signed_jwt = idts.to_jwt(
             key=GITHUB_KEY.get_signing_key("rsa", issuer_id=_github_id),
             algorithm="RS256",
             lifetime=300,
@@ -518,36 +534,37 @@
                 _url,
                 body=at.to_json(),
                 adding_headers={"Content-Type": "application/json"},
                 status=200,
             )
             client.get_service("accesstoken").endpoint = _url
 
-            _response = AuthorizationResponse(code="access_code", state=res["state"])
+            _response = AuthorizationResponse(code="access_code", state=_state)
             _ = rph_1.finalize_auth(client, _session["iss"], _response.to_dict())
-            resp = rph_1.get_access_and_id_token(state=res["state"])
+            resp = rph_1.get_access_and_id_token(state=_state)
             assert resp["access_token"] == "accessTok"
             assert isinstance(resp["id_token"], IdToken)
 
     def test_get_user_info(self):
         rph_1 = RPHandler(
             BASE_URL, client_configs=CLIENT_CONFIG, keyjar=CLI_KEY, module_dirs=["oidc"]
         )
 
-        res = rph_1.begin(issuer_id="github")
-        _session = rph_1.get_session_information(res["state"])
+        url = rph_1.begin(issuer_id="github")
+        _state = get_state_from_url(url)
+        _session = rph_1.get_session_information(_state)
         client = rph_1.issuer2rp[_session["iss"]]
         _context = client.get_context()
         _nonce = _session["nonce"]
         _iss = _session["iss"]
         _aud = _context.get_client_id()
         idval = {"nonce": _nonce, "sub": "EndUserSubject", "iss": _iss, "aud": _aud}
 
         _github_id = iss_id("github")
-        _keyjar = _context.upstream_get('attribute', 'keyjar')
+        _keyjar = _context.upstream_get("attribute", "keyjar")
         _keyjar.import_jwks(GITHUB_KEY.export_jwks(issuer_id=_github_id), _github_id)
 
         idts = IdToken(**idval)
         _signed_jwt = idts.to_jwt(
             key=GITHUB_KEY.get_signing_key("rsa", issuer_id=_github_id),
             algorithm="RS256",
             lifetime=300,
@@ -568,15 +585,15 @@
                 _url,
                 body=at.to_json(),
                 adding_headers={"Content-Type": "application/json"},
                 status=200,
             )
             client.get_service("accesstoken").endpoint = _url
 
-            _response = AuthorizationResponse(code="access_code", state=res["state"])
+            _response = AuthorizationResponse(code="access_code", state=_state)
             auth_response = rph_1.finalize_auth(client, _session["iss"], _response.to_dict())
 
             token_resp = rph_1.get_access_and_id_token(auth_response, client=client)
 
         _url = "https://github.com/user_info"
         with responses.RequestsMock() as rsps:
             rsps.add(
@@ -584,24 +601,25 @@
                 _url,
                 body='{"sub":"EndUserSubject"}',
                 adding_headers={"Content-Type": "application/json"},
                 status=200,
             )
             client.get_service("userinfo").endpoint = _url
 
-            userinfo_resp = rph_1.get_user_info(res["state"], client, token_resp["access_token"])
+            userinfo_resp = rph_1.get_user_info(_state, client, token_resp["access_token"])
             assert userinfo_resp
 
     def test_userinfo_in_id_token(self):
         rph_1 = RPHandler(
             BASE_URL, client_configs=CLIENT_CONFIG, keyjar=CLI_KEY, module_dirs=["oidc"]
         )
 
-        res = rph_1.begin(issuer_id="github")
-        _session = rph_1.get_session_information(res["state"])
+        url = rph_1.begin(issuer_id="github")
+        _state = get_state_from_url(url)
+        _session = rph_1.get_session_information(_state)
         client = rph_1.issuer2rp[_session["iss"]]
         # _context = client.client_get("service_context")
         _nonce = _session["nonce"]
         _iss = _session["iss"]
         _aud = client.get_client_id()
         idval = {
             "nonce": _nonce,
```

### Comparing `idpyoidc-2.0.0/tests/test_client_50_ciba.py` & `idpyoidc-2.1.0/tests/test_client_50_ciba.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_client_51_identity_assurance.py` & `idpyoidc-2.1.0/tests/test_client_51_identity_assurance.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             "sub": "e8148603-8934-4245-825b-c108b8b6b945",
             "verified_claims": {
                 "verification": {"trust_framework": "ial_example_gold"},
                 "claims": {"given_name": "Max", "family_name": "Meier", "birthdate": "1956-01-28"},
             },
         }
 
-        _jwt = JWT(key_jar=self.service.upstream_get("attribute",'keyjar'))
+        _jwt = JWT(key_jar=self.service.upstream_get("attribute", "keyjar"))
         _jws = _jwt.pack(payload=_distributed_respone)
 
         resp = {
             "iss": "https://server.example.com",
             "sub": "248289761001",
             "email": "janedoe@example.com",
             "email_verified": True,
```

### Comparing `idpyoidc-2.0.0/tests/test_client_55_token_exchange.py` & `idpyoidc-2.1.0/tests/test_client_55_token_exchange.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,43 +48,39 @@
             "client_id": "client_id",
             "client_secret": "a longesh password",
             "redirect_uris": ["https://example.com/cli/authz_cb"],
             "issuer": self._iss,
             "requests_dir": "requests",
             "base_url": "https://example.com/cli/",
         }
-        entity = Entity(keyjar=make_keyjar(), config=client_config,
-                        services={
-                            "discovery": {
-                                "class":
-                                    "idpyoidc.client.oauth2.server_metadata.ServerMetadata"},
-                            "authorization": {
-                                "class": "idpyoidc.client.oauth2.authorization.Authorization"},
-                            "access_token": {
-                                "class": "idpyoidc.client.oauth2.access_token.AccessToken"},
-                            "token_exchange": {
-                                "class":
-                                    "idpyoidc.client.oauth2.token_exchange.TokenExchange"
-                            },
-                        }
-                        )
+        entity = Entity(
+            keyjar=make_keyjar(),
+            config=client_config,
+            services={
+                "discovery": {"class": "idpyoidc.client.oauth2.server_metadata.ServerMetadata"},
+                "authorization": {"class": "idpyoidc.client.oauth2.authorization.Authorization"},
+                "access_token": {"class": "idpyoidc.client.oauth2.access_token.AccessToken"},
+                "token_exchange": {"class": "idpyoidc.client.oauth2.token_exchange.TokenExchange"},
+            },
+        )
         entity.get_context().issuer = "https://example.com"
         self.service = entity.get_service("token_exchange")
         _cstate = self.service.upstream_get("context").cstate
         # Add history
         auth_response = AuthorizationResponse(code="access_code")
         _cstate.update("abcde", auth_response)
 
         idtval = {"nonce": "KUEYfRM2VzKDaaKD", "sub": "diana", "iss": ISS, "aud": "client_id"}
         idt = create_jws(idtval)
 
         ver_idt = IdToken().from_jwt(idt, make_keyjar())
 
-        token_response = AccessTokenResponse(access_token="access_token", id_token=idt,
-                                             __verified_id_token=ver_idt)
+        token_response = AccessTokenResponse(
+            access_token="access_token", id_token=idt, __verified_id_token=ver_idt
+        )
         _cstate.update("abcde", token_response)
 
     def test_construct(self):
         _req = self.service.construct(state="abcde")
         assert isinstance(_req, Message)
         assert len(_req) == 2
         assert "subject_token" in _req
```

### Comparing `idpyoidc-2.0.0/tests/test_server_00_configure.py` & `idpyoidc-2.1.0/tests/test_server_00_configure.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_server_00a_client_configure.py` & `idpyoidc-2.1.0/tests/test_server_00a_client_configure.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_server_01_claims.py` & `idpyoidc-2.1.0/tests/test_server_01_claims.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,18 +135,19 @@
             "redirect_uris": [("https://example.com/cb", None)],
             "client_salt": "salted",
             "token_endpoint_auth_method": "client_secret_post",
             "response_types": ["code", "token", "code id_token", "id_token"],
             "add_claims": {
                 "always": {},
             },
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"]
+            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"],
         }
-        self.server.get_attribute('keyjar').add_symmetric("client_1", "hemligtochintekort",
-                                                          ["sig", "enc"])
+        self.server.get_attribute("keyjar").add_symmetric(
+            "client_1", "hemligtochintekort", ["sig", "enc"]
+        )
         self.claims_interface = self.context.claims_interface
 
         self.user_id = USER_ID
 
     def _create_session(self, auth_req, sub_type="public", sector_identifier=""):
         if sector_identifier:
             authz_req = auth_req.copy()
```

### Comparing `idpyoidc-2.0.0/tests/test_server_01_construct.py` & `idpyoidc-2.1.0/tests/test_server_01_construct.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_server_02_session_token.py` & `idpyoidc-2.1.0/tests/test_server_02_session_token.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_server_03_authz_handling.py` & `idpyoidc-2.1.0/tests/test_server_03_authz_handling.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,17 +128,17 @@
         server = Server(conf)
         server.context.cdb["client_1"] = {
             "client_secret": "hemligtochintekort",
             "redirect_uris": [("https://example.com/cb", None)],
             "client_salt": "salted",
             "token_endpoint_auth_method": "client_secret_post",
             "response_types": ["code", "token", "code id_token", "id_token"],
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"]
+            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"],
         }
-        server.get_attribute('keyjar').add_symmetric(
+        server.get_attribute("keyjar").add_symmetric(
             "client_1", "hemligtochintekort", ["sig", "enc"]
         )
         server.endpoint = do_endpoints(conf, server.upstream_get)
         self.session_manager = server.context.session_manager
         self.user_id = USER_ID
         self.server = server
         self.authz = server.context.authz
```

### Comparing `idpyoidc-2.0.0/tests/test_server_04_session_info.py` & `idpyoidc-2.1.0/tests/test_server_04_session_info.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_server_05_token_handler.py` & `idpyoidc-2.1.0/tests/test_server_05_token_handler.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_server_06_grant.py` & `idpyoidc-2.1.0/tests/test_server_06_grant.py`

 * *Files 0% similar despite different names*

```diff
@@ -435,15 +435,15 @@
         grant.scope = ["openid", "email", "address"]
         grant.claims = {"userinfo": {"given_name": None, "email": None}}
         grant.resources = ["https://api.example.com"]
 
         # Default usage rules
         self.context.cdb["client_id"] = {}
         rules = get_usage_rules("access_token", self.context, grant, "client_id")
-        assert rules == {"supports_minting": [], "expires_in": 3600}
+        assert rules == {"expires_in": 3600}
 
         # client specific usage rules
         self.context.cdb["client_id"] = {"access_token": {"expires_in": 600}}
 
     def test_assigned_scope(self):
         session_id = self._create_session(AREQ)
         session_info = self.context.session_manager.get_session_info(
```

### Comparing `idpyoidc-2.0.0/tests/test_server_07_sess_mngm_db.py` & `idpyoidc-2.1.0/tests/test_server_07_sess_mngm_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,21 +21,25 @@
     response_type="code",
 )
 
 
 class TestDB:
     @pytest.fixture(autouse=True)
     def setup_environment(self):
-        self.db = Database(crypt_config=CRYPT_CONFIG,
-                           session_params={"node_type": ["user", "client", "grant"],
-                                           "node_info_class": {
-                                               "user": UserSessionInfo,
-                                               "client": ClientSessionInfo,
-                                               "grant": Grant}
-                                           })
+        self.db = Database(
+            crypt_config=CRYPT_CONFIG,
+            session_params={
+                "node_type": ["user", "client", "grant"],
+                "node_info_class": {
+                    "user": UserSessionInfo,
+                    "client": ClientSessionInfo,
+                    "grant": Grant,
+                },
+            },
+        )
 
     def test_user_info(self):
         with pytest.raises(KeyError):
             self.db.get(["diana"])
 
         user_info = UserSessionInfo("diana", foo="bar")
         self.db.set(["diana"], user_info)
@@ -100,21 +104,21 @@
         grant = Grant(authentication_event=authn_event, authorization_request=AUTHZ_REQ)
 
         access_code = SessionToken("access_code", value="1234567890")
         grant.issued_token.append(access_code)
 
         self.db.set(["diana", "client_1", "G1"], grant)
         stored_client_info = self.db.get(["diana", "client_1"])
-        assert isinstance(stored_client_info,ClientSessionInfo)
+        assert isinstance(stored_client_info, ClientSessionInfo)
         assert set(stored_client_info.keys()) == {
             "subordinate",
             "revoked",
             "type",
             "extra_args",
-            "id"
+            "id",
         }
 
         stored_grant_info = self.db.get(["diana", "client_1", "G1"])
         assert stored_grant_info.issued_at
 
     def test_jump_ahead(self):
         grant = Grant()
@@ -122,15 +126,15 @@
         grant.issued_token.append(access_code)
 
         self.db.set(["diana", "client_1", "G1"], grant)
 
         user_info = self.db.get(["diana"])
         assert user_info.subordinate == ["diana;;client_1"]
         client_info = self.db.get(["diana", "client_1"])
-        assert client_info.subordinate == ['diana;;client_1;;G1']
+        assert client_info.subordinate == ["diana;;client_1;;G1"]
         grant_info = self.db.get(["diana", "client_1", "G1"])
         assert grant_info.issued_at
         assert len(grant_info.issued_token) == 1
         token = grant_info.issued_token[0]
         assert token.value == "1234567890"
         assert token.token_class == "access_code"
```

### Comparing `idpyoidc-2.0.0/tests/test_server_08_id_token.py` & `idpyoidc-2.1.0/tests/test_server_08_id_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
             "client_salt": "salted",
             "token_endpoint_auth_method": "client_secret_post",
             "response_types": ["code", "token", "code id_token", "id_token"],
             "add_claims": {
                 "always": {},
                 "by_scope": {},
             },
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"]
+            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"],
         }
         self.server.keyjar.add_symmetric("client_1", "hemligtochintekort", ["sig", "enc"])
         self.session_manager = self.context.session_manager
         self.user_id = USER_ID
 
     def _create_session(self, auth_req, sub_type="public", sector_identifier="", authn_info=""):
         if sector_identifier:
@@ -431,19 +431,15 @@
         # default signing alg
         assert algs == {"sign": True, "encrypt": False, "sign_alg": "RS256"}
 
         algs = get_sign_and_encrypt_algorithms(
             self.context, client_info, "id_token", sign=True, encrypt=True
         )
         # default signing alg
-        assert algs == {
-            "sign": True,
-            "encrypt": True,
-            "sign_alg": "RS256"
-        }
+        assert algs == {"sign": True, "encrypt": True, "sign_alg": "RS256"}
 
     def test_available_claims(self):
         req = dict(AREQ)
         req["claims"] = {"id_token": {"nickname": {"essential": True}}}
         session_id = self._create_session(req)
         grant = self.session_manager[session_id]
 
@@ -502,17 +498,15 @@
         assert "foobar" not in res
 
     def test_client_claims(self):
         session_id = self._create_session(AREQ)
         grant = self.session_manager[session_id]
 
         self.session_manager.token_handler["id_token"].kwargs["enable_claims_per_client"] = True
-        self.context.cdb["client_1"]["add_claims"]["always"]["id_token"] = {
-            "address": None
-        }
+        self.context.cdb["client_1"]["add_claims"]["always"]["id_token"] = {"address": None}
 
         _claims = self.context.claims_interface.get_claims(
             session_id=session_id, scopes=AREQ["scope"], claims_release_point="id_token"
         )
         grant.claims = {"id_token": _claims}
 
         id_token = self._mint_id_token(grant, session_id)
```

### Comparing `idpyoidc-2.0.0/tests/test_server_09_authn_context.py` & `idpyoidc-2.1.0/tests/test_server_09_authn_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         "implicit",
         "urn:ietf:params:oauth:grant-type:jwt-bearer",
         "refresh_token",
     ],
     "claim_types_supported": ["normal", "aggregated", "distributed"],
     "claims_parameter_supported": True,
     "request_parameter_supported": True,
-    "request_uri_parameter_supported": True,
+    # "request_uri_parameter_supported": True,
 }
 
 BASEDIR = os.path.abspath(os.path.dirname(__file__))
 
 
 def full_path(local_file):
     return os.path.join(BASEDIR, local_file)
```

### Comparing `idpyoidc-2.0.0/tests/test_server_10_session_manager.py` & `idpyoidc-2.1.0/tests/test_server_10_session_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,22 @@
                 "post_logout_redirect_uri": (f"{CLI1}logout_cb", ""),
                 "token_usage_rules": {
                     "authorization_code": {
                         "supports_minting": ["access_token", "refresh_token", "id_token"]
                     },
                     "refresh_token": {"supports_minting": ["id_token"]},
                 },
-                "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"]
+                "allowed_scopes": [
+                    "openid",
+                    "profile",
+                    "email",
+                    "address",
+                    "phone",
+                    "offline_access",
+                ],
             }
         }
 
         self.session_manager = server.context.session_manager
         self.authn_event = AuthnEvent(
             uid="uid", valid_until=utc_time_sans_frac() + 1, authn_info="authn_class_ref"
         )
@@ -147,15 +154,15 @@
             auth_req=authz_req,
             user_id="diana",
             client_id="client_1",
             sub_type=sub_type,
         )
 
         _user_info_1 = self.session_manager.get_user_session_info(session_key_1)
-        assert _user_info_1.subordinate == ['diana;;client_1']
+        assert _user_info_1.subordinate == ["diana;;client_1"]
         _client_info_1 = self.session_manager.get_client_session_info(session_key_1)
         assert len(_client_info_1.subordinate) == 1
         # grant = self.session_manager.get_grant(session_key_1)
 
         # Second session
         authn_req = AUTH_REQ.copy()
         authn_req["client_id"] = "client_2"
@@ -349,15 +356,15 @@
         assert set(_session_info.keys()) == {
             "client_id",
             "grant_id",
             "user_id",
             "user",
             "client",
             "grant",
-            "branch_id"
+            "branch_id",
         }
         assert _session_info["user_id"] == "diana"
         assert _session_info["client_id"] == "client_1"
 
     def test_get_session_info_by_token(self):
         _session_id = self.session_manager.create_session(
             authn_event=self.authn_event,
@@ -375,15 +382,15 @@
         assert set(_session_info.keys()) == {
             "client_id",
             "branch_id",
             "grant_id",
             "user_id",
             "user",
             "client",
-            "grant"
+            "grant",
         }
         assert _session_info["user_id"] == "diana"
         assert _session_info["client_id"] == "client_1"
 
     def test_token_usage_default(self):
         _session_id = self.session_manager.create_session(
             authn_event=self.authn_event,
@@ -511,15 +518,15 @@
             "token_usage_rules": {
                 "authorization_code": {
                     "expires_in": 600,
                     "supports_minting": ["access_token", "refresh_token"],
                 },
                 "refresh_token": {"supports_minting": ["access_token"]},
             },
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"]
+            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"],
         }
 
         token_usage_rules = self.endpoint_context.authz.usage_rules("client_1")
 
         _session_id = self.session_manager.create_session(
             authn_event=self.authn_event,
             auth_req=AUTH_REQ,
@@ -667,15 +674,16 @@
         else:
             raise Exception("get_authentication_events MUST return a list of AuthnEvent")
 
         # and now add_grant
         grant = self.session_manager[_session_id]
         grant_kwargs = grant.parameter
         for i in ("not_before", "used"):
-            grant_kwargs.pop(i)
+            if i in grant_kwargs:
+                del grant_kwargs[i]
         self.session_manager.add_grant(["diana", "client_1"], **grant_kwargs)
 
     def test_find_latest_idtoken(self):
         token_usage_rules = self.endpoint_context.authz.usage_rules("client_1")
         _session_id = self.session_manager.create_session(
             authn_event=self.authn_event,
             auth_req=AUTH_REQ,
```

### Comparing `idpyoidc-2.0.0/tests/test_server_11_session_manager_pairwise.py` & `idpyoidc-2.1.0/tests/test_server_11_session_manager_pairwise.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_server_12_session_life.py` & `idpyoidc-2.1.0/tests/test_server_12_session_life.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,15 @@
         "authorization_code",
         "implicit",
         "urn:ietf:params:oauth:grant-type:jwt-bearer",
     ],
     "claim_types_supported": ["normal", "aggregated", "distributed"],
     "claims_parameter_supported": True,
     "request_parameter_supported": True,
-    "request_uri_parameter_supported": True,
+    # "request_uri_parameter_supported": True,
 }
 BASEDIR = os.path.abspath(os.path.dirname(__file__))
 
 
 class TestSessionJWTToken:
     @pytest.fixture(autouse=True)
     def setup_session_manager(self):
```

### Comparing `idpyoidc-2.0.0/tests/test_server_13_user_authn.py` & `idpyoidc-2.1.0/tests/test_server_13_user_authn.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_server_14_userinfo.py` & `idpyoidc-2.1.0/tests/test_server_14_userinfo.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_server_15_login_hint.py` & `idpyoidc-2.1.0/tests/test_server_15_login_hint.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_server_16_endpoint.py` & `idpyoidc-2.1.0/tests/test_server_16_endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
                 "code": {"lifetime": 600, "kwargs": {"crypt_conf": CRYPT_CONFIG}},
                 "token": {"lifetime": 600, "kwargs": {"crypt_conf": CRYPT_CONFIG}},
                 "refresh": {"lifetime": 600, "kwargs": {"crypt_conf": CRYPT_CONFIG}},
             },
         }
         server = Server(OPConfiguration(conf=conf, base_path=BASEDIR), cwd=BASEDIR)
 
-        server.context.cdb["client_id"] = {}
+        server.context.cdb["client_id"] = {"redirect_uris": [("https://example.com/cb", None)]}
         self.context = server.context
         _endpoints = do_endpoints(conf, server.unit_get)
         self.endpoint = _endpoints[""]
 
     def test_parse_urlencoded(self):
         self.endpoint.request_format = "urlencoded"
         request = REQ.to_urlencoded()
@@ -104,15 +104,15 @@
         self.endpoint.request_format = "json"
         request = REQ.to_dict()
         req = self.endpoint.parse_request(request)
         assert req == REQ
 
     def test_parse_jwt(self):
         self.endpoint.request_format = "jwt"
-        kj = self.endpoint.upstream_get('attribute','keyjar')
+        kj = self.endpoint.upstream_get("attribute", "keyjar")
         request = REQ.to_jwt(kj.get_signing_key("RSA"), "RS256")
         req = self.endpoint.parse_request(request)
         assert req == REQ
 
     def test_construct(self):
         msg = self.endpoint.construct(EXAMPLE_MSG, {})
         assert set(msg.keys()) == set(EXAMPLE_MSG.keys())
```

### Comparing `idpyoidc-2.0.0/tests/test_server_16_endpoint_context.py` & `idpyoidc-2.1.0/tests/test_server_16_endpoint_context.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,22 +42,15 @@
     "client_authn_method": [
         "private_key_jwt",
         "client_secret_jwt",
         "client_secret_post",
         "client_secret_basic",
     ],
     "subject_types_supported": ["public", "pairwise"],
-    "endpoint": {
-
-        "userinfo": {
-            "path": "userinfo",
-            "class": Endpoint_1,
-            "kwargs": {}
-        }
-    },
+    "endpoint": {"userinfo": {"path": "userinfo", "class": Endpoint_1, "kwargs": {}}},
     "token_handler_args": {
         "jwks_def": {
             "private_path": "private/token_jwks.json",
             "read_only": False,
             "key_defs": [{"type": "oct", "bytes": "24", "use": ["enc"], "kid": "code"}],
         },
         "code": {"lifetime": 600, "kwargs": {"crypt_conf": CRYPT_CONFIG}},
@@ -84,31 +77,31 @@
     },
     "claims_interface": {"class": "idpyoidc.server.session.claims.ClaimsInterface", "kwargs": {}},
     "session_params": SESSION_PARAMS,
 }
 
 
 class TestEndpointContext:
-
     @pytest.fixture(autouse=True)
     def create_endpoint_context(self):
         server = Server(conf)
         server.context.map_supported_to_preferred()
         self.context = server.context
 
     def test(self):
         self.context.set_provider_info()
         assert set(self.context.provider_info.keys()) == {
-            'id_token_signing_alg_values_supported',
-            'issuer',
-            'jwks_uri',
-            'scopes_supported',
-            'subject_types_supported',
-            'userinfo_signing_alg_values_supported',
-            'version'}
+            "id_token_signing_alg_values_supported",
+            "issuer",
+            "jwks_uri",
+            "scopes_supported",
+            "subject_types_supported",
+            "userinfo_signing_alg_values_supported",
+            "version",
+        }
 
 
 class Tokenish(Endpoint):
     _supports = {
         "token_endpoint_auth_methods_supported": [
             "client_secret_post",
             "client_secret_basic",
@@ -167,31 +160,39 @@
         "endpoint": {"path": "endpoint", "class": Tokenish, "kwargs": {}},
     }
 
     server = Server(OPConfiguration(conf=conf, base_path=BASEDIR), cwd=BASEDIR)
     server.context.cdb["client_id"] = {}
     server.context.set_provider_info()
     pi = server.context.provider_info
-    assert set(pi.keys()) == {'acr_values_supported',
-                              'id_token_signing_alg_values_supported',
-                              'issuer',
-                              'jwks_uri',
-                              'scopes_supported',
-                              'subject_types_supported',
-                              'token_endpoint_auth_methods_supported',
-                              'version'}
+    assert set(pi.keys()) == {
+        "acr_values_supported",
+        "id_token_signing_alg_values_supported",
+        "issuer",
+        "jwks_uri",
+        "scopes_supported",
+        "subject_types_supported",
+        "token_endpoint_auth_methods_supported",
+        "version",
+    }
 
     if kwargs:
-        if 'token_endpoint_auth_methods_supported' in kwargs:
-            assert pi["token_endpoint_auth_methods_supported"] == ['client_secret_jwt',
-                                                                   'private_key_jwt']
+        if "token_endpoint_auth_methods_supported" in kwargs:
+            assert pi["token_endpoint_auth_methods_supported"] == [
+                "client_secret_jwt",
+                "private_key_jwt",
+            ]
         else:
-            assert pi["token_endpoint_auth_methods_supported"] == ['client_secret_post',
-                                                                   'client_secret_basic',
-                                                                   'client_secret_jwt',
-                                                                   'private_key_jwt']
+            assert pi["token_endpoint_auth_methods_supported"] == [
+                "client_secret_post",
+                "client_secret_basic",
+                "client_secret_jwt",
+                "private_key_jwt",
+            ]
 
     else:
-        assert pi["token_endpoint_auth_methods_supported"] == ['client_secret_post',
-                                                               'client_secret_basic',
-                                                               'client_secret_jwt',
-                                                               'private_key_jwt']
+        assert pi["token_endpoint_auth_methods_supported"] == [
+            "client_secret_post",
+            "client_secret_basic",
+            "client_secret_jwt",
+            "private_key_jwt",
+        ]
```

### Comparing `idpyoidc-2.0.0/tests/test_server_17_client_authn.py` & `idpyoidc-2.1.0/tests/test_server_17_client_authn.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,17 @@
 class Endpoint_2(Endpoint):
     name = "endpoint_2"
 
 
 class Endpoint_3(Endpoint):
     name = "endpoint_3"
 
-    def __init__(self, upstream_get: Callable, add_claims_by_scope: Optional[bool] = True, **kwargs):
+    def __init__(
+        self, upstream_get: Callable, add_claims_by_scope: Optional[bool] = True, **kwargs
+    ):
         Endpoint.__init__(
             self,
             upstream_get,
             add_claims_by_scope=add_claims_by_scope,
             **kwargs,
         )
         # Add the issuer ID as an allowed JWT target
@@ -247,52 +249,42 @@
         client_keyjar.import_jwks(KEYJAR.export_jwks(private=True), CONF["issuer"])
 
         _jwks = client_keyjar.export_jwks()
         self.server.keyjar.import_jwks(_jwks, client_id)
 
         _jwt = JWT(client_keyjar, iss=client_id, sign_alg="RS256")
         _jwt.with_jti = True
-        _assertion = _jwt.pack(
-            {"aud": [self.server.get_endpoint("endpoint_1").full_path]}
-        )
+        _assertion = _jwt.pack({"aud": [self.server.get_endpoint("endpoint_1").full_path]})
 
         request = {"client_assertion": _assertion, "client_assertion_type": JWT_BEARER}
 
         # This should be OK
         assert self.method.is_usable(request=request)
-        self.method.verify(
-            request=request, endpoint=self.server.get_endpoint("endpoint_1")
-        )
+        self.method.verify(request=request, endpoint=self.server.get_endpoint("endpoint_1"))
 
         # This should NOT be OK
         with pytest.raises(InvalidToken):
-            self.method.verify(
-                request=request, endpoint=self.server.get_endpoint("authorization")
-            )
+            self.method.verify(request=request, endpoint=self.server.get_endpoint("authorization"))
 
         # This should NOT be OK because this is the second time the token appears
         with pytest.raises(InvalidToken):
-            self.method.verify(
-                request=request, endpoint=self.server.get_endpoint("endpoint_1")
-            )
+            self.method.verify(request=request, endpoint=self.server.get_endpoint("endpoint_1"))
 
     def test_private_key_jwt_auth_endpoint(self):
         # Own dynamic keys
         client_keyjar = build_keyjar(KEYDEFS)
         # The servers keys
         client_keyjar.import_jwks(KEYJAR.export_jwks(private=True), CONF["issuer"])
 
         _jwks = client_keyjar.export_jwks()
         self.server.keyjar.import_jwks(_jwks, client_id)
 
         _jwt = JWT(client_keyjar, iss=client_id, sign_alg="RS256")
         _jwt.with_jti = True
-        _assertion = _jwt.pack(
-            {"aud": [self.server.get_endpoint("endpoint_2").full_path]}
-        )
+        _assertion = _jwt.pack({"aud": [self.server.get_endpoint("endpoint_2").full_path]})
 
         request = {"client_assertion": _assertion, "client_assertion_type": JWT_BEARER}
 
         assert self.method.is_usable(request=request)
         authn_info = self.method.verify(
             request=request,
             endpoint=self.server.get_endpoint("endpoint_2"),
@@ -333,15 +325,18 @@
         server.endpoint = do_endpoints(CONF, server.unit_get)
         self.server = server
         self.context = server.context
         self.method = BearerBody(server.unit_get)
 
     def test_bearer_body(self):
         request = {"access_token": "1234567890"}
-        assert self.method.verify(request, get_client_id_from_token=get_client_id_from_token) == {"token": "1234567890", "method": "bearer_body"}
+        assert self.method.verify(request, get_client_id_from_token=get_client_id_from_token) == {
+            "token": "1234567890",
+            "method": "bearer_body",
+        }
 
     def test_bearer_body_no_token(self):
         request = {}
         with pytest.raises(ClientAuthenticationError):
             self.method.verify(request=request)
 
 
@@ -484,17 +479,15 @@
         res = verify_client(
             request=request,
             endpoint=self.server.get_endpoint("endpoint_4"),
         )
         assert res == {"method": "public", "client_id": client_id}
 
     def test_verify_per_client_per_endpoint(self):
-        self.server.context.cdb[client_id]["registration_endpoint_client_authn_method"] = [
-            "public"
-        ]
+        self.server.context.cdb[client_id]["registration_endpoint_client_authn_method"] = ["public"]
         self.server.context.cdb[client_id]["token_endpoint_client_authn_method"] = [
             "client_secret_post"
         ]
 
         request = {"client_id": client_id}
         res = verify_client(
             request=request,
@@ -706,15 +699,12 @@
     conf["client_authn_methods"] = {"custom": MagicMock(return_value=mock)}
     conf["endpoint"]["registration"]["kwargs"]["client_authn_method"] = ["custom"]
     server = Server(conf=conf, keyjar=KEYJAR)
     server.context.cdb[client_id] = {"client_secret": client_secret}
     server.endpoint = do_endpoints(CONF, server.unit_get)
 
     request = {"redirect_uris": ["https://example.com/cb"]}
-    res = verify_client(
-        request=request,
-        endpoint=server.get_endpoint("endpoint_4")
-    )
+    res = verify_client(request=request, endpoint=server.get_endpoint("endpoint_4"))
 
     assert res == {"client_id": "client_id", "method": "custom"}
     mock.is_usable.assert_called_once()
     mock.verify.assert_called_once()
```

### Comparing `idpyoidc-2.0.0/tests/test_server_20a_server.py` & `idpyoidc-2.1.0/tests/test_server_20a_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
+from copy import copy
+from copy import deepcopy
 import io
 import json
 import os
-from copy import copy
-from copy import deepcopy
 
-import yaml
 from cryptojwt.key_jar import build_keyjar
+import yaml
 
 from idpyoidc.server import Server
 from idpyoidc.server.configure import OPConfiguration
 from idpyoidc.server.login_hint import LoginHintLookup
-from idpyoidc.server.oidc.add_on.pkce import add_pkce_support
+from idpyoidc.server.oauth2.add_on.pkce import add_support
 from idpyoidc.server.oidc.authorization import Authorization
 from idpyoidc.server.oidc.provider_config import ProviderConfiguration
 from idpyoidc.server.oidc.registration import Registration
 from idpyoidc.server.oidc.session import Session
 from idpyoidc.server.oidc.token import Token
 from idpyoidc.server.oidc.userinfo import UserInfo
 from idpyoidc.server.user_authn.authn_context import INTERNETPROTOCOLPASSWORD
@@ -69,15 +69,15 @@
         "anon": {
             "acr": INTERNETPROTOCOLPASSWORD,
             "class": "idpyoidc.server.user_authn.user.NoAuthn",
             "kwargs": {"user": "diana"},
         }
     },
     "claims_interface": {"class": "idpyoidc.server.session.claims.ClaimsInterface", "kwargs": {}},
-    "add_on": {"pkce": {"function": add_pkce_support, "kwargs": {"essential": True}}},
+    "add_on": {"pkce": {"function": add_support, "kwargs": {"essential": True}}},
     "template_dir": "template",
     "login_hint_lookup": {"class": LoginHintLookup, "kwargs": {}},
     "session_params": SESSION_PARAMS,
     "token_handler_args": {
         "code": {"lifetime": 600, "kwargs": {"crypt_conf": CRYPT_CONFIG}},
         "token": {"lifetime": 600, "kwargs": {"crypt_conf": CRYPT_CONFIG}},
         "refresh": {"lifetime": 600, "kwargs": {"crypt_conf": CRYPT_CONFIG}},
@@ -115,24 +115,19 @@
     _conf = json.loads(_str)
 
     configuration = OPConfiguration(conf=_conf, base_path=BASEDIR, domain="127.0.0.1", port=443)
 
     server = Server(configuration)
     assert set(server.context.provider_info["response_types_supported"]) == {
         "code",
-        "token",
         "id_token",
-        "code token",
         "code id_token",
-        "id_token token",
-        "code id_token token",
     }
     assert server.context.provider_info["request_uri_parameter_supported"] is True
-    assert server.context.get_preference('jwks_uri') == \
-           "https://127.0.0.1:443/static/jwks.json"
+    assert server.context.get_preference("jwks_uri") == "https://127.0.0.1:443/static/jwks.json"
 
 
 def test_capabilities_subset1():
     _cnf = deepcopy(CONF)
     _cnf["response_types_supported"] = ["code"]
     server = Server(_cnf)
     assert server.context.provider_info["response_types_supported"] == ["code"]
```

### Comparing `idpyoidc-2.0.0/tests/test_server_20b_claims.py` & `idpyoidc-2.1.0/tests/test_server_20b_claims.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,19 +121,17 @@
             "redirect_uris": [("https://example.com/cb", None)],
             "client_salt": "salted",
             "token_endpoint_auth_method": "client_secret_post",
             "response_types": ["code", "token", "code id_token", "id_token"],
             "add_claims": {
                 "always": {},
             },
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"]
+            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"],
         }
-        server.keyjar.add_symmetric(
-            "client_1", "hemligtochintekort", ["sig", "enc"]
-        )
+        server.keyjar.add_symmetric("client_1", "hemligtochintekort", ["sig", "enc"])
         self.claims_interface = server.context.claims_interface
         self.context = server.context
         self.session_manager = self.context.session_manager
         self.user_id = USER_ID
         self.server = server
 
     def _create_session(self, auth_req, sub_type="public", sector_identifier=""):
```

### Comparing `idpyoidc-2.0.0/tests/test_server_20c_authz_handling.py` & `idpyoidc-2.1.0/tests/test_server_20c_authz_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,19 +104,17 @@
         server = Server(conf)
         server.context.cdb["client_1"] = {
             "client_secret": "hemligtochintekort",
             "redirect_uris": [("https://example.com/cb", None)],
             "client_salt": "salted",
             "token_endpoint_auth_method": "client_secret_post",
             "response_types": ["code", "token", "code id_token", "id_token"],
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"]
+            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"],
         }
-        server.keyjar.add_symmetric(
-            "client_1", "hemligtochintekort", ["sig", "enc"]
-        )
+        server.keyjar.add_symmetric("client_1", "hemligtochintekort", ["sig", "enc"])
         self.session_manager = server.context.session_manager
         self.user_id = USER_ID
         self.server = server
         self.authz = server.context.authz
 
     def _create_session(self, auth_req, sub_type="public", sector_identifier=""):
         if sector_identifier:
```

### Comparing `idpyoidc-2.0.0/tests/test_server_20d_client_authn.py` & `idpyoidc-2.1.0/tests/test_server_20d_client_authn.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,38 +218,32 @@
 
         # This should be OK
         assert self.method.is_usable(request=request)
         self.method.verify(request=request, endpoint=self.server.get_endpoint("token"))
 
         # This should NOT be OK
         with pytest.raises(InvalidToken):
-            self.method.verify(
-                request=request, endpoint=self.server.get_endpoint("authorization")
-            )
+            self.method.verify(request=request, endpoint=self.server.get_endpoint("authorization"))
 
         # This should NOT be OK because this is the second time the token appears
         with pytest.raises(InvalidToken):
-            self.method.verify(
-                request=request, endpoint=self.server.get_endpoint("token")
-            )
+            self.method.verify(request=request, endpoint=self.server.get_endpoint("token"))
 
     def test_private_key_jwt_auth_endpoint(self):
         # Own dynamic keys
         client_keyjar = build_keyjar(KEYDEFS)
         # The servers keys
         client_keyjar.import_jwks(KEYJAR.export_jwks(private=True), CONF["issuer"])
 
         _jwks = client_keyjar.export_jwks()
         self.server.keyjar.import_jwks(_jwks, client_id)
 
         _jwt = JWT(client_keyjar, iss=client_id, sign_alg="RS256")
         _jwt.with_jti = True
-        _assertion = _jwt.pack(
-            {"aud": [self.server.get_endpoint("authorization").full_path]}
-        )
+        _assertion = _jwt.pack({"aud": [self.server.get_endpoint("authorization").full_path]})
 
         request = {"client_assertion": _assertion, "client_assertion_type": JWT_BEARER}
 
         assert self.method.is_usable(request=request)
         authn_info = self.method.verify(
             request=request,
             endpoint=self.server.get_endpoint("authorization"),
@@ -289,15 +283,17 @@
         self.server = server
         self.context = server.context
         self.method = BearerBody(server.unit_get)
 
     def test_bearer_body(self):
         request = {"access_token": "1234567890"}
         assert self.method.verify(request, get_client_id_from_token=get_client_id_from_token) == {
-            "token": "1234567890", "method": "bearer_body"}
+            "token": "1234567890",
+            "method": "bearer_body",
+        }
 
     def test_bearer_body_no_token(self):
         request = {}
         with pytest.raises(ClientAuthenticationError):
             self.method.verify(request=request)
 
 
@@ -438,17 +434,15 @@
         res = verify_client(
             request=request,
             endpoint=self.server.get_endpoint("registration"),
         )
         assert res == {"method": "public", "client_id": client_id}
 
     def test_verify_per_client_per_endpoint(self):
-        self.server.context.cdb[client_id]["registration_endpoint_client_authn_method"] = [
-            "public"
-        ]
+        self.server.context.cdb[client_id]["registration_endpoint_client_authn_method"] = ["public"]
         self.server.context.cdb[client_id]["token_endpoint_client_authn_method"] = [
             "client_secret_post"
         ]
 
         request = {"client_id": client_id}
         res = verify_client(
             request=request,
@@ -658,15 +652,12 @@
     conf = dict(CONF)
     conf["client_authn_methods"] = {"custom": MagicMock(return_value=mock)}
     conf["endpoint"]["registration"]["kwargs"]["client_authn_method"] = ["custom"]
     server = Server(conf=conf, keyjar=KEYJAR)
     server.context.cdb[client_id] = {"client_secret": client_secret}
 
     request = {"redirect_uris": ["https://example.com/cb"]}
-    res = verify_client(
-        request=request,
-        endpoint=server.get_endpoint("registration")
-    )
+    res = verify_client(request=request, endpoint=server.get_endpoint("registration"))
 
     assert res == {"client_id": "client_id", "method": "custom"}
     mock.is_usable.assert_called_once()
     mock.verify.assert_called_once()
```

### Comparing `idpyoidc-2.0.0/tests/test_server_20e_jwt_token.py` & `idpyoidc-2.1.0/tests/test_server_20e_jwt_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         "authorization_code",
         "implicit",
         "urn:ietf:params:oauth:grant-type:jwt-bearer",
     ],
     "claim_types_supported": ["normal", "aggregated", "distributed"],
     "claims_parameter_supported": True,
     "request_parameter_supported": True,
-    "request_uri_parameter_supported": True,
+    # "request_uri_parameter_supported": True,
 }
 
 AUTH_REQ = AuthorizationRequest(
     client_id="client_1",
     redirect_uri="https://example.com/cb",
     scope=["openid"],
     state="STATE",
@@ -203,15 +203,15 @@
             "client_salt": "salted",
             "token_endpoint_auth_method": "client_secret_post",
             "response_types": ["code", "token", "code id_token", "id_token"],
             "add_claims": {
                 "always": {},
                 "by_scope": {},
             },
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"]
+            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"],
         }
         self.session_manager = self.context.session_manager
         self.user_id = "diana"
         self.endpoint = self.server.get_endpoint("session")
 
     def _create_session(self, auth_req, sub_type="public", sector_identifier=""):
         if sector_identifier:
@@ -265,17 +265,15 @@
         _info = self.session_manager.token_handler.info(access_token.value)
         assert _info["token_class"] == "access_token"
         assert _info["sid"] == session_id
 
     @pytest.mark.parametrize("enable_claims_per_client", [True, False])
     def test_enable_claims_per_client(self, enable_claims_per_client):
         # Set up configuration
-        self.context.cdb["client_1"]["add_claims"]["always"]["access_token"] = {
-            "address": None
-        }
+        self.context.cdb["client_1"]["add_claims"]["always"]["access_token"] = {"address": None}
         self.context.session_manager.token_handler.handler["access_token"].kwargs[
             "enable_claims_per_client"
         ] = enable_claims_per_client
 
         session_id = self._create_session(AUTH_REQ)
         # apply consent
         grant = self.context.authz(session_id=session_id, request=AUTH_REQ)
@@ -407,15 +405,23 @@
             "client_salt": "salted",
             "token_endpoint_auth_method": "client_secret_post",
             "response_types": ["code", "token", "code id_token", "id_token"],
             "add_claims": {
                 "always": {},
                 "by_scope": {},
             },
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access", "webid"]
+            "allowed_scopes": [
+                "openid",
+                "profile",
+                "email",
+                "address",
+                "phone",
+                "offline_access",
+                "webid",
+            ],
         }
         self.session_manager = self.context.session_manager
         self.user_id = "diana"
         self.endpoint = self.server.get_endpoint("session")
 
     def _create_session(self, auth_req, sub_type="public", sector_identifier=""):
         if sector_identifier:
@@ -513,15 +519,15 @@
         # grant = self.session_manager[session_id]
         code = self._mint_token("authorization_code", grant, session_id)
         access_token = self._mint_token(
             "access_token",
             grant,
             session_id,
             code,
-            scope=["openid", 'foobar'],
+            scope=["openid", "foobar"],
             aud=["https://audience.example.com"],
         )
 
         _verifier = JWT(self.server.keyjar)
         _info = _verifier.unpack(access_token.value)
 
         assert _info["token_class"] == "access_token"
```

### Comparing `idpyoidc-2.0.0/tests/test_server_20f_userinfo.py` & `idpyoidc-2.1.0/tests/test_server_20f_userinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
         self.endpoint_context = server.context
         # Just has to be there
         self.endpoint_context.cdb["client1"] = {
             "add_claims": {
                 "always": {},
                 "by_scope": {},
             },
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"]
+            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"],
         }
         self.session_manager = self.endpoint_context.session_manager
         self.claims_interface = ClaimsInterface(server.unit_get)
         self.user_id = "diana"
         self.server = server
 
     def _create_session(self, auth_req, sub_type="public", sector_identifier=""):
@@ -420,15 +420,23 @@
         }
 
     @pytest.fixture(autouse=True)
     def create_endpoint_context(self, conf):
         self.server = Server(conf)
         self.endpoint_context = self.server.context
         self.endpoint_context.cdb["client1"] = {
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access", "research_and_scholarship"]
+            "allowed_scopes": [
+                "openid",
+                "profile",
+                "email",
+                "address",
+                "phone",
+                "offline_access",
+                "research_and_scholarship",
+            ]
         }
         self.session_manager = self.endpoint_context.session_manager
         self.claims_interface = ClaimsInterface(self.server.unit_get)
         self.user_id = "diana"
 
     def _create_session(self, auth_req, sub_type="public", sector_identifier=""):
         if sector_identifier:
```

### Comparing `idpyoidc-2.0.0/tests/test_server_20g_cookie_handler.py` & `idpyoidc-2.1.0/tests/test_server_20g_cookie_handler.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_server_21_oidc_discovery_endpoint.py` & `idpyoidc-2.1.0/tests/test_server_21_oidc_discovery_endpoint.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_server_22_oidc_provider_config_endpoint.py` & `idpyoidc-2.1.0/tests/test_server_22_oidc_provider_config_endpoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 class TestProviderConfigEndpoint(object):
     @pytest.fixture
     def conf(self):
         return {
             "issuer": "https://example.com/",
             "httpc_params": {"verify": False},
-            "capabilities": CAPABILITIES,
+            "preference": CAPABILITIES,
             "keys": {"uri_path": "static/jwks.json", "key_defs": KEYDEFS},
             "endpoint": {
                 "provider_config": {
                     "path": ".well-known/openid-configuration",
                     "class": ProviderConfiguration,
                     "kwargs": {},
                 },
```

### Comparing `idpyoidc-2.0.0/tests/test_server_23_oidc_registration_endpoint.py` & `idpyoidc-2.1.0/tests/test_server_23_oidc_registration_endpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,17 @@
                 },
                 "userinfo": {"path": "userinfo", "class": UserInfo, "kwargs": {}},
             },
             "template_dir": "template",
             "session_params": SESSION_PARAMS,
         }
         server = Server(OPConfiguration(conf=conf, base_path=BASEDIR), cwd=BASEDIR)
-        server.context.cdb["client_id"] = {}
+        server.context.cdb["client_id"] = {
+            "redirect_uris": [("https://example.com/cb", None)],
+        }
         self.endpoint = server.get_endpoint("registration")
 
     def test_parse(self):
         _req = self.endpoint.parse_request(CLI_REQ.to_json())
 
         assert isinstance(_req, RegistrationRequest)
         assert set(_req.keys()).difference(set(CLI_REQ.keys())) == set()
@@ -335,15 +337,18 @@
         _req = MSG.copy()
         _req["initiate_login_uri"] = "http://ilu.example.com"
         _resp = self.endpoint.process_request(request=RegistrationRequest(**_req))
         assert "error" in _resp
         assert _resp["error"] == "invalid_configuration_request"
 
     def test_register_unsupported_response_type(self):
-        self.endpoint.upstream_get("context").provider_info["response_types_supported"] = ["token", "id_token"]
+        self.endpoint.upstream_get("context").provider_info["response_types_supported"] = [
+            "token",
+            "id_token",
+        ]
         _msg = MSG.copy()
         _msg["response_types"] = ["id_token token"]
         _req = self.endpoint.parse_request(RegistrationRequest(**_msg).to_json())
         _resp = self.endpoint.process_request(request=_req)
         assert _resp["error"] == "invalid_request"
         assert "response_type" in _resp["error_description"]
```

### Comparing `idpyoidc-2.0.0/tests/test_server_24_oauth2_authorization_endpoint.py` & `idpyoidc-2.1.0/tests/test_server_24_oauth2_authorization_endpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,15 +266,15 @@
         self.context = context
         self.endpoint = server.get_endpoint("authorization")
         self.session_manager = context.session_manager
         self.user_id = "diana"
 
         self.rp_keyjar = KeyJar()
         self.rp_keyjar.add_symmetric("client_1", "hemligtkodord1234567890")
-        self.endpoint.upstream_get("attribute",'keyjar').add_symmetric(
+        self.endpoint.upstream_get("attribute", "keyjar").add_symmetric(
             "client_1", "hemligtkodord1234567890"
         )
 
     def _create_session(self, auth_req, sub_type="public", sector_identifier=""):
         if sector_identifier:
             areq = auth_req.copy()
             areq["sector_identifier_uri"] = sector_identifier
@@ -487,15 +487,15 @@
             scope="openid",
         )
 
         self.endpoint.upstream_get("context").cdb["client_id"] = {
             "client_id": "client_id",
             "redirect_uris": [("https://rp.example.com/cb", {})],
             "id_token_signed_response_alg": "ES256",
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"]
+            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"],
         }
 
         session_id = self._create_session(request)
 
         resp = self.endpoint.create_authn_response(request, session_id)
         assert isinstance(resp["response_args"], AuthorizationErrorResponse)
 
@@ -566,15 +566,15 @@
             scope="openid THAT-BLOODY_SCOPE",
         )
         redirect_uri = request["redirect_uri"]
         cinfo = {
             "client_id": "client_id",
             "redirect_uris": [("https://rp.example.com/cb", {})],
             "id_token_signed_response_alg": "RS256",
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"]
+            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"],
         }
 
         _context = self.endpoint.upstream_get("context")
         _context.cdb["client_id"] = cinfo
 
         kaka = _context.cookie_handler.make_cookie_content("value", "sso")
 
@@ -704,22 +704,22 @@
             "id_token_signed_response_alg": "RS256",
         }
         res = self.endpoint.setup_auth(request, redirect_uri, cinfo, None, req_user="adam")
         assert "error" in res
 
     def test_unwrap_identity(self):
         identity = {
-            'sid':
-                'Z0FBQUFBQmlZQXFBeDlvSjRENVVYSDBFeTZ6YzVQWTRGVy1laFk2ZmJIbWdPeUhzbVJYbWo5clVPQ045MXpiSVYwS0pfZkREaVUwX2VaVU9HMk9hUktxaGR0R0dQMlRLOXVWQWVTYWJMdDFsVWZJUEItWS1NVi1WQXllNEVlYm9KMDJsSmFYU0pLYWVJeVRKZkJCYmE1T2RpWXRPM3ZmanRlMThfLUNvcnd4ZXVxcFBWdDY0M18tbXNzbjFvbGl4OFdJRTF6YTcwQ3dqNjdsRHdUa1V4ZTlZMjU3SVlXaXdSSTVJSFJJNENwand3a2pOdmV2WGFPRGZhSnZma2NkZ01ZZk1iS3hma1phcQ==',
-            'state': '80ec120d9a322e70e02503e9a99e734174c1e6cb',
-            'timestamp': 1650461312,
-            'uid': '6260077f56d8970e543aa380',
-            'grant_id': 'c636b820c0ad11ecbdd1acde48001122'}
+            "sid": "Z0FBQUFBQmlZQXFBeDlvSjRENVVYSDBFeTZ6YzVQWTRGVy1laFk2ZmJIbWdPeUhzbVJYbWo5clVPQ045MXpiSVYwS0pfZkREaVUwX2VaVU9HMk9hUktxaGR0R0dQMlRLOXVWQWVTYWJMdDFsVWZJUEItWS1NVi1WQXllNEVlYm9KMDJsSmFYU0pLYWVJeVRKZkJCYmE1T2RpWXRPM3ZmanRlMThfLUNvcnd4ZXVxcFBWdDY0M18tbXNzbjFvbGl4OFdJRTF6YTcwQ3dqNjdsRHdUa1V4ZTlZMjU3SVlXaXdSSTVJSFJJNENwand3a2pOdmV2WGFPRGZhSnZma2NkZ01ZZk1iS3hma1phcQ==",
+            "state": "80ec120d9a322e70e02503e9a99e734174c1e6cb",
+            "timestamp": 1650461312,
+            "uid": "6260077f56d8970e543aa380",
+            "grant_id": "c636b820c0ad11ecbdd1acde48001122",
+        }
         _id = self.endpoint._unwrap_identity(identity)
-        assert _id["uid"] == '6260077f56d8970e543aa380'
+        assert _id["uid"] == "6260077f56d8970e543aa380"
 
     # def test_sso(self):
     #     _pr_resp = self.endpoint.parse_request(AUTH_REQ_DICT)
     #     _resp = self.endpoint.process_request(_pr_resp)
     #     msg = self.endpoint.do_response(**_resp)
     #
     #     request = AuthorizationRequest(
```

### Comparing `idpyoidc-2.0.0/tests/test_server_24_oauth2_authorization_endpoint_jar.py` & `idpyoidc-2.1.0/tests/test_server_24_oauth2_authorization_endpoint_jar.py`

 * *Files identical despite different names*

### Comparing `idpyoidc-2.0.0/tests/test_server_24_oauth2_resource_indicators.py` & `idpyoidc-2.1.0/tests/test_server_24_oauth2_resource_indicators.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,24 +34,28 @@
 from idpyoidc.server.oauth2.authorization import FORM_POST
 from idpyoidc.server.oauth2.authorization import Authorization
 from idpyoidc.server.oauth2.token import Token
 from idpyoidc.server.oauth2.authorization import get_uri
 from idpyoidc.server.oauth2.authorization import inputs
 from idpyoidc.server.oauth2.authorization import join_query
 from idpyoidc.server.oauth2.authorization import verify_uri
-from idpyoidc.server.oauth2.authorization import validate_resource_indicators_policy as validate_authorization_resource_indicators_policy
-from idpyoidc.server.oauth2.token_helper import validate_resource_indicators_policy as validate_token_resource_indicators_policy
+from idpyoidc.server.oauth2.authorization import (
+    validate_resource_indicators_policy as validate_authorization_resource_indicators_policy,
+)
+from idpyoidc.server.oauth2.token_helper import (
+    validate_resource_indicators_policy as validate_token_resource_indicators_policy,
+)
 from idpyoidc.server.user_info import UserInfo
 from idpyoidc.time_util import in_a_while
 from tests import CRYPT_CONFIG
 from tests import SESSION_PARAMS
 
 KEYDEFS = [
     {"type": "RSA", "key": "", "use": ["sig"]},
-    {"type": "EC", "crv": "P-256", "use": ["sig"]}
+    {"type": "EC", "crv": "P-256", "use": ["sig"]},
 ]
 
 COOKIE_KEYDEFS = [
     {"type": "oct", "kid": "sig", "use": ["sig"]},
     {"type": "oct", "kid": "enc", "use": ["enc"]},
 ]
 
@@ -348,17 +352,15 @@
                     "client_secret_jwt",
                     "private_key_jwt",
                 ],
                 "resource_indicators": {
                     "policy": {
                         "function": validate_token_resource_indicators_policy,
                         "kwargs": {
-                            "resource_servers_per_client": {
-                                "client_1": ["client_2", "client_3"]
-                            },
+                            "resource_servers_per_client": {"client_1": ["client_2", "client_3"]},
                         },
                     }
                 },
             },
         },
     },
     "authentication": {
@@ -406,14 +408,15 @@
                 "expires_in": 43200,
             }
         },
     },
     "session_params": SESSION_PARAMS,
 }
 
+
 class TestEndpoint(object):
     @pytest.fixture(autouse=False)
     def create_endpoint_ri_disabled(self):
         conf = RESOURCE_INDICATORS_DISABLED
         server = Server(ASConfiguration(conf=conf, base_path=BASEDIR), cwd=BASEDIR)
 
         endpoint_context = server.context
@@ -478,15 +481,15 @@
         # Constructing an authorization code is now done
         _code = grant.mint_token(
             session_id=session_id,
             context=self.endpoint_context,
             token_class="authorization_code",
             token_handler=self.session_manager.token_handler["authorization_code"],
             usage_rules=usage_rules,
-            resources=grant.resources
+            resources=grant.resources,
         )
 
         if _exp_in:
             if isinstance(_exp_in, str):
                 _exp_in = int(_exp_in)
             if _exp_in:
                 _code.expires_at = utc_time_sans_frac() + _exp_in
@@ -517,15 +520,17 @@
             scope="openid",
         )
 
         msg = self.endpoint._post_parse_request(request, "client_1", endpoint_context)
         assert "error" in msg
         assert msg["error_description"] == "Missing resource parameter"
 
-    def test_authorization_code_req_no_resource_indicators_disabled(self, create_endpoint_ri_disabled):
+    def test_authorization_code_req_no_resource_indicators_disabled(
+        self, create_endpoint_ri_disabled
+    ):
         """
         Test successful authorization request when resource indicators is disabled.
         """
         endpoint_context = self.endpoint.upstream_get("context")
         request = AUTH_REQ.copy()
         del request["resource"]
 
@@ -548,17 +553,15 @@
         for the authorization endpoint and requested resource is not permitted for client.
         """
         endpoint_context = self.endpoint.upstream_get("context")
         endpoint_context.cdb["client_1"]["resource_indicators"] = {
             "authorization_code": {
                 "policy": {
                     "function": validate_authorization_resource_indicators_policy,
-                    "kwargs": {
-                        "resource_servers_per_client":["client_3"]
-                    },
+                    "kwargs": {"resource_servers_per_client": ["client_3"]},
                 },
             },
         }
         request = AUTH_REQ.copy()
         client_id = request["client_id"]
 
         msg = self.endpoint._post_parse_request(request, "client_1", endpoint_context)
@@ -585,15 +588,15 @@
 
     def test_authorization_code_req_invalid_resource_client(self, create_endpoint_ri_enabled):
         """
         Test that appropriate error message is returned when resource indicators is enabled
         for the authorization endpoint and requested resource is not permitted for client.
         """
         request = AUTH_REQ.copy()
-        request["resource"] = "client_2"
+        request["resource"] = "client_3"
         client_id = request["client_id"]
         endpoint_context = self.endpoint.upstream_get("context")
 
         msg = self.endpoint._post_parse_request(request, client_id, endpoint_context)
 
         assert "error" in msg
         assert msg["error"] == "invalid_target"
@@ -603,15 +606,15 @@
         """
         Test successful access_token request when resource indicators is enabled.
         """
         self.endpoint.upstream_get("context").cdb["client_3"] = {
             "client_id": "client_3",
             "redirect_uris": [("https://rp.example.com/cb", {})],
             "id_token_signed_response_alg": "ES256",
-            "allowed_scopes": ["openid"]
+            "allowed_scopes": ["openid"],
         }
         session_id = self._create_session(AUTH_REQ)
         grant = self.session_manager[session_id]
         code = self._mint_code(grant, AUTH_REQ["client_id"])
 
         assert code.resources != []
 
@@ -657,15 +660,15 @@
         Test that the requested access_token has the correct scopes based on the allowed scopes of
         the requested resources
         """
         self.endpoint.upstream_get("context").cdb["client_3"] = {
             "client_id": "client_3",
             "redirect_uris": [("https://rp.example.com/cb", {})],
             "id_token_signed_response_alg": "ES256",
-            "allowed_scopes": ["openid"]
+            "allowed_scopes": ["openid"],
         }
 
         session_id = self._create_session(AUTH_REQ)
         grant = self.session_manager[session_id]
         code = self._mint_code(grant, AUTH_REQ["client_id"])
 
         assert code.resources != []
```

### Comparing `idpyoidc-2.0.0/tests/test_server_24_oauth2_token_endpoint.py` & `idpyoidc-2.1.0/tests/test_server_24_oauth2_token_endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,26 +168,25 @@
             },
         },
         "session_params": {"encrypter": SESSION_PARAMS},
     }
 
 
 class TestEndpoint(object):
-
     @pytest.fixture(autouse=True)
     def create_endpoint(self, conf):
         server = Server(ASConfiguration(conf=conf, base_path=BASEDIR), cwd=BASEDIR)
         context = server.context
         context.cdb["client_1"] = {
             "client_secret": "hemligt",
             "redirect_uris": [("https://example.com/cb", None)],
             "client_salt": "salted",
             "endpoint_auth_method": "client_secret_post",
             "response_types": ["code", "token", "code id_token", "id_token"],
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"]
+            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"],
         }
         server.keyjar.import_jwks(CLIENT_KEYJAR.export_jwks(), "client_1")
         self.session_manager = context.session_manager
         self.token_endpoint = server.get_endpoint("token")
         self.user_id = "diana"
         self.context = context
 
@@ -252,15 +251,15 @@
         grant = self.session_manager[session_id]
         code = self._mint_code(grant, AUTH_REQ["client_id"])
 
         _token_request = TOKEN_REQ_DICT.copy()
         _token_request["code"] = code.value
         _req = self.token_endpoint.parse_request(_token_request)
 
-        assert set(_req.keys()).difference(set(_token_request.keys())) == {'authenticated'}
+        assert set(_req.keys()).difference(set(_token_request.keys())) == {"authenticated"}
 
     def test_auth_code_grant_disallowed_per_client(self):
         areq = AUTH_REQ.copy()
         areq["scope"] = ["email"]
         self.context.cdb["client_1"]["grant_types_supported"] = []
 
         session_id = self._create_session(areq)
@@ -453,15 +452,15 @@
     def test_new_refresh_token(self, conf):
         self.context.cdb["client_1"] = {
             "client_secret": "hemligt",
             "redirect_uris": [("https://example.com/cb", None)],
             "client_salt": "salted",
             "endpoint_auth_method": "client_secret_post",
             "response_types": ["code", "token", "code id_token", "id_token"],
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"]
+            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"],
         }
 
         areq = AUTH_REQ.copy()
         areq["scope"] = ["email"]
 
         session_id = self._create_session(areq)
         grant = self.context.authz(session_id, areq)
@@ -493,15 +492,15 @@
     def test_revoke_on_issue_refresh_token(self, conf):
         self.context.cdb["client_1"] = {
             "client_secret": "hemligt",
             "redirect_uris": [("https://example.com/cb", None)],
             "client_salt": "salted",
             "endpoint_auth_method": "client_secret_post",
             "response_types": ["code", "token", "code id_token", "id_token"],
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"]
+            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"],
         }
 
         self.token_endpoint.revoke_refresh_on_issue = True
         areq = AUTH_REQ.copy()
         areq["scope"] = ["email"]
 
         session_id = self._create_session(areq)
@@ -531,15 +530,15 @@
     def test_revoke_on_issue_refresh_token_per_client(self, conf):
         self.context.cdb["client_1"] = {
             "client_secret": "hemligt",
             "redirect_uris": [("https://example.com/cb", None)],
             "client_salt": "salted",
             "endpoint_auth_method": "client_secret_post",
             "response_types": ["code", "token", "code id_token", "id_token"],
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"]
+            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"],
         }
         self.context.cdb[AUTH_REQ["client_id"]]["revoke_refresh_on_issue"] = True
         areq = AUTH_REQ.copy()
         areq["scope"] = ["openid", "offline_access"]
 
         session_id = self._create_session(areq)
         grant = self.context.authz(session_id, areq)
@@ -702,15 +701,15 @@
         _resp = self.token_endpoint.process_request(request=_req, issue_refresh=True)
 
         _request = REFRESH_TOKEN_REQ.copy()
         _request["refresh_token"] = _resp["response_args"]["refresh_token"]
         _req = self.token_endpoint.parse_request(_request.to_json())
         res = self.token_endpoint.process_request(_req)
         assert "error" in res
-        assert res["error_description"] == 'Minting of access_token not supported'
+        assert res["error_description"] == "Minting of access_token not supported"
 
     def test_do_refresh_access_token_revoked(self):
         areq = AUTH_REQ.copy()
         areq["scope"] = ["email"]
 
         session_id = self._create_session(areq)
         grant = self.context.authz(session_id, areq)
@@ -731,16 +730,17 @@
         _req = self.token_endpoint.parse_request(_request.to_json())
         # A revoked token is caught already when parsing the query.
         assert isinstance(_req, TokenErrorResponse)
 
     def test_configure_grant_types(self):
         conf = {"access_token": {"class": "idpyoidc.server.oidc.token.AccessTokenHelper"}}
 
-        _helper = self.token_endpoint.configure_types(conf,
-                                                      self.token_endpoint.helper_by_grant_type)
+        _helper = self.token_endpoint.configure_types(
+            conf, self.token_endpoint.helper_by_grant_type
+        )
 
         assert len(_helper) == 1
         assert "access_token" in _helper
         assert "refresh_token" not in _helper
 
     def test_token_request_other_client(self):
         _context = self.context
@@ -795,15 +795,15 @@
     "jwks_file": "private/token_jwks.json",
     "code": {"lifetime": 600, "kwargs": {"crypt_conf": CRYPT_CONFIG}},
     "token": {
         "class": "idpyoidc.server.token.jwt_token.JWTToken",
         "kwargs": {
             "lifetime": 3600,
             "add_claims_by_scope": True,
-            "aud": ["https://example.org/appl"]
+            "aud": ["https://example.org/appl"],
         },
     },
     "refresh": {
         "class": "idpyoidc.server.token.jwt_token.JWTToken",
         "kwargs": {
             "lifetime": 3600,
             "aud": ["https://example.org/appl"],
@@ -815,73 +815,63 @@
     "code": {"lifetime": 600, "kwargs": {"crypt_conf": CRYPT_CONFIG}},
     "token": {
         "class": "idpyoidc.server.token.jwt_token.JWTToken",
         "kwargs": {
             "lifetime": 3600,
             "add_claims_by_scope": True,
             "aud": ["https://example.org/appl"],
-            "profile": 'idpyoidc.message.oauth2.JWTAccessToken',
-            "with_jti": True
+            "profile": "idpyoidc.message.oauth2.JWTAccessToken",
+            "with_jti": True,
         },
     },
     "refresh": {
         "class": "idpyoidc.server.token.jwt_token.JWTToken",
         "kwargs": {
             "lifetime": 3600,
             "aud": ["https://example.org/appl"],
         },
     },
 }
 
 CONTEXT = OidcContext()
 CONTEXT.cwd = BASEDIR
 CONTEXT.issuer = "https://op.example.com"
-CONTEXT.cdb = {
-    "client_1": {}
-}
+CONTEXT.cdb = {"client_1": {}}
 KEYJAR = KeyJar()
 KEYJAR.import_jwks(CLIENT_KEYJAR.export_jwks(private=True), "client_1")
 KEYJAR.import_jwks(CLIENT_KEYJAR.export_jwks(private=True), "")
 
 
 def upstream_get(what, *args):
     if what == "context":
         if not args:
             return CONTEXT
-    elif what == 'attribute':
-        if args[0] == 'keyjar':
+    elif what == "attribute":
+        if args[0] == "keyjar":
             return KEYJAR
 
 
 def test_def_jwttoken():
     _handler = handler.factory(upstream_get=upstream_get, **DEFAULT_TOKEN_HANDLER_ARGS)
-    token_handler = _handler['access_token']
-    token_payload = {
-        'sub': 'subject_id',
-        'aud': 'resource_1',
-        'client_id': 'client_1'
-    }
-    value = token_handler(session_id='session_id', **token_payload)
+    token_handler = _handler["access_token"]
+    token_payload = {"sub": "subject_id", "aud": "resource_1", "client_id": "client_1"}
+    value = token_handler(session_id="session_id", **token_payload)
 
     _jws = factory(value)
     msg = JWTAccessToken(**_jws.jwt.payload())
     # test if all required claims are there
     msg.verify()
     assert True
 
 
 def test_jwttoken():
     _handler = handler.factory(upstream_get=upstream_get, **TOKEN_HANDLER_ARGS)
-    token_handler = _handler['access_token']
-    token_payload = {
-        'sub': 'subject_id',
-        'aud': 'resource_1',
-        'client_id': 'client_1'
-    }
-    value = token_handler(session_id='session_id', **token_payload)
+    token_handler = _handler["access_token"]
+    token_payload = {"sub": "subject_id", "aud": "resource_1", "client_id": "client_1"}
+    value = token_handler(session_id="session_id", **token_payload)
 
     _jws = factory(value)
     msg = JWTAccessToken(**_jws.jwt.payload())
     # test if all required claims are there
     msg.verify()
     assert True
 
@@ -889,102 +879,110 @@
 class MyAccessToken(Message):
     c_param = {
         "iss": SINGLE_REQUIRED_STRING,
         "exp": SINGLE_REQUIRED_INT,
         "aud": REQUIRED_LIST_OF_STRINGS,
         "sub": SINGLE_REQUIRED_STRING,
         "iat": SINGLE_REQUIRED_INT,
-        'usage': SINGLE_REQUIRED_STRING
+        "usage": SINGLE_REQUIRED_STRING,
     }
 
 
 def test_jwttoken_2():
     _handler = handler.factory(upstream_get=upstream_get, **TOKEN_HANDLER_ARGS)
-    token_handler = _handler['access_token']
-    token_payload = {
-        'sub': 'subject_id',
-        'aud': 'Skiresort',
-        'usage': 'skilift'
-    }
-    value = token_handler(session_id='session_id', profile=MyAccessToken, **token_payload)
+    token_handler = _handler["access_token"]
+    token_payload = {"sub": "subject_id", "aud": "Skiresort", "usage": "skilift"}
+    value = token_handler(session_id="session_id", profile=MyAccessToken, **token_payload)
 
     _jws = factory(value)
     msg = MyAccessToken(**_jws.jwt.payload())
     # test if all required claims are there
     msg.verify()
     assert True
 
 
 class TestClientCredentialsFlow(object):
-
     @pytest.fixture(autouse=True)
     def create_endpoint(self, conf):
         server = Server(ASConfiguration(conf=conf, base_path=BASEDIR), cwd=BASEDIR)
         context = server.context
         context.cdb["client_1"] = {
             "client_secret": "hemligt",
             "redirect_uris": [("https://example.com/cb", None)],
             "client_salt": "salted",
             "endpoint_auth_method": "client_secret_post",
             "response_types": ["code", "token", "code id_token", "id_token"],
             "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"],
-            "grant_types_supported": ['client_credentials', 'password']
+            "grant_types_supported": ["client_credentials", "password"],
         }
         self.session_manager = context.session_manager
         self.token_endpoint = server.get_endpoint("token")
         self.user_id = "diana"
         self.context = context
 
     def test_client_credentials(self):
-        request = CCAccessTokenRequest(client_id="client_1", client_secret='hemligt',
-                                       grant_type='client_credentials', scope="whatever")
+        request = CCAccessTokenRequest(
+            client_id="client_1",
+            client_secret="hemligt",
+            grant_type="client_credentials",
+            scope="whatever",
+        )
         request = self.token_endpoint.parse_request(request)
         response = self.token_endpoint.process_request(request)
-        assert set(response.keys()) == {'response_args', 'cookie', 'http_headers'}
-        assert set(response["response_args"].keys()) == {'access_token', 'token_type', 'scope',
-                                                         'expires_in'}
+        assert set(response.keys()) == {"response_args", "cookie", "http_headers"}
+        assert set(response["response_args"].keys()) == {
+            "access_token",
+            "token_type",
+            "scope",
+            "expires_in",
+        }
 
 
 class TestResourceOwnerPasswordCredentialsFlow(object):
-
     @pytest.fixture(autouse=True)
     def create_endpoint(self, conf):
         conf["authentication"] = {
             "user": {
                 "acr": "urn:oasis:names:tc:SAML:2.0:ac:classes:InternetProtocolPassword",
                 "class": "idpyoidc.server.user_authn.user.UserPass",
                 "kwargs": {
                     "db_conf": {
                         "class": "idpyoidc.server.util.JSONDictDB",
-                        "kwargs": {"filename": "passwd.json"}
+                        "kwargs": {"filename": "passwd.json"},
                     }
-                }
+                },
             }
         }
 
         server = Server(ASConfiguration(conf=conf, base_path=BASEDIR), cwd=BASEDIR)
         context = server.context
         context.cdb["client_1"] = {
             "client_secret": "hemligt",
             "redirect_uris": [("https://example.com/cb", None)],
             "client_salt": "salted",
             "endpoint_auth_method": "client_secret_post",
             "response_types": ["code", "token", "code id_token", "id_token"],
             "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"],
-            "grant_types_supported": ['client_credentials', 'password'],
+            "grant_types_supported": ["client_credentials", "password"],
         }
         self.session_manager = context.session_manager
         self.token_endpoint = server.get_endpoint("token")
         self.context = context
 
     def test_resource_owner_password_credentials(self):
-        request = ROPCAccessTokenRequest(client_id="client_1",
-                                         client_secret='hemligt',
-                                         grant_type='password',
-                                         username='diana',
-                                         password='krall',
-                                         scope="whatever")
+        request = ROPCAccessTokenRequest(
+            client_id="client_1",
+            client_secret="hemligt",
+            grant_type="password",
+            username="diana",
+            password="krall",
+            scope="whatever",
+        )
         request = self.token_endpoint.parse_request(request)
         response = self.token_endpoint.process_request(request)
-        assert set(response.keys()) == {'response_args', 'cookie', 'http_headers'}
-        assert set(response["response_args"].keys()) == {'access_token', 'token_type', 'scope',
-                                                         'expires_in'}
+        assert set(response.keys()) == {"response_args", "cookie", "http_headers"}
+        assert set(response["response_args"].keys()) == {
+            "access_token",
+            "token_type",
+            "scope",
+            "expires_in",
+        }
```

### Comparing `idpyoidc-2.0.0/tests/test_server_24_oidc_authorization_endpoint.py` & `idpyoidc-2.1.0/tests/test_server_24_oidc_authorization_endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,21 +60,16 @@
 KEYDEFS = [
     {"type": "RSA", "key": "", "use": ["sig"]},
     {"type": "EC", "crv": "P-256", "use": ["sig"]},
 ]
 
 RESPONSE_TYPES_SUPPORTED = [
     ["code"],
-    ["token"],
     ["id_token"],
-    ["code", "token"],
     ["code", "id_token"],
-    ["id_token", "token"],
-    ["code", "token", "id_token"],
-    ["none"],
 ]
 
 CAPABILITIES = {
     "subject_types_supported": ["public", "pairwise", "ephemeral"],
     "grant_types_supported": [
         "authorization_code",
         "implicit",
@@ -116,40 +111,38 @@
 oidc_clients:
   client_1:
     "client_secret": 'hemligtkodord'
     "redirect_uris":
         - ['https://example.com/cb', '']
     "client_salt": "salted"
     'token_endpoint_auth_method': 'client_secret_post'
-    'response_types':
+    response_types_supported:
         - 'code'
-        - 'token'
         - 'code id_token'
         - 'id_token'
-        - 'code id_token token'
     allowed_scopes:
         - 'openid'
         - 'profile'
         - 'email'
         - 'address'
         - 'phone'
         - 'offline_access'
   client2:
     client_secret: "spraket_sr.se"
     redirect_uris:
       - ['https://app1.example.net/foo', '']
       - ['https://app2.example.net/bar', '']
-    response_types:
+    response_types_supported:
       - code
   client3:
     client_secret: '2222222222222222222222222222222222222222'
     redirect_uris:
       - ['https://127.0.0.1:8090/authz_cb/bobcat', '']
     post_logout_redirect_uri: ['https://openidconnect.net/', '']
-    response_types:
+    response_types_supported:
       - code
     allowed_scopes:
         - 'openid'
         - 'profile'
         - 'email'
         - 'address'
         - 'phone'
@@ -290,17 +283,15 @@
         }
         server = Server(OPConfiguration(conf=conf, base_path=BASEDIR), cwd=BASEDIR)
 
         context = server.context
 
         _clients = yaml.safe_load(io.StringIO(client_yaml))
         context.cdb = _clients["oidc_clients"]
-        server.keyjar.import_jwks(
-            server.keyjar.export_jwks(True, ""), conf["issuer"]
-        )
+        server.keyjar.import_jwks(server.keyjar.export_jwks(True, ""), conf["issuer"])
         self.context = context
         self.endpoint = server.get_endpoint("authorization")
         self.session_manager = context.session_manager
         self.user_id = "diana"
 
         self.rp_keyjar = KeyJar()
         self.rp_keyjar.add_symmetric("client_1", "hemligtkodord1234567890")
@@ -373,22 +364,14 @@
         assert part.fragment
         _frag_msg = parse_qs(part.fragment)
         assert _frag_msg
         assert "id_token" in _frag_msg
         assert "code" not in _frag_msg
         assert "token" not in _frag_msg
 
-    def test_do_response_id_token_token(self):
-        _orig_req = AUTH_REQ_DICT.copy()
-        _orig_req["response_type"] = "id_token token"
-        _orig_req["nonce"] = "rnd_nonce"
-        _pr_resp = self.endpoint.parse_request(_orig_req)
-        assert isinstance(_pr_resp, AuthorizationErrorResponse)
-        assert _pr_resp["error"] == "invalid_request"
-
     def test_do_response_code_token(self):
         _orig_req = AUTH_REQ_DICT.copy()
         _orig_req["response_type"] = "code token"
         _pr_resp = self.endpoint.parse_request(_orig_req)
         assert isinstance(_pr_resp, AuthorizationErrorResponse)
         assert _pr_resp["error"] == "invalid_request"
 
@@ -405,41 +388,23 @@
         assert part.fragment
         _frag_msg = parse_qs(part.fragment)
         assert _frag_msg
         assert "id_token" in _frag_msg
         assert "code" in _frag_msg
         assert "access_token" not in _frag_msg
 
-    def test_do_response_code_id_token_token(self):
-        _orig_req = AUTH_REQ_DICT.copy()
-        _orig_req["response_type"] = "code id_token token"
-        _orig_req["nonce"] = "rnd_nonce"
-        _pr_resp = self.endpoint.parse_request(_orig_req)
-        _resp = self.endpoint.process_request(_pr_resp)
-        msg = self.endpoint.do_response(**_resp)
-        assert isinstance(msg, dict)
-        part = urlparse(msg["response"])
-        assert part.query == ""
-        assert part.fragment
-        _frag_msg = parse_qs(part.fragment)
-        assert _frag_msg
-        assert "id_token" in _frag_msg
-        assert "code" in _frag_msg
-        assert "access_token" in _frag_msg
-
     def test_id_token_claims(self):
         _req = AUTH_REQ_DICT.copy()
         _req["claims"] = CLAIMS
         _req["response_type"] = "id_token"
         _req["nonce"] = "rnd_nonce"
         _pr_resp = self.endpoint.parse_request(_req)
         _resp = self.endpoint.process_request(_pr_resp)
         idt = verify_id_token(
-            _resp["response_args"],
-            keyjar=self.endpoint.upstream_get("attribute","keyjar")
+            _resp["response_args"], keyjar=self.endpoint.upstream_get("attribute", "keyjar")
         )
         assert idt
         # from config
         assert "given_name" in _resp["response_args"]["__verified_id_token"]
         assert "nickname" in _resp["response_args"]["__verified_id_token"]
         # Could have gotten email but didn't ask for it
         assert "email" in _resp["response_args"]["__verified_id_token"]
@@ -450,21 +415,21 @@
         assert re_authenticate(request, authn)
 
     def test_id_token_acr(self):
         _req = AUTH_REQ_DICT.copy()
         _req["claims"] = {
             "id_token": {"acr": {"value": "http://www.swamid.se/policy/assurance/al1"}}
         }
-        _req["response_type"] = "code id_token token"
+        _req["response_type"] = "code id_token"
         _req["nonce"] = "rnd_nonce"
         _pr_resp = self.endpoint.parse_request(_req)
         _resp = self.endpoint.process_request(_pr_resp)
         res = verify_id_token(
             _resp["response_args"],
-            keyjar=self.endpoint.upstream_get("attribute","keyjar"),
+            keyjar=self.endpoint.upstream_get("attribute", "keyjar"),
         )
         assert res
         res = _resp["response_args"][verified_claim_name("id_token")]
         assert res["acr"] == "http://www.swamid.se/policy/assurance/al1"
 
     def test_verify_uri_unknown_client(self):
         request = {"redirect_uri": "https://rp.example.com/cb"}
@@ -603,15 +568,15 @@
         )
 
         _ec = self.endpoint.upstream_get("context")
         _ec.cdb["client_id"] = {
             "client_id": "client_id",
             "redirect_uris": [("https://rp.example.com/cb", {})],
             "id_token_signed_response_alg": "ES256",
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"]
+            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"],
         }
 
         session_id = self._create_session(request)
 
         resp = self.endpoint.create_authn_response(request, session_id)
         assert isinstance(resp["response_args"], AuthorizationResponse)
 
@@ -631,15 +596,15 @@
         )
 
         _ec = self.endpoint.upstream_get("context")
         _ec.cdb["client_id"] = {
             "client_id": "client_id",
             "redirect_uris": [("https://rp.example.com/cb", {})],
             "id_token_signed_response_alg": "ES256",
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"]
+            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"],
         }
 
         session_id = self._create_session(request)
 
         resp = self.endpoint.create_authn_response(request, session_id)
         assert isinstance(resp["response_args"], AuthorizationResponse)
 
@@ -826,17 +791,15 @@
         redirect_uri = request["redirect_uri"]
 
         method_spec = {
             "acr": INTERNETPROTOCOLPASSWORD,
             "kwargs": {"user": "knoll"},
             "class": NoAuthn,
         }
-        self.endpoint.upstream_get("context").authn_broker["foo"] = init_method(
-            method_spec, None
-        )
+        self.endpoint.upstream_get("context").authn_broker["foo"] = init_method(method_spec, None)
 
         item = self.endpoint.upstream_get("context").authn_broker.db["anon"]
         item["method"].fail = NoSuchAuthentication
         item = self.endpoint.upstream_get("context").authn_broker.db["foo"]
         item["method"].fail = NoSuchAuthentication
 
         res = self.endpoint.pick_authn_method(request, redirect_uri)
@@ -860,23 +823,25 @@
                 "request": _jws,
                 "redirect_uri": AUTH_REQ.get("redirect_uri"),
                 "response_type": AUTH_REQ.get("response_type"),
                 "client_id": AUTH_REQ.get("client_id"),
                 "scope": AUTH_REQ.get("scope"),
             }
         )
-        assert set(_req.keys()) == {'__verified_request',
-                                    'aud',
-                                    'client_id',
-                                    'iat',
-                                    'iss',
-                                    'redirect_uri',
-                                    'response_type',
-                                    'scope',
-                                    'state'}
+        assert set(_req.keys()) == {
+            "__verified_request",
+            "aud",
+            "client_id",
+            "iat",
+            "iss",
+            "redirect_uri",
+            "response_type",
+            "scope",
+            "state",
+        }
 
     def test_parse_request_uri(self):
         _jwt = JWT(key_jar=self.rp_keyjar, iss="client_1", sign_alg="HS256")
         _jws = _jwt.pack(
             AUTH_REQ_DICT,
             aud=self.endpoint.upstream_get("context").provider_info["issuer"],
         )
@@ -897,64 +862,46 @@
 
         assert "__verified_request" in _req
 
     def test_verify_response_type(self):
         request = AuthorizationRequest(
             client_id="client_id",
             redirect_uri="https://rp.example.com/cb",
-            response_type=["id_token token"],
+            response_type=["id_token"],
             state="state",
             nonce="nonce",
             scope="openid",
         )
         client_info = {
             "client_id": "client_id",
             "redirect_uris": [("https://rp.example.com/cb", {})],
             "id_token_signed_response_alg": "RS256",
             "policy_uri": "https://example.com/policy.html",
         }
 
         assert self.endpoint.verify_response_type(request, client_info) is False
 
-        client_info["response_types"] = [
+        client_info["response_types_supported"] = [
             "code",
             "code id_token",
             "id_token",
-            "id_token token",
         ]
 
         assert self.endpoint.verify_response_type(request, client_info) is True
 
-    # @pytest.mark.parametrize("exp_in", [360, "360", 0])
-    # def test_mint_token_exp_at(self, exp_in):
-    #     request = AuthorizationRequest(
-    #         client_id="client_1",
-    #         response_type=["code"],
-    #         redirect_uri="https://example.com/cb",
-    #         state="state",
-    #         scope="openid",
-    #     )
-    #     self.session_manager.set(["user_id", "client_id", "grant.id"], grant)
-    #
-    #     code = self.endpoint.mint_token("authorization_code", grant, sid)
-    #     if exp_in in [360, "360"]:
-    #         assert code.expires_at
-    #     else:
-    #         assert code.expires_at == 0
-
     def test_do_request_uri(self):
         request = AuthorizationRequest(
             redirect_uri="https://rp.example.com/cb",
             request_uri="https://example.com/request",
         )
 
         orig_request = AuthorizationRequest(
             client_id="client_id",
             redirect_uri="https://rp.example.com/cb",
-            response_type=["id_token token"],
+            response_type=["id_token"],
             state="state",
             nonce="nonce",
             scope="openid",
         )
         _jwt = JWT(key_jar=self.rp_keyjar, iss="client_1", sign_alg="HS256")
         _jws = _jwt.pack(
             orig_request.to_dict(),
@@ -1240,17 +1187,15 @@
         }
         server = Server(OPConfiguration(conf=conf, base_path=BASEDIR), cwd=BASEDIR)
 
         context = server.context
 
         _clients = yaml.safe_load(io.StringIO(client_yaml))
         context.cdb = _clients["oidc_clients"]
-        server.keyjar.import_jwks(
-            server.keyjar.export_jwks(True, ""), conf["issuer"]
-        )
+        server.keyjar.import_jwks(server.keyjar.export_jwks(True, ""), conf["issuer"])
         self.endpoint = server.get_endpoint("authorization")
         self.session_manager = context.session_manager
         self.user_id = "diana"
 
         self.rp_keyjar = KeyJar()
         self.rp_keyjar.add_symmetric("client_1", "hemligtkodord1234567890")
         server.keyjar.add_symmetric("client_1", "hemligtkodord1234567890")
@@ -1468,15 +1413,18 @@
             sid=self.context.session_manager.encrypted_session_id(
                 "adam", "client 12345", "0123456789"
             ),
             state=authn_req["state"],
             client_id=authn_req["client_id"],
         )
 
-        kakor = [{
-            'value': '{"sub": "adam", "sid": "Z0FBQUFBQmlhVl", "state": "state_identifier", '
-                     '"client_id": "client 12345"}',
-            'type': '',
-            'timestamp': '1651070251'}]
+        kakor = [
+            {
+                "value": '{"sub": "adam", "sid": "Z0FBQUFBQmlhVl", "state": "state_identifier", '
+                '"client_id": "client 12345"}',
+                "type": "",
+                "timestamp": "1651070251",
+            }
+        ]
 
         _info, _time_stamp = method.authenticated_as(client_id="client 12345", cookie=kakor)
         assert _info == {}
```

### Comparing `idpyoidc-2.0.0/tests/test_server_26_oidc_userinfo_endpoint.py` & `idpyoidc-2.1.0/tests/test_server_26_oidc_userinfo_endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,38 +17,30 @@
 from idpyoidc.server.oidc.authorization import Authorization
 from idpyoidc.server.oidc.provider_config import ProviderConfiguration
 from idpyoidc.server.oidc.registration import Registration
 from idpyoidc.server.oidc.token import Token
 from idpyoidc.server.scopes import SCOPE2CLAIMS
 from idpyoidc.server.user_authn.authn_context import INTERNETPROTOCOLPASSWORD
 from idpyoidc.server.user_info import UserInfo
-from idpyoidc.server.oidc.userinfo import validate_userinfo_policy
 from idpyoidc.time_util import utc_time_sans_frac
 from tests import CRYPT_CONFIG
 from tests import SESSION_PARAMS
 
-
 KEYDEFS = [
     {"type": "RSA", "key": "", "use": ["sig"]},
     {"type": "EC", "crv": "P-256", "use": ["sig"]},
 ]
 
-RESPONSE_TYPES_SUPPORTED = [
-    ["code"],
-    ["token"],
-    ["id_token"],
-    ["code", "token"],
-    ["code", "id_token"],
-    ["id_token", "token"],
-    ["code", "token", "id_token"],
-    ["none"],
-]
+# RESPONSE_TYPES_SUPPORTED = [
+#     ["code"],
+#     ["id_token"],
+#     ["code", "id_token"],
+# ]
 
-CAPABILITIES = {
-}
+CAPABILITIES = {}
 
 AUTH_REQ = AuthorizationRequest(
     client_id="client_1",
     redirect_uri="https://example.com/cb",
     scope=["openid"],
     state="STATE",
     response_type="code",
@@ -77,15 +69,15 @@
 class TestEndpoint(object):
     @pytest.fixture(autouse=True)
     def create_endpoint(self):
         conf = {
             "issuer": "https://example.com/",
             "httpc_params": {"verify": False, "timeout": 1},
             "subject_types_supported": ["public", "pairwise", "ephemeral"],
-            'claims_supported': [
+            "claims_supported": [
                 "address",
                 "birthdate",
                 "email",
                 "email_verified",
                 "eduperson_scoped_affiliation",
                 "family_name",
                 "gender",
@@ -98,15 +90,16 @@
                 "phone_number_verified",
                 "picture",
                 "preferred_username",
                 "profile",
                 "sub",
                 "updated_at",
                 "website",
-                "zoneinfo"],
+                "zoneinfo",
+            ],
             "grant_types_supported": [
                 "authorization_code",
                 "implicit",
                 "urn:ietf:params:oauth:grant-type:jwt-bearer",
                 "refresh_token",
             ],
             "claim_types_supported": [
@@ -210,16 +203,24 @@
 
         self.context = self.server.context
         self.context.cdb["client_1"] = {
             "client_secret": "hemligt",
             "redirect_uris": [("https://example.com/cb", None)],
             "client_salt": "salted",
             "token_endpoint_auth_method": "client_secret_post",
-            "response_types": ["code", "token", "code id_token", "id_token"],
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access", "research_and_scholarship"]
+            "response_types_supported": ["code", "code id_token", "id_token"],
+            "allowed_scopes": [
+                "openid",
+                "profile",
+                "email",
+                "address",
+                "phone",
+                "offline_access",
+                "research_and_scholarship",
+            ],
         }
         self.endpoint = self.server.get_endpoint("userinfo")
         self.session_manager = self.context.session_manager
         self.user_id = "diana"
 
     def _create_session(self, auth_req, sub_type="public", sector_identifier="", authn_info=None):
         if sector_identifier:
@@ -252,39 +253,37 @@
             token_handler=self.session_manager.token_handler[token_class],
             expires_at=utc_time_sans_frac() + 900,  # 15 minutes from now
             based_on=token_ref,  # Means the token (tok) was used to mint this token
         )
 
     def test_init(self):
         assert self.endpoint
-        assert set(
-            self.endpoint.upstream_get("context").provider_info["claims_supported"]
-        ) == {
-                   "address",
-                   "birthdate",
-                   "email",
-                   "email_verified",
-                   "eduperson_scoped_affiliation",
-                   "family_name",
-                   "gender",
-                   "given_name",
-                   "locale",
-                   "middle_name",
-                   "name",
-                   "nickname",
-                   "phone_number",
-                   "phone_number_verified",
-                   "picture",
-                   "preferred_username",
-                   "profile",
-                   "sub",
-                   "updated_at",
-                   "website",
-                   "zoneinfo",
-               }
+        assert set(self.endpoint.upstream_get("context").provider_info["claims_supported"]) == {
+            "address",
+            "birthdate",
+            "email",
+            "email_verified",
+            "eduperson_scoped_affiliation",
+            "family_name",
+            "gender",
+            "given_name",
+            "locale",
+            "middle_name",
+            "name",
+            "nickname",
+            "phone_number",
+            "phone_number_verified",
+            "picture",
+            "preferred_username",
+            "profile",
+            "sub",
+            "updated_at",
+            "website",
+            "zoneinfo",
+        }
 
     def test_parse(self):
         session_id = self._create_session(AUTH_REQ)
         grant = self.session_manager[session_id]
 
         # Free standing access token, not based on an authorization code
         access_token = self._mint_token("access_token", grant, session_id)
@@ -464,15 +463,15 @@
         assert set(args["response_args"].keys()) == {
             "eduperson_scoped_affiliation",
             "given_name",
             "email_verified",
             "email",
             "family_name",
             "name",
-            "sub"
+            "sub",
         }
 
     def test_allowed_scopes_per_client(self):
         self.context.cdb["client_1"]["scopes_to_claims"] = {
             **SCOPE2CLAIMS,
             "research_and_scholarship_2": [
                 "name",
@@ -630,19 +629,23 @@
         assert _response["acr"] == _acr
 
     def test_process_request_absent_userinfo_conf(self):
         # consider to have a configuration without userinfo defined in
         ec = self.endpoint.upstream_get("context")
         ec.userinfo = None
 
-        session_id = self._create_session(AUTH_REQ)
+        _auth_req = AUTH_REQ.copy()
+        _auth_req["scope"] = ["openid", "email"]
+
+        session_id = self._create_session(_auth_req)
         grant = self.session_manager[session_id]
 
+        code = self._mint_code(grant, session_id)
         with pytest.raises(ImproperlyConfigured):
-            code = self._mint_code(grant, session_id)
+            self._mint_token("access_token", grant, session_id, code)
 
     def test_userinfo_policy(self):
         _auth_req = AUTH_REQ.copy()
 
         session_id = self._create_session(_auth_req)
         grant = self.session_manager[session_id]
         access_token = self._mint_token("access_token", grant, session_id)
@@ -671,20 +674,16 @@
 
         http_info = {"headers": {"authorization": "Bearer {}".format(access_token.value)}}
 
         def _custom_validate_userinfo_policy(request, token, response_info, **kwargs):
             return {"custom": "policy"}
 
         self.context.cdb["client_1"]["userinfo"] = {
-            "policy": {
-                "function": _custom_validate_userinfo_policy,
-                "kwargs": {}
-            }
+            "policy": {"function": _custom_validate_userinfo_policy, "kwargs": {}}
         }
 
         _req = self.endpoint.parse_request({}, http_info=http_info)
         args = self.endpoint.process_request(_req)
         assert args
         res = self.endpoint.do_response(request=_req, **args)
         _response = json.loads(res["response"])
         assert "custom" in _response
-
```

### Comparing `idpyoidc-2.0.0/tests/test_server_30_oidc_end_session.py` & `idpyoidc-2.1.0/tests/test_server_30_oidc_end_session.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,26 +41,17 @@
     {"type": "RSA", "use": ["sig"]},
     {"type": "EC", "crv": "P-256", "use": ["sig"]},
 ]
 
 KEYJAR = build_keyjar(KEYDEFS)
 KEYJAR.import_jwks(KEYJAR.export_jwks(private=True), ISS)
 
-RESPONSE_TYPES_SUPPORTED = [
-    ["code"],
-    ["token"],
-    ["id_token"],
-    ["code", "token"],
-    ["code", "id_token"],
-    ["id_token", "token"],
-    ["code", "token", "id_token"],
-    ["none"],
-]
+RESPONSE_TYPES_SUPPORTED = [["code"], ["id_token"], ["code", "id_token"]]
 
-CAPABILITIES = {
+PREFRERENCES = {
     "response_types_supported": [" ".join(x) for x in RESPONSE_TYPES_SUPPORTED],
     "token_endpoint_auth_methods_supported": [
         "client_secret_post",
         "client_secret_basic",
         "client_secret_jwt",
         "private_key_jwt",
     ],
@@ -102,15 +93,15 @@
 class TestEndpoint(object):
     @pytest.fixture(autouse=True)
     def create_endpoint(self):
         conf = {
             "issuer": ISS,
             "password": "mycket hemlig zebra",
             "verify_ssl": False,
-            "capabilities": CAPABILITIES,
+            "preferences": PREFRERENCES,
             "keys": {"uri_path": "jwks.json", "key_defs": KEYDEFS},
             "endpoint": {
                 "provider_config": {
                     "path": "{}/.well-known/openid-configuration",
                     "class": ProviderConfiguration,
                     "kwargs": {"client_authn_method": None},
                 },
@@ -203,26 +194,40 @@
         context = server.context
         context.cdb = {
             "client_1": {
                 "client_secret": "hemligt",
                 "redirect_uris": [("{}cb".format(CLI1), None)],
                 "client_salt": "salted",
                 "token_endpoint_auth_method": "client_secret_post",
-                "response_types": ["code", "token", "code id_token", "id_token"],
+                "response_types_supported": ["code", "code id_token", "id_token"],
                 "post_logout_redirect_uri": [f"{CLI1}logout_cb", ""],
-                "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"]
+                "allowed_scopes": [
+                    "openid",
+                    "profile",
+                    "email",
+                    "address",
+                    "phone",
+                    "offline_access",
+                ],
             },
             "client_2": {
                 "client_secret": "hemligare",
                 "redirect_uris": [("{}cb".format(CLI2), None)],
                 "client_salt": "saltare",
                 "token_endpoint_auth_method": "client_secret_post",
-                "response_types": ["code", "token", "code id_token", "id_token"],
+                "response_types_supported": ["code", "code id_token", "id_token"],
                 "post_logout_redirect_uri": [f"{CLI2}logout_cb", ""],
-                "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"]
+                "allowed_scopes": [
+                    "openid",
+                    "profile",
+                    "email",
+                    "address",
+                    "phone",
+                    "offline_access",
+                ],
             },
         }
         self.context = context
         self.session_manager = context.session_manager
         self.authn_endpoint = server.get_endpoint("authorization")
         self.session_endpoint = server.get_endpoint("session")
         self.token_endpoint = server.get_endpoint("token")
@@ -332,15 +337,15 @@
         id_token = resp_args["id_token"]
 
         _uid, _cid, _gid = self.session_manager.decrypt_session_id(_session_id)
         cookie = self._create_cookie(self.session_manager.session_key(_uid, "client_66", _gid))
         http_info = {"cookie": [cookie]}
 
         msg = Message(id_token=id_token)
-        verify_id_token(msg, keyjar=self.session_endpoint.upstream_get("attribute",'keyjar'))
+        verify_id_token(msg, keyjar=self.session_endpoint.upstream_get("attribute", "keyjar"))
 
         msg2 = Message(id_token_hint=id_token)
         msg2[verified_claim_name("id_token_hint")] = msg[verified_claim_name("id_token")]
         with pytest.raises(ValueError):
             self.session_endpoint.process_request(msg2, http_info=http_info)
 
     def test_end_session_endpoint_with_cookie_dual_login(self):
@@ -399,15 +404,15 @@
 
         cookie = self._create_cookie(_session_id)
         http_info = {"cookie": [cookie]}
 
         post_logout_redirect_uri = "https://demo.example.com/log_out"
 
         msg = Message(id_token=id_token)
-        verify_id_token(msg, keyjar=self.session_endpoint.upstream_get("attribute",'keyjar'))
+        verify_id_token(msg, keyjar=self.session_endpoint.upstream_get("attribute", "keyjar"))
 
         with pytest.raises(RedirectURIError):
             self.session_endpoint.process_request(
                 {
                     "post_logout_redirect_uri": post_logout_redirect_uri,
                     "state": "abcde",
                     "id_token_hint": id_token,
@@ -488,17 +493,15 @@
         _session_info = self.session_manager.get_session_info_by_token(
             _code, client_session_info=True, handler_key="authorization_code"
         )
 
         self.session_endpoint.upstream_get("context").cdb["client_1"][
             "backchannel_logout_uri"
         ] = "https://example.com/bc_logout"
-        self.session_endpoint.upstream_get("context").cdb["client_1"][
-            "client_id"
-        ] = "client_1"
+        self.session_endpoint.upstream_get("context").cdb["client_1"]["client_id"] = "client_1"
 
         res = self.session_endpoint.logout_from_client(_session_info["branch_id"])
         assert set(res.keys()) == {"blu"}
         assert set(res["blu"].keys()) == {"client_1"}
         _spec = res["blu"]["client_1"]
         assert _spec[0] == "https://example.com/bc_logout"
         _jwt = self.session_endpoint.unpack_signed_jwt(_spec[1], "RS256")
@@ -518,17 +521,15 @@
         )
 
         # del self.session_endpoint.upstream_get("context").cdb['client_1'][
         # 'backchannel_logout_uri']
         self.session_endpoint.upstream_get("context").cdb["client_1"][
             "frontchannel_logout_uri"
         ] = "https://example.com/fc_logout"
-        self.session_endpoint.upstream_get("context").cdb["client_1"][
-            "client_id"
-        ] = "client_1"
+        self.session_endpoint.upstream_get("context").cdb["client_1"]["client_id"] = "client_1"
 
         res = self.session_endpoint.logout_from_client(_session_info["branch_id"])
         assert set(res.keys()) == {"flu"}
         assert set(res["flu"].keys()) == {"client_1"}
         _spec = res["flu"]["client_1"]
         assert _spec == '<iframe src="https://example.com/fc_logout">'
 
@@ -553,23 +554,19 @@
             "id_token", _session_info2["grant"], _session_info2["branch_id"], _grant_code2
         )
 
         # client0
         self.session_endpoint.upstream_get("context").cdb["client_1"][
             "backchannel_logout_uri"
         ] = "https://example.com/bc_logout"
-        self.session_endpoint.upstream_get("context").cdb["client_1"][
-            "client_id"
-        ] = "client_1"
+        self.session_endpoint.upstream_get("context").cdb["client_1"]["client_id"] = "client_1"
         self.session_endpoint.upstream_get("context").cdb["client_2"][
             "frontchannel_logout_uri"
         ] = "https://example.com/fc_logout"
-        self.session_endpoint.upstream_get("context").cdb["client_2"][
-            "client_id"
-        ] = "client_2"
+        self.session_endpoint.upstream_get("context").cdb["client_2"]["client_id"] = "client_2"
 
         res = self.session_endpoint.logout_all_clients(_session_info["branch_id"])
 
         assert res
         assert set(res.keys()) == {"blu", "flu"}
         # Front channel logout
         assert set(res["flu"].keys()) == {"client_2"}
@@ -631,23 +628,19 @@
         )
         self._code_auth2("abcdefg")
 
         # client0
         self.session_endpoint.upstream_get("context").cdb["client_1"][
             "backchannel_logout_uri"
         ] = "https://example.com/bc_logout"
-        self.session_endpoint.upstream_get("context").cdb["client_1"][
-            "client_id"
-        ] = "client_1"
+        self.session_endpoint.upstream_get("context").cdb["client_1"]["client_id"] = "client_1"
         self.session_endpoint.upstream_get("context").cdb["client_2"][
             "frontchannel_logout_uri"
         ] = "https://example.com/fc_logout"
-        self.session_endpoint.upstream_get("context").cdb["client_2"][
-            "client_id"
-        ] = "client_2"
+        self.session_endpoint.upstream_get("context").cdb["client_2"]["client_id"] = "client_2"
 
         _uid, _cid, _gid = self.session_manager.decrypt_session_id(_session_info["branch_id"])
         self.session_endpoint.upstream_get("context").session_manager.delete([_uid, _cid])
 
         with pytest.raises(InvalidBranchID):
             self.session_endpoint.logout_all_clients(_session_info["branch_id"])
```

### Comparing `idpyoidc-2.0.0/tests/test_server_31_oauth2_introspection.py` & `idpyoidc-2.1.0/tests/test_server_31_oauth2_introspection.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         "implicit",
         "urn:ietf:params:oauth:grant-type:jwt-bearer",
         "refresh_token",
     ],
     "claim_types_supported": ["normal", "aggregated", "distributed"],
     "claims_parameter_supported": True,
     "request_parameter_supported": True,
-    "request_uri_parameter_supported": True,
+    # "request_uri_parameter_supported": True,
 }
 
 AUTH_REQ = AuthorizationRequest(
     client_id="client_1",
     redirect_uri="https://example.com/cb",
     scope=["openid"],
     state="STATE",
@@ -87,15 +87,14 @@
 
 def full_path(local_file):
     return os.path.join(BASEDIR, local_file)
 
 
 @pytest.mark.parametrize("jwt_token", [True, False])
 class TestEndpoint:
-
     @pytest.fixture(autouse=True)
     def create_endpoint(self, jwt_token):
         conf = {
             "issuer": "https://example.com/",
             "httpc_params": {"verify": False, "timeout": 1},
             "capabilities": CAPABILITIES,
             "keys": {"uri_path": "jwks.json", "key_defs": KEYDEFS},
@@ -129,14 +128,15 @@
                 },
                 "introspection": {
                     "path": "{}/intro",
                     "class": Introspection,
                     "kwargs": {
                         "client_authn_method": ["client_secret_post"],
                         "enable_claims_per_client": False,
+                        "enforce_audience_restriction": True,
                     },
                 },
                 "token": {
                     "path": "token",
                     "class": Token,
                     "kwargs": {
                         "client_authn_method": [
@@ -201,15 +201,15 @@
             "response_types": ["code", "token", "code id_token", "id_token"],
             "add_claims": {
                 "always": {
                     "introspection": ["nickname", "eduperson_scoped_affiliation"],
                 },
                 "by_scope": {},
             },
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"]
+            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"],
         }
         server.keyjar.import_jwks_as_json(
             server.keyjar.export_jwks_as_json(private=True), context.issuer
         )
         self.introspection_endpoint = server.get_endpoint("introspection")
         self.token_endpoint = server.get_endpoint("token")
         self.session_manager = context.session_manager
@@ -262,24 +262,22 @@
                 "token": access_token.value,
                 "client_id": "client_1",
                 "client_secret": _context.cdb["client_1"]["client_secret"],
             }
         )
 
         assert isinstance(_req, TokenIntrospectionRequest)
-        assert set(_req.keys()) == {"token", "client_id", "client_secret", 'authenticated'}
+        assert set(_req.keys()) == {"token", "client_id", "client_secret", "authenticated"}
 
     def test_parse_with_wrong_client_authn(self):
         access_token = self._get_access_token(AUTH_REQ)
 
         _basic_token = "{}:{}".format(
             "client_1",
-            self.introspection_endpoint.upstream_get("context").cdb["client_1"][
-                "client_secret"
-            ],
+            self.introspection_endpoint.upstream_get("context").cdb["client_1"]["client_secret"],
         )
         _basic_token = as_unicode(base64.b64encode(as_bytes(_basic_token)))
         _basic_authz = "Basic {}".format(_basic_token)
         http_info = {"headers": {"authorization": _basic_authz}}
 
         with pytest.raises(ClientAuthenticationError):
             self.introspection_endpoint.parse_request(
```

### Comparing `idpyoidc-2.0.0/tests/test_server_32_oidc_read_registration.py` & `idpyoidc-2.1.0/tests/test_server_32_oidc_read_registration.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,14 @@
     "post_logout_redirect_uri": "https://rp.example.com/pl",
 }
 
 CLI_REQ = RegistrationRequest(**msg)
 
 
 class TestEndpoint(object):
-
     @pytest.fixture(autouse=True)
     def create_endpoint(self):
         conf = {
             "issuer": "https://example.com/",
             "httpc_params": {"verify": False, "timeout": 1},
             "token_handler_args": {
                 "code": {"lifetime": 600, "kwargs": {"crypt_conf": CRYPT_CONFIG}},
@@ -124,15 +123,17 @@
             },
             "template_dir": "template",
             "session_params": SESSION_PARAMS,
         }
         server = Server(OPConfiguration(conf=conf, base_path=BASEDIR), cwd=BASEDIR)
         self.registration_endpoint = server.get_endpoint("registration")
         self.registration_api_endpoint = server.get_endpoint("registration_read")
-        server.context.cdb["client_1"] = {}
+        server.context.cdb["client_1"] = {
+            "redirect_uris": [("https://example.com/cb", ""), ("https://example.com/2nd_cb", "")]
+        }
 
     def test_do_response(self):
         _req = self.registration_endpoint.parse_request(CLI_REQ.to_json())
         _resp = self.registration_endpoint.process_request(request=_req)
         msg = self.registration_endpoint.do_response(**_resp)
         assert isinstance(msg, dict)
         _msg = json.loads(msg["response"])
@@ -146,15 +147,15 @@
             }
         }
 
         _api_req = self.registration_api_endpoint.parse_request(
             "client_id={}".format(_resp["response_args"]["client_id"]),
             http_info=http_info,
         )
-        assert set(_api_req.keys()) == {"client_id", 'authenticated'}
+        assert set(_api_req.keys()) == {"client_id", "authenticated"}
 
         _info = self.registration_api_endpoint.process_request(request=_api_req)
         assert set(_info.keys()) == {"response_args"}
         assert _info["response_args"] == _resp["response_args"]
 
         _endp_response = self.registration_api_endpoint.do_response(_info)
         assert set(_endp_response.keys()) == {"response", "http_headers"}
```

### Comparing `idpyoidc-2.0.0/tests/test_server_33_oauth2_pkce.py` & `idpyoidc-2.1.0/tests/test_server_33_oauth2_pkce.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,18 @@
 from idpyoidc.message.oidc import AuthorizationRequest
 from idpyoidc.message.oidc import AuthorizationResponse
 from idpyoidc.message.oidc import TokenErrorResponse
 from idpyoidc.server import Server
 from idpyoidc.server.configure import ASConfiguration
 from idpyoidc.server.configure import OPConfiguration
 from idpyoidc.server.cookie_handler import CookieHandler
-from idpyoidc.server.oidc.add_on.pkce import CC_METHOD
-from idpyoidc.server.oidc.add_on.pkce import add_pkce_support
+from idpyoidc.server.oauth2.add_on.pkce import CC_METHOD
+from idpyoidc.server.oauth2.add_on.pkce import add_support
 from idpyoidc.server.oidc.authorization import Authorization
 from idpyoidc.server.oidc.token import Token
-
 from . import CRYPT_CONFIG
 from . import SESSION_PARAMS
 from . import full_path
 
 BASECH = string.ascii_letters + string.digits + "-._~"
 
 KEYDEFS = [
@@ -89,18 +88,16 @@
     "client_secret": 'hemligt'
     "redirect_uris":
         - ['https://example.com/cb', '']
     "client_salt": "salted"
     'token_endpoint_auth_method': 'client_secret_post'
     'response_types':
         - 'code'
-        - 'token'
         - 'code id_token'
         - 'id_token'
-        - 'code id_token token'
     allowed_scopes:
         - 'openid'
         - 'profile'
         - 'email'
         - 'address'
         - 'phone'
         - 'offline_access'
@@ -168,15 +165,15 @@
                 "class": "idpyoidc.server.user_authn.user.NoAuthn",
                 "kwargs": {"user": "diana"},
             }
         },
         "template_dir": "template",
         "add_on": {
             "pkce": {
-                "function": "idpyoidc.server.oidc.add_on.pkce.add_pkce_support",
+                "function": "idpyoidc.server.oauth2.add_on.pkce.add_support",
                 "kwargs": {"essential": True},
             }
         },
         "cookie_handler": {
             "class": CookieHandler,
             "kwargs": {
                 "sign_key": "ghsNKDDLshZTPn974nOsIGhedULrsqnsGoBFBLwUKuJhE2ch",
@@ -414,15 +411,15 @@
                 "class": "idpyoidc.server.oauth2.introspection.Introspection",
                 "kwargs": {},
             }
         },
     }
     configuration = OPConfiguration(conf, base_path=BASEDIR, domain="127.0.0.1", port=443)
     server = Server(configuration)
-    add_pkce_support(server.get_endpoints())
+    add_support(server.get_endpoints())
 
     assert "pkce" not in server.get_context().args
 
 
 def test_missing_token_endpoint():
     conf = {
         "issuer": "https://example.com/",
@@ -439,10 +436,10 @@
                 "class": "idpyoidc.server.oauth2.introspection.Introspection",
                 "kwargs": {},
             },
         },
     }
     configuration = OPConfiguration(conf, base_path=BASEDIR, domain="127.0.0.1", port=443)
     server = Server(configuration)
-    add_pkce_support(server.get_endpoints())
+    add_support(server.get_endpoints())
 
     assert "pkce" not in server.get_context().args
```

### Comparing `idpyoidc-2.0.0/tests/test_server_34_oidc_sso.py` & `idpyoidc-2.1.0/tests/test_server_34_oidc_sso.py`

 * *Files 3% similar despite different names*

```diff
@@ -195,17 +195,15 @@
             "session_params": SESSION_PARAMS,
         }
         server = Server(OPConfiguration(conf=conf, base_path=BASEDIR), cwd=BASEDIR)
 
         context = server.context
         _clients = yaml.safe_load(io.StringIO(client_yaml))
         context.cdb = _clients["oidc_clients"]
-        server.keyjar.import_jwks(
-            server.keyjar.export_jwks(True, ""), conf["issuer"]
-        )
+        server.keyjar.import_jwks(server.keyjar.export_jwks(True, ""), conf["issuer"])
         self.endpoint = server.get_endpoint("authorization")
         self.context = context
         self.rp_keyjar = KeyJar()
         self.rp_keyjar.add_symmetric("client_1", "hemligtkodord1234567890")
         server.keyjar.add_symmetric("client_1", "hemligtkodord1234567890")
 
     def test_sso(self):
@@ -268,33 +266,25 @@
         request = self.endpoint.parse_request(AUTH_REQ_2.to_dict())
         redirect_uri = request["redirect_uri"]
         cinfo = self.endpoint.upstream_get("context").cdb[request["client_id"]]
         info = self.endpoint.setup_auth(request, redirect_uri, cinfo, cookie=kakor)
         # No valid login cookie so new session
         assert info["session_id"] != sid2
 
-        user_session_info = self.endpoint.upstream_get("context").session_manager.get(
-            ["diana"]
-        )
+        user_session_info = self.endpoint.upstream_get("context").session_manager.get(["diana"])
         assert len(user_session_info.subordinate) == 3
         assert set(user_session_info.subordinate) == {
             "diana;;client_1",
             "diana;;client_2",
             "diana;;client_3",
         }
 
         # Should be one grant for each of client_2 and client_3 and
         # 2 grants for client_1
 
-        csi1 = self.endpoint.upstream_get("context").session_manager.get(
-            ["diana", "client_1"]
-        )
-        csi2 = self.endpoint.upstream_get("context").session_manager.get(
-            ["diana", "client_2"]
-        )
-        csi3 = self.endpoint.upstream_get("context").session_manager.get(
-            ["diana", "client_3"]
-        )
+        csi1 = self.endpoint.upstream_get("context").session_manager.get(["diana", "client_1"])
+        csi2 = self.endpoint.upstream_get("context").session_manager.get(["diana", "client_2"])
+        csi3 = self.endpoint.upstream_get("context").session_manager.get(["diana", "client_3"])
 
         assert len(csi1.subordinate) == 2
         assert len(csi2.subordinate) == 1
         assert len(csi3.subordinate) == 2
```

### Comparing `idpyoidc-2.0.0/tests/test_server_35_oidc_token_endpoint.py` & `idpyoidc-2.1.0/tests/test_server_35_oidc_token_endpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,27 +194,26 @@
             },
         },
         "session_params": SESSION_PARAMS,
     }
 
 
 class TestEndpoint(_TestEndpoint):
-
     @pytest.fixture(autouse=True)
     def create_endpoint(self, conf):
         self.server = Server(OPConfiguration(conf=conf, base_path=BASEDIR), cwd=BASEDIR)
 
         context = self.server.context
         context.cdb["client_1"] = {
             "client_secret": "hemligt",
             "redirect_uris": [("https://example.com/cb", None)],
             "client_salt": "salted",
             "endpoint_auth_method": "client_secret_post",
             "response_types": ["code", "token", "code id_token", "id_token"],
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"]
+            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"],
         }
         self.server.keyjar.import_jwks(CLIENT_KEYJAR.export_jwks(), "client_1")
         context.userinfo = USERINFO
         self.session_manager = context.session_manager
         self.token_endpoint = self.server.get_endpoint("token")
         self.user_id = "diana"
         self.context = context
@@ -280,15 +279,15 @@
         grant = self.session_manager[session_id]
         code = self._mint_code(grant, AUTH_REQ["client_id"])
 
         _token_request = TOKEN_REQ_DICT.copy()
         _token_request["code"] = code.value
         _req = self.token_endpoint.parse_request(_token_request)
 
-        assert set(_req.keys()).difference(set(_token_request.keys())) == {'authenticated'}
+        assert set(_req.keys()).difference(set(_token_request.keys())) == {"authenticated"}
 
     def test_process_request(self):
         session_id = self._create_session(AUTH_REQ)
         grant = self.session_manager[session_id]
         code = self._mint_code(grant, AUTH_REQ["client_id"])
 
         _token_request = TOKEN_REQ_DICT.copy()
@@ -390,15 +389,15 @@
             "token_type",
             "expires_in",
             "refresh_token",
             "id_token",
             "scope",
         }
         AuthorizationResponse().from_jwt(
-            _resp["response_args"]["id_token"], self.server.get_attribute('keyjar'), sender=""
+            _resp["response_args"]["id_token"], self.server.get_attribute("keyjar"), sender=""
         )
 
         msg = self.token_endpoint.do_response(request=_req, **_resp)
         assert isinstance(msg, dict)
 
     def test_do_2nd_refresh_access_token(self):
         areq = AUTH_REQ.copy()
@@ -770,15 +769,15 @@
     def test_new_refresh_token(self, conf):
         self.context.cdb["client_1"] = {
             "client_secret": "hemligt",
             "redirect_uris": [("https://example.com/cb", None)],
             "client_salt": "salted",
             "endpoint_auth_method": "client_secret_post",
             "response_types": ["code", "token", "code id_token", "id_token"],
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"]
+            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"],
         }
 
         areq = AUTH_REQ.copy()
         areq["scope"] = ["openid", "offline_access"]
 
         session_id = self._create_session(areq)
         grant = self.context.authz(session_id, areq)
@@ -810,15 +809,15 @@
     def test_revoke_on_issue_refresh_token(self, conf):
         self.context.cdb["client_1"] = {
             "client_secret": "hemligt",
             "redirect_uris": [("https://example.com/cb", None)],
             "client_salt": "salted",
             "endpoint_auth_method": "client_secret_post",
             "response_types": ["code", "token", "code id_token", "id_token"],
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"]
+            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"],
         }
         self.token_endpoint.revoke_refresh_on_issue = True
         areq = AUTH_REQ.copy()
         areq["scope"] = ["openid", "offline_access"]
 
         session_id = self._create_session(areq)
         grant = self.context.authz(session_id, areq)
@@ -850,15 +849,15 @@
     def test_revoke_on_issue_refresh_token_per_client(self, conf):
         self.context.cdb["client_1"] = {
             "client_secret": "hemligt",
             "redirect_uris": [("https://example.com/cb", None)],
             "client_salt": "salted",
             "endpoint_auth_method": "client_secret_post",
             "response_types": ["code", "token", "code id_token", "id_token"],
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"]
+            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"],
         }
         self.context.cdb[AUTH_REQ["client_id"]]["revoke_refresh_on_issue"] = True
         areq = AUTH_REQ.copy()
         areq["scope"] = ["openid", "offline_access"]
 
         session_id = self._create_session(areq)
         grant = self.context.authz(session_id, areq)
@@ -934,16 +933,17 @@
         _req = self.token_endpoint.parse_request(_request.to_urlencoded())
         # A revoked token is caught already when parsing the query.
         assert isinstance(_req, TokenErrorResponse)
 
     def test_configure_grant_types(self):
         conf = {"access_token": {"class": "idpyoidc.server.oidc.token.AccessTokenHelper"}}
 
-        _helper = self.token_endpoint.configure_types(conf,
-                                                      self.token_endpoint.helper_by_grant_type)
+        _helper = self.token_endpoint.configure_types(
+            conf, self.token_endpoint.helper_by_grant_type
+        )
 
         assert len(_helper) == 1
         assert "access_token" in _helper
         assert "refresh_token" not in _helper
 
     def test_access_token_lifetime(self):
         lifetime = 100
@@ -1011,27 +1011,26 @@
             request=_req,
         )
         assert isinstance(_resp, TokenErrorResponse)
         assert _resp.to_dict() == {"error": "invalid_grant", "error_description": "Wrong client"}
 
 
 class TestOldTokens(object):
-
     @pytest.fixture(autouse=True)
     def create_endpoint(self, conf):
         server = Server(OPConfiguration(conf=conf, base_path=BASEDIR), cwd=BASEDIR)
 
         context = server.context
         context.cdb["client_1"] = {
             "client_secret": "hemligt",
             "redirect_uris": [("https://example.com/cb", None)],
             "client_salt": "salted",
             "endpoint_auth_method": "client_secret_post",
             "response_types": ["code", "token", "code id_token", "id_token"],
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"]
+            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"],
         }
         server.keyjar.import_jwks(CLIENT_KEYJAR.export_jwks(), "client_1")
         self.session_manager = context.session_manager
         self.token_endpoint = server.get_endpoint("token")
         self.user_id = "diana"
         self.context = context
 
@@ -1117,15 +1116,15 @@
 
         payload = {"sid": session_id, "ttype": "T"}
         payload = _handler.load_custom_claims(payload)
 
         # payload.update(kwargs)
         _context = _handler.upstream_get("context")
         signer = JWT(
-            key_jar=_handler.upstream_get('attribute', 'keyjar'),
+            key_jar=_handler.upstream_get("attribute", "keyjar"),
             iss=_handler.issuer,
             lifetime=300,
             sign_alg=_handler.alg,
         )
 
         _old_type_token = signer.pack(payload)
```

### Comparing `idpyoidc-2.0.0/tests/test_server_36_oauth2_token_exchange.py` & `idpyoidc-2.1.0/tests/test_server_36_oauth2_token_exchange.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,15 +182,15 @@
             "redirect_uris": [("https://example.com/cb", None)],
             "client_salt": "salted",
             "token_endpoint_auth_method": "client_secret_post",
             "grant_types_supported": [
                 "authorization_code",
                 "urn:ietf:params:oauth:grant-type:jwt-bearer",
                 "refresh_token",
-                "urn:ietf:params:oauth:grant-type:token-exchange"
+                "urn:ietf:params:oauth:grant-type:token-exchange",
             ],
             "response_types": ["code", "token", "code id_token", "id_token"],
             "allowed_scopes": ["openid", "profile", "offline_access"],
         }
         self.context.cdb["client_2"] = {
             "client_secret": "hemligt",
             "redirect_uris": [("https://example.com/cb", None)],
@@ -263,23 +263,23 @@
         _req = self.endpoint.parse_request(_token_request)
         _resp = self.endpoint.process_request(request=_req)
         _token_value = _resp["response_args"][list(token.keys())[0]]
 
         token_exchange_req = TokenExchangeRequest(
             grant_type="urn:ietf:params:oauth:grant-type:token-exchange",
             subject_token=_token_value,
-            subject_token_type=token[list(token.keys())[0]]
+            subject_token_type=token[list(token.keys())[0]],
         )
 
         _req = self.endpoint.parse_request(
             token_exchange_req.to_urlencoded(),
             {"headers": {"authorization": "Basic {}".format("Y2xpZW50XzI6aGVtbGlndA==")}},
         )
         _resp = self.endpoint.process_request(request=_req)
-        print(_resp['response_args'])
+        print(_resp["response_args"])
         assert set(_resp["response_args"].keys()) == {
             "access_token",
             "token_type",
             "scope",
             "expires_in",
             "issued_token_type",
         }
@@ -407,22 +407,25 @@
                 "urn:ietf:params:oauth:token-type:access_token",
                 "urn:ietf:params:oauth:token-type:refresh_token",
             ],
             "default_requested_token_type": "urn:ietf:params:oauth:token-type:access_token",
             "policy": {
                 "": {
                     "function": "idpyoidc.server.oauth2.token_helper.validate_token_exchange_policy",
-                    "kwargs": {
-                        "scope": ["openid", "profile", "offline_access"]
-                    },
+                    "kwargs": {"scope": ["openid", "profile", "offline_access"]},
                 }
             },
         }
 
-        self.context.cdb["client_1"]["allowed_scopes"] = ["openid", "email", "profile", "offline_access"]
+        self.context.cdb["client_1"]["allowed_scopes"] = [
+            "openid",
+            "email",
+            "profile",
+            "offline_access",
+        ]
 
         areq = AUTH_REQ.copy()
         areq["scope"].append("profile")
 
         session_id = self._create_session(areq)
         grant = self.context.authz(session_id, areq)
 
@@ -436,15 +439,15 @@
         _token_value = _resp["response_args"]["access_token"]
 
         token_exchange_req = TokenExchangeRequest(
             grant_type="urn:ietf:params:oauth:grant-type:token-exchange",
             subject_token=_token_value,
             subject_token_type="urn:ietf:params:oauth:token-type:access_token",
             requested_token_type="urn:ietf:params:oauth:token-type:access_token",
-            scope="openid profile offline_access"
+            scope="openid profile offline_access",
         )
 
         _req = self.endpoint.parse_request(
             token_exchange_req.to_urlencoded(),
             {"headers": {"authorization": "Basic {}".format("Y2xpZW50XzE6aGVtbGlndA==")}},
         )
         _resp = self.endpoint.process_request(request=_req)
@@ -465,20 +468,18 @@
                 "urn:ietf:params:oauth:token-type:access_token",
                 "urn:ietf:params:oauth:token-type:refresh_token",
             ],
             "default_requested_token_type": "urn:ietf:params:oauth:token-type:access_token",
             "policy": {
                 "": {
                     "function": "idpyoidc.server.oauth2.token_helper.validate_token_exchange_policy",
-                    "kwargs": {
-                        "scope": ["openid", "profile", "offline_access"]
-                    },
+                    "kwargs": {"scope": ["openid", "profile", "offline_access"]},
                 }
             },
-            "allowed_scopes": ["openid", "email", "profile", "offline_access"]
+            "allowed_scopes": ["openid", "email", "profile", "offline_access"],
         }
 
         areq = AUTH_REQ.copy()
         areq["scope"].append("profile")
 
         session_id = self._create_session(areq)
         grant = self.context.authz(session_id, areq)
@@ -492,15 +493,15 @@
         _token_value = _resp["response_args"]["access_token"]
 
         token_exchange_req = TokenExchangeRequest(
             grant_type="urn:ietf:params:oauth:grant-type:token-exchange",
             subject_token=_token_value,
             subject_token_type="urn:ietf:params:oauth:token-type:access_token",
             requested_token_type="urn:ietf:params:oauth:token-type:access_token",
-            scope="email"
+            scope="email",
         )
 
         _req = self.endpoint.parse_request(
             token_exchange_req.to_urlencoded(),
             {"headers": {"authorization": "Basic {}".format("Y2xpZW50XzE6aGVtbGlndA==")}},
         )
         _resp = self.endpoint.process_request(request=_req)
@@ -519,20 +520,18 @@
                 "urn:ietf:params:oauth:token-type:access_token",
                 "urn:ietf:params:oauth:token-type:refresh_token",
             ],
             "default_requested_token_type": "urn:ietf:params:oauth:token-type:access_token",
             "policy": {
                 "": {
                     "function": "idpyoidc.server.oauth2.token_helper.validate_token_exchange_policy",
-                    "kwargs": {
-                        "scope": ["openid", "offline_access"]
-                    },
+                    "kwargs": {"scope": ["openid", "offline_access"]},
                 }
             },
-            "allowed_scopes": ["openid", "email", "profile", "offline_access"]
+            "allowed_scopes": ["openid", "email", "profile", "offline_access"],
         }
 
         areq = AUTH_REQ.copy()
         areq["scope"].append("profile")
 
         session_id = self._create_session(areq)
         grant = self.context.authz(session_id, areq)
@@ -545,30 +544,32 @@
 
         _token_value = _resp["response_args"]["access_token"]
 
         token_exchange_req = TokenExchangeRequest(
             grant_type="urn:ietf:params:oauth:grant-type:token-exchange",
             subject_token=_token_value,
             subject_token_type="urn:ietf:params:oauth:token-type:access_token",
-            requested_token_type="urn:ietf:params:oauth:token-type:access_token"
+            requested_token_type="urn:ietf:params:oauth:token-type:access_token",
         )
 
         _req = self.endpoint.parse_request(
             token_exchange_req.to_urlencoded(),
             {"headers": {"authorization": "Basic {}".format("Y2xpZW50XzE6aGVtbGlndA==")}},
         )
         _resp = self.endpoint.process_request(request=_req)
         assert _resp["response_args"]["scope"] == ["openid"]
 
     def test_additional_parameters(self):
         """
         Test that a token exchange with additional parameters including
         scope, audience and subject_token_type works.
         """
-        conf = self.endpoint.grant_type_helper["urn:ietf:params:oauth:grant-type:token-exchange"].config
+        conf = self.endpoint.grant_type_helper[
+            "urn:ietf:params:oauth:grant-type:token-exchange"
+        ].config
         conf["policy"][""]["kwargs"] = {}
         conf["policy"][""]["kwargs"]["audience"] = ["https://example.com"]
         conf["policy"][""]["kwargs"]["resource"] = ["https://example.com"]
 
         areq = AUTH_REQ.copy()
 
         session_id = self._create_session(areq)
@@ -608,18 +609,18 @@
 
     def test_token_exchange_fails_if_disabled(self):
         """
         Test that token exchange fails if it's not included in Token's
         grant_types_supported (that are set in its helper attribute).
         """
         self.context.cdb["client_1"]["grant_types_supported"] = [
-            'authorization_code',
-            'implicit',
-            'urn:ietf:params:oauth:grant-type:jwt-bearer',
-            'refresh_token'
+            "authorization_code",
+            "implicit",
+            "urn:ietf:params:oauth:grant-type:jwt-bearer",
+            "refresh_token",
         ]
 
         areq = AUTH_REQ.copy()
 
         session_id = self._create_session(areq)
         grant = self.context.authz(session_id, areq)
         code = self._mint_code(grant, areq["client_id"])
@@ -641,23 +642,25 @@
         _req = self.endpoint.parse_request(
             token_exchange_req.to_urlencoded(),
             {"headers": {"authorization": "Basic {}".format("Y2xpZW50XzE6aGVtbGlndA==")}},
         )
         _resp = self.endpoint.process_request(request=_req)
         assert _resp["error"] == "invalid_request"
         assert (
-                _resp["error_description"]
-                == "Unsupported grant_type: urn:ietf:params:oauth:grant-type:token-exchange"
+            _resp["error_description"]
+            == "Unsupported grant_type: urn:ietf:params:oauth:grant-type:token-exchange"
         )
 
     def test_wrong_resource(self):
         """
         Test that requesting a token for an unknown resource fails.
         """
-        conf = self.endpoint.grant_type_helper["urn:ietf:params:oauth:grant-type:token-exchange"].config
+        conf = self.endpoint.grant_type_helper[
+            "urn:ietf:params:oauth:grant-type:token-exchange"
+        ].config
         conf["policy"][""]["kwargs"] = {}
         conf["policy"][""]["kwargs"]["resource"] = ["https://example.com"]
         areq = AUTH_REQ.copy()
 
         session_id = self._create_session(areq)
         grant = self.context.authz(session_id, areq)
         code = self._mint_code(grant, areq["client_id"])
@@ -719,15 +722,17 @@
         assert _resp["error"] == "invalid_target"
         assert _resp["error_description"] == "Refresh token has single owner"
 
     def test_wrong_audience(self):
         """
         Test that requesting a token for an unknown audience fails.
         """
-        conf = self.endpoint.grant_type_helper["urn:ietf:params:oauth:grant-type:token-exchange"].config
+        conf = self.endpoint.grant_type_helper[
+            "urn:ietf:params:oauth:grant-type:token-exchange"
+        ].config
         conf["policy"][""]["kwargs"] = {}
         conf["policy"][""]["kwargs"]["audience"] = ["https://example.com"]
         areq = AUTH_REQ.copy()
 
         session_id = self._create_session(areq)
         grant = self.context.authz(session_id, areq)
         code = self._mint_code(grant, areq["client_id"])
@@ -1038,17 +1043,15 @@
                 "urn:ietf:params:oauth:token-type:access_token",
                 "urn:ietf:params:oauth:token-type:refresh_token",
             ],
             "default_requested_token_type": "urn:ietf:params:oauth:token-type:access_token",
             "policy": {
                 "": {
                     "function": "idpyoidc.server.oauth2.token_helper.validate_token_exchange_policy",
-                    "kwargs": {
-                        "scope": ["offline_access", "profile"]
-                    },
+                    "kwargs": {"scope": ["offline_access", "profile"]},
                 }
             },
         }
 
         areq = AUTH_REQ.copy()
         areq["scope"].append("profile")
         areq["scope"].append("offline_access")
@@ -1127,17 +1130,15 @@
                 "urn:ietf:params:oauth:token-type:access_token",
                 "urn:ietf:params:oauth:token-type:refresh_token",
             ],
             "default_requested_token_type": "urn:ietf:params:oauth:token-type:access_token",
             "policy": {
                 "": {
                     "function": "idpyoidc.server.oauth2.token_helper.validate_token_exchange_policy",
-                    "kwargs": {
-                        "scope": ["profile"]
-                    },
+                    "kwargs": {"scope": ["profile"]},
                 }
             },
         }
         self.context.cdb["client_1"]["allowed_scopes"] = ["openid", "profile"]
 
         areq = AUTH_REQ.copy()
         areq["scope"].append("profile")
@@ -1215,25 +1216,23 @@
                 "urn:ietf:params:oauth:token-type:access_token",
                 "urn:ietf:params:oauth:token-type:refresh_token",
             ],
             "default_requested_token_type": "urn:ietf:params:oauth:token-type:access_token",
             "policy": {
                 "": {
                     "function": "idpyoidc.server.oauth2.token_helper.validate_token_exchange_policy",
-                    "kwargs": {
-                        "scope": ["offline_access", "profile"]
-                    },
+                    "kwargs": {"scope": ["offline_access", "profile"]},
                 }
             },
         }
         self.context.cdb["client_1"]["grant_types_supported"] = [
-            'authorization_code',
-            'implicit',
-            'urn:ietf:params:oauth:grant-type:jwt-bearer',
-            'urn:ietf:params:oauth:grant-type:token-exchange'
+            "authorization_code",
+            "implicit",
+            "urn:ietf:params:oauth:grant-type:jwt-bearer",
+            "urn:ietf:params:oauth:grant-type:token-exchange",
         ]
 
         areq = AUTH_REQ.copy()
         areq["scope"].append("profile")
         areq["scope"].append("offline_access")
 
         session_id = self._create_session(areq)
@@ -1323,25 +1322,23 @@
                 "urn:ietf:params:oauth:token-type:access_token",
                 "urn:ietf:params:oauth:token-type:refresh_token",
             ],
             "default_requested_token_type": "urn:ietf:params:oauth:token-type:access_token",
             "policy": {
                 "": {
                     "function": "idpyoidc.server.oauth2.token_helper.validate_token_exchange_policy",
-                    "kwargs": {
-                        "scope": ["offline_access", "profile"]
-                    },
+                    "kwargs": {"scope": ["offline_access", "profile"]},
                 }
             },
         }
         self.context.cdb["client_1"]["grant_types_supported"] = [
-            'authorization_code',
-            'implicit',
-            'urn:ietf:params:oauth:grant-type:jwt-bearer',
-            'urn:ietf:params:oauth:grant-type:token-exchange'
+            "authorization_code",
+            "implicit",
+            "urn:ietf:params:oauth:grant-type:jwt-bearer",
+            "urn:ietf:params:oauth:grant-type:token-exchange",
         ]
 
         areq = AUTH_REQ.copy()
         areq["scope"].append("profile")
         areq["scope"].append("offline_access")
 
         session_id = self._create_session(areq)
@@ -1373,16 +1370,15 @@
         _req = self.endpoint.parse_request(
             token_exchange_req.to_urlencoded(),
             {"headers": {"authorization": "Basic {}".format("Y2xpZW50XzE6aGVtbGlndA==")}},
         )
         _resp = self.endpoint.process_request(request=_req)
         assert _resp["error"] == "invalid_request"
         assert (
-                _resp["error_description"]
-                == "Exchanging this subject token to refresh token forbidden"
+            _resp["error_description"] == "Exchanging this subject token to refresh token forbidden"
         )
 
         token_exchange_req["scope"] = "offline_access"
 
         _req = self.endpoint.parse_request(
             token_exchange_req.to_urlencoded(),
             {"headers": {"authorization": "Basic {}".format("Y2xpZW50XzE6aGVtbGlndA==")}},
@@ -1421,17 +1417,15 @@
                 "urn:ietf:params:oauth:token-type:access_token",
                 "urn:ietf:params:oauth:token-type:refresh_token",
             ],
             "default_requested_token_type": "urn:ietf:params:oauth:token-type:access_token",
             "policy": {
                 "": {
                     "function": "idpyoidc.server.oauth2.token_helper.validate_token_exchange_policy",
-                    "kwargs": {
-                        "scope": ["profile"]
-                    },
+                    "kwargs": {"scope": ["profile"]},
                 }
             },
         }
 
         areq = AUTH_REQ.copy()
         areq["scope"].append("profile")
         areq["scope"].append("offline_access")
@@ -1456,50 +1450,43 @@
         _req = self.endpoint.parse_request(
             token_exchange_req.to_urlencoded(),
             {"headers": {"authorization": "Basic {}".format("Y2xpZW50XzE6aGVtbGlndA==")}},
         )
         _resp = self.endpoint.process_request(request=_req)
         assert _resp["error"] == "invalid_request"
         assert (
-                _resp["error_description"]
-                == "Exchanging this subject token to refresh token forbidden"
+            _resp["error_description"] == "Exchanging this subject token to refresh token forbidden"
         )
 
         token_exchange_req["scope"] = "profile"
 
         _req = self.endpoint.parse_request(
             token_exchange_req.to_urlencoded(),
             {"headers": {"authorization": "Basic {}".format("Y2xpZW50XzE6aGVtbGlndA==")}},
         )
         _resp = self.endpoint.process_request(request=_req)
         assert _resp["error"] == "invalid_request"
         assert (
-                _resp["error_description"]
-                == "Exchanging this subject token to refresh token forbidden"
+            _resp["error_description"] == "Exchanging this subject token to refresh token forbidden"
         )
 
         token_exchange_req["scope"] = "offline_access"
 
         _req = self.endpoint.parse_request(
             token_exchange_req.to_urlencoded(),
             {"headers": {"authorization": "Basic {}".format("Y2xpZW50XzE6aGVtbGlndA==")}},
         )
         _resp = self.endpoint.process_request(request=_req)
         assert _resp["error"] == "invalid_scope"
-        assert (
-                _resp["error_description"]
-                == "Invalid requested scopes"
-        )
+        assert _resp["error_description"] == "Invalid requested scopes"
 
         token_exchange_req["scope"] = "offline_access profile"
 
         _req = self.endpoint.parse_request(
             token_exchange_req.to_urlencoded(),
             {"headers": {"authorization": "Basic {}".format("Y2xpZW50XzE6aGVtbGlndA==")}},
         )
         _resp = self.endpoint.process_request(request=_req)
         assert _resp["error"] == "invalid_request"
         assert (
-                _resp["error_description"]
-                == "Exchanging this subject token to refresh token forbidden"
+            _resp["error_description"] == "Exchanging this subject token to refresh token forbidden"
         )
-
```

### Comparing `idpyoidc-2.0.0/tests/test_server_38_oauth2_revocation_endpoint.py` & `idpyoidc-2.1.0/tests/test_server_38_oauth2_revocation_endpoint.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,21 +29,16 @@
 KEYDEFS = [
     {"type": "RSA", "key": "", "use": ["sig"]},
     {"type": "EC", "crv": "P-256", "use": ["sig"]},
 ]
 
 RESPONSE_TYPES_SUPPORTED = [
     ["code"],
-    ["token"],
     ["id_token"],
-    ["code", "token"],
     ["code", "id_token"],
-    ["id_token", "token"],
-    ["code", "token", "id_token"],
-    ["none"],
 ]
 
 CAPABILITIES = {
     "response_types_supported": [" ".join(x) for x in RESPONSE_TYPES_SUPPORTED],
     "token_endpoint_auth_methods_supported": [
         "client_secret_post",
         "client_secret_basic",
@@ -57,15 +52,15 @@
         "implicit",
         "urn:ietf:params:oauth:grant-type:jwt-bearer",
         "refresh_token",
     ],
     "claim_types_supported": ["normal", "aggregated", "distributed"],
     "claims_parameter_supported": True,
     "request_parameter_supported": True,
-    "request_uri_parameter_supported": True,
+    # "request_uri_parameter_supported": True,
 }
 
 AUTH_REQ = AuthorizationRequest(
     client_id="client_1",
     redirect_uri="https://example.com/cb",
     scope=["openid", "offline_access"],
     state="STATE",
@@ -87,15 +82,14 @@
 
 def full_path(local_file):
     return os.path.join(BASEDIR, local_file)
 
 
 @pytest.mark.parametrize("jwt_token", [True, False])
 class TestEndpoint:
-
     @pytest.fixture(autouse=True)
     def create_endpoint(self, jwt_token):
         conf = {
             "issuer": "https://example.com/",
             "httpc_params": {"verify": False, "timeout": 1},
             "capabilities": CAPABILITIES,
             "keys": {"uri_path": "jwks.json", "key_defs": KEYDEFS},
@@ -208,16 +202,23 @@
             "response_types": ["code", "token", "code id_token", "id_token"],
             "add_claims": {
                 "always": {
                     "introspection": ["nickname", "eduperson_scoped_affiliation"],
                 },
                 "by_scope": {},
             },
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access",
-                               "research_and_scholarship"]
+            "allowed_scopes": [
+                "openid",
+                "profile",
+                "email",
+                "address",
+                "phone",
+                "offline_access",
+                "research_and_scholarship",
+            ],
         }
         endpoint_context.keyjar.import_jwks_as_json(
             endpoint_context.keyjar.export_jwks_as_json(private=True),
             endpoint_context.issuer,
         )
         self.revocation_endpoint = server.get_endpoint("token_revocation")
         self.token_endpoint = server.get_endpoint("token")
@@ -280,15 +281,15 @@
                 "token": access_token.value,
                 "client_id": "client_1",
                 "client_secret": _context.cdb["client_1"]["client_secret"],
             }
         )
 
         assert isinstance(_req, TokenRevocationRequest)
-        assert set(_req.keys()) == {"token", "client_id", "client_secret", 'authenticated'}
+        assert set(_req.keys()) == {"token", "client_id", "client_secret", "authenticated"}
 
     def test_parse_with_wrong_client_authn(self):
         access_token = self._get_access_token(AUTH_REQ)
 
         _basic_token = "{}:{}".format(
             "client_1",
             self.revocation_endpoint.upstream_get("endpoint_context").cdb["client_1"][
@@ -314,15 +315,15 @@
                 "client_secret": self.revocation_endpoint.upstream_get("endpoint_context").cdb[
                     "client_1"
                 ]["client_secret"],
             }
         )
         _resp = self.revocation_endpoint.process_request(_req)
         assert _resp
-        assert set(_resp.keys()) == {"response_args"}
+        assert set(_resp.keys()) == {"response_msg"}
 
     def test_do_response(self):
         access_token = self._get_access_token(AUTH_REQ)
 
         _req = self.revocation_endpoint.parse_request(
             {
                 "token": access_token.value,
@@ -333,15 +334,15 @@
             }
         )
         _resp = self.revocation_endpoint.process_request(_req)
         msg_info = self.revocation_endpoint.do_response(request=_req, **_resp)
         assert isinstance(msg_info, dict)
         assert set(msg_info.keys()) == {"response", "http_headers"}
         assert msg_info["http_headers"] == [
-            ("Content-type", "application/json; charset=utf-8"),
+            ("Content-type", "text/plain"),
             ("Pragma", "no-cache"),
             ("Cache-Control", "no-store"),
         ]
 
     def test_do_response_no_token(self):
         # access_token = self._get_access_token(AUTH_REQ)
         _context = self.revocation_endpoint.upstream_get("endpoint_context")
@@ -362,56 +363,54 @@
             {
                 "token": access_token.value,
                 "client_id": "client_1",
                 "client_secret": _context.cdb["client_1"]["client_secret"],
             }
         )
         _resp = self.revocation_endpoint.process_request(_req)
-        assert "response_args" in _resp
+        assert "response_msg" in _resp
         assert access_token.revoked
 
     def test_access_token_per_client(self):
-
         def custom_token_revocation_policy(token, session_info, **kwargs):
             _token = token
             _token.revoke()
-            response_args = {"response_args": {"type": "custom"}}
-            return TokenRevocationResponse(**response_args)
+            # response_args = {"response_args": {"type": "custom"}}
+            # return TokenRevocationResponse(**response_args)
+            return {"response_msg": "OK"}
 
         access_token = self._get_access_token(AUTH_REQ)
         assert access_token.revoked is False
         _context = self.revocation_endpoint.upstream_get("endpoint_context")
         _context.cdb["client_1"]["token_revocation"] = {
             "token_types_supported": [
                 "access_token",
             ],
             "policy": {
                 "": {
                     "function": validate_token_revocation_policy,
                 },
                 "access_token": {
                     "function": custom_token_revocation_policy,
-                }
+                },
             },
         }
         _req = self.revocation_endpoint.parse_request(
             {
                 "token": access_token.value,
                 "client_id": "client_1",
                 "client_secret": _context.cdb["client_1"]["client_secret"],
             }
         )
         _resp = self.revocation_endpoint.process_request(_req)
-        assert "response_args" in _resp
-        assert "type" in _resp["response_args"]
-        assert _resp["response_args"]["type"] == "custom"
+        assert "response_msg" in _resp
+        assert _resp["response_msg"] == "OK"
         assert access_token.revoked
 
     def test_missing_token_policy_per_client(self):
-
         def custom_token_revocation_policy(token, session_info, **kwargs):
             _token = token
             _token.revoke()
             response_args = {"response_args": {"type": "custom"}}
             return TokenRevocationResponse(**response_args)
 
         access_token = self._get_access_token(AUTH_REQ)
@@ -423,26 +422,26 @@
             ],
             "policy": {
                 "": {
                     "function": validate_token_revocation_policy,
                 },
                 "refresh_token": {
                     "function": custom_token_revocation_policy,
-                }
+                },
             },
         }
         _req = self.revocation_endpoint.parse_request(
             {
                 "token": access_token.value,
                 "client_id": "client_1",
                 "client_secret": _context.cdb["client_1"]["client_secret"],
             }
         )
         _resp = self.revocation_endpoint.process_request(_req)
-        assert "response_args" in _resp
+        assert "response_msg" in _resp
         assert access_token.revoked
 
     def test_code(self):
         session_id = self._create_session(AUTH_REQ)
 
         # Apply consent
         grant = self.token_endpoint.upstream_get("endpoint_context").authz(session_id, AUTH_REQ)
@@ -456,30 +455,30 @@
             {
                 "token": code.value,
                 "client_id": "client_1",
                 "client_secret": _context.cdb["client_1"]["client_secret"],
             }
         )
         _resp = self.revocation_endpoint.process_request(_req)
-        assert "response_args" in _resp
+        assert "response_msg" in _resp
         assert code.revoked
 
     def test_refresh_token(self):
         refresh_token = self._get_refresh_token(AUTH_REQ)
         assert refresh_token.revoked is False
         _context = self.revocation_endpoint.upstream_get("endpoint_context")
         _req = self.revocation_endpoint.parse_request(
             {
                 "token": refresh_token.value,
                 "client_id": "client_1",
                 "client_secret": _context.cdb["client_1"]["client_secret"],
             }
         )
         _resp = self.revocation_endpoint.process_request(_req)
-        assert "response_args" in _resp
+        assert "response_msg" in _resp
         assert refresh_token.revoked
 
     def test_expired_access_token(self):
         access_token = self._get_access_token(AUTH_REQ)
         access_token.expires_at = utc_time_sans_frac() - 1000
 
         _context = self.revocation_endpoint.upstream_get("endpoint_context")
@@ -488,15 +487,15 @@
             {
                 "token": access_token.value,
                 "client_id": "client_1",
                 "client_secret": _context.cdb["client_1"]["client_secret"],
             }
         )
         _resp = self.revocation_endpoint.process_request(_req)
-        assert "response_args" in _resp
+        assert "response_msg" in _resp
 
     def test_revoked_access_token(self):
         access_token = self._get_access_token(AUTH_REQ)
         access_token.revoked = True
 
         _context = self.revocation_endpoint.upstream_get("endpoint_context")
 
@@ -504,15 +503,15 @@
             {
                 "token": access_token.value,
                 "client_id": "client_1",
                 "client_secret": _context.cdb["client_1"]["client_secret"],
             }
         )
         _resp = self.revocation_endpoint.process_request(_req)
-        assert "response_args" in _resp
+        assert "response_msg" in _resp
 
     def test_unsupported_token_type(self):
         self.revocation_endpoint.token_types_supported = ["access_token"]
         session_id = self._create_session(AUTH_REQ)
 
         # Apply consent
         grant = self.token_endpoint.upstream_get("endpoint_context").authz(session_id, AUTH_REQ)
```

### Comparing `idpyoidc-2.0.0/tests/test_server_40_oauth2_pushed_authorization.py` & `idpyoidc-2.1.0/tests/test_server_40_oauth2_pushed_authorization.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,23 +163,19 @@
             },
             "session_params": SESSION_PARAMS,
         }
         server = Server(ASConfiguration(conf=conf, base_path=BASEDIR), cwd=BASEDIR)
         context = server.context
         _clients = yaml.safe_load(io.StringIO(client_yaml))
         context.cdb = verify_oidc_client_information(_clients["oidc_clients"])
-        server.keyjar.import_jwks(
-            server.keyjar.export_jwks(True, ""), conf["issuer"]
-        )
+        server.keyjar.import_jwks(server.keyjar.export_jwks(True, ""), conf["issuer"])
 
         self.rp_keyjar = init_key_jar(key_defs=KEYDEFS, issuer_id="s6BhdRkqt3")
         # Add RP's keys to the OP's keyjar
-        server.keyjar.import_jwks(
-            self.rp_keyjar.export_jwks(issuer_id="s6BhdRkqt3"), "s6BhdRkqt3"
-        )
+        server.keyjar.import_jwks(self.rp_keyjar.export_jwks(issuer_id="s6BhdRkqt3"), "s6BhdRkqt3")
 
         self.pushed_authorization_endpoint = server.get_endpoint("pushed_authorization")
         self.authorization_endpoint = server.get_endpoint("authorization")
 
     def test_init(self):
         assert self.pushed_authorization_endpoint
 
@@ -195,15 +191,15 @@
             "state",
             "redirect_uri",
             "response_type",
             "scope",
             "code_challenge_method",
             "client_id",
             "code_challenge",
-            'authenticated'
+            "authenticated",
         }
 
     def test_pushed_auth_request(self):
         _msg = Message().from_urlencoded(AUTHN_REQUEST)
         _jwt = JWT(key_jar=self.rp_keyjar, iss="s6BhdRkqt3")
         _jws = _jwt.pack(_msg.to_dict())
 
@@ -222,15 +218,15 @@
             "response_type",
             "scope",
             "code_challenge_method",
             "client_id",
             "code_challenge",
             "request",
             "__verified_request",
-            'authenticated'
+            "authenticated",
         }
 
     def test_pushed_auth_urlencoded_process(self):
         http_info = {
             "headers": {"authorization": "Basic czZCaGRSa3F0Mzo3RmpmcDBaQnIxS3REUmJuZlZkbUl3"}
         }
 
@@ -241,15 +237,15 @@
             "state",
             "redirect_uri",
             "response_type",
             "scope",
             "code_challenge_method",
             "client_id",
             "code_challenge",
-            'authenticated'
+            "authenticated",
         }
 
         _resp = self.pushed_authorization_endpoint.process_request(_req)
 
         _msg = Message().from_urlencoded(AUTHN_REQUEST)
         assert _resp["return_uri"] == _msg["redirect_uri"]
```

### Comparing `idpyoidc-2.0.0/tests/test_server_50_persistence.py` & `idpyoidc-2.1.0/tests/test_server_50_persistence.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,34 +201,45 @@
         try:
             shutil.rmtree("db")
         except FileNotFoundError:
             pass
 
         # Both have to use the same keyjar
         _keyjar = init_key_jar(key_defs=KEYDEFS)
-        _keyjar.import_jwks_as_json(_keyjar.export_jwks_as_json(True, ""),
-                                    ENDPOINT_CONTEXT_CONFIG['issuer'])
+        _keyjar.import_jwks_as_json(
+            _keyjar.export_jwks_as_json(True, ""), ENDPOINT_CONTEXT_CONFIG["issuer"]
+        )
         server1 = Server(
-            OPConfiguration(conf=ENDPOINT_CONTEXT_CONFIG, base_path=BASEDIR), cwd=BASEDIR,
-            keyjar=_keyjar
+            OPConfiguration(conf=ENDPOINT_CONTEXT_CONFIG, base_path=BASEDIR),
+            cwd=BASEDIR,
+            keyjar=_keyjar,
         )
 
         server2 = Server(
-            OPConfiguration(conf=ENDPOINT_CONTEXT_CONFIG, base_path=BASEDIR), cwd=BASEDIR,
-            keyjar=_keyjar
+            OPConfiguration(conf=ENDPOINT_CONTEXT_CONFIG, base_path=BASEDIR),
+            cwd=BASEDIR,
+            keyjar=_keyjar,
         )
         # The top most part (Server class instance) is not
 
         server1.context.cdb["client_1"] = {
             "client_secret": "hemligt",
             "redirect_uris": [("https://example.com/cb", None)],
             "client_salt": "salted",
             "token_endpoint_auth_method": "client_secret_post",
             "response_types": ["code", "token", "code id_token", "id_token"],
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access", "research_and_scholarship"]
+            "allowed_scopes": [
+                "openid",
+                "profile",
+                "email",
+                "address",
+                "phone",
+                "offline_access",
+                "research_and_scholarship",
+            ],
         }
 
         # make server2 endpoint context a copy of server 1 endpoint context
         _store = server1.context.dump()
         server2.context.load(
             _store,
             init_args={
@@ -296,20 +307,21 @@
         _store = self.session_manager[fro].dump()
         self.session_manager[to].load(
             _store, init_args={"upstream_get": self.endpoint[to].upstream_get}
         )
 
     def test_init(self):
         assert self.endpoint[1]
-        assert set(
-            self.endpoint[1].upstream_get("context").provider_info["scopes_supported"]
-        ) == {"openid"}
-        assert self.endpoint[1].upstream_get("context").provider_info[
-                   "claims_parameter_supported"] == \
-               self.endpoint[2].upstream_get("context").provider_info["claims_parameter_supported"]
+        assert set(self.endpoint[1].upstream_get("context").provider_info["scopes_supported"]) == {
+            "openid"
+        }
+        assert (
+            self.endpoint[1].upstream_get("context").provider_info["claims_parameter_supported"]
+            == self.endpoint[2].upstream_get("context").provider_info["claims_parameter_supported"]
+        )
 
     def test_parse(self):
         session_id = self._create_session(AUTH_REQ, index=1)
         grant = self.endpoint[1].upstream_get("context").authz(session_id, AUTH_REQ)
         # grant, session_id = self._do_grant(AUTH_REQ, index=1)
         code = self._mint_code(grant, session_id, index=1)
         access_token = self._mint_access_token(grant, session_id, code, 1)
```

### Comparing `idpyoidc-2.0.0/tests/test_server_60_dpop.py` & `idpyoidc-2.1.0/tests/test_server_60_dpop.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from idpyoidc.message.oauth2 import AuthorizationRequest
 from idpyoidc.server import Server
 from idpyoidc.server import user_info
 from idpyoidc.server.authn_event import create_authn_event
 from idpyoidc.server.client_authn import verify_client
 from idpyoidc.server.configure import OPConfiguration
 from idpyoidc.server.oauth2.add_on.dpop import DPoPProof
-from idpyoidc.server.oauth2.add_on.dpop import post_parse_request
+from idpyoidc.server.oauth2.add_on.dpop import token_post_parse_request
 from idpyoidc.server.oauth2.authorization import Authorization
 from idpyoidc.server.oidc.token import Token
 from idpyoidc.server.user_authn.authn_context import INTERNETPROTOCOLPASSWORD
 from idpyoidc.time_util import utc_time_sans_frac
 from tests import CRYPT_CONFIG
 from tests import SESSION_PARAMS
 
@@ -62,21 +62,16 @@
 ISSUER = "https://example.com/"
 
 KEYJAR = init_key_jar(key_defs=KEYDEFS, issuer_id=ISSUER)
 KEYJAR.import_jwks(KEYJAR.export_jwks(True, ISSUER), "")
 
 RESPONSE_TYPES_SUPPORTED = [
     ["code"],
-    ["token"],
     ["id_token"],
-    ["code", "token"],
     ["code", "id_token"],
-    ["id_token", "token"],
-    ["code", "token", "id_token"],
-    ["none"],
 ]
 
 CAPABILITIES = {
     "response_types_supported": [" ".join(x) for x in RESPONSE_TYPES_SUPPORTED],
     "token_endpoint_auth_methods_supported": [
         "client_secret_post",
         "client_secret_basic",
@@ -84,15 +79,15 @@
         "private_key_jwt",
     ],
     "response_modes_supported": ["query", "fragment", "form_post"],
     "subject_types_supported": ["public", "pairwise", "ephemeral"],
     "claim_types_supported": ["normal", "aggregated", "distributed"],
     "claims_parameter_supported": True,
     "request_parameter_supported": True,
-    "request_uri_parameter_supported": True,
+    # "request_uri_parameter_supported": True,
 }
 
 AUTH_REQ = AuthorizationRequest(
     client_id="client_1",
     redirect_uri="https://example.com/cb",
     scope=["openid"],
     state="STATE",
@@ -184,15 +179,15 @@
         self.context = server.context
         self.context.cdb["client_1"] = {
             "client_secret": "hemligt",
             "redirect_uris": [("https://example.com/cb", None)],
             "client_salt": "salted",
             "token_endpoint_auth_method": "client_secret_post",
             "response_types": ["code", "token", "code id_token", "id_token"],
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"]
+            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"],
         }
         self.user_id = "diana"
         self.token_endpoint = server.get_endpoint("token")
         self.session_manager = self.context.session_manager
 
     def _create_session(self, auth_req, sub_type="public", sector_identifier=""):
         if sector_identifier:
@@ -224,15 +219,15 @@
             if isinstance(_exp_in, str):
                 _exp_in = int(_exp_in)
             if _exp_in:
                 _code.expires_at = utc_time_sans_frac() + _exp_in
         return _code
 
     def test_post_parse_request(self):
-        auth_req = post_parse_request(
+        auth_req = token_post_parse_request(
             AUTH_REQ,
             AUTH_REQ["client_id"],
             self.context,
             http_info={
                 "headers": {"dpop": DPOP_HEADER},
                 "url": "https://server.example.com/token",
                 "method": "POST",
```

### Comparing `idpyoidc-2.0.0/tests/test_server_61_add_on.py` & `idpyoidc-2.1.0/tests/test_server_61_add_on.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,21 +24,16 @@
 ISSUER = "https://example.com/"
 
 KEYJAR = init_key_jar(key_defs=KEYDEFS, issuer_id=ISSUER)
 KEYJAR.import_jwks(KEYJAR.export_jwks(True, ISSUER), "")
 
 RESPONSE_TYPES_SUPPORTED = [
     ["code"],
-    ["token"],
     ["id_token"],
-    ["code", "token"],
     ["code", "id_token"],
-    ["id_token", "token"],
-    ["code", "token", "id_token"],
-    ["none"],
 ]
 
 CAPABILITIES = {
     "response_types_supported": [" ".join(x) for x in RESPONSE_TYPES_SUPPORTED],
     "token_endpoint_auth_methods_supported": [
         "client_secret_post",
         "client_secret_basic",
@@ -51,15 +46,15 @@
         "authorization_code",
         "implicit",
         "urn:ietf:params:oauth:grant-type:jwt-bearer",
     ],
     "claim_types_supported": ["normal", "aggregated", "distributed"],
     "claims_parameter_supported": True,
     "request_parameter_supported": True,
-    "request_uri_parameter_supported": True,
+    # "request_uri_parameter_supported": True,
 }
 
 AUTH_REQ = AuthorizationRequest(
     client_id="client_1",
     redirect_uri="https://example.com/cb",
     scope=["openid"],
     state="STATE",
@@ -139,15 +134,15 @@
         self.context = server.context
         self.context.cdb["client_1"] = {
             "client_secret": "hemligt",
             "redirect_uris": [("https://example.com/cb", None)],
             "client_salt": "salted",
             "token_endpoint_auth_method": "client_secret_post",
             "response_types": ["code", "token", "code id_token", "id_token"],
-            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"]
+            "allowed_scopes": ["openid", "profile", "email", "address", "phone", "offline_access"],
         }
         self.endpoint = server.get_endpoint("authorization")
 
     def test_process_request(self):
         _context = self.endpoint.upstream_get("context")
         assert _context.add_on["extra_args"] == {"authorization": {"iss": "issuer"}}
```

### Comparing `idpyoidc-2.0.0/tests/test_tandem_08_oauth2_cc_ropc.py` & `idpyoidc-2.1.0/tests/test_tandem_oauth2_cc_ropc.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,28 +33,26 @@
 }
 
 SESSION_PARAMS = {"encrypter": CRYPT_CONFIG}
 
 CONFIG = {
     "issuer": "https://example.net/",
     "httpc_params": {"verify": False},
-    "preference": {
-        "grant_types_supported": ["client_credentials", "password"]
-    },
-    "keys": {"uri_path": "jwks.json", "key_defs": KEYDEFS, 'read_only': False},
+    "preference": {"grant_types_supported": ["client_credentials", "password"]},
+    "keys": {"uri_path": "jwks.json", "key_defs": KEYDEFS, "read_only": False},
     "token_handler_args": {
         "jwks_defs": {"key_defs": KEYDEFS},
         "token": {
             "class": "idpyoidc.server.token.jwt_token.JWTToken",
             "kwargs": {
                 "lifetime": 3600,
                 "add_claims_by_scope": True,
                 "aud": ["https://example.org/appl"],
-            }
-        }
+            },
+        },
     },
     "endpoint": {
         "token": {
             "path": "token",
             "class": Token,
             "kwargs": {
                 "client_authn_method": ["client_secret_basic", "client_secret_post"],
@@ -92,44 +90,45 @@
     "authentication": {
         "user": {
             "acr": "urn:oasis:names:tc:SAML:2.0:ac:classes:InternetProtocolPassword",
             "class": "idpyoidc.server.user_authn.user.UserPass",
             "kwargs": {
                 "db_conf": {
                     "class": "idpyoidc.server.util.JSONDictDB",
-                    "kwargs": {"filename": full_path("passwd.json")}
+                    "kwargs": {"filename": full_path("passwd.json")},
                 }
-            }
+            },
         }
-    }
+    },
 }
 
 CLIENT_BASE_URL = "https://example.com"
 
 CLIENT_CONFIG = {
     "client_id": "client_1",
     "client_secret": "another password",
-    "base_url": CLIENT_BASE_URL
+    "base_url": CLIENT_BASE_URL,
 }
 CLIENT_SERVICES = {
     "resource_owner_password_credentials": {
         "class": "idpyoidc.client.oauth2.resource_owner_password_credentials.ROPCAccessTokenRequest"
     }
 }
 
 
 def test_ropc():
     # Client side
 
     client = Client(config=CLIENT_CONFIG, services=CLIENT_SERVICES)
     client.get_service("resource_owner_password_credentials").endpoint = "https://example.com/token"
 
-    service = client.get_service('resource_owner_password_credentials')
+    service = client.get_service("resource_owner_password_credentials")
     client_request_info = service.get_request_parameters(
-        request_args={'username': 'diana', 'password': 'krall'})
+        request_args={"username": "diana", "password": "krall"}
+    )
 
     # Server side
 
     server = Server(ASConfiguration(conf=CONFIG, base_path=BASEDIR), cwd=BASEDIR)
     server.context.cdb["client_1"] = {
         "client_secret": "another password",
         "redirect_uris": [("https://example.com/cb", None)],
@@ -137,9 +136,9 @@
         "endpoint_auth_method": "client_secret_post",
         "response_types": ["code", "code id_token", "id_token"],
         "allowed_scopes": ["resourceA"],
         # "grant_types_supported": ['client_credentials', 'password']
     }
 
     token_endpoint = server.get_endpoint("token")
-    request = token_endpoint.parse_request(client_request_info['request'])
+    request = token_endpoint.parse_request(client_request_info["request"])
     assert request
```

### Comparing `idpyoidc-2.0.0/tests/test_tandem_10_oauth2_token_exchange.py` & `idpyoidc-2.1.0/tests/test_tandem_oauth2_token_exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,17 +77,15 @@
 _OAUTH2_SERVICES = {
     "claims": {"class": "idpyoidc.client.oauth2.server_metadata.ServerMetadata"},
     "authorization": {"class": "idpyoidc.client.oauth2.authorization.Authorization"},
     "access_token": {"class": "idpyoidc.client.oauth2.access_token.AccessToken"},
     "refresh_access_token": {
         "class": "idpyoidc.client.oauth2.refresh_access_token.RefreshAccessToken"
     },
-    "token_exchange": {
-        "class": "idpyoidc.client.oauth2.token_exchange.TokenExchange"
-    }
+    "token_exchange": {"class": "idpyoidc.client.oauth2.token_exchange.TokenExchange"},
 }
 
 
 class TestEndpoint(object):
     @pytest.fixture(autouse=True)
     def create_endpoint(self):
         server_conf = {
@@ -114,15 +112,15 @@
                 "authorization": {
                     "path": "authorization",
                     "class": "idpyoidc.server.oauth2.authorization.Authorization",
                     "kwargs": {},
                 },
                 "token": {
                     "path": "token",
-                    "class": "idpyoidc.server.oidc.token.Token",
+                    "class": "idpyoidc.server.oauth2.token.Token",
                     "kwargs": {},
                 },
             },
             "authentication": {
                 "anon": {
                     "acr": INTERNETPROTOCOLPASSWORD,
                     "class": "idpyoidc.server.user_authn.user.NoAuthn",
@@ -181,41 +179,45 @@
         client_1_config = {
             "issuer": server_conf["issuer"],
             "client_secret": "hemligtlösenord",
             "client_id": "client_1",
             "redirect_uris": ["https://example.com/cb"],
             "client_salt": "salted_peanuts_cooking",
             "token_endpoint_auth_methods_supported": ["client_secret_post"],
-            "response_types_supported": ["code", "token", "code id_token", "id_token"],
+            "response_types_supported": ["code", "code id_token", "id_token"],
             "allowed_scopes": ["openid", "profile", "offline_access"],
         }
         client_2_config = {
             "issuer": server_conf["issuer"],
             "client_id": "client_2",
             "client_secret": "hemligtlösenord",
             "redirect_uris": ["https://example.com/cb"],
             "client_salt": "salted_peanuts_cooking",
             "token_endpoint_auth_methods_supported": ["client_secret_post"],
-            "response_types_supported": ["code", "token", "code id_token", "id_token"],
+            "response_types_supported": ["code", "code id_token", "id_token"],
             "allowed_scopes": ["openid", "profile", "offline_access"],
         }
-        self.client_1 = Client(client_type='oauth2', config=client_1_config,
-                               keyjar=build_keyjar(KEYDEFS),
-                               services=_OAUTH2_SERVICES)
-        self.client_2 = Client(client_type='oauth2', config=client_2_config,
-                               keyjar=build_keyjar(KEYDEFS),
-                               services=_OAUTH2_SERVICES)
+        self.client_1 = Client(
+            client_type="oauth2",
+            config=client_1_config,
+            keyjar=build_keyjar(KEYDEFS),
+            services=_OAUTH2_SERVICES,
+        )
+        self.client_2 = Client(
+            client_type="oauth2",
+            config=client_2_config,
+            keyjar=build_keyjar(KEYDEFS),
+            services=_OAUTH2_SERVICES,
+        )
 
         self.context = self.server.context
         self.context.cdb["client_1"] = client_1_config
         self.context.cdb["client_2"] = client_2_config
-        self.context.keyjar.import_jwks(
-            self.client_1.keyjar.export_jwks(), "client_1")
-        self.context.keyjar.import_jwks(
-            self.client_2.keyjar.export_jwks(), "client_2")
+        self.context.keyjar.import_jwks(self.client_1.keyjar.export_jwks(), "client_1")
+        self.context.keyjar.import_jwks(self.client_2.keyjar.export_jwks(), "client_2")
 
         self.context.set_provider_info()
 
         # self.endpoint = self.server.upstream_get("endpoint", "token")
         # self.introspection_endpoint = self.server.upstream_get("endpoint", "introspection")
         self.session_manager = self.context.session_manager
         self.user_id = "diana"
@@ -230,15 +232,16 @@
         _server = self.server.get_endpoint(endpoint_type)
         if areq:
             if headers:
                 argv = {"http_info": {"headers": headers}}
             else:
                 argv = {}
             areq.lax = True
-            _pr_resp = _server.parse_request(areq.to_urlencoded(), **argv)
+            _req = areq.serialize(_server.request_format)
+            _pr_resp = _server.parse_request(_req, **argv)
         else:
             _pr_resp = _server.parse_request(areq)
 
         if is_error_message(_pr_resp):
             return areq, _pr_resp
 
         _resp = _server.process_request(_pr_resp)
@@ -250,53 +253,49 @@
         resp = _client.parse_response(_response["response"])
         _client.update_service_context(_resp["response_args"], key=state)
         return areq, resp
 
     def process_setup(self, token=None, scope=None):
         # ***** Discovery *********
 
-        _req, _resp = self.do_query('server_metadata', 'server_metadata', {}, '')
+        _req, _resp = self.do_query("server_metadata", "server_metadata", {}, "")
 
         # ***** Authorization Request **********
-        _nonce = rndstr(24),
+        _nonce = (rndstr(24),)
         _context = self.client_1.get_service_context()
         # Need a new state for a new authorization request
         _state = _context.cstate.create_state(iss=_context.get("issuer"))
         _context.cstate.bind_key(_nonce, _state)
 
-        req_args = {
-            "response_type": ["code"],
-            "nonce": _nonce,
-            "state": _state
-        }
+        req_args = {"response_type": ["code"], "nonce": _nonce, "state": _state}
 
         if scope:
             _scope = scope
         else:
             _scope = ["openid"]
 
             if token and list(token.keys())[0] == "refresh_token":
                 _scope = ["openid", "offline_access"]
 
         req_args["scope"] = _scope
 
-        areq, auth_response = self.do_query('authorization', 'authorization', req_args, _state)
+        areq, auth_response = self.do_query("authorization", "authorization", req_args, _state)
 
         # ***** Token Request **********
 
         req_args = {
             "code": auth_response["code"],
             "state": auth_response["state"],
             "redirect_uri": areq["redirect_uri"],
             "grant_type": "authorization_code",
             "client_id": self.client_1.get_client_id(),
             "client_secret": _context.get_usage("client_secret"),
         }
 
-        _token_request, resp = self.do_query("accesstoken", 'token', req_args, _state)
+        _token_request, resp = self.do_query("accesstoken", "token", req_args, _state)
 
         return resp, _state, _scope
 
     @pytest.mark.parametrize(
         "token",
         [
             {"access_token": "urn:ietf:params:oauth:token-type:access_token"},
@@ -312,20 +311,21 @@
 
         # ****** Token Exchange Request **********
 
         req_args = {
             "grant_type": "urn:ietf:params:oauth:grant-type:token-exchange",
             "requested_token_type": token[list(token.keys())[0]],
             "subject_token": resp["access_token"],
-            "subject_token_type": 'urn:ietf:params:oauth:token-type:access_token',
-            "state": _state
+            "subject_token_type": "urn:ietf:params:oauth:token-type:access_token",
+            "state": _state,
         }
 
-        _token_exchange_request, _te_resp = self.do_query("token_exchange", "token", req_args,
-                                                          _state)
+        _token_exchange_request, _te_resp = self.do_query(
+            "token_exchange", "token", req_args, _state
+        )
 
         assert set(_te_resp.keys()) == {
             "access_token",
             "token_type",
             "scope",
             "expires_in",
             "issued_token_type",
@@ -352,35 +352,35 @@
             ],
             "requested_token_types_supported": [
                 "urn:ietf:params:oauth:token-type:access_token",
                 "urn:ietf:params:oauth:token-type:refresh_token",
             ],
             "policy": {
                 "": {
-                    "function":
-                        "idpyoidc.server.oauth2.token_helper.validate_token_exchange_policy",
+                    "function": "idpyoidc.server.oauth2.token_helper.validate_token_exchange_policy",
                     "kwargs": {"scope": ["openid", "offline_access"]},
                 }
             },
         }
 
         resp, _state, _scope = self.process_setup(token)
 
         # ****** Token Exchange Request **********
 
         req_args = {
             "grant_type": "urn:ietf:params:oauth:grant-type:token-exchange",
             "requested_token_type": token[list(token.keys())[0]],
             "subject_token": resp["access_token"],
-            "subject_token_type": 'urn:ietf:params:oauth:token-type:access_token',
-            "state": _state
+            "subject_token_type": "urn:ietf:params:oauth:token-type:access_token",
+            "state": _state,
         }
 
-        _token_exchange_request, _te_resp = self.do_query("token_exchange", "token", req_args,
-                                                          _state)
+        _token_exchange_request, _te_resp = self.do_query(
+            "token_exchange", "token", req_args, _state
+        )
 
         assert set(_te_resp.keys()) == {
             "access_token",
             "token_type",
             "scope",
             "expires_in",
             "issued_token_type",
@@ -409,16 +409,17 @@
             "subject_token": resp["access_token"],
             "subject_token_type": "urn:ietf:params:oauth:token-type:access_token",
             "requested_token_type": "urn:ietf:params:oauth:token-type:access_token",
             "audience": ["https://example.com"],
             "resource": ["https://example.com"],
         }
 
-        _token_exchange_request, _te_resp = self.do_query("token_exchange", "token", req_args,
-                                                          _state)
+        _token_exchange_request, _te_resp = self.do_query(
+            "token_exchange", "token", req_args, _state
+        )
 
         assert set(_te_resp.keys()) == {
             "access_token",
             "token_type",
             "expires_in",
             "issued_token_type",
             "scope",
@@ -436,15 +437,15 @@
 
         # ****** Token Exchange Request **********
 
         req_args = {
             "grant_type": "urn:ietf:params:oauth:grant-type:token-exchange",
             "subject_token": resp["access_token"],
             "subject_token_type": "urn:ietf:params:oauth:token-type:access_token",
-            "resource": ["https://example.com/api"]
+            "resource": ["https://example.com/api"],
         }
 
         _te_request, _te_resp = self.do_query("token_exchange", "token", req_args, _state)
 
         assert _te_resp["error"] == "invalid_request"
         assert _te_resp["error_description"] == "Do not know how to handle this type of request"
 
@@ -477,15 +478,16 @@
 
     def test_refresh_token_audience(self):
         """
         Test that requesting a refresh token with audience fails.
         """
 
         resp, _state, _scope = self.process_setup(
-            {"refresh_token": "urn:ietf:params:oauth:token-type:refresh_token"})
+            {"refresh_token": "urn:ietf:params:oauth:token-type:refresh_token"}
+        )
 
         # ****** Token Exchange Request **********
 
         req_args = {
             "grant_type": "urn:ietf:params:oauth:grant-type:token-exchange",
             "subject_token": resp["refresh_token"],
             "subject_token_type": "urn:ietf:params:oauth:token-type:refresh_token",
@@ -525,15 +527,16 @@
         assert _te_resp["error_description"] == "Unknown audience"
 
     def test_exchange_refresh_token_to_refresh_token(self):
         """
         Test whether exchanging a refresh token to another refresh token works.
         """
         resp, _state, _scope = self.process_setup(
-            {"refresh_token": "urn:ietf:params:oauth:token-type:refresh_token"})
+            {"refresh_token": "urn:ietf:params:oauth:token-type:refresh_token"}
+        )
 
         # ****** Token Exchange Request **********
 
         req_args = {
             "grant_type": "urn:ietf:params:oauth:grant-type:token-exchange",
             "subject_token": resp["refresh_token"],
             "subject_token_type": "urn:ietf:params:oauth:token-type:refresh_token",
```

