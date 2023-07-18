# Comparing `tmp/stigg_api_client_v2-0.491.3.tar.gz` & `tmp/stigg_api_client_v2-0.491.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.491.3.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.491.8.tar", max compression
```

## Comparing `stigg_api_client_v2-0.491.3.tar` & `stigg_api_client_v2-0.491.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1644 2023-07-17 13:49:28.255658 stigg_api_client_v2-0.491.3/README.md
--rw-r--r--   0        0        0      432 2023-07-17 13:50:21.216693 stigg_api_client_v2-0.491.3/pyproject.toml
--rw-r--r--   0        0        0       62 2023-07-17 13:49:28.259658 stigg_api_client_v2-0.491.3/stigg/__init__.py
--rw-r--r--   0        0        0     1520 2023-07-17 13:49:28.259658 stigg_api_client_v2-0.491.3/stigg/client.py
--rw-r--r--   0        0        0    40220 2023-07-17 13:50:19.180501 stigg_api_client_v2-0.491.3/stigg/generated/__init__.py
--rw-r--r--   0        0        0      460 2023-07-17 13:50:17.520344 stigg_api_client_v2-0.491.3/stigg/generated/archive_customer.py
--rw-r--r--   0        0        0     7303 2023-07-17 13:50:18.572443 stigg_api_client_v2-0.491.3/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0    68032 2023-07-17 13:50:18.836468 stigg_api_client_v2-0.491.3/stigg/generated/async_client.py
--rw-r--r--   0        0        0     2731 2023-07-17 13:50:12.455864 stigg_api_client_v2-0.491.3/stigg/generated/base_client.py
--rw-r--r--   0        0        0     1951 2023-07-17 13:50:18.572443 stigg_api_client_v2-0.491.3/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-07-17 13:50:17.456338 stigg_api_client_v2-0.491.3/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-07-17 13:50:17.476340 stigg_api_client_v2-0.491.3/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    67605 2023-07-17 13:50:12.715888 stigg_api_client_v2-0.491.3/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-07-17 13:50:17.508343 stigg_api_client_v2-0.491.3/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0    24352 2023-07-17 13:50:14.672074 stigg_api_client_v2-0.491.3/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-07-17 13:50:17.464339 stigg_api_client_v2-0.491.3/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-07-17 13:50:17.472339 stigg_api_client_v2-0.491.3/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-07-17 13:50:18.572443 stigg_api_client_v2-0.491.3/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    56214 2023-07-17 13:50:18.568443 stigg_api_client_v2-0.491.3/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-07-17 13:50:17.536345 stigg_api_client_v2-0.491.3/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-07-17 13:50:17.548347 stigg_api_client_v2-0.491.3/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-07-17 13:50:17.528345 stigg_api_client_v2-0.491.3/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-07-17 13:50:17.596351 stigg_api_client_v2-0.491.3/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-07-17 13:50:17.568349 stigg_api_client_v2-0.491.3/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-07-17 13:50:17.560348 stigg_api_client_v2-0.491.3/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-07-17 13:50:17.604352 stigg_api_client_v2-0.491.3/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-07-17 13:50:17.552347 stigg_api_client_v2-0.491.3/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-07-17 13:50:17.576349 stigg_api_client_v2-0.491.3/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-07-17 13:50:17.588350 stigg_api_client_v2-0.491.3/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-07-17 13:50:17.416334 stigg_api_client_v2-0.491.3/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-07-17 13:50:17.408333 stigg_api_client_v2-0.491.3/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-07-17 13:50:17.440336 stigg_api_client_v2-0.491.3/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0   126904 2023-07-17 13:50:17.388332 stigg_api_client_v2-0.491.3/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-07-17 13:50:17.516343 stigg_api_client_v2-0.491.3/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-07-17 13:50:17.404333 stigg_api_client_v2-0.491.3/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-07-17 13:50:17.436336 stigg_api_client_v2-0.491.3/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-07-17 13:50:17.496342 stigg_api_client_v2-0.491.3/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      301 2023-07-17 13:50:17.492341 stigg_api_client_v2-0.491.3/stigg/generated/report_event.py
--rw-r--r--   0        0        0      637 2023-07-17 13:50:17.488341 stigg_api_client_v2-0.491.3/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-07-17 13:50:18.576444 stigg_api_client_v2-0.491.3/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-07-17 13:50:17.424335 stigg_api_client_v2-0.491.3/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-07-17 13:50:17.448337 stigg_api_client_v2-0.491.3/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      445 2023-07-17 13:50:17.612353 stigg_api_client_v2-0.491.3/stigg/generated/usage_history.py
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.491.3/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-07-18 12:53:51.949091 stigg_api_client_v2-0.491.8/README.md
+-rw-r--r--   0        0        0      432 2023-07-18 12:54:54.101047 stigg_api_client_v2-0.491.8/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-07-18 12:53:51.949091 stigg_api_client_v2-0.491.8/stigg/__init__.py
+-rw-r--r--   0        0        0     1520 2023-07-18 12:53:51.949091 stigg_api_client_v2-0.491.8/stigg/client.py
+-rw-r--r--   0        0        0    40220 2023-07-18 12:54:51.893039 stigg_api_client_v2-0.491.8/stigg/generated/__init__.py
+-rw-r--r--   0        0        0      460 2023-07-18 12:54:49.997032 stigg_api_client_v2-0.491.8/stigg/generated/archive_customer.py
+-rw-r--r--   0        0        0     7303 2023-07-18 12:54:51.225036 stigg_api_client_v2-0.491.8/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0    68208 2023-07-18 12:54:51.533038 stigg_api_client_v2-0.491.8/stigg/generated/async_client.py
+-rw-r--r--   0        0        0     2731 2023-07-18 12:54:44.257008 stigg_api_client_v2-0.491.8/stigg/generated/base_client.py
+-rw-r--r--   0        0        0     1951 2023-07-18 12:54:51.225036 stigg_api_client_v2-0.491.8/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-07-18 12:54:49.925032 stigg_api_client_v2-0.491.8/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-07-18 12:54:49.949032 stigg_api_client_v2-0.491.8/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    67781 2023-07-18 12:54:44.561010 stigg_api_client_v2-0.491.8/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-07-18 12:54:49.981032 stigg_api_client_v2-0.491.8/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0    24352 2023-07-18 12:54:46.705018 stigg_api_client_v2-0.491.8/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-07-18 12:54:49.933032 stigg_api_client_v2-0.491.8/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-07-18 12:54:49.941032 stigg_api_client_v2-0.491.8/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-07-18 12:54:51.225036 stigg_api_client_v2-0.491.8/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    56253 2023-07-18 12:54:51.221037 stigg_api_client_v2-0.491.8/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-07-18 12:54:50.013032 stigg_api_client_v2-0.491.8/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-07-18 12:54:50.029032 stigg_api_client_v2-0.491.8/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-07-18 12:54:50.005032 stigg_api_client_v2-0.491.8/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-07-18 12:54:50.081032 stigg_api_client_v2-0.491.8/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-07-18 12:54:50.045032 stigg_api_client_v2-0.491.8/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-07-18 12:54:50.041032 stigg_api_client_v2-0.491.8/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-07-18 12:54:50.093032 stigg_api_client_v2-0.491.8/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-07-18 12:54:50.033032 stigg_api_client_v2-0.491.8/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-07-18 12:54:50.057032 stigg_api_client_v2-0.491.8/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-07-18 12:54:50.073032 stigg_api_client_v2-0.491.8/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-07-18 12:54:49.881031 stigg_api_client_v2-0.491.8/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-07-18 12:54:49.873031 stigg_api_client_v2-0.491.8/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-07-18 12:54:49.909031 stigg_api_client_v2-0.491.8/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0   126904 2023-07-18 12:54:49.853031 stigg_api_client_v2-0.491.8/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-07-18 12:54:49.989032 stigg_api_client_v2-0.491.8/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-07-18 12:54:49.869032 stigg_api_client_v2-0.491.8/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-07-18 12:54:49.901032 stigg_api_client_v2-0.491.8/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-07-18 12:54:49.973032 stigg_api_client_v2-0.491.8/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      301 2023-07-18 12:54:49.965032 stigg_api_client_v2-0.491.8/stigg/generated/report_event.py
+-rw-r--r--   0        0        0      637 2023-07-18 12:54:49.961032 stigg_api_client_v2-0.491.8/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-07-18 12:54:51.229036 stigg_api_client_v2-0.491.8/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-07-18 12:54:49.889032 stigg_api_client_v2-0.491.8/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-07-18 12:54:49.917032 stigg_api_client_v2-0.491.8/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      445 2023-07-18 12:54:50.101032 stigg_api_client_v2-0.491.8/stigg/generated/usage_history.py
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.491.8/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.491.3/README.md` & `stigg_api_client_v2-0.491.8/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.491.3/stigg/client.py` & `stigg_api_client_v2-0.491.8/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.491.3/stigg/generated/__init__.py` & `stigg_api_client_v2-0.491.8/stigg/generated/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 13:50
+# Generated by ariadne-codegen on 2023-07-18 12:54
 
 from .archive_customer import ArchiveCustomer, ArchiveCustomerArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .async_client import AsyncClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
