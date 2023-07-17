# Comparing `tmp/rubi-2.1.3.tar.gz` & `tmp/rubi-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubi-2.1.3.tar", max compression
+gzip compressed data, was "rubi-2.1.4.tar", max compression
```

## Comparing `rubi-2.1.3.tar` & `rubi-2.1.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    11357 2023-07-14 16:15:23.260074 rubi-2.1.3/LICENSE
--rw-r--r--   0        0        0     2757 2023-07-14 16:15:23.260074 rubi-2.1.3/README.md
--rw-r--r--   0        0        0     6735 2023-07-14 16:15:23.260074 rubi-2.1.3/network_config/ERC20.json
--rw-r--r--   0        0        0     1920 2023-07-14 16:15:23.260074 rubi-2.1.3/network_config/README.md
--rw-r--r--   0        0        0    32732 2023-07-14 16:15:23.264074 rubi-2.1.3/network_config/abitrum_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-14 16:15:23.264074 rubi-2.1.3/network_config/abitrum_goerli/abis/router.json
--rw-r--r--   0        0        0      721 2023-07-14 16:15:23.264074 rubi-2.1.3/network_config/abitrum_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-07-14 16:15:23.264074 rubi-2.1.3/network_config/optimism/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-14 16:15:23.264074 rubi-2.1.3/network_config/optimism/abis/router.json
--rw-r--r--   0        0        0      745 2023-07-14 16:15:23.264074 rubi-2.1.3/network_config/optimism/network.yaml
--rw-r--r--   0        0        0    32732 2023-07-14 16:15:23.264074 rubi-2.1.3/network_config/optimism_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-14 16:15:23.264074 rubi-2.1.3/network_config/optimism_goerli/abis/router.json
--rw-r--r--   0        0        0      648 2023-07-14 16:15:23.264074 rubi-2.1.3/network_config/optimism_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-07-14 16:15:23.264074 rubi-2.1.3/network_config/polygon_mumbai/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-14 16:15:23.264074 rubi-2.1.3/network_config/polygon_mumbai/abis/router.json
--rw-r--r--   0        0        0      721 2023-07-14 16:15:23.264074 rubi-2.1.3/network_config/polygon_mumbai/network.yaml
--rw-r--r--   0        0        0     1746 2023-07-14 16:15:55.491984 rubi-2.1.3/pyproject.toml
--rw-r--r--   0        0        0      124 2023-07-14 16:15:23.268074 rubi-2.1.3/rubi/__init__.py
--rw-r--r--   0        0        0    29209 2023-07-14 16:15:23.268074 rubi-2.1.3/rubi/client.py
--rw-r--r--   0        0        0      163 2023-07-14 16:15:23.268074 rubi-2.1.3/rubi/contracts/__init__.py
--rw-r--r--   0        0        0    65755 2023-07-14 16:15:23.268074 rubi-2.1.3/rubi/contracts/aid.py
--rw-r--r--   0        0        0    12261 2023-07-14 16:15:23.268074 rubi-2.1.3/rubi/contracts/base_contract.py
--rw-r--r--   0        0        0       74 2023-07-14 16:15:23.268074 rubi-2.1.3/rubi/contracts/contract_types/__init__.py
--rw-r--r--   0        0        0    15898 2023-07-14 16:15:23.268074 rubi-2.1.3/rubi/contracts/contract_types/events.py
--rw-r--r--   0        0        0     2805 2023-07-14 16:15:23.268074 rubi-2.1.3/rubi/contracts/contract_types/transaction_reciept.py
--rw-r--r--   0        0        0    18565 2023-07-14 16:15:23.268074 rubi-2.1.3/rubi/contracts/erc20.py
--rw-r--r--   0        0        0    24878 2023-07-14 16:15:23.268074 rubi-2.1.3/rubi/contracts/market.py
--rw-r--r--   0        0        0    14915 2023-07-14 16:15:23.268074 rubi-2.1.3/rubi/contracts/router.py
--rw-r--r--   0        0        0       77 2023-07-14 16:15:23.268074 rubi-2.1.3/rubi/data/README.md
--rw-r--r--   0        0        0       31 2023-07-14 16:15:23.268074 rubi-2.1.3/rubi/data/__init__.py
--rw-r--r--   0        0        0    10146 2023-07-14 16:15:23.268074 rubi-2.1.3/rubi/data/market.py
--rw-r--r--   0        0        0       72 2023-07-14 16:15:23.268074 rubi-2.1.3/rubi/network/__init__.py
--rw-r--r--   0        0        0     8346 2023-07-14 16:15:23.268074 rubi-2.1.3/rubi/network/network.py
--rw-r--r--   0        0        0       94 2023-07-14 16:15:23.268074 rubi-2.1.3/rubi/rubicon_types/__init__.py
--rw-r--r--   0        0        0    15796 2023-07-14 16:15:23.268074 rubi-2.1.3/rubi/rubicon_types/order.py
--rw-r--r--   0        0        0    11554 2023-07-14 16:15:23.268074 rubi-2.1.3/rubi/rubicon_types/order_query.py
--rw-r--r--   0        0        0     6323 2023-07-14 16:15:23.268074 rubi-2.1.3/rubi/rubicon_types/orderbook.py
--rw-r--r--   0        0        0     2779 2023-07-14 16:15:23.268074 rubi-2.1.3/rubi/rubicon_types/pair.py
--rw-r--r--   0        0        0     3635 1970-01-01 00:00:00.000000 rubi-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-17 22:27:07.371072 rubi-2.1.4/LICENSE
+-rw-r--r--   0        0        0     2757 2023-07-17 22:27:07.371072 rubi-2.1.4/README.md
+-rw-r--r--   0        0        0     6735 2023-07-17 22:27:07.371072 rubi-2.1.4/network_config/ERC20.json
+-rw-r--r--   0        0        0     1920 2023-07-17 22:27:07.371072 rubi-2.1.4/network_config/README.md
+-rw-r--r--   0        0        0    32732 2023-07-17 22:27:07.371072 rubi-2.1.4/network_config/abitrum_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-17 22:27:07.375072 rubi-2.1.4/network_config/abitrum_goerli/abis/router.json
+-rw-r--r--   0        0        0      721 2023-07-17 22:27:07.375072 rubi-2.1.4/network_config/abitrum_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-17 22:27:07.375072 rubi-2.1.4/network_config/optimism/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-17 22:27:07.375072 rubi-2.1.4/network_config/optimism/abis/router.json
+-rw-r--r--   0        0        0      745 2023-07-17 22:27:07.375072 rubi-2.1.4/network_config/optimism/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-17 22:27:07.375072 rubi-2.1.4/network_config/optimism_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-17 22:27:07.375072 rubi-2.1.4/network_config/optimism_goerli/abis/router.json
+-rw-r--r--   0        0        0      648 2023-07-17 22:27:07.375072 rubi-2.1.4/network_config/optimism_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-17 22:27:07.375072 rubi-2.1.4/network_config/polygon_mumbai/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-17 22:27:07.375072 rubi-2.1.4/network_config/polygon_mumbai/abis/router.json
+-rw-r--r--   0        0        0      721 2023-07-17 22:27:07.375072 rubi-2.1.4/network_config/polygon_mumbai/network.yaml
+-rw-r--r--   0        0        0     1746 2023-07-17 22:27:41.599217 rubi-2.1.4/pyproject.toml
+-rw-r--r--   0        0        0      124 2023-07-17 22:27:07.375072 rubi-2.1.4/rubi/__init__.py
+-rw-r--r--   0        0        0    29209 2023-07-17 22:27:07.375072 rubi-2.1.4/rubi/client.py
+-rw-r--r--   0        0        0      163 2023-07-17 22:27:07.375072 rubi-2.1.4/rubi/contracts/__init__.py
+-rw-r--r--   0        0        0    65755 2023-07-17 22:27:07.375072 rubi-2.1.4/rubi/contracts/aid.py
+-rw-r--r--   0        0        0    12261 2023-07-17 22:27:07.375072 rubi-2.1.4/rubi/contracts/base_contract.py
+-rw-r--r--   0        0        0       74 2023-07-17 22:27:07.375072 rubi-2.1.4/rubi/contracts/contract_types/__init__.py
+-rw-r--r--   0        0        0    15898 2023-07-17 22:27:07.375072 rubi-2.1.4/rubi/contracts/contract_types/events.py
+-rw-r--r--   0        0        0     2805 2023-07-17 22:27:07.375072 rubi-2.1.4/rubi/contracts/contract_types/transaction_reciept.py
+-rw-r--r--   0        0        0    18565 2023-07-17 22:27:07.379072 rubi-2.1.4/rubi/contracts/erc20.py
+-rw-r--r--   0        0        0    24878 2023-07-17 22:27:07.379072 rubi-2.1.4/rubi/contracts/market.py
+-rw-r--r--   0        0        0    14915 2023-07-17 22:27:07.379072 rubi-2.1.4/rubi/contracts/router.py
+-rw-r--r--   0        0        0       77 2023-07-17 22:27:07.379072 rubi-2.1.4/rubi/data/README.md
+-rw-r--r--   0        0        0       31 2023-07-17 22:27:07.379072 rubi-2.1.4/rubi/data/__init__.py
+-rw-r--r--   0        0        0    10146 2023-07-17 22:27:07.379072 rubi-2.1.4/rubi/data/market.py
+-rw-r--r--   0        0        0       72 2023-07-17 22:27:07.379072 rubi-2.1.4/rubi/network/__init__.py
+-rw-r--r--   0        0        0     8346 2023-07-17 22:27:07.379072 rubi-2.1.4/rubi/network/network.py
+-rw-r--r--   0        0        0       94 2023-07-17 22:27:07.379072 rubi-2.1.4/rubi/rubicon_types/__init__.py
+-rw-r--r--   0        0        0    15796 2023-07-17 22:27:07.379072 rubi-2.1.4/rubi/rubicon_types/order.py
+-rw-r--r--   0        0        0    11554 2023-07-17 22:27:07.379072 rubi-2.1.4/rubi/rubicon_types/order_query.py
+-rw-r--r--   0        0        0     6323 2023-07-17 22:27:07.379072 rubi-2.1.4/rubi/rubicon_types/orderbook.py
+-rw-r--r--   0        0        0     2779 2023-07-17 22:27:07.379072 rubi-2.1.4/rubi/rubicon_types/pair.py
+-rw-r--r--   0        0        0     3635 1970-01-01 00:00:00.000000 rubi-2.1.4/PKG-INFO
```

### Comparing `rubi-2.1.3/LICENSE` & `rubi-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/README.md` & `rubi-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/network_config/ERC20.json` & `rubi-2.1.4/network_config/ERC20.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/network_config/README.md` & `rubi-2.1.4/network_config/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/network_config/abitrum_goerli/abis/market.json` & `rubi-2.1.4/network_config/abitrum_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/network_config/abitrum_goerli/abis/router.json` & `rubi-2.1.4/network_config/abitrum_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/network_config/abitrum_goerli/network.yaml` & `rubi-2.1.4/network_config/abitrum_goerli/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/network_config/optimism/abis/market.json` & `rubi-2.1.4/network_config/optimism/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/network_config/optimism/abis/router.json` & `rubi-2.1.4/network_config/optimism/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/network_config/optimism/network.yaml` & `rubi-2.1.4/network_config/optimism/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/network_config/optimism_goerli/abis/market.json` & `rubi-2.1.4/network_config/optimism_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/network_config/optimism_goerli/abis/router.json` & `rubi-2.1.4/network_config/optimism_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/network_config/optimism_goerli/network.yaml` & `rubi-2.1.4/network_config/optimism_goerli/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/network_config/polygon_mumbai/abis/market.json` & `rubi-2.1.4/network_config/polygon_mumbai/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/network_config/polygon_mumbai/abis/router.json` & `rubi-2.1.4/network_config/polygon_mumbai/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/network_config/polygon_mumbai/network.yaml` & `rubi-2.1.4/network_config/polygon_mumbai/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/pyproject.toml` & `rubi-2.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rubi"
-version = "2.1.3"
+version = "2.1.4"
 description = "A python SDK for the Rubicon Protocol"
 authors = ["denver <denver@rubicon.finance>", "adam <adam@rubicon.finance>"]
 readme = "README.md"
 include = ["network_config/**/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `rubi-2.1.3/rubi/client.py` & `rubi-2.1.4/rubi/client.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/rubi/contracts/aid.py` & `rubi-2.1.4/rubi/contracts/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/rubi/contracts/base_contract.py` & `rubi-2.1.4/rubi/contracts/base_contract.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/rubi/contracts/contract_types/events.py` & `rubi-2.1.4/rubi/contracts/contract_types/events.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/rubi/contracts/contract_types/transaction_reciept.py` & `rubi-2.1.4/rubi/contracts/contract_types/transaction_reciept.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/rubi/contracts/erc20.py` & `rubi-2.1.4/rubi/contracts/erc20.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/rubi/contracts/market.py` & `rubi-2.1.4/rubi/contracts/market.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/rubi/contracts/router.py` & `rubi-2.1.4/rubi/contracts/router.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/rubi/data/market.py` & `rubi-2.1.4/rubi/data/market.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/rubi/network/network.py` & `rubi-2.1.4/rubi/network/network.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/rubi/rubicon_types/order.py` & `rubi-2.1.4/rubi/rubicon_types/order.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/rubi/rubicon_types/order_query.py` & `rubi-2.1.4/rubi/rubicon_types/order_query.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/rubi/rubicon_types/orderbook.py` & `rubi-2.1.4/rubi/rubicon_types/orderbook.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/rubi/rubicon_types/pair.py` & `rubi-2.1.4/rubi/rubicon_types/pair.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.3/PKG-INFO` & `rubi-2.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubi
-Version: 2.1.3
+Version: 2.1.4
 Summary: A python SDK for the Rubicon Protocol
 Author: denver
 Author-email: denver@rubicon.finance
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

