# Comparing `tmp/rubi-2.1.4.tar.gz` & `tmp/rubi-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubi-2.1.4.tar", max compression
+gzip compressed data, was "rubi-2.1.5.tar", max compression
```

## Comparing `rubi-2.1.4.tar` & `rubi-2.1.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    11357 2023-07-17 22:27:07.371072 rubi-2.1.4/LICENSE
--rw-r--r--   0        0        0     2757 2023-07-17 22:27:07.371072 rubi-2.1.4/README.md
--rw-r--r--   0        0        0     6735 2023-07-17 22:27:07.371072 rubi-2.1.4/network_config/ERC20.json
--rw-r--r--   0        0        0     1920 2023-07-17 22:27:07.371072 rubi-2.1.4/network_config/README.md
--rw-r--r--   0        0        0    32732 2023-07-17 22:27:07.371072 rubi-2.1.4/network_config/abitrum_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-17 22:27:07.375072 rubi-2.1.4/network_config/abitrum_goerli/abis/router.json
--rw-r--r--   0        0        0      721 2023-07-17 22:27:07.375072 rubi-2.1.4/network_config/abitrum_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-07-17 22:27:07.375072 rubi-2.1.4/network_config/optimism/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-17 22:27:07.375072 rubi-2.1.4/network_config/optimism/abis/router.json
--rw-r--r--   0        0        0      745 2023-07-17 22:27:07.375072 rubi-2.1.4/network_config/optimism/network.yaml
--rw-r--r--   0        0        0    32732 2023-07-17 22:27:07.375072 rubi-2.1.4/network_config/optimism_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-17 22:27:07.375072 rubi-2.1.4/network_config/optimism_goerli/abis/router.json
--rw-r--r--   0        0        0      648 2023-07-17 22:27:07.375072 rubi-2.1.4/network_config/optimism_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-07-17 22:27:07.375072 rubi-2.1.4/network_config/polygon_mumbai/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-17 22:27:07.375072 rubi-2.1.4/network_config/polygon_mumbai/abis/router.json
--rw-r--r--   0        0        0      721 2023-07-17 22:27:07.375072 rubi-2.1.4/network_config/polygon_mumbai/network.yaml
--rw-r--r--   0        0        0     1746 2023-07-17 22:27:41.599217 rubi-2.1.4/pyproject.toml
--rw-r--r--   0        0        0      124 2023-07-17 22:27:07.375072 rubi-2.1.4/rubi/__init__.py
--rw-r--r--   0        0        0    29209 2023-07-17 22:27:07.375072 rubi-2.1.4/rubi/client.py
--rw-r--r--   0        0        0      163 2023-07-17 22:27:07.375072 rubi-2.1.4/rubi/contracts/__init__.py
--rw-r--r--   0        0        0    65755 2023-07-17 22:27:07.375072 rubi-2.1.4/rubi/contracts/aid.py
--rw-r--r--   0        0        0    12261 2023-07-17 22:27:07.375072 rubi-2.1.4/rubi/contracts/base_contract.py
--rw-r--r--   0        0        0       74 2023-07-17 22:27:07.375072 rubi-2.1.4/rubi/contracts/contract_types/__init__.py
--rw-r--r--   0        0        0    15898 2023-07-17 22:27:07.375072 rubi-2.1.4/rubi/contracts/contract_types/events.py
--rw-r--r--   0        0        0     2805 2023-07-17 22:27:07.375072 rubi-2.1.4/rubi/contracts/contract_types/transaction_reciept.py
--rw-r--r--   0        0        0    18565 2023-07-17 22:27:07.379072 rubi-2.1.4/rubi/contracts/erc20.py
--rw-r--r--   0        0        0    24878 2023-07-17 22:27:07.379072 rubi-2.1.4/rubi/contracts/market.py
--rw-r--r--   0        0        0    14915 2023-07-17 22:27:07.379072 rubi-2.1.4/rubi/contracts/router.py
--rw-r--r--   0        0        0       77 2023-07-17 22:27:07.379072 rubi-2.1.4/rubi/data/README.md
--rw-r--r--   0        0        0       31 2023-07-17 22:27:07.379072 rubi-2.1.4/rubi/data/__init__.py
--rw-r--r--   0        0        0    10146 2023-07-17 22:27:07.379072 rubi-2.1.4/rubi/data/market.py
--rw-r--r--   0        0        0       72 2023-07-17 22:27:07.379072 rubi-2.1.4/rubi/network/__init__.py
--rw-r--r--   0        0        0     8346 2023-07-17 22:27:07.379072 rubi-2.1.4/rubi/network/network.py
--rw-r--r--   0        0        0       94 2023-07-17 22:27:07.379072 rubi-2.1.4/rubi/rubicon_types/__init__.py
--rw-r--r--   0        0        0    15796 2023-07-17 22:27:07.379072 rubi-2.1.4/rubi/rubicon_types/order.py
--rw-r--r--   0        0        0    11554 2023-07-17 22:27:07.379072 rubi-2.1.4/rubi/rubicon_types/order_query.py
--rw-r--r--   0        0        0     6323 2023-07-17 22:27:07.379072 rubi-2.1.4/rubi/rubicon_types/orderbook.py
--rw-r--r--   0        0        0     2779 2023-07-17 22:27:07.379072 rubi-2.1.4/rubi/rubicon_types/pair.py
--rw-r--r--   0        0        0     3635 1970-01-01 00:00:00.000000 rubi-2.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-17 23:26:52.908798 rubi-2.1.5/LICENSE
+-rw-r--r--   0        0        0     2757 2023-07-17 23:26:52.908798 rubi-2.1.5/README.md
+-rw-r--r--   0        0        0     6735 2023-07-17 23:26:52.912798 rubi-2.1.5/network_config/ERC20.json
+-rw-r--r--   0        0        0     1920 2023-07-17 23:26:52.912798 rubi-2.1.5/network_config/README.md
+-rw-r--r--   0        0        0    32732 2023-07-17 23:26:52.912798 rubi-2.1.5/network_config/abitrum_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-17 23:26:52.912798 rubi-2.1.5/network_config/abitrum_goerli/abis/router.json
+-rw-r--r--   0        0        0      833 2023-07-17 23:26:52.912798 rubi-2.1.5/network_config/abitrum_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-17 23:26:52.912798 rubi-2.1.5/network_config/optimism/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-17 23:26:52.912798 rubi-2.1.5/network_config/optimism/abis/router.json
+-rw-r--r--   0        0        0      858 2023-07-17 23:26:52.912798 rubi-2.1.5/network_config/optimism/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-17 23:26:52.912798 rubi-2.1.5/network_config/optimism_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-17 23:26:52.912798 rubi-2.1.5/network_config/optimism_goerli/abis/router.json
+-rw-r--r--   0        0        0      760 2023-07-17 23:26:52.912798 rubi-2.1.5/network_config/optimism_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-17 23:26:52.912798 rubi-2.1.5/network_config/polygon_mumbai/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-17 23:26:52.912798 rubi-2.1.5/network_config/polygon_mumbai/abis/router.json
+-rw-r--r--   0        0        0      832 2023-07-17 23:26:52.912798 rubi-2.1.5/network_config/polygon_mumbai/network.yaml
+-rw-r--r--   0        0        0     1746 2023-07-17 23:27:19.977023 rubi-2.1.5/pyproject.toml
+-rw-r--r--   0        0        0      124 2023-07-17 23:26:52.912798 rubi-2.1.5/rubi/__init__.py
+-rw-r--r--   0        0        0    29209 2023-07-17 23:26:52.912798 rubi-2.1.5/rubi/client.py
+-rw-r--r--   0        0        0      163 2023-07-17 23:26:52.912798 rubi-2.1.5/rubi/contracts/__init__.py
+-rw-r--r--   0        0        0    65755 2023-07-17 23:26:52.912798 rubi-2.1.5/rubi/contracts/aid.py
+-rw-r--r--   0        0        0    12261 2023-07-17 23:26:52.912798 rubi-2.1.5/rubi/contracts/base_contract.py
+-rw-r--r--   0        0        0       74 2023-07-17 23:26:52.912798 rubi-2.1.5/rubi/contracts/contract_types/__init__.py
+-rw-r--r--   0        0        0    15898 2023-07-17 23:26:52.912798 rubi-2.1.5/rubi/contracts/contract_types/events.py
+-rw-r--r--   0        0        0     2805 2023-07-17 23:26:52.912798 rubi-2.1.5/rubi/contracts/contract_types/transaction_reciept.py
+-rw-r--r--   0        0        0    18565 2023-07-17 23:26:52.916798 rubi-2.1.5/rubi/contracts/erc20.py
+-rw-r--r--   0        0        0    24878 2023-07-17 23:26:52.916798 rubi-2.1.5/rubi/contracts/market.py
+-rw-r--r--   0        0        0    14915 2023-07-17 23:26:52.916798 rubi-2.1.5/rubi/contracts/router.py
+-rw-r--r--   0        0        0       77 2023-07-17 23:26:52.916798 rubi-2.1.5/rubi/data/README.md
+-rw-r--r--   0        0        0       31 2023-07-17 23:26:52.916798 rubi-2.1.5/rubi/data/__init__.py
+-rw-r--r--   0        0        0    10670 2023-07-17 23:26:52.916798 rubi-2.1.5/rubi/data/market.py
+-rw-r--r--   0        0        0       72 2023-07-17 23:26:52.916798 rubi-2.1.5/rubi/network/__init__.py
+-rw-r--r--   0        0        0     8450 2023-07-17 23:26:52.916798 rubi-2.1.5/rubi/network/network.py
+-rw-r--r--   0        0        0       94 2023-07-17 23:26:52.916798 rubi-2.1.5/rubi/rubicon_types/__init__.py
+-rw-r--r--   0        0        0    15796 2023-07-17 23:26:52.916798 rubi-2.1.5/rubi/rubicon_types/order.py
+-rw-r--r--   0        0        0    11554 2023-07-17 23:26:52.916798 rubi-2.1.5/rubi/rubicon_types/order_query.py
+-rw-r--r--   0        0        0     6323 2023-07-17 23:26:52.916798 rubi-2.1.5/rubi/rubicon_types/orderbook.py
+-rw-r--r--   0        0        0     2779 2023-07-17 23:26:52.916798 rubi-2.1.5/rubi/rubicon_types/pair.py
+-rw-r--r--   0        0        0     3635 1970-01-01 00:00:00.000000 rubi-2.1.5/PKG-INFO
```

### Comparing `rubi-2.1.4/LICENSE` & `rubi-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rubi-2.1.4/README.md` & `rubi-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.1.4/network_config/ERC20.json` & `rubi-2.1.5/network_config/ERC20.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.4/network_config/README.md` & `rubi-2.1.5/network_config/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.1.4/network_config/abitrum_goerli/abis/market.json` & `rubi-2.1.5/network_config/abitrum_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.4/network_config/abitrum_goerli/abis/router.json` & `rubi-2.1.5/network_config/abitrum_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.4/network_config/abitrum_goerli/network.yaml` & `rubi-2.1.5/network_config/abitrum_goerli/network.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 name: "Arbitrum Goerli"
 chain_id: 421613
 currency: "ETH"
 rpc_url: "https://goerli-rollup.arbitrum.io/rpc"
 explorer_url: "https://goerli-rollup-explorer.arbitrum.io"
 market_data_url: "https://api.rubicon.finance/subgraphs/name/RubiconV2_Arbitrum_Goerli"