```

### Comparing `stigg_api_client_v2-0.491.3/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.491.8/stigg/generated/async_base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 13:50
+# Generated by ariadne-codegen on 2023-07-18 12:54
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.491.3/stigg/generated/async_client.py` & `stigg_api_client_v2-0.491.8/stigg/generated/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 13:50
+# Generated by ariadne-codegen on 2023-07-18 12:54
 # Source: operations.graphql
 
 from .archive_customer import ArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
@@ -92,14 +92,15 @@
               maxUnitQuantity
               billingCountryCode
               price {
                 amount
                 currency
               }
               feature {
+                refId
                 featureUnits
                 featureUnitsPlural
                 displayName
                 description
               }
             }
 
@@ -270,14 +271,15 @@
               maxUnitQuantity
               billingCountryCode
               price {
                 amount
                 currency
               }
               feature {
+                refId
                 featureUnits
                 featureUnitsPlural
                 displayName
                 description
               }
             }
 
@@ -381,14 +383,15 @@
               maxUnitQuantity
               billingCountryCode
               price {
                 amount
                 currency
               }
               feature {
+                refId
                 featureUnits
                 featureUnitsPlural
                 displayName
                 description
               }
             }
 
@@ -477,14 +480,15 @@
               maxUnitQuantity
               billingCountryCode
               price {
                 amount
                 currency
               }
               feature {
+                refId
                 featureUnits
                 featureUnitsPlural
                 displayName
                 description
               }
             }
 
