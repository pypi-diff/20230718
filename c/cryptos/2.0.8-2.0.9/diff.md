# Comparing `tmp/cryptos-2.0.8.tar.gz` & `tmp/cryptos-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptos-2.0.8.tar", last modified: Tue May 23 16:19:10 2023, max compression
+gzip compressed data, was "cryptos-2.0.9.tar", last modified: Tue Jul 18 14:56:40 2023, max compression
```

## Comparing `cryptos-2.0.8.tar` & `cryptos-2.0.9.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 16:19:10.468214 cryptos-2.0.8/
--rw-rw-rw-   0        0        0     1293 2022-10-03 10:19:24.000000 cryptos-2.0.8/LICENSE
--rw-rw-rw-   0        0        0      112 2023-05-05 12:53:53.000000 cryptos-2.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0    41635 2023-05-23 16:19:10.468214 cryptos-2.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    40920 2023-05-23 16:18:56.000000 cryptos-2.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 16:19:10.256192 cryptos-2.0.8/crypto_scripts/
--rw-rw-rw-   0        0        0        0 2023-03-22 18:26:27.000000 cryptos-2.0.8/crypto_scripts/__init__.py
--rw-rw-rw-   0        0        0      889 2023-03-22 18:26:27.000000 cryptos-2.0.8/crypto_scripts/broadcast.py
--rw-rw-rw-   0        0        0     1888 2023-05-23 16:18:56.000000 cryptos-2.0.8/crypto_scripts/convert_private_key.py
--rw-rw-rw-   0        0        0     1472 2023-03-22 18:26:27.000000 cryptos-2.0.8/crypto_scripts/create_private_key.py
--rw-rw-rw-   0        0        0     2987 2023-03-22 18:26:27.000000 cryptos-2.0.8/crypto_scripts/cryptosend.py
--rw-rw-rw-   0        0        0     8914 2023-05-23 16:18:56.000000 cryptos-2.0.8/crypto_scripts/explorer.py
--rw-rw-rw-   0        0        0     1088 2023-03-22 18:26:27.000000 cryptos-2.0.8/crypto_scripts/get_block_sizes.py
--rw-rw-rw-   0        0        0     3471 2023-03-22 18:26:27.000000 cryptos-2.0.8/crypto_scripts/subscribe.py
--rw-rw-rw-   0        0        0     3631 2023-05-23 16:18:56.000000 cryptos-2.0.8/crypto_scripts/view_private_key_addresses.py
-drwxrwxrwx   0        0        0        0 2023-05-23 16:19:10.299362 cryptos-2.0.8/cryptos/
--rw-rw-rw-   0        0        0      275 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/__init__.py
--rw-rw-rw-   0        0        0     3131 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/blocks.py
--rw-rw-rw-   0        0        0     6798 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/cashaddr.py
-drwxrwxrwx   0        0        0        0 2023-05-23 16:19:10.324510 cryptos-2.0.8/cryptos/coins/
--rw-rw-rw-   0        0        0      153 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/coins/__init__.py
--rw-rw-rw-   0        0        0    18357 2023-05-23 16:18:56.000000 cryptos-2.0.8/cryptos/coins/base.py
--rw-rw-rw-   0        0        0      162 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/coins/bitcoin.py
--rw-rw-rw-   0        0        0      183 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/coins/bitcoin_cash.py
--rw-rw-rw-   0        0        0      147 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/coins/dash.py
--rw-rw-rw-   0        0        0      151 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/coins/dogecoin.py
--rw-rw-rw-   0        0        0      167 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/coins/litecoin.py
-drwxrwxrwx   0        0        0        0 2023-05-23 16:19:10.340786 cryptos-2.0.8/cryptos/coins_async/
--rw-rw-rw-   0        0        0      124 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/coins_async/__init__.py
--rw-rw-rw-   0        0        0    50144 2023-05-23 16:18:56.000000 cryptos-2.0.8/cryptos/coins_async/base.py
--rw-rw-rw-   0        0        0     1252 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/coins_async/bitcoin.py
--rw-rw-rw-   0        0        0     1352 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/coins_async/bitcoin_cash.py
--rw-rw-rw-   0        0        0      746 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/coins_async/dash.py
--rw-rw-rw-   0        0        0      931 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/coins_async/dogecoin.py
--rw-rw-rw-   0        0        0      976 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/coins_async/litecoin.py
--rw-rw-rw-   0        0        0     1657 2022-10-03 10:19:24.000000 cryptos-2.0.8/cryptos/composite.py
--rw-rw-rw-   0        0        0      402 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/constants.py
--rw-rw-rw-   0        0        0     8911 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/deterministic.py
-drwxrwxrwx   0        0        0        0 2023-05-23 16:19:10.340786 cryptos-2.0.8/cryptos/electrumx_client/
--rw-rw-rw-   0        0        0       37 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/electrumx_client/__init__.py
--rw-rw-rw-   0        0        0    22725 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/electrumx_client/client.py
-drwxrwxrwx   0        0        0        0 2023-05-23 16:19:10.356047 cryptos-2.0.8/cryptos/electrumx_client/servers/
--rw-rw-rw-   0        0        0    10969 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/electrumx_client/servers/bitcoin.json
--rw-rw-rw-   0        0        0     3618 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/electrumx_client/servers/bitcoin_cash.json
--rw-rw-rw-   0        0        0     1093 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/electrumx_client/servers/bitcoin_cash_testnet.json
--rw-rw-rw-   0        0        0      936 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/electrumx_client/servers/bitcoin_testnet.json
--rw-rw-rw-   0        0        0      384 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/electrumx_client/servers/dash.json
--rw-rw-rw-   0        0        0      486 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/electrumx_client/servers/dash_testnet.json
--rw-rw-rw-   0        0        0      254 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/electrumx_client/servers/doge.json
--rw-rw-rw-   0        0        0      254 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/electrumx_client/servers/doge_testnet.json
--rw-rw-rw-   0        0        0      973 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/electrumx_client/servers/litecoin.json
--rw-rw-rw-   0        0        0      283 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/electrumx_client/servers/litecoin_testnet.json
--rw-rw-rw-   0        0        0      257 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/electrumx_client/servers/testing.json
--rw-rw-rw-   0        0        0     2400 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/electrumx_client/types.py
--rw-rw-rw-   0        0        0    15164 2022-10-03 10:19:24.000000 cryptos-2.0.8/cryptos/english.txt
-drwxrwxrwx   0        0        0        0 2023-05-23 16:19:10.368055 cryptos-2.0.8/cryptos/explorers/
--rw-rw-rw-   0        0        0      644 2022-10-03 10:19:24.000000 cryptos-2.0.8/cryptos/explorers/__init__.py
--rw-rw-rw-   0        0        0     3268 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/explorers/base_insight.py
--rw-rw-rw-   0        0        0      338 2022-10-03 10:19:24.000000 cryptos-2.0.8/cryptos/explorers/bitpay.py
--rw-rw-rw-   0        0        0     4045 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/explorers/blockchain.py
--rw-rw-rw-   0        0        0     1074 2022-10-03 10:19:24.000000 cryptos-2.0.8/cryptos/explorers/blockcypher.py
--rw-rw-rw-   0        0        0     1280 2022-10-03 10:19:24.000000 cryptos-2.0.8/cryptos/explorers/blockdozer.py
--rw-rw-rw-   0        0        0     1264 2022-10-03 10:19:24.000000 cryptos-2.0.8/cryptos/explorers/btg_explorer.py
--rw-rw-rw-   0        0        0     1242 2022-10-03 10:19:24.000000 cryptos-2.0.8/cryptos/explorers/dash_siampm.py
--rw-rw-rw-   0        0        0     3047 2022-10-03 10:19:24.000000 cryptos-2.0.8/cryptos/explorers/sochain.py
--rw-rw-rw-   0        0        0      559 2022-10-03 10:19:24.000000 cryptos-2.0.8/cryptos/explorers/utils.py
--rw-rw-rw-   0        0        0    18584 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/keystore.py
--rw-rw-rw-   0        0        0    19302 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/main.py
--rw-rw-rw-   0        0        0     8436 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/mnemonic.py
--rw-rw-rw-   0        0        0     2838 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/opcodes.py
--rw-rw-rw-   0        0        0     3494 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/py3specials.py
--rw-rw-rw-   0        0        0    15159 2022-10-03 10:19:24.000000 cryptos-2.0.8/cryptos/ripemd.py
--rw-rw-rw-   0        0        0      364 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/script_utils.py
--rw-rw-rw-   0        0        0     6099 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/segwit_addr.py
--rw-rw-rw-   0        0        0     3777 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/stealth.py
-drwxrwxrwx   0        0        0        0 2023-05-23 16:19:10.385707 cryptos-2.0.8/cryptos/testing/
--rw-rw-rw-   0        0        0        0 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/testing/__init__.py
--rw-rw-rw-   0        0        0    33904 2023-05-23 16:18:56.000000 cryptos-2.0.8/cryptos/testing/testcases.py
--rw-rw-rw-   0        0        0    56457 2023-05-23 16:18:56.000000 cryptos-2.0.8/cryptos/testing/testcases_async.py
--rw-rw-rw-   0        0        0    21694 2023-04-03 17:25:43.000000 cryptos-2.0.8/cryptos/transaction.py
--rw-rw-rw-   0        0        0     2414 2023-04-03 17:25:43.000000 cryptos-2.0.8/cryptos/types.py
--rw-rw-rw-   0        0        0     2040 2023-03-24 21:15:30.000000 cryptos-2.0.8/cryptos/utils.py
--rw-rw-rw-   0        0        0    12247 2023-05-23 16:18:56.000000 cryptos-2.0.8/cryptos/wallet.py
--rw-rw-rw-   0        0        0     6746 2023-03-22 13:46:57.000000 cryptos-2.0.8/cryptos/wallet_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-23 16:19:10.316905 cryptos-2.0.8/cryptos.egg-info/
--rw-rw-rw-   0        0        0    41635 2023-05-23 16:19:10.000000 cryptos-2.0.8/cryptos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3093 2023-05-23 16:19:10.000000 cryptos-2.0.8/cryptos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 16:19:10.000000 cryptos-2.0.8/cryptos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      438 2023-05-23 16:19:10.000000 cryptos-2.0.8/cryptos.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       80 2023-05-23 16:19:10.000000 cryptos-2.0.8/cryptos.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-05-23 16:19:10.000000 cryptos-2.0.8/cryptos.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 16:19:10.468214 cryptos-2.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1801 2023-05-23 16:18:56.000000 cryptos-2.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 16:19:10.401375 cryptos-2.0.8/tests/
--rw-rw-rw-   0        0        0        0 2023-03-22 13:46:57.000000 cryptos-2.0.8/tests/__init__.py
--rw-rw-rw-   0        0        0     5596 2023-03-22 13:46:57.000000 cryptos-2.0.8/tests/electrum_subscribe_mock_server.py
-drwxrwxrwx   0        0        0        0 2023-05-23 16:19:10.401375 cryptos-2.0.8/tests/test_coins/
--rw-rw-rw-   0        0        0        0 2023-03-22 13:46:57.000000 cryptos-2.0.8/tests/test_coins/__init__.py
--rw-rw-rw-   0        0        0    13157 2023-04-03 13:33:46.000000 cryptos-2.0.8/tests/test_coins/test_bitcoin_testnet.py
-drwxrwxrwx   0        0        0        0 2023-05-23 16:19:10.468214 cryptos-2.0.8/tests/test_coins_async/
--rw-rw-rw-   0        0        0        0 2023-03-22 13:46:57.000000 cryptos-2.0.8/tests/test_coins_async/__init__.py
--rw-rw-rw-   0        0        0    16130 2023-04-03 17:25:43.000000 cryptos-2.0.8/tests/test_coins_async/test_bitcoin.py
--rw-rw-rw-   0        0        0    11403 2023-03-24 22:06:15.000000 cryptos-2.0.8/tests/test_coins_async/test_bitcoin_cash.py
--rw-rw-rw-   0        0        0     8815 2023-03-22 13:46:57.000000 cryptos-2.0.8/tests/test_coins_async/test_bitcoin_cash_testnet.py
--rw-rw-rw-   0        0        0    10667 2023-04-03 12:02:39.000000 cryptos-2.0.8/tests/test_coins_async/test_bitcoin_testnet.py
--rw-rw-rw-   0        0        0     5932 2023-03-22 13:46:57.000000 cryptos-2.0.8/tests/test_coins_async/test_dash.py
--rw-rw-rw-   0        0        0     5829 2023-04-03 12:02:39.000000 cryptos-2.0.8/tests/test_coins_async/test_dash_testnet.py
--rw-rw-rw-   0        0        0     7355 2023-03-22 13:46:57.000000 cryptos-2.0.8/tests/test_coins_async/test_dogecoin.py
--rw-rw-rw-   0        0        0     5694 2023-03-22 13:46:57.000000 cryptos-2.0.8/tests/test_coins_async/test_dogecoin_testnet.py
--rw-rw-rw-   0        0        0    14402 2023-05-23 16:18:56.000000 cryptos-2.0.8/tests/test_coins_async/test_litecoin.py
--rw-rw-rw-   0        0        0     9245 2023-03-22 13:46:57.000000 cryptos-2.0.8/tests/test_coins_async/test_litecoin_testnet.py
--rw-rw-rw-   0        0        0    26157 2023-03-22 13:46:57.000000 cryptos-2.0.8/tests/test_electrum_client.py
--rw-rw-rw-   0        0        0    28702 2023-03-22 13:46:57.000000 cryptos-2.0.8/tests/test_general.py
--rw-rw-rw-   0        0        0     4366 2023-03-22 13:46:57.000000 cryptos-2.0.8/tests/test_stealth.py
--rw-rw-rw-   0        0        0    32352 2023-03-22 13:46:57.000000 cryptos-2.0.8/tests/test_wallet.py
+drwxrwxrwx   0        0        0        0 2023-07-18 14:56:40.794374 cryptos-2.0.9/
+-rw-rw-rw-   0        0        0     1293 2022-10-03 10:19:24.000000 cryptos-2.0.9/LICENSE
+-rw-rw-rw-   0        0        0      112 2023-05-05 12:53:53.000000 cryptos-2.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    41586 2023-07-18 14:56:40.794374 cryptos-2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    40920 2023-05-23 16:18:56.000000 cryptos-2.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 14:56:40.610196 cryptos-2.0.9/crypto_scripts/
+-rw-rw-rw-   0        0        0        0 2023-03-22 18:26:27.000000 cryptos-2.0.9/crypto_scripts/__init__.py
+-rw-rw-rw-   0        0        0      889 2023-03-22 18:26:27.000000 cryptos-2.0.9/crypto_scripts/broadcast.py
+-rw-rw-rw-   0        0        0     1888 2023-05-23 16:18:56.000000 cryptos-2.0.9/crypto_scripts/convert_private_key.py
+-rw-rw-rw-   0        0        0     1472 2023-03-22 18:26:27.000000 cryptos-2.0.9/crypto_scripts/create_private_key.py
+-rw-rw-rw-   0        0        0     2987 2023-03-22 18:26:27.000000 cryptos-2.0.9/crypto_scripts/cryptosend.py
+-rw-rw-rw-   0        0        0     8914 2023-05-23 16:18:56.000000 cryptos-2.0.9/crypto_scripts/explorer.py
+-rw-rw-rw-   0        0        0     1088 2023-03-22 18:26:27.000000 cryptos-2.0.9/crypto_scripts/get_block_sizes.py
+-rw-rw-rw-   0        0        0     3471 2023-03-22 18:26:27.000000 cryptos-2.0.9/crypto_scripts/subscribe.py
+-rw-rw-rw-   0        0        0     3631 2023-05-23 16:18:56.000000 cryptos-2.0.9/crypto_scripts/view_private_key_addresses.py
+drwxrwxrwx   0        0        0        0 2023-07-18 14:56:40.655923 cryptos-2.0.9/cryptos/
+-rw-rw-rw-   0        0        0      275 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/__init__.py
+-rw-rw-rw-   0        0        0     3131 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/blocks.py
+-rw-rw-rw-   0        0        0     6798 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/cashaddr.py
+drwxrwxrwx   0        0        0        0 2023-07-18 14:56:40.687955 cryptos-2.0.9/cryptos/coins/
+-rw-rw-rw-   0        0        0      153 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/coins/__init__.py
+-rw-rw-rw-   0        0        0    18357 2023-05-23 16:18:56.000000 cryptos-2.0.9/cryptos/coins/base.py
+-rw-rw-rw-   0        0        0      162 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/coins/bitcoin.py
+-rw-rw-rw-   0        0        0      183 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/coins/bitcoin_cash.py
+-rw-rw-rw-   0        0        0      147 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/coins/dash.py
+-rw-rw-rw-   0        0        0      151 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/coins/dogecoin.py
+-rw-rw-rw-   0        0        0      167 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/coins/litecoin.py
+drwxrwxrwx   0        0        0        0 2023-07-18 14:56:40.694086 cryptos-2.0.9/cryptos/coins_async/
+-rw-rw-rw-   0        0        0      124 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/coins_async/__init__.py
+-rw-rw-rw-   0        0        0    50144 2023-05-23 16:18:56.000000 cryptos-2.0.9/cryptos/coins_async/base.py
+-rw-rw-rw-   0        0        0     1252 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/coins_async/bitcoin.py
+-rw-rw-rw-   0        0        0     1352 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/coins_async/bitcoin_cash.py
+-rw-rw-rw-   0        0        0      746 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/coins_async/dash.py
+-rw-rw-rw-   0        0        0      929 2023-07-18 14:54:54.000000 cryptos-2.0.9/cryptos/coins_async/dogecoin.py
+-rw-rw-rw-   0        0        0      976 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/coins_async/litecoin.py
+-rw-rw-rw-   0        0        0     1657 2022-10-03 10:19:24.000000 cryptos-2.0.9/cryptos/composite.py
+-rw-rw-rw-   0        0        0      402 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/constants.py
+-rw-rw-rw-   0        0        0     8911 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/deterministic.py
+drwxrwxrwx   0        0        0        0 2023-07-18 14:56:40.710862 cryptos-2.0.9/cryptos/electrumx_client/
+-rw-rw-rw-   0        0        0       37 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/electrumx_client/__init__.py
+-rw-rw-rw-   0        0        0    22725 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/electrumx_client/client.py
+drwxrwxrwx   0        0        0        0 2023-07-18 14:56:40.726682 cryptos-2.0.9/cryptos/electrumx_client/servers/
+-rw-rw-rw-   0        0        0    10969 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/electrumx_client/servers/bitcoin.json
+-rw-rw-rw-   0        0        0     3618 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/electrumx_client/servers/bitcoin_cash.json
+-rw-rw-rw-   0        0        0     1093 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/electrumx_client/servers/bitcoin_cash_testnet.json
+-rw-rw-rw-   0        0        0      936 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/electrumx_client/servers/bitcoin_testnet.json
+-rw-rw-rw-   0        0        0      720 2023-07-18 14:54:54.000000 cryptos-2.0.9/cryptos/electrumx_client/servers/dash.json
+-rw-rw-rw-   0        0        0      486 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/electrumx_client/servers/dash_testnet.json
+-rw-rw-rw-   0        0        0      339 2023-07-18 14:54:54.000000 cryptos-2.0.9/cryptos/electrumx_client/servers/doge.json
+-rw-rw-rw-   0        0        0      254 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/electrumx_client/servers/doge_testnet.json
+-rw-rw-rw-   0        0        0      973 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/electrumx_client/servers/litecoin.json
+-rw-rw-rw-   0        0        0      283 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/electrumx_client/servers/litecoin_testnet.json
+-rw-rw-rw-   0        0        0      257 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/electrumx_client/servers/testing.json
+-rw-rw-rw-   0        0        0     2400 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/electrumx_client/types.py
+-rw-rw-rw-   0        0        0    15164 2022-10-03 10:19:24.000000 cryptos-2.0.9/cryptos/english.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 14:56:40.742524 cryptos-2.0.9/cryptos/explorers/
+-rw-rw-rw-   0        0        0      644 2022-10-03 10:19:24.000000 cryptos-2.0.9/cryptos/explorers/__init__.py
+-rw-rw-rw-   0        0        0     3268 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/explorers/base_insight.py
+-rw-rw-rw-   0        0        0      338 2022-10-03 10:19:24.000000 cryptos-2.0.9/cryptos/explorers/bitpay.py
+-rw-rw-rw-   0        0        0     4045 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/explorers/blockchain.py
+-rw-rw-rw-   0        0        0     1074 2022-10-03 10:19:24.000000 cryptos-2.0.9/cryptos/explorers/blockcypher.py
+-rw-rw-rw-   0        0        0     1280 2022-10-03 10:19:24.000000 cryptos-2.0.9/cryptos/explorers/blockdozer.py
+-rw-rw-rw-   0        0        0     1264 2022-10-03 10:19:24.000000 cryptos-2.0.9/cryptos/explorers/btg_explorer.py
+-rw-rw-rw-   0        0        0     1242 2022-10-03 10:19:24.000000 cryptos-2.0.9/cryptos/explorers/dash_siampm.py
+-rw-rw-rw-   0        0        0     3047 2022-10-03 10:19:24.000000 cryptos-2.0.9/cryptos/explorers/sochain.py
+-rw-rw-rw-   0        0        0      559 2022-10-03 10:19:24.000000 cryptos-2.0.9/cryptos/explorers/utils.py
+-rw-rw-rw-   0        0        0    18584 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/keystore.py
+-rw-rw-rw-   0        0        0    19302 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/main.py
+-rw-rw-rw-   0        0        0     8436 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/mnemonic.py
+-rw-rw-rw-   0        0        0     2838 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/opcodes.py
+-rw-rw-rw-   0        0        0     3494 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/py3specials.py
+-rw-rw-rw-   0        0        0    15159 2022-10-03 10:19:24.000000 cryptos-2.0.9/cryptos/ripemd.py
+-rw-rw-rw-   0        0        0      364 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/script_utils.py
+-rw-rw-rw-   0        0        0     6099 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/segwit_addr.py
+-rw-rw-rw-   0        0        0     3777 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/stealth.py
+drwxrwxrwx   0        0        0        0 2023-07-18 14:56:40.742524 cryptos-2.0.9/cryptos/testing/
+-rw-rw-rw-   0        0        0        0 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/testing/__init__.py
+-rw-rw-rw-   0        0        0    33904 2023-05-23 16:18:56.000000 cryptos-2.0.9/cryptos/testing/testcases.py
+-rw-rw-rw-   0        0        0    56457 2023-05-23 16:18:56.000000 cryptos-2.0.9/cryptos/testing/testcases_async.py
+-rw-rw-rw-   0        0        0    21694 2023-04-03 17:25:43.000000 cryptos-2.0.9/cryptos/transaction.py
+-rw-rw-rw-   0        0        0     2414 2023-04-03 17:25:43.000000 cryptos-2.0.9/cryptos/types.py
+-rw-rw-rw-   0        0        0     2040 2023-03-24 21:15:30.000000 cryptos-2.0.9/cryptos/utils.py
+-rw-rw-rw-   0        0        0    12247 2023-05-23 16:18:56.000000 cryptos-2.0.9/cryptos/wallet.py
+-rw-rw-rw-   0        0        0     6746 2023-03-22 13:46:57.000000 cryptos-2.0.9/cryptos/wallet_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-18 14:56:40.672170 cryptos-2.0.9/cryptos.egg-info/
+-rw-rw-rw-   0        0        0    41586 2023-07-18 14:56:40.000000 cryptos-2.0.9/cryptos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3093 2023-07-18 14:56:40.000000 cryptos-2.0.9/cryptos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 14:56:40.000000 cryptos-2.0.9/cryptos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      438 2023-07-18 14:56:40.000000 cryptos-2.0.9/cryptos.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       80 2023-07-18 14:56:40.000000 cryptos-2.0.9/cryptos.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-07-18 14:56:40.000000 cryptos-2.0.9/cryptos.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 14:56:40.794374 cryptos-2.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1749 2023-07-18 14:55:28.000000 cryptos-2.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 14:56:40.759085 cryptos-2.0.9/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-22 13:46:57.000000 cryptos-2.0.9/tests/__init__.py
+-rw-rw-rw-   0        0        0     5596 2023-03-22 13:46:57.000000 cryptos-2.0.9/tests/electrum_subscribe_mock_server.py
+drwxrwxrwx   0        0        0        0 2023-07-18 14:56:40.769503 cryptos-2.0.9/tests/test_coins/
+-rw-rw-rw-   0        0        0        0 2023-03-22 13:46:57.000000 cryptos-2.0.9/tests/test_coins/__init__.py
+-rw-rw-rw-   0        0        0    13157 2023-04-03 13:33:46.000000 cryptos-2.0.9/tests/test_coins/test_bitcoin_testnet.py
+drwxrwxrwx   0        0        0        0 2023-07-18 14:56:40.785837 cryptos-2.0.9/tests/test_coins_async/
+-rw-rw-rw-   0        0        0        0 2023-03-22 13:46:57.000000 cryptos-2.0.9/tests/test_coins_async/__init__.py
+-rw-rw-rw-   0        0        0    16130 2023-04-03 17:25:43.000000 cryptos-2.0.9/tests/test_coins_async/test_bitcoin.py
+-rw-rw-rw-   0        0        0    11403 2023-03-24 22:06:15.000000 cryptos-2.0.9/tests/test_coins_async/test_bitcoin_cash.py
+-rw-rw-rw-   0        0        0     8815 2023-03-22 13:46:57.000000 cryptos-2.0.9/tests/test_coins_async/test_bitcoin_cash_testnet.py
+-rw-rw-rw-   0        0        0    10667 2023-04-03 12:02:39.000000 cryptos-2.0.9/tests/test_coins_async/test_bitcoin_testnet.py
+-rw-rw-rw-   0        0        0     5932 2023-03-22 13:46:57.000000 cryptos-2.0.9/tests/test_coins_async/test_dash.py
+-rw-rw-rw-   0        0        0     5829 2023-04-03 12:02:39.000000 cryptos-2.0.9/tests/test_coins_async/test_dash_testnet.py
+-rw-rw-rw-   0        0        0     7355 2023-03-22 13:46:57.000000 cryptos-2.0.9/tests/test_coins_async/test_dogecoin.py
+-rw-rw-rw-   0        0        0     5694 2023-03-22 13:46:57.000000 cryptos-2.0.9/tests/test_coins_async/test_dogecoin_testnet.py
+-rw-rw-rw-   0        0        0    14402 2023-05-23 16:18:56.000000 cryptos-2.0.9/tests/test_coins_async/test_litecoin.py
+-rw-rw-rw-   0        0        0     9245 2023-03-22 13:46:57.000000 cryptos-2.0.9/tests/test_coins_async/test_litecoin_testnet.py
+-rw-rw-rw-   0        0        0    26157 2023-03-22 13:46:57.000000 cryptos-2.0.9/tests/test_electrum_client.py
+-rw-rw-rw-   0        0        0    28702 2023-03-22 13:46:57.000000 cryptos-2.0.9/tests/test_general.py
+-rw-rw-rw-   0        0        0     4366 2023-03-22 13:46:57.000000 cryptos-2.0.9/tests/test_stealth.py
+-rw-rw-rw-   0        0        0    32352 2023-03-22 13:46:57.000000 cryptos-2.0.9/tests/test_wallet.py
```

### Comparing `cryptos-2.0.8/LICENSE` & `cryptos-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/PKG-INFO` & `cryptos-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: cryptos
-Version: 2.0.8
+Version: 2.0.9
 Summary: Python Crypto Coin Tools
 Home-page: http://github.com/primal100/pybitcointools
 Author: Paul Martin
 Author-email: greatestloginnameever@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security :: Cryptography
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pycryptotools, Python library for Crypto coins signatures and transactions
```

### Comparing `cryptos-2.0.8/README.md` & `cryptos-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/crypto_scripts/broadcast.py` & `cryptos-2.0.9/crypto_scripts/broadcast.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/crypto_scripts/convert_private_key.py` & `cryptos-2.0.9/crypto_scripts/convert_private_key.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/crypto_scripts/create_private_key.py` & `cryptos-2.0.9/crypto_scripts/create_private_key.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/crypto_scripts/cryptosend.py` & `cryptos-2.0.9/crypto_scripts/cryptosend.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/crypto_scripts/explorer.py` & `cryptos-2.0.9/crypto_scripts/explorer.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/crypto_scripts/get_block_sizes.py` & `cryptos-2.0.9/crypto_scripts/get_block_sizes.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/crypto_scripts/subscribe.py` & `cryptos-2.0.9/crypto_scripts/subscribe.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/crypto_scripts/view_private_key_addresses.py` & `cryptos-2.0.9/crypto_scripts/view_private_key_addresses.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/blocks.py` & `cryptos-2.0.9/cryptos/blocks.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/cashaddr.py` & `cryptos-2.0.9/cryptos/cashaddr.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/coins/base.py` & `cryptos-2.0.9/cryptos/coins/base.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/coins_async/base.py` & `cryptos-2.0.9/cryptos/coins_async/base.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/coins_async/bitcoin.py` & `cryptos-2.0.9/cryptos/coins_async/bitcoin.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/coins_async/bitcoin_cash.py` & `cryptos-2.0.9/cryptos/coins_async/bitcoin_cash.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/coins_async/dash.py` & `cryptos-2.0.9/cryptos/coins_async/dash.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/coins_async/dogecoin.py` & `cryptos-2.0.9/cryptos/coins_async/dogecoin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from .bitcoin import BaseCoin
 