+market_data_fallback_url: "https://api.thegraph.com/subgraphs/name/denverbaumgartner/rubiconv2-arbitrum-goerli"
 
 rubicon:
  market:
   address: "0x506407f25B746C39807c03A96DD595a6BE223211"
  router:
   address: "0x3AbA34a8C9616eA927225C045EEa5d5b51a7a6FC"
```

### Comparing `rubi-2.1.4/network_config/optimism/abis/market.json` & `rubi-2.1.5/network_config/optimism/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.4/network_config/optimism/abis/router.json` & `rubi-2.1.5/network_config/optimism/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.4/network_config/optimism/network.yaml` & `rubi-2.1.5/network_config/optimism/network.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 name: "Optimism"
 chain_id: 10
 currency: "ETH"
 rpc_url: "https://mainnet.optimism.io"
 explorer_url: "https://optimistic.etherscan.io/"
 market_data_url: "https://api.rubicon.finance/subgraphs/name/RubiconV2_Optimism_Mainnet_Dev"
+market_data_fallback_url: "https://api.thegraph.com/subgraphs/name/denverbaumgartner/rubiconv2-optimism-mainnet"
 
 rubicon:
  market:
   address: "0x7a512d3609211e719737e82c7bb7271ec05da70d"
  router:
   address: "0x7Af14ADc8Aea70f063c7eA3B2C1AD0D7A59C4bFf"
