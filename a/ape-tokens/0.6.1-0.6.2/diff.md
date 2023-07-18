# Comparing `tmp/ape-tokens-0.6.1.tar.gz` & `tmp/ape-tokens-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-tokens-0.6.1.tar", last modified: Tue Jun 13 13:41:10 2023, max compression
+gzip compressed data, was "ape-tokens-0.6.2.tar", last modified: Tue Jul 18 20:03:29 2023, max compression
```

## Comparing `ape-tokens-0.6.1.tar` & `ape-tokens-0.6.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:41:10.818383 ape-tokens-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:41:10.814383 ape-tokens-0.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:41:10.814383 ape-tokens-0.6.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:41:10.814383 ape-tokens-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/.github/workflows/commit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-13 13:41:10.818383 ape-tokens-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:41:10.814383 ape-tokens-0.6.1/ape_tokens/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/ape_tokens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/ape_tokens/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/ape_tokens/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/ape_tokens/managers.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 13:41:10.000000 ape-tokens-0.6.1/ape_tokens/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:41:10.818383 ape-tokens-0.6.1/ape_tokens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-13 13:41:10.000000 ape-tokens-0.6.1/ape_tokens.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-13 13:41:10.000000 ape-tokens-0.6.1/ape_tokens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:41:10.000000 ape-tokens-0.6.1/ape_tokens.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 13:41:10.000000 ape-tokens-0.6.1/ape_tokens.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:41:10.000000 ape-tokens-0.6.1/ape_tokens.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-13 13:41:10.000000 ape-tokens-0.6.1/ape_tokens.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 13:41:10.000000 ape-tokens-0.6.1/ape_tokens.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-13 13:41:10.818383 ape-tokens-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:41:10.818383 ape-tokens-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:29.135065 ape-tokens-0.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:29.131065 ape-tokens-0.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:29.131065 ape-tokens-0.6.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-18 20:02:14.000000 ape-tokens-0.6.2/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-18 20:02:14.000000 ape-tokens-0.6.2/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-18 20:02:14.000000 ape-tokens-0.6.2/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-18 20:02:14.000000 ape-tokens-0.6.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-18 20:02:14.000000 ape-tokens-0.6.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:29.131065 ape-tokens-0.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-18 20:02:14.000000 ape-tokens-0.6.2/.github/workflows/commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-18 20:02:14.000000 ape-tokens-0.6.2/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-18 20:02:14.000000 ape-tokens-0.6.2/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-18 20:02:14.000000 ape-tokens-0.6.2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-18 20:02:14.000000 ape-tokens-0.6.2/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-18 20:02:14.000000 ape-tokens-0.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 20:02:14.000000 ape-tokens-0.6.2/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-18 20:02:14.000000 ape-tokens-0.6.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-07-18 20:02:14.000000 ape-tokens-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-18 20:03:29.135065 ape-tokens-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-18 20:02:14.000000 ape-tokens-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:29.131065 ape-tokens-0.6.2/ape_tokens/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-18 20:02:14.000000 ape-tokens-0.6.2/ape_tokens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-18 20:02:14.000000 ape-tokens-0.6.2/ape_tokens/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-18 20:02:14.000000 ape-tokens-0.6.2/ape_tokens/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-07-18 20:02:14.000000 ape-tokens-0.6.2/ape_tokens/managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-18 20:03:28.000000 ape-tokens-0.6.2/ape_tokens/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:29.131065 ape-tokens-0.6.2/ape_tokens.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-18 20:03:29.000000 ape-tokens-0.6.2/ape_tokens.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-18 20:03:29.000000 ape-tokens-0.6.2/ape_tokens.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 20:03:29.000000 ape-tokens-0.6.2/ape_tokens.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-18 20:03:29.000000 ape-tokens-0.6.2/ape_tokens.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 20:03:29.000000 ape-tokens-0.6.2/ape_tokens.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-18 20:03:29.000000 ape-tokens-0.6.2/ape_tokens.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-18 20:03:29.000000 ape-tokens-0.6.2/ape_tokens.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-18 20:02:14.000000 ape-tokens-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-18 20:03:29.135065 ape-tokens-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-07-18 20:02:14.000000 ape-tokens-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:29.135065 ape-tokens-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:02:14.000000 ape-tokens-0.6.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-18 20:02:14.000000 ape-tokens-0.6.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-18 20:02:14.000000 ape-tokens-0.6.2/tests/test_integration.py
```

### Comparing `ape-tokens-0.6.1/.github/ISSUE_TEMPLATE/bug.md` & `ape-tokens-0.6.2/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.6.1/.github/ISSUE_TEMPLATE/feature.md` & `ape-tokens-0.6.2/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.6.1/.github/ISSUE_TEMPLATE/work-item.md` & `ape-tokens-0.6.2/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.6.1/.github/release-drafter.yml` & `ape-tokens-0.6.2/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.6.1/.github/workflows/commit.yaml` & `ape-tokens-0.6.2/.github/workflows/commit.yaml`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.6.1/.github/workflows/prtitle.yaml` & `ape-tokens-0.6.2/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.6.1/.github/workflows/publish.yaml` & `ape-tokens-0.6.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.6.1/.github/workflows/test.yaml` & `ape-tokens-0.6.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.6.1/.gitignore` & `ape-tokens-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.6.1/.pre-commit-config.yaml` & `ape-tokens-0.6.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.6.1/LICENSE` & `ape-tokens-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.6.1/PKG-INFO` & `ape-tokens-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-tokens
-Version: 0.6.1
+Version: 0.6.2
 Summary: ape-tokens: tokenlists plugin for Ape
 Home-page: https://github.com/ApeWorX/ape-tokens
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ape-tokens-0.6.1/README.md` & `ape-tokens-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.6.1/ape_tokens/converters.py` & `ape-tokens-0.6.2/ape_tokens/converters.py`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.6.1/ape_tokens/managers.py` & `ape-tokens-0.6.2/ape_tokens/managers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from ape.api import Address
+from ape.contracts import ContractInstance
 from ape.types import ContractType