-
 class Doge(BaseCoin):
     coin_symbol = "DOGE"
     display_name = "Dogecoin"
     segwit_supported = False
     magicbyte = 0x1e
     minimum_fee = 300000
     script_magicbyte = 0x16
```

### Comparing `cryptos-2.0.8/cryptos/coins_async/litecoin.py` & `cryptos-2.0.9/cryptos/coins_async/litecoin.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/composite.py` & `cryptos-2.0.9/cryptos/composite.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/deterministic.py` & `cryptos-2.0.9/cryptos/deterministic.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/electrumx_client/client.py` & `cryptos-2.0.9/cryptos/electrumx_client/client.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/electrumx_client/servers/bitcoin.json` & `cryptos-2.0.9/cryptos/electrumx_client/servers/bitcoin.json`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/electrumx_client/servers/bitcoin_cash.json` & `cryptos-2.0.9/cryptos/electrumx_client/servers/bitcoin_cash.json`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/electrumx_client/servers/bitcoin_cash_testnet.json` & `cryptos-2.0.9/cryptos/electrumx_client/servers/bitcoin_cash_testnet.json`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/electrumx_client/servers/bitcoin_testnet.json` & `cryptos-2.0.9/cryptos/electrumx_client/servers/bitcoin_testnet.json`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/electrumx_client/servers/litecoin.json` & `cryptos-2.0.9/cryptos/electrumx_client/servers/litecoin.json`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/electrumx_client/types.py` & `cryptos-2.0.9/cryptos/electrumx_client/types.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/english.txt` & `cryptos-2.0.9/cryptos/english.txt`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/explorers/__init__.py` & `cryptos-2.0.9/cryptos/explorers/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/explorers/base_insight.py` & `cryptos-2.0.9/cryptos/explorers/base_insight.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/explorers/blockchain.py` & `cryptos-2.0.9/cryptos/explorers/blockchain.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/explorers/blockcypher.py` & `cryptos-2.0.9/cryptos/explorers/blockcypher.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/explorers/blockdozer.py` & `cryptos-2.0.9/cryptos/explorers/blockdozer.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/explorers/btg_explorer.py` & `cryptos-2.0.9/cryptos/explorers/btg_explorer.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/explorers/dash_siampm.py` & `cryptos-2.0.9/cryptos/explorers/dash_siampm.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/explorers/sochain.py` & `cryptos-2.0.9/cryptos/explorers/sochain.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/explorers/utils.py` & `cryptos-2.0.9/cryptos/explorers/utils.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/keystore.py` & `cryptos-2.0.9/cryptos/keystore.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/main.py` & `cryptos-2.0.9/cryptos/main.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/mnemonic.py` & `cryptos-2.0.9/cryptos/mnemonic.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/opcodes.py` & `cryptos-2.0.9/cryptos/opcodes.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/py3specials.py` & `cryptos-2.0.9/cryptos/py3specials.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/ripemd.py` & `cryptos-2.0.9/cryptos/ripemd.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/segwit_addr.py` & `cryptos-2.0.9/cryptos/segwit_addr.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/stealth.py` & `cryptos-2.0.9/cryptos/stealth.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/testing/testcases.py` & `cryptos-2.0.9/cryptos/testing/testcases.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/testing/testcases_async.py` & `cryptos-2.0.9/cryptos/testing/testcases_async.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/transaction.py` & `cryptos-2.0.9/cryptos/transaction.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/types.py` & `cryptos-2.0.9/cryptos/types.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/utils.py` & `cryptos-2.0.9/cryptos/utils.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/wallet.py` & `cryptos-2.0.9/cryptos/wallet.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos/wallet_utils.py` & `cryptos-2.0.9/cryptos/wallet_utils.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/cryptos.egg-info/PKG-INFO` & `cryptos-2.0.9/cryptos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: cryptos
-Version: 2.0.8
+Version: 2.0.9
 Summary: Python Crypto Coin Tools
 Home-page: http://github.com/primal100/pybitcointools
 Author: Paul Martin
 Author-email: greatestloginnameever@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security :: Cryptography
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pycryptotools, Python library for Crypto coins signatures and transactions
```

### Comparing `cryptos-2.0.8/cryptos.egg-info/SOURCES.txt` & `cryptos-2.0.9/cryptos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/setup.py` & `cryptos-2.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 setup(name='cryptos',
-      version='2.0.8',
+      version='2.0.9',
       description='Python Crypto Coin Tools',
       long_description=open('README.md').read(),
       long_description_content_type='text/markdown',
       author='Paul Martin',
       author_email='greatestloginnameever@gmail.com',
       url='http://github.com/primal100/pybitcointools',
       packages=find_packages(),
@@ -24,15 +24,14 @@
       classifiers=[
             'Development Status :: 5 - Production/Stable',
             'Intended Audience :: Developers',
             'Intended Audience :: Education',
             'License :: OSI Approved :: MIT License',
             'Operating System :: OS Independent',
             'Programming Language :: Python',
-            'Programming Language :: Python :: 2',
             'Programming Language :: Python :: 3',
             'Topic :: Security :: Cryptography',
       ],
       entry_points='''
             [console_scripts]
             broadcast=crypto_scripts.broadcast:main
             convert_private_key=crypto_scripts.convert_private_key:main
```

### Comparing `cryptos-2.0.8/tests/electrum_subscribe_mock_server.py` & `cryptos-2.0.9/tests/electrum_subscribe_mock_server.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/tests/test_coins/test_bitcoin_testnet.py` & `cryptos-2.0.9/tests/test_coins/test_bitcoin_testnet.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/tests/test_coins_async/test_bitcoin.py` & `cryptos-2.0.9/tests/test_coins_async/test_bitcoin.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/tests/test_coins_async/test_bitcoin_cash.py` & `cryptos-2.0.9/tests/test_coins_async/test_bitcoin_cash.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/tests/test_coins_async/test_bitcoin_cash_testnet.py` & `cryptos-2.0.9/tests/test_coins_async/test_bitcoin_cash_testnet.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/tests/test_coins_async/test_bitcoin_testnet.py` & `cryptos-2.0.9/tests/test_coins_async/test_bitcoin_testnet.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/tests/test_coins_async/test_dash.py` & `cryptos-2.0.9/tests/test_coins_async/test_dash.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/tests/test_coins_async/test_dash_testnet.py` & `cryptos-2.0.9/tests/test_coins_async/test_dash_testnet.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/tests/test_coins_async/test_dogecoin.py` & `cryptos-2.0.9/tests/test_coins_async/test_dogecoin.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/tests/test_coins_async/test_dogecoin_testnet.py` & `cryptos-2.0.9/tests/test_coins_async/test_dogecoin_testnet.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/tests/test_coins_async/test_litecoin.py` & `cryptos-2.0.9/tests/test_coins_async/test_litecoin.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/tests/test_coins_async/test_litecoin_testnet.py` & `cryptos-2.0.9/tests/test_coins_async/test_litecoin_testnet.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/tests/test_electrum_client.py` & `cryptos-2.0.9/tests/test_electrum_client.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/tests/test_general.py` & `cryptos-2.0.9/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/tests/test_stealth.py` & `cryptos-2.0.9/tests/test_stealth.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.8/tests/test_wallet.py` & `cryptos-2.0.9/tests/test_wallet.py`

 * *Files identical despite different names*

