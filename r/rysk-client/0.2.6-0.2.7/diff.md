# Comparing `tmp/rysk_client-0.2.6.tar.gz` & `tmp/rysk_client-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rysk_client-0.2.6.tar", max compression
+gzip compressed data, was "rysk_client-0.2.7.tar", max compression
```

## Comparing `rysk_client-0.2.6.tar` & `rysk_client-0.2.7.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0    45006 2023-07-18 12:45:47.828723 rysk_client-0.2.6/README.md
--rw-r--r--   0        0        0      726 2023-07-18 12:45:47.832723 rysk_client-0.2.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/__init__.py
--rw-r--r--   0        0        0     9029 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/cli.py
--rw-r--r--   0        0        0    24651 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/client.py
--rw-r--r--   0        0        0      974 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/beyond_pricer/__init__.py
--rw-r--r--   0        0        0    35992 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/beyond_pricer/build/beyond_pricer.json
--rw-r--r--   0        0        0    13187 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.py
--rw-r--r--   0        0        0      527 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.yaml
--rw-r--r--   0        0        0      971 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/d_h_v_lens/__init__.py
--rw-r--r--   0        0        0    35311 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/d_h_v_lens/build/d_h_v_lens.json
--rw-r--r--   0        0        0     6580 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.py
--rw-r--r--   0        0        0      601 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.yaml
--rw-r--r--   0        0        0      968 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/o_token/__init__.py
--rw-r--r--   0        0        0    15813 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/o_token/build/o_token.json
--rw-r--r--   0        0        0     8845 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/o_token/contract.py
--rw-r--r--   0        0        0      509 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/o_token/contract.yaml
--rw-r--r--   0        0        0      976 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/option_exchange/__init__.py
--rw-r--r--   0        0        0    38053 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/option_exchange/build/option_exchange.json
--rw-r--r--   0        0        0    11285 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/option_exchange/contract.py
--rw-r--r--   0        0        0      533 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/option_exchange/contract.yaml
--rw-r--r--   0        0        0      976 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/opyn_controller/__init__.py
--rw-r--r--   0        0        0    42143 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/opyn_controller/build/opyn_controller.json
--rw-r--r--   0        0        0    13308 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/opyn_controller/contract.py
--rw-r--r--   0        0        0      533 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/opyn_controller/contract.yaml
--rw-r--r--   0        0        0      981 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/opyn_option_registry/__init__.py
--rw-r--r--   0        0        0    38232 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/opyn_option_registry/build/opyn_option_registry.json
--rw-r--r--   0        0        0    10787 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.py
--rw-r--r--   0        0        0      547 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.yaml
--rw-r--r--   0        0        0      965 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/usdc/__init__.py
--rw-r--r--   0        0        0    11137 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/usdc/build/usdc.json
--rw-r--r--   0        0        0     6104 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/usdc/contract.py
--rw-r--r--   0        0        0      580 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/usdc/contract.yaml
--rw-r--r--   0        0        0      979 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/user_position_lens/__init__.py
--rw-r--r--   0        0        0     2515 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/user_position_lens/build/user_position_lens.json
--rw-r--r--   0        0        0     4220 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/user_position_lens/contract.py
--rw-r--r--   0        0        0      541 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/user_position_lens/contract.yaml
--rw-r--r--   0        0        0      965 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/weth/__init__.py
--rw-r--r--   0        0        0    15880 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/weth/build/weth.json
--rw-r--r--   0        0        0     6490 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/weth/contract.py
--rw-r--r--   0        0        0      580 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/weth/contract.yaml
--rw-r--r--   0        0        0      488 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/packages/packages.json
--rw-r--r--   0        0        0      690 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/src/action_type.py
--rw-r--r--   0        0        0     1142 2023-07-18 12:45:47.832723 rysk_client-0.2.6/rysk_client/src/collateral.py
--rw-r--r--   0        0        0     5480 2023-07-18 12:45:47.836722 rysk_client-0.2.6/rysk_client/src/constants.py
--rw-r--r--   0        0        0      212 2023-07-18 12:45:47.836722 rysk_client-0.2.6/rysk_client/src/crypto.py
--rw-r--r--   0        0        0      185 2023-07-18 12:45:47.836722 rysk_client-0.2.6/rysk_client/src/exceptions.py
--rw-r--r--   0        0        0     9777 2023-07-18 12:45:47.836722 rysk_client-0.2.6/rysk_client/src/operation_factory.py
--rw-r--r--   0        0        0      507 2023-07-18 12:45:47.836722 rysk_client-0.2.6/rysk_client/src/order.py
--rw-r--r--   0        0        0      182 2023-07-18 12:45:47.836722 rysk_client-0.2.6/rysk_client/src/order_side.py
--rw-r--r--   0        0        0     4538 2023-07-18 12:45:47.836722 rysk_client-0.2.6/rysk_client/src/pnl_calculator.py
--rw-r--r--   0        0        0      517 2023-07-18 12:45:47.836722 rysk_client-0.2.6/rysk_client/src/position.py
--rw-r--r--   0        0        0     1114 2023-07-18 12:45:47.836722 rysk_client-0.2.6/rysk_client/src/position_manager.py
--rw-r--r--   0        0        0      193 2023-07-18 12:45:47.836722 rysk_client-0.2.6/rysk_client/src/position_side.py
--rw-r--r--   0        0        0     9137 2023-07-18 12:45:47.836722 rysk_client-0.2.6/rysk_client/src/rysk_option_market.py
--rw-r--r--   0        0        0     3253 2023-07-18 12:45:47.836722 rysk_client-0.2.6/rysk_client/src/subgraph.py
--rw-r--r--   0        0        0     3443 2023-07-18 12:45:47.836722 rysk_client-0.2.6/rysk_client/src/utils.py
--rw-r--r--   0        0        0    13973 2023-07-18 12:45:47.836722 rysk_client-0.2.6/rysk_client/web3_client.py
--rw-r--r--   0        0        0    45624 1970-01-01 00:00:00.000000 rysk_client-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0    45006 2023-07-18 12:45:47.898309 rysk_client-0.2.7/README.md
+-rw-r--r--   0        0        0      726 2023-07-18 12:45:47.898309 rysk_client-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-18 12:45:47.898309 rysk_client-0.2.7/rysk_client/__init__.py
+-rw-r--r--   0        0        0     9029 2023-07-18 12:45:47.898309 rysk_client-0.2.7/rysk_client/cli.py
+-rw-r--r--   0        0        0    24651 2023-07-18 12:45:47.898309 rysk_client-0.2.7/rysk_client/client.py
+-rw-r--r--   0        0        0      974 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/beyond_pricer/__init__.py
+-rw-r--r--   0        0        0    35992 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/beyond_pricer/build/beyond_pricer.json
+-rw-r--r--   0        0        0    13187 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.py
+-rw-r--r--   0        0        0      527 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.yaml
+-rw-r--r--   0        0        0      971 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/d_h_v_lens/__init__.py
+-rw-r--r--   0        0        0    35311 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/d_h_v_lens/build/d_h_v_lens.json
+-rw-r--r--   0        0        0     6580 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.py
+-rw-r--r--   0        0        0      601 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.yaml
+-rw-r--r--   0        0        0      968 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/o_token/__init__.py
+-rw-r--r--   0        0        0    15813 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/o_token/build/o_token.json
+-rw-r--r--   0        0        0     8845 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/o_token/contract.py
+-rw-r--r--   0        0        0      509 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/o_token/contract.yaml
+-rw-r--r--   0        0        0      976 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/option_exchange/__init__.py
+-rw-r--r--   0        0        0    38053 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/option_exchange/build/option_exchange.json
+-rw-r--r--   0        0        0    11285 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/option_exchange/contract.py
+-rw-r--r--   0        0        0      533 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/option_exchange/contract.yaml
+-rw-r--r--   0        0        0      976 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/opyn_controller/__init__.py
+-rw-r--r--   0        0        0    42143 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/opyn_controller/build/opyn_controller.json
+-rw-r--r--   0        0        0    13308 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/opyn_controller/contract.py
+-rw-r--r--   0        0        0      533 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/opyn_controller/contract.yaml
+-rw-r--r--   0        0        0      981 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/opyn_option_registry/__init__.py
+-rw-r--r--   0        0        0    38232 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/opyn_option_registry/build/opyn_option_registry.json
+-rw-r--r--   0        0        0    10787 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.py
+-rw-r--r--   0        0        0      547 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.yaml
+-rw-r--r--   0        0        0      965 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/usdc/__init__.py
+-rw-r--r--   0        0        0    11137 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/usdc/build/usdc.json
+-rw-r--r--   0        0        0     6104 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/usdc/contract.py
+-rw-r--r--   0        0        0      580 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/usdc/contract.yaml
+-rw-r--r--   0        0        0      979 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/user_position_lens/__init__.py
+-rw-r--r--   0        0        0     2515 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/user_position_lens/build/user_position_lens.json
+-rw-r--r--   0        0        0     4220 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/user_position_lens/contract.py
+-rw-r--r--   0        0        0      541 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/user_position_lens/contract.yaml
+-rw-r--r--   0        0        0      965 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/weth/__init__.py
+-rw-r--r--   0        0        0    15880 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/weth/build/weth.json
+-rw-r--r--   0        0        0     6490 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/weth/contract.py
+-rw-r--r--   0        0        0      580 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/weth/contract.yaml
+-rw-r--r--   0        0        0      488 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/packages/packages.json
+-rw-r--r--   0        0        0      690 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/src/action_type.py
+-rw-r--r--   0        0        0     1142 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/src/collateral.py
+-rw-r--r--   0        0        0     5480 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/src/constants.py
+-rw-r--r--   0        0        0      212 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/src/crypto.py
+-rw-r--r--   0        0        0      185 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/src/exceptions.py
+-rw-r--r--   0        0        0     9777 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/src/operation_factory.py
+-rw-r--r--   0        0        0      507 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/src/order.py
+-rw-r--r--   0        0        0      182 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/src/order_side.py
+-rw-r--r--   0        0        0     4538 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/src/pnl_calculator.py
+-rw-r--r--   0        0        0      517 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/src/position.py
+-rw-r--r--   0        0        0     1114 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/src/position_manager.py
+-rw-r--r--   0        0        0      193 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/src/position_side.py
+-rw-r--r--   0        0        0     9137 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/src/rysk_option_market.py
+-rw-r--r--   0        0        0     3253 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/src/subgraph.py
+-rw-r--r--   0        0        0     3443 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/src/utils.py
+-rw-r--r--   0        0        0    13973 2023-07-18 12:45:47.902309 rysk_client-0.2.7/rysk_client/web3_client.py
+-rw-r--r--   0        0        0    45624 1970-01-01 00:00:00.000000 rysk_client-0.2.7/PKG-INFO
```

### Comparing `rysk_client-0.2.6/README.md` & `rysk_client-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/pyproject.toml` & `rysk_client-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rysk_client"
-version = "0.2.6"
+version = "0.2.7"
 description = ""
 authors = ["8baller <8ball030@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "rysk_client", from = "." },
 ]
 