@@ -804,14 +808,15 @@
               maxUnitQuantity
               billingCountryCode
               price {
                 amount
                 currency
               }
               feature {
+                refId
                 featureUnits
                 featureUnitsPlural
                 displayName
                 description
               }
             }
 
@@ -1063,14 +1068,15 @@
               maxUnitQuantity
               billingCountryCode
               price {
                 amount
                 currency
               }
               feature {
+                refId
                 featureUnits
                 featureUnitsPlural
                 displayName
                 description
               }
             }
 
@@ -1299,14 +1305,15 @@
               maxUnitQuantity
               billingCountryCode
               price {
                 amount
                 currency
               }
               feature {
+                refId
                 featureUnits
                 featureUnitsPlural
                 displayName
                 description
               }
             }
 
@@ -1673,14 +1680,15 @@
               maxUnitQuantity
               billingCountryCode
               price {
                 amount
                 currency
               }
               feature {
+                refId
                 featureUnits
                 featureUnitsPlural
                 displayName
                 description
               }
             }
```

### Comparing `stigg_api_client_v2-0.491.3/stigg/generated/base_client.py` & `stigg_api_client_v2-0.491.8/stigg/generated/base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 13:50
+# Generated by ariadne-codegen on 2023-07-18 12:54
 
 import json
 from typing import Any, Dict, Optional, TypeVar, cast
 
 import httpx
 from pydantic import BaseModel
 from pydantic.json import pydantic_encoder
