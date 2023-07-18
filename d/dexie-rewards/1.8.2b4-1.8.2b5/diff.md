# Comparing `tmp/dexie_rewards-1.8.2b4.tar.gz` & `tmp/dexie_rewards-1.8.2b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexie_rewards-1.8.2b4.tar", max compression
+gzip compressed data, was "dexie_rewards-1.8.2b5.tar", max compression
```

## Comparing `dexie_rewards-1.8.2b4.tar` & `dexie_rewards-1.8.2b5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-05-02 08:44:23.355168 dexie_rewards-1.8.2b4/LICENSE
--rw-r--r--   0        0        0     5817 2023-06-30 14:39:04.284007 dexie_rewards-1.8.2b4/README.md
--rw-r--r--   0        0        0      864 2023-07-04 02:27:59.235171 dexie_rewards-1.8.2b4/pyproject.toml
--rw-r--r--   0        0        0      219 2023-05-04 04:23:21.607369 dexie_rewards-1.8.2b4/src/dexie_rewards/__init__.py
--rw-r--r--   0        0        0     1125 2023-06-30 04:40:39.340510 dexie_rewards-1.8.2b4/src/dexie_rewards/config.py
--rw-r--r--   0        0        0      822 2023-05-12 12:18:23.796037 dexie_rewards-1.8.2b4/src/dexie_rewards/decorators/with_db_connection.py
--rw-r--r--   0        0        0     1169 2023-06-10 08:56:40.443038 dexie_rewards-1.8.2b4/src/dexie_rewards/decorators/with_wallet_rpc_client.py
--rw-r--r--   0        0        0      234 2023-05-08 10:51:08.009870 dexie_rewards-1.8.2b4/src/dexie_rewards/main.py
--rw-r--r--   0        0        0     5013 2023-06-30 09:40:10.161232 dexie_rewards-1.8.2b4/src/dexie_rewards/rewards/claim.py
--rw-r--r--   0        0        0     1921 2023-05-13 03:55:02.188725 dexie_rewards-1.8.2b4/src/dexie_rewards/rewards/list.py
--rw-r--r--   0        0        0      272 2023-05-08 10:18:31.545940 dexie_rewards-1.8.2b4/src/dexie_rewards/rewards/main.py
--rw-r--r--   0        0        0     5159 2023-06-30 09:37:14.115364 dexie_rewards-1.8.2b4/src/dexie_rewards/rewards/utils.py
--rw-r--r--   0        0        0     2294 2023-05-19 15:21:53.341294 dexie_rewards-1.8.2b4/src/dexie_rewards/services/dexie_api.py
--rw-r--r--   0        0        0     3756 2023-05-13 03:51:52.828154 dexie_rewards-1.8.2b4/src/dexie_rewards/services/dexie_db.py
--rw-r--r--   0        0        0     1792 2023-06-11 05:27:12.034750 dexie_rewards-1.8.2b4/src/dexie_rewards/services/wallet_rpc_client.py
--rw-r--r--   0        0        0     1124 2023-06-30 04:32:23.576365 dexie_rewards-1.8.2b4/src/dexie_rewards/types/offer_reward.py
--rw-r--r--   0        0        0      229 2023-05-09 11:06:14.984159 dexie_rewards-1.8.2b4/src/dexie_rewards/types/utils.py
--rw-r--r--   0        0        0     1863 2023-06-10 08:56:40.444913 dexie_rewards-1.8.2b4/src/dexie_rewards/utils.py
--rw-r--r--   0        0        0     6653 1970-01-01 00:00:00.000000 dexie_rewards-1.8.2b4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-30 14:18:44.184005 dexie_rewards-1.8.2b5/LICENSE
+-rw-r--r--   0        0        0     5817 2023-06-30 14:39:04.000000 dexie_rewards-1.8.2b5/README.md
+-rw-r--r--   0        0        0      864 2023-07-18 09:10:09.127037 dexie_rewards-1.8.2b5/pyproject.toml
+-rw-r--r--   0        0        0      219 2023-05-04 04:23:21.000000 dexie_rewards-1.8.2b5/src/dexie_rewards/__init__.py
+-rw-r--r--   0        0        0     1125 2023-06-30 04:40:39.000000 dexie_rewards-1.8.2b5/src/dexie_rewards/config.py
+-rw-r--r--   0        0        0      822 2023-05-12 12:18:23.000000 dexie_rewards-1.8.2b5/src/dexie_rewards/decorators/with_db_connection.py
+-rw-r--r--   0        0        0     1169 2023-06-10 08:56:40.000000 dexie_rewards-1.8.2b5/src/dexie_rewards/decorators/with_wallet_rpc_client.py
+-rw-r--r--   0        0        0      234 2023-05-08 10:51:08.000000 dexie_rewards-1.8.2b5/src/dexie_rewards/main.py
+-rw-r--r--   0        0        0     5013 2023-06-30 09:40:10.000000 dexie_rewards-1.8.2b5/src/dexie_rewards/rewards/claim.py
+-rw-r--r--   0        0        0     1921 2023-05-13 03:55:02.000000 dexie_rewards-1.8.2b5/src/dexie_rewards/rewards/list.py
+-rw-r--r--   0        0        0      272 2023-05-08 10:18:31.000000 dexie_rewards-1.8.2b5/src/dexie_rewards/rewards/main.py
+-rw-r--r--   0        0        0     5159 2023-06-30 09:37:14.000000 dexie_rewards-1.8.2b5/src/dexie_rewards/rewards/utils.py
+-rw-r--r--   0        0        0     2294 2023-05-19 15:21:53.000000 dexie_rewards-1.8.2b5/src/dexie_rewards/services/dexie_api.py
+-rw-r--r--   0        0        0     3756 2023-05-13 03:51:52.000000 dexie_rewards-1.8.2b5/src/dexie_rewards/services/dexie_db.py
+-rw-r--r--   0        0        0     1792 2023-06-11 05:27:12.000000 dexie_rewards-1.8.2b5/src/dexie_rewards/services/wallet_rpc_client.py
+-rw-r--r--   0        0        0     1124 2023-06-30 04:32:23.000000 dexie_rewards-1.8.2b5/src/dexie_rewards/types/offer_reward.py
+-rw-r--r--   0        0        0      229 2023-05-09 11:06:14.000000 dexie_rewards-1.8.2b5/src/dexie_rewards/types/utils.py
+-rw-r--r--   0        0        0     1863 2023-06-10 08:56:40.000000 dexie_rewards-1.8.2b5/src/dexie_rewards/utils.py
+-rw-r--r--   0        0        0     6653 1970-01-01 00:00:00.000000 dexie_rewards-1.8.2b5/PKG-INFO
```

### Comparing `dexie_rewards-1.8.2b4/LICENSE` & `dexie_rewards-1.8.2b5/LICENSE`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.2b4/README.md` & `dexie_rewards-1.8.2b5/README.md`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.2b4/pyproject.toml` & `dexie_rewards-1.8.2b5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dexie-rewards"
-version = "1.8.2-b4"
+version = "1.8.2-b5"
 description = "dexie-rewards is a Python CLI helper tool designed automatically to claim dexie liquidity rewards for offers created using the official Chia Wallet."
 authors = ["Dexie Contributors <pypi@dexie.space>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "dexie_rewards", from = "src" }]
 
 [tool.poetry.dependencies]
```

### Comparing `dexie_rewards-1.8.2b4/src/dexie_rewards/config.py` & `dexie_rewards-1.8.2b5/src/dexie_rewards/config.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.2b4/src/dexie_rewards/decorators/with_db_connection.py` & `dexie_rewards-1.8.2b5/src/dexie_rewards/decorators/with_db_connection.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.2b4/src/dexie_rewards/decorators/with_wallet_rpc_client.py` & `dexie_rewards-1.8.2b5/src/dexie_rewards/decorators/with_wallet_rpc_client.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.2b4/src/dexie_rewards/rewards/claim.py` & `dexie_rewards-1.8.2b5/src/dexie_rewards/rewards/claim.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.2b4/src/dexie_rewards/rewards/list.py` & `dexie_rewards-1.8.2b5/src/dexie_rewards/rewards/list.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.2b4/src/dexie_rewards/rewards/utils.py` & `dexie_rewards-1.8.2b5/src/dexie_rewards/rewards/utils.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.2b4/src/dexie_rewards/services/dexie_api.py` & `dexie_rewards-1.8.2b5/src/dexie_rewards/services/dexie_api.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.2b4/src/dexie_rewards/services/dexie_db.py` & `dexie_rewards-1.8.2b5/src/dexie_rewards/services/dexie_db.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.2b4/src/dexie_rewards/services/wallet_rpc_client.py` & `dexie_rewards-1.8.2b5/src/dexie_rewards/services/wallet_rpc_client.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.2b4/src/dexie_rewards/types/offer_reward.py` & `dexie_rewards-1.8.2b5/src/dexie_rewards/types/offer_reward.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.2b4/src/dexie_rewards/utils.py` & `dexie_rewards-1.8.2b5/src/dexie_rewards/utils.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.2b4/PKG-INFO` & `dexie_rewards-1.8.2b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexie-rewards
-Version: 1.8.2b4
+Version: 1.8.2b5
 Summary: dexie-rewards is a Python CLI helper tool designed automatically to claim dexie liquidity rewards for offers created using the official Chia Wallet.
 License: Apache-2.0
 Author: Dexie Contributors
 Author-email: pypi@dexie.space
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