@@ -13,15 +13,15 @@
 ccxt = ">=1.72.82"
 rich-click = "^1.6.1"
 websocket-client = ">=0.32.0,<1"
 web3 = "~5"
 pyyaml = "5.3.1"
 
 [tool.poetry.group.dev.dependencies]
-autonomy-dev = {extras = ["all"], version = "^0.2.6"}
+autonomy-dev = {extras = ["all"], version = "^0.2.7"}
 jupyterlab = ">=1.0.1"
 types-requests = "^2.31.0.1"
 bumpversion = "^0.6.0"
 responses = "^0.23.1"
 pytest-rerunfailures = "^11.1.2"
 docker = "^6.0.0"
```

### Comparing `rysk_client-0.2.6/rysk_client/cli.py` & `rysk_client-0.2.7/rysk_client/cli.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/client.py` & `rysk_client-0.2.7/rysk_client/client.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/beyond_pricer/__init__.py` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/beyond_pricer/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/beyond_pricer/build/beyond_pricer.json` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/beyond_pricer/build/beyond_pricer.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.py` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.yaml` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/d_h_v_lens/__init__.py` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/d_h_v_lens/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/d_h_v_lens/build/d_h_v_lens.json` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/d_h_v_lens/build/d_h_v_lens.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.py` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.yaml` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/o_token/__init__.py` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/o_token/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/o_token/build/o_token.json` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/o_token/build/o_token.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/o_token/contract.py` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/o_token/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/option_exchange/__init__.py` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/option_exchange/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/option_exchange/build/option_exchange.json` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/option_exchange/build/option_exchange.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/option_exchange/contract.py` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/option_exchange/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/option_exchange/contract.yaml` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/option_exchange/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/opyn_controller/__init__.py` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/opyn_controller/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/opyn_controller/build/opyn_controller.json` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/opyn_controller/build/opyn_controller.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/opyn_controller/contract.py` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/opyn_controller/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/opyn_controller/contract.yaml` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/opyn_controller/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/opyn_option_registry/__init__.py` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/opyn_option_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/opyn_option_registry/build/opyn_option_registry.json` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/opyn_option_registry/build/opyn_option_registry.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.py` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.yaml` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/usdc/__init__.py` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/usdc/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/usdc/build/usdc.json` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/usdc/build/usdc.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/usdc/contract.py` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/usdc/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/usdc/contract.yaml` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/usdc/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/user_position_lens/__init__.py` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/user_position_lens/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/user_position_lens/build/user_position_lens.json` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/user_position_lens/build/user_position_lens.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/user_position_lens/contract.py` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/user_position_lens/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/user_position_lens/contract.yaml` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/user_position_lens/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/weth/__init__.py` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/weth/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/weth/build/weth.json` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/weth/build/weth.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/weth/contract.py` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/weth/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/packages/eightballer/contracts/weth/contract.yaml` & `rysk_client-0.2.7/rysk_client/packages/eightballer/contracts/weth/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/src/action_type.py` & `rysk_client-0.2.7/rysk_client/src/action_type.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/src/collateral.py` & `rysk_client-0.2.7/rysk_client/src/collateral.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/src/constants.py` & `rysk_client-0.2.7/rysk_client/src/constants.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/src/operation_factory.py` & `rysk_client-0.2.7/rysk_client/src/operation_factory.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/src/pnl_calculator.py` & `rysk_client-0.2.7/rysk_client/src/pnl_calculator.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/src/position.py` & `rysk_client-0.2.7/rysk_client/src/position.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/src/position_manager.py` & `rysk_client-0.2.7/rysk_client/src/position_manager.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/src/rysk_option_market.py` & `rysk_client-0.2.7/rysk_client/src/rysk_option_market.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/src/subgraph.py` & `rysk_client-0.2.7/rysk_client/src/subgraph.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/src/utils.py` & `rysk_client-0.2.7/rysk_client/src/utils.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/rysk_client/web3_client.py` & `rysk_client-0.2.7/rysk_client/web3_client.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.6/PKG-INFO` & `rysk_client-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rysk-client
-Version: 0.2.6
+Version: 0.2.7
 Summary: 
 Author: 8baller
 Author-email: 8ball030@gmail.com
 Requires-Python: >=3.8,<=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