```

### Comparing `stigg_api_client_v2-0.491.3/stigg/generated/base_model.py` & `stigg_api_client_v2-0.491.8/stigg/generated/base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 13:50
+# Generated by ariadne-codegen on 2023-07-18 12:54
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.491.3/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.491.8/stigg/generated/cancel_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 13:50
+# Generated by ariadne-codegen on 2023-07-18 12:54
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.491.3/stigg/generated/client.py` & `stigg_api_client_v2-0.491.8/stigg/generated/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 13:50
+# Generated by ariadne-codegen on 2023-07-18 12:54
 # Source: operations.graphql
 
 from .archive_customer import ArchiveCustomer
 from .base_client import BaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
@@ -90,14 +90,15 @@
               maxUnitQuantity
               billingCountryCode
               price {
                 amount
                 currency
               }
               feature {
+                refId
                 featureUnits
                 featureUnitsPlural
                 displayName
                 description
               }
             }
 
@@ -266,14 +267,15 @@
               maxUnitQuantity
               billingCountryCode
               price {
                 amount
                 currency
               }
               feature {
+                refId
                 featureUnits
                 featureUnitsPlural
                 displayName
                 description
               }
             }
 
@@ -375,14 +377,15 @@
               maxUnitQuantity
               billingCountryCode
               price {
                 amount
                 currency
               }
               feature {
+                refId
                 featureUnits
                 featureUnitsPlural
                 displayName
                 description
               }
             }
 
@@ -471,14 +474,15 @@
               maxUnitQuantity
               billingCountryCode
               price {
                 amount
                 currency
               }
               feature {
+                refId
                 featureUnits
                 featureUnitsPlural
                 displayName
                 description
               }
             }
 
@@ -798,14 +802,15 @@
               maxUnitQuantity
               billingCountryCode
               price {
                 amount
                 currency
               }
               feature {
+                refId
                 featureUnits
                 featureUnitsPlural
                 displayName
                 description
               }
             }
 
@@ -1055,14 +1060,15 @@
               maxUnitQuantity
               billingCountryCode
               price {
                 amount
                 currency
               }
               feature {
+                refId
                 featureUnits
                 featureUnitsPlural
                 displayName
                 description
               }
             }
 
@@ -1291,14 +1297,15 @@
               maxUnitQuantity
               billingCountryCode
               price {
                 amount
                 currency
               }
               feature {
+                refId
                 featureUnits
                 featureUnitsPlural
                 displayName
                 description
               }
             }
 
@@ -1665,14 +1672,15 @@
               maxUnitQuantity
               billingCountryCode
               price {
                 amount
                 currency
               }
               feature {
+                refId
                 featureUnits
                 featureUnitsPlural
                 displayName
                 description
               }
             }
```

### Comparing `stigg_api_client_v2-0.491.3/stigg/generated/create_subscription.py` & `stigg_api_client_v2-0.491.8/stigg/generated/create_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 13:50
+# Generated by ariadne-codegen on 2023-07-18 12:54
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.491.3/stigg/generated/enums.py` & `stigg_api_client_v2-0.491.8/stigg/generated/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 13:50
+# Generated by ariadne-codegen on 2023-07-18 12:54
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
     CustomerIsArchived = "CustomerIsArchived"
```

### Comparing `stigg_api_client_v2-0.491.3/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.491.8/stigg/generated/estimate_subscription.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 13:50
+# Generated by ariadne-codegen on 2023-07-18 12:54
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.491.3/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.491.8/stigg/generated/estimate_subscription_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 13:50
+# Generated by ariadne-codegen on 2023-07-18 12:54
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.491.3/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.491.8/stigg/generated/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 13:50
+# Generated by ariadne-codegen on 2023-07-18 12:54
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.491.3/stigg/generated/fragments.py` & `stigg_api_client_v2-0.491.8/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 13:50
+# Generated by ariadne-codegen on 2023-07-18 12:54
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -49,14 +49,15 @@
 
 class PriceFragmentPrice(BaseModel):
     amount: float
     currency: Currency
 
 
 class PriceFragmentFeature(BaseModel):