```

### Comparing `rubi-2.1.4/network_config/optimism_goerli/abis/market.json` & `rubi-2.1.5/network_config/optimism_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.4/network_config/optimism_goerli/abis/router.json` & `rubi-2.1.5/network_config/optimism_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.4/network_config/optimism_goerli/network.yaml` & `rubi-2.1.5/network_config/optimism_goerli/network.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 name: "Optimism Goerli"
 chain_id: 420
 currency: "ETH"
 rpc_url: "https://goerli.optimism.io"
 explorer_url: "https://goerli-explorer.optimism.io/"
 market_data_url: "https://api.rubicon.finance/subgraphs/name/RubiconV2_Optimism_Goerli"
+market_data_fallback_url: "https://api.thegraph.com/subgraphs/name/denverbaumgartner/rubiconv2-optimism-goerli"
 
 rubicon:
  market:
   address: "0x9d0D6c259566d8161a1b2c513af0463992db38bc"
  router:
   address: "0x0a0795d7015aB52BcDd987975474bD73062B5494"
```

### Comparing `rubi-2.1.4/network_config/polygon_mumbai/abis/market.json` & `rubi-2.1.5/network_config/polygon_mumbai/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.4/network_config/polygon_mumbai/abis/router.json` & `rubi-2.1.5/network_config/polygon_mumbai/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.4/network_config/polygon_mumbai/network.yaml` & `rubi-2.1.5/network_config/polygon_mumbai/network.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 name: "Polygon Mumbai"
 chain_id: 80001
 currency: "MATIC"
 rpc_url: "https://rpc-mumbai.maticvigil.com/"
 explorer_url: "https://mumbai.polygonscan.com/"
 market_data_url: "https://api.thegraph.com/subgraphs/name/denverbaumgartner/rubiconv2-polygon-mumbai"
