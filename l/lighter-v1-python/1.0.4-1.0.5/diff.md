# Comparing `tmp/lighter-v1-python-1.0.4.tar.gz` & `tmp/lighter-v1-python-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lighter-v1-python-1.0.4.tar", last modified: Wed May 10 17:47:00 2023, max compression
+gzip compressed data, was "lighter-v1-python-1.0.5.tar", last modified: Tue Jul 18 12:06:30 2023, max compression
```

## Comparing `lighter-v1-python-1.0.4.tar` & `lighter-v1-python-1.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 ahmetavci   (501) staff       (20)        0 2023-05-10 17:47:00.294110 lighter-v1-python-1.0.4/
--rw-r--r--   0 ahmetavci   (501) staff       (20)    11357 2023-02-16 12:31:17.000000 lighter-v1-python-1.0.4/LICENSE
--rw-r--r--   0 ahmetavci   (501) staff       (20)     6233 2023-05-10 17:47:00.293979 lighter-v1-python-1.0.4/PKG-INFO
--rw-r--r--   0 ahmetavci   (501) staff       (20)     5419 2023-03-27 10:20:02.000000 lighter-v1-python-1.0.4/README.md
-drwxr-xr-x   0 ahmetavci   (501) staff       (20)        0 2023-05-10 17:47:00.292082 lighter-v1-python-1.0.4/lighter/
--rw-r--r--   0 ahmetavci   (501) staff       (20)        0 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.4/lighter/__init__.py
-drwxr-xr-x   0 ahmetavci   (501) staff       (20)        0 2023-05-10 17:47:00.292571 lighter-v1-python-1.0.4/lighter/abi/
--rw-r--r--   0 ahmetavci   (501) staff       (20)     4841 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.4/lighter/abi/erc20.json
--rw-r--r--   0 ahmetavci   (501) staff       (20)     5643 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.4/lighter/abi/factory.json
--rw-r--r--   0 ahmetavci   (501) staff       (20)    11602 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.4/lighter/abi/orderbook.json
--rw-r--r--   0 ahmetavci   (501) staff       (20)     9730 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.4/lighter/abi/router.json
--rw-r--r--   0 ahmetavci   (501) staff       (20)     1158 2023-05-10 17:43:58.000000 lighter-v1-python-1.0.4/lighter/constants.py
--rw-r--r--   0 ahmetavci   (501) staff       (20)      869 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.4/lighter/errors.py
-drwxr-xr-x   0 ahmetavci   (501) staff       (20)        0 2023-05-10 17:47:00.292779 lighter-v1-python-1.0.4/lighter/helpers/
--rw-r--r--   0 ahmetavci   (501) staff       (20)        0 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.4/lighter/helpers/__init__.py
--rw-r--r--   0 ahmetavci   (501) staff       (20)      413 2023-03-27 10:20:02.000000 lighter-v1-python-1.0.4/lighter/helpers/request_helpers.py
--rw-r--r--   0 ahmetavci   (501) staff       (20)     5319 2023-05-10 17:43:58.000000 lighter-v1-python-1.0.4/lighter/lighter_client.py
-drwxr-xr-x   0 ahmetavci   (501) staff       (20)        0 2023-05-10 17:47:00.293119 lighter-v1-python-1.0.4/lighter/modules/
--rw-r--r--   0 ahmetavci   (501) staff       (20)        0 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.4/lighter/modules/__init__.py
--rw-r--r--   0 ahmetavci   (501) staff       (20)     9492 2023-03-27 10:20:02.000000 lighter-v1-python-1.0.4/lighter/modules/api.py
--rw-r--r--   0 ahmetavci   (501) staff       (20)    58421 2023-05-10 17:43:58.000000 lighter-v1-python-1.0.4/lighter/modules/blockchain.py
-drwxr-xr-x   0 ahmetavci   (501) staff       (20)        0 2023-05-10 17:47:00.293822 lighter-v1-python-1.0.4/lighter_v1_python.egg-info/
--rw-r--r--   0 ahmetavci   (501) staff       (20)     6233 2023-05-10 17:47:00.000000 lighter-v1-python-1.0.4/lighter_v1_python.egg-info/PKG-INFO
--rw-r--r--   0 ahmetavci   (501) staff       (20)      558 2023-05-10 17:47:00.000000 lighter-v1-python-1.0.4/lighter_v1_python.egg-info/SOURCES.txt
--rw-r--r--   0 ahmetavci   (501) staff       (20)        1 2023-05-10 17:47:00.000000 lighter-v1-python-1.0.4/lighter_v1_python.egg-info/dependency_links.txt
--rw-r--r--   0 ahmetavci   (501) staff       (20)      194 2023-05-10 17:47:00.000000 lighter-v1-python-1.0.4/lighter_v1_python.egg-info/requires.txt
--rw-r--r--   0 ahmetavci   (501) staff       (20)        8 2023-05-10 17:47:00.000000 lighter-v1-python-1.0.4/lighter_v1_python.egg-info/top_level.txt
--rw-r--r--   0 ahmetavci   (501) staff       (20)       38 2023-05-10 17:47:00.294149 lighter-v1-python-1.0.4/setup.cfg
--rw-r--r--   0 ahmetavci   (501) staff       (20)     1426 2023-05-10 17:46:45.000000 lighter-v1-python-1.0.4/setup.py
+drwxr-xr-x   0 ahmetavci   (501) staff       (20)        0 2023-07-18 12:06:30.439323 lighter-v1-python-1.0.5/
+-rw-r--r--   0 ahmetavci   (501) staff       (20)    11357 2023-02-16 12:31:17.000000 lighter-v1-python-1.0.5/LICENSE
+-rw-r--r--   0 ahmetavci   (501) staff       (20)     6235 2023-07-18 12:06:30.439198 lighter-v1-python-1.0.5/PKG-INFO
+-rw-r--r--   0 ahmetavci   (501) staff       (20)     5421 2023-07-18 12:02:16.000000 lighter-v1-python-1.0.5/README.md
+drwxr-xr-x   0 ahmetavci   (501) staff       (20)        0 2023-07-18 12:06:30.437022 lighter-v1-python-1.0.5/lighter/
+-rw-r--r--   0 ahmetavci   (501) staff       (20)        0 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.5/lighter/__init__.py
+drwxr-xr-x   0 ahmetavci   (501) staff       (20)        0 2023-07-18 12:06:30.437725 lighter-v1-python-1.0.5/lighter/abi/
+-rw-r--r--   0 ahmetavci   (501) staff       (20)     4841 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.5/lighter/abi/erc20.json
+-rw-r--r--   0 ahmetavci   (501) staff       (20)     5643 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.5/lighter/abi/factory.json
+-rw-r--r--   0 ahmetavci   (501) staff       (20)    11602 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.5/lighter/abi/orderbook.json
+-rw-r--r--   0 ahmetavci   (501) staff       (20)     9730 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.5/lighter/abi/router.json
+-rw-r--r--   0 ahmetavci   (501) staff       (20)     1583 2023-07-18 11:57:19.000000 lighter-v1-python-1.0.5/lighter/constants.py
+-rw-r--r--   0 ahmetavci   (501) staff       (20)      869 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.5/lighter/errors.py
+drwxr-xr-x   0 ahmetavci   (501) staff       (20)        0 2023-07-18 12:06:30.438053 lighter-v1-python-1.0.5/lighter/helpers/
+-rw-r--r--   0 ahmetavci   (501) staff       (20)        0 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.5/lighter/helpers/__init__.py
+-rw-r--r--   0 ahmetavci   (501) staff       (20)      413 2023-03-27 10:20:02.000000 lighter-v1-python-1.0.5/lighter/helpers/request_helpers.py
+-rw-r--r--   0 ahmetavci   (501) staff       (20)     5211 2023-07-18 11:57:19.000000 lighter-v1-python-1.0.5/lighter/lighter_client.py
+drwxr-xr-x   0 ahmetavci   (501) staff       (20)        0 2023-07-18 12:06:30.438451 lighter-v1-python-1.0.5/lighter/modules/
+-rw-r--r--   0 ahmetavci   (501) staff       (20)        0 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.5/lighter/modules/__init__.py
+-rw-r--r--   0 ahmetavci   (501) staff       (20)     9707 2023-07-18 11:57:19.000000 lighter-v1-python-1.0.5/lighter/modules/api.py
+-rw-r--r--   0 ahmetavci   (501) staff       (20)    58371 2023-07-18 11:57:19.000000 lighter-v1-python-1.0.5/lighter/modules/blockchain.py
+drwxr-xr-x   0 ahmetavci   (501) staff       (20)        0 2023-07-18 12:06:30.439033 lighter-v1-python-1.0.5/lighter_v1_python.egg-info/
+-rw-r--r--   0 ahmetavci   (501) staff       (20)     6235 2023-07-18 12:06:30.000000 lighter-v1-python-1.0.5/lighter_v1_python.egg-info/PKG-INFO
+-rw-r--r--   0 ahmetavci   (501) staff       (20)      558 2023-07-18 12:06:30.000000 lighter-v1-python-1.0.5/lighter_v1_python.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmetavci   (501) staff       (20)        1 2023-07-18 12:06:30.000000 lighter-v1-python-1.0.5/lighter_v1_python.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmetavci   (501) staff       (20)      194 2023-07-18 12:06:30.000000 lighter-v1-python-1.0.5/lighter_v1_python.egg-info/requires.txt
+-rw-r--r--   0 ahmetavci   (501) staff       (20)        8 2023-07-18 12:06:30.000000 lighter-v1-python-1.0.5/lighter_v1_python.egg-info/top_level.txt
+-rw-r--r--   0 ahmetavci   (501) staff       (20)       38 2023-07-18 12:06:30.439356 lighter-v1-python-1.0.5/setup.cfg
+-rw-r--r--   0 ahmetavci   (501) staff       (20)     1426 2023-07-18 12:00:49.000000 lighter-v1-python-1.0.5/setup.py
```

### Comparing `lighter-v1-python-1.0.4/LICENSE` & `lighter-v1-python-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lighter-v1-python-1.0.4/PKG-INFO` & `lighter-v1-python-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lighter-v1-python
-Version: 1.0.4
+Version: 1.0.5
 Summary: lighter Python rest api and blockchain interactions for Limit Orders
 Home-page: https://github.com/elliottech/lighter-v1-python
 Author: Elliot
 Author-email: ahmet@elliot.ai
 License: Apache 2.0
 Keywords: lighter exchange rest api defi ethereum optimism l2 eth
 Classifier: Intended Audience :: Developers