-from ape.utils import cached_property
+from ape.utils import ManagerAccessMixin, cached_property
 from eth_utils import to_checksum_address
 from tokenlists import TokenListManager
 
 ERC20 = ContractType(
     **{
         "contractName": "ERC20",
         "abi": [
@@ -101,26 +101,30 @@
                 ],
             },
         ],
     }
 )
 
 
-class TokenManager(dict):
+class TokenManager(ManagerAccessMixin, dict):
     @cached_property
     def _manager(self) -> TokenListManager:
         return TokenListManager()
 
     @cached_property
     def _Contract(self):
         from ape import Contract
 
         return Contract
 
-    def __getitem__(self, symbol: str) -> Address:
+    def __getitem__(self, symbol: str) -> ContractInstance:
         try:
-            token_info = self._manager.get_token_info(symbol)
+            token_info = self._manager.get_token_info(
+                symbol, chain_id=self.network_manager.network.chain_id
+            )
 
         except ValueError as e:
             raise KeyError(f"Symbol '{symbol}' is not a known token symbol") from e
 
-        return self._Contract(to_checksum_address(token_info.address), contract_type=ERC20)
+        return self.chain_manager.contracts.instance_at(
+            to_checksum_address(token_info.address), contract_type=ERC20
+        )
```

### Comparing `ape-tokens-0.6.1/ape_tokens.egg-info/PKG-INFO` & `ape-tokens-0.6.2/ape_tokens.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-tokens
-Version: 0.6.1
+Version: 0.6.2
 Summary: ape-tokens: tokenlists plugin for Ape
 Home-page: https://github.com/ApeWorX/ape-tokens
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ape-tokens-0.6.1/ape_tokens.egg-info/SOURCES.txt` & `ape-tokens-0.6.2/ape_tokens.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.6.1/ape_tokens.egg-info/requires.txt` & `ape-tokens-0.6.2/ape_tokens.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.6.1/pyproject.toml` & `ape-tokens-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.6.1/setup.py` & `ape-tokens-0.6.2/setup.py`

 * *Files identical despite different names*

