# Comparing `tmp/openworld-sdk-python-fraudpreventionv2-1.2.1.tar.gz` & `tmp/openworld-sdk-python-fraudpreventionv2-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openworld-sdk-python-fraudpreventionv2-1.2.1.tar", last modified: Tue Jul 11 14:33:07 2023, max compression
+gzip compressed data, was "openworld-sdk-python-fraudpreventionv2-1.3.0.tar", last modified: Tue Jul 18 15:00:35 2023, max compression
```

## Comparing `openworld-sdk-python-fraudpreventionv2-1.2.1.tar` & `openworld-sdk-python-fraudpreventionv2-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:33:07.961057 openworld-sdk-python-fraudpreventionv2-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-11 14:33:07.961057 openworld-sdk-python-fraudpreventionv2-1.2.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:33:07.957057 openworld-sdk-python-fraudpreventionv2-1.2.1/openworld/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:33:07.957057 openworld-sdk-python-fraudpreventionv2-1.2.1/openworld/sdk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:33:07.961057 openworld-sdk-python-fraudpreventionv2-1.2.1/openworld/sdk/fraudpreventionv2/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-11 14:33:01.000000 openworld-sdk-python-fraudpreventionv2-1.2.1/openworld/sdk/fraudpreventionv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-07-11 14:33:01.000000 openworld-sdk-python-fraudpreventionv2-1.2.1/openworld/sdk/fraudpreventionv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    99892 2023-07-11 14:33:01.000000 openworld-sdk-python-fraudpreventionv2-1.2.1/openworld/sdk/fraudpreventionv2/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:33:07.961057 openworld-sdk-python-fraudpreventionv2-1.2.1/openworld_sdk_python_fraudpreventionv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-11 14:33:07.000000 openworld-sdk-python-fraudpreventionv2-1.2.1/openworld_sdk_python_fraudpreventionv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-11 14:33:07.000000 openworld-sdk-python-fraudpreventionv2-1.2.1/openworld_sdk_python_fraudpreventionv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:33:07.000000 openworld-sdk-python-fraudpreventionv2-1.2.1/openworld_sdk_python_fraudpreventionv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-11 14:33:07.000000 openworld-sdk-python-fraudpreventionv2-1.2.1/openworld_sdk_python_fraudpreventionv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 14:33:07.000000 openworld-sdk-python-fraudpreventionv2-1.2.1/openworld_sdk_python_fraudpreventionv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:33:07.961057 openworld-sdk-python-fraudpreventionv2-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-11 14:32:53.000000 openworld-sdk-python-fraudpreventionv2-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:00:35.514364 openworld-sdk-python-fraudpreventionv2-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-18 15:00:35.514364 openworld-sdk-python-fraudpreventionv2-1.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:00:35.514364 openworld-sdk-python-fraudpreventionv2-1.3.0/openworld/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:00:35.514364 openworld-sdk-python-fraudpreventionv2-1.3.0/openworld/sdk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:00:35.514364 openworld-sdk-python-fraudpreventionv2-1.3.0/openworld/sdk/fraudpreventionv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-18 15:00:28.000000 openworld-sdk-python-fraudpreventionv2-1.3.0/openworld/sdk/fraudpreventionv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-07-18 15:00:28.000000 openworld-sdk-python-fraudpreventionv2-1.3.0/openworld/sdk/fraudpreventionv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118595 2023-07-18 15:00:28.000000 openworld-sdk-python-fraudpreventionv2-1.3.0/openworld/sdk/fraudpreventionv2/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:00:35.514364 openworld-sdk-python-fraudpreventionv2-1.3.0/openworld_sdk_python_fraudpreventionv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-18 15:00:35.000000 openworld-sdk-python-fraudpreventionv2-1.3.0/openworld_sdk_python_fraudpreventionv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-18 15:00:35.000000 openworld-sdk-python-fraudpreventionv2-1.3.0/openworld_sdk_python_fraudpreventionv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:00:35.000000 openworld-sdk-python-fraudpreventionv2-1.3.0/openworld_sdk_python_fraudpreventionv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-18 15:00:35.000000 openworld-sdk-python-fraudpreventionv2-1.3.0/openworld_sdk_python_fraudpreventionv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 15:00:35.000000 openworld-sdk-python-fraudpreventionv2-1.3.0/openworld_sdk_python_fraudpreventionv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 15:00:35.514364 openworld-sdk-python-fraudpreventionv2-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-18 15:00:21.000000 openworld-sdk-python-fraudpreventionv2-1.3.0/setup.py
```

### Comparing `openworld-sdk-python-fraudpreventionv2-1.2.1/PKG-INFO` & `openworld-sdk-python-fraudpreventionv2-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openworld-sdk-python-fraudpreventionv2
-Version: 1.2.1
+Version: 1.3.0
 Summary: Open World F r a u d P r e v e n t i o n V 2 SDK for Python
 Home-page: https://github.com/ExpediaGroup/openworld-sdk-python
 Author: Expedia Group
 Author-email: oss@expediagroup.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
```

### Comparing `openworld-sdk-python-fraudpreventionv2-1.2.1/openworld/sdk/fraudpreventionv2/__init__.py` & `openworld-sdk-python-fraudpreventionv2-1.3.0/openworld/sdk/fraudpreventionv2/__init__.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-fraudpreventionv2-1.2.1/openworld/sdk/fraudpreventionv2/client.py` & `openworld-sdk-python-fraudpreventionv2-1.3.0/openworld/sdk/fraudpreventionv2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         r"""F r a u d P r e v e n t i o n V 2 API Client.
 
         Args:
             client_config(ClientConfig): SDK Client Configurations Holder.
         """
         python_version = platform.python_version()
         os_name, os_version, *_ = platform.platform().split('-')
