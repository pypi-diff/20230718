# Comparing `tmp/hyperliquid_python_sdk-0.1.8.tar.gz` & `tmp/hyperliquid_python_sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperliquid_python_sdk-0.1.8.tar", max compression
+gzip compressed data, was "hyperliquid_python_sdk-0.1.9.tar", max compression
```

## Comparing `hyperliquid_python_sdk-0.1.8.tar` & `hyperliquid_python_sdk-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1083 2023-05-16 01:06:14.480083 hyperliquid_python_sdk-0.1.8/LICENSE.md
--rw-r--r--   0        0        0     5741 2023-05-16 01:06:14.495874 hyperliquid_python_sdk-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-05-16 01:06:14.471293 hyperliquid_python_sdk-0.1.8/hyperliquid/__init__.py
--rw-r--r--   0        0        0     1677 2023-05-16 01:06:14.479107 hyperliquid_python_sdk-0.1.8/hyperliquid/api.py
--rw-r--r--   0        0        0     4557 2023-05-16 01:06:14.471030 hyperliquid_python_sdk-0.1.8/hyperliquid/exchange.py
--rw-r--r--   0        0        0     4938 2023-05-16 01:06:14.479409 hyperliquid_python_sdk-0.1.8/hyperliquid/info.py
--rw-r--r--   0        0        0        0 2023-05-16 01:06:14.473421 hyperliquid_python_sdk-0.1.8/hyperliquid/utils/__init__.py
--rw-r--r--   0        0        0      144 2023-05-16 01:06:14.473252 hyperliquid_python_sdk-0.1.8/hyperliquid/utils/constants.py
--rw-r--r--   0        0        0      479 2023-05-16 01:06:14.472868 hyperliquid_python_sdk-0.1.8/hyperliquid/utils/error.py
--rw-r--r--   0        0        0     5070 2023-05-16 01:06:14.472421 hyperliquid_python_sdk-0.1.8/hyperliquid/utils/signing.py
--rw-r--r--   0        0        0     2174 2023-05-16 01:06:14.473857 hyperliquid_python_sdk-0.1.8/hyperliquid/utils/types.py
--rw-r--r--   0        0        0     4691 2023-05-16 01:06:14.479757 hyperliquid_python_sdk-0.1.8/hyperliquid/websocket_manager.py
--rw-r--r--   0        0        0     3859 2023-05-16 01:06:14.490743 hyperliquid_python_sdk-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     7371 1970-01-01 00:00:00.000000 hyperliquid_python_sdk-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-03-30 16:09:48.731040 hyperliquid_python_sdk-0.1.9/LICENSE.md
+-rw-r--r--   0        0        0     5741 2023-05-18 16:58:16.662593 hyperliquid_python_sdk-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-03-20 20:28:58.636849 hyperliquid_python_sdk-0.1.9/hyperliquid/__init__.py
+-rw-r--r--   0        0        0     1677 2023-03-30 17:02:32.596191 hyperliquid_python_sdk-0.1.9/hyperliquid/api.py
+-rw-r--r--   0        0        0     4557 2023-05-18 16:58:16.664933 hyperliquid_python_sdk-0.1.9/hyperliquid/exchange.py
+-rw-r--r--   0        0        0     7585 2023-06-20 20:52:06.327149 hyperliquid_python_sdk-0.1.9/hyperliquid/info.py
+-rw-r--r--   0        0        0        0 2023-03-20 20:28:58.637272 hyperliquid_python_sdk-0.1.9/hyperliquid/utils/__init__.py
+-rw-r--r--   0        0        0      144 2023-03-24 21:41:42.619628 hyperliquid_python_sdk-0.1.9/hyperliquid/utils/constants.py
+-rw-r--r--   0        0        0      479 2023-03-20 20:28:58.637442 hyperliquid_python_sdk-0.1.9/hyperliquid/utils/error.py
+-rw-r--r--   0        0        0     5823 2023-06-20 22:09:11.651106 hyperliquid_python_sdk-0.1.9/hyperliquid/utils/signing.py
+-rw-r--r--   0        0        0     2174 2023-05-18 16:58:16.665553 hyperliquid_python_sdk-0.1.9/hyperliquid/utils/types.py
+-rw-r--r--   0        0        0     4691 2023-05-18 16:58:16.665738 hyperliquid_python_sdk-0.1.9/hyperliquid/websocket_manager.py
+-rw-r--r--   0        0        0     3859 2023-06-20 22:13:25.379550 hyperliquid_python_sdk-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     7371 1970-01-01 00:00:00.000000 hyperliquid_python_sdk-0.1.9/PKG-INFO
```

### Comparing `hyperliquid_python_sdk-0.1.8/LICENSE.md` & `hyperliquid_python_sdk-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hyperliquid_python_sdk-0.1.8/README.md` & `hyperliquid_python_sdk-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `hyperliquid_python_sdk-0.1.8/hyperliquid/api.py` & `hyperliquid_python_sdk-0.1.9/hyperliquid/api.py`

 * *Files identical despite different names*