+market_data_fallback_url: "https://api.thegraph.com/subgraphs/name/denverbaumgartner/rubiconv2-polygon-mumbai"
 
 rubicon:
  market:
   address: "0x10418D9e730fa659b0Baf0b640ee41FcF4EA2aaE"
  router:
   address: "0xbA81dF0251A017C2fB687e5469a897529442f008"
```

### Comparing `rubi-2.1.4/pyproject.toml` & `rubi-2.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rubi"
-version = "2.1.4"
+version = "2.1.5"
 description = "A python SDK for the Rubicon Protocol"
 authors = ["denver <denver@rubicon.finance>", "adam <adam@rubicon.finance>"]
 readme = "README.md"
 include = ["network_config/**/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `rubi-2.1.4/rubi/client.py` & `rubi-2.1.5/rubi/client.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.4/rubi/contracts/aid.py` & `rubi-2.1.5/rubi/contracts/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.4/rubi/contracts/base_contract.py` & `rubi-2.1.5/rubi/contracts/base_contract.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.4/rubi/contracts/contract_types/events.py` & `rubi-2.1.5/rubi/contracts/contract_types/events.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.4/rubi/contracts/contract_types/transaction_reciept.py` & `rubi-2.1.5/rubi/contracts/contract_types/transaction_reciept.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.4/rubi/contracts/erc20.py` & `rubi-2.1.5/rubi/contracts/erc20.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.4/rubi/contracts/market.py` & `rubi-2.1.5/rubi/contracts/market.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.4/rubi/contracts/router.py` & `rubi-2.1.5/rubi/contracts/router.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.4/rubi/data/market.py` & `rubi-2.1.5/rubi/data/market.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,44 +29,56 @@
     :type network: Network
     """
 
     def __init__(
         self,
         subgrounds: Subgrounds,
         subgraph_url: str,
+        subgraph_fallback_url: str,
         network: Optional[Network] = None,
         network_tokens: Optional[Dict[ChecksumAddress, ERC20]] = None,
     ):
         """constructor method"""
         self.sg = subgrounds
         self.subgraph_url = subgraph_url
+        self.subgraph_fallback_url = subgraph_fallback_url
         self.network = network  # type: Network | None
         self.tokens = network_tokens  # type: Dict[ChecksumAddress, ERC20] | None
 
         # initialize the subgraph
-        try:
-            self.data = self.sg.load_subgraph(self.subgraph_url)
-            # TODO: we should add a check here to guarantee the schema matches what we expect to be receiving
-        except:
-            # TODO: not sure exactly what error we should be throwing here, this is if the url does not work
-            raise ValueError(
-                f"subgraph_url: {subgraph_url} failed when attempting to load."
-            )
+        for attempt in range(3):
+            try:
+                self.data = self.sg.load_subgraph(
+                    self.subgraph_url
+                )  # TODO: we should add a check here to guarantee the schema matches what we expect to be receiving
+                break
+            except Exception as e:
+                if attempt < 2:
+                    continue
+                else:
+                    try:
+                        self.data = self.sg.load_subgraph(self.subgraph_fallback_url)
+                        break
+                    except:
+                        raise ValueError(
+                            f"Both subgraph_url: {self.subgraph_url} and fallback_url: {self.subgraph_fallback_url} failed when attempting to load. Error: {str(e)}"
+                        )
 
         # Initialize the query classes
         self.offer_query = OrderQuery(self.sg, self.data, self.network, self.tokens)
 
     @classmethod
     def from_network_with_tokens(
         cls, network: Network, network_tokens: Dict[ChecksumAddress, ERC20]
     ) -> "MarketData":
         """Initialize a MarketData object using a Network object."""
         return cls(
             subgrounds=network.subgrounds,
             subgraph_url=network.market_data_url,
+            subgraph_fallback_url=network.market_data_fallback_url,
             network=network,
             network_tokens=network_tokens,
         )
 
     #####################################
     # Subgraph Query Methods            #
     #####################################
```

### Comparing `rubi-2.1.4/rubi/network/network.py` & `rubi-2.1.5/rubi/network/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         # The below all come from network_config/{network_name}/network.yaml
         name: str,
         chain_id: int,
         currency: str,
         rpc_url: str,
         explorer_url: str,
         market_data_url: str,
+        market_data_fallback_url: str,
         rubicon: dict,
         token_addresses: dict,
         # optional custom token config file from the user
         custom_token_addresses_file: Optional[str] = None,
     ):
         """Initializes a Network instance.
 
@@ -74,14 +75,15 @@
 
         self.currency = currency
         self.rpc_url = rpc_url
         self.explorer_url = explorer_url
         # TODO: currently we are utilizing just a single url, we should switch to a dictionary as the number of
         #  subgraphs we support grows
         self.market_data_url = market_data_url
+        self.market_data_fallback_url = market_data_fallback_url
         self.rubicon = RubiconContracts(path=path, w3=self.w3, **rubicon)
 
         checksummed_token_addresses: dict[str, ChecksumAddress] = {}
         for k, v in token_addresses.items():
             checksummed_token_addresses[k] = self.w3.to_checksum_address(v)
 
         if custom_token_addresses_file:
```

### Comparing `rubi-2.1.4/rubi/rubicon_types/order.py` & `rubi-2.1.5/rubi/rubicon_types/order.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.4/rubi/rubicon_types/order_query.py` & `rubi-2.1.5/rubi/rubicon_types/order_query.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.4/rubi/rubicon_types/orderbook.py` & `rubi-2.1.5/rubi/rubicon_types/orderbook.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.4/rubi/rubicon_types/pair.py` & `rubi-2.1.5/rubi/rubicon_types/pair.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.4/PKG-INFO` & `rubi-2.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubi
-Version: 2.1.4
+Version: 2.1.5
 Summary: A python SDK for the Rubicon Protocol
 Author: denver
 Author-email: denver@rubicon.finance
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