-        sdk_metadata = f'open-world-sdk-python-fraudpreventionv2/1.2.1'
+        sdk_metadata = f'open-world-sdk-python-fraudpreventionv2/1.3.0'
 
         self.__api_client = ApiClient(client_config, _OpenWorldAuthClient)
 
         self.__user_agent = f'{sdk_metadata} (Python {python_version}; {os_name} {os_version})'
 
     def screen(
         self, transaction_id: UUID = uuid4(), body: OrderPurchaseScreenRequest = None
```

### Comparing `openworld-sdk-python-fraudpreventionv2-1.2.1/openworld/sdk/fraudpreventionv2/model.py` & `openworld-sdk-python-fraudpreventionv2-1.3.0/openworld/sdk/fraudpreventionv2/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import Any, List, Literal, Optional, Union
 
-from pydantic import BaseModel, EmailStr, Extra, Field, constr
+from pydantic import BaseModel, EmailStr, Extra, Field, confloat, conint, constr
 
 
 class Code(
     Enum,
 ):
     r"""pydantic model Code: Snake cased all caps error code interpreted from the HTTP status code that can programmatically be acted upon.
     Attributes:
@@ -230,27 +230,27 @@
     smart_union=True,
     extra=Extra.forbid,
 ):
     r"""pydantic model CancellationReason: Reason of order update cancellation.
     Attributes:
         primary_reason_code(Optional[constr(max_length=200)], optional): Primary cancellation reason code.
         sub_reason_code(Optional[constr(max_length=200)], optional): Substitute cancellation reason code.
-        primary_reason_description(constr(max_length=200)): Primary cancellation reason code. Required if `order_status = CANCELLED`.
+        primary_reason_description(Optional[constr(max_length=200)], optional): Primary cancellation reason code. Required if `order_status = CANCELLED`.
         sub_reason_description(Optional[constr(max_length=200)], optional): Substitute cancellation reason description.
 
     """
     primary_reason_code: Optional[constr(max_length=200)] = None
     """
     Primary cancellation reason code.
     """
     sub_reason_code: Optional[constr(max_length=200)] = None
     """
     Substitute cancellation reason code.
     """
-    primary_reason_description: constr(max_length=200) = None
+    primary_reason_description: Optional[constr(max_length=200)] = None
     """
     Primary cancellation reason code. Required if `order_status = CANCELLED`.
     """
     sub_reason_description: Optional[constr(max_length=200)] = None
     """
     Substitute cancellation reason description.
     """
@@ -671,14 +671,130 @@
     address: Address = None
     timezone: Optional[constr(max_length=200)] = Field(None, example='America/New_York')
     """
     The timezone associated with the location of the station, specifying the local time offset from Coordinated Universal Time (UTC).
     """
 
 
+class Activity(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
+    r"""pydantic model Activity: Provides essential details about a specific activity.
+    Attributes:
+        type(constr(max_length=200)): This field provides a categorization of the different types of activities available within the activity product. It is designed to accommodate the preferences of the API consumer, allowing them to assign a descriptive label or keyword that accurately represents the nature of each activity. Here are some suggested values for this field: | Adventures: This category includes activities such as hiking, zip-lining, rock climbing, bungee jumping, and other adventurous pursuits. | Air, Balloon & Helicopter Tours: This category offers activities like hot air balloon rides, helicopter tours, and aerial sightseeing experiences. | Cruises & Water Tours: This includes options such as boat cruises, yacht tours, river rafting, snorkeling, and diving expeditions. | Nightlife: This category encompasses activities like clubbing, pub crawls, live music events, and cultural performances. These activities predominantly occur during the evening or nighttime.
+        description(constr(max_length=200)): This field within the trip information provides additional details or a brief explanation about the specific trip or activity being described
+
+    """
+    type: constr(max_length=200) = Field(..., example='Balloon & Helicopter Tours')
+    """
+    This field provides a categorization of the different types of activities available within the activity product. It is designed to accommodate the preferences of the API consumer, allowing them to assign a descriptive label or keyword that accurately represents the nature of each activity. Here are some suggested values for this field: | Adventures: This category includes activities such as hiking, zip-lining, rock climbing, bungee jumping, and other adventurous pursuits. | Air, Balloon & Helicopter Tours: This category offers activities like hot air balloon rides, helicopter tours, and aerial sightseeing experiences. | Cruises & Water Tours: This includes options such as boat cruises, yacht tours, river rafting, snorkeling, and diving expeditions. | Nightlife: This category encompasses activities like clubbing, pub crawls, live music events, and cultural performances. These activities predominantly occur during the evening or nighttime.
+    """
+    description: constr(max_length=200) = Field(..., example='2-Day, 2 Day Ticket Weekend')
+    """
+    This field within the trip information provides additional details or a brief explanation about the specific trip or activity being described
+    """
+
+
+class Coordinates(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
+    r"""pydantic model Coordinates: Group of attributes intended to hold information about location coordinates.
+    Attributes:
+        latitude(Optional[confloat(ge=-90.0, le=90.0)], optional): The latitude in degrees. It must be in the range [-90.0, +90.0].
+        longitude(Optional[confloat(ge=-180.0, le=180.0)], optional): The longitude in degrees. It must be in the range [-180.0, +180.0].
+
+    """
+    latitude: Optional[confloat(ge=-90.0, le=90.0)] = None
+    """
+    The latitude in degrees. It must be in the range [-90.0, +90.0].
+    """
+    longitude: Optional[confloat(ge=-180.0, le=180.0)] = None
+    """
+    The longitude in degrees. It must be in the range [-180.0, +180.0].
+    """
+
+
+class Type1(
+    Enum,
+):
+    r"""pydantic model Type1: This field indicates the nature or relationship of the vendor associated with a particular activity. | THIRD_PARTY: This value indicates that the vendor is an external entity or third-party provider. | DIRECT: This value signifies that the vendor is a direct entity or provider associated with the organization or platform offering the activity.
+    Attributes:
+        THIRD_PARTY(Any): --
+        DIRECT(Any): --
+
+    """
+    THIRD_PARTY: Any = 'THIRD_PARTY'
+    DIRECT: Any = 'DIRECT'
+
+
+class OperatingCompanyModel(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
+    r"""pydantic model OperatingCompanyModel: This field helps to identify and understand the specific provider or operating company involved in offering the activity.
+    Attributes:
+        name(str): This field includes the provider's name.
+        type(Type1): This field indicates the nature or relationship of the vendor associated with a particular activity. | THIRD_PARTY: This value indicates that the vendor is an external entity or third-party provider. | DIRECT: This value signifies that the vendor is a direct entity or provider associated with the organization or platform offering the activity.
+
+    """
+    name: str = Field(..., example='VIATOR')
+    """
+    This field includes the provider's name.
+    """
+    type: Type1 = None
+    """
+    This field indicates the nature or relationship of the vendor associated with a particular activity. | THIRD_PARTY: This value indicates that the vendor is an external entity or third-party provider. | DIRECT: This value signifies that the vendor is a direct entity or provider associated with the organization or platform offering the activity.
+    """
+
+
+class Category(
+    Enum,
+):
+    r"""pydantic model Category: Describes the type or category of the ticket.
+    Attributes:
+        ADULT(Any): --
+        CHILD(Any): --
+        SENIOR(Any): --
+        STUDENT(Any): --
+        OTHER(Any): --
+
+    """
+    ADULT: Any = 'ADULT'
+    CHILD: Any = 'CHILD'
+    SENIOR: Any = 'SENIOR'
+    STUDENT: Any = 'STUDENT'
+    OTHER: Any = 'OTHER'
+
+
+class Ticket(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
+    r"""pydantic model Ticket: This field provides information about the tickets related to the activity.
+    Attributes:
+        category(Category): Describes the type or category of the ticket.
+        quantity(conint(ge=1, le=30)): This field represents the count or number of a specific ticket type associated with an activity.
+
+    """
+    category: Category = None
+    """
+    Describes the type or category of the ticket.
+    """
+    quantity: conint(ge=1, le=30) = None
+    """
+    This field represents the count or number of a specific ticket type associated with an activity.
+    """
+
+
 class FlightType(
     Enum,
 ):
     r"""pydantic model FlightType: Identifies the type of air trip based on the air destinations.
     Attributes:
         ROUNDTRIP(Any): --
         ONEWAY(Any): --
@@ -765,14 +881,50 @@
     * `VISA_ELECTRON`             : `VISA`
     * `CARTA_SI`                  : `VISA`
     * `CARTE_BLEUE`               : `VISA`
     * `VISA_DANKORT`              : `VISA`
     * `POSTEPAY_VISA_ELECTRON`    : `VISA`
     * `PAYPAL`                    :
 
+    'brand' with 'Points' payment_type is an enum value with following:
+    * `EXPEDIA_REWARDS`
+    * `AMEX_POINTS`
+    * `BANK_OF_AMERICA_REWARDS`
+    * `DISCOVER_POINTS`
+    * `MASTER_CARD_POINTS`
+    * `CITI_THANK_YOU_POINTS`
+    * `MERRILL_LYNCH_REWARDS`
+    * `WELLS_FARGO_POINTS`
+    * `DELTA_SKY_MILES`
+    * `UNITED_POINTS`
+    * `DISCOVER_MILES`
+    * `ALASKA_MILES`
+    * `RBC_REWARDS`
+    * `BILT_REWARDS`
+    * `ORBUCKS`
+    * `CHEAP_CASH`
+    * `BONUS_PLUS`
+    * `ULTIMATE_REWARDS`
+
+    'brand' with 'GiftCard' payment_type is an enum value with following:
+    * `GIFT_CARD`
+
+    'brand' with 'InternetBankPayment' payment_type is an enum value with following:
+    * `IBP`
+    * `LOCAL_DEBIT_CARD`
+    * `SOFORT`
+    * `YANDEX`
+    * `WEB_MONEY`
+    * `QIWI`
+    * `BITCOIN`
+
+    'brand' with 'DirectDebit' payment_type is an enum value with following:
+    * `EVL`
+    * `INTER_COMPANY`
+
     Attributes:
         AMERICAN_EXPRESS(Any): --
         DINERS_CLUB_INTERNATIONAL(Any): --
         BC_CARD(Any): --
         DISCOVER(Any): --
         JCB(Any): --
         MASTER_CARD(Any): --
@@ -785,14 +937,42 @@
         VISA_DELTA(Any): --
         VISA_ELECTRON(Any): --
         CARTA_SI(Any): --
         CARTE_BLEUE(Any): --
         VISA_DANKORT(Any): --
         POSTEPAY_VISA_ELECTRON(Any): --
         PAYPAL(Any): --
+        EXPEDIA_REWARDS(Any): --
+        AMEX_POINTS(Any): --
+        BANK_OF_AMERICA_REWARDS(Any): --
+        DISCOVER_POINTS(Any): --
+        MASTER_CARD_POINTS(Any): --
+        CITI_THANK_YOU_POINTS(Any): --
+        MERRILL_LYNCH_REWARDS(Any): --
+        WELLS_FARGO_POINTS(Any): --
+        DELTA_SKY_MILES(Any): --
+        UNITED_POINTS(Any): --
+        DISCOVER_MILES(Any): --
+        ALASKA_MILES(Any): --
+        RBC_REWARDS(Any): --
+        BILT_REWARDS(Any): --
+        ORBUCKS(Any): --
+        CHEAP_CASH(Any): --
+        BONUS_PLUS(Any): --
+        ULTIMATE_REWARDS(Any): --
+        GIFT_CARD(Any): --
+        IBP(Any): --
+        LOCAL_DEBIT_CARD(Any): --
+        SOFORT(Any): --
+        YANDEX(Any): --
+        WEB_MONEY(Any): --
+        QIWI(Any): --
+        BITCOIN(Any): --
+        EVL(Any): --
+        INTER_COMPANY(Any): --
 
     """
     AMERICAN_EXPRESS: Any = 'AMERICAN_EXPRESS'
     DINERS_CLUB_INTERNATIONAL: Any = 'DINERS_CLUB_INTERNATIONAL'
     BC_CARD: Any = 'BC_CARD'
     DISCOVER: Any = 'DISCOVER'
     JCB: Any = 'JCB'
@@ -806,14 +986,42 @@
     VISA_DELTA: Any = 'VISA_DELTA'
     VISA_ELECTRON: Any = 'VISA_ELECTRON'
     CARTA_SI: Any = 'CARTA_SI'
     CARTE_BLEUE: Any = 'CARTE_BLEUE'
     VISA_DANKORT: Any = 'VISA_DANKORT'
     POSTEPAY_VISA_ELECTRON: Any = 'POSTEPAY_VISA_ELECTRON'
     PAYPAL: Any = 'PAYPAL'
+    EXPEDIA_REWARDS: Any = 'EXPEDIA_REWARDS'
+    AMEX_POINTS: Any = 'AMEX_POINTS'
+    BANK_OF_AMERICA_REWARDS: Any = 'BANK_OF_AMERICA_REWARDS'
+    DISCOVER_POINTS: Any = 'DISCOVER_POINTS'
+    MASTER_CARD_POINTS: Any = 'MASTER_CARD_POINTS'
+    CITI_THANK_YOU_POINTS: Any = 'CITI_THANK_YOU_POINTS'
+    MERRILL_LYNCH_REWARDS: Any = 'MERRILL_LYNCH_REWARDS'
+    WELLS_FARGO_POINTS: Any = 'WELLS_FARGO_POINTS'
+    DELTA_SKY_MILES: Any = 'DELTA_SKY_MILES'
+    UNITED_POINTS: Any = 'UNITED_POINTS'
+    DISCOVER_MILES: Any = 'DISCOVER_MILES'
+    ALASKA_MILES: Any = 'ALASKA_MILES'
+    RBC_REWARDS: Any = 'RBC_REWARDS'
+    BILT_REWARDS: Any = 'BILT_REWARDS'
+    ORBUCKS: Any = 'ORBUCKS'
+    CHEAP_CASH: Any = 'CHEAP_CASH'
+    BONUS_PLUS: Any = 'BONUS_PLUS'
+    ULTIMATE_REWARDS: Any = 'ULTIMATE_REWARDS'
+    GIFT_CARD: Any = 'GIFT_CARD'
+    IBP: Any = 'IBP'
+    LOCAL_DEBIT_CARD: Any = 'LOCAL_DEBIT_CARD'
+    SOFORT: Any = 'SOFORT'
+    YANDEX: Any = 'YANDEX'
+    WEB_MONEY: Any = 'WEB_MONEY'
+    QIWI: Any = 'QIWI'
+    BITCOIN: Any = 'BITCOIN'
+    EVL: Any = 'EVL'
+    INTER_COMPANY: Any = 'INTER_COMPANY'
 
 
 class PaymentThreeDSCriteria(
     BaseModel,
     smart_union=True,
     extra=Extra.forbid,
 ):
@@ -883,45 +1091,53 @@
     COMPLETED: Any = 'COMPLETED'
     FAILED: Any = 'FAILED'
 
 
 class PaymentMethod(
     Enum,
 ):
-    r"""pydantic model PaymentMethod: The payment method used at the time of purchase for the transaction. Supported `method`'s are: `CREDIT_CARD`, `PAYPAL`, `POINTS`.
+    r"""pydantic model PaymentMethod: The payment method used at the time of purchase for the transaction. Supported `method`'s are: `CREDIT_CARD`, `PAYPAL`, `POINTS`, `GIFT_CARD`, `INTERNET_BANK_PAYMENT`, `DIRECT_DEBIT`.
     Attributes:
         CREDIT_CARD(Any): --
         PAYPAL(Any): --
         POINTS(Any): --
+        GIFT_CARD(Any): --
+        INTERNET_BANK_PAYMENT(Any): --
+        DIRECT_DEBIT(Any): --
 
     """
     CREDIT_CARD: Any = 'CREDIT_CARD'
     PAYPAL: Any = 'PAYPAL'
     POINTS: Any = 'POINTS'
+    GIFT_CARD: Any = 'GIFT_CARD'
+    INTERNET_BANK_PAYMENT: Any = 'INTERNET_BANK_PAYMENT'
+    DIRECT_DEBIT: Any = 'DIRECT_DEBIT'
 
 
 class TravelProductType(
     Enum,
 ):
     r"""pydantic model TravelProductType: Type of product.
     Attributes:
         CRUISE(Any): --
         AIR(Any): --
         CAR(Any): --
         INSURANCE(Any): --
         HOTEL(Any): --
         RAIL(Any): --
+        ACTIVITIES(Any): --
 
     """
     CRUISE: Any = 'CRUISE'
     AIR: Any = 'AIR'
     CAR: Any = 'CAR'
     INSURANCE: Any = 'INSURANCE'
     HOTEL: Any = 'HOTEL'
     RAIL: Any = 'RAIL'
+    ACTIVITIES: Any = 'ACTIVITIES'
 
 
 class CardType(
     Enum,
 ):
     r"""pydantic model CardType: The 'card_type' field value is an enum value which is associated with the payment method of the specific payment instrument.
     For credit card payment method ensure attributes mentioned in dictionary below are set to corresponding values only.
@@ -1305,21 +1521,22 @@
     r"""pydantic model TravelProduct: The `type` field value is used as a discriminator, with the following mapping:
     * `CRUISE`: `Cruise`
     * `AIR`: `Air`
     * `CAR`: `Car`
     * `INSURANCE`: `Insurance`
     * `HOTEL`: `Hotel`
     * `RAIL`: `Rail`
+    * `ACTIVITIES`: `Activities`
 
     Attributes:
         price(Amount): --
         type(TravelProductType): --
-        inventory_type(constr(max_length=30)): Type of inventory. Ensure attributes mentioned in dictionary below are set to corresponding values only. `inventory_type` has the following mapping with TravelProduct `type` attribute: *       inventory_type            :      type * ------------------------------------------------------ *  `Cruise`                       : `CRUISE` *  `Air`                          : `AIR` *  `Car`                          : `CAR` *  `Insurance`                    : `INSURANCE` *  `Hotel`                        : `HOTEL` *  `Rail`                         :  `RAIL`
+        inventory_type(constr(max_length=30)): Type of inventory. Ensure attributes mentioned in dictionary below are set to corresponding values only. `inventory_type` has the following mapping with TravelProduct `type` attribute: *       inventory_type            :      type * ------------------------------------------------------ *  `Cruise`                       : `CRUISE` *  `Air`                          : `AIR` *  `Car`                          : `CAR` *  `Insurance`                    : `INSURANCE` *  `Hotel`                        : `HOTEL` *  `Rail`                         :  `RAIL` *  `Activities`                   :  `ACTIVITIES`
         inventory_source(InventorySource): Identifies the business model through which the supply is being sold. Merchant/Agency. * `MERCHANT` is used when Partner is the merchant of record for this order. * `AGENCY` is used when this order is through an agency booking.
-        travelers_references(List[constr(max_length=50)]): List of travelerGuids who are part of the traveling party on the order for the product. Information for each product and its required travelers should be provided in the API request. If the product booking does not require accompanying quest information then that does not need to be provided in the API request. Example: * For Air products, all travelers' details are required to complete the booking. * For Hotel products, typically the details on the person checking-in is required. * For Car products, typically only the primary driver information is required. If multiple traveler details are in the itinerary, this structure allows to fill up traveler details once in the `travelers` section, and then associate individual products to the respective travelers. This association is made using `traveler_id` field. A GUID can be generated for each object in the `travelers` section. The same GUID can be provided in the `traveler_references` below. The `travelers` array should have at least one `traveler` object, and each `traveler` object should have a `traveler_id` which is not necessarily an account id. Example: *   Travelers * ------------ *  A - GUID1 *  B - GUID2 *  C - GUID3 * *   Products * ------------ * Air *   [GUID1, GUID2, GUID3] * Hotel *   [GUID1] * Car *   [GUID3] * Rail *   [GUID2] * Above example shows all three travelers will be associated with the Air product, * however, only Traveler A will be associated with the Hotel product, * and only Traveler C will be associated with the Car product. * Traveler B will be associated with the Rail product.
+        travelers_references(List[constr(max_length=50)]): List of travelerGuids who are part of the traveling party on the order for the product. Information for each product and its required travelers should be provided in the API request. If the product booking does not require accompanying quest information then that does not need to be provided in the API request. Example: * For Air products, all travelers' details are required to complete the booking. * For Hotel products, typically the details on the person checking-in is required. * For Car products, typically only the primary driver information is required. If multiple traveler details are in the itinerary, this structure allows to fill up traveler details once in the `travelers` section, and then associate individual products to the respective travelers. This association is made using `traveler_id` field. A GUID can be generated for each object in the `travelers` section. The same GUID can be provided in the `traveler_references` below. The `travelers` array should have at least one `traveler` object, and each `traveler` object should have a `traveler_id` which is not necessarily an account id. Example: *   Travelers * ------------ *  A - GUID1 *  B - GUID2 *  C - GUID3 * *   Products * ------------ * Air *   [GUID1, GUID2, GUID3] * Hotel *   [GUID1] * Car *   [GUID3] * Rail *   [GUID2] * Activities *   [GUID1] * The example above demonstrates the association of travelers with various products. * All three travelers (A, B, and C) are associated with the Air product. * Traveler A is associated with the Hotel and Activities products. * Traveler C is associated with the Car product. * Traveler B is associated with the Rail product.
 
     """
     price: Amount = None
     type: TravelProductType = None
     inventory_type: constr(max_length=30) = None
     """
     Type of inventory.
@@ -1329,14 +1546,15 @@
     * ------------------------------------------------------
     *  `Cruise`                       : `CRUISE`
     *  `Air`                          : `AIR`
     *  `Car`                          : `CAR`
     *  `Insurance`                    : `INSURANCE`
     *  `Hotel`                        : `HOTEL`
     *  `Rail`                         :  `RAIL`
+    *  `Activities`                   :  `ACTIVITIES`
 
     """
     inventory_source: InventorySource = None
     """
     Identifies the business model through which the supply is being sold. Merchant/Agency.
     * `MERCHANT` is used when Partner is the merchant of record for this order.
     * `AGENCY` is used when this order is through an agency booking.
@@ -1367,18 +1585,21 @@
     *   [GUID1, GUID2, GUID3]
     * Hotel
     *   [GUID1]
     * Car
     *   [GUID3]
     * Rail
     *   [GUID2]
-    * Above example shows all three travelers will be associated with the Air product,
-    * however, only Traveler A will be associated with the Hotel product,
-    * and only Traveler C will be associated with the Car product.
-    * Traveler B will be associated with the Rail product.
+    * Activities
+    *   [GUID1]
+    * The example above demonstrates the association of travelers with various products.
+    * All three travelers (A, B, and C) are associated with the Air product.
+    * Traveler A is associated with the Hotel and Activities products.
+    * Traveler C is associated with the Car product.
+    * Traveler B is associated with the Rail product.
 
     """
 
 
 class RailSegments(
     BaseModel,
     smart_union=True,
@@ -1418,14 +1639,53 @@
     """
     operating_company: Optional[OperatingCompany] = None
     """
     This attribute captures the name or identifier of the company responsible for operating the Rail product. It represents the specific operating entity, such as Amtrak, British Railways, or a bus company.
     """
 
 
+class Activities(
+    TravelProductGeneric,
+    smart_union=True,
+    extra=Extra.forbid,
+):
+    r"""pydantic model Activities
+    Attributes:
+        activity(Activity): --
+        operating_company(OperatingCompanyModel): --
+        is_coupon_required(Optional[bool], optional): A coupon is typically a document or electronic code that confirms your reservation or purchase for the activity. It serves as proof of payment and allows you to participate in the activity. This field indicates whether a coupon is necessary for this activity. | For example, let's consider two scenarios: | Activity: Adventure Park | is_coupon_required: false | In this case, the attribute is set to 'false,' indicating that no coupon is necessary. However, you might still need to purchase a ticket to gain entry to the adventure park. The ticket serves as proof of payment and grants you access to the park's activities and attractions. | Activity: Spa Package | is_coupon_required: true | Here, the attribute is set to 'true,' indicating that a coupon is required. To participate in the spa package, you would need to present the designated coupon at the spa. The coupon confirms your reservation, serves as proof of payment, and may entitle you to specific spa treatments or discounts.
+        location_coordinates(Optional[Coordinates], optional): --
+        start_time(datetime): The field represents the start time of a activity, using the ISO-8061 date and time format yyyy-MM-ddTHH:mm:ss.SSSZ.
+        end_time(datetime): The field represents the end time of a activity, using the ISO-8061 date and time format yyyy-MM-ddTHH:mm:ss.SSSZ.
+        ticket(List[Ticket]): This field provides information about the tickets available for the activity.
+        type(Literal['ACTIVITIES']): --
+
+    """
+    activity: Activity = None
+    operating_company: OperatingCompanyModel = None
+    is_coupon_required: Optional[bool] = None
+    """
+    A coupon is typically a document or electronic code that confirms your reservation or purchase for the activity. It serves as proof of payment and allows you to participate in the activity. This field indicates whether a coupon is necessary for this activity. | For example, let's consider two scenarios: | Activity: Adventure Park | is_coupon_required: false | In this case, the attribute is set to 'false,' indicating that no coupon is necessary. However, you might still need to purchase a ticket to gain entry to the adventure park. The ticket serves as proof of payment and grants you access to the park's activities and attractions. | Activity: Spa Package | is_coupon_required: true | Here, the attribute is set to 'true,' indicating that a coupon is required. To participate in the spa package, you would need to present the designated coupon at the spa. The coupon confirms your reservation, serves as proof of payment, and may entitle you to specific spa treatments or discounts.
+    """
+    location_coordinates: Optional[Coordinates] = None
+    start_time: datetime = None
+    """
+    The field represents the start time of a activity, using the ISO-8061 date and time format yyyy-MM-ddTHH:mm:ss.SSSZ.
+    """
+    end_time: datetime = None
+    """
+    The field represents the end time of a activity, using the ISO-8061 date and time format yyyy-MM-ddTHH:mm:ss.SSSZ.
+    """
+    ticket: List[Ticket] = Field(..., maxItems=40, minItems=1)
+    """
+    This field provides information about the tickets available for the activity.
+    """
+    type: Literal['ACTIVITIES'] = 'ACTIVITIES'
+
+
 class Air(
     TravelProductGeneric,
     smart_union=True,
     extra=Extra.forbid,
 ):
     r"""pydantic model Air
     Attributes:
@@ -1938,17 +2198,20 @@
     smart_union=True,
     extra=Extra.forbid,
 ):
     r"""pydantic model Payment: The `method` field value is used as a discriminator, with the following mapping:
     * `CREDIT_CARD`: `CreditCard`
     * `PAYPAL`: `PayPal`
     * `POINTS`: `Points`
+    * `GIFT_CARD`: `GiftCard`
+    * `INTERNET_BANK_PAYMENT`: `InternetBankPayment`
+    * `DIRECT_DEBIT`: `DirectDebit`
 
     Attributes:
-        brand(Brand): The `brand` field value is the payment brand used for payment on this transaction. For credit card payment method ensure attributes mentioned in dictionary below are set to corresponding values only. Ensure to comply with the naming standards provided in below dictionary. For example, some Payment processors use “Japan Credit Bureau” but “JCB” should be used when calling Fraud API. Incorrect `brand` - `card_type` combination will result in data quality issues and result in degraded risk recommendation. 'brand' is an enum value with the following mapping with CreditCard 'card_type' attribute: *       brand                 :      card_type * ------------------------------------------------------- * `AMERICAN_EXPRESS`          : `AMERICAN_EXPRESS` * `DINERS_CLUB_INTERNATIONAL` : `DINERS_CLUB` * `BC_CARD`                   : `DINERS_CLUB` * `DISCOVER`                  : `DISCOVER` * `BC_CARD`                   : `DISCOVER` * `DINERS_CLUB_INTERNATIONAL` : `DISCOVER` * `JCB`                       : `DISCOVER` * `JCB`                       : `JCB` * `MASTER_CARD`               : `MASTER_CARD` * `MAESTRO`                   : `MASTER_CARD` * `POSTEPAY_MASTERCARD`       : `MASTER_CARD` * `SOLO`                      : `SOLO` * `SWITCH`                    : `SWITCH` * `MAESTRO`                   : `MAESTRO` * `CHINA_UNION_PAY`           : `CHINA_UNION_PAY` * `VISA`                      : `VISA` * `VISA_DELTA`                : `VISA` * `VISA_ELECTRON`             : `VISA` * `CARTA_SI`                  : `VISA` * `CARTE_BLEUE`               : `VISA` * `VISA_DANKORT`              : `VISA` * `POSTEPAY_VISA_ELECTRON`    : `VISA` * `PAYPAL`                    :
+        brand(Brand): The `brand` field value is the payment brand used for payment on this transaction. For credit card payment method ensure attributes mentioned in dictionary below are set to corresponding values only. Ensure to comply with the naming standards provided in below dictionary. For example, some Payment processors use “Japan Credit Bureau” but “JCB” should be used when calling Fraud API. Incorrect `brand` - `card_type` combination will result in data quality issues and result in degraded risk recommendation. 'brand' is an enum value with the following mapping with CreditCard 'card_type' attribute: *       brand                 :      card_type * ------------------------------------------------------- * `AMERICAN_EXPRESS`          : `AMERICAN_EXPRESS` * `DINERS_CLUB_INTERNATIONAL` : `DINERS_CLUB` * `BC_CARD`                   : `DINERS_CLUB` * `DISCOVER`                  : `DISCOVER` * `BC_CARD`                   : `DISCOVER` * `DINERS_CLUB_INTERNATIONAL` : `DISCOVER` * `JCB`                       : `DISCOVER` * `JCB`                       : `JCB` * `MASTER_CARD`               : `MASTER_CARD` * `MAESTRO`                   : `MASTER_CARD` * `POSTEPAY_MASTERCARD`       : `MASTER_CARD` * `SOLO`                      : `SOLO` * `SWITCH`                    : `SWITCH` * `MAESTRO`                   : `MAESTRO` * `CHINA_UNION_PAY`           : `CHINA_UNION_PAY` * `VISA`                      : `VISA` * `VISA_DELTA`                : `VISA` * `VISA_ELECTRON`             : `VISA` * `CARTA_SI`                  : `VISA` * `CARTE_BLEUE`               : `VISA` * `VISA_DANKORT`              : `VISA` * `POSTEPAY_VISA_ELECTRON`    : `VISA` * `PAYPAL`                    :  'brand' with 'Points' payment_type is an enum value with following: * `EXPEDIA_REWARDS` * `AMEX_POINTS` * `BANK_OF_AMERICA_REWARDS` * `DISCOVER_POINTS` * `MASTER_CARD_POINTS` * `CITI_THANK_YOU_POINTS` * `MERRILL_LYNCH_REWARDS` * `WELLS_FARGO_POINTS` * `DELTA_SKY_MILES` * `UNITED_POINTS` * `DISCOVER_MILES` * `ALASKA_MILES` * `RBC_REWARDS` * `BILT_REWARDS` * `ORBUCKS` * `CHEAP_CASH` * `BONUS_PLUS` * `ULTIMATE_REWARDS`  'brand' with 'GiftCard' payment_type is an enum value with following: * `GIFT_CARD`  'brand' with 'InternetBankPayment' payment_type is an enum value with following: * `IBP` * `LOCAL_DEBIT_CARD` * `SOFORT` * `YANDEX` * `WEB_MONEY` * `QIWI` * `BITCOIN`  'brand' with 'DirectDebit' payment_type is an enum value with following: * `EVL` * `INTER_COMPANY`
         method(PaymentMethod): --
         reason(Optional[PaymentReason], optional): --
         billing_name(Name): --
         billing_address(Address): --
         billing_email_address(EmailStr): Email address associated with the payment.
         authorized_amount(Optional[Amount], optional): --
         verified_amount(Optional[Amount], optional): --
@@ -1985,14 +2248,50 @@
     * `VISA_ELECTRON`             : `VISA`
     * `CARTA_SI`                  : `VISA`
     * `CARTE_BLEUE`               : `VISA`
     * `VISA_DANKORT`              : `VISA`
     * `POSTEPAY_VISA_ELECTRON`    : `VISA`
     * `PAYPAL`                    :
 
+    'brand' with 'Points' payment_type is an enum value with following:
+    * `EXPEDIA_REWARDS`
+    * `AMEX_POINTS`
+    * `BANK_OF_AMERICA_REWARDS`
+    * `DISCOVER_POINTS`
+    * `MASTER_CARD_POINTS`
+    * `CITI_THANK_YOU_POINTS`
+    * `MERRILL_LYNCH_REWARDS`
+    * `WELLS_FARGO_POINTS`
+    * `DELTA_SKY_MILES`
+    * `UNITED_POINTS`
+    * `DISCOVER_MILES`
+    * `ALASKA_MILES`
+    * `RBC_REWARDS`
+    * `BILT_REWARDS`
+    * `ORBUCKS`
+    * `CHEAP_CASH`
+    * `BONUS_PLUS`
+    * `ULTIMATE_REWARDS`
+
+    'brand' with 'GiftCard' payment_type is an enum value with following:
+    * `GIFT_CARD`
+
+    'brand' with 'InternetBankPayment' payment_type is an enum value with following:
+    * `IBP`
+    * `LOCAL_DEBIT_CARD`
+    * `SOFORT`
+    * `YANDEX`
+    * `WEB_MONEY`
+    * `QIWI`
+    * `BITCOIN`
+
+    'brand' with 'DirectDebit' payment_type is an enum value with following:
+    * `EVL`
+    * `INTER_COMPANY`
+
     """
     method: PaymentMethod = None
     reason: Optional[PaymentReason] = None
     billing_name: Name = None
     billing_address: Address = None
     billing_email_address: EmailStr = None
     """
@@ -2009,21 +2308,21 @@
     smart_union=True,
     extra=Extra.forbid,
 ):
     r"""pydantic model CreditCard
     Attributes:
         card_type(CardType): The 'card_type' field value is an enum value which is associated with the payment method of the specific payment instrument. For credit card payment method ensure attributes mentioned in dictionary below are set to corresponding values only. Ensure to comply with the naming standards provided in below dictionary. For example, some Payment processors use “Japan Credit Bureau” but “JCB” should be used when calling Fraud API. Incorrect `card_type` - `brand` combination will result in data quality issues and result in degraded risk recommendation. 'card_type' is an enum value with the following mapping with Payment `brand` attribute: *       card_type            :          brand * -------------------------------------------------------- * `AMERICAN_EXPRESS`         : `AMERICAN_EXPRESS` * `DINERS_CLUB`              : `DINERS_CLUB_INTERNATIONAL` * `DINERS_CLUB`              : `BC_CARD` * `DISCOVER`                 : `DISCOVER` * `DISCOVER`                 : `BC_CARD` * `DISCOVER`                 : `DINERS_CLUB_INTERNATIONAL` * `DISCOVER`                 : `JCB` * `JCB`                      : `JCB` * `MASTER_CARD`              : `MASTER_CARD` * `MASTER_CARD`              : `MAESTRO` * `MASTER_CARD`              : `POSTEPAY_MASTERCARD` * `SOLO`                     : `SOLO` * `SWITCH`                   : `SWITCH` * `MAESTRO`                  : `MAESTRO` * `CHINA_UNION_PAY`          : `CHINA_UNION_PAY` * `VISA`                     : `VISA` * `VISA`                     : `VISA_DELTA` * `VISA`                     : `VISA_ELECTRON` * `VISA`                     : `CARTA_SI` * `VISA`                     : `CARTE_BLEUE` * `VISA`                     : `VISA_DANKORT` * `VISA`                     : `POSTEPAY_VISA_ELECTRON`
         card_number(constr(max_length=200)): All the digits (unencrypted) of the credit card number associated with the payment.
-        expiry_date(Optional[datetime], optional): Expiration date of the credit card used for payment, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
+        expiry_date(datetime): Expiration date of the credit card used for payment, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
         electronic_commerce_indicator(Optional[constr(max_length=200)], optional): Electronic Commerce Indicator, a two or three digit number usually returned by a 3rd party payment processor in regards to the authentication used when gathering the cardholder's payment credentials.
         virtual_credit_card_flag(Optional[bool], optional): A flag to indicate that the bank card being used for the charge is a virtual credit card.
         wallet_type(Optional[constr(max_length=200)], optional): If a virtual/digital form of payment was used, the type of digital wallet should be specified here. Possible `wallet_type`'s include: `Google` or `ApplePay`.
         card_avs_response(Optional[constr(max_length=50)], optional): A field used to confirm if the address provided at the time of purchase matches what the bank has on file for the Credit Card.
         card_cvv_response(Optional[constr(max_length=20)], optional): A field used to confirm the Card Verification Value on the Credit Card matches the Credit Card used at the time of purchase.
-        telephones(Optional[List[Telephone]], optional): Telephone(s) associated with card holder and credit card.
+        telephones(List[Telephone]): Telephone(s) associated with card holder and credit card.
         merchant_order_code(Optional[constr(max_length=200)], optional): Reference code passed to acquiring bank at the time of payment. This code is the key ID that ties back to payments data at the payment level.
         card_authentication_failure_count(Optional[int], optional): Total authentication failure count for given card.
         method(Literal['CREDIT_CARD']): --
 
     """
     card_type: CardType = None
     """
@@ -2058,15 +2357,15 @@
     * `VISA`                     : `POSTEPAY_VISA_ELECTRON`
 
     """
     card_number: constr(max_length=200) = None
     """
     All the digits (unencrypted) of the credit card number associated with the payment.
     """
