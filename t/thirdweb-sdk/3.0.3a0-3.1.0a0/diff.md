# Comparing `tmp/thirdweb_sdk-3.0.3a0.tar.gz` & `tmp/thirdweb_sdk-3.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thirdweb_sdk-3.0.3a0.tar", max compression
+gzip compressed data, was "thirdweb_sdk-3.1.0a0.tar", max compression
```

## Comparing `thirdweb_sdk-3.0.3a0.tar` & `thirdweb_sdk-3.1.0a0.tar`

### file list

```diff
@@ -1,353 +1,354 @@
--rw-r--r--   0        0        0    10942 2023-03-13 04:51:11.285705 thirdweb_sdk-3.0.3a0/LICENSE
--rw-r--r--   0        0        0     5877 2023-03-21 02:20:09.125450 thirdweb_sdk-3.0.3a0/README.md
--rw-r--r--   0        0        0     2644 2023-05-12 02:13:24.212202 thirdweb_sdk-3.0.3a0/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-03-13 04:51:11.293180 thirdweb_sdk-3.0.3a0/thirdweb/.DS_Store
--rw-r--r--   0        0        0       30 2023-03-13 04:51:11.293237 thirdweb_sdk-3.0.3a0/thirdweb/__init__.py
--rw-r--r--   0        0        0    20818 2023-03-21 21:23:13.236831 thirdweb_sdk-3.0.3a0/thirdweb/abi/__init__.py
--rw-r--r--   0        0        0    85792 2023-03-21 21:23:13.237140 thirdweb_sdk-3.0.3a0/thirdweb/abi/airdrop_erc1155.py
--rw-r--r--   0        0        0    68008 2023-03-21 21:23:13.237423 thirdweb_sdk-3.0.3a0/thirdweb/abi/airdrop_erc1155_claimable.py
--rw-r--r--   0        0        0    80026 2023-03-21 21:23:13.237714 thirdweb_sdk-3.0.3a0/thirdweb/abi/airdrop_erc20.py
--rw-r--r--   0        0        0    59394 2023-03-21 21:23:13.237980 thirdweb_sdk-3.0.3a0/thirdweb/abi/airdrop_erc20_claimable.py
--rw-r--r--   0        0        0    80078 2023-03-21 21:23:13.238277 thirdweb_sdk-3.0.3a0/thirdweb/abi/airdrop_erc721.py
--rw-r--r--   0        0        0    64449 2023-03-21 21:23:13.238530 thirdweb_sdk-3.0.3a0/thirdweb/abi/airdrop_erc721_claimable.py
--rw-r--r--   0        0        0     9165 2023-03-21 21:23:13.238692 thirdweb_sdk-3.0.3a0/thirdweb/abi/app_u_r_i.py
--rw-r--r--   0        0        0     8936 2023-03-21 21:23:13.238839 thirdweb_sdk-3.0.3a0/thirdweb/abi/batch_mint_metadata.py
--rw-r--r--   0        0        0     3300 2023-03-21 21:23:13.238969 thirdweb_sdk-3.0.3a0/thirdweb/abi/context.py
--rw-r--r--   0        0        0     9470 2023-03-21 21:23:13.239125 thirdweb_sdk-3.0.3a0/thirdweb/abi/contract_metadata.py
--rw-r--r--   0        0        0     9520 2023-03-21 21:23:13.239295 thirdweb_sdk-3.0.3a0/thirdweb/abi/contract_metadata_logic.py
--rw-r--r--   0        0        0     6115 2023-03-21 21:23:13.239442 thirdweb_sdk-3.0.3a0/thirdweb/abi/contract_metadata_storage.py
--rw-r--r--   0        0        0    90485 2023-03-21 21:23:13.239903 thirdweb_sdk-3.0.3a0/thirdweb/abi/contract_publisher.py
--rw-r--r--   0        0        0     3308 2023-03-21 21:23:13.240119 thirdweb_sdk-3.0.3a0/thirdweb/abi/counters.py
--rw-r--r--   0        0        0     5790 2023-03-21 21:23:13.240283 thirdweb_sdk-3.0.3a0/thirdweb/abi/currency_transfer_lib.py
--rw-r--r--   0        0        0    12320 2023-03-21 21:23:13.240459 thirdweb_sdk-3.0.3a0/thirdweb/abi/default_operator_filterer.py
--rw-r--r--   0        0        0    10109 2023-03-21 21:23:13.240627 thirdweb_sdk-3.0.3a0/thirdweb/abi/default_operator_filterer_upgradeable.py
--rw-r--r--   0        0        0    21950 2023-03-21 21:23:13.240845 thirdweb_sdk-3.0.3a0/thirdweb/abi/delayed_reveal.py
--rw-r--r--   0        0        0    76514 2023-03-21 21:23:13.241162 thirdweb_sdk-3.0.3a0/thirdweb/abi/direct_listings_logic.py
--rw-r--r--   0        0        0     6079 2023-03-21 21:23:13.241334 thirdweb_sdk-3.0.3a0/thirdweb/abi/direct_listings_storage.py
--rw-r--r--   0        0        0    41239 2023-03-21 21:23:13.241551 thirdweb_sdk-3.0.3a0/thirdweb/abi/drop.py
--rw-r--r--   0        0        0    46630 2023-03-21 21:23:13.241777 thirdweb_sdk-3.0.3a0/thirdweb/abi/drop1155.py
--rw-r--r--   0        0        0   229869 2023-03-21 21:23:13.242485 thirdweb_sdk-3.0.3a0/thirdweb/abi/drop_erc1155.py
--rw-r--r--   0        0        0   206478 2023-03-21 21:23:13.243046 thirdweb_sdk-3.0.3a0/thirdweb/abi/drop_erc20.py
--rw-r--r--   0        0        0   243271 2023-03-21 21:23:13.243687 thirdweb_sdk-3.0.3a0/thirdweb/abi/drop_erc721.py
--rw-r--r--   0        0        0    33157 2023-03-21 21:23:13.243907 thirdweb_sdk-3.0.3a0/thirdweb/abi/drop_single_phase.py
--rw-r--r--   0        0        0    37416 2023-03-21 21:23:13.244123 thirdweb_sdk-3.0.3a0/thirdweb/abi/drop_single_phase1155.py
--rw-r--r--   0        0        0   241058 2023-03-21 21:23:13.244635 thirdweb_sdk-3.0.3a0/thirdweb/abi/droperc1155_v2.py
--rw-r--r--   0        0        0   226555 2023-03-21 21:23:13.245160 thirdweb_sdk-3.0.3a0/thirdweb/abi/droperc20_v2.py
--rw-r--r--   0        0        0   249102 2023-03-21 21:23:13.245721 thirdweb_sdk-3.0.3a0/thirdweb/abi/droperc721_v3.py
--rw-r--r--   0        0        0    43296 2023-03-21 21:23:13.245944 thirdweb_sdk-3.0.3a0/thirdweb/abi/dropsinglephase1155_v1.py
--rw-r--r--   0        0        0    38914 2023-03-21 21:23:13.246156 thirdweb_sdk-3.0.3a0/thirdweb/abi/dropsinglephase_v1.py
--rw-r--r--   0        0        0     3442 2023-03-21 21:23:13.246326 thirdweb_sdk-3.0.3a0/thirdweb/abi/e_i_p712_chainless_domain.py
--rw-r--r--   0        0        0     3284 2023-03-21 21:23:13.246467 thirdweb_sdk-3.0.3a0/thirdweb/abi/ecdsa.py
--rw-r--r--   0        0        0   156536 2023-03-21 21:23:13.246871 thirdweb_sdk-3.0.3a0/thirdweb/abi/edition_stake.py
--rw-r--r--   0        0        0     3292 2023-03-21 21:23:13.247008 thirdweb_sdk-3.0.3a0/thirdweb/abi/eip712.py
--rw-r--r--   0        0        0    64754 2023-03-21 21:23:13.247249 thirdweb_sdk-3.0.3a0/thirdweb/abi/english_auctions_logic.py
--rw-r--r--   0        0        0     6097 2023-03-21 21:23:13.247424 thirdweb_sdk-3.0.3a0/thirdweb/abi/english_auctions_storage.py
--rw-r--r--   0        0        0     3378 2023-03-21 21:23:13.247600 thirdweb_sdk-3.0.3a0/thirdweb/abi/enumerable_set.py
--rw-r--r--   0        0        0    43189 2023-03-21 21:23:13.247814 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc1155.py
--rw-r--r--   0        0        0   115583 2023-03-21 21:23:13.248175 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc1155_base.py
--rw-r--r--   0        0        0   139620 2023-03-21 21:23:13.248544 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc1155_delayed_reveal.py
--rw-r--r--   0        0        0   170049 2023-03-21 21:23:13.248978 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc1155_drop.py
--rw-r--r--   0        0        0    18760 2023-03-21 21:23:13.249150 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc1155_holder.py
--rw-r--r--   0        0        0   121380 2023-03-21 21:23:13.249486 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc1155_lazy_mint.py
--rw-r--r--   0        0        0   112914 2023-03-21 21:23:13.249801 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc1155_preset_upgradeable.py
--rw-r--r--   0        0        0    18357 2023-03-21 21:23:13.249969 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc1155_receiver.py
--rw-r--r--   0        0        0   134633 2023-03-21 21:23:13.250319 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc1155_signature_mint.py
--rw-r--r--   0        0        0     6858 2023-03-21 21:23:13.250859 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc165.py
--rw-r--r--   0        0        0     6039 2023-03-21 21:23:13.251003 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc1967_proxy.py
--rw-r--r--   0        0        0     5644 2023-03-21 21:23:13.251135 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc1967_upgrade.py
--rw-r--r--   0        0        0    39698 2023-03-21 21:23:13.251312 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc20.py
--rw-r--r--   0        0        0    72167 2023-03-21 21:23:13.251539 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc20_base.py
--rw-r--r--   0        0        0   104921 2023-03-21 21:23:13.251834 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc20_drop.py
--rw-r--r--   0        0        0   136778 2023-03-21 21:23:13.252201 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc20_drop_vote.py
--rw-r--r--   0        0        0    50917 2023-03-21 21:23:13.252406 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc20_permit.py
--rw-r--r--   0        0        0    90382 2023-03-21 21:23:13.252677 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc20_signature_mint.py
--rw-r--r--   0        0        0   122210 2023-03-21 21:23:13.253003 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc20_signature_mint_vote.py
--rw-r--r--   0        0        0   103909 2023-03-21 21:23:13.253295 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc20_vote.py
--rw-r--r--   0        0        0    82607 2023-03-21 21:23:13.253572 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc20_votes.py
--rw-r--r--   0        0        0     6811 2023-03-21 21:23:13.253736 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc2771_context.py
--rw-r--r--   0        0        0     7980 2023-03-21 21:23:13.253881 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc2771_context_consumer.py
--rw-r--r--   0        0        0     6856 2023-03-21 21:23:13.254037 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc2771_context_logic.py
--rw-r--r--   0        0        0     6079 2023-03-21 21:23:13.254191 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc2771_context_storage.py
--rw-r--r--   0        0        0     7631 2023-03-21 21:23:13.254332 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc2771_context_upgradeable.py
--rw-r--r--   0        0        0     6955 2023-03-21 21:23:13.254489 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc2771_context_upgradeable_logic.py
--rw-r--r--   0        0        0     6282 2023-03-21 21:23:13.254610 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc2771_context_upgradeable_storage.py
--rw-r--r--   0        0        0    53696 2023-03-21 21:23:13.254828 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc721_a_upgradeable.py
--rw-r--r--   0        0        0   119717 2023-03-21 21:23:13.255136 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc721_base.py
--rw-r--r--   0        0        0   142298 2023-03-21 21:23:13.255489 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc721_delayed_reveal.py
--rw-r--r--   0        0        0   169717 2023-03-21 21:23:13.255907 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc721_drop.py
--rw-r--r--   0        0        0     8931 2023-03-21 21:23:13.256062 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc721_holder.py
--rw-r--r--   0        0        0   124064 2023-03-21 21:23:13.256406 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc721_lazy_mint.py
--rw-r--r--   0        0        0   182421 2023-03-21 21:23:13.256821 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc721_multiwrap.py
--rw-r--r--   0        0        0   138584 2023-03-21 21:23:13.257156 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc721_signature_mint.py
--rw-r--r--   0        0        0    52988 2023-03-21 21:23:13.257362 thirdweb_sdk-3.0.3a0/thirdweb/abi/erc721a.py
--rw-r--r--   0        0        0     3300 2023-03-21 21:23:13.257494 thirdweb_sdk-3.0.3a0/thirdweb/abi/fee_type.py
--rw-r--r--   0        0        0    11166 2023-03-21 21:23:13.257651 thirdweb_sdk-3.0.3a0/thirdweb/abi/forwarder_consumer.py
--rw-r--r--   0        0        0    26106 2023-03-21 21:23:13.257810 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_airdrop_erc1155.py
--rw-r--r--   0        0        0    10788 2023-03-21 21:23:13.257985 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_airdrop_erc1155_claimable.py
--rw-r--r--   0        0        0    25450 2023-03-21 21:23:13.258153 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_airdrop_erc20.py
--rw-r--r--   0        0        0    10033 2023-03-21 21:23:13.258293 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_airdrop_erc20_claimable.py
--rw-r--r--   0        0        0    25497 2023-03-21 21:23:13.258455 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_airdrop_erc721.py
--rw-r--r--   0        0        0    10043 2023-03-21 21:23:13.258592 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_airdrop_erc721_claimable.py
--rw-r--r--   0        0        0     9175 2023-03-21 21:23:13.258726 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_app_u_r_i.py
--rw-r--r--   0        0        0     5661 2023-03-21 21:23:13.258854 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_beacon.py
--rw-r--r--   0        0        0    11588 2023-03-21 21:23:13.258998 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_burnable_erc1155.py
--rw-r--r--   0        0        0     9891 2023-03-21 21:23:13.259133 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_burnable_erc20.py
--rw-r--r--   0        0        0     6533 2023-03-21 21:23:13.259256 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_burnable_erc721.py
--rw-r--r--   0        0        0     3394 2023-03-21 21:23:13.259376 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_claim_condition.py
--rw-r--r--   0        0        0     3474 2023-03-21 21:23:13.259510 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_claim_condition_multi_phase.py
--rw-r--r--   0        0        0    10930 2023-03-21 21:23:13.259648 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_claim_conditions_single_phase.py
--rw-r--r--   0        0        0    13127 2023-03-21 21:23:13.259788 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_claimable_erc1155.py
--rw-r--r--   0        0        0    11876 2023-03-21 21:23:13.259913 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_claimable_erc721.py
--rw-r--r--   0        0        0     7811 2023-03-21 21:23:13.260053 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_context.py
--rw-r--r--   0        0        0    23449 2023-03-21 21:23:13.260235 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_contract_deployer.py
--rw-r--r--   0        0        0     8413 2023-03-21 21:23:13.260387 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_contract_factory.py
--rw-r--r--   0        0        0     9480 2023-03-21 21:23:13.260521 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_contract_metadata.py
--rw-r--r--   0        0        0    44219 2023-03-21 21:23:13.260712 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_contract_publisher.py
--rw-r--r--   0        0        0    11835 2023-03-21 21:23:13.260853 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_delayed_reveal.py
--rw-r--r--   0        0        0    15264 2023-03-21 21:23:13.260989 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_delayed_reveal_deprecated.py
--rw-r--r--   0        0        0    57624 2023-03-21 21:23:13.261211 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_direct_listings.py
--rw-r--r--   0        0        0    20142 2023-03-21 21:23:13.261365 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_drop.py
--rw-r--r--   0        0        0    21722 2023-03-21 21:23:13.261543 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_drop1155.py
--rw-r--r--   0        0        0     3426 2023-03-21 21:23:13.261696 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_drop_claim_condition.py
--rw-r--r--   0        0        0    60183 2023-03-21 21:23:13.261901 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_drop_erc1155.py
--rw-r--r--   0        0        0    43180 2023-03-21 21:23:13.262090 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_drop_erc20.py
--rw-r--r--   0        0        0    66414 2023-03-21 21:23:13.262347 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_drop_erc721.py
--rw-r--r--   0        0        0    20224 2023-03-21 21:23:13.262510 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_drop_single_phase.py
--rw-r--r--   0        0        0    21804 2023-03-21 21:23:13.262667 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_drop_single_phase1155.py
--rw-r--r--   0        0        0    11373 2023-03-21 21:23:13.262807 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_edition_stake.py
--rw-r--r--   0        0        0    55894 2023-03-21 21:23:13.263009 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_english_auctions.py
--rw-r--r--   0        0        0     5838 2023-03-21 21:23:13.263163 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_erc1155_enumerable.py
--rw-r--r--   0        0        0     6466 2023-03-21 21:23:13.263300 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_erc1155_metadata.py
--rw-r--r--   0        0        0    18366 2023-03-21 21:23:13.263446 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_erc1155_receiver.py
--rw-r--r--   0        0        0     6575 2023-03-21 21:23:13.263588 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_erc1155_supply.py
--rw-r--r--   0        0        0     5815 2023-03-21 21:23:13.263713 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_erc1822_proxiable.py
--rw-r--r--   0        0        0     9937 2023-03-21 21:23:13.263831 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_erc20_metadata.py
--rw-r--r--   0        0        0    14843 2023-03-21 21:23:13.263957 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_erc20_permit.py
--rw-r--r--   0        0        0     6820 2023-03-21 21:23:13.264083 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_erc2771_context.py
--rw-r--r--   0        0        0    10336 2023-03-21 21:23:13.264227 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_erc721_enumerable.py
--rw-r--r--   0        0        0    10879 2023-03-21 21:23:13.264362 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_erc721_metadata.py
--rw-r--r--   0        0        0     8622 2023-03-21 21:23:13.264491 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_erc721_receiver.py
--rw-r--r--   0        0        0     5733 2023-03-21 21:23:13.264619 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_erc721_supply.py
--rw-r--r--   0        0        0     7383 2023-03-21 21:23:13.264746 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_fee_tier_placement_extension.py
--rw-r--r--   0        0        0     9333 2023-03-21 21:23:13.264861 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_lazy_mint.py
--rw-r--r--   0        0        0     9955 2023-03-21 21:23:13.264991 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_lazy_mint_with_tier.py
--rw-r--r--   0        0        0    68265 2023-03-21 21:23:13.265206 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_marketplace.py
--rw-r--r--   0        0        0     8961 2023-03-21 21:23:13.265364 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_mintable_erc1155.py
--rw-r--r--   0        0        0     7682 2023-03-21 21:23:13.265488 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_mintable_erc20.py
--rw-r--r--   0        0        0     7691 2023-03-21 21:23:13.265603 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_mintable_erc721.py
--rw-r--r--   0        0        0     6643 2023-03-21 21:23:13.265712 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_multicall.py
--rw-r--r--   0        0        0    15555 2023-03-21 21:23:13.265837 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_multiwrap.py
--rw-r--r--   0        0        0    11286 2023-03-21 21:23:13.265950 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_n_f_t_stake.py
--rw-r--r--   0        0        0    32749 2023-03-21 21:23:13.266098 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_offers.py
--rw-r--r--   0        0        0    94730 2023-03-21 21:23:13.266342 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_operator_filter_registry.py
--rw-r--r--   0        0        0     9845 2023-03-21 21:23:13.266490 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_operator_filter_toggle.py
--rw-r--r--   0        0        0     9391 2023-03-21 21:23:13.266630 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_ownable.py
--rw-r--r--   0        0        0    19897 2023-03-21 21:23:13.266769 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_pack.py
--rw-r--r--   0        0        0    31414 2023-03-21 21:23:13.266928 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_pack_v_r_f_direct.py
--rw-r--r--   0        0        0    23527 2023-03-21 21:23:13.267072 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_permissions.py
--rw-r--r--   0        0        0    30461 2023-03-21 21:23:13.267260 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_permissions_enumerable.py
--rw-r--r--   0        0        0    11346 2023-03-21 21:23:13.267463 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_platform_fee.py
--rw-r--r--   0        0        0    15146 2023-03-21 21:23:13.267593 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_plugin_map.py
--rw-r--r--   0        0        0     9980 2023-03-21 21:23:13.267723 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_primary_sale.py
--rw-r--r--   0        0        0    27471 2023-03-21 21:23:13.267868 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_router.py
--rw-r--r--   0        0        0    27105 2023-03-21 21:23:13.268058 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_royalty.py
--rw-r--r--   0        0        0     9998 2023-03-21 21:23:13.268194 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_signature_action.py
--rw-r--r--   0        0        0    16148 2023-03-21 21:23:13.268332 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_signature_mint_erc1155.py
--rw-r--r--   0        0        0    15154 2023-03-21 21:23:13.268485 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_signature_mint_erc20.py
--rw-r--r--   0        0        0    15923 2023-03-21 21:23:13.268633 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_signature_mint_erc721.py
--rw-r--r--   0        0        0    27313 2023-03-21 21:23:13.268779 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_staking1155.py
--rw-r--r--   0        0        0    19685 2023-03-21 21:23:13.268918 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_staking20.py
--rw-r--r--   0        0        0    18920 2023-03-21 21:23:13.269054 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_staking721.py
--rw-r--r--   0        0        0     7095 2023-03-21 21:23:13.269185 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_t_w_fee.py
--rw-r--r--   0        0        0    26206 2023-03-21 21:23:13.269336 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_t_w_multichain_registry.py
--rw-r--r--   0        0        0    21103 2023-03-21 21:23:13.269504 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_t_w_registry.py
--rw-r--r--   0        0        0    13067 2023-03-21 21:23:13.269651 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_thirdweb_contract.py
--rw-r--r--   0        0        0     3370 2023-03-21 21:23:13.269761 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_token_bundle.py
--rw-r--r--   0        0        0    53182 2023-03-21 21:23:13.270402 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_token_erc1155.py
--rw-r--r--   0        0        0    46867 2023-03-21 21:23:13.270660 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_token_erc20.py
--rw-r--r--   0        0        0    58484 2023-03-21 21:23:13.271450 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_token_erc721.py
--rw-r--r--   0        0        0    11351 2023-03-21 21:23:13.271592 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_token_stake.py
--rw-r--r--   0        0        0    27443 2023-03-21 21:23:13.271753 thirdweb_sdk-3.0.3a0/thirdweb/abi/i_votes.py
--rw-r--r--   0        0        0     3418 2023-03-21 21:23:13.271870 thirdweb_sdk-3.0.3a0/thirdweb/abi/iclaimcondition_v1.py
--rw-r--r--   0        0        0     3450 2023-03-21 21:23:13.271980 thirdweb_sdk-3.0.3a0/thirdweb/abi/idropclaimcondition_v2.py
--rw-r--r--   0        0        0    61520 2023-03-21 21:23:13.272188 thirdweb_sdk-3.0.3a0/thirdweb/abi/idroperc1155_v2.py
--rw-r--r--   0        0        0    44262 2023-03-21 21:23:13.272388 thirdweb_sdk-3.0.3a0/thirdweb/abi/idroperc20_v2.py
--rw-r--r--   0        0        0    67599 2023-03-21 21:23:13.272611 thirdweb_sdk-3.0.3a0/thirdweb/abi/idroperc721_v3.py
--rw-r--r--   0        0        0    21795 2023-03-21 21:23:13.272779 thirdweb_sdk-3.0.3a0/thirdweb/abi/idropsinglephase1155_v1.py
--rw-r--r--   0        0        0    20215 2023-03-21 21:23:13.272932 thirdweb_sdk-3.0.3a0/thirdweb/abi/idropsinglephase_v1.py
--rw-r--r--   0        0        0    31974 2023-03-21 21:23:13.273101 thirdweb_sdk-3.0.3a0/thirdweb/abi/ierc1155.py
--rw-r--r--   0        0        0     6867 2023-03-21 21:23:13.273333 thirdweb_sdk-3.0.3a0/thirdweb/abi/ierc165.py
--rw-r--r--   0        0        0    24799 2023-03-21 21:23:13.273460 thirdweb_sdk-3.0.3a0/thirdweb/abi/ierc20.py
--rw-r--r--   0        0        0    10953 2023-03-21 21:23:13.273598 thirdweb_sdk-3.0.3a0/thirdweb/abi/ierc2981.py
--rw-r--r--   0        0        0    39092 2023-03-21 21:23:13.273809 thirdweb_sdk-3.0.3a0/thirdweb/abi/ierc721.py
--rw-r--r--   0        0        0    49418 2023-03-21 21:23:13.274000 thirdweb_sdk-3.0.3a0/thirdweb/abi/ierc721a.py
--rw-r--r--   0        0        0     3362 2023-03-21 21:23:13.274132 thirdweb_sdk-3.0.3a0/thirdweb/abi/init_storage.py
--rw-r--r--   0        0        0     4108 2023-03-21 21:23:13.274281 thirdweb_sdk-3.0.3a0/thirdweb/abi/initializable.py
--rw-r--r--   0        0        0    13842 2023-03-21 21:23:13.274439 thirdweb_sdk-3.0.3a0/thirdweb/abi/isignatureminterc721_v1.py
--rw-r--r--   0        0        0    11782 2023-03-21 21:23:13.274565 thirdweb_sdk-3.0.3a0/thirdweb/abi/iweth.py
--rw-r--r--   0        0        0    14519 2023-03-21 21:23:13.274700 thirdweb_sdk-3.0.3a0/thirdweb/abi/lazy_mint.py
--rw-r--r--   0        0        0    19969 2023-03-21 21:23:13.274856 thirdweb_sdk-3.0.3a0/thirdweb/abi/lazy_mint_with_tier.py
--rw-r--r--   0        0        0   156959 2023-03-21 21:23:13.275265 thirdweb_sdk-3.0.3a0/thirdweb/abi/marketplace.py
--rw-r--r--   0        0        0   117081 2023-03-21 21:23:13.275601 thirdweb_sdk-3.0.3a0/thirdweb/abi/marketplace_v3.py
--rw-r--r--   0        0        0     3276 2023-03-21 21:23:13.275761 thirdweb_sdk-3.0.3a0/thirdweb/abi/math.py
--rw-r--r--   0        0        0     3362 2023-03-21 21:23:13.275902 thirdweb_sdk-3.0.3a0/thirdweb/abi/merkle_proof.py
--rw-r--r--   0        0        0     9839 2023-03-21 21:23:13.276042 thirdweb_sdk-3.0.3a0/thirdweb/abi/mock.py
--rw-r--r--   0        0        0     8147 2023-03-21 21:23:13.276190 thirdweb_sdk-3.0.3a0/thirdweb/abi/mock_contract.py
--rw-r--r--   0        0        0    43400 2023-03-21 21:23:13.276392 thirdweb_sdk-3.0.3a0/thirdweb/abi/mock_contract_publisher.py
--rw-r--r--   0        0        0     6634 2023-03-21 21:23:13.276550 thirdweb_sdk-3.0.3a0/thirdweb/abi/multicall.py
--rw-r--r--   0        0        0   188886 2023-03-21 21:23:13.277020 thirdweb_sdk-3.0.3a0/thirdweb/abi/multiwrap.py
--rw-r--r--   0        0        0   127828 2023-03-21 21:23:13.277343 thirdweb_sdk-3.0.3a0/thirdweb/abi/n_f_t_stake.py
--rw-r--r--   0        0        0    41556 2023-03-21 21:23:13.277556 thirdweb_sdk-3.0.3a0/thirdweb/abi/offers_logic.py
--rw-r--r--   0        0        0     5890 2023-03-21 21:23:13.277742 thirdweb_sdk-3.0.3a0/thirdweb/abi/offers_storage.py
--rw-r--r--   0        0        0     9837 2023-03-21 21:23:13.277906 thirdweb_sdk-3.0.3a0/thirdweb/abi/operator_filter_toggle.py
--rw-r--r--   0        0        0    12250 2023-03-21 21:23:13.278071 thirdweb_sdk-3.0.3a0/thirdweb/abi/operator_filterer.py
--rw-r--r--   0        0        0    10025 2023-03-21 21:23:13.278242 thirdweb_sdk-3.0.3a0/thirdweb/abi/operator_filterer_upgradeable.py
--rw-r--r--   0        0        0     9381 2023-03-21 21:23:13.278404 thirdweb_sdk-3.0.3a0/thirdweb/abi/ownable.py
--rw-r--r--   0        0        0   189507 2023-03-21 21:23:13.278843 thirdweb_sdk-3.0.3a0/thirdweb/abi/pack.py
--rw-r--r--   0        0        0   192431 2023-03-21 21:23:13.279296 thirdweb_sdk-3.0.3a0/thirdweb/abi/pack_v_r_f_direct.py
--rw-r--r--   0        0        0    42973 2023-03-21 21:23:13.279504 thirdweb_sdk-3.0.3a0/thirdweb/abi/payment_splitter_upgradeable.py
--rw-r--r--   0        0        0    29535 2023-03-21 21:23:13.279694 thirdweb_sdk-3.0.3a0/thirdweb/abi/permissions.py
--rw-r--r--   0        0        0    36480 2023-03-21 21:23:13.279895 thirdweb_sdk-3.0.3a0/thirdweb/abi/permissions_enumerable.py
--rw-r--r--   0        0        0    36540 2023-03-21 21:23:13.280089 thirdweb_sdk-3.0.3a0/thirdweb/abi/permissions_enumerable_logic.py
--rw-r--r--   0        0        0     6205 2023-03-21 21:23:13.280250 thirdweb_sdk-3.0.3a0/thirdweb/abi/permissions_enumerable_storage.py
--rw-r--r--   0        0        0    29595 2023-03-21 21:23:13.280415 thirdweb_sdk-3.0.3a0/thirdweb/abi/permissions_logic.py
--rw-r--r--   0        0        0     5980 2023-03-21 21:23:13.280568 thirdweb_sdk-3.0.3a0/thirdweb/abi/permissions_storage.py
--rw-r--r--   0        0        0    11336 2023-03-21 21:23:13.280726 thirdweb_sdk-3.0.3a0/thirdweb/abi/platform_fee.py
--rw-r--r--   0        0        0    11386 2023-03-21 21:23:13.280882 thirdweb_sdk-3.0.3a0/thirdweb/abi/platform_fee_logic.py
--rw-r--r--   0        0        0     5985 2023-03-21 21:23:13.281049 thirdweb_sdk-3.0.3a0/thirdweb/abi/platform_fee_storage.py
--rw-r--r--   0        0        0    15127 2023-03-21 21:23:13.281212 thirdweb_sdk-3.0.3a0/thirdweb/abi/plugin_map.py
--rw-r--r--   0        0        0     9970 2023-03-21 21:23:13.281363 thirdweb_sdk-3.0.3a0/thirdweb/abi/primary_sale.py
--rw-r--r--   0        0        0     3400 2023-03-21 21:23:13.281512 thirdweb_sdk-3.0.3a0/thirdweb/abi/proxy.py
--rw-r--r--   0        0        0     6116 2023-03-21 21:23:13.281669 thirdweb_sdk-3.0.3a0/thirdweb/abi/proxy_for_upgradeable.py
--rw-r--r--   0        0        0     3394 2023-03-21 21:23:13.281808 thirdweb_sdk-3.0.3a0/thirdweb/abi/reentrancy_guard.py
--rw-r--r--   0        0        0     3434 2023-03-21 21:23:13.281960 thirdweb_sdk-3.0.3a0/thirdweb/abi/reentrancy_guard_logic.py
--rw-r--r--   0        0        0     6097 2023-03-21 21:23:13.282103 thirdweb_sdk-3.0.3a0/thirdweb/abi/reentrancy_guard_storage.py
--rw-r--r--   0        0        0     4225 2023-03-21 21:23:13.282265 thirdweb_sdk-3.0.3a0/thirdweb/abi/reentrancy_guard_upgradeable.py
--rw-r--r--   0        0        0    38781 2023-03-21 21:23:13.282466 thirdweb_sdk-3.0.3a0/thirdweb/abi/router.py
--rw-r--r--   0        0        0    39070 2023-03-21 21:23:13.282675 thirdweb_sdk-3.0.3a0/thirdweb/abi/router_immutable.py
--rw-r--r--   0        0        0     5890 2023-03-21 21:23:13.282818 thirdweb_sdk-3.0.3a0/thirdweb/abi/router_storage.py
--rw-r--r--   0        0        0    27102 2023-03-21 21:23:13.282994 thirdweb_sdk-3.0.3a0/thirdweb/abi/royalty.py
--rw-r--r--   0        0        0     3308 2023-03-21 21:23:13.283141 thirdweb_sdk-3.0.3a0/thirdweb/abi/safe_cast.py
--rw-r--r--   0        0        0     3316 2023-03-21 21:23:13.283262 thirdweb_sdk-3.0.3a0/thirdweb/abi/safe_erc20.py
--rw-r--r--   0        0        0     3308 2023-03-21 21:23:13.283384 thirdweb_sdk-3.0.3a0/thirdweb/abi/safe_math.py
--rw-r--r--   0        0        0     9992 2023-03-21 21:23:13.283531 thirdweb_sdk-3.0.3a0/thirdweb/abi/signature_action.py
--rw-r--r--   0        0        0    10824 2023-03-21 21:23:13.283687 thirdweb_sdk-3.0.3a0/thirdweb/abi/signature_action_upgradeable.py
--rw-r--r--   0        0        0   231932 2023-03-21 21:23:13.284160 thirdweb_sdk-3.0.3a0/thirdweb/abi/signature_drop.py
--rw-r--r--   0        0        0    16142 2023-03-21 21:23:13.284389 thirdweb_sdk-3.0.3a0/thirdweb/abi/signature_mint_erc1155.py
--rw-r--r--   0        0        0    16979 2023-03-21 21:23:13.284556 thirdweb_sdk-3.0.3a0/thirdweb/abi/signature_mint_erc1155_upgradeable.py
--rw-r--r--   0        0        0    15148 2023-03-21 21:23:13.284777 thirdweb_sdk-3.0.3a0/thirdweb/abi/signature_mint_erc20.py
--rw-r--r--   0        0        0    15983 2023-03-21 21:23:13.284942 thirdweb_sdk-3.0.3a0/thirdweb/abi/signature_mint_erc20_upgradeable.py
--rw-r--r--   0        0        0    15917 2023-03-21 21:23:13.285134 thirdweb_sdk-3.0.3a0/thirdweb/abi/signature_mint_erc721.py
--rw-r--r--   0        0        0    16753 2023-03-21 21:23:13.285291 thirdweb_sdk-3.0.3a0/thirdweb/abi/signature_mint_erc721_upgradeable.py
--rw-r--r--   0        0        0   237737 2023-03-21 21:23:13.285730 thirdweb_sdk-3.0.3a0/thirdweb/abi/signaturedrop_v4.py
--rw-r--r--   0        0        0    42531 2023-03-21 21:23:13.285946 thirdweb_sdk-3.0.3a0/thirdweb/abi/soulbound_erc721_a.py
--rw-r--r--   0        0        0   101885 2023-03-21 21:23:13.286193 thirdweb_sdk-3.0.3a0/thirdweb/abi/split.py
--rw-r--r--   0        0        0    72420 2023-03-21 21:23:13.286430 thirdweb_sdk-3.0.3a0/thirdweb/abi/staking1155.py
--rw-r--r--   0        0        0   111245 2023-03-21 21:23:13.286697 thirdweb_sdk-3.0.3a0/thirdweb/abi/staking1155_base.py
--rw-r--r--   0        0        0    73314 2023-03-21 21:23:13.286919 thirdweb_sdk-3.0.3a0/thirdweb/abi/staking1155_upgradeable.py
--rw-r--r--   0        0        0    49004 2023-03-21 21:23:13.287115 thirdweb_sdk-3.0.3a0/thirdweb/abi/staking20.py
--rw-r--r--   0        0        0    72923 2023-03-21 21:23:13.287329 thirdweb_sdk-3.0.3a0/thirdweb/abi/staking20_base.py
--rw-r--r--   0        0        0    49928 2023-03-21 21:23:13.287516 thirdweb_sdk-3.0.3a0/thirdweb/abi/staking20_upgradeable.py
--rw-r--r--   0        0        0    50405 2023-03-21 21:23:13.287702 thirdweb_sdk-3.0.3a0/thirdweb/abi/staking721.py
--rw-r--r--   0        0        0    85256 2023-03-21 21:23:13.287922 thirdweb_sdk-3.0.3a0/thirdweb/abi/staking721_base.py
--rw-r--r--   0        0        0    51319 2023-03-21 21:23:13.288130 thirdweb_sdk-3.0.3a0/thirdweb/abi/staking721_upgradeable.py
--rw-r--r--   0        0        0     3316 2023-03-21 21:23:13.288248 thirdweb_sdk-3.0.3a0/thirdweb/abi/t_w_address.py
--rw-r--r--   0        0        0     3316 2023-03-21 21:23:13.288348 thirdweb_sdk-3.0.3a0/thirdweb/abi/t_w_bit_maps.py
--rw-r--r--   0        0        0    89887 2023-03-21 21:23:13.288497 thirdweb_sdk-3.0.3a0/thirdweb/abi/t_w_factory.py
--rw-r--r--   0        0        0    75523 2023-03-21 21:23:13.288703 thirdweb_sdk-3.0.3a0/thirdweb/abi/t_w_fee.py
--rw-r--r--   0        0        0    67405 2023-03-21 21:23:13.288905 thirdweb_sdk-3.0.3a0/thirdweb/abi/t_w_multichain_registry.py
--rw-r--r--   0        0        0    37213 2023-03-21 21:23:13.289082 thirdweb_sdk-3.0.3a0/thirdweb/abi/t_w_multichain_registry_logic.py
--rw-r--r--   0        0        0    75392 2023-03-21 21:23:13.289301 thirdweb_sdk-3.0.3a0/thirdweb/abi/t_w_multichain_registry_router.py
--rw-r--r--   0        0        0     6169 2023-03-21 21:23:13.289435 thirdweb_sdk-3.0.3a0/thirdweb/abi/t_w_multichain_registry_storage.py
--rw-r--r--   0        0        0     3738 2023-03-21 21:23:13.289536 thirdweb_sdk-3.0.3a0/thirdweb/abi/t_w_proxy.py
--rw-r--r--   0        0        0    59703 2023-03-21 21:23:13.289758 thirdweb_sdk-3.0.3a0/thirdweb/abi/t_w_registry.py
--rw-r--r--   0        0        0     3378 2023-03-21 21:23:13.289874 thirdweb_sdk-3.0.3a0/thirdweb/abi/t_w_storage_slot.py
--rw-r--r--   0        0        0     3316 2023-03-21 21:23:13.289982 thirdweb_sdk-3.0.3a0/thirdweb/abi/t_w_strings.py
--rw-r--r--   0        0        0   206242 2023-03-21 21:23:13.290372 thirdweb_sdk-3.0.3a0/thirdweb/abi/tiered_drop.py
--rw-r--r--   0        0        0    15273 2023-03-21 21:23:13.290500 thirdweb_sdk-3.0.3a0/thirdweb/abi/token_bundle.py
--rw-r--r--   0        0        0   182279 2023-03-21 21:23:13.290887 thirdweb_sdk-3.0.3a0/thirdweb/abi/token_erc1155.py
--rw-r--r--   0        0        0   176744 2023-03-21 21:23:13.291274 thirdweb_sdk-3.0.3a0/thirdweb/abi/token_erc20.py
--rw-r--r--   0        0        0   185235 2023-03-21 21:23:13.291683 thirdweb_sdk-3.0.3a0/thirdweb/abi/token_erc721.py
--rw-r--r--   0        0        0   118802 2023-03-21 21:23:13.291949 thirdweb_sdk-3.0.3a0/thirdweb/abi/token_stake.py
--rw-r--r--   0        0        0    35792 2023-03-21 21:23:13.292111 thirdweb_sdk-3.0.3a0/thirdweb/abi/token_store.py
--rw-r--r--   0        0        0    15519 2023-03-21 21:23:13.292243 thirdweb_sdk-3.0.3a0/thirdweb/abi/upgradeable.py
--rw-r--r--   0        0        0   180710 2023-03-21 21:23:13.292582 thirdweb_sdk-3.0.3a0/thirdweb/abi/vote_erc20.py
--rw-r--r--   0        0        0        0 2023-03-13 04:51:11.298098 thirdweb_sdk-3.0.3a0/thirdweb/common/__init__.py
--rw-r--r--   0        0        0     4797 2023-03-13 04:51:11.298195 thirdweb_sdk-3.0.3a0/thirdweb/common/claim_conditions.py
--rw-r--r--   0        0        0     4039 2023-03-13 04:51:11.298272 thirdweb_sdk-3.0.3a0/thirdweb/common/currency.py
--rw-r--r--   0        0        0     2706 2023-03-13 04:51:11.298342 thirdweb_sdk-3.0.3a0/thirdweb/common/error.py
--rw-r--r--   0        0        0     3962 2023-03-21 02:20:09.125984 thirdweb_sdk-3.0.3a0/thirdweb/common/feature_detection.py
--rw-r--r--   0        0        0     4696 2023-03-13 04:51:11.298476 thirdweb_sdk-3.0.3a0/thirdweb/common/marketplace.py
--rw-r--r--   0        0        0     4657 2023-03-13 04:51:11.298549 thirdweb_sdk-3.0.3a0/thirdweb/common/merkle_tree.py
--rw-r--r--   0        0        0     2699 2023-03-13 04:51:11.298625 thirdweb_sdk-3.0.3a0/thirdweb/common/nft.py
--rw-r--r--   0        0        0     1241 2023-03-13 04:51:11.298693 thirdweb_sdk-3.0.3a0/thirdweb/common/sign.py
--rw-r--r--   0        0        0      287 2023-03-13 04:51:11.298753 thirdweb_sdk-3.0.3a0/thirdweb/common/signature_minting.py
--rw-r--r--   0        0        0     2552 2023-03-13 04:51:11.298824 thirdweb_sdk-3.0.3a0/thirdweb/common/snapshots.py
--rw-r--r--   0        0        0        0 2023-03-13 04:51:11.298891 thirdweb_sdk-3.0.3a0/thirdweb/constants/__init__.py
--rw-r--r--   0        0        0     3044 2023-03-13 04:51:11.298995 thirdweb_sdk-3.0.3a0/thirdweb/constants/addresses.py
--rw-r--r--   0        0        0      284 2023-03-13 04:51:11.299055 thirdweb_sdk-3.0.3a0/thirdweb/constants/chains.py
--rw-r--r--   0        0        0      182 2023-03-13 04:51:11.299107 thirdweb_sdk-3.0.3a0/thirdweb/constants/contract.py
--rw-r--r--   0        0        0     2457 2023-03-13 04:51:11.299165 thirdweb_sdk-3.0.3a0/thirdweb/constants/currency.py
--rw-r--r--   0        0        0      190 2023-03-13 04:51:11.299216 thirdweb_sdk-3.0.3a0/thirdweb/constants/events.py
--rw-r--r--   0        0        0      983 2023-03-13 04:51:11.299284 thirdweb_sdk-3.0.3a0/thirdweb/constants/role.py
--rw-r--r--   0        0        0      544 2023-03-13 04:51:11.299350 thirdweb_sdk-3.0.3a0/thirdweb/constants/rpc.py
--rw-r--r--   0        0        0     1518 2023-03-13 04:51:11.299410 thirdweb_sdk-3.0.3a0/thirdweb/constants/urls.py
--rw-r--r--   0        0        0      254 2023-03-13 04:51:11.299504 thirdweb_sdk-3.0.3a0/thirdweb/contracts/__init__.py
--rw-r--r--   0        0        0     7736 2023-05-12 02:13:06.833075 thirdweb_sdk-3.0.3a0/thirdweb/contracts/custom.py
--rw-r--r--   0        0        0     7971 2023-05-10 23:38:42.149747 thirdweb_sdk-3.0.3a0/thirdweb/contracts/edition.py
--rw-r--r--   0        0        0     5889 2023-05-10 23:38:42.149973 thirdweb_sdk-3.0.3a0/thirdweb/contracts/edition_drop.py
--rw-r--r--   0        0        0     1680 2023-03-13 04:51:11.299821 thirdweb_sdk-3.0.3a0/thirdweb/contracts/maps.py
--rw-r--r--   0        0        0    12680 2023-05-10 23:38:42.150209 thirdweb_sdk-3.0.3a0/thirdweb/contracts/marketplace.py
--rw-r--r--   0        0        0    12283 2023-05-10 23:38:42.150430 thirdweb_sdk-3.0.3a0/thirdweb/contracts/multiwrap.py
--rw-r--r--   0        0        0     7480 2023-05-10 23:38:42.150645 thirdweb_sdk-3.0.3a0/thirdweb/contracts/nft_collection.py
--rw-r--r--   0        0        0     8288 2023-05-10 23:38:42.150854 thirdweb_sdk-3.0.3a0/thirdweb/contracts/nft_drop.py
--rw-r--r--   0        0        0     5889 2023-05-10 23:38:42.151061 thirdweb_sdk-3.0.3a0/thirdweb/contracts/token.py
--rw-r--r--   0        0        0       29 2023-03-13 04:51:11.300414 thirdweb_sdk-3.0.3a0/thirdweb/core/__init__.py
--rw-r--r--   0        0        0       54 2023-03-13 04:51:11.300500 thirdweb_sdk-3.0.3a0/thirdweb/core/auth/__init__.py
--rw-r--r--   0        0        0    13845 2023-03-13 04:51:11.300598 thirdweb_sdk-3.0.3a0/thirdweb/core/auth/wallet_authenticator.py
--rw-r--r--   0        0        0        0 2023-03-13 04:51:11.300659 thirdweb_sdk-3.0.3a0/thirdweb/core/classes/__init__.py
--rw-r--r--   0        0        0     1318 2023-03-21 22:42:36.159881 thirdweb_sdk-3.0.3a0/thirdweb/core/classes/base_contract.py
--rw-r--r--   0        0        0     4014 2023-03-13 04:51:11.300801 thirdweb_sdk-3.0.3a0/thirdweb/core/classes/contract_deployer.py
--rw-r--r--   0        0        0     3359 2023-03-23 03:04:29.207240 thirdweb_sdk-3.0.3a0/thirdweb/core/classes/contract_events.py
--rw-r--r--   0        0        0     2110 2023-03-24 01:37:36.263013 thirdweb_sdk-3.0.3a0/thirdweb/core/classes/contract_metadata.py
--rw-r--r--   0        0        0     1983 2023-03-24 01:37:36.263235 thirdweb_sdk-3.0.3a0/thirdweb/core/classes/contract_platform_fee.py
--rw-r--r--   0        0        0     4275 2023-03-24 01:37:36.263461 thirdweb_sdk-3.0.3a0/thirdweb/core/classes/contract_roles.py
--rw-r--r--   0        0        0     4231 2023-05-10 22:38:00.168091 thirdweb_sdk-3.0.3a0/thirdweb/core/classes/contract_royalty.py
--rw-r--r--   0        0        0     1388 2023-03-24 01:37:36.263947 thirdweb_sdk-3.0.3a0/thirdweb/core/classes/contract_sales.py
--rw-r--r--   0        0        0     6879 2023-05-10 23:38:42.151333 thirdweb_sdk-3.0.3a0/thirdweb/core/classes/contract_wrapper.py
--rw-r--r--   0        0        0     2361 2023-03-13 04:51:11.301333 thirdweb_sdk-3.0.3a0/thirdweb/core/classes/drop_claim_conditions.py
--rw-r--r--   0        0        0     2722 2023-03-13 04:51:11.301386 thirdweb_sdk-3.0.3a0/thirdweb/core/classes/drop_erc1155_claim_conditions.py
--rw-r--r--   0        0        0    24253 2023-03-24 02:09:56.316705 thirdweb_sdk-3.0.3a0/thirdweb/core/classes/erc_1155.py
--rw-r--r--   0        0        0     8047 2023-03-13 04:51:11.301549 thirdweb_sdk-3.0.3a0/thirdweb/core/classes/erc_1155_signature_minting.py
--rw-r--r--   0        0        0     5534 2023-03-23 03:00:03.895228 thirdweb_sdk-3.0.3a0/thirdweb/core/classes/erc_1155_standard.py
--rw-r--r--   0        0        0    11065 2023-03-24 01:37:36.264471 thirdweb_sdk-3.0.3a0/thirdweb/core/classes/erc_20.py
--rw-r--r--   0        0        0     6733 2023-03-13 04:51:11.301730 thirdweb_sdk-3.0.3a0/thirdweb/core/classes/erc_20_signature_minting.py
--rw-r--r--   0        0        0     6779 2023-03-23 03:00:03.895861 thirdweb_sdk-3.0.3a0/thirdweb/core/classes/erc_20_standard.py
--rw-r--r--   0        0        0    23244 2023-03-24 01:37:46.685537 thirdweb_sdk-3.0.3a0/thirdweb/core/classes/erc_721.py
--rw-r--r--   0        0        0     7822 2023-03-13 04:51:11.301886 thirdweb_sdk-3.0.3a0/thirdweb/core/classes/erc_721_signature_minting.py
--rw-r--r--   0        0        0     5646 2023-03-23 03:00:03.896556 thirdweb_sdk-3.0.3a0/thirdweb/core/classes/erc_721_standard.py
--rw-r--r--   0        0        0     6575 2023-03-13 04:51:11.301958 thirdweb_sdk-3.0.3a0/thirdweb/core/classes/factory.py
--rw-r--r--   0        0        0     9448 2023-05-10 23:38:42.151573 thirdweb_sdk-3.0.3a0/thirdweb/core/classes/ipfs_storage.py
--rw-r--r--   0        0        0    11102 2023-03-13 04:51:11.302151 thirdweb_sdk-3.0.3a0/thirdweb/core/classes/marketplace_auction.py
--rw-r--r--   0        0        0    12104 2023-03-13 04:51:11.302217 thirdweb_sdk-3.0.3a0/thirdweb/core/classes/marketplace_direct.py
--rw-r--r--   0        0        0     2764 2023-03-13 04:51:11.302278 thirdweb_sdk-3.0.3a0/thirdweb/core/classes/provider_handler.py
--rw-r--r--   0        0        0     1257 2023-03-13 04:51:11.302340 thirdweb_sdk-3.0.3a0/thirdweb/core/classes/registry.py
--rw-r--r--   0        0        0     4780 2023-03-13 04:51:11.302405 thirdweb_sdk-3.0.3a0/thirdweb/core/classes/sharded_merkle_tree.py
--rw-r--r--   0        0        0     3227 2023-03-13 04:51:11.302500 thirdweb_sdk-3.0.3a0/thirdweb/core/helpers/storage.py
--rw-r--r--   0        0        0     7739 2023-03-13 04:51:11.302575 thirdweb_sdk-3.0.3a0/thirdweb/core/sdk.py
--rw-r--r--   0        0        0      254 2023-03-13 04:51:11.302670 thirdweb_sdk-3.0.3a0/thirdweb/types/__init__.py
--rw-r--r--   0        0        0     1482 2023-03-13 04:51:11.302742 thirdweb_sdk-3.0.3a0/thirdweb/types/auth.py
--rw-r--r--   0        0        0     1836 2023-03-23 03:00:03.896883 thirdweb_sdk-3.0.3a0/thirdweb/types/contract.py
--rw-r--r--   0        0        0     3111 2023-03-13 04:51:11.302929 thirdweb_sdk-3.0.3a0/thirdweb/types/contracts/claim_conditions.py
--rw-r--r--   0        0        0     5664 2023-03-13 04:51:11.303002 thirdweb_sdk-3.0.3a0/thirdweb/types/contracts/signature.py
--rw-r--r--   0        0        0      528 2023-03-13 04:51:11.303061 thirdweb_sdk-3.0.3a0/thirdweb/types/currency.py
--rw-r--r--   0        0        0      578 2023-03-13 04:51:11.303126 thirdweb_sdk-3.0.3a0/thirdweb/types/events.py
--rw-r--r--   0        0        0     2519 2023-03-13 04:51:11.303186 thirdweb_sdk-3.0.3a0/thirdweb/types/marketplace.py
--rw-r--r--   0        0        0      945 2023-03-13 04:51:11.303247 thirdweb_sdk-3.0.3a0/thirdweb/types/multiwrap.py
--rw-r--r--   0        0        0     3574 2023-03-13 04:51:11.303318 thirdweb_sdk-3.0.3a0/thirdweb/types/nft.py
--rw-r--r--   0        0        0     1084 2023-03-13 04:51:11.303390 thirdweb_sdk-3.0.3a0/thirdweb/types/sdk.py
--rw-r--r--   0        0        0      329 2023-03-23 03:04:29.209187 thirdweb_sdk-3.0.3a0/thirdweb/types/settings/__init__.py
--rw-r--r--   0        0        0     4111 2023-03-13 04:51:11.303569 thirdweb_sdk-3.0.3a0/thirdweb/types/settings/metadata.py
--rw-r--r--   0        0        0      215 2023-03-13 04:51:11.303629 thirdweb_sdk-3.0.3a0/thirdweb/types/storage.py
--rw-r--r--   0        0        0      334 2023-03-13 04:51:11.303692 thirdweb_sdk-3.0.3a0/thirdweb/types/tx.py
--rw-r--r--   0        0        0     6696 1970-01-01 00:00:00.000000 thirdweb_sdk-3.0.3a0/PKG-INFO
+-rw-r--r--   0        0        0    10942 2023-03-13 04:51:11.285705 thirdweb_sdk-3.1.0a0/LICENSE
+-rw-r--r--   0        0        0     6440 2023-07-18 18:53:20.930778 thirdweb_sdk-3.1.0a0/README.md
+-rw-r--r--   0        0        0     2644 2023-07-18 19:29:42.377863 thirdweb_sdk-3.1.0a0/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-03-13 04:51:11.293180 thirdweb_sdk-3.1.0a0/thirdweb/.DS_Store
+-rw-r--r--   0        0        0       30 2023-03-13 04:51:11.293237 thirdweb_sdk-3.1.0a0/thirdweb/__init__.py
+-rw-r--r--   0        0        0    20818 2023-03-21 21:23:13.236831 thirdweb_sdk-3.1.0a0/thirdweb/abi/__init__.py
+-rw-r--r--   0        0        0    85792 2023-03-21 21:23:13.237140 thirdweb_sdk-3.1.0a0/thirdweb/abi/airdrop_erc1155.py
+-rw-r--r--   0        0        0    68008 2023-03-21 21:23:13.237423 thirdweb_sdk-3.1.0a0/thirdweb/abi/airdrop_erc1155_claimable.py
+-rw-r--r--   0        0        0    80026 2023-03-21 21:23:13.237714 thirdweb_sdk-3.1.0a0/thirdweb/abi/airdrop_erc20.py
+-rw-r--r--   0        0        0    59394 2023-03-21 21:23:13.237980 thirdweb_sdk-3.1.0a0/thirdweb/abi/airdrop_erc20_claimable.py
+-rw-r--r--   0        0        0    80078 2023-03-21 21:23:13.238277 thirdweb_sdk-3.1.0a0/thirdweb/abi/airdrop_erc721.py
+-rw-r--r--   0        0        0    64449 2023-03-21 21:23:13.238530 thirdweb_sdk-3.1.0a0/thirdweb/abi/airdrop_erc721_claimable.py
+-rw-r--r--   0        0        0     9165 2023-03-21 21:23:13.238692 thirdweb_sdk-3.1.0a0/thirdweb/abi/app_u_r_i.py
+-rw-r--r--   0        0        0     8936 2023-03-21 21:23:13.238839 thirdweb_sdk-3.1.0a0/thirdweb/abi/batch_mint_metadata.py
+-rw-r--r--   0        0        0     3300 2023-03-21 21:23:13.238969 thirdweb_sdk-3.1.0a0/thirdweb/abi/context.py
+-rw-r--r--   0        0        0     9470 2023-03-21 21:23:13.239125 thirdweb_sdk-3.1.0a0/thirdweb/abi/contract_metadata.py
+-rw-r--r--   0        0        0     9520 2023-03-21 21:23:13.239295 thirdweb_sdk-3.1.0a0/thirdweb/abi/contract_metadata_logic.py
+-rw-r--r--   0        0        0     6115 2023-03-21 21:23:13.239442 thirdweb_sdk-3.1.0a0/thirdweb/abi/contract_metadata_storage.py
+-rw-r--r--   0        0        0    90485 2023-03-21 21:23:13.239903 thirdweb_sdk-3.1.0a0/thirdweb/abi/contract_publisher.py
+-rw-r--r--   0        0        0     3308 2023-03-21 21:23:13.240119 thirdweb_sdk-3.1.0a0/thirdweb/abi/counters.py
+-rw-r--r--   0        0        0     5790 2023-03-21 21:23:13.240283 thirdweb_sdk-3.1.0a0/thirdweb/abi/currency_transfer_lib.py
+-rw-r--r--   0        0        0    12320 2023-03-21 21:23:13.240459 thirdweb_sdk-3.1.0a0/thirdweb/abi/default_operator_filterer.py
+-rw-r--r--   0        0        0    10109 2023-03-21 21:23:13.240627 thirdweb_sdk-3.1.0a0/thirdweb/abi/default_operator_filterer_upgradeable.py
+-rw-r--r--   0        0        0    21950 2023-03-21 21:23:13.240845 thirdweb_sdk-3.1.0a0/thirdweb/abi/delayed_reveal.py
+-rw-r--r--   0        0        0    76514 2023-03-21 21:23:13.241162 thirdweb_sdk-3.1.0a0/thirdweb/abi/direct_listings_logic.py
+-rw-r--r--   0        0        0     6079 2023-03-21 21:23:13.241334 thirdweb_sdk-3.1.0a0/thirdweb/abi/direct_listings_storage.py
+-rw-r--r--   0        0        0    41239 2023-03-21 21:23:13.241551 thirdweb_sdk-3.1.0a0/thirdweb/abi/drop.py
+-rw-r--r--   0        0        0    46630 2023-03-21 21:23:13.241777 thirdweb_sdk-3.1.0a0/thirdweb/abi/drop1155.py
+-rw-r--r--   0        0        0   229869 2023-03-21 21:23:13.242485 thirdweb_sdk-3.1.0a0/thirdweb/abi/drop_erc1155.py
+-rw-r--r--   0        0        0   206478 2023-03-21 21:23:13.243046 thirdweb_sdk-3.1.0a0/thirdweb/abi/drop_erc20.py
+-rw-r--r--   0        0        0   243271 2023-03-21 21:23:13.243687 thirdweb_sdk-3.1.0a0/thirdweb/abi/drop_erc721.py
+-rw-r--r--   0        0        0    33157 2023-03-21 21:23:13.243907 thirdweb_sdk-3.1.0a0/thirdweb/abi/drop_single_phase.py
+-rw-r--r--   0        0        0    37416 2023-03-21 21:23:13.244123 thirdweb_sdk-3.1.0a0/thirdweb/abi/drop_single_phase1155.py
+-rw-r--r--   0        0        0   241058 2023-03-21 21:23:13.244635 thirdweb_sdk-3.1.0a0/thirdweb/abi/droperc1155_v2.py
+-rw-r--r--   0        0        0   226555 2023-03-21 21:23:13.245160 thirdweb_sdk-3.1.0a0/thirdweb/abi/droperc20_v2.py
+-rw-r--r--   0        0        0   249102 2023-03-21 21:23:13.245721 thirdweb_sdk-3.1.0a0/thirdweb/abi/droperc721_v3.py
+-rw-r--r--   0        0        0    43296 2023-03-21 21:23:13.245944 thirdweb_sdk-3.1.0a0/thirdweb/abi/dropsinglephase1155_v1.py
+-rw-r--r--   0        0        0    38914 2023-03-21 21:23:13.246156 thirdweb_sdk-3.1.0a0/thirdweb/abi/dropsinglephase_v1.py
+-rw-r--r--   0        0        0     3442 2023-03-21 21:23:13.246326 thirdweb_sdk-3.1.0a0/thirdweb/abi/e_i_p712_chainless_domain.py
+-rw-r--r--   0        0        0     3284 2023-03-21 21:23:13.246467 thirdweb_sdk-3.1.0a0/thirdweb/abi/ecdsa.py
+-rw-r--r--   0        0        0   156536 2023-03-21 21:23:13.246871 thirdweb_sdk-3.1.0a0/thirdweb/abi/edition_stake.py
+-rw-r--r--   0        0        0     3292 2023-03-21 21:23:13.247008 thirdweb_sdk-3.1.0a0/thirdweb/abi/eip712.py
+-rw-r--r--   0        0        0    64754 2023-03-21 21:23:13.247249 thirdweb_sdk-3.1.0a0/thirdweb/abi/english_auctions_logic.py
+-rw-r--r--   0        0        0     6097 2023-03-21 21:23:13.247424 thirdweb_sdk-3.1.0a0/thirdweb/abi/english_auctions_storage.py
+-rw-r--r--   0        0        0     3378 2023-03-21 21:23:13.247600 thirdweb_sdk-3.1.0a0/thirdweb/abi/enumerable_set.py
+-rw-r--r--   0        0        0    43189 2023-03-21 21:23:13.247814 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc1155.py
+-rw-r--r--   0        0        0   115583 2023-03-21 21:23:13.248175 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc1155_base.py
+-rw-r--r--   0        0        0   139620 2023-03-21 21:23:13.248544 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc1155_delayed_reveal.py
+-rw-r--r--   0        0        0   170049 2023-03-21 21:23:13.248978 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc1155_drop.py
+-rw-r--r--   0        0        0    18760 2023-03-21 21:23:13.249150 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc1155_holder.py
+-rw-r--r--   0        0        0   121380 2023-03-21 21:23:13.249486 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc1155_lazy_mint.py
+-rw-r--r--   0        0        0   112914 2023-03-21 21:23:13.249801 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc1155_preset_upgradeable.py
+-rw-r--r--   0        0        0    18357 2023-03-21 21:23:13.249969 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc1155_receiver.py
+-rw-r--r--   0        0        0   134633 2023-03-21 21:23:13.250319 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc1155_signature_mint.py
+-rw-r--r--   0        0        0     6858 2023-03-21 21:23:13.250859 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc165.py
+-rw-r--r--   0        0        0     6039 2023-03-21 21:23:13.251003 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc1967_proxy.py
+-rw-r--r--   0        0        0     5644 2023-03-21 21:23:13.251135 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc1967_upgrade.py
+-rw-r--r--   0        0        0    39698 2023-03-21 21:23:13.251312 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc20.py
+-rw-r--r--   0        0        0    72167 2023-03-21 21:23:13.251539 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc20_base.py
+-rw-r--r--   0        0        0   104921 2023-03-21 21:23:13.251834 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc20_drop.py
+-rw-r--r--   0        0        0   136778 2023-03-21 21:23:13.252201 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc20_drop_vote.py
+-rw-r--r--   0        0        0    50917 2023-03-21 21:23:13.252406 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc20_permit.py
+-rw-r--r--   0        0        0    90382 2023-03-21 21:23:13.252677 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc20_signature_mint.py
+-rw-r--r--   0        0        0   122210 2023-03-21 21:23:13.253003 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc20_signature_mint_vote.py
+-rw-r--r--   0        0        0   103909 2023-03-21 21:23:13.253295 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc20_vote.py
+-rw-r--r--   0        0        0    82607 2023-03-21 21:23:13.253572 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc20_votes.py
+-rw-r--r--   0        0        0     6811 2023-03-21 21:23:13.253736 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc2771_context.py
+-rw-r--r--   0        0        0     7980 2023-03-21 21:23:13.253881 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc2771_context_consumer.py
+-rw-r--r--   0        0        0     6856 2023-03-21 21:23:13.254037 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc2771_context_logic.py
+-rw-r--r--   0        0        0     6079 2023-03-21 21:23:13.254191 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc2771_context_storage.py
+-rw-r--r--   0        0        0     7631 2023-03-21 21:23:13.254332 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc2771_context_upgradeable.py
+-rw-r--r--   0        0        0     6955 2023-03-21 21:23:13.254489 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc2771_context_upgradeable_logic.py
+-rw-r--r--   0        0        0     6282 2023-03-21 21:23:13.254610 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc2771_context_upgradeable_storage.py
+-rw-r--r--   0        0        0    53696 2023-03-21 21:23:13.254828 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc721_a_upgradeable.py
+-rw-r--r--   0        0        0   119717 2023-03-21 21:23:13.255136 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc721_base.py
+-rw-r--r--   0        0        0   142298 2023-03-21 21:23:13.255489 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc721_delayed_reveal.py
+-rw-r--r--   0        0        0   169717 2023-03-21 21:23:13.255907 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc721_drop.py
+-rw-r--r--   0        0        0     8931 2023-03-21 21:23:13.256062 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc721_holder.py
+-rw-r--r--   0        0        0   124064 2023-03-21 21:23:13.256406 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc721_lazy_mint.py
+-rw-r--r--   0        0        0   182421 2023-03-21 21:23:13.256821 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc721_multiwrap.py
+-rw-r--r--   0        0        0   138584 2023-03-21 21:23:13.257156 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc721_signature_mint.py
+-rw-r--r--   0        0        0    52988 2023-03-21 21:23:13.257362 thirdweb_sdk-3.1.0a0/thirdweb/abi/erc721a.py
+-rw-r--r--   0        0        0     3300 2023-03-21 21:23:13.257494 thirdweb_sdk-3.1.0a0/thirdweb/abi/fee_type.py
+-rw-r--r--   0        0        0    11166 2023-03-21 21:23:13.257651 thirdweb_sdk-3.1.0a0/thirdweb/abi/forwarder_consumer.py
+-rw-r--r--   0        0        0    26106 2023-03-21 21:23:13.257810 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_airdrop_erc1155.py
+-rw-r--r--   0        0        0    10788 2023-03-21 21:23:13.257985 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_airdrop_erc1155_claimable.py
+-rw-r--r--   0        0        0    25450 2023-03-21 21:23:13.258153 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_airdrop_erc20.py
+-rw-r--r--   0        0        0    10033 2023-03-21 21:23:13.258293 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_airdrop_erc20_claimable.py
+-rw-r--r--   0        0        0    25497 2023-03-21 21:23:13.258455 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_airdrop_erc721.py
+-rw-r--r--   0        0        0    10043 2023-03-21 21:23:13.258592 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_airdrop_erc721_claimable.py
+-rw-r--r--   0        0        0     9175 2023-03-21 21:23:13.258726 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_app_u_r_i.py
+-rw-r--r--   0        0        0     5661 2023-03-21 21:23:13.258854 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_beacon.py
+-rw-r--r--   0        0        0    11588 2023-03-21 21:23:13.258998 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_burnable_erc1155.py
+-rw-r--r--   0        0        0     9891 2023-03-21 21:23:13.259133 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_burnable_erc20.py
+-rw-r--r--   0        0        0     6533 2023-03-21 21:23:13.259256 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_burnable_erc721.py
+-rw-r--r--   0        0        0     3394 2023-03-21 21:23:13.259376 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_claim_condition.py
+-rw-r--r--   0        0        0     3474 2023-03-21 21:23:13.259510 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_claim_condition_multi_phase.py
+-rw-r--r--   0        0        0    10930 2023-03-21 21:23:13.259648 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_claim_conditions_single_phase.py
+-rw-r--r--   0        0        0    13127 2023-03-21 21:23:13.259788 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_claimable_erc1155.py
+-rw-r--r--   0        0        0    11876 2023-03-21 21:23:13.259913 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_claimable_erc721.py
+-rw-r--r--   0        0        0     7811 2023-03-21 21:23:13.260053 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_context.py
+-rw-r--r--   0        0        0    23449 2023-03-21 21:23:13.260235 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_contract_deployer.py
+-rw-r--r--   0        0        0     8413 2023-03-21 21:23:13.260387 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_contract_factory.py
+-rw-r--r--   0        0        0     9480 2023-03-21 21:23:13.260521 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_contract_metadata.py
+-rw-r--r--   0        0        0    44219 2023-03-21 21:23:13.260712 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_contract_publisher.py
+-rw-r--r--   0        0        0    11835 2023-03-21 21:23:13.260853 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_delayed_reveal.py
+-rw-r--r--   0        0        0    15264 2023-03-21 21:23:13.260989 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_delayed_reveal_deprecated.py
+-rw-r--r--   0        0        0    57624 2023-03-21 21:23:13.261211 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_direct_listings.py
+-rw-r--r--   0        0        0    20142 2023-03-21 21:23:13.261365 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_drop.py
+-rw-r--r--   0        0        0    21722 2023-03-21 21:23:13.261543 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_drop1155.py
+-rw-r--r--   0        0        0     3426 2023-03-21 21:23:13.261696 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_drop_claim_condition.py
+-rw-r--r--   0        0        0    60183 2023-03-21 21:23:13.261901 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_drop_erc1155.py
+-rw-r--r--   0        0        0    43180 2023-03-21 21:23:13.262090 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_drop_erc20.py
+-rw-r--r--   0        0        0    66414 2023-03-21 21:23:13.262347 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_drop_erc721.py
+-rw-r--r--   0        0        0    20224 2023-03-21 21:23:13.262510 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_drop_single_phase.py
+-rw-r--r--   0        0        0    21804 2023-03-21 21:23:13.262667 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_drop_single_phase1155.py
+-rw-r--r--   0        0        0    11373 2023-03-21 21:23:13.262807 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_edition_stake.py
+-rw-r--r--   0        0        0    55894 2023-03-21 21:23:13.263009 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_english_auctions.py
+-rw-r--r--   0        0        0     5838 2023-03-21 21:23:13.263163 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_erc1155_enumerable.py
+-rw-r--r--   0        0        0     6466 2023-03-21 21:23:13.263300 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_erc1155_metadata.py
+-rw-r--r--   0        0        0    18366 2023-03-21 21:23:13.263446 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_erc1155_receiver.py
+-rw-r--r--   0        0        0     6575 2023-03-21 21:23:13.263588 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_erc1155_supply.py
+-rw-r--r--   0        0        0     5815 2023-03-21 21:23:13.263713 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_erc1822_proxiable.py
+-rw-r--r--   0        0        0     9937 2023-03-21 21:23:13.263831 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_erc20_metadata.py
+-rw-r--r--   0        0        0    14843 2023-03-21 21:23:13.263957 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_erc20_permit.py
+-rw-r--r--   0        0        0     6820 2023-03-21 21:23:13.264083 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_erc2771_context.py
+-rw-r--r--   0        0        0    10336 2023-03-21 21:23:13.264227 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_erc721_enumerable.py
+-rw-r--r--   0        0        0    10879 2023-03-21 21:23:13.264362 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_erc721_metadata.py
+-rw-r--r--   0        0        0     8622 2023-03-21 21:23:13.264491 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_erc721_receiver.py
+-rw-r--r--   0        0        0     5733 2023-03-21 21:23:13.264619 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_erc721_supply.py
+-rw-r--r--   0        0        0     7383 2023-03-21 21:23:13.264746 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_fee_tier_placement_extension.py
+-rw-r--r--   0        0        0     9333 2023-03-21 21:23:13.264861 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_lazy_mint.py
+-rw-r--r--   0        0        0     9955 2023-03-21 21:23:13.264991 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_lazy_mint_with_tier.py
+-rw-r--r--   0        0        0    68265 2023-03-21 21:23:13.265206 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_marketplace.py
+-rw-r--r--   0        0        0     8961 2023-03-21 21:23:13.265364 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_mintable_erc1155.py
+-rw-r--r--   0        0        0     7682 2023-03-21 21:23:13.265488 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_mintable_erc20.py
+-rw-r--r--   0        0        0     7691 2023-03-21 21:23:13.265603 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_mintable_erc721.py
+-rw-r--r--   0        0        0     6643 2023-03-21 21:23:13.265712 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_multicall.py
+-rw-r--r--   0        0        0    15555 2023-03-21 21:23:13.265837 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_multiwrap.py
+-rw-r--r--   0        0        0    11286 2023-03-21 21:23:13.265950 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_n_f_t_stake.py
+-rw-r--r--   0        0        0    32749 2023-03-21 21:23:13.266098 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_offers.py
+-rw-r--r--   0        0        0    94730 2023-03-21 21:23:13.266342 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_operator_filter_registry.py
+-rw-r--r--   0        0        0     9845 2023-03-21 21:23:13.266490 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_operator_filter_toggle.py
+-rw-r--r--   0        0        0     9391 2023-03-21 21:23:13.266630 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_ownable.py
+-rw-r--r--   0        0        0    19897 2023-03-21 21:23:13.266769 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_pack.py
+-rw-r--r--   0        0        0    31414 2023-03-21 21:23:13.266928 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_pack_v_r_f_direct.py
+-rw-r--r--   0        0        0    23527 2023-03-21 21:23:13.267072 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_permissions.py
+-rw-r--r--   0        0        0    30461 2023-03-21 21:23:13.267260 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_permissions_enumerable.py
+-rw-r--r--   0        0        0    11346 2023-03-21 21:23:13.267463 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_platform_fee.py
+-rw-r--r--   0        0        0    15146 2023-03-21 21:23:13.267593 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_plugin_map.py
+-rw-r--r--   0        0        0     9980 2023-03-21 21:23:13.267723 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_primary_sale.py
+-rw-r--r--   0        0        0    27471 2023-03-21 21:23:13.267868 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_router.py
+-rw-r--r--   0        0        0    27105 2023-03-21 21:23:13.268058 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_royalty.py
+-rw-r--r--   0        0        0     9998 2023-03-21 21:23:13.268194 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_signature_action.py
+-rw-r--r--   0        0        0    16148 2023-03-21 21:23:13.268332 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_signature_mint_erc1155.py
+-rw-r--r--   0        0        0    15154 2023-03-21 21:23:13.268485 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_signature_mint_erc20.py
+-rw-r--r--   0        0        0    15923 2023-03-21 21:23:13.268633 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_signature_mint_erc721.py
+-rw-r--r--   0        0        0    27313 2023-03-21 21:23:13.268779 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_staking1155.py
+-rw-r--r--   0        0        0    19685 2023-03-21 21:23:13.268918 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_staking20.py
+-rw-r--r--   0        0        0    18920 2023-03-21 21:23:13.269054 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_staking721.py
+-rw-r--r--   0        0        0     7095 2023-03-21 21:23:13.269185 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_t_w_fee.py
+-rw-r--r--   0        0        0    26206 2023-03-21 21:23:13.269336 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_t_w_multichain_registry.py
+-rw-r--r--   0        0        0    21103 2023-03-21 21:23:13.269504 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_t_w_registry.py
+-rw-r--r--   0        0        0    13067 2023-03-21 21:23:13.269651 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_thirdweb_contract.py
+-rw-r--r--   0        0        0     3370 2023-03-21 21:23:13.269761 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_token_bundle.py
+-rw-r--r--   0        0        0    53182 2023-03-21 21:23:13.270402 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_token_erc1155.py
+-rw-r--r--   0        0        0    46867 2023-03-21 21:23:13.270660 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_token_erc20.py
+-rw-r--r--   0        0        0    58484 2023-03-21 21:23:13.271450 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_token_erc721.py
+-rw-r--r--   0        0        0    11351 2023-03-21 21:23:13.271592 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_token_stake.py
+-rw-r--r--   0        0        0    27443 2023-03-21 21:23:13.271753 thirdweb_sdk-3.1.0a0/thirdweb/abi/i_votes.py
+-rw-r--r--   0        0        0     3418 2023-03-21 21:23:13.271870 thirdweb_sdk-3.1.0a0/thirdweb/abi/iclaimcondition_v1.py
+-rw-r--r--   0        0        0     3450 2023-03-21 21:23:13.271980 thirdweb_sdk-3.1.0a0/thirdweb/abi/idropclaimcondition_v2.py
+-rw-r--r--   0        0        0    61520 2023-03-21 21:23:13.272188 thirdweb_sdk-3.1.0a0/thirdweb/abi/idroperc1155_v2.py
+-rw-r--r--   0        0        0    44262 2023-03-21 21:23:13.272388 thirdweb_sdk-3.1.0a0/thirdweb/abi/idroperc20_v2.py
+-rw-r--r--   0        0        0    67599 2023-03-21 21:23:13.272611 thirdweb_sdk-3.1.0a0/thirdweb/abi/idroperc721_v3.py
+-rw-r--r--   0        0        0    21795 2023-03-21 21:23:13.272779 thirdweb_sdk-3.1.0a0/thirdweb/abi/idropsinglephase1155_v1.py
+-rw-r--r--   0        0        0    20215 2023-03-21 21:23:13.272932 thirdweb_sdk-3.1.0a0/thirdweb/abi/idropsinglephase_v1.py
+-rw-r--r--   0        0        0    31974 2023-03-21 21:23:13.273101 thirdweb_sdk-3.1.0a0/thirdweb/abi/ierc1155.py
+-rw-r--r--   0        0        0     6867 2023-03-21 21:23:13.273333 thirdweb_sdk-3.1.0a0/thirdweb/abi/ierc165.py
+-rw-r--r--   0        0        0    24799 2023-03-21 21:23:13.273460 thirdweb_sdk-3.1.0a0/thirdweb/abi/ierc20.py
+-rw-r--r--   0        0        0    10953 2023-03-21 21:23:13.273598 thirdweb_sdk-3.1.0a0/thirdweb/abi/ierc2981.py
+-rw-r--r--   0        0        0    39092 2023-03-21 21:23:13.273809 thirdweb_sdk-3.1.0a0/thirdweb/abi/ierc721.py
+-rw-r--r--   0        0        0    49418 2023-03-21 21:23:13.274000 thirdweb_sdk-3.1.0a0/thirdweb/abi/ierc721a.py
+-rw-r--r--   0        0        0     3362 2023-03-21 21:23:13.274132 thirdweb_sdk-3.1.0a0/thirdweb/abi/init_storage.py
+-rw-r--r--   0        0        0     4108 2023-03-21 21:23:13.274281 thirdweb_sdk-3.1.0a0/thirdweb/abi/initializable.py
+-rw-r--r--   0        0        0    13842 2023-03-21 21:23:13.274439 thirdweb_sdk-3.1.0a0/thirdweb/abi/isignatureminterc721_v1.py
+-rw-r--r--   0        0        0    11782 2023-03-21 21:23:13.274565 thirdweb_sdk-3.1.0a0/thirdweb/abi/iweth.py
+-rw-r--r--   0        0        0    14519 2023-03-21 21:23:13.274700 thirdweb_sdk-3.1.0a0/thirdweb/abi/lazy_mint.py
+-rw-r--r--   0        0        0    19969 2023-03-21 21:23:13.274856 thirdweb_sdk-3.1.0a0/thirdweb/abi/lazy_mint_with_tier.py
+-rw-r--r--   0        0        0   156959 2023-03-21 21:23:13.275265 thirdweb_sdk-3.1.0a0/thirdweb/abi/marketplace.py
+-rw-r--r--   0        0        0   117081 2023-03-21 21:23:13.275601 thirdweb_sdk-3.1.0a0/thirdweb/abi/marketplace_v3.py
+-rw-r--r--   0        0        0     3276 2023-03-21 21:23:13.275761 thirdweb_sdk-3.1.0a0/thirdweb/abi/math.py
+-rw-r--r--   0        0        0     3362 2023-03-21 21:23:13.275902 thirdweb_sdk-3.1.0a0/thirdweb/abi/merkle_proof.py
+-rw-r--r--   0        0        0     9839 2023-03-21 21:23:13.276042 thirdweb_sdk-3.1.0a0/thirdweb/abi/mock.py
+-rw-r--r--   0        0        0     8147 2023-03-21 21:23:13.276190 thirdweb_sdk-3.1.0a0/thirdweb/abi/mock_contract.py
+-rw-r--r--   0        0        0    43400 2023-03-21 21:23:13.276392 thirdweb_sdk-3.1.0a0/thirdweb/abi/mock_contract_publisher.py
+-rw-r--r--   0        0        0     6634 2023-03-21 21:23:13.276550 thirdweb_sdk-3.1.0a0/thirdweb/abi/multicall.py
+-rw-r--r--   0        0        0   188886 2023-03-21 21:23:13.277020 thirdweb_sdk-3.1.0a0/thirdweb/abi/multiwrap.py
+-rw-r--r--   0        0        0   127828 2023-03-21 21:23:13.277343 thirdweb_sdk-3.1.0a0/thirdweb/abi/n_f_t_stake.py
+-rw-r--r--   0        0        0    41556 2023-03-21 21:23:13.277556 thirdweb_sdk-3.1.0a0/thirdweb/abi/offers_logic.py
+-rw-r--r--   0        0        0     5890 2023-03-21 21:23:13.277742 thirdweb_sdk-3.1.0a0/thirdweb/abi/offers_storage.py
+-rw-r--r--   0        0        0     9837 2023-03-21 21:23:13.277906 thirdweb_sdk-3.1.0a0/thirdweb/abi/operator_filter_toggle.py
+-rw-r--r--   0        0        0    12250 2023-03-21 21:23:13.278071 thirdweb_sdk-3.1.0a0/thirdweb/abi/operator_filterer.py
+-rw-r--r--   0        0        0    10025 2023-03-21 21:23:13.278242 thirdweb_sdk-3.1.0a0/thirdweb/abi/operator_filterer_upgradeable.py
+-rw-r--r--   0        0        0     9381 2023-03-21 21:23:13.278404 thirdweb_sdk-3.1.0a0/thirdweb/abi/ownable.py
+-rw-r--r--   0        0        0   189507 2023-03-21 21:23:13.278843 thirdweb_sdk-3.1.0a0/thirdweb/abi/pack.py
+-rw-r--r--   0        0        0   192431 2023-03-21 21:23:13.279296 thirdweb_sdk-3.1.0a0/thirdweb/abi/pack_v_r_f_direct.py
+-rw-r--r--   0        0        0    42973 2023-03-21 21:23:13.279504 thirdweb_sdk-3.1.0a0/thirdweb/abi/payment_splitter_upgradeable.py
+-rw-r--r--   0        0        0    29535 2023-03-21 21:23:13.279694 thirdweb_sdk-3.1.0a0/thirdweb/abi/permissions.py
+-rw-r--r--   0        0        0    36480 2023-03-21 21:23:13.279895 thirdweb_sdk-3.1.0a0/thirdweb/abi/permissions_enumerable.py
+-rw-r--r--   0        0        0    36540 2023-03-21 21:23:13.280089 thirdweb_sdk-3.1.0a0/thirdweb/abi/permissions_enumerable_logic.py
+-rw-r--r--   0        0        0     6205 2023-03-21 21:23:13.280250 thirdweb_sdk-3.1.0a0/thirdweb/abi/permissions_enumerable_storage.py
+-rw-r--r--   0        0        0    29595 2023-03-21 21:23:13.280415 thirdweb_sdk-3.1.0a0/thirdweb/abi/permissions_logic.py
+-rw-r--r--   0        0        0     5980 2023-03-21 21:23:13.280568 thirdweb_sdk-3.1.0a0/thirdweb/abi/permissions_storage.py
+-rw-r--r--   0        0        0    11336 2023-03-21 21:23:13.280726 thirdweb_sdk-3.1.0a0/thirdweb/abi/platform_fee.py
+-rw-r--r--   0        0        0    11386 2023-03-21 21:23:13.280882 thirdweb_sdk-3.1.0a0/thirdweb/abi/platform_fee_logic.py
+-rw-r--r--   0        0        0     5985 2023-03-21 21:23:13.281049 thirdweb_sdk-3.1.0a0/thirdweb/abi/platform_fee_storage.py
+-rw-r--r--   0        0        0    15127 2023-03-21 21:23:13.281212 thirdweb_sdk-3.1.0a0/thirdweb/abi/plugin_map.py
+-rw-r--r--   0        0        0     9970 2023-03-21 21:23:13.281363 thirdweb_sdk-3.1.0a0/thirdweb/abi/primary_sale.py
+-rw-r--r--   0        0        0     3400 2023-03-21 21:23:13.281512 thirdweb_sdk-3.1.0a0/thirdweb/abi/proxy.py
+-rw-r--r--   0        0        0     6116 2023-03-21 21:23:13.281669 thirdweb_sdk-3.1.0a0/thirdweb/abi/proxy_for_upgradeable.py
+-rw-r--r--   0        0        0     3394 2023-03-21 21:23:13.281808 thirdweb_sdk-3.1.0a0/thirdweb/abi/reentrancy_guard.py
+-rw-r--r--   0        0        0     3434 2023-03-21 21:23:13.281960 thirdweb_sdk-3.1.0a0/thirdweb/abi/reentrancy_guard_logic.py
+-rw-r--r--   0        0        0     6097 2023-03-21 21:23:13.282103 thirdweb_sdk-3.1.0a0/thirdweb/abi/reentrancy_guard_storage.py
+-rw-r--r--   0        0        0     4225 2023-03-21 21:23:13.282265 thirdweb_sdk-3.1.0a0/thirdweb/abi/reentrancy_guard_upgradeable.py
+-rw-r--r--   0        0        0    38781 2023-03-21 21:23:13.282466 thirdweb_sdk-3.1.0a0/thirdweb/abi/router.py
+-rw-r--r--   0        0        0    39070 2023-03-21 21:23:13.282675 thirdweb_sdk-3.1.0a0/thirdweb/abi/router_immutable.py
+-rw-r--r--   0        0        0     5890 2023-03-21 21:23:13.282818 thirdweb_sdk-3.1.0a0/thirdweb/abi/router_storage.py
+-rw-r--r--   0        0        0    27102 2023-03-21 21:23:13.282994 thirdweb_sdk-3.1.0a0/thirdweb/abi/royalty.py
+-rw-r--r--   0        0        0     3308 2023-03-21 21:23:13.283141 thirdweb_sdk-3.1.0a0/thirdweb/abi/safe_cast.py
+-rw-r--r--   0        0        0     3316 2023-03-21 21:23:13.283262 thirdweb_sdk-3.1.0a0/thirdweb/abi/safe_erc20.py
+-rw-r--r--   0        0        0     3308 2023-03-21 21:23:13.283384 thirdweb_sdk-3.1.0a0/thirdweb/abi/safe_math.py
+-rw-r--r--   0        0        0     9992 2023-03-21 21:23:13.283531 thirdweb_sdk-3.1.0a0/thirdweb/abi/signature_action.py
+-rw-r--r--   0        0        0    10824 2023-03-21 21:23:13.283687 thirdweb_sdk-3.1.0a0/thirdweb/abi/signature_action_upgradeable.py
+-rw-r--r--   0        0        0   231932 2023-03-21 21:23:13.284160 thirdweb_sdk-3.1.0a0/thirdweb/abi/signature_drop.py
+-rw-r--r--   0        0        0    16142 2023-03-21 21:23:13.284389 thirdweb_sdk-3.1.0a0/thirdweb/abi/signature_mint_erc1155.py
+-rw-r--r--   0        0        0    16979 2023-03-21 21:23:13.284556 thirdweb_sdk-3.1.0a0/thirdweb/abi/signature_mint_erc1155_upgradeable.py
+-rw-r--r--   0        0        0    15148 2023-03-21 21:23:13.284777 thirdweb_sdk-3.1.0a0/thirdweb/abi/signature_mint_erc20.py
+-rw-r--r--   0        0        0    15983 2023-03-21 21:23:13.284942 thirdweb_sdk-3.1.0a0/thirdweb/abi/signature_mint_erc20_upgradeable.py
+-rw-r--r--   0        0        0    15917 2023-03-21 21:23:13.285134 thirdweb_sdk-3.1.0a0/thirdweb/abi/signature_mint_erc721.py
+-rw-r--r--   0        0        0    16753 2023-03-21 21:23:13.285291 thirdweb_sdk-3.1.0a0/thirdweb/abi/signature_mint_erc721_upgradeable.py
+-rw-r--r--   0        0        0   237737 2023-03-21 21:23:13.285730 thirdweb_sdk-3.1.0a0/thirdweb/abi/signaturedrop_v4.py
+-rw-r--r--   0        0        0    42531 2023-03-21 21:23:13.285946 thirdweb_sdk-3.1.0a0/thirdweb/abi/soulbound_erc721_a.py
+-rw-r--r--   0        0        0   101885 2023-03-21 21:23:13.286193 thirdweb_sdk-3.1.0a0/thirdweb/abi/split.py
+-rw-r--r--   0        0        0    72420 2023-03-21 21:23:13.286430 thirdweb_sdk-3.1.0a0/thirdweb/abi/staking1155.py
+-rw-r--r--   0        0        0   111245 2023-03-21 21:23:13.286697 thirdweb_sdk-3.1.0a0/thirdweb/abi/staking1155_base.py
+-rw-r--r--   0        0        0    73314 2023-03-21 21:23:13.286919 thirdweb_sdk-3.1.0a0/thirdweb/abi/staking1155_upgradeable.py
+-rw-r--r--   0        0        0    49004 2023-03-21 21:23:13.287115 thirdweb_sdk-3.1.0a0/thirdweb/abi/staking20.py
+-rw-r--r--   0        0        0    72923 2023-03-21 21:23:13.287329 thirdweb_sdk-3.1.0a0/thirdweb/abi/staking20_base.py
+-rw-r--r--   0        0        0    49928 2023-03-21 21:23:13.287516 thirdweb_sdk-3.1.0a0/thirdweb/abi/staking20_upgradeable.py
+-rw-r--r--   0        0        0    50405 2023-03-21 21:23:13.287702 thirdweb_sdk-3.1.0a0/thirdweb/abi/staking721.py
+-rw-r--r--   0        0        0    85256 2023-03-21 21:23:13.287922 thirdweb_sdk-3.1.0a0/thirdweb/abi/staking721_base.py
+-rw-r--r--   0        0        0    51319 2023-03-21 21:23:13.288130 thirdweb_sdk-3.1.0a0/thirdweb/abi/staking721_upgradeable.py
+-rw-r--r--   0        0        0     3316 2023-03-21 21:23:13.288248 thirdweb_sdk-3.1.0a0/thirdweb/abi/t_w_address.py
+-rw-r--r--   0        0        0     3316 2023-03-21 21:23:13.288348 thirdweb_sdk-3.1.0a0/thirdweb/abi/t_w_bit_maps.py
+-rw-r--r--   0        0        0    89887 2023-03-21 21:23:13.288497 thirdweb_sdk-3.1.0a0/thirdweb/abi/t_w_factory.py
+-rw-r--r--   0        0        0    75523 2023-03-21 21:23:13.288703 thirdweb_sdk-3.1.0a0/thirdweb/abi/t_w_fee.py
+-rw-r--r--   0        0        0    67405 2023-03-21 21:23:13.288905 thirdweb_sdk-3.1.0a0/thirdweb/abi/t_w_multichain_registry.py
+-rw-r--r--   0        0        0    37213 2023-03-21 21:23:13.289082 thirdweb_sdk-3.1.0a0/thirdweb/abi/t_w_multichain_registry_logic.py
+-rw-r--r--   0        0        0    75392 2023-03-21 21:23:13.289301 thirdweb_sdk-3.1.0a0/thirdweb/abi/t_w_multichain_registry_router.py
+-rw-r--r--   0        0        0     6169 2023-03-21 21:23:13.289435 thirdweb_sdk-3.1.0a0/thirdweb/abi/t_w_multichain_registry_storage.py
+-rw-r--r--   0        0        0     3738 2023-03-21 21:23:13.289536 thirdweb_sdk-3.1.0a0/thirdweb/abi/t_w_proxy.py
+-rw-r--r--   0        0        0    59703 2023-03-21 21:23:13.289758 thirdweb_sdk-3.1.0a0/thirdweb/abi/t_w_registry.py
+-rw-r--r--   0        0        0     3378 2023-03-21 21:23:13.289874 thirdweb_sdk-3.1.0a0/thirdweb/abi/t_w_storage_slot.py
+-rw-r--r--   0        0        0     3316 2023-03-21 21:23:13.289982 thirdweb_sdk-3.1.0a0/thirdweb/abi/t_w_strings.py
+-rw-r--r--   0        0        0   206242 2023-03-21 21:23:13.290372 thirdweb_sdk-3.1.0a0/thirdweb/abi/tiered_drop.py
+-rw-r--r--   0        0        0    15273 2023-03-21 21:23:13.290500 thirdweb_sdk-3.1.0a0/thirdweb/abi/token_bundle.py
+-rw-r--r--   0        0        0   182279 2023-03-21 21:23:13.290887 thirdweb_sdk-3.1.0a0/thirdweb/abi/token_erc1155.py
+-rw-r--r--   0        0        0   176744 2023-03-21 21:23:13.291274 thirdweb_sdk-3.1.0a0/thirdweb/abi/token_erc20.py
+-rw-r--r--   0        0        0   185235 2023-03-21 21:23:13.291683 thirdweb_sdk-3.1.0a0/thirdweb/abi/token_erc721.py
+-rw-r--r--   0        0        0   118802 2023-03-21 21:23:13.291949 thirdweb_sdk-3.1.0a0/thirdweb/abi/token_stake.py
+-rw-r--r--   0        0        0    35792 2023-03-21 21:23:13.292111 thirdweb_sdk-3.1.0a0/thirdweb/abi/token_store.py
+-rw-r--r--   0        0        0    15519 2023-03-21 21:23:13.292243 thirdweb_sdk-3.1.0a0/thirdweb/abi/upgradeable.py
+-rw-r--r--   0        0        0   180710 2023-03-21 21:23:13.292582 thirdweb_sdk-3.1.0a0/thirdweb/abi/vote_erc20.py
+-rw-r--r--   0        0        0        0 2023-03-13 04:51:11.298098 thirdweb_sdk-3.1.0a0/thirdweb/common/__init__.py
+-rw-r--r--   0        0        0     4797 2023-03-13 04:51:11.298195 thirdweb_sdk-3.1.0a0/thirdweb/common/claim_conditions.py
+-rw-r--r--   0        0        0     4039 2023-03-13 04:51:11.298272 thirdweb_sdk-3.1.0a0/thirdweb/common/currency.py
+-rw-r--r--   0        0        0     2706 2023-03-13 04:51:11.298342 thirdweb_sdk-3.1.0a0/thirdweb/common/error.py
+-rw-r--r--   0        0        0     3962 2023-03-21 02:20:09.125984 thirdweb_sdk-3.1.0a0/thirdweb/common/feature_detection.py
+-rw-r--r--   0        0        0      161 2023-07-18 18:53:20.931998 thirdweb_sdk-3.1.0a0/thirdweb/common/keys.py
+-rw-r--r--   0        0        0     4696 2023-03-13 04:51:11.298476 thirdweb_sdk-3.1.0a0/thirdweb/common/marketplace.py
+-rw-r--r--   0        0        0     4657 2023-03-13 04:51:11.298549 thirdweb_sdk-3.1.0a0/thirdweb/common/merkle_tree.py
+-rw-r--r--   0        0        0     2699 2023-03-13 04:51:11.298625 thirdweb_sdk-3.1.0a0/thirdweb/common/nft.py
+-rw-r--r--   0        0        0     1241 2023-03-13 04:51:11.298693 thirdweb_sdk-3.1.0a0/thirdweb/common/sign.py
+-rw-r--r--   0        0        0      287 2023-03-13 04:51:11.298753 thirdweb_sdk-3.1.0a0/thirdweb/common/signature_minting.py
+-rw-r--r--   0        0        0     2552 2023-03-13 04:51:11.298824 thirdweb_sdk-3.1.0a0/thirdweb/common/snapshots.py
+-rw-r--r--   0        0        0        0 2023-03-13 04:51:11.298891 thirdweb_sdk-3.1.0a0/thirdweb/constants/__init__.py
+-rw-r--r--   0        0        0     3044 2023-03-13 04:51:11.298995 thirdweb_sdk-3.1.0a0/thirdweb/constants/addresses.py
+-rw-r--r--   0        0        0      284 2023-03-13 04:51:11.299055 thirdweb_sdk-3.1.0a0/thirdweb/constants/chains.py
+-rw-r--r--   0        0        0      182 2023-03-13 04:51:11.299107 thirdweb_sdk-3.1.0a0/thirdweb/constants/contract.py
+-rw-r--r--   0        0        0     2457 2023-03-13 04:51:11.299165 thirdweb_sdk-3.1.0a0/thirdweb/constants/currency.py
+-rw-r--r--   0        0        0      190 2023-03-13 04:51:11.299216 thirdweb_sdk-3.1.0a0/thirdweb/constants/events.py
+-rw-r--r--   0        0        0      983 2023-03-13 04:51:11.299284 thirdweb_sdk-3.1.0a0/thirdweb/constants/role.py
+-rw-r--r--   0        0        0      544 2023-03-13 04:51:11.299350 thirdweb_sdk-3.1.0a0/thirdweb/constants/rpc.py
+-rw-r--r--   0        0        0     1739 2023-07-18 18:53:20.932184 thirdweb_sdk-3.1.0a0/thirdweb/constants/urls.py
+-rw-r--r--   0        0        0      254 2023-03-13 04:51:11.299504 thirdweb_sdk-3.1.0a0/thirdweb/contracts/__init__.py
+-rw-r--r--   0        0        0     7951 2023-07-18 18:53:20.932405 thirdweb_sdk-3.1.0a0/thirdweb/contracts/custom.py
+-rw-r--r--   0        0        0     8186 2023-07-18 18:53:20.932627 thirdweb_sdk-3.1.0a0/thirdweb/contracts/edition.py
+-rw-r--r--   0        0        0     6104 2023-07-18 18:53:20.932850 thirdweb_sdk-3.1.0a0/thirdweb/contracts/edition_drop.py
+-rw-r--r--   0        0        0     1680 2023-03-13 04:51:11.299821 thirdweb_sdk-3.1.0a0/thirdweb/contracts/maps.py
+-rw-r--r--   0        0        0    12895 2023-07-18 18:53:20.933097 thirdweb_sdk-3.1.0a0/thirdweb/contracts/marketplace.py
+-rw-r--r--   0        0        0    12498 2023-07-18 18:53:20.933374 thirdweb_sdk-3.1.0a0/thirdweb/contracts/multiwrap.py
+-rw-r--r--   0        0        0     7695 2023-07-18 18:53:20.933613 thirdweb_sdk-3.1.0a0/thirdweb/contracts/nft_collection.py
+-rw-r--r--   0        0        0     8503 2023-07-18 18:53:20.933817 thirdweb_sdk-3.1.0a0/thirdweb/contracts/nft_drop.py
+-rw-r--r--   0        0        0     6104 2023-07-18 18:53:20.934038 thirdweb_sdk-3.1.0a0/thirdweb/contracts/token.py
+-rw-r--r--   0        0        0       29 2023-03-13 04:51:11.300414 thirdweb_sdk-3.1.0a0/thirdweb/core/__init__.py
+-rw-r--r--   0        0        0       54 2023-03-13 04:51:11.300500 thirdweb_sdk-3.1.0a0/thirdweb/core/auth/__init__.py
+-rw-r--r--   0        0        0    13845 2023-03-13 04:51:11.300598 thirdweb_sdk-3.1.0a0/thirdweb/core/auth/wallet_authenticator.py
+-rw-r--r--   0        0        0        0 2023-03-13 04:51:11.300659 thirdweb_sdk-3.1.0a0/thirdweb/core/classes/__init__.py
+-rw-r--r--   0        0        0     1318 2023-03-21 22:42:36.159881 thirdweb_sdk-3.1.0a0/thirdweb/core/classes/base_contract.py
+-rw-r--r--   0        0        0     3976 2023-07-18 18:53:20.934567 thirdweb_sdk-3.1.0a0/thirdweb/core/classes/contract_deployer.py
+-rw-r--r--   0        0        0     3359 2023-03-23 03:04:29.207240 thirdweb_sdk-3.1.0a0/thirdweb/core/classes/contract_events.py
+-rw-r--r--   0        0        0     2110 2023-03-24 01:37:36.263013 thirdweb_sdk-3.1.0a0/thirdweb/core/classes/contract_metadata.py
+-rw-r--r--   0        0        0     1983 2023-03-24 01:37:36.263235 thirdweb_sdk-3.1.0a0/thirdweb/core/classes/contract_platform_fee.py
+-rw-r--r--   0        0        0     4275 2023-03-24 01:37:36.263461 thirdweb_sdk-3.1.0a0/thirdweb/core/classes/contract_roles.py
+-rw-r--r--   0        0        0     4231 2023-05-10 22:38:00.168091 thirdweb_sdk-3.1.0a0/thirdweb/core/classes/contract_royalty.py
+-rw-r--r--   0        0        0     1388 2023-03-24 01:37:36.263947 thirdweb_sdk-3.1.0a0/thirdweb/core/classes/contract_sales.py
+-rw-r--r--   0        0        0     6879 2023-05-10 23:38:42.151333 thirdweb_sdk-3.1.0a0/thirdweb/core/classes/contract_wrapper.py
+-rw-r--r--   0        0        0     2361 2023-03-13 04:51:11.301333 thirdweb_sdk-3.1.0a0/thirdweb/core/classes/drop_claim_conditions.py
+-rw-r--r--   0        0        0     2722 2023-03-13 04:51:11.301386 thirdweb_sdk-3.1.0a0/thirdweb/core/classes/drop_erc1155_claim_conditions.py
+-rw-r--r--   0        0        0    24253 2023-03-24 02:09:56.316705 thirdweb_sdk-3.1.0a0/thirdweb/core/classes/erc_1155.py
+-rw-r--r--   0        0        0     8047 2023-03-13 04:51:11.301549 thirdweb_sdk-3.1.0a0/thirdweb/core/classes/erc_1155_signature_minting.py
+-rw-r--r--   0        0        0     5534 2023-03-23 03:00:03.895228 thirdweb_sdk-3.1.0a0/thirdweb/core/classes/erc_1155_standard.py
+-rw-r--r--   0        0        0    11065 2023-03-24 01:37:36.264471 thirdweb_sdk-3.1.0a0/thirdweb/core/classes/erc_20.py
+-rw-r--r--   0        0        0     6733 2023-03-13 04:51:11.301730 thirdweb_sdk-3.1.0a0/thirdweb/core/classes/erc_20_signature_minting.py
+-rw-r--r--   0        0        0     6779 2023-03-23 03:00:03.895861 thirdweb_sdk-3.1.0a0/thirdweb/core/classes/erc_20_standard.py
+-rw-r--r--   0        0        0    23244 2023-03-24 01:37:46.685537 thirdweb_sdk-3.1.0a0/thirdweb/core/classes/erc_721.py
+-rw-r--r--   0        0        0     7822 2023-03-13 04:51:11.301886 thirdweb_sdk-3.1.0a0/thirdweb/core/classes/erc_721_signature_minting.py
+-rw-r--r--   0        0        0     5646 2023-03-23 03:00:03.896556 thirdweb_sdk-3.1.0a0/thirdweb/core/classes/erc_721_standard.py
+-rw-r--r--   0        0        0     6448 2023-07-18 18:53:20.935049 thirdweb_sdk-3.1.0a0/thirdweb/core/classes/factory.py
+-rw-r--r--   0        0        0     8646 2023-07-18 18:53:20.935421 thirdweb_sdk-3.1.0a0/thirdweb/core/classes/ipfs_storage.py
+-rw-r--r--   0        0        0    11102 2023-03-13 04:51:11.302151 thirdweb_sdk-3.1.0a0/thirdweb/core/classes/marketplace_auction.py
+-rw-r--r--   0        0        0    12104 2023-03-13 04:51:11.302217 thirdweb_sdk-3.1.0a0/thirdweb/core/classes/marketplace_direct.py
+-rw-r--r--   0        0        0     2764 2023-03-13 04:51:11.302278 thirdweb_sdk-3.1.0a0/thirdweb/core/classes/provider_handler.py
+-rw-r--r--   0        0        0     1257 2023-03-13 04:51:11.302340 thirdweb_sdk-3.1.0a0/thirdweb/core/classes/registry.py
+-rw-r--r--   0        0        0     4780 2023-03-13 04:51:11.302405 thirdweb_sdk-3.1.0a0/thirdweb/core/classes/sharded_merkle_tree.py
+-rw-r--r--   0        0        0     3227 2023-03-13 04:51:11.302500 thirdweb_sdk-3.1.0a0/thirdweb/core/helpers/storage.py
+-rw-r--r--   0        0        0     8063 2023-07-18 18:53:20.935765 thirdweb_sdk-3.1.0a0/thirdweb/core/sdk.py
+-rw-r--r--   0        0        0      254 2023-03-13 04:51:11.302670 thirdweb_sdk-3.1.0a0/thirdweb/types/__init__.py
+-rw-r--r--   0        0        0     1482 2023-03-13 04:51:11.302742 thirdweb_sdk-3.1.0a0/thirdweb/types/auth.py
+-rw-r--r--   0        0        0     1836 2023-03-23 03:00:03.896883 thirdweb_sdk-3.1.0a0/thirdweb/types/contract.py
+-rw-r--r--   0        0        0     3111 2023-03-13 04:51:11.302929 thirdweb_sdk-3.1.0a0/thirdweb/types/contracts/claim_conditions.py
+-rw-r--r--   0        0        0     5664 2023-03-13 04:51:11.303002 thirdweb_sdk-3.1.0a0/thirdweb/types/contracts/signature.py
+-rw-r--r--   0        0        0      528 2023-03-13 04:51:11.303061 thirdweb_sdk-3.1.0a0/thirdweb/types/currency.py
+-rw-r--r--   0        0        0      578 2023-03-13 04:51:11.303126 thirdweb_sdk-3.1.0a0/thirdweb/types/events.py
+-rw-r--r--   0        0        0     2519 2023-03-13 04:51:11.303186 thirdweb_sdk-3.1.0a0/thirdweb/types/marketplace.py
+-rw-r--r--   0        0        0      945 2023-03-13 04:51:11.303247 thirdweb_sdk-3.1.0a0/thirdweb/types/multiwrap.py
+-rw-r--r--   0        0        0     3574 2023-03-13 04:51:11.303318 thirdweb_sdk-3.1.0a0/thirdweb/types/nft.py
+-rw-r--r--   0        0        0     1121 2023-07-18 18:53:20.936085 thirdweb_sdk-3.1.0a0/thirdweb/types/sdk.py
+-rw-r--r--   0        0        0      329 2023-03-23 03:04:29.209187 thirdweb_sdk-3.1.0a0/thirdweb/types/settings/__init__.py
+-rw-r--r--   0        0        0     4111 2023-03-13 04:51:11.303569 thirdweb_sdk-3.1.0a0/thirdweb/types/settings/metadata.py
+-rw-r--r--   0        0        0      215 2023-03-13 04:51:11.303629 thirdweb_sdk-3.1.0a0/thirdweb/types/storage.py
+-rw-r--r--   0        0        0      334 2023-03-13 04:51:11.303692 thirdweb_sdk-3.1.0a0/thirdweb/types/tx.py
+-rw-r--r--   0        0        0     7259 1970-01-01 00:00:00.000000 thirdweb_sdk-3.1.0a0/PKG-INFO
```

### Comparing `thirdweb_sdk-3.0.3a0/LICENSE` & `thirdweb_sdk-3.1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/README.md` & `thirdweb_sdk-3.1.0a0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -17,25 +17,29 @@
 
 ```bash
 pip install thirdweb-sdk
 ```
 
 ## Getting Started
 