+    ref_id: str = Field(alias="refId")
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
 
 
 class PackageEntitlementFragment(BaseModel):
@@ -124,14 +125,25 @@
     status: SyncStatus
 
 
 class CouponFragmentCustomers(BaseModel):
     id: str
 
 
+class SlimCustomerFragment(BaseModel):
+    id: str
+    name: Optional[str]
+    email: Optional[str]
+    created_at: Optional[Any] = Field(alias="createdAt")
+    updated_at: Any = Field(alias="updatedAt")
+    ref_id: str = Field(alias="refId")
+    billing_id: Optional[str] = Field(alias="billingId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class PromotionalEntitlementFragment(BaseModel):
     status: PromotionalEntitlementStatus
     usage_limit: Optional[float] = Field(alias="usageLimit")
     feature_id: str = Field(alias="featureId")
     has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
     reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
     end_date: Optional[Any] = Field(alias="endDate")
@@ -146,25 +158,14 @@
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     ref_id: str = Field(alias="refId")
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
 
 
-class SlimCustomerFragment(BaseModel):
-    id: str
-    name: Optional[str]
-    email: Optional[str]
-    created_at: Optional[Any] = Field(alias="createdAt")
-    updated_at: Any = Field(alias="updatedAt")
-    ref_id: str = Field(alias="refId")
-    billing_id: Optional[str] = Field(alias="billingId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class CustomerFragment(SlimCustomerFragment):
     has_payment_method: bool = Field(alias="hasPaymentMethod")
     has_active_subscription: bool = Field(alias="hasActiveSubscription")
     default_payment_expiration_month: Optional[int] = Field(
         alias="defaultPaymentExpirationMonth"
     )
     default_payment_expiration_year: Optional[int] = Field(
@@ -328,21 +329,54 @@
     weekly_according_to: Optional[WeeklyAccordingTo] = Field(alias="weeklyAccordingTo")
 
 
 class CustomerPortalEntitlementFeature(FeatureFragment):
     pass
 
 
+class CustomerResourceFragment(BaseModel):
+    resource_id: str = Field(alias="resourceId")
+
+
+class CustomerPortalPromotionalEntitlement(BaseModel):
+    display_name: str = Field(alias="displayName")
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    period: PromotionalEntitlementPeriod
+    start_date: Any = Field(alias="startDate")
+    end_date: Optional[Any] = Field(alias="endDate")
+
+
 class CustomerPortalSubscriptionAddon(BaseModel):
     addon_id: str = Field(alias="addonId")
     description: Optional[str]
     display_name: str = Field(alias="displayName")
     quantity: int
 
 
+class CustomerPortalSubscriptionPriceFragment(BaseModel):
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+    billing_model: Optional[BillingModel] = Field(alias="billingModel")
+    price: Optional["CustomerPortalSubscriptionPriceFragmentPrice"]
+    feature: Optional["CustomerPortalSubscriptionPriceFragmentFeature"]
+
+
+class CustomerPortalSubscriptionPriceFragmentPrice(BaseModel):
+    amount: float
+    currency: Currency
+
+
+class CustomerPortalSubscriptionPriceFragmentFeature(BaseModel):
+    id: str
+    ref_id: str = Field(alias="refId")
+    display_name: str = Field(alias="displayName")
+    feature_units: Optional[str] = Field(alias="featureUnits")
+    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+
+
 class CustomerPortalSubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
     scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
     target_package: Optional[
@@ -387,34 +421,14 @@
     BaseModel
 ):
     typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
     new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
     feature_id: Optional[str] = Field(alias="featureId")
 
 
-class CustomerPortalSubscriptionPriceFragment(BaseModel):
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
-    billing_model: Optional[BillingModel] = Field(alias="billingModel")
-    price: Optional["CustomerPortalSubscriptionPriceFragmentPrice"]
-    feature: Optional["CustomerPortalSubscriptionPriceFragmentFeature"]
-
-
-class CustomerPortalSubscriptionPriceFragmentPrice(BaseModel):
-    amount: float
-    currency: Currency
-
-
-class CustomerPortalSubscriptionPriceFragmentFeature(BaseModel):
-    id: str
-    ref_id: str = Field(alias="refId")
-    display_name: str = Field(alias="displayName")
-    feature_units: Optional[str] = Field(alias="featureUnits")
-    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
-
-
 class CustomerPortalSubscriptionFragment(BaseModel):
     subscription_id: str = Field(alias="subscriptionId")
     plan_name: str = Field(alias="planName")
     pricing_type: PricingType = Field(alias="pricingType")
     prices: List["CustomerPortalSubscriptionFragmentPrices"]
     pricing: "CustomerPortalSubscriptionFragmentPricing"
     status: SubscriptionStatus
@@ -492,27 +506,14 @@
 
 class CustomerPortalSubscriptionFragmentScheduledUpdates(
     CustomerPortalSubscriptionScheduledUpdateData
 ):
     pass
 
 
-class CustomerResourceFragment(BaseModel):
-    resource_id: str = Field(alias="resourceId")
-
-
-class CustomerPortalPromotionalEntitlement(BaseModel):
-    display_name: str = Field(alias="displayName")
-    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    period: PromotionalEntitlementPeriod
-    start_date: Any = Field(alias="startDate")
-    end_date: Optional[Any] = Field(alias="endDate")
-
-
 class CustomerPortalFragment(BaseModel):
     subscriptions: List["CustomerPortalFragmentSubscriptions"]
     entitlements: List["CustomerPortalFragmentEntitlements"]
     promotional_entitlements: List[
         "CustomerPortalFragmentPromotionalEntitlements"
     ] = Field(alias="promotionalEntitlements")
     billing_information: "CustomerPortalFragmentBillingInformation" = Field(
@@ -547,14 +548,65 @@
     pass
 
 
 class CustomerPortalFragmentResource(CustomerResourceFragment):
     pass
 
 
+class SubscriptionScheduledUpdateData(BaseModel):
+    subscription_schedule_type: SubscriptionScheduleType = Field(
+        alias="subscriptionScheduleType"
+    )
+    schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
+    scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
+    target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
+        alias="targetPackage"
+    )
+    schedule_variables: Optional[
+        Annotated[
+            Union[
+                "SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables",
+                "SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables",
+                "SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables",
+            ],
+            Field(discriminator="typename__"),
+        ]
+    ] = Field(alias="scheduleVariables")
+
+
+class SubscriptionScheduledUpdateDataTargetPackage(BaseModel):
+    id: str
+    ref_id: str = Field(alias="refId")
+    display_name: str = Field(alias="displayName")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables(
+    BaseModel
+):
+    typename__: Literal["BillingPeriodChangeVariables"] = Field(alias="__typename")
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables(
+    BaseModel
+):
+    typename__: Literal["DowngradeChangeVariables"] = Field(alias="__typename")
+    addon_ref_ids: Optional[str] = Field(alias="addonRefIds")
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+    downgrade_plan_ref_id: str = Field(alias="downgradePlanRefId")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables(
+    BaseModel
+):
+    typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
+    new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
+    feature_id: Optional[str] = Field(alias="featureId")
+
+
 class ProductFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: Optional[str] = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     product_settings: "ProductFragmentProductSettings" = Field(alias="productSettings")
 
@@ -619,65 +671,14 @@
 
 
 class PlanFragmentDefaultTrialConfig(BaseModel):
     duration: float
     units: TrialPeriodUnits
 
 
-class SubscriptionScheduledUpdateData(BaseModel):
-    subscription_schedule_type: SubscriptionScheduleType = Field(
-        alias="subscriptionScheduleType"
-    )
-    schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
-    scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
-    target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
-        alias="targetPackage"
-    )
-    schedule_variables: Optional[
-        Annotated[
-            Union[
-                "SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables",
-                "SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables",
-                "SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables",
-            ],
-            Field(discriminator="typename__"),
-        ]
-    ] = Field(alias="scheduleVariables")
-
-
-class SubscriptionScheduledUpdateDataTargetPackage(BaseModel):
-    id: str
-    ref_id: str = Field(alias="refId")
-    display_name: str = Field(alias="displayName")
-
-
-class SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables(
-    BaseModel
-):
-    typename__: Literal["BillingPeriodChangeVariables"] = Field(alias="__typename")
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
-
-
-class SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables(
-    BaseModel
-):
-    typename__: Literal["DowngradeChangeVariables"] = Field(alias="__typename")
-    addon_ref_ids: Optional[str] = Field(alias="addonRefIds")
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
-    downgrade_plan_ref_id: str = Field(alias="downgradePlanRefId")
-
-
-class SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables(
-    BaseModel
-):
-    typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
-    new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
-    feature_id: Optional[str] = Field(alias="featureId")
-
-
 class TotalPriceFragment(BaseModel):
     sub_total: "TotalPriceFragmentSubTotal" = Field(alias="subTotal")
     total: "TotalPriceFragmentTotal"
 
 
 class TotalPriceFragmentSubTotal(BaseModel):
     amount: float
@@ -1350,17 +1351,17 @@
 PackageEntitlementFragmentFeature.update_forward_refs()
 AddonFragment.update_forward_refs()
 AddonFragmentEntitlements.update_forward_refs()
 AddonFragmentPrices.update_forward_refs()
 CouponFragment.update_forward_refs()
 CouponFragmentSyncStates.update_forward_refs()
 CouponFragmentCustomers.update_forward_refs()
+SlimCustomerFragment.update_forward_refs()
 PromotionalEntitlementFragment.update_forward_refs()
 PromotionalEntitlementFragmentFeature.update_forward_refs()
-SlimCustomerFragment.update_forward_refs()
 CustomerFragment.update_forward_refs()
 CustomerFragmentTrialedPlans.update_forward_refs()
 CustomerFragmentExperimentInfo.update_forward_refs()
 CustomerFragmentCoupon.update_forward_refs()
 CustomerFragmentEligibleForTrial.update_forward_refs()
 CustomerFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalBillingInformation.update_forward_refs()
@@ -1374,60 +1375,60 @@
 CustomerPortalConfigurationFragmentPalette.update_forward_refs()
 CustomerPortalConfigurationFragmentTypography.update_forward_refs()
 FeatureFragment.update_forward_refs()
 CustomerPortalEntitlement.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationMonthlyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationWeeklyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementFeature.update_forward_refs()
+CustomerResourceFragment.update_forward_refs()
+CustomerPortalPromotionalEntitlement.update_forward_refs()
 CustomerPortalSubscriptionAddon.update_forward_refs()
+CustomerPortalSubscriptionPriceFragment.update_forward_refs()
+CustomerPortalSubscriptionPriceFragmentPrice.update_forward_refs()
+CustomerPortalSubscriptionPriceFragmentFeature.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateData.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
-CustomerPortalSubscriptionPriceFragment.update_forward_refs()
-CustomerPortalSubscriptionPriceFragmentPrice.update_forward_refs()
-CustomerPortalSubscriptionPriceFragmentFeature.update_forward_refs()
 CustomerPortalSubscriptionFragment.update_forward_refs()
 CustomerPortalSubscriptionFragmentPrices.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricing.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingFeature.update_forward_refs()
 CustomerPortalSubscriptionFragmentBillingPeriodRange.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceSubTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceAddonsTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentAddons.update_forward_refs()
 CustomerPortalSubscriptionFragmentScheduledUpdates.update_forward_refs()
-CustomerResourceFragment.update_forward_refs()
-CustomerPortalPromotionalEntitlement.update_forward_refs()
 CustomerPortalFragment.update_forward_refs()
 CustomerPortalFragmentSubscriptions.update_forward_refs()
 CustomerPortalFragmentEntitlements.update_forward_refs()
 CustomerPortalFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalFragmentBillingInformation.update_forward_refs()
 CustomerPortalFragmentConfiguration.update_forward_refs()
 CustomerPortalFragmentResource.update_forward_refs()
+SubscriptionScheduledUpdateData.update_forward_refs()
+SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 ProductFragment.update_forward_refs()
 ProductFragmentProductSettings.update_forward_refs()
 ProductFragmentProductSettingsDowngradePlan.update_forward_refs()
 PlanFragment.update_forward_refs()
 PlanFragmentProduct.update_forward_refs()
 PlanFragmentBasePlan.update_forward_refs()
 PlanFragmentEntitlements.update_forward_refs()
 PlanFragmentInheritedEntitlements.update_forward_refs()
 PlanFragmentCompatibleAddons.update_forward_refs()
 PlanFragmentPrices.update_forward_refs()
 PlanFragmentDefaultTrialConfig.update_forward_refs()
-SubscriptionScheduledUpdateData.update_forward_refs()
-SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 TotalPriceFragment.update_forward_refs()
 TotalPriceFragmentSubTotal.update_forward_refs()
 TotalPriceFragmentTotal.update_forward_refs()
 SubscriptionFragment.update_forward_refs()
 SubscriptionFragmentResource.update_forward_refs()
 SubscriptionFragmentExperimentInfo.update_forward_refs()
 SubscriptionFragmentPrices.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.491.3/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.491.8/stigg/generated/get_active_subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 13:50
+# Generated by ariadne-codegen on 2023-07-18 12:54
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.491.3/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.491.8/stigg/generated/get_coupons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 13:50
+# Generated by ariadne-codegen on 2023-07-18 12:54
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.491.3/stigg/generated/get_customer_by_id.py` & `stigg_api_client_v2-0.491.8/stigg/generated/get_customer_by_id.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 13:50
+# Generated by ariadne-codegen on 2023-07-18 12:54
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.491.3/stigg/generated/get_customer_portal_by_ref_id.py` & `stigg_api_client_v2-0.491.8/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 13:50
+# Generated by ariadne-codegen on 2023-07-18 12:54
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CustomerPortalFragment
```

### Comparing `stigg_api_client_v2-0.491.3/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.491.8/stigg/generated/get_mock_paywall.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 13:50
+# Generated by ariadne-codegen on 2023-07-18 12:54
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.491.3/stigg/generated/get_products.py` & `stigg_api_client_v2-0.491.8/stigg/generated/get_products.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 13:50
+# Generated by ariadne-codegen on 2023-07-18 12:54
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import ProductFragment
```

### Comparing `stigg_api_client_v2-0.491.3/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.491.8/stigg/generated/get_sdk_configuration.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 13:50
+# Generated by ariadne-codegen on 2023-07-18 12:54
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.491.3/stigg/generated/input_types.py` & `stigg_api_client_v2-0.491.8/stigg/generated/input_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 13:50
+# Generated by ariadne-codegen on 2023-07-18 12:54
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.491.3/stigg/generated/migrate_subscription_to_latest.py` & `stigg_api_client_v2-0.491.8/stigg/generated/migrate_subscription_to_latest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 13:50
+# Generated by ariadne-codegen on 2023-07-18 12:54
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.491.3/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.491.8/stigg/generated/provision_customer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 13:50
+# Generated by ariadne-codegen on 2023-07-18 12:54
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.491.3/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.491.8/stigg/generated/provision_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 13:50
+# Generated by ariadne-codegen on 2023-07-18 12:54
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.491.3/stigg/generated/report_usage.py` & `stigg_api_client_v2-0.491.8/stigg/generated/report_usage.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 13:50
+# Generated by ariadne-codegen on 2023-07-18 12:54
 # Source: operations.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.491.3/stigg/generated/update_subscription.py` & `stigg_api_client_v2-0.491.8/stigg/generated/update_subscription.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-17 13:50
+# Generated by ariadne-codegen on 2023-07-18 12:54
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.491.3/PKG-INFO` & `stigg_api_client_v2-0.491.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.491.3
+Version: 0.491.8
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