-    expiry_date: Optional[datetime] = None
+    expiry_date: datetime = None
     """
     Expiration date of the credit card used for payment, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
     """
     electronic_commerce_indicator: Optional[constr(max_length=200)] = None
     """
     Electronic Commerce Indicator, a two or three digit number usually returned by a 3rd party payment processor in regards to the authentication used when gathering the cardholder's payment credentials.
     """
@@ -2082,15 +2381,15 @@
     """
     A field used to confirm if the address provided at the time of purchase matches what the bank has on file for the Credit Card.
     """
     card_cvv_response: Optional[constr(max_length=20)] = None
     """
     A field used to confirm the Card Verification Value on the Credit Card matches the Credit Card used at the time of purchase.
     """
-    telephones: Optional[List[Telephone]] = Field(None, maxItems=20, minItems=1)
+    telephones: List[Telephone] = Field(..., maxItems=20, minItems=1)
     """
     Telephone(s) associated with card holder and credit card.
     """
     merchant_order_code: Optional[constr(max_length=200)] = None
     """
     Reference code passed to acquiring bank at the time of payment. This code is the key ID that ties back to payments data at the payment level.
     """
@@ -2132,20 +2431,109 @@
 class Points(
     PaymentGeneric,
     smart_union=True,
     extra=Extra.forbid,
 ):
     r"""pydantic model Points
     Attributes:
+        account_id(constr(max_length=200)): Points account id.
         method(Literal['POINTS']): --
 
     """