-To start using this SDK, you just need to pass in a provider configuration.
+To start using this SDK, you just need to pass in a provider configuration. It's also strongly recommended that you use your thirdweb API keys with the SDK in order to get the best infrastructure performance (across RPCs, IPFS, etc.) - you can learn more about creating and using API keys [here](https://portal.thirdweb.com/api-keys).
 
 ### Instantiating the SDK
 
 Once you have all the necessary dependencies, you can follow the following setup steps to get started with the SDK read-only functions:
 
 ```python
 from thirdweb import ThirdwebSDK
+from thirdweb.types import SDKOptions
 
-# You can create a new instance of the SDK to use by just passing in a network name
-sdk = ThirdwebSDK("mumbai")
+# Get your secret key from the thirdweb api keys dashboard
+SECRET_KEY = "..."
+
+# You can create a new instance of the SDK to use by passing in a network name and your api key
+sdk = ThirdwebSDK("mumbai", options=SDKOptions(secret_key=SECRET_KEY))
 ```
 
 The SDK supports the `mainnet`, `rinkeby`, `goerli`, `polygon`, `mumbai`, `fantom`, and `avalanche` networks.
 
 Alternatively, if you want to use your own custom RPC URL, you can pass in the RPC URL directly as follows:
 
 ```python
@@ -69,20 +73,24 @@
 > :warning: Never commit private keys to file tracking history, or your account could be compromised.
 
 Meanwhile, if you want to use write functions as well and connect a signer, you can use the following setup:
 
 ```python
 from thirdweb import ThirdwebSDK
 from thirdweb.types.nft import NFTMetadataInput