@@ -30,18 +30,18 @@
 
 ## Getting Started
 
 The `Client` object has four main modules;
 
 - `Api`: allows interaction with the lighter api
 - `AsyncApi`: allows for async interaction with the lighter api
-- `Blockchain`: allows interaction with ligter contracts
-- `AsyncBlockchain`: allows async interaction with ligter contracts
+- `Blockchain`: allows interaction with lighter contracts
+- `AsyncBlockchain`: allows async interaction with lighter contracts
 
-`Client` can be created with private key or not depending on whether you are going to use the api or interract with the contracts. For more complete examples, see the [examples](./examples/) directory.
+`Client` can be created with private key or not depending on whether you are going to use the api or interact with the contracts. For more complete examples, see the [examples](./examples/) directory.
 
 ### API
 
 Following parameters are required to use `Api` module:
 
 - `api_auth`: You should get the key from our servers.
 - `web3_provider_url`: You need a node to interact with the contract. We suggest alchemy which provides 300M free compute units monthly, You can register and get your keys [here](https://www.alchemy.com/)
@@ -66,15 +66,15 @@
 
 Following parameters are required to use `Blockchain` module:
 
 - `api_auth`: You should get the key from our servers.
 - `private_key`: You need to provide your wallet private key to sign your transactions.
 - `web3_provider_url`: You need a node to interact with the contract. We suggest alchemy which provides 300M free compute units monthly, You can register and get your keys [here](https://www.alchemy.com/)
 
-Blockchain module enables you to do multiple operations in one transaction. The number of operations is limited to 4 millions gas. So the limits are rougly;
+Blockchain module enables you to do multiple operations in one transaction. The number of operations is limited to 4 million gas. So the limits are roughly;
 
 - 25 order creations in one transaction
 - 100 order cancellations in one transaction
 - 25 order updates in one transaction
 
 ```python
 from lighter.lighter_client import Client
@@ -134,15 +134,15 @@
 
 client = Client(
     private_key=private_key, api_auth=api_auth, web3_provider_url="ALCHEMY_URL"
 )
 
 
 async def main():
-    client.async_blockchain # to initalize the module
+    client.async_blockchain # to initialize the module
     sizes = ["0.0001"]
     prices = ["1000"]
     sides = [OrderSide.SELL]
 
     # Test async api
     print(await client.async_api.get_blockchains())
     print(await client.async_api.get_orderbook("WETH_USDC"))
```

### Comparing `lighter-v1-python-1.0.4/README.md` & `lighter-v1-python-1.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 
 ## Getting Started
 
 The `Client` object has four main modules;
 
 - `Api`: allows interaction with the lighter api
 - `AsyncApi`: allows for async interaction with the lighter api
-- `Blockchain`: allows interaction with ligter contracts
-- `AsyncBlockchain`: allows async interaction with ligter contracts
+- `Blockchain`: allows interaction with lighter contracts
+- `AsyncBlockchain`: allows async interaction with lighter contracts
 
-`Client` can be created with private key or not depending on whether you are going to use the api or interract with the contracts. For more complete examples, see the [examples](./examples/) directory.
+`Client` can be created with private key or not depending on whether you are going to use the api or interact with the contracts. For more complete examples, see the [examples](./examples/) directory.
 
 ### API
 
 Following parameters are required to use `Api` module:
 
 - `api_auth`: You should get the key from our servers.
 - `web3_provider_url`: You need a node to interact with the contract. We suggest alchemy which provides 300M free compute units monthly, You can register and get your keys [here](https://www.alchemy.com/)
@@ -46,15 +46,15 @@
 
 Following parameters are required to use `Blockchain` module:
 
 - `api_auth`: You should get the key from our servers.
 - `private_key`: You need to provide your wallet private key to sign your transactions.
 - `web3_provider_url`: You need a node to interact with the contract. We suggest alchemy which provides 300M free compute units monthly, You can register and get your keys [here](https://www.alchemy.com/)
 
-Blockchain module enables you to do multiple operations in one transaction. The number of operations is limited to 4 millions gas. So the limits are rougly;
+Blockchain module enables you to do multiple operations in one transaction. The number of operations is limited to 4 million gas. So the limits are roughly;
 
 - 25 order creations in one transaction
 - 100 order cancellations in one transaction
 - 25 order updates in one transaction
 
 ```python
 from lighter.lighter_client import Client
@@ -114,15 +114,15 @@
 
 client = Client(
     private_key=private_key, api_auth=api_auth, web3_provider_url="ALCHEMY_URL"
 )
 
 
 async def main():
-    client.async_blockchain # to initalize the module
+    client.async_blockchain # to initialize the module
     sizes = ["0.0001"]
     prices = ["1000"]
     sides = [OrderSide.SELL]
 
     # Test async api
     print(await client.async_api.get_blockchains())
     print(await client.async_api.get_orderbook("WETH_USDC"))
```

### Comparing `lighter-v1-python-1.0.4/lighter/abi/erc20.json` & `lighter-v1-python-1.0.5/lighter/abi/erc20.json`

 * *Files identical despite different names*

### Comparing `lighter-v1-python-1.0.4/lighter/abi/factory.json` & `lighter-v1-python-1.0.5/lighter/abi/factory.json`

 * *Files identical despite different names*

### Comparing `lighter-v1-python-1.0.4/lighter/abi/orderbook.json` & `lighter-v1-python-1.0.5/lighter/abi/orderbook.json`

 * *Files identical despite different names*

### Comparing `lighter-v1-python-1.0.4/lighter/abi/router.json` & `lighter-v1-python-1.0.5/lighter/abi/router.json`

 * *Files identical despite different names*

### Comparing `lighter-v1-python-1.0.4/lighter/constants.py` & `lighter-v1-python-1.0.5/lighter/constants.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,54 @@
-HOST = "https://mensa.elliot.ai"
+HOST = "https://api.lighter.xyz"
 TEST_HOST = "https://lighter-test.elliot.ai"
 
 # ------------ Blockchain IDs -----------
 BLOCKCHAIN_ARBITRUM_GOERLI_ID = 421613
 BLOCKCHAIN_ARBITRUM_ID = 42161
 
 # ------------ Assets -------------------
 TOKEN_USDC = "USDC"
 TOKEN_WBTC = "WBTC"
 TOKEN_WETH = "WETH"
 TOKEN_LINK = "LINK"
 TOKEN_UNI = "UNI"
 
 # ------------ Orderbooks -------------------
-ORDERBOOK_WETH_USDC = "WETH_USDC"
-ORDERBOOK_WBTC_USDC = "WBTC_USDC"
-ORDERBOOK_WETH_WBTC = "WETH_WBTC"
-ORDERBOOK_UNI_USDC = "UNI_USDC"
-ORDERBOOK_LINK_USDC = "LINK_USDC"
-
+ORDERBOOK_WETH_USDC = "WETH-USDC"
+ORDERBOOK_WBTC_USDC = "WBTC-USDC"
+ORDERBOOK_WETH_WBTC = "WETH-WBTC"
+ORDERBOOK_UNI_USDC = "UNI-USDC"
+ORDERBOOK_LINK_USDC = "LINK-USDC"
+ORDERBOOK_USDT_USDC = "USDT-USDC"
+ORDERBOOK_USDC_USDC = "USDC-USDC"
 
 # ------------ Order Statuses -------------------
-ORDER_STATUS_OPEN = "partially_filled"
+ORDER_STATUS_OPEN = "open"
 ORDER_STATUS_FILLED = "filled"
 ORDER_STATUS_CANCELLED = "canceled"
 
 # ------------ Order Types -------------------
 ORDER_TYPE_LIMIT = "limit"
 ORDER_TYPE_MARKET = "market"
 
 
+# ------------ Order Sides -------------------
+ORDER_SIDE_SELL = "sell"
+ORDER_SIDE_BUY = "buy"
+
+
+# ------------ Candlestick Resolutions -------------------
+CANDLESTICK_RESOLUTION_1MIN = "1min"
+CANDLESTICK_RESOLUTION_5MIN = "5min"
+CANDLESTICK_RESOLUTION_15MIN = "15min"
+CANDLESTICK_RESOLUTION_1H = "1h"
+CANDLESTICK_RESOLUTION_4H = "4h"
+CANDLESTICK_RESOLUTION_1D = "1d"
+
+
 # ------------ Ethereum Transactions ------------
 DEFAULT_GAS_AMOUNT = 4000000
 DEFAULT_GAS_MULTIPLIER = 1.2
 DEFAULT_GAS_PRICE = 4000000000
 DEFAULT_MAX_FEE_PER_GAS = 2000000000
 DEFAULT_MAX_PRIORITY_FEE_PER_GAS = 0
 MAX_SOLIDITY_UINT = (
```

### Comparing `lighter-v1-python-1.0.4/lighter/errors.py` & `lighter-v1-python-1.0.5/lighter/errors.py`

 * *Files identical despite different names*

### Comparing `lighter-v1-python-1.0.4/lighter/lighter_client.py` & `lighter-v1-python-1.0.5/lighter/lighter_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,19 +71,18 @@
     def blockchain(self):
         """
         Get the blockchain module, used for interracting with contracts.
         """
 
         if not self._blockchain:
             if self.web3 and self.private_key:
-                orderbooks: List[Orderbook] = self.api.get_orderbook_meta()[
-                    "orderbookmetas"
-                ]
+                orderbooks: List[Orderbook] = self.api.get_orderbook_meta()
+                
 
-                chains = self.api.get_blockchains()["blockchains"]
+                chains = self.api.get_blockchains()
 
                 chain = next(
                     (
                         item
                         for item in chains
                         if item["chain_id"] == str(self.blockchain_id)
                     ),
@@ -118,19 +117,18 @@
     def async_blockchain(self) -> AsyncBlockchain:
         """
         Get the blockchain module, used for interracting with contracts.
         """
 
         if not self._async_blockchain:
             if self.async_web3 and self.private_key:
-                orderbooks: List[Orderbook] = self.api.get_orderbook_meta()[
-                    "orderbookmetas"
-                ]
+                orderbooks: List[Orderbook] = self.api.get_orderbook_meta()
+                
 
-                chains = self.api.get_blockchains()["blockchains"]
+                chains = self.api.get_blockchains()
 
                 chain = next(
                     (
                         item
                         for item in chains
                         if item["chain_id"] == str(self.blockchain_id)
                     ),
```

### Comparing `lighter-v1-python-1.0.4/lighter/modules/api.py` & `lighter-v1-python-1.0.5/lighter/modules/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,40 +76,45 @@
                 raise LighterApiError(f"Invalid response: {await response.text}")
 
     async def get_blockchains(self) -> dict:
         uri = "/blockchains"
         return await self._get(uri)
 
     async def get_orderbook_meta(self) -> dict:
-        uri = "/orderbookmetas"
+        uri = "/order_book_metas"
         return await self._get(uri, {"blockchain_id": self.blockchain_id})
 
     async def get_orderbook(self, orderbook_symbol: str) -> dict:
-        uri = "/orderbook"
+        uri = "/order_book"
         return await self._get(
             uri,
-            {"blockchain_id": self.blockchain_id, "orderbook_symbol": orderbook_symbol},
+            {
+                "blockchain_id": self.blockchain_id,
+                "order_book_symbol": orderbook_symbol,
+            },
         )
 
     async def get_candles(
         self,
         orderbook_symbol: str,
-        resolution: int,
         timestamp_start: int,
         timestamp_end: int,
+        resolution: str,
+        count_back: Optional[int] = None,
     ) -> dict:
-        uri = "/candles"
+        uri = "/candlesticks"
         return await self._get(
             uri,
             {
                 "blockchain_id": self.blockchain_id,
-                "orderbook_symbol": orderbook_symbol,
-                "resolution_min": resolution,
+                "order_book_symbol": orderbook_symbol,
                 "start_timestamp": timestamp_start,
                 "end_timestamp": timestamp_end,
+                "resolution": resolution,
+                "count_back": count_back,
             },
         )
 
     async def get_orders(
         self,
         owner: str,
         orderbook_symbol: Optional[str] = None,
@@ -120,66 +125,64 @@
         end_timestamp: Optional[int] = None,
     ) -> dict:
         uri = "/orders"
         return await self._get(
             uri,
             {
                 "blockchain_id": self.blockchain_id,
-                "orderbook_symbol": orderbook_symbol,
+                "order_book_symbol": orderbook_symbol,
                 "owner": owner,
                 "status": status,
                 "type": type,
                 "limit": limit,
                 "start_timestamp": start_timestamp,
                 "end_timestamp": end_timestamp,
             },
         )
 
     async def get_trades(
         self,
         owner: str,
-        orderbook_symbol: Optional[str] = None,
+        orderbook_symbol: str,
         limit: Optional[int] = None,
         starting_before: Optional[int] = None,
     ) -> dict:
         uri = "/trades"
         return await self._get(
             uri,
             {
                 "blockchain_id": self.blockchain_id,
-                "orderbook_symbol": orderbook_symbol,
+                "order_book_symbol": orderbook_symbol,
                 "owner": owner,
                 "limit": limit,
                 "before": starting_before,
             },
         )
 
-    async def _get_hint_ids(
+    async def get_hint_ids(
         self, orderbook_symbol: str, prices: List[str], sides: List[str]
     ) -> dict:
         uri = "/hint_id"
         return await self._get(
             uri,
             {
                 "blockchain_id": self.blockchain_id,
-                "orderbook_symbol": orderbook_symbol,
+                "order_book_symbol": orderbook_symbol,
                 "prices": ",".join(prices),
                 "sides": ",".join(sides),
             },
-            False,
         )
 
-    async def _get_gas_price(self) -> dict:
+    async def get_gas_price(self) -> dict:
         uri = "/gas_price"
         return await self._get(
             uri,
             {
                 "blockchain_id": self.blockchain_id,
             },
-            False,
         )
 
 
 class Api(BaseApi):
     def __init__(
         self,
         host: str,
@@ -224,104 +227,109 @@
 
     # ============ Requests ============
     def get_blockchains(self) -> dict:
         uri = "/blockchains"
         return self._get(uri)
 
     def get_orderbook_meta(self) -> dict:
-        uri = "/orderbookmetas"
+        uri = "/order_book_metas"
         return self._get(uri, {"blockchain_id": self.blockchain_id})
 
     def get_orderbook(self, orderbook_symbol: str) -> dict:
-        uri = "/orderbook"
+        uri = "/order_book"
         return self._get(
             uri,
-            {"blockchain_id": self.blockchain_id, "orderbook_symbol": orderbook_symbol},
+            {
+                "blockchain_id": self.blockchain_id,
+                "order_book_symbol": orderbook_symbol,
+            },
         )
 
     def get_candles(
         self,
         orderbook_symbol: str,
-        resolution: int,
         timestamp_start: int,
         timestamp_end: int,
+        resolution: str,
+        count_back: Optional[int] = None,
     ) -> dict:
-        uri = "/candles"
+        uri = "/candlesticks"
         return self._get(
             uri,
             {
                 "blockchain_id": self.blockchain_id,
-                "orderbook_symbol": orderbook_symbol,
-                "resolution_min": resolution,
+                "order_book_symbol": orderbook_symbol,
                 "start_timestamp": timestamp_start,
                 "end_timestamp": timestamp_end,
+                "resolution": resolution,
+                "count_back": count_back,
             },
         )
 
     def get_orders(
         self,
         owner: str,
         orderbook_symbol: Optional[str] = None,
         status: Optional[str] = None,
+        side: Optional[str] = None,
         type: Optional[str] = None,
         limit: Optional[int] = None,
         start_timestamp: Optional[int] = None,
         end_timestamp: Optional[int] = None,
     ) -> dict:
         uri = "/orders"
         return self._get(
             uri,
             {
                 "blockchain_id": self.blockchain_id,
-                "orderbook_symbol": orderbook_symbol,
+                "order_book_symbol": orderbook_symbol,
                 "owner": owner,
                 "status": status,
                 "type": type,
+                "side": side,
                 "limit": limit,
-                "start_timestamp": start_timestamp,
-                "end_timestamp": end_timestamp,
+                "after": start_timestamp,
+                "before": end_timestamp,
             },
         )
 
     def get_trades(
         self,
         owner: str,
-        orderbook_symbol: Optional[str] = None,
+        orderbook_symbol: str,
         limit: Optional[int] = None,
         starting_before: Optional[int] = None,
     ) -> dict:
         uri = "/trades"
         return self._get(
             uri,
             {
                 "blockchain_id": self.blockchain_id,
-                "orderbook_symbol": orderbook_symbol,
+                "order_book_symbol": orderbook_symbol,
                 "owner": owner,
                 "limit": limit,
                 "before": starting_before,
             },
         )
 
-    def _get_hint_ids(
+    def get_hint_ids(
         self, orderbook_symbol: str, prices: List[str], sides: List[str]
     ) -> dict:
         uri = "/hint_id"
         return self._get(
             uri,
             {
                 "blockchain_id": self.blockchain_id,
-                "orderbook_symbol": orderbook_symbol,
+                "order_book_symbol": orderbook_symbol,
                 "prices": ",".join(prices),
                 "sides": ",".join(sides),
             },
-            False,
         )
 
-    def _get_gas_price(self) -> dict:
+    def get_gas_price(self) -> dict:
         uri = "/gas_price"
         return self._get(
             uri,
             {
                 "blockchain_id": self.blockchain_id,
             },
-            False,
         )
```

### Comparing `lighter-v1-python-1.0.4/lighter/modules/blockchain.py` & `lighter-v1-python-1.0.5/lighter/modules/blockchain.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 Token = TypedDict(
     "Token", {"symbol": str, "decimal": int, "address": str, "pow_decimal": int}
 )
 
 
 class OrderStatus(Enum):
-    PARTIALLY_FILLED = "PARTIALLY_FILLED"
+    OPEN = "OPEN"
     FILLED = "FILLED"
     CANCELED = "CANCELED"
 
 
 class OrderType(Enum):
     LIMIT = "LIMIT"
     MARKET = "MARKET"
@@ -770,15 +770,15 @@
                     "orderbook": orderbook_symbol,
                     "order_id": created_event["order_id"],
                     "size": created_event["size"],
                     "filled_size": fill_size,
                     "price": created_event["price"],
                     "status": OrderStatus.FILLED
                     if fill_size == created_event["size"]
-                    else OrderStatus.PARTIALLY_FILLED,
+                    else OrderStatus.OPEN,
                     "type": created_event["type"],
                     "side": created_event["side"],
                     "fills": fills,
                 }
             )
 
         return {
@@ -1024,15 +1024,15 @@
         orderbook = self._get_orderbook(orderbook_symbol)
         sides_str = [side.value.lower() for side in sides]
         return (await self._api._get_hint_ids(orderbook["symbol"], prices, sides_str))[
             "hint_ids"
         ]
 
     async def _get_gas_price(self) -> int:
-        return (await self._api._get_gas_price())["gas_price"]
+        return (await self._api.get_gas_price())["gas_price"]
 
     async def get_eth_balance(
         self,
         owner: Optional[str] = None,
     ) -> Union[int, decimal.Decimal]:
         owner = owner or (await self.account).address
         if owner is None:
@@ -1419,15 +1419,15 @@
                     "orderbook": orderbook_symbol,
                     "order_id": created_event["order_id"],
                     "size": created_event["size"],
                     "filled_size": fill_size,
                     "price": created_event["price"],
                     "status": OrderStatus.FILLED
                     if fill_size == created_event["size"]
-                    else OrderStatus.PARTIALLY_FILLED,
+                    else OrderStatus.OPEN,
                     "type": created_event["type"],
                     "side": created_event["side"],
                     "fills": fills,
                 }
             )
 
         return {
@@ -1667,15 +1667,15 @@
         orderbook = self._get_orderbook(orderbook_symbol)
         sides_str = [side.value.lower() for side in sides]
         return self._api._get_hint_ids(orderbook["symbol"], prices, sides_str)[
             "hint_ids"
         ]
 
     def _get_gas_price(self) -> int:
-        return self._api._get_gas_price()["gas_price"]
+        return self._api.get_gas_price()["gas_price"]
 
     def get_eth_balance(
         self,
         owner: Optional[str] = None,
     ) -> Union[int, decimal.Decimal]:
         owner = owner or self.account.address
         if owner is None:
```

### Comparing `lighter-v1-python-1.0.4/lighter_v1_python.egg-info/PKG-INFO` & `lighter-v1-python-1.0.5/lighter_v1_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lighter-v1-python
-Version: 1.0.4
+Version: 1.0.5
 Summary: lighter Python rest api and blockchain interactions for Limit Orders
 Home-page: https://github.com/elliottech/lighter-v1-python
 Author: Elliot
 Author-email: ahmet@elliot.ai
 License: Apache 2.0
 Keywords: lighter exchange rest api defi ethereum optimism l2 eth
 Classifier: Intended Audience :: Developers
@@ -30,18 +30,18 @@
 
 ## Getting Started
 
 The `Client` object has four main modules;
 
 - `Api`: allows interaction with the lighter api
 - `AsyncApi`: allows for async interaction with the lighter api
-- `Blockchain`: allows interaction with ligter contracts
-- `AsyncBlockchain`: allows async interaction with ligter contracts
+- `Blockchain`: allows interaction with lighter contracts
+- `AsyncBlockchain`: allows async interaction with lighter contracts
 
-`Client` can be created with private key or not depending on whether you are going to use the api or interract with the contracts. For more complete examples, see the [examples](./examples/) directory.
+`Client` can be created with private key or not depending on whether you are going to use the api or interact with the contracts. For more complete examples, see the [examples](./examples/) directory.
 
 ### API
 
 Following parameters are required to use `Api` module:
 
 - `api_auth`: You should get the key from our servers.
 - `web3_provider_url`: You need a node to interact with the contract. We suggest alchemy which provides 300M free compute units monthly, You can register and get your keys [here](https://www.alchemy.com/)
@@ -66,15 +66,15 @@
 
 Following parameters are required to use `Blockchain` module:
 
 - `api_auth`: You should get the key from our servers.
 - `private_key`: You need to provide your wallet private key to sign your transactions.
 - `web3_provider_url`: You need a node to interact with the contract. We suggest alchemy which provides 300M free compute units monthly, You can register and get your keys [here](https://www.alchemy.com/)
 
-Blockchain module enables you to do multiple operations in one transaction. The number of operations is limited to 4 millions gas. So the limits are rougly;
+Blockchain module enables you to do multiple operations in one transaction. The number of operations is limited to 4 million gas. So the limits are roughly;
 
 - 25 order creations in one transaction
 - 100 order cancellations in one transaction
 - 25 order updates in one transaction
 
 ```python
 from lighter.lighter_client import Client
@@ -134,15 +134,15 @@
 
 client = Client(
     private_key=private_key, api_auth=api_auth, web3_provider_url="ALCHEMY_URL"
 )
 
 
 async def main():
-    client.async_blockchain # to initalize the module
+    client.async_blockchain # to initialize the module
     sizes = ["0.0001"]
     prices = ["1000"]
     sides = [OrderSide.SELL]
 
     # Test async api
     print(await client.async_api.get_blockchains())
     print(await client.async_api.get_orderbook("WETH_USDC"))
```

### Comparing `lighter-v1-python-1.0.4/lighter_v1_python.egg-info/SOURCES.txt` & `lighter-v1-python-1.0.5/lighter_v1_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lighter-v1-python-1.0.4/setup.py` & `lighter-v1-python-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "dateparser>=1.0.0",
     "nest-asyncio>=1.5.6",
     "pytest-asyncio>=0.21.0",
 ]
 
 setup(
     name="lighter-v1-python",
-    version="1.0.4",
+    version="1.0.5",
     packages=find_packages(),
     package_data={
         "lighter": [
             "abi/*.json",
         ],
     },
     description="lighter Python rest api and blockchain interactions for Limit Orders",
```