### Comparing `hyperliquid_python_sdk-0.1.8/hyperliquid/exchange.py` & `hyperliquid_python_sdk-0.1.9/hyperliquid/exchange.py`

 * *Files identical despite different names*

### Comparing `hyperliquid_python_sdk-0.1.8/hyperliquid/info.py` & `hyperliquid_python_sdk-0.1.9/hyperliquid/info.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from hyperliquid.api import API
-from hyperliquid.utils.types import Any, Callable, Meta, Subscription, cast
+from hyperliquid.utils.types import Any, Callable, Meta, Optional, Subscription, cast
 from hyperliquid.websocket_manager import WebsocketManager
 
 
 class Info(API):
     def __init__(self, base_url=None, skip_ws=False):
         super().__init__(base_url)
         if not skip_ws:
@@ -133,14 +133,99 @@
                     },
                     ...
                 ]
             }
         """
         return cast(Meta, self.post("/info", {"type": "meta"}))
 
+    def funding_history(self, coin: str, startTime: int, endTime: Optional[int] = None) -> Any:
+        """Retrieve funding history for a given coin
+
+        POST /info
+
+        Args:
+            coin (str): Coin to retrieve funding history for.
+            startTime (int): Unix timestamp in milliseconds.
+            endTime (int): Unix timestamp in milliseconds.
+
+        Returns:
+            [
+                {
+                    coin: str,
+                    fundingRate: float string,
+                    premium: float string,
+                    time: int
+                },
+                ...
+            ]
+        """
+        if endTime is not None:
+            return self.post(
+                "/info", {"type": "fundingHistory", "coin": coin, "startTime": startTime, "endTime": endTime}
+            )
+        return self.post("/info", {"type": "fundingHistory", "coin": coin, "startTime": startTime})
+
+    def l2_snapshot(self, coin: str) -> Any:
+        """Retrieve L2 snapshot for a given coin
+
+        POST /info
+
+        Args:
+            coin (str): Coin to retrieve L2 snapshot for.
+
+        Returns:
+            {
+                coin: str,
+                levels: [
+                    [
+                        {
+                            n: int,
+                            px: float string,
+                            sz: float string
+                        },
+                        ...
+                    ],
+                    ...
+                ],
+                time: int
+            }
+        """
+        return self.post("/info", {"type": "l2Book", "coin": coin})
+
+    def candles_snapshot(self, coin: str, interval: str, startTime: int, endTime: int) -> Any:
+        """Retrieve candles snapshot for a given coin
+
+        POST /info
+
+        Args:
+            coin (str): Coin to retrieve candles snapshot for.
+            interval (str): Candlestick interval.
+            startTime (int): Unix timestamp in milliseconds.
+            endTime (int): Unix timestamp in milliseconds.
+
+        Returns:
+            [
+                {
+                    T: int,
+                    c: float string,
+                    h: float string,
+                    i: str,
+                    l: float string,
+                    n: int,
+                    o: float string,
+                    s: string,
+                    t: int,
+                    v: float string
+                },
+                ...
+            ]
+        """
+        req = {"coin": coin, "interval": interval, "startTime": startTime, "endTime": endTime}
+        return self.post("/info", {"type": "candleSnapshot", "req": req})
+
     def subscribe(self, subscription: Subscription, callback: Callable[[Any], None]) -> int:
         if self.ws_manager is None:
             raise RuntimeError("Cannot call subscribe since skip_ws was used")
         else:
             return self.ws_manager.subscribe(subscription, callback)
 
     def unsubscribe(self, subscription: Subscription, subscription_id: int) -> bool:
```

### Comparing `hyperliquid_python_sdk-0.1.8/hyperliquid/utils/signing.py` & `hyperliquid_python_sdk-0.1.9/hyperliquid/utils/signing.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,19 +7,21 @@
 from hyperliquid.utils.types import Any, Literal, Tuple, TypedDict, Union
 
 ZERO_ADDRESS = "0x0000000000000000000000000000000000000000"
 
 Tif = Union[Literal["Alo"], Literal["Ioc"], Literal["Gtc"]]
 Tpsl = Union[Literal["tp"], Literal["sl"]]
 LimitOrderType = TypedDict("LimitOrderType", {"tif": Tif})
-TriggerOrderType = TypedDict("TriggerOrderType", {"triggerPx": int, "isMarket": bool, "tpsl": Tpsl})
+TriggerOrderType = TypedDict("TriggerOrderType", {"triggerPx": float, "isMarket": bool, "tpsl": Tpsl})
+TriggerOrderTypeWire = TypedDict("TriggerOrderTypeWire", {"triggerPx": str, "isMarket": bool, "tpsl": Tpsl})
 OrderType = TypedDict("OrderType", {"limit": LimitOrderType, "trigger": TriggerOrderType}, total=False)
+OrderTypeWire = TypedDict("OrderTypeWire", {"limit": LimitOrderType, "trigger": TriggerOrderTypeWire}, total=False)
 
 
-def order_type_to_tuple(order_type: OrderType) -> Tuple[int, int]:
+def order_type_to_tuple(order_type: OrderType) -> Tuple[int, float]:
     if "limit" in order_type:
         tif = order_type["limit"]["tif"]
         if tif == "Gtc":
             return 2, 0
         elif tif == "Alo":
             return 1, 0
         elif tif == "Ioc":
@@ -65,27 +67,42 @@
         order["reduceOnly"],
         order_type_array[0],
         float_to_int_for_hashing(order_type_array[1]),
     )
 
 
 OrderWire = TypedDict(
-    "OrderWire", {"asset": int, "isBuy": bool, "limitPx": str, "sz": str, "reduceOnly": bool, "orderType": OrderType}
+    "OrderWire",
+    {"asset": int, "isBuy": bool, "limitPx": str, "sz": str, "reduceOnly": bool, "orderType": OrderTypeWire},
 )
 
 
+def order_type_to_wire(order_type: OrderType) -> OrderTypeWire:
+    if "limit" in order_type:
+        return {"limit": order_type["limit"]}
+    elif "trigger" in order_type:
+        return {
+            "trigger": {
+                "triggerPx": float_to_wire(order_type["trigger"]["triggerPx"]),
+                "tpsl": order_type["trigger"]["tpsl"],
+                "isMarket": order_type["trigger"]["isMarket"],
+            }
+        }
+    raise ValueError("Invalid order type", order_type)
+
+
 def order_spec_to_order_wire(order_spec: OrderSpec) -> OrderWire:
     order = order_spec["order"]
     return {
         "asset": order["asset"],
         "isBuy": order["isBuy"],
         "limitPx": float_to_wire(order["limitPx"]),
         "sz": float_to_wire(order["sz"]),
         "reduceOnly": order["reduceOnly"],
-        "orderType": order_spec["orderType"],
+        "orderType": order_type_to_wire(order_spec["orderType"]),
     }
 
 
 def construct_phantom_agent(signature_types, signature_data):
     connection_id = encode(signature_types, signature_data)
 
     return {"source": "a", "connectionId": keccak(connection_id)}
```

### Comparing `hyperliquid_python_sdk-0.1.8/hyperliquid/utils/types.py` & `hyperliquid_python_sdk-0.1.9/hyperliquid/utils/types.py`

 * *Files identical despite different names*

### Comparing `hyperliquid_python_sdk-0.1.8/hyperliquid/websocket_manager.py` & `hyperliquid_python_sdk-0.1.9/hyperliquid/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `hyperliquid_python_sdk-0.1.8/pyproject.toml` & `hyperliquid_python_sdk-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hyperliquid-python-sdk"
-version = "0.1.8"
+version = "0.1.9"
 description = "SDK for Hyperliquid API trading with Python."
 readme = "README.md"
 authors = ["Hyperliquid <hello@hyperliquid.xyz>"]
 license = "MIT"
 repository = "https://github.com/hyperliquid-dex/hyperliquid-python-sdk"
 homepage = "https://github.com/hyperliquid-dex/hyperliquid-python-sdk"
 packages = [
```

### Comparing `hyperliquid_python_sdk-0.1.8/PKG-INFO` & `hyperliquid_python_sdk-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperliquid-python-sdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: SDK for Hyperliquid API trading with Python.
 Home-page: https://github.com/hyperliquid-dex/hyperliquid-python-sdk
 License: MIT
 Author: Hyperliquid
 Author-email: hello@hyperliquid.xyz
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
```