+import os
+
+# Get your secret key from the thirdweb api keys dashboard
+SECRET_KEY = "..."
 
-# Learn more about securely accessing your private key: https://portal.thirdweb.com/web3-sdk/set-up-the-sdk/securing-your-private-key
-PRIVATE_KEY = "<your-private-key-here>",
+# This PRIVATE KEY is coming from your environment variables. Make sure to never put it in a tracked file or share it with anyone.
+PRIVATE_KEY = os.environ.get("PRIVATE_KEY")
 
 # Now you can create a new instance of the SDK with your private key
-sdk = ThirdwebSDK.from_private_key(PRIVATE_KEY, "mumbai")
+sdk = ThirdwebSDK.from_private_key(PRIVATE_KEY, "mumbai", options=SDKOptions(secret_key=SECRET_KEY))
 
 # Instantiate a new NFT Collection contract as described above.
 NFT_COLLECTION_ADDRESS = "0x.."
 nft_collection = sdk.get_nft_collection(NFT_COLLECTION_ADDRESS)
 
 # Now you can use any of the SDK contract functions including write functions
 nft_collection.mint(NFTMetadataInput.from_json({ "name": "Cool NFT", "description": "Minted with the Python SDK!" }))
```

#### html2text {}

```diff
@@ -1,72 +1,79 @@
 
 
                        ****** thirdweb Python SDK ******
                [pypi_version] [Build_Status] [Join_our_Discord!]
                     Best in class Web3 SDK for Python 3.7+
 
 ## Installation ```bash pip install thirdweb-sdk ``` ## Getting Started To
