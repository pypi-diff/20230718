# Comparing `tmp/openapi_pydantic-0.3.1.tar.gz` & `tmp/openapi_pydantic-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi_pydantic-0.3.1.tar", max compression
+gzip compressed data, was "openapi_pydantic-0.3.2.tar", max compression
```

## Comparing `openapi_pydantic-0.3.1.tar` & `openapi_pydantic-0.3.2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0     1896 2023-07-10 22:38:45.858524 openapi_pydantic-0.3.1/LICENSE
--rw-r--r--   0        0        0     9803 2023-07-10 22:38:45.858524 openapi_pydantic-0.3.1/README.md
--rw-r--r--   0        0        0     1417 2023-07-10 22:38:45.858524 openapi_pydantic-0.3.1/openapi_pydantic/__init__.py
--rw-r--r--   0        0        0     3196 2023-07-10 22:38:45.858524 openapi_pydantic-0.3.1/openapi_pydantic/compat.py
--rw-r--r--   0        0        0       26 2023-07-10 22:38:45.858524 openapi_pydantic-0.3.1/openapi_pydantic/py.typed
--rw-r--r--   0        0        0     6860 2023-07-10 22:38:45.858524 openapi_pydantic-0.3.1/openapi_pydantic/util.py
--rw-r--r--   0        0        0     1474 2023-07-10 22:38:45.858524 openapi_pydantic-0.3.1/openapi_pydantic/v3/__init__.py
--rw-r--r--   0        0        0      849 2023-07-10 22:38:45.858524 openapi_pydantic-0.3.1/openapi_pydantic/v3/parser.py
--rw-r--r--   0        0        0     1659 2023-07-10 22:38:45.858524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/README.md
--rw-r--r--   0        0        0     2297 2023-07-10 22:38:45.858524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/__init__.py
--rw-r--r--   0        0        0      747 2023-07-10 22:38:45.858524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/callback.py
--rw-r--r--   0        0        0     4770 2023-07-10 22:38:45.858524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/components.py
--rw-r--r--   0        0        0     1026 2023-07-10 22:38:45.858524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/contact.py
--rw-r--r--   0        0        0      283 2023-07-10 22:38:45.858524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/datatype.py
--rw-r--r--   0        0        0     1419 2023-07-10 22:38:45.858524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/discriminator.py
--rw-r--r--   0        0        0     3242 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/encoding.py
--rw-r--r--   0        0        0     1667 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/example.py
--rw-r--r--   0        0        0      934 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/external_documentation.py
--rw-r--r--   0        0        0     1836 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/header.py
--rw-r--r--   0        0        0     2023 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/info.py
--rw-r--r--   0        0        0      818 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/license.py
--rw-r--r--   0        0        0     3083 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/link.py
--rw-r--r--   0        0        0     2940 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/media_type.py
--rw-r--r--   0        0        0     2058 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/oauth_flow.py
--rw-r--r--   0        0        0     1008 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/oauth_flows.py
--rw-r--r--   0        0        0     2857 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/open_api.py
--rw-r--r--   0        0        0     6103 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/operation.py
--rw-r--r--   0        0        0     7683 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/parameter.py
--rw-r--r--   0        0        0     4554 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/path_item.py
--rw-r--r--   0        0        0     1017 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/paths.py
--rw-r--r--   0        0        0     1118 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/reference.py
--rw-r--r--   0        0        0     2836 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/request_body.py
--rw-r--r--   0        0        0     3198 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/response.py
--rw-r--r--   0        0        0     2050 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/responses.py
--rw-r--r--   0        0        0    21677 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/schema.py
--rw-r--r--   0        0        0     1325 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/security_requirement.py
--rw-r--r--   0        0        0     3529 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/security_scheme.py
--rw-r--r--   0        0        0     1906 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/server.py
--rw-r--r--   0        0        0     1244 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/server_variable.py
--rw-r--r--   0        0        0     1142 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/tag.py
--rw-r--r--   0        0        0     7770 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/util.py
--rw-r--r--   0        0        0     2047 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/xml.py
--rw-r--r--   0        0        0     1719 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/README.md
--rw-r--r--   0        0        0     2297 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/__init__.py
--rw-r--r--   0        0        0      806 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/callback.py
--rw-r--r--   0        0        0     4929 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/components.py
--rw-r--r--   0        0        0     1022 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/contact.py
--rw-r--r--   0        0        0      238 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/datatype.py
--rw-r--r--   0        0        0     1419 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/discriminator.py
--rw-r--r--   0        0        0     3674 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/encoding.py
--rw-r--r--   0        0        0     1769 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/example.py
--rw-r--r--   0        0        0      932 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/external_documentation.py
--rw-r--r--   0        0        0     1835 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/header.py
--rw-r--r--   0        0        0     2141 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/info.py
--rw-r--r--   0        0        0     1189 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/license.py
--rw-r--r--   0        0        0     3163 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/link.py
--rw-r--r--   0        0        0     3008 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/media_type.py
--rw-r--r--   0        0        0     2239 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/oauth_flow.py
--rw-r--r--   0        0        0     1008 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/oauth_flows.py
--rw-r--r--   0        0        0     3695 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/open_api.py
--rw-r--r--   0        0        0     6385 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/operation.py
--rw-r--r--   0        0        0     7685 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/parameter.py
--rw-r--r--   0        0        0     4634 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/path_item.py
--rw-r--r--   0        0        0     1040 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/paths.py
--rw-r--r--   0        0        0     1687 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/reference.py
--rw-r--r--   0        0        0     2836 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/request_body.py
--rw-r--r--   0        0        0     3187 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/response.py
--rw-r--r--   0        0        0     2048 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/responses.py
--rw-r--r--   0        0        0    38296 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/schema.py
--rw-r--r--   0        0        0     1434 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/security_requirement.py
--rw-r--r--   0        0        0     3916 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/security_scheme.py
--rw-r--r--   0        0        0     1907 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/server.py
--rw-r--r--   0        0        0     1242 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/server_variable.py
--rw-r--r--   0        0        0     1142 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/tag.py
--rw-r--r--   0        0        0     2123 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/xml.py
--rw-r--r--   0        0        0     1221 2023-07-10 22:38:45.862524 openapi_pydantic-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    10663 1970-01-01 00:00:00.000000 openapi_pydantic-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1896 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/LICENSE
+-rw-r--r--   0        0        0     9803 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/README.md
+-rw-r--r--   0        0        0     1417 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/openapi_pydantic/__init__.py
+-rw-r--r--   0        0        0     3215 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/openapi_pydantic/compat.py
+-rw-r--r--   0        0        0       26 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/openapi_pydantic/py.typed
+-rw-r--r--   0        0        0     6866 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/openapi_pydantic/util.py
+-rw-r--r--   0        0        0     1474 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/openapi_pydantic/v3/__init__.py
+-rw-r--r--   0        0        0      849 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/openapi_pydantic/v3/parser.py
+-rw-r--r--   0        0        0     1659 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/README.md
+-rw-r--r--   0        0        0     2297 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/__init__.py
+-rw-r--r--   0        0        0      747 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/callback.py
+-rw-r--r--   0        0        0     4770 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/components.py
+-rw-r--r--   0        0        0     1026 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/contact.py
+-rw-r--r--   0        0        0      283 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/datatype.py
+-rw-r--r--   0        0        0     1419 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/discriminator.py
+-rw-r--r--   0        0        0     3242 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/encoding.py
+-rw-r--r--   0        0        0     1667 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/example.py
+-rw-r--r--   0        0        0      934 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/external_documentation.py
+-rw-r--r--   0        0        0     1836 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/header.py
+-rw-r--r--   0        0        0     2023 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/info.py
+-rw-r--r--   0        0        0      818 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/license.py
+-rw-r--r--   0        0        0     3083 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/link.py
+-rw-r--r--   0        0        0     2940 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/media_type.py
+-rw-r--r--   0        0        0     2058 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/oauth_flow.py
+-rw-r--r--   0        0        0     1008 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/oauth_flows.py
+-rw-r--r--   0        0        0     2857 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/open_api.py
+-rw-r--r--   0        0        0     6103 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/operation.py
+-rw-r--r--   0        0        0     7683 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/parameter.py
+-rw-r--r--   0        0        0     4554 2023-07-18 17:40:20.825466 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/path_item.py
+-rw-r--r--   0        0        0     1017 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/paths.py
+-rw-r--r--   0        0        0     1118 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/reference.py
+-rw-r--r--   0        0        0     2836 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/request_body.py
+-rw-r--r--   0        0        0     3198 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/response.py
+-rw-r--r--   0        0        0     2050 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/responses.py
+-rw-r--r--   0        0        0    21677 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/schema.py
+-rw-r--r--   0        0        0     1325 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/security_requirement.py
+-rw-r--r--   0        0        0     3529 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/security_scheme.py
+-rw-r--r--   0        0        0     1906 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/server.py
+-rw-r--r--   0        0        0     1244 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/server_variable.py
+-rw-r--r--   0        0        0     1142 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/tag.py
+-rw-r--r--   0        0        0     7780 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/util.py
+-rw-r--r--   0        0        0     2047 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/xml.py
+-rw-r--r--   0        0        0     1719 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/README.md
+-rw-r--r--   0        0        0     2297 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/__init__.py
+-rw-r--r--   0        0        0      806 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/callback.py
+-rw-r--r--   0        0        0     4929 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/components.py
+-rw-r--r--   0        0        0     1022 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/contact.py
+-rw-r--r--   0        0        0      238 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/datatype.py
+-rw-r--r--   0        0        0     1419 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/discriminator.py
+-rw-r--r--   0        0        0     3674 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/encoding.py
+-rw-r--r--   0        0        0     1769 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/example.py
+-rw-r--r--   0        0        0      932 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/external_documentation.py
+-rw-r--r--   0        0        0     1835 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/header.py
+-rw-r--r--   0        0        0     2141 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/info.py
+-rw-r--r--   0        0        0     1189 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/license.py
+-rw-r--r--   0        0        0     3163 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/link.py
+-rw-r--r--   0        0        0     3008 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/media_type.py
+-rw-r--r--   0        0        0     2239 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/oauth_flow.py
+-rw-r--r--   0        0        0     1008 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/oauth_flows.py
+-rw-r--r--   0        0        0     3695 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/open_api.py
+-rw-r--r--   0        0        0     6385 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/operation.py
+-rw-r--r--   0        0        0     7685 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/parameter.py
+-rw-r--r--   0        0        0     4634 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/path_item.py
+-rw-r--r--   0        0        0     1040 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/paths.py
+-rw-r--r--   0        0        0     1687 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/reference.py
+-rw-r--r--   0        0        0     2836 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/request_body.py
+-rw-r--r--   0        0        0     3187 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/response.py
+-rw-r--r--   0        0        0     2048 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/responses.py
+-rw-r--r--   0        0        0    38296 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/schema.py
+-rw-r--r--   0        0        0     1434 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/security_requirement.py
+-rw-r--r--   0        0        0     3916 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/security_scheme.py
+-rw-r--r--   0        0        0     1907 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/server.py
+-rw-r--r--   0        0        0     1242 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/server_variable.py
+-rw-r--r--   0        0        0     1142 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/tag.py
+-rw-r--r--   0        0        0     2123 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/xml.py
+-rw-r--r--   0        0        0     1221 2023-07-18 17:40:20.829467 openapi_pydantic-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    10663 1970-01-01 00:00:00.000000 openapi_pydantic-0.3.2/PKG-INFO
```

### Comparing `openapi_pydantic-0.3.1/LICENSE` & `openapi_pydantic-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/README.md` & `openapi_pydantic-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/__init__.py` & `openapi_pydantic-0.3.2/openapi_pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/compat.py` & `openapi_pydantic-0.3.2/openapi_pydantic/compat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Compatibility layer to make this package usable with Pydantic 1 or 2"""
 
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING, Dict, List, Optional, Tuple
 
 from pydantic.version import VERSION as PYDANTIC_VERSION
 
 __all__ = [
     "PYDANTIC_V2",
     "ConfigDict",
     "JsonSchemaMode",
@@ -26,15 +26,15 @@
     from typing import Any, Literal, Type, TypedDict
 
     from pydantic import BaseModel
     from pydantic import ConfigDict as PydanticConfigDict
 
     def ConfigDict(
         extra: Literal["allow", "ignore", "forbid"] = "allow",
-        json_schema_extra: Optional[dict[str, Any]] = None,
+        json_schema_extra: Optional[Dict[str, Any]] = None,
         populate_by_name: bool = True,
     ) -> PydanticConfigDict:
         """Stub for pydantic.ConfigDict in Pydantic 2"""
         ...
 
     class Extra(Enum):
         """Stub for pydantic.Extra in Pydantic 1"""
@@ -45,29 +45,29 @@
 
     class RootModel(BaseModel):
         """Stub for pydantic.RootModel in Pydantic 2"""
 
     JsonSchemaMode = Literal["validation", "serialization"]
 
     def models_json_schema(
-        models: list[tuple[Type[BaseModel], JsonSchemaMode]],
+        models: List[Tuple[Type[BaseModel], JsonSchemaMode]],
         *,
         by_alias: bool = True,
         ref_template: str = "#/$defs/{model}",
         schema_generator: Optional[type] = None,
-    ) -> tuple[dict, dict[str, Any]]:
+    ) -> Tuple[Dict, Dict[str, Any]]:
         """Stub for pydantic.json_schema.models_json_schema in Pydantic 2"""
         ...
 
     def v1_schema(
-        models: list[Type[BaseModel]],
+        models: List[Type[BaseModel]],
         *,
         by_alias: bool = True,
         ref_prefix: str = "#/$defs",
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         """Stub for pydantic.schema.schema in Pydantic 1"""
         ...
 
     DEFS_KEY = "$defs"
 
     class MinLengthArg(TypedDict):
         pass
```

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/util.py` & `openapi_pydantic-0.3.2/openapi_pydantic/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import Any, Generic, List, Optional, Set, Type, TypeVar, cast
+from typing import Any, Dict, Generic, List, Optional, Set, Type, TypeVar, cast
 
 from pydantic import BaseModel
 
 from openapi_pydantic.compat import (
     DEFS_KEY,
     PYDANTIC_V2,
     JsonSchemaMode,
@@ -106,15 +106,15 @@
                 )
         new_open_api.components.schemas.update(_validate_schemas(schema_definitions))
     else:
         new_open_api.components.schemas = _validate_schemas(schema_definitions)
     return new_open_api
 
 
-def _validate_schemas(schema_definitions: dict[str, Any]) -> dict[str, Schema]:
+def _validate_schemas(schema_definitions: Dict[str, Any]) -> Dict[str, Schema]:
     """Convert JSON Schema definitions to parsed OpenAPI objects"""
     # Note: if an error occurs in schema_validate(), it may indicate that
     # the generated JSON schemas are not compatible with the version
     # of OpenAPI this module depends on.
     return {
         key: schema_validate(schema_dict)
         for key, schema_dict in schema_definitions[DEFS_KEY].items()
```

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/__init__.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/parser.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/parser.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/README.md` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/README.md`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/__init__.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/callback.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/callback.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/components.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/components.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/contact.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/contact.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/discriminator.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/discriminator.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/encoding.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/encoding.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/example.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/example.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/external_documentation.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/external_documentation.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/header.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/header.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/info.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/info.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/license.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/license.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/link.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/link.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/media_type.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/media_type.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/oauth_flow.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/oauth_flows.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/oauth_flows.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/open_api.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/open_api.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/operation.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/operation.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/parameter.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/parameter.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/path_item.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/path_item.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/paths.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/paths.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/reference.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/reference.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/request_body.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/request_body.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/response.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/response.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/responses.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/responses.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/schema.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -600,15 +600,15 @@
 if TYPE_CHECKING:
 
     def schema_validate(
         obj: Any,
         *,
         strict: Optional[bool] = None,
         from_attributes: Optional[bool] = None,
-        context: Optional[dict[str, Any]] = None
+        context: Optional[Dict[str, Any]] = None
     ) -> Schema:
         ...
 
 elif PYDANTIC_V2:
     schema_validate = Schema.model_validate
 
 else:
```

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/security_requirement.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/security_requirement.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/security_scheme.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/security_scheme.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/server.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/server.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/server_variable.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/server_variable.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/tag.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/tag.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/util.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 from typing import (
     TYPE_CHECKING,
     Any,
+    Dict,
     Generic,
     List,
     Optional,
     Set,
     Type,
     TypeVar,
     Union,
@@ -149,16 +150,16 @@
         new_open_api.components.schemas.update(_validate_schemas(schema_definitions))
     else:
         new_open_api.components.schemas = _validate_schemas(schema_definitions)
     return new_open_api
 
 
 def _validate_schemas(
-    schema_definitions: dict[str, Any]
-) -> dict[str, Union[Reference, Schema]]:
+    schema_definitions: Dict[str, Any]
+) -> Dict[str, Union[Reference, Schema]]:
     """Convert JSON Schema definitions to parsed OpenAPI objects"""
     # Note: if an error occurs in schema_validate(), it may indicate that
     # the generated JSON schemas are not compatible with the version
     # of OpenAPI this module depends on.
     return {
         key: schema_validate(schema_dict)
         for key, schema_dict in schema_definitions[DEFS_KEY].items()
```

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_0_3/xml.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_0_3/xml.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/README.md` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/README.md`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/__init__.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/callback.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/callback.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/components.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/components.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/contact.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/contact.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/discriminator.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/discriminator.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/encoding.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/encoding.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/example.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/example.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/external_documentation.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/external_documentation.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/header.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/header.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/info.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/info.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/license.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/license.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/link.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/link.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/media_type.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/media_type.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/oauth_flow.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/oauth_flows.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/oauth_flows.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/open_api.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/open_api.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/operation.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/operation.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/parameter.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/parameter.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/path_item.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/path_item.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/paths.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/paths.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/reference.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/reference.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/request_body.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/request_body.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/response.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/response.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/responses.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/responses.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/schema.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -957,15 +957,15 @@
 if TYPE_CHECKING:
 
     def schema_validate(
         obj: Any,
         *,
         strict: Optional[bool] = None,
         from_attributes: Optional[bool] = None,
-        context: Optional[dict[str, Any]] = None
+        context: Optional[Dict[str, Any]] = None
     ) -> Schema:
         ...
 
 elif PYDANTIC_V2:
     schema_validate = Schema.model_validate
 
 else:
```

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/security_requirement.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/security_requirement.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/security_scheme.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/security_scheme.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/server.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/server.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/server_variable.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/server_variable.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/tag.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/tag.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/openapi_pydantic/v3/v3_1_0/xml.py` & `openapi_pydantic-0.3.2/openapi_pydantic/v3/v3_1_0/xml.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.3.1/pyproject.toml` & `openapi_pydantic-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openapi-pydantic"
-version = "0.3.1"
+version = "0.3.2"
 description = "Pydantic OpenAPI schema implementation"
 authors = ["Mike Oakley <mike-oakley@users.noreply.github.com>"]
 readme = "README.md"
 repository = "https://github.com/mike-oakley/openapi-pydantic"
 license = "MIT"
 keywords = [
   "openapi",
```

### Comparing `openapi_pydantic-0.3.1/PKG-INFO` & `openapi_pydantic-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-pydantic
-Version: 0.3.1
+Version: 0.3.2
 Summary: Pydantic OpenAPI schema implementation
 Home-page: https://github.com/mike-oakley/openapi-pydantic
 License: MIT
 Keywords: openapi,schema,parser,pydantic,validation
 Author: Mike Oakley
 Author-email: mike-oakley@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
```