+    account_id: constr(max_length=200) = None
+    """
+    Points account id.
+    """
     method: Literal['POINTS'] = 'POINTS'
 
 
+class GiftCard(
+    PaymentGeneric,
+    smart_union=True,
+    extra=Extra.forbid,
+):
+    r"""pydantic model GiftCard
+    Attributes:
+        card_number(constr(regex=r'^[0-9A-Za-z]{4,16}$', max_length=16)): Gift card number.
+        card_holder_name(constr(max_length=200)): The name of gift card holder.
+        pin(constr(regex=r'^[0-9]{4,8}$', max_length=8)): The PIN of gift card.
+        method(Literal['GIFT_CARD']): --
+
+    """
+    card_number: constr(regex=r'^[0-9A-Za-z]{4,16}$', max_length=16) = Field(..., example='123456ABCDabcd')
+    """
+    Gift card number.
+    """
+    card_holder_name: constr(max_length=200) = None
+    """
+    The name of gift card holder.
+    """
+    pin: constr(regex=r'^[0-9]{4,8}$', max_length=8) = Field(..., example='123456')
+    """
+    The PIN of gift card.
+    """
+    method: Literal['GIFT_CARD'] = 'GIFT_CARD'
+
+
+class InternetBankPayment(
+    PaymentGeneric,
+    smart_union=True,
+    extra=Extra.forbid,
+):
+    r"""pydantic model InternetBankPayment
+    Attributes:
+        bank_id(constr(max_length=15)): The bank_id provided by the internet bank payment(IBP) provider (DRWP aka NetGiro) for the bank used for processing the payment.
+        bank_branch_code(constr(max_length=15)): A code that identifies the bank branch for internet bank payment(IBP).
+        telephones(List[Telephone]): Telephone(s) associated with internet bank payment(IBP) provider.
+        method(Literal['INTERNET_BANK_PAYMENT']): --
+
+    """
+    bank_id: constr(max_length=15) = None
+    """
+    The bank_id provided by the internet bank payment(IBP) provider (DRWP aka NetGiro) for the bank used for processing the payment.
+    """
+    bank_branch_code: constr(max_length=15) = None
+    """
+    A code that identifies the bank branch for internet bank payment(IBP).
+    """
+    telephones: List[Telephone] = Field(..., maxItems=20, minItems=1)
+    """
+    Telephone(s) associated with internet bank payment(IBP) provider.
+    """
+    method: Literal['INTERNET_BANK_PAYMENT'] = 'INTERNET_BANK_PAYMENT'
+
+
+class DirectDebit(
+    PaymentGeneric,
+    smart_union=True,
+    extra=Extra.forbid,
+):
+    r"""pydantic model DirectDebit
+    Attributes:
+        routing_number(constr(max_length=15)): A code that identifies the financial institution for a specific bank account.
+        account_number(constr(max_length=100)): Cleartext (unencrypted) DirectDebit bank account number associated with the payment instrument.
+        telephones(List[Telephone]): Telephone(s) associated with direct debit payment provider.
+        method(Literal['DIRECT_DEBIT']): --
+
+    """
+    routing_number: constr(max_length=15) = Field(..., example='100000000')
+    """
+    A code that identifies the financial institution for a specific bank account.
+    """
+    account_number: constr(max_length=100) = None
+    """
+    Cleartext (unencrypted) DirectDebit bank account number associated with the payment instrument.
+    """
+    telephones: List[Telephone] = Field(..., maxItems=20, minItems=1)
+    """
+    Telephone(s) associated with direct debit payment provider.
+    """
+    method: Literal['DIRECT_DEBIT'] = 'DIRECT_DEBIT'
+
+
 class TransactionDetails(
     BaseModel,
     smart_union=True,
     extra=Extra.forbid,
 ):
     r"""pydantic model TransactionDetails
     Attributes:
@@ -2220,17 +2608,17 @@
     transaction: Optional[OrderPurchaseTransaction] = None
 
 
 RefundUpdate = Union[IssuedRefundUpdate, SettledRefundUpdate, RefundUpdateGeneric]
 
 OrderPurchaseUpdateRequest = Union[OrderUpdate, ChargebackFeedback, InsultFeedback, RefundUpdate, PaymentUpdate, OrderPurchaseUpdateRequestGeneric]
 
-TravelProduct = Union[Rail, Air, Cruise, Car, Hotel, Insurance, TravelProductGeneric]
+TravelProduct = Union[Rail, Activities, Air, Cruise, Car, Hotel, Insurance, TravelProductGeneric]
 
-Payment = Union[CreditCard, PayPal, Points, PaymentGeneric]
+Payment = Union[CreditCard, PayPal, Points, GiftCard, InternetBankPayment, DirectDebit, PaymentGeneric]
 
 
 Error.update_forward_refs()
 
 
 UnauthorizedError.update_forward_refs()
 
@@ -2288,14 +2676,26 @@
 
 OperatingCompany.update_forward_refs()
 
 
 RailwayStationDetails.update_forward_refs()
 
 
+Activity.update_forward_refs()
+
+
+Coordinates.update_forward_refs()
+
+
+OperatingCompanyModel.update_forward_refs()
+
+
+Ticket.update_forward_refs()
+
+
 AirSegment.update_forward_refs()
 
 
 HotelAddress.update_forward_refs()
 
 
 PaymentThreeDSCriteria.update_forward_refs()
@@ -2330,14 +2730,17 @@
 
 OrderPurchaseScreenResponse.update_forward_refs()
 
 
 RailSegments.update_forward_refs()
 
 
+Activities.update_forward_refs()
+
+
 Air.update_forward_refs()
 
 
 Cruise.update_forward_refs()
 
 
 Car.update_forward_refs()
@@ -2399,14 +2802,23 @@
 
 PayPal.update_forward_refs()
 
 
 Points.update_forward_refs()
 
 
+GiftCard.update_forward_refs()
+
+
+InternetBankPayment.update_forward_refs()
+
+
+DirectDebit.update_forward_refs()
+
+
 TransactionDetails.update_forward_refs()
 
 
 OrderPurchaseTransaction.update_forward_refs()
 
 
 OrderPurchaseScreenRequest.update_forward_refs()
```

### Comparing `openworld-sdk-python-fraudpreventionv2-1.2.1/openworld_sdk_python_fraudpreventionv2.egg-info/PKG-INFO` & `openworld-sdk-python-fraudpreventionv2-1.3.0/openworld_sdk_python_fraudpreventionv2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openworld-sdk-python-fraudpreventionv2
-Version: 1.2.1
+Version: 1.3.0
 Summary: Open World F r a u d P r e v e n t i o n V 2 SDK for Python
 Home-page: https://github.com/ExpediaGroup/openworld-sdk-python
 Author: Expedia Group
 Author-email: oss@expediagroup.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
```

### Comparing `openworld-sdk-python-fraudpreventionv2-1.2.1/setup.py` & `openworld-sdk-python-fraudpreventionv2-1.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 
 from setuptools import setup
 
 setup(
     name='openworld-sdk-python-fraudpreventionv2',
-    version='1.2.1',
+    version='1.3.0',
     packages=['openworld.sdk.fraudpreventionv2'],
     package_dir={'openworld-sdk-python-fraudpreventionv2': '.'},
     license='Apache License, Version 2.0',
     author='Expedia Group',
     author_email='oss@expediagroup.com',
     url='https://github.com/ExpediaGroup/openworld-sdk-python',
     classifiers=[
```