-start using this SDK, you just need to pass in a provider configuration. ###
-Instantiating the SDK Once you have all the necessary dependencies, you can
-follow the following setup steps to get started with the SDK read-only
-functions: ```python from thirdweb import ThirdwebSDK # You can create a new
-instance of the SDK to use by just passing in a network name sdk = ThirdwebSDK
-("mumbai") ``` The SDK supports the `mainnet`, `rinkeby`, `goerli`, `polygon`,
-`mumbai`, `fantom`, and `avalanche` networks. Alternatively, if you want to use
-your own custom RPC URL, you can pass in the RPC URL directly as follows:
-```python from thirdweb import ThirdwebSDK # Set your RPC_URL RPC_URL = "https:
-//rpc-mainnet.matic.network" # And now you can instantiate the SDK with it sdk
-= ThirdwebSDK(RPC_URL) ``` ### Working With Contracts Once you instantiate the
-SDK, you can use it to access your thirdweb contracts. You can use the SDK's
-contract getter functions like `get_token`, `get_edition`,
-`get_nft_collection`, and `get_marketplace` to get the respective SDK contract
-instances. To use an NFT Collection contract for example, you can do the
-following. ```python # Add your NFT Collection contract address here
-NFT_COLLECTION_ADDRESS = "0x.." # And you can instantiate your contract with
-just one line nft_collection = sdk.get_nft_collection(NFT_COLLECTION_ADDRESS) #
-Now you can use any of the read-only SDK contract functions nfts =
-nft_collection.get_all() print(nfts) ``` ### Signing Transactions > :warning:
-Never commit private keys to file tracking history, or your account could be
-compromised. Meanwhile, if you want to use write functions as well and connect
-a signer, you can use the following setup: ```python from thirdweb import
-ThirdwebSDK from thirdweb.types.nft import NFTMetadataInput # Learn more about
-securely accessing your private key: https://portal.thirdweb.com/web3-sdk/set-
-up-the-sdk/securing-your-private-key PRIVATE_KEY = "", # Now you can create a
-new instance of the SDK with your private key sdk =
-ThirdwebSDK.from_private_key(PRIVATE_KEY, "mumbai") # Instantiate a new NFT
-Collection contract as described above. NFT_COLLECTION_ADDRESS = "0x.."
-nft_collection = sdk.get_nft_collection(NFT_COLLECTION_ADDRESS) # Now you can
-use any of the SDK contract functions including write functions
-nft_collection.mint(NFTMetadataInput.from_json({ "name": "Cool NFT",
-"description": "Minted with the Python SDK!" })) ``` ## Development Environment
-In this section, we'll go over the steps to get started with running the Python
-SDK repository locally and contributing to the code. If you aren't interested
-in contributing to the thirdweb Python SDK, you can ignore this section. ###
-Poetry Environment Setup If you want to work with this repository, make sure to
-setup [Poetry](https://python-poetry.org/docs/), you're virtual environment,
-and the code styling tools. Assuming you've installed and setup poetry, you can
-setup this repository with: ```bash $ make init ``` ### Running Tests Once you
-have run the initialization step, you can run the following to run all tests:
-```bash $ make test ``` ### Publishing the Package To make a build & publish
-the package, you need to have a `pypi` account with permission to edit the
-`thirdweb-sdk` pypi package. You can authenticate your pypi account with poetry
-with the following command: ```bash poetry config pypi-token.pypi pypi-token-
-here ``` Then, you can build and release a prerelease version with the
-following command: ```bash make publish ``` ### Code Style Setup Make sure you
-have `mypy`, `pylint`, and `black` installed (all included in the dev
-dependencies with `poetry install`. If you're working in VSCode, there a few
-steps to get everything working with the poetry .venv: 1. To setup poetry
-virtual environment inside your VSCode so it gets recognized as part of your
-project (import for linters), you can take the following steps from this [stack
-overflow answer](https://stackoverflow.com/questions/59882884/vscode-doesnt-
-show-poetry-virtualenvs-in-select-interpreter-option). You need to run `poetry
-config virtualenvs.in-project true` and then make sure you delete/create a new
-poetry env. 2. In `.vscode/settings.json`, you should have the following:
-```json { "python.linting.mypyEnabled": true, "python.linting.enabled": true,
-"python.linting.pylintEnabled": false } ``` 3. Make sure to set your VSCode
-`Python: Interpreter` setting to the Python version inside your poetry virtual
-environment. ### Generate Python ABI Wrappers Use the [abi-gen](https://
-www.npmjs.com/package/@0x/abi-gen) package to create the Python ABIs. You can
-install it with the following command: ```bash $ npm install -g @0x/abi-gen ```
-Assuming you have the thirdweb contract ABIs in this directory at `/abi`, you
-can run the following command to generate the necessary ABIs. ```bash $ make
-abi ```
+start using this SDK, you just need to pass in a provider configuration. It's
+also strongly recommended that you use your thirdweb API keys with the SDK in
+order to get the best infrastructure performance (across RPCs, IPFS, etc.) -
+you can learn more about creating and using API keys [here](https://
+portal.thirdweb.com/api-keys). ### Instantiating the SDK Once you have all the
+necessary dependencies, you can follow the following setup steps to get started
+with the SDK read-only functions: ```python from thirdweb import ThirdwebSDK
+from thirdweb.types import SDKOptions # Get your secret key from the thirdweb
+api keys dashboard SECRET_KEY = "..." # You can create a new instance of the
+SDK to use by passing in a network name and your api key sdk = ThirdwebSDK
+("mumbai", options=SDKOptions(secret_key=SECRET_KEY)) ``` The SDK supports the
+`mainnet`, `rinkeby`, `goerli`, `polygon`, `mumbai`, `fantom`, and `avalanche`
+networks. Alternatively, if you want to use your own custom RPC URL, you can
+pass in the RPC URL directly as follows: ```python from thirdweb import
+ThirdwebSDK # Set your RPC_URL RPC_URL = "https://rpc-mainnet.matic.network" #
+And now you can instantiate the SDK with it sdk = ThirdwebSDK(RPC_URL) ``` ###
+Working With Contracts Once you instantiate the SDK, you can use it to access
+your thirdweb contracts. You can use the SDK's contract getter functions like
+`get_token`, `get_edition`, `get_nft_collection`, and `get_marketplace` to get
+the respective SDK contract instances. To use an NFT Collection contract for
+example, you can do the following. ```python # Add your NFT Collection contract
+address here NFT_COLLECTION_ADDRESS = "0x.." # And you can instantiate your
+contract with just one line nft_collection = sdk.get_nft_collection
+(NFT_COLLECTION_ADDRESS) # Now you can use any of the read-only SDK contract
+functions nfts = nft_collection.get_all() print(nfts) ``` ### Signing
+Transactions > :warning: Never commit private keys to file tracking history, or
+your account could be compromised. Meanwhile, if you want to use write
+functions as well and connect a signer, you can use the following setup:
+```python from thirdweb import ThirdwebSDK from thirdweb.types.nft import
+NFTMetadataInput import os # Get your secret key from the thirdweb api keys
+dashboard SECRET_KEY = "..." # This PRIVATE KEY is coming from your environment
+variables. Make sure to never put it in a tracked file or share it with anyone.
+PRIVATE_KEY = os.environ.get("PRIVATE_KEY") # Now you can create a new instance
+of the SDK with your private key sdk = ThirdwebSDK.from_private_key
+(PRIVATE_KEY, "mumbai", options=SDKOptions(secret_key=SECRET_KEY)) #
+Instantiate a new NFT Collection contract as described above.
+NFT_COLLECTION_ADDRESS = "0x.." nft_collection = sdk.get_nft_collection
+(NFT_COLLECTION_ADDRESS) # Now you can use any of the SDK contract functions
+including write functions nft_collection.mint(NFTMetadataInput.from_json(
+{ "name": "Cool NFT", "description": "Minted with the Python SDK!" })) ``` ##
+Development Environment In this section, we'll go over the steps to get started
+with running the Python SDK repository locally and contributing to the code. If
+you aren't interested in contributing to the thirdweb Python SDK, you can
+ignore this section. ### Poetry Environment Setup If you want to work with this
+repository, make sure to setup [Poetry](https://python-poetry.org/docs/),
+you're virtual environment, and the code styling tools. Assuming you've
+installed and setup poetry, you can setup this repository with: ```bash $ make
+init ``` ### Running Tests Once you have run the initialization step, you can
+run the following to run all tests: ```bash $ make test ``` ### Publishing the
+Package To make a build & publish the package, you need to have a `pypi`
+account with permission to edit the `thirdweb-sdk` pypi package. You can
+authenticate your pypi account with poetry with the following command: ```bash
+poetry config pypi-token.pypi pypi-token-here ``` Then, you can build and
+release a prerelease version with the following command: ```bash make publish
+``` ### Code Style Setup Make sure you have `mypy`, `pylint`, and `black`
+installed (all included in the dev dependencies with `poetry install`. If
+you're working in VSCode, there a few steps to get everything working with the
+poetry .venv: 1. To setup poetry virtual environment inside your VSCode so it
+gets recognized as part of your project (import for linters), you can take the
+following steps from this [stack overflow answer](https://stackoverflow.com/
+questions/59882884/vscode-doesnt-show-poetry-virtualenvs-in-select-interpreter-
+option). You need to run `poetry config virtualenvs.in-project true` and then
+make sure you delete/create a new poetry env. 2. In `.vscode/settings.json`,
+you should have the following: ```json { "python.linting.mypyEnabled": true,
+"python.linting.enabled": true, "python.linting.pylintEnabled": false } ``` 3.
+Make sure to set your VSCode `Python: Interpreter` setting to the Python
+version inside your poetry virtual environment. ### Generate Python ABI
+Wrappers Use the [abi-gen](https://www.npmjs.com/package/@0x/abi-gen) package
+to create the Python ABIs. You can install it with the following command:
+```bash $ npm install -g @0x/abi-gen ``` Assuming you have the thirdweb
+contract ABIs in this directory at `/abi`, you can run the following command to
+generate the necessary ABIs. ```bash $ make abi ```
```

### Comparing `thirdweb_sdk-3.0.3a0/pyproject.toml` & `thirdweb_sdk-3.1.0a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 authors = ["thirdweb <sdk@thirdweb.com>"]
 description = ""
 name = "thirdweb-sdk"
 packages = [
   {include = "thirdweb"},
 ]
 readme = "README.md"
-version = "3.0.3a0"
+version = "3.1.0a0"
 
 [tool.poetry.dependencies]
 python = ">=3.7.1"
 dacite = "^1.6.0"
 mypy-extensions = "^0.4.3"
 thirdweb-contract-wrappers = "^2.0.4"
 web3 = "5.27.0"
```

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/.DS_Store` & `thirdweb_sdk-3.1.0a0/thirdweb/.DS_Store`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/__init__.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/__init__.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/airdrop_erc1155.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/airdrop_erc1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/airdrop_erc1155_claimable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/airdrop_erc1155_claimable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/airdrop_erc20.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/airdrop_erc20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/airdrop_erc20_claimable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/airdrop_erc20_claimable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/airdrop_erc721.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/airdrop_erc721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/airdrop_erc721_claimable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/airdrop_erc721_claimable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/app_u_r_i.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/app_u_r_i.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/batch_mint_metadata.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/batch_mint_metadata.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/context.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/context.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/contract_metadata.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/contract_metadata.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/contract_metadata_logic.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/contract_metadata_logic.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/contract_metadata_storage.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/contract_metadata_storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/contract_publisher.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/contract_publisher.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/counters.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/counters.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/currency_transfer_lib.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/currency_transfer_lib.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/default_operator_filterer.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/default_operator_filterer.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/default_operator_filterer_upgradeable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/default_operator_filterer_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/delayed_reveal.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/delayed_reveal.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/direct_listings_logic.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/direct_listings_logic.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/direct_listings_storage.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/direct_listings_storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/drop.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/drop.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/drop1155.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/drop1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/drop_erc1155.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/drop_erc1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/drop_erc20.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/drop_erc20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/drop_erc721.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/drop_erc721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/drop_single_phase.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/drop_single_phase.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/drop_single_phase1155.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/drop_single_phase1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/droperc1155_v2.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/droperc1155_v2.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/droperc20_v2.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/droperc20_v2.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/droperc721_v3.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/droperc721_v3.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/dropsinglephase1155_v1.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/dropsinglephase1155_v1.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/dropsinglephase_v1.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/dropsinglephase_v1.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/e_i_p712_chainless_domain.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/e_i_p712_chainless_domain.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/ecdsa.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/ecdsa.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/edition_stake.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/edition_stake.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/eip712.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/eip712.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/english_auctions_logic.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/english_auctions_logic.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/english_auctions_storage.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/english_auctions_storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/enumerable_set.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/enumerable_set.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc1155.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc1155_base.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc1155_base.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc1155_delayed_reveal.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc1155_delayed_reveal.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc1155_drop.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc1155_drop.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc1155_holder.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc1155_holder.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc1155_lazy_mint.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc1155_lazy_mint.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc1155_preset_upgradeable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc1155_preset_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc1155_receiver.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc1155_receiver.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc1155_signature_mint.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc1155_signature_mint.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc165.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc165.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc1967_proxy.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc1967_proxy.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc1967_upgrade.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc1967_upgrade.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc20.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc20_base.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc20_base.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc20_drop.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc20_drop.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc20_drop_vote.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc20_drop_vote.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc20_permit.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc20_permit.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc20_signature_mint.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc20_signature_mint.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc20_signature_mint_vote.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc20_signature_mint_vote.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc20_vote.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc20_vote.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc20_votes.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc20_votes.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc2771_context.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc2771_context.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc2771_context_consumer.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc2771_context_consumer.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc2771_context_logic.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc2771_context_logic.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc2771_context_storage.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc2771_context_storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc2771_context_upgradeable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc2771_context_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc2771_context_upgradeable_logic.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc2771_context_upgradeable_logic.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc2771_context_upgradeable_storage.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc2771_context_upgradeable_storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc721_a_upgradeable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc721_a_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc721_base.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc721_base.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc721_delayed_reveal.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc721_delayed_reveal.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc721_drop.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc721_drop.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc721_holder.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc721_holder.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc721_lazy_mint.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc721_lazy_mint.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc721_multiwrap.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc721_multiwrap.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc721_signature_mint.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc721_signature_mint.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/erc721a.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/erc721a.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/fee_type.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/fee_type.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/forwarder_consumer.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/forwarder_consumer.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_airdrop_erc1155.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_airdrop_erc1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_airdrop_erc1155_claimable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_airdrop_erc1155_claimable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_airdrop_erc20.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_airdrop_erc20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_airdrop_erc20_claimable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_airdrop_erc20_claimable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_airdrop_erc721.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_airdrop_erc721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_airdrop_erc721_claimable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_airdrop_erc721_claimable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_app_u_r_i.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_app_u_r_i.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_beacon.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_beacon.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_burnable_erc1155.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_burnable_erc1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_burnable_erc20.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_burnable_erc20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_burnable_erc721.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_burnable_erc721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_claim_condition.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_claim_condition.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_claim_condition_multi_phase.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_claim_condition_multi_phase.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_claim_conditions_single_phase.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_claim_conditions_single_phase.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_claimable_erc1155.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_claimable_erc1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_claimable_erc721.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_claimable_erc721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_context.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_context.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_contract_deployer.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_contract_deployer.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_contract_factory.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_contract_factory.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_contract_metadata.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_contract_metadata.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_contract_publisher.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_contract_publisher.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_delayed_reveal.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_delayed_reveal.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_delayed_reveal_deprecated.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_delayed_reveal_deprecated.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_direct_listings.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_direct_listings.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_drop.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_drop.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_drop1155.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_drop1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_drop_claim_condition.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_drop_claim_condition.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_drop_erc1155.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_drop_erc1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_drop_erc20.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_drop_erc20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_drop_erc721.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_drop_erc721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_drop_single_phase.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_drop_single_phase.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_drop_single_phase1155.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_drop_single_phase1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_edition_stake.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_edition_stake.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_english_auctions.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_english_auctions.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_erc1155_enumerable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_erc1155_enumerable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_erc1155_metadata.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_erc1155_metadata.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_erc1155_receiver.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_erc1155_receiver.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_erc1155_supply.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_erc1155_supply.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_erc1822_proxiable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_erc1822_proxiable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_erc20_metadata.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_erc20_metadata.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_erc20_permit.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_erc20_permit.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_erc2771_context.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_erc2771_context.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_erc721_enumerable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_erc721_enumerable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_erc721_metadata.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_erc721_metadata.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_erc721_receiver.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_erc721_receiver.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_erc721_supply.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_erc721_supply.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_fee_tier_placement_extension.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_fee_tier_placement_extension.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_lazy_mint.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_lazy_mint.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_lazy_mint_with_tier.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_lazy_mint_with_tier.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_marketplace.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_marketplace.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_mintable_erc1155.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_mintable_erc1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_mintable_erc20.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_mintable_erc20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_mintable_erc721.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_mintable_erc721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_multicall.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_multicall.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_multiwrap.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_multiwrap.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_n_f_t_stake.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_n_f_t_stake.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_offers.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_offers.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_operator_filter_registry.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_operator_filter_registry.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_operator_filter_toggle.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_operator_filter_toggle.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_ownable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_ownable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_pack.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_pack.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_pack_v_r_f_direct.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_pack_v_r_f_direct.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_permissions.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_permissions.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_permissions_enumerable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_permissions_enumerable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_platform_fee.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_platform_fee.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_plugin_map.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_plugin_map.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_primary_sale.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_primary_sale.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_router.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_router.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_royalty.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_royalty.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_signature_action.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_signature_action.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_signature_mint_erc1155.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_signature_mint_erc1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_signature_mint_erc20.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_signature_mint_erc20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_signature_mint_erc721.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_signature_mint_erc721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_staking1155.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_staking1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_staking20.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_staking20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_staking721.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_staking721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_t_w_fee.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_t_w_fee.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_t_w_multichain_registry.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_t_w_multichain_registry.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_t_w_registry.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_t_w_registry.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_thirdweb_contract.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_thirdweb_contract.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_token_bundle.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_token_bundle.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_token_erc1155.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_token_erc1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_token_erc20.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_token_erc20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_token_erc721.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_token_erc721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_token_stake.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_token_stake.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/i_votes.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/i_votes.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/iclaimcondition_v1.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/iclaimcondition_v1.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/idropclaimcondition_v2.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/idropclaimcondition_v2.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/idroperc1155_v2.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/idroperc1155_v2.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/idroperc20_v2.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/idroperc20_v2.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/idroperc721_v3.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/idroperc721_v3.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/idropsinglephase1155_v1.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/idropsinglephase1155_v1.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/idropsinglephase_v1.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/idropsinglephase_v1.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/ierc1155.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/ierc1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/ierc165.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/ierc165.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/ierc20.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/ierc20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/ierc2981.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/ierc2981.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/ierc721.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/ierc721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/ierc721a.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/ierc721a.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/init_storage.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/init_storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/initializable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/initializable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/isignatureminterc721_v1.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/isignatureminterc721_v1.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/iweth.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/iweth.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/lazy_mint.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/lazy_mint.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/lazy_mint_with_tier.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/lazy_mint_with_tier.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/marketplace.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/marketplace.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/marketplace_v3.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/marketplace_v3.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/math.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/math.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/merkle_proof.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/merkle_proof.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/mock.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/mock.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/mock_contract.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/mock_contract.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/mock_contract_publisher.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/mock_contract_publisher.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/multicall.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/multicall.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/multiwrap.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/multiwrap.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/n_f_t_stake.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/n_f_t_stake.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/offers_logic.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/offers_logic.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/offers_storage.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/offers_storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/operator_filter_toggle.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/operator_filter_toggle.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/operator_filterer.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/operator_filterer.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/operator_filterer_upgradeable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/operator_filterer_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/ownable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/ownable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/pack.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/pack.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/pack_v_r_f_direct.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/pack_v_r_f_direct.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/payment_splitter_upgradeable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/payment_splitter_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/permissions.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/permissions.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/permissions_enumerable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/permissions_enumerable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/permissions_enumerable_logic.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/permissions_enumerable_logic.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/permissions_enumerable_storage.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/permissions_enumerable_storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/permissions_logic.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/permissions_logic.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/permissions_storage.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/permissions_storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/platform_fee.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/platform_fee.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/platform_fee_logic.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/platform_fee_logic.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/platform_fee_storage.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/platform_fee_storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/plugin_map.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/plugin_map.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/primary_sale.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/primary_sale.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/proxy.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/proxy.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/proxy_for_upgradeable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/proxy_for_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/reentrancy_guard.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/reentrancy_guard.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/reentrancy_guard_logic.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/reentrancy_guard_logic.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/reentrancy_guard_storage.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/reentrancy_guard_storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/reentrancy_guard_upgradeable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/reentrancy_guard_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/router.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/router.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/router_immutable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/router_immutable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/router_storage.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/router_storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/royalty.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/royalty.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/safe_cast.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/safe_cast.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/safe_erc20.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/safe_erc20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/safe_math.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/safe_math.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/signature_action.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/signature_action.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/signature_action_upgradeable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/signature_action_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/signature_drop.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/signature_drop.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/signature_mint_erc1155.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/signature_mint_erc1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/signature_mint_erc1155_upgradeable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/signature_mint_erc1155_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/signature_mint_erc20.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/signature_mint_erc20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/signature_mint_erc20_upgradeable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/signature_mint_erc20_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/signature_mint_erc721.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/signature_mint_erc721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/signature_mint_erc721_upgradeable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/signature_mint_erc721_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/signaturedrop_v4.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/signaturedrop_v4.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/soulbound_erc721_a.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/soulbound_erc721_a.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/split.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/split.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/staking1155.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/staking1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/staking1155_base.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/staking1155_base.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/staking1155_upgradeable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/staking1155_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/staking20.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/staking20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/staking20_base.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/staking20_base.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/staking20_upgradeable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/staking20_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/staking721.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/staking721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/staking721_base.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/staking721_base.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/staking721_upgradeable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/staking721_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/t_w_address.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/t_w_address.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/t_w_bit_maps.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/t_w_bit_maps.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/t_w_factory.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/t_w_factory.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/t_w_fee.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/t_w_fee.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/t_w_multichain_registry.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/t_w_multichain_registry.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/t_w_multichain_registry_logic.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/t_w_multichain_registry_logic.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/t_w_multichain_registry_router.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/t_w_multichain_registry_router.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/t_w_multichain_registry_storage.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/t_w_multichain_registry_storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/t_w_proxy.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/t_w_proxy.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/t_w_registry.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/t_w_registry.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/t_w_storage_slot.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/t_w_storage_slot.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/t_w_strings.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/t_w_strings.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/tiered_drop.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/tiered_drop.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/token_bundle.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/token_bundle.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/token_erc1155.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/token_erc1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/token_erc20.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/token_erc20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/token_erc721.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/token_erc721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/token_stake.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/token_stake.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/token_store.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/token_store.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/upgradeable.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/abi/vote_erc20.py` & `thirdweb_sdk-3.1.0a0/thirdweb/abi/vote_erc20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/common/claim_conditions.py` & `thirdweb_sdk-3.1.0a0/thirdweb/common/claim_conditions.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/common/currency.py` & `thirdweb_sdk-3.1.0a0/thirdweb/common/currency.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/common/error.py` & `thirdweb_sdk-3.1.0a0/thirdweb/common/error.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/common/feature_detection.py` & `thirdweb_sdk-3.1.0a0/thirdweb/common/feature_detection.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/common/marketplace.py` & `thirdweb_sdk-3.1.0a0/thirdweb/common/marketplace.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/common/merkle_tree.py` & `thirdweb_sdk-3.1.0a0/thirdweb/common/merkle_tree.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/common/nft.py` & `thirdweb_sdk-3.1.0a0/thirdweb/common/nft.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/common/sign.py` & `thirdweb_sdk-3.1.0a0/thirdweb/common/sign.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/common/snapshots.py` & `thirdweb_sdk-3.1.0a0/thirdweb/common/snapshots.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/constants/addresses.py` & `thirdweb_sdk-3.1.0a0/thirdweb/constants/addresses.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/constants/currency.py` & `thirdweb_sdk-3.1.0a0/thirdweb/constants/currency.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/constants/role.py` & `thirdweb_sdk-3.1.0a0/thirdweb/constants/role.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/constants/rpc.py` & `thirdweb_sdk-3.1.0a0/thirdweb/constants/rpc.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/contracts/custom.py` & `thirdweb_sdk-3.1.0a0/thirdweb/contracts/custom.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,23 +38,27 @@
 
 class CustomContract(BaseContract[Any]):
     """
     An SDK interface for a custom contract instance.
 
     ```python
     from thirdweb import ThirdwebSDK
+    from thirdweb.types import SDKOptions
+
+    # Get your secret key from the thirdweb api keys dashboard
+    secret_key = "..."
 
     # You can customize this to a supported network or your own RPC URL
     network = "mumbai"
 
     # Now we can create a new instance of the SDK
-    sdk = ThirdwebSDK(network)
+    sdk = ThirdwebSDK(network, options=SDKOptions(secret_key=secret_key))
 
     # If you want to send transactions, you can instantiate the SDK with a private key instead:
-    #   sdk = ThirdwebSDK.from_private_key(PRIVATE_KEY, network)
+    #   sdk = ThirdwebSDK.from_private_key(PRIVATE_KEY, network, options=SDKOptions(secret_key=secret_key))
 
     contract = sdk.get_contract("{{contract_address}}")
 
     # If your contract follows the ERC721 standard, contract.nft will be present
     nfts = contract.nft.get_all()
 
     # You can call any contract read function as follows
```

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/contracts/edition.py` & `thirdweb_sdk-3.1.0a0/thirdweb/contracts/edition.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,23 +29,27 @@
 
 class Edition(ERC1155Standard[TokenERC1155]):
     """
     Create a collection of NFTs that lets you mint multiple copies of each NFT.
 
     ```python
     from thirdweb import ThirdwebSDK
+    from thirdweb.types import SDKOptions
+
+    # Get your secret key from the thirdweb api keys dashboard
+    secret_key = "..."
 
     # You can customize this to a supported network or your own RPC URL
     network = "mumbai"
 
     # Now we can create a new instance of the SDK
-    sdk = ThirdwebSDK(network)
+    sdk = ThirdwebSDK(network, options=SDKOptions(secret_key=secret_key))
 
     # If you want to send transactions, you can instantiate the SDK with a private key instead:
-    #   sdk = ThirdwebSDK.from_private_key(PRIVATE_KEY, network)
+    #   sdk = ThirdwebSDK.from_private_key(PRIVATE_KEY, network, options=SDKOptions(secret_key=secret_key))
 
     contract = sdk.get_edition("{{contract_address}}")
     ```
     """
 
     _abi_type = TokenERC1155
```

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/contracts/edition_drop.py` & `thirdweb_sdk-3.1.0a0/thirdweb/contracts/edition_drop.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,23 +26,27 @@
 
 class EditionDrop(ERC1155Standard[DropERC1155]):
     """
     Setup a collection of NFTs with a customizable number of each NFT that are minted as users claim them.
 
     ```python
     from thirdweb import ThirdwebSDK
+    from thirdweb.types import SDKOptions
+
+    # Get your secret key from the thirdweb api keys dashboard
+    secret_key = "..."
 
     # You can customize this to a supported network or your own RPC URL
     network = "mumbai"
 
     # Now we can create a new instance of the SDK
-    sdk = ThirdwebSDK(network)
+    sdk = ThirdwebSDK(network, options=SDKOptions(secret_key=secret_key))
 
     # If you want to send transactions, you can instantiate the SDK with a private key instead:
-    #   sdk = ThirdwebSDK.from_private_key(PRIVATE_KEY, network)
+    #   sdk = ThirdwebSDK.from_private_key(PRIVATE_KEY, network, options=SDKOptions(secret_key=secret_key))
 
     contract = sdk.get_edition_drop("{{contract_address}}")
     ```
     """
 
     _abi_type = DropERC1155
```

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/contracts/maps.py` & `thirdweb_sdk-3.1.0a0/thirdweb/contracts/maps.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/contracts/marketplace.py` & `thirdweb_sdk-3.1.0a0/thirdweb/contracts/marketplace.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,23 +32,27 @@
 
 class Marketplace(BaseContract[MarketplaceABI]):
     """
     Create your own whitelabel marketplace that enables users to buy and sell any digital assets.
 
     ```python
     from thirdweb import ThirdwebSDK
+    from thirdweb.types import SDKOptions
+
+    # Get your secret key from the thirdweb api keys dashboard
+    secret_key = "..."
 
     # You can customize this to a supported network or your own RPC URL
     network = "mumbai"
 
     # Now we can create a new instance of the SDK
-    sdk = ThirdwebSDK(network)
+    sdk = ThirdwebSDK(network, options=SDKOptions(secret_key=secret_key))
 
     # If you want to send transactions, you can instantiate the SDK with a private key instead:
-    #   sdk = ThirdwebSDK.from_private_key(PRIVATE_KEY, network)
+    #   sdk = ThirdwebSDK.from_private_key(PRIVATE_KEY, network, options=SDKOptions(secret_key=secret_key))
 
     contract = sdk.get_marketplace("{{contract_address}}")
     ```
     """
 
     _abi_type = MarketplaceABI
     _storage: IpfsStorage
```

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/contracts/multiwrap.py` & `thirdweb_sdk-3.1.0a0/thirdweb/contracts/multiwrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,23 +38,27 @@
 class Multiwrap(ERC721Standard[MultiwrapABI]):
     """
     Multiwrap lets you wrap any number of ERC20, ERC721, or ERC1155 tokens into
     a single wrapped token bundle.
 
     ```python
     from thirdweb import ThirdwebSDK
+    from thirdweb.types import SDKOptions
+
+    # Get your secret key from the thirdweb api keys dashboard
+    secret_key = "..."
 
     # You can customize this to a supported network or your own RPC URL
     network = "mumbai"
 
     # Now we can create a new instance of the SDK
-    sdk = ThirdwebSDK(network)
+    sdk = ThirdwebSDK(network, options=SDKOptions(secret_key=secret_key))
 
     # If you want to send transactions, you can instantiate the SDK with a private key instead:
-    #   sdk = ThirdwebSDK.from_private_key(PRIVATE_KEY, network)
+    #   sdk = ThirdwebSDK.from_private_key(PRIVATE_KEY, network, options=SDKOptions(secret_key=secret_key))
 
     contract = sdk.get_multiwrap("{{contract_address}}")
     ```
     """
 
     _abi_type = MultiwrapABI
```

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/contracts/nft_collection.py` & `thirdweb_sdk-3.1.0a0/thirdweb/contracts/nft_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,23 +27,27 @@
 
 class NFTCollection(ERC721Standard[TokenERC721]):
     """
     Create a collection of one-of-one NFTs.
 
     ```python
     from thirdweb import ThirdwebSDK
+    from thirdweb.types import SDKOptions
+
+    # Get your secret key from the thirdweb api keys dashboard
+    secret_key = "..."
 
     # You can customize this to a supported network or your own RPC URL
     network = "mumbai"
 
     # Now we can create a new instance of the SDK
-    sdk = ThirdwebSDK(network)
+    sdk = ThirdwebSDK(network, options=SDKOptions(secret_key=secret_key))
 
     # If you want to send transactions, you can instantiate the SDK with a private key instead:
-    #   sdk = ThirdwebSDK.from_private_key(PRIVATE_KEY, network)
+    #   sdk = ThirdwebSDK.from_private_key(PRIVATE_KEY, network, options=SDKOptions(secret_key=secret_key))
 
     contract = sdk.get_nft_collection("{{contract_address}}")
     ```
     """
 
     _abi_type = TokenERC721
```

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/contracts/nft_drop.py` & `thirdweb_sdk-3.1.0a0/thirdweb/contracts/nft_drop.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,23 +29,27 @@
 
 class NFTDrop(ERC721Standard[DropERC721]):
     """
     Setup a collection of one-of-one NFTs that are minted as users claim them.
 
     ```python
     from thirdweb import ThirdwebSDK
+    from thirdweb.types import SDKOptions
+
+    # Get your secret key from the thirdweb api keys dashboard
+    secret_key = "..."
 
     # You can customize this to a supported network or your own RPC URL
     network = "mumbai"
 
     # Now we can create a new instance of the SDK
-    sdk = ThirdwebSDK(network)
+    sdk = ThirdwebSDK(network, options=SDKOptions(secret_key=secret_key))
 
     # If you want to send transactions, you can instantiate the SDK with a private key instead:
-    #   sdk = ThirdwebSDK.from_private_key(PRIVATE_KEY, network)
+    #   sdk = ThirdwebSDK.from_private_key(PRIVATE_KEY, network, options=SDKOptions(secret_key=secret_key))
 
     contract = sdk.get_nft_drop("{{contract_address}}")
     ```
     """
 
     _abi_type = DropERC721
```

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/contracts/token.py` & `thirdweb_sdk-3.1.0a0/thirdweb/contracts/token.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,23 +24,27 @@
 
 class Token(ERC20Standard):
     """
     Create a standard crypto token or cryptocurrency.
 
     ```python
     from thirdweb import ThirdwebSDK
+    from thirdweb.types import SDKOptions
+
+    # Get your secret key from the thirdweb api keys dashboard
+    secret_key = "..."
 
     # You can customize this to a supported network or your own RPC URL
     network = "mumbai"
 
     # Now we can create a new instance of the SDK
-    sdk = ThirdwebSDK(network)
+    sdk = ThirdwebSDK(network, options=SDKOptions(secret_key=secret_key))
 
     # If you want to send transactions, you can instantiate the SDK with a private key instead:
-    #   sdk = ThirdwebSDK.from_private_key(PRIVATE_KEY, network)
+    #   sdk = ThirdwebSDK.from_private_key(PRIVATE_KEY, network, options=SDKOptions(secret_key=secret_key))
 
     contract = sdk.get_token("{{contract_address}}")
     ```
     """
 
     _abi_type = TokenERC20
```

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/auth/wallet_authenticator.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/auth/wallet_authenticator.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/classes/base_contract.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/classes/base_contract.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/classes/contract_deployer.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/classes/contract_deployer.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,17 +26,17 @@
     __registry: ContractRegistry
 
     _storage: IpfsStorage
 
     def __init__(
         self,
         provider: Web3,
-        signer: Optional[LocalAccount] = None,
-        options: SDKOptions = SDKOptions(),
-        storage: IpfsStorage = IpfsStorage(),
+        signer: Optional[LocalAccount],
+        options: SDKOptions,
+        storage: IpfsStorage,
     ):
         super().__init__(provider, signer, options)
         self._storage = storage
 
     def deploy_nft_collection(self, metadata: NFTCollectionContractMetadata) -> str:
         """
         Deploy an NFT Collection contract.
```

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/classes/contract_events.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/classes/contract_events.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/classes/contract_metadata.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/classes/contract_metadata.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/classes/contract_platform_fee.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/classes/contract_platform_fee.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/classes/contract_roles.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/classes/contract_roles.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/classes/contract_royalty.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/classes/contract_royalty.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/classes/contract_sales.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/classes/contract_sales.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/classes/contract_wrapper.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/classes/contract_wrapper.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/classes/drop_claim_conditions.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/classes/drop_claim_conditions.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/classes/drop_erc1155_claim_conditions.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/classes/drop_erc1155_claim_conditions.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/classes/erc_1155.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/classes/erc_1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/classes/erc_1155_signature_minting.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/classes/erc_1155_signature_minting.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/classes/erc_1155_standard.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/classes/erc_1155_standard.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/classes/erc_20.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/classes/erc_20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/classes/erc_20_signature_minting.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/classes/erc_20_signature_minting.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/classes/erc_20_standard.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/classes/erc_20_standard.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/classes/erc_721.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/classes/erc_721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/classes/erc_721_signature_minting.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/classes/erc_721_signature_minting.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/classes/erc_721_standard.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/classes/erc_721_standard.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/classes/factory.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/classes/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,30 +40,28 @@
 class ContractFactory(ContractWrapper[TWFactory]):
     _storage: IpfsStorage
 
     def __init__(
         self,
         factory_address: str,
         provider: Web3,
-        signer: Optional[LocalAccount] = None,
-        options: SDKOptions = SDKOptions(),
-        storage: IpfsStorage = IpfsStorage(),
+        signer: Optional[LocalAccount],
+        options: SDKOptions,
+        storage: IpfsStorage,
     ):
         abi = TWFactory(provider, factory_address)
         super().__init__(abi, provider, signer, options)
         self._storage = storage
 
     def deploy(
         self, contract_type: ContractType, contract_metadata: Dict[str, Any]
     ) -> str:
         # First, we upload the contract metadata to IPFS
         contract_uri = self._storage.upload_metadata(
-            contract_metadata,
-            self._contract_abi.contract_address,
-            self.get_signer_address(),
+            contract_metadata
         )
 
         # Then, we get setup the contract interface for the contract we want to deploy
         contract = CONTRACTS_MAP[contract_type]
         interface = self.get_provider().eth.contract(
             address=cast(Address, self._contract_abi.contract_address),
             abi=contract._abi_type.abi(),
```

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/classes/ipfs_storage.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/classes/ipfs_storage.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from abc import ABC
 from io import IOBase
 import re
 import json
 from requests import get, Response, post
-from typing import Any, Dict, List, Sequence, TextIO, BinaryIO, Union, cast
+from typing import Any, Dict, List, Optional, Sequence, TextIO, BinaryIO, Union, cast
 from thirdweb.common.error import (
     DuplicateFileNameException,
     FetchException,
     UploadException,
 )
+from thirdweb.common.keys import derive_client_id_from_secret_key
 from thirdweb.constants.urls import (
     DEFAULT_IPFS_GATEWAY,
-    PINATA_IPFS_URL,
-    TW_IPFS_SERVER_URL,
+    TW_STORAGE_SERVER_URL,
 )
 from thirdweb.core.helpers.storage import (
     replace_file_properties_with_hashes,
     replace_gateway_url_with_hash,
     replace_hash_with_gateway_url,
     resolve_gateway_url,
 )
@@ -37,17 +37,26 @@
 
     # Now all the IPFS functions will be available on the sdk.storage name space
     sdk.storage.get("<IPFS_HASH>")
     ```
     """
 
     _gateway_url: str
+    _secret_key: Optional[str]
 
-    def __init__(self, gateway_url=DEFAULT_IPFS_GATEWAY):
-        self._gateway_url = re.sub(r"\/$", "", gateway_url) + "/"
+    def __init__(self, secret_key: Optional[str], gateway_url: Optional[str] = None):
+        self._secret_key = secret_key
+
+        if gateway_url is not None:
+            self._gateway_url = re.sub(r"\/$", "", gateway_url) + "/"
+        elif secret_key is not None:
+            client_id = derive_client_id_from_secret_key(self._secret_key)
+            self._gateway_url = f"https://{client_id}.ipfscdn.io/ipfs/"
+        else:
+            self._gateway_url = DEFAULT_IPFS_GATEWAY
 
     def get(self, hash: str) -> Any:
         """
         Gets IPFS data at a given hash and returns the data.
 
         :param hash: hash of the data to get.
         :returns: dictionary of the data if JSON, otherwise raw data.
@@ -59,119 +68,89 @@
 
             if isinstance(data, dict) or isinstance(data, list) or isinstance(data, str):
                 return replace_hash_with_gateway_url(data, "ipfs://", self._gateway_url)
             return data
         except:
             return res.text
 
-    def get_upload_token(self, contract_address: str) -> str:
-        """
-        Gets an upload token for a given contract address.
-
-        :param contract_address: address of the contract to get the token for.
-        :returns: upload token.
-        """
-
-        res = get(
-            f"{TW_IPFS_SERVER_URL}/grant",
-            headers={
-                "X-App-Name": f"CONSOLE-PYTHON-SDK-{contract_address}",
-            },
-        )
-
-        if not res.ok:
-            raise FetchException("Failed to upload token")
-
-        return res.text
-
     def upload(
         self,
         data: Union[TextIO, BinaryIO, str],
-        contract_address: str = "",
-        signer_address: str = "",
     ) -> str:
         """
         Uploads data to IPFS and returns the hash of the data.
 
         :param data: data to upload.
         :param contract_address: optional address of the contract to get the token for.
         :param signer_address: optional address of the signer to get the token for.
         :returns: hash of the data.
         """
 
-        cid = self.upload_batch([data], 0, contract_address, signer_address)
+        cid = self.upload_batch([data], 0)
         return f"{cid}0"
 
     def upload_batch(
         self,
         files: Sequence[Union[TextIO, BinaryIO, str, Dict[str, Any]]],
         file_start_number: int = 0,
-        contract_address: str = "",
-        signer_address: str = "",
     ) -> str:
         """
         Uploads a list of files to IPFS and returns the hash.
 
         :param files: list of files to upload.
         :param file_start_number: optional number to start the file names with.
         :param contract_address: optional address of the contract to get the token for.
         :param signer_address: optional address of the signer to get the token for.
         :returns: hash of the data.
         """
 
         cid_with_filename = self._upload_batch_with_cid(
             files,
             file_start_number,
-            contract_address,
-            signer_address,
         )
 
         return f"ipfs://{cid_with_filename.cid}"
 
     def upload_metadata(
         self,
         metadata: Dict[str, Any],
-        contract_address: str = "",
-        signer_address: str = "",
     ) -> str:
         """
         Uploads metadata to IPFS and returns the hash of the metadata.
 
         :param metadata: metadata to upload.
         :param contract_address: optional address of the contract to get the token for.
         :param signer_address: optional address of the signer to get the token for.
         :returns: hash of the metadata.
         """
 
         uri_with_metadata = self.upload_metadata_batch(
-            [metadata], 0, contract_address, signer_address
+            [metadata], 0
         )
 
         return uri_with_metadata.metadata_uris[0]
 
     def upload_metadata_batch(
         self,
         metadatas: Sequence[Dict[str, Any]],
         file_start_number: int = 0,
-        contract_address: str = "",
-        signer_address: str = "",
     ) -> UriWithMetadata:
         """
         Uploads a list of metadata to IPFS and returns the hash.
 
         :param metadatas: list of metadata to upload.
         :param file_start_number: optional number to start the file names with.
         :param contract_address: optional address of the contract to get the token for.
         :param signer_address: optional address of the signer to get the token for.
         :returns: hash of the metadata.
         """
 
         metadata_to_upload = self._batch_upload_properties(metadatas)
         cid_with_filename = self._upload_batch_with_cid(
-            metadata_to_upload, file_start_number, contract_address, signer_address
+            metadata_to_upload, file_start_number
         )
 
         base_uri = f"ipfs://{cid_with_filename.cid}/"
         metadata_uris = [
             f"{base_uri}{filename}" for filename in cid_with_filename.filenames
         ]
 
@@ -179,15 +158,16 @@
 
     """
     INTERNAL FUNCTIONS
     """
 
     def _get(self, hash: str) -> Response:
         hash = resolve_gateway_url(hash, "ipfs://", self._gateway_url)
-        res = get(hash)
+        headers = { "x-secret-key": self._secret_key } if ".ipfscdn.io" in self._gateway_url else {}
+        res = get(hash, headers=headers)
 
         if not res.ok:
             raise FetchException(f"Could not get {hash}")
 
         return res
 
     def _batch_upload_properties(self, metadatas: Sequence[Dict[str, Any]]):
@@ -230,30 +210,16 @@
                 elif isinstance(val, dict) or isinstance(val, list):
                     self._build_file_properties_map(val, files)
         return files
 
     def _upload_batch_with_cid(
         self,
         files: Sequence[Union[TextIO, BinaryIO, str, Dict[str, Any]]],
-        file_start_number: int = 0,
-        contract_address: str = "",
-        signer_address: str = "",
+        file_start_number: int = 0
     ) -> CidWithFileName:
-
-        token = self.get_upload_token(contract_address)
-
-        metadata = {
-            "name": f"CONSOLE-PYTHON-SDK-{contract_address}",
-            "keyvalues": {
-                "sdk": "python",
-                "contractAddress": contract_address,
-                "signerAddress": signer_address,
-            },
-        }
-
         form: List[Any] = []
         file_names: List[str] = []
 
         for i, file in enumerate(files):
             file_name = f"{file_start_number + i}"
             file_data = cast(Union[str, Dict[str, Any]], file)
 
@@ -279,18 +245,18 @@
 
             file_names.append(file_name)
             form.append(("file", (f"files/{file_name}", file_data)))
 
         # form.append(("pinataMetadata", metadata))
 
         res = post(
-            PINATA_IPFS_URL,
+            f"{TW_STORAGE_SERVER_URL}/ipfs/upload",
             files=form,
             headers={
-                "Authorization": f"Bearer {token}",
+                "x-secret-key": self._secret_key,
             },
         )
         body = res.json()
 
         if not res.ok:
             raise UploadException(f"Failed to upload files to IPFS. {res.json()}")
```

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/classes/marketplace_auction.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/classes/marketplace_auction.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/classes/marketplace_direct.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/classes/marketplace_direct.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/classes/provider_handler.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/classes/provider_handler.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/classes/registry.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/classes/registry.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/classes/sharded_merkle_tree.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/classes/sharded_merkle_tree.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/helpers/storage.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/helpers/storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/core/sdk.py` & `thirdweb_sdk-3.1.0a0/thirdweb/core/sdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from eth_account import Account
 from thirdweb.common.feature_detection import (
     fetch_contract_metadata_from_address,
 )
+from thirdweb.common.keys import derive_client_id_from_secret_key
 from thirdweb.constants.urls import get_provider_for_network
 from thirdweb.contracts import Marketplace
 from thirdweb.contracts.custom import CustomContract
 from thirdweb.contracts.edition_drop import EditionDrop
 from thirdweb.contracts.nft_drop import NFTDrop
 from thirdweb.contracts.multiwrap import Multiwrap
 from thirdweb.core.auth.wallet_authenticator import WalletAuthenticator
@@ -52,27 +53,34 @@
         sdk = ThirdwebSDK(network, signer, options)
         return sdk
 
     def __init__(
         self,
         network: str,
         signer: Optional[LocalAccount] = None,
-        options: SDKOptions = SDKOptions(),
-        storage: IpfsStorage = IpfsStorage(),
+        options: SDKOptions = None,
+        storage: IpfsStorage = None,
     ):
         """
         Initialize the thirdweb SDK.
 
         :param provider: web3 provider instance to use for getting on-chain data
         :param signer: signer to use for sending transactions
         :param options: optional SDK configuration options
         :param storage: optional IPFS storage instance to use for storing data
         """
 
-        provider = get_provider_for_network(network)
+        if options is None:
+            options = SDKOptions()
+
+        if storage is None:
+            storage = IpfsStorage(options.secret_key)
+
+        client_id = derive_client_id_from_secret_key(options.secret_key) if options.secret_key is not None else None
+        provider = get_provider_for_network(network, client_id)
         super().__init__(provider, signer, options)
 
         self.auth = WalletAuthenticator(provider, signer, options)
         self.deployer = ContractDeployer(provider, signer, options, storage)
         self.storage = storage
 
     def get_nft_collection(self, address: str) -> NFTCollection:
```

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/types/auth.py` & `thirdweb_sdk-3.1.0a0/thirdweb/types/auth.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/types/contract.py` & `thirdweb_sdk-3.1.0a0/thirdweb/types/contract.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/types/contracts/claim_conditions.py` & `thirdweb_sdk-3.1.0a0/thirdweb/types/contracts/claim_conditions.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/types/contracts/signature.py` & `thirdweb_sdk-3.1.0a0/thirdweb/types/contracts/signature.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/types/currency.py` & `thirdweb_sdk-3.1.0a0/thirdweb/types/currency.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/types/events.py` & `thirdweb_sdk-3.1.0a0/thirdweb/types/events.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/types/marketplace.py` & `thirdweb_sdk-3.1.0a0/thirdweb/types/marketplace.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/types/multiwrap.py` & `thirdweb_sdk-3.1.0a0/thirdweb/types/multiwrap.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/types/nft.py` & `thirdweb_sdk-3.1.0a0/thirdweb/types/nft.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/types/sdk.py` & `thirdweb_sdk-3.1.0a0/thirdweb/types/sdk.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,9 +42,10 @@
     """
     Optional settings to configure the SDK
 
     :param read_only_settings: optional read-only RPC settings
     :param gas_settings: gas settings
     """
 
+    secret_key: Optional[str] = None
     read_only_settings: Optional[ReadOnlySettings] = None
     gas_settings: GasSettings = GasSettings()
```

### Comparing `thirdweb_sdk-3.0.3a0/thirdweb/types/settings/metadata.py` & `thirdweb_sdk-3.1.0a0/thirdweb/types/settings/metadata.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.3a0/PKG-INFO` & `thirdweb_sdk-3.1.0a0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thirdweb-sdk
-Version: 3.0.3a0
+Version: 3.1.0a0
 Summary: 
 Author: thirdweb
 Author-email: sdk@thirdweb.com
 Requires-Python: >=3.7.1
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -40,25 +40,29 @@
 
 ```bash
 pip install thirdweb-sdk
 ```
 
 ## Getting Started
 
-To start using this SDK, you just need to pass in a provider configuration.
+To start using this SDK, you just need to pass in a provider configuration. It's also strongly recommended that you use your thirdweb API keys with the SDK in order to get the best infrastructure performance (across RPCs, IPFS, etc.) - you can learn more about creating and using API keys [here](https://portal.thirdweb.com/api-keys).
 
 ### Instantiating the SDK
 
 Once you have all the necessary dependencies, you can follow the following setup steps to get started with the SDK read-only functions:
 
 ```python
 from thirdweb import ThirdwebSDK
+from thirdweb.types import SDKOptions
 
-# You can create a new instance of the SDK to use by just passing in a network name
-sdk = ThirdwebSDK("mumbai")
+# Get your secret key from the thirdweb api keys dashboard
+SECRET_KEY = "..."
+
+# You can create a new instance of the SDK to use by passing in a network name and your api key
+sdk = ThirdwebSDK("mumbai", options=SDKOptions(secret_key=SECRET_KEY))
 ```
 
 The SDK supports the `mainnet`, `rinkeby`, `goerli`, `polygon`, `mumbai`, `fantom`, and `avalanche` networks.
 
 Alternatively, if you want to use your own custom RPC URL, you can pass in the RPC URL directly as follows:
 
 ```python
@@ -92,20 +96,24 @@
 > :warning: Never commit private keys to file tracking history, or your account could be compromised.
 
 Meanwhile, if you want to use write functions as well and connect a signer, you can use the following setup:
 
 ```python
 from thirdweb import ThirdwebSDK
 from thirdweb.types.nft import NFTMetadataInput
+import os
+
+# Get your secret key from the thirdweb api keys dashboard
+SECRET_KEY = "..."
 
-# Learn more about securely accessing your private key: https://portal.thirdweb.com/web3-sdk/set-up-the-sdk/securing-your-private-key
-PRIVATE_KEY = "<your-private-key-here>",
+# This PRIVATE KEY is coming from your environment variables. Make sure to never put it in a tracked file or share it with anyone.
+PRIVATE_KEY = os.environ.get("PRIVATE_KEY")
 
 # Now you can create a new instance of the SDK with your private key
-sdk = ThirdwebSDK.from_private_key(PRIVATE_KEY, "mumbai")
+sdk = ThirdwebSDK.from_private_key(PRIVATE_KEY, "mumbai", options=SDKOptions(secret_key=SECRET_KEY))
 
 # Instantiate a new NFT Collection contract as described above.
 NFT_COLLECTION_ADDRESS = "0x.."
 nft_collection = sdk.get_nft_collection(NFT_COLLECTION_ADDRESS)
 
 # Now you can use any of the SDK contract functions including write functions
 nft_collection.mint(NFTMetadataInput.from_json({ "name": "Cool NFT", "description": "Minted with the Python SDK!" }))
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thirdweb-sdk Version: 3.0.3a0 Summary: Author:
+Metadata-Version: 2.1 Name: thirdweb-sdk Version: 3.1.0a0 Summary: Author:
 thirdweb Author-email: sdk@thirdweb.com Requires-Python: >=3.7.1 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: cbor2 (>=5.4.3,<6.0.0) Requires-Dist: dacite
 (>=1.6.0,<2.0.0) Requires-Dist: mypy-extensions (>=0.4.3,<0.5.0) Requires-Dist:
 pyee (>=9.0.4,<10.0.0) Requires-Dist: pymerkle (>=2.0.2,<3.0.0) Requires-Dist:
@@ -12,72 +12,79 @@
 
 
                        ****** thirdweb Python SDK ******
                [pypi_version] [Build_Status] [Join_our_Discord!]
                     Best in class Web3 SDK for Python 3.7+
 
 ## Installation ```bash pip install thirdweb-sdk ``` ## Getting Started To
-start using this SDK, you just need to pass in a provider configuration. ###
-Instantiating the SDK Once you have all the necessary dependencies, you can
-follow the following setup steps to get started with the SDK read-only
-functions: ```python from thirdweb import ThirdwebSDK # You can create a new
-instance of the SDK to use by just passing in a network name sdk = ThirdwebSDK
-("mumbai") ``` The SDK supports the `mainnet`, `rinkeby`, `goerli`, `polygon`,
-`mumbai`, `fantom`, and `avalanche` networks. Alternatively, if you want to use
-your own custom RPC URL, you can pass in the RPC URL directly as follows:
-```python from thirdweb import ThirdwebSDK # Set your RPC_URL RPC_URL = "https:
-//rpc-mainnet.matic.network" # And now you can instantiate the SDK with it sdk
-= ThirdwebSDK(RPC_URL) ``` ### Working With Contracts Once you instantiate the
-SDK, you can use it to access your thirdweb contracts. You can use the SDK's
-contract getter functions like `get_token`, `get_edition`,
-`get_nft_collection`, and `get_marketplace` to get the respective SDK contract
-instances. To use an NFT Collection contract for example, you can do the
-following. ```python # Add your NFT Collection contract address here
-NFT_COLLECTION_ADDRESS = "0x.." # And you can instantiate your contract with
-just one line nft_collection = sdk.get_nft_collection(NFT_COLLECTION_ADDRESS) #
-Now you can use any of the read-only SDK contract functions nfts =
-nft_collection.get_all() print(nfts) ``` ### Signing Transactions > :warning:
-Never commit private keys to file tracking history, or your account could be
-compromised. Meanwhile, if you want to use write functions as well and connect
-a signer, you can use the following setup: ```python from thirdweb import
-ThirdwebSDK from thirdweb.types.nft import NFTMetadataInput # Learn more about
-securely accessing your private key: https://portal.thirdweb.com/web3-sdk/set-
-up-the-sdk/securing-your-private-key PRIVATE_KEY = "", # Now you can create a
-new instance of the SDK with your private key sdk =
-ThirdwebSDK.from_private_key(PRIVATE_KEY, "mumbai") # Instantiate a new NFT
-Collection contract as described above. NFT_COLLECTION_ADDRESS = "0x.."
-nft_collection = sdk.get_nft_collection(NFT_COLLECTION_ADDRESS) # Now you can
-use any of the SDK contract functions including write functions
-nft_collection.mint(NFTMetadataInput.from_json({ "name": "Cool NFT",
-"description": "Minted with the Python SDK!" })) ``` ## Development Environment
-In this section, we'll go over the steps to get started with running the Python
-SDK repository locally and contributing to the code. If you aren't interested
-in contributing to the thirdweb Python SDK, you can ignore this section. ###
-Poetry Environment Setup If you want to work with this repository, make sure to
-setup [Poetry](https://python-poetry.org/docs/), you're virtual environment,
-and the code styling tools. Assuming you've installed and setup poetry, you can
-setup this repository with: ```bash $ make init ``` ### Running Tests Once you
-have run the initialization step, you can run the following to run all tests:
-```bash $ make test ``` ### Publishing the Package To make a build & publish
-the package, you need to have a `pypi` account with permission to edit the
-`thirdweb-sdk` pypi package. You can authenticate your pypi account with poetry
-with the following command: ```bash poetry config pypi-token.pypi pypi-token-
-here ``` Then, you can build and release a prerelease version with the
-following command: ```bash make publish ``` ### Code Style Setup Make sure you
-have `mypy`, `pylint`, and `black` installed (all included in the dev
-dependencies with `poetry install`. If you're working in VSCode, there a few
-steps to get everything working with the poetry .venv: 1. To setup poetry
-virtual environment inside your VSCode so it gets recognized as part of your
-project (import for linters), you can take the following steps from this [stack
-overflow answer](https://stackoverflow.com/questions/59882884/vscode-doesnt-
-show-poetry-virtualenvs-in-select-interpreter-option). You need to run `poetry
-config virtualenvs.in-project true` and then make sure you delete/create a new
-poetry env. 2. In `.vscode/settings.json`, you should have the following:
-```json { "python.linting.mypyEnabled": true, "python.linting.enabled": true,
-"python.linting.pylintEnabled": false } ``` 3. Make sure to set your VSCode
-`Python: Interpreter` setting to the Python version inside your poetry virtual
-environment. ### Generate Python ABI Wrappers Use the [abi-gen](https://
-www.npmjs.com/package/@0x/abi-gen) package to create the Python ABIs. You can
-install it with the following command: ```bash $ npm install -g @0x/abi-gen ```
-Assuming you have the thirdweb contract ABIs in this directory at `/abi`, you
-can run the following command to generate the necessary ABIs. ```bash $ make
-abi ```
+start using this SDK, you just need to pass in a provider configuration. It's
+also strongly recommended that you use your thirdweb API keys with the SDK in
+order to get the best infrastructure performance (across RPCs, IPFS, etc.) -
+you can learn more about creating and using API keys [here](https://
+portal.thirdweb.com/api-keys). ### Instantiating the SDK Once you have all the
+necessary dependencies, you can follow the following setup steps to get started
+with the SDK read-only functions: ```python from thirdweb import ThirdwebSDK
+from thirdweb.types import SDKOptions # Get your secret key from the thirdweb
+api keys dashboard SECRET_KEY = "..." # You can create a new instance of the
+SDK to use by passing in a network name and your api key sdk = ThirdwebSDK
+("mumbai", options=SDKOptions(secret_key=SECRET_KEY)) ``` The SDK supports the
+`mainnet`, `rinkeby`, `goerli`, `polygon`, `mumbai`, `fantom`, and `avalanche`
+networks. Alternatively, if you want to use your own custom RPC URL, you can
+pass in the RPC URL directly as follows: ```python from thirdweb import
+ThirdwebSDK # Set your RPC_URL RPC_URL = "https://rpc-mainnet.matic.network" #
+And now you can instantiate the SDK with it sdk = ThirdwebSDK(RPC_URL) ``` ###
+Working With Contracts Once you instantiate the SDK, you can use it to access
+your thirdweb contracts. You can use the SDK's contract getter functions like
+`get_token`, `get_edition`, `get_nft_collection`, and `get_marketplace` to get
+the respective SDK contract instances. To use an NFT Collection contract for
+example, you can do the following. ```python # Add your NFT Collection contract
+address here NFT_COLLECTION_ADDRESS = "0x.." # And you can instantiate your
+contract with just one line nft_collection = sdk.get_nft_collection
+(NFT_COLLECTION_ADDRESS) # Now you can use any of the read-only SDK contract
+functions nfts = nft_collection.get_all() print(nfts) ``` ### Signing
+Transactions > :warning: Never commit private keys to file tracking history, or
+your account could be compromised. Meanwhile, if you want to use write
+functions as well and connect a signer, you can use the following setup:
+```python from thirdweb import ThirdwebSDK from thirdweb.types.nft import
+NFTMetadataInput import os # Get your secret key from the thirdweb api keys
+dashboard SECRET_KEY = "..." # This PRIVATE KEY is coming from your environment
+variables. Make sure to never put it in a tracked file or share it with anyone.
+PRIVATE_KEY = os.environ.get("PRIVATE_KEY") # Now you can create a new instance
+of the SDK with your private key sdk = ThirdwebSDK.from_private_key
+(PRIVATE_KEY, "mumbai", options=SDKOptions(secret_key=SECRET_KEY)) #
+Instantiate a new NFT Collection contract as described above.
+NFT_COLLECTION_ADDRESS = "0x.." nft_collection = sdk.get_nft_collection
+(NFT_COLLECTION_ADDRESS) # Now you can use any of the SDK contract functions
+including write functions nft_collection.mint(NFTMetadataInput.from_json(
+{ "name": "Cool NFT", "description": "Minted with the Python SDK!" })) ``` ##
+Development Environment In this section, we'll go over the steps to get started
+with running the Python SDK repository locally and contributing to the code. If
+you aren't interested in contributing to the thirdweb Python SDK, you can
+ignore this section. ### Poetry Environment Setup If you want to work with this
+repository, make sure to setup [Poetry](https://python-poetry.org/docs/),
+you're virtual environment, and the code styling tools. Assuming you've
+installed and setup poetry, you can setup this repository with: ```bash $ make
+init ``` ### Running Tests Once you have run the initialization step, you can
+run the following to run all tests: ```bash $ make test ``` ### Publishing the
+Package To make a build & publish the package, you need to have a `pypi`
+account with permission to edit the `thirdweb-sdk` pypi package. You can
+authenticate your pypi account with poetry with the following command: ```bash
+poetry config pypi-token.pypi pypi-token-here ``` Then, you can build and
+release a prerelease version with the following command: ```bash make publish
+``` ### Code Style Setup Make sure you have `mypy`, `pylint`, and `black`
+installed (all included in the dev dependencies with `poetry install`. If
+you're working in VSCode, there a few steps to get everything working with the
+poetry .venv: 1. To setup poetry virtual environment inside your VSCode so it
+gets recognized as part of your project (import for linters), you can take the
+following steps from this [stack overflow answer](https://stackoverflow.com/
+questions/59882884/vscode-doesnt-show-poetry-virtualenvs-in-select-interpreter-
+option). You need to run `poetry config virtualenvs.in-project true` and then
+make sure you delete/create a new poetry env. 2. In `.vscode/settings.json`,
+you should have the following: ```json { "python.linting.mypyEnabled": true,
+"python.linting.enabled": true, "python.linting.pylintEnabled": false } ``` 3.
+Make sure to set your VSCode `Python: Interpreter` setting to the Python
+version inside your poetry virtual environment. ### Generate Python ABI
+Wrappers Use the [abi-gen](https://www.npmjs.com/package/@0x/abi-gen) package
+to create the Python ABIs. You can install it with the following command:
+```bash $ npm install -g @0x/abi-gen ``` Assuming you have the thirdweb
+contract ABIs in this directory at `/abi`, you can run the following command to
+generate the necessary ABIs. ```bash $ make abi ```
```

