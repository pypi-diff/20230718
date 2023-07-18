# Comparing `tmp/formance-sdk-python-1.0.20230714.tar.gz` & `tmp/formance-sdk-python-1.0.20230718.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formance-sdk-python-1.0.20230714.tar", last modified: Fri Jul 14 09:39:56 2023, max compression
+gzip compressed data, was "formance-sdk-python-1.0.20230718.tar", last modified: Tue Jul 18 10:36:34 2023, max compression
```

## Comparing `formance-sdk-python-1.0.20230714.tar` & `formance-sdk-python-1.0.20230718.tar`

### file list

```diff
@@ -1,299 +1,297 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:39:56.642732 formance-sdk-python-1.0.20230714/
--rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-07-14 09:39:56.642732 formance-sdk-python-1.0.20230714/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     9914 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 09:39:56.642732 formance-sdk-python-1.0.20230714/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1188 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:39:56.598731 formance-sdk-python-1.0.20230714/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:39:56.598731 formance-sdk-python-1.0.20230714/src/formance_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-07-14 09:39:56.000000 formance-sdk-python-1.0.20230714/src/formance_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-07-14 09:39:56.000000 formance-sdk-python-1.0.20230714/src/formance_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:39:56.000000 formance-sdk-python-1.0.20230714/src/formance_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-14 09:39:56.000000 formance-sdk-python-1.0.20230714/src/formance_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-14 09:39:56.000000 formance-sdk-python-1.0.20230714/src/formance_sdk_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:39:56.598731 formance-sdk-python-1.0.20230714/src/sdk/
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23184 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/auth.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17573 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/flows.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33109 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/ledger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:39:56.602731 formance-sdk-python-1.0.20230714/src/sdk/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:39:56.614731 formance-sdk-python-1.0.20230714/src/sdk/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7015 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1046 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/activateconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1149 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/addmetadataontransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1232 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/addmetadatatoaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      791 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/addscopetoclient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/addtransientscope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      784 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/cancelevent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1296 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/changeconfigsecret.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/confirmhold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      653 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/connectorsstripetransfer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1129 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/connectorstransfer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1652 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/countaccounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3181 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/counttransactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1293 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/createbalance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      643 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/createclient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      636 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/createscope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1103 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/createsecret.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1719 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/createtransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1221 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/createtransactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      854 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/createwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      799 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/createworkflow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1060 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/creditwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1052 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/deactivateconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1299 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/debitwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      634 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/deleteclient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      837 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/deleteconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      629 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/deletescope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      801 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/deletescopefromclient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      786 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/deletesecret.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      825 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/deletetransientscope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      744 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/flowsgetserverinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1256 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/getaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1155 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/getbalance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/getbalances.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1300 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/getbalancesaggregated.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1052 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/getconnectortask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1019 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/gethold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1954 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/getholds.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      791 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/getinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/getinstance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1105 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/getinstancehistory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1301 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/getinstancestagehistory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/getledgerinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1259 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/getmanyconfigs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      992 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/getmapping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      820 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/getpayment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      597 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/getserverinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1169 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/gettransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1712 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/gettransactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      625 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/getversions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1002 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/getwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1060 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/getwalletsummary.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      985 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/getworkflow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      842 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/insertconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      841 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/installconnector.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4055 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/listaccounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      625 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/listallconnectors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/listbalances.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      638 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/listclients.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      674 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/listconfigsavailableconnectors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      940 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/listconnectorstransfers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1538 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/listconnectortasks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1207 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/listinstances.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3221 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/listlogs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1511 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/listpayments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      631 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/listscopes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4816 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/listtransactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      624 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/listusers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1752 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/listwallets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      794 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/listworkflows.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      605 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/paymentsgetserverinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1527 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/paymentslistaccounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      842 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/readclient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      963 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/readconnectorconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      831 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/readscope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      979 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/readstats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      820 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/readuser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      730 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/resetconnector.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1175 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/reverttransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1927 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/runscript.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1334 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/runworkflow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      603 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/searchgetserverinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1219 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/sendevent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1015 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/testconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      738 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/uninstallconnector.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1103 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/updateclient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1161 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/updatemapping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      850 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/updatemetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1087 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/updatescope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/updatewallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      813 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/voidhold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      815 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/operations/walletsgetserverinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:39:56.642732 formance-sdk-python-1.0.20230714/src/sdk/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10411 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      589 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/accountresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1399 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/accountscursor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1391 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/accountscursorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1318 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/accountwithvolumesandbalances.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/activityconfirmhold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      787 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/activitycreatetransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/activitycreatetransactionoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      790 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/activitycreditwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      785 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/activitydebitwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      485 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/activitydebitwalletoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      538 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/activitygetaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      584 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/activitygetaccountoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      420 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/activitygetpayment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      496 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/activitygetpaymentoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      419 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/activitygetwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      539 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/activitygetwalletoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      545 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/activityreverttransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/activityreverttransactionoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1511 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/activitystripetransfer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      418 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/activityvoidhold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      456 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/aggregatebalancesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      432 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/assetholder.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2179 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/attempt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      501 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/attemptresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/balance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1347 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/balancescursorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1150 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/balancewithassets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      826 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/bankingcircleconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2136 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/client.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      877 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/clientsecret.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      508 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      428 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/configchangesecret.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      720 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/configinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      516 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/configinforesponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      554 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/configresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      899 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/configsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      759 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/configuser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      815 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/confirmholdrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/connector.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      466 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/connectorconfigresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1389 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/connectorsconfigsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1027 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/connectorsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      682 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/contract.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1024 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/createbalancerequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      520 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/createbalanceresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1591 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/createclientrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      598 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/createclientresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      648 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/createscoperequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      592 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/createscoperesponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      647 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/createsecretrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      598 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/createsecretresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      611 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/createwalletrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      514 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/createwalletresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/createworkflowrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      526 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/createworkflowresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1228 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/creditwalletrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1149 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/currencycloudconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1540 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/debitwalletrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      536 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/debitwalletresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1062 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/dummypayconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      703 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/error.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      972 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/errorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      407 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/errorsenum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1495 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/expandeddebithold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      557 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/getbalanceresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/getholdresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1420 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/getholdsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1494 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/gettransactionsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/getversionsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/getwalletresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1146 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/getwalletsummaryresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      617 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/getworkflowinstancehistoryresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      648 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/getworkflowinstancehistorystageresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/getworkflowinstanceresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      519 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/getworkflowresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1152 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/hold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      552 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/ledgeraccountsubject.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1070 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/ledgerinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/ledgerinforesponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      549 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/ledgerstorage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1452 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/listbalancesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      604 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/listclientsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/listrunsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      598 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/listscopesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      592 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/listusersresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1434 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/listwalletsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      532 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/listworkflowsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1255 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/log.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1363 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/logscursorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      499 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/mapping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      585 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/mappingresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1346 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/migrationinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      754 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/modulrconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      623 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/monetary.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3120 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/payment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1277 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/paymentadjustment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/paymentmetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      501 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/paymentresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1309 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/paymentsaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1367 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/paymentscursor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      320 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/paymentstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      779 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/posting.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2230 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/posttransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1958 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/query.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      598 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/readclientresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      592 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/readscoperesponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      586 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/readuserresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2507 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/response.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/runworkflowresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      931 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/scope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/script.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1917 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/scriptresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      987 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/secret.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      313 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      452 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/serverinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      891 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/stagedelay.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1147 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/stagesend.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1300 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/stagesenddestination.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      631 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/stagesenddestinationaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/stagesenddestinationpayment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      632 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/stagesenddestinationwallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1235 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/stagesendsource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      626 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/stagesendsourceaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/stagesendsourcepayment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      627 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/stagesendsourcewallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1399 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/stagestatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      422 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/stagewaitevent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      549 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      491 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/statsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1008 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/stripeconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1508 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/stripetransferrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      206 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/stripetransferresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2346 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/taskbankingcircle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2178 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/taskcurrencycloud.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2500 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/taskdummypay.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2492 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/taskmodulr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      455 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/taskresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/taskscursor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2378 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/taskstripe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2482 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/taskwise.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1866 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/transaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1294 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/transactiondata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      521 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/transactionresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      538 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/transactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1419 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/transactionscursorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      528 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/transactionsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      871 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/transferrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      516 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/transferresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2045 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/transfersresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1591 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/updateclientrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      598 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/updateclientresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      648 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/updatescoperequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      592 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/updatescoperesponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      838 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      652 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      736 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/volume.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1198 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/wallet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      712 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/walletserrorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2076 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/walletstransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/walletsubject.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      659 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/walletsvolume.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1662 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/walletwithbalances.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1498 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/webhooksconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      900 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/webhookserrorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      507 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/webhookserrorsenum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/wiseconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1212 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/workflow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      644 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/workflowconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2038 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/workflowinstance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1528 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/workflowinstancehistory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2667 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/workflowinstancehistorystage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3397 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/workflowinstancehistorystageinput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2340 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/models/shared/workflowinstancehistorystageoutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21682 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/payments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4327 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      993 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/sdkconfiguration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3036 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:39:56.642732 formance-sdk-python-1.0.20230714/src/sdk/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3762 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/utils/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24619 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/wallets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12342 2023-07-14 09:39:42.000000 formance-sdk-python-1.0.20230714/src/sdk/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:36:34.410211 formance-sdk-python-1.0.20230718/
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-18 10:36:34.410211 formance-sdk-python-1.0.20230718/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9412 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 10:36:34.410211 formance-sdk-python-1.0.20230718/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1118 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:36:34.346211 formance-sdk-python-1.0.20230718/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:36:34.350211 formance-sdk-python-1.0.20230718/src/formance_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-18 10:36:34.000000 formance-sdk-python-1.0.20230718/src/formance_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-07-18 10:36:34.000000 formance-sdk-python-1.0.20230718/src/formance_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 10:36:34.000000 formance-sdk-python-1.0.20230718/src/formance_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-18 10:36:34.000000 formance-sdk-python-1.0.20230718/src/formance_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-18 10:36:34.000000 formance-sdk-python-1.0.20230718/src/formance_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:36:34.354211 formance-sdk-python-1.0.20230718/src/sdk/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20635 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16276 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/flows.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30317 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/ledger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:36:34.354211 formance-sdk-python-1.0.20230718/src/sdk/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:36:34.370211 formance-sdk-python-1.0.20230718/src/sdk/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6913 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1050 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/activateconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1153 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/addmetadataontransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1236 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/addmetadatatoaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      795 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/addscopetoclient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      823 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/addtransientscope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/cancelevent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1300 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/changeconfigsecret.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1067 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/confirmhold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      545 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/connectorsstripetransfer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1133 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/connectorstransfer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1453 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/countaccounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2997 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/counttransactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/createbalance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      645 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/createclient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      638 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/createscope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1107 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/createsecret.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1723 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/createtransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/createtransactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      856 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/createwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      801 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/createworkflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1064 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/creditwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1056 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/deactivateconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1303 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/debitwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      638 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/deleteclient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      841 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/deleteconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      633 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/deletescope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      805 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/deletescopefromclient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      790 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/deletesecret.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      829 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/deletetransientscope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      746 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/flowsgetserverinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1260 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1159 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getbalance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2443 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getbalances.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1304 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getbalancesaggregated.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1056 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getconnectortask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/gethold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1958 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getholds.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      793 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1051 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getinstance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1109 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getinstancehistory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1305 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getinstancestagehistory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1018 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getledgerinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1263 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getmanyconfigs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      996 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getmapping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getpayment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      599 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getserverinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1173 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/gettransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1716 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/gettransactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      627 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getversions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1006 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1064 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getwalletsummary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      989 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/getworkflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      844 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/insertconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      845 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/installconnector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3889 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listaccounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      627 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listallconnectors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      823 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listbalances.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      640 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listclients.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      676 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listconfigsavailableconnectors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      944 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listconnectorstransfers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1542 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listconnectortasks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1211 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listinstances.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3229 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listlogs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1515 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listpayments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      633 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listscopes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4638 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listtransactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      626 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listusers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1756 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listwallets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      796 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/listworkflows.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/paymentsgetserverinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1531 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/paymentslistaccounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      846 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/readclient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      967 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/readconnectorconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      835 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/readscope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      983 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/readstats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/readuser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      734 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/resetconnector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1179 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/reverttransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1935 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/runscript.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1338 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/runworkflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      570 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      605 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/searchgetserverinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/sendevent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1019 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/testconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      742 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/uninstallconnector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1107 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/updateclient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1165 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/updatemapping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      854 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/updatemetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1091 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/updatescope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1334 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/updatewallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/voidhold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/operations/walletsgetserverinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:36:34.410211 formance-sdk-python-1.0.20230718/src/sdk/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9954 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      813 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      591 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/accountresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1403 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/accountscursor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1395 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/accountscursorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1222 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/accountwithvolumesandbalances.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activityconfirmhold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      789 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitycreatetransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      527 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitycreatetransactionoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitycreditwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      787 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitydebitwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      487 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitydebitwalletoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      540 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitygetaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      586 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitygetaccountoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      422 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitygetpayment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      498 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitygetpaymentoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitygetwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      541 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitygetwalletoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      547 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activityreverttransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      527 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activityreverttransactionoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1250 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitystripetransfer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      420 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/activityvoidhold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      458 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/aggregatebalancesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      434 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/assetholder.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2181 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/attempt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/attemptresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1013 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/balance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1351 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/balancescursorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1152 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/balancewithassets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      828 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/bankingcircleconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2138 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/client.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      879 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/clientsecret.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      510 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      430 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/configchangesecret.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      722 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/configinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      518 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/configinforesponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      556 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/configresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      903 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/configsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      761 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/configuser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/confirmholdrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/connector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      468 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/connectorconfigresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1397 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/connectorsconfigsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1031 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/connectorsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      636 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/contract.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1026 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/createbalancerequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      522 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/createbalanceresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1593 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/createclientrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/createclientresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      650 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/createscoperequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      594 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/createscoperesponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      649 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/createsecretrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/createsecretresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      613 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/createwalletrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      516 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/createwalletresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      653 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/createworkflowrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      528 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/createworkflowresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/creditwalletrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1151 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/currencycloudconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1542 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/debitwalletrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      538 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/debitwalletresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1064 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/dummypayconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      705 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/error.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      974 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/errorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      407 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/errorsenum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1497 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/expandeddebithold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      559 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/getbalanceresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      546 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/getholdresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1424 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/getholdsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1498 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/gettransactionsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/getversionsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      553 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/getwalletresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/getwalletsummaryresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/getworkflowinstancehistoryresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      650 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/getworkflowinstancehistorystageresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      570 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/getworkflowinstanceresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      521 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/getworkflowresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1154 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/hold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      554 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/ledgeraccountsubject.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1074 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/ledgerinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      602 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/ledgerinforesponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/ledgerstorage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1456 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/listbalancesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      606 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/listclientsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      570 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/listrunsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/listscopesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      594 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/listusersresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1438 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/listwalletsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      534 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/listworkflowsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1237 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/log.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1367 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/logscursorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      501 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/mapping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      587 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/mappingresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/migrationinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      756 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/modulrconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      625 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/monetary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3096 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/payment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1233 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/paymentadjustment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      505 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/paymentmetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/paymentresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/paymentsaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1371 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/paymentscursor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      320 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/paymentstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      781 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/posting.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2155 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/posttransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1920 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/query.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/readclientresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      594 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/readscoperesponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/readuserresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2380 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/response.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      562 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/runworkflowresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      933 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/scope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1059 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/script.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1923 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/scriptresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      989 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/secret.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      315 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      454 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/serverinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      893 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagedelay.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1149 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesend.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1302 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesenddestination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      633 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesenddestinationaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      433 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesenddestinationpayment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      634 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesenddestinationwallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1237 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesendsource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      628 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesendsourceaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      426 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesendsourcepayment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      629 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesendsourcewallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1401 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagestatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagewaitevent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      493 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/statsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1010 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stripeconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1249 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/stripetransferrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2282 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskbankingcircle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2114 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskcurrencycloud.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2446 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskdummypay.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2442 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskmodulr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      457 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1301 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskscursor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2328 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskstripe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2436 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskwise.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1868 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/transaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1296 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/transactiondata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      523 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/transactionresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      540 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/transactionscursorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      530 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/transactionsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      873 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/transferrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      518 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/transferresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2049 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/transfersresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1593 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/updateclientrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/updateclientresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      650 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/updatescoperequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      594 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/updatescoperesponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      840 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/user.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      654 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      738 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/volume.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1200 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/wallet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      714 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/walletserrorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2078 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/walletstransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/walletsubject.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      661 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/walletsvolume.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1666 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/walletwithbalances.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1500 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/webhooksconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      902 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/webhookserrorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      507 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/webhookserrorsenum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/wiseconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1214 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/workflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      646 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/workflowconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2040 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/workflowinstance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1530 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/workflowinstancehistory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2669 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/workflowinstancehistorystage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3399 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/workflowinstancehistorystageinput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2342 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/models/shared/workflowinstancehistorystageoutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19606 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/payments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5284 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3152 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:36:34.410211 formance-sdk-python-1.0.20230718/src/sdk/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/utils/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22535 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/wallets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11685 2023-07-18 10:36:21.000000 formance-sdk-python-1.0.20230718/src/sdk/webhooks.py
```

### Comparing `formance-sdk-python-1.0.20230714/src/formance_sdk_python.egg-info/SOURCES.txt` & `formance-sdk-python-1.0.20230718/src/formance_sdk_python.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 src/formance_sdk_python.egg-info/top_level.txt
 src/sdk/__init__.py
 src/sdk/auth.py
 src/sdk/flows.py
 src/sdk/ledger.py
 src/sdk/payments.py
 src/sdk/sdk.py
-src/sdk/sdkconfiguration.py
 src/sdk/search.py
 src/sdk/wallets.py
 src/sdk/webhooks.py
 src/sdk/models/__init__.py
 src/sdk/models/operations/__init__.py
 src/sdk/models/operations/activateconfig.py
 src/sdk/models/operations/addmetadataontransaction.py
@@ -238,15 +237,14 @@
 src/sdk/models/shared/stagesendsourcewallet.py
 src/sdk/models/shared/stagestatus.py
 src/sdk/models/shared/stagewaitevent.py
 src/sdk/models/shared/stats.py
 src/sdk/models/shared/statsresponse.py
 src/sdk/models/shared/stripeconfig.py
 src/sdk/models/shared/stripetransferrequest.py
-src/sdk/models/shared/stripetransferresponse.py
 src/sdk/models/shared/taskbankingcircle.py
 src/sdk/models/shared/taskcurrencycloud.py
 src/sdk/models/shared/taskdummypay.py
 src/sdk/models/shared/taskmodulr.py
 src/sdk/models/shared/taskresponse.py
 src/sdk/models/shared/taskscursor.py
 src/sdk/models/shared/taskstripe.py
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/auth.py` & `formance-sdk-python-1.0.20230718/src/sdk/auth.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,76 +1,86 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-from .sdkconfiguration import SDKConfiguration
-from sdk import utils
+import requests as requests_http
+from . import utils
 from sdk.models import operations, shared
 from typing import Optional
 
 class Auth:
-    sdk_configuration: SDKConfiguration
-
-    def __init__(self, sdk_config: SDKConfiguration) -> None:
-        self.sdk_configuration = sdk_config
+    _client: requests_http.Session
+    _security_client: requests_http.Session
+    _server_url: str
+    _language: str
+    _sdk_version: str
+    _gen_version: str
+
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+        self._client = client
+        self._security_client = security_client
+        self._server_url = server_url
+        self._language = language
+        self._sdk_version = sdk_version
+        self._gen_version = gen_version
         
     
     def add_scope_to_client(self, request: operations.AddScopeToClientRequest) -> operations.AddScopeToClientResponse:
         r"""Add scope to client"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.AddScopeToClientRequest, base_url, '/api/auth/clients/{clientId}/scopes/{scopeId}', request)
         headers = {}
         headers['Accept'] = '*/*'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('PUT', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.AddScopeToClientResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
 
         return res
 
     
     def add_transient_scope(self, request: operations.AddTransientScopeRequest) -> operations.AddTransientScopeResponse:
         r"""Add a transient scope to a scope
         Add a transient scope to a scope
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.AddTransientScopeRequest, base_url, '/api/auth/scopes/{scopeId}/transient/{transientScopeId}', request)
         headers = {}
         headers['Accept'] = '*/*'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('PUT', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.AddTransientScopeResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
 
         return res
 
     
     def create_client(self, request: shared.CreateClientRequest) -> operations.CreateClientResponse:
         r"""Create client"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
-        url = base_url + '/api/auth/clients'
+        url = base_url.removesuffix('/') + '/api/auth/clients'
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CreateClientResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 201:
@@ -81,25 +91,25 @@
         return res
 
     
     def create_scope(self, request: shared.CreateScopeRequest) -> operations.CreateScopeResponse:
         r"""Create scope
         Create scope
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
-        url = base_url + '/api/auth/scopes'
+        url = base_url.removesuffix('/') + '/api/auth/scopes'
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CreateScopeResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 201:
@@ -108,25 +118,25 @@
                 res.create_scope_response = out
 
         return res
 
     
     def create_secret(self, request: operations.CreateSecretRequest) -> operations.CreateSecretResponse:
         r"""Add a secret to a client"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.CreateSecretRequest, base_url, '/api/auth/clients/{clientId}/secrets', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "create_secret_request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CreateSecretResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -135,126 +145,126 @@
                 res.create_secret_response = out
 
         return res
 
     
     def delete_client(self, request: operations.DeleteClientRequest) -> operations.DeleteClientResponse:
         r"""Delete client"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.DeleteClientRequest, base_url, '/api/auth/clients/{clientId}', request)
         headers = {}
         headers['Accept'] = '*/*'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('DELETE', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.DeleteClientResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
 
         return res
 
     
     def delete_scope(self, request: operations.DeleteScopeRequest) -> operations.DeleteScopeResponse:
         r"""Delete scope
         Delete scope
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.DeleteScopeRequest, base_url, '/api/auth/scopes/{scopeId}', request)
         headers = {}
         headers['Accept'] = '*/*'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('DELETE', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.DeleteScopeResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
 
         return res
 
     
     def delete_scope_from_client(self, request: operations.DeleteScopeFromClientRequest) -> operations.DeleteScopeFromClientResponse:
         r"""Delete scope from client"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.DeleteScopeFromClientRequest, base_url, '/api/auth/clients/{clientId}/scopes/{scopeId}', request)
         headers = {}
         headers['Accept'] = '*/*'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('DELETE', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.DeleteScopeFromClientResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
 
         return res
 
     
     def delete_secret(self, request: operations.DeleteSecretRequest) -> operations.DeleteSecretResponse:
         r"""Delete a secret from a client"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.DeleteSecretRequest, base_url, '/api/auth/clients/{clientId}/secrets/{secretId}', request)
         headers = {}
         headers['Accept'] = '*/*'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('DELETE', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.DeleteSecretResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
 
         return res
 
     
     def delete_transient_scope(self, request: operations.DeleteTransientScopeRequest) -> operations.DeleteTransientScopeResponse:
         r"""Delete a transient scope from a scope
         Delete a transient scope from a scope
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.DeleteTransientScopeRequest, base_url, '/api/auth/scopes/{scopeId}/transient/{transientScopeId}', request)
         headers = {}
         headers['Accept'] = '*/*'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('DELETE', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.DeleteTransientScopeResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
 
         return res
 
     
     def get_server_info(self) -> operations.GetServerInfoResponse:
         r"""Get server info"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
-        url = base_url + '/api/auth/_info'
+        url = base_url.removesuffix('/') + '/api/auth/_info'
         headers = {}
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetServerInfoResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -263,22 +273,22 @@
                 res.server_info = out
 
         return res
 
     
     def list_clients(self) -> operations.ListClientsResponse:
         r"""List clients"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
-        url = base_url + '/api/auth/clients'
+        url = base_url.removesuffix('/') + '/api/auth/clients'
         headers = {}
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListClientsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -289,22 +299,22 @@
         return res
 
     
     def list_scopes(self) -> operations.ListScopesResponse:
         r"""List scopes
         List Scopes
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
-        url = base_url + '/api/auth/scopes'
+        url = base_url.removesuffix('/') + '/api/auth/scopes'
         headers = {}
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListScopesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -315,22 +325,22 @@
         return res
 
     
     def list_users(self) -> operations.ListUsersResponse:
         r"""List users
         List users
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
-        url = base_url + '/api/auth/users'
+        url = base_url.removesuffix('/') + '/api/auth/users'
         headers = {}
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListUsersResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -339,22 +349,22 @@
                 res.list_users_response = out
 
         return res
 
     
     def read_client(self, request: operations.ReadClientRequest) -> operations.ReadClientResponse:
         r"""Read client"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.ReadClientRequest, base_url, '/api/auth/clients/{clientId}', request)
         headers = {}
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ReadClientResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -365,22 +375,22 @@
         return res
 
     
     def read_scope(self, request: operations.ReadScopeRequest) -> operations.ReadScopeResponse:
         r"""Read scope
         Read scope
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.ReadScopeRequest, base_url, '/api/auth/scopes/{scopeId}', request)
         headers = {}
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ReadScopeResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -391,22 +401,22 @@
         return res
 
     
     def read_user(self, request: operations.ReadUserRequest) -> operations.ReadUserResponse:
         r"""Read user
         Read user
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.ReadUserRequest, base_url, '/api/auth/users/{userId}', request)
         headers = {}
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ReadUserResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -415,25 +425,25 @@
                 res.read_user_response = out
 
         return res
 
     
     def update_client(self, request: operations.UpdateClientRequest) -> operations.UpdateClientResponse:
         r"""Update client"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.UpdateClientRequest, base_url, '/api/auth/clients/{clientId}', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "update_client_request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('PUT', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.UpdateClientResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -444,25 +454,25 @@
         return res
 
     
     def update_scope(self, request: operations.UpdateScopeRequest) -> operations.UpdateScopeResponse:
         r"""Update scope
         Update scope
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.UpdateScopeRequest, base_url, '/api/auth/scopes/{scopeId}', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "update_scope_request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('PUT', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.UpdateScopeResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/flows.py` & `formance-sdk-python-1.0.20230718/src/sdk/flows.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-from .sdkconfiguration import SDKConfiguration
-from sdk import utils
+import requests as requests_http
+from . import utils
 from sdk.models import operations, shared
 from typing import Optional
 
 class Flows:
-    sdk_configuration: SDKConfiguration
-
-    def __init__(self, sdk_config: SDKConfiguration) -> None:
-        self.sdk_configuration = sdk_config
+    _client: requests_http.Session
+    _security_client: requests_http.Session
+    _server_url: str
+    _language: str
+    _sdk_version: str
+    _gen_version: str
+
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+        self._client = client
+        self._security_client = security_client
+        self._server_url = server_url
+        self._language = language
+        self._sdk_version = sdk_version
+        self._gen_version = gen_version
         
     
     def flowsget_server_info(self) -> operations.FlowsgetServerInfoResponse:
         r"""Get server info"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
-        url = base_url + '/api/orchestration/_info'
+        url = base_url.removesuffix('/') + '/api/orchestration/_info'
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.FlowsgetServerInfoResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -40,22 +50,22 @@
         return res
 
     
     def cancel_event(self, request: operations.CancelEventRequest) -> operations.CancelEventResponse:
         r"""Cancel a running workflow
         Cancel a running workflow
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.CancelEventRequest, base_url, '/api/orchestration/instances/{instanceID}/abort', request)
         headers = {}
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('PUT', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CancelEventResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 204:
@@ -68,25 +78,25 @@
         return res
 
     
     def create_workflow(self, request: shared.CreateWorkflowRequest) -> operations.CreateWorkflowResponse:
         r"""Create workflow
         Create a workflow
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
-        url = base_url + '/api/orchestration/workflows'
+        url = base_url.removesuffix('/') + '/api/orchestration/workflows'
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CreateWorkflowResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 201:
@@ -101,22 +111,22 @@
         return res
 
     
     def get_instance(self, request: operations.GetInstanceRequest) -> operations.GetInstanceResponse:
         r"""Get a workflow instance by id
         Get a workflow instance by id
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.GetInstanceRequest, base_url, '/api/orchestration/instances/{instanceID}', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetInstanceResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -131,22 +141,22 @@
         return res
 
     
     def get_instance_history(self, request: operations.GetInstanceHistoryRequest) -> operations.GetInstanceHistoryResponse:
         r"""Get a workflow instance history by id
         Get a workflow instance history by id
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.GetInstanceHistoryRequest, base_url, '/api/orchestration/instances/{instanceID}/history', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetInstanceHistoryResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -161,22 +171,22 @@
         return res
 
     
     def get_instance_stage_history(self, request: operations.GetInstanceStageHistoryRequest) -> operations.GetInstanceStageHistoryResponse:
         r"""Get a workflow instance stage history
         Get a workflow instance stage history
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.GetInstanceStageHistoryRequest, base_url, '/api/orchestration/instances/{instanceID}/stages/{number}/history', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetInstanceStageHistoryResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -191,22 +201,22 @@
         return res
 
     
     def get_workflow(self, request: operations.GetWorkflowRequest) -> operations.GetWorkflowResponse:
         r"""Get a flow by id
         Get a flow by id
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.GetWorkflowRequest, base_url, '/api/orchestration/workflows/{flowId}', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetWorkflowResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -221,23 +231,23 @@
         return res
 
     
     def list_instances(self, request: operations.ListInstancesRequest) -> operations.ListInstancesResponse:
         r"""List instances of a workflow
         List instances of a workflow
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
-        url = base_url + '/api/orchestration/instances'
+        url = base_url.removesuffix('/') + '/api/orchestration/instances'
         headers = {}
         query_params = utils.get_query_params(operations.ListInstancesRequest, request)
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, params=query_params, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListInstancesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -252,22 +262,22 @@
         return res
 
     
     def list_workflows(self) -> operations.ListWorkflowsResponse:
         r"""List registered workflows
         List registered workflows
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
-        url = base_url + '/api/orchestration/workflows'
+        url = base_url.removesuffix('/') + '/api/orchestration/workflows'
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListWorkflowsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -282,26 +292,26 @@
         return res
 
     
     def run_workflow(self, request: operations.RunWorkflowRequest) -> operations.RunWorkflowResponse:
         r"""Run workflow
         Run workflow
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.RunWorkflowRequest, base_url, '/api/orchestration/workflows/{workflowID}/instances', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         query_params = utils.get_query_params(operations.RunWorkflowRequest, request)
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.RunWorkflowResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 201:
@@ -316,25 +326,25 @@
         return res
 
     
     def send_event(self, request: operations.SendEventRequest) -> operations.SendEventResponse:
         r"""Send an event to a running workflow
         Send an event to a running workflow
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.SendEventRequest, base_url, '/api/orchestration/instances/{instanceID}/events', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.SendEventResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 204:
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/ledger.py` & `formance-sdk-python-1.0.20230718/src/sdk/ledger.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-from .sdkconfiguration import SDKConfiguration
-from sdk import utils
+import requests as requests_http
+from . import utils
 from sdk.models import operations, shared
 from typing import Optional
 
 class Ledger:
-    sdk_configuration: SDKConfiguration
-
-    def __init__(self, sdk_config: SDKConfiguration) -> None:
-        self.sdk_configuration = sdk_config
+    _client: requests_http.Session
+    _security_client: requests_http.Session
+    _server_url: str
+    _language: str
+    _sdk_version: str
+    _gen_version: str
+
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+        self._client = client
+        self._security_client = security_client
+        self._server_url = server_url
+        self._language = language
+        self._sdk_version = sdk_version
+        self._gen_version = gen_version
         
     
     def create_transactions(self, request: operations.CreateTransactionsRequest) -> operations.CreateTransactionsResponse:
         r"""Create a new batch of transactions to a ledger"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.CreateTransactionsRequest, base_url, '/api/ledger/{ledger}/transactions/batch', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "transactions", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CreateTransactionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -43,25 +53,25 @@
                 res.error_response = out
 
         return res
 
     
     def add_metadata_on_transaction(self, request: operations.AddMetadataOnTransactionRequest) -> operations.AddMetadataOnTransactionResponse:
         r"""Set the metadata of a transaction by its ID"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.AddMetadataOnTransactionRequest, base_url, '/api/ledger/{ledger}/transactions/{txid}/metadata', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.AddMetadataOnTransactionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 204:
@@ -72,27 +82,27 @@
                 res.error_response = out
 
         return res
 
     
     def add_metadata_to_account(self, request: operations.AddMetadataToAccountRequest) -> operations.AddMetadataToAccountResponse:
         r"""Add metadata to an account"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.AddMetadataToAccountRequest, base_url, '/api/ledger/{ledger}/accounts/{address}/metadata', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.AddMetadataToAccountResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 204:
@@ -103,23 +113,23 @@
                 res.error_response = out
 
         return res
 
     
     def count_accounts(self, request: operations.CountAccountsRequest) -> operations.CountAccountsResponse:
         r"""Count the accounts from a ledger"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.CountAccountsRequest, base_url, '/api/ledger/{ledger}/accounts', request)
         headers = {}
         query_params = utils.get_query_params(operations.CountAccountsRequest, request)
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('HEAD', url, params=query_params, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CountAccountsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -131,23 +141,23 @@
                 res.error_response = out
 
         return res
 
     
     def count_transactions(self, request: operations.CountTransactionsRequest) -> operations.CountTransactionsResponse:
         r"""Count the transactions from a ledger"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.CountTransactionsRequest, base_url, '/api/ledger/{ledger}/transactions', request)
         headers = {}
         query_params = utils.get_query_params(operations.CountTransactionsRequest, request)
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('HEAD', url, params=query_params, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CountTransactionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -159,28 +169,28 @@
                 res.error_response = out
 
         return res
 
     
     def create_transaction(self, request: operations.CreateTransactionRequest) -> operations.CreateTransactionResponse:
         r"""Create a new transaction to a ledger"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.CreateTransactionRequest, base_url, '/api/ledger/{ledger}/transactions', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "post_transaction", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
         query_params = utils.get_query_params(operations.CreateTransactionRequest, request)
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CreateTransactionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -193,22 +203,22 @@
                 res.error_response = out
 
         return res
 
     
     def get_account(self, request: operations.GetAccountRequest) -> operations.GetAccountResponse:
         r"""Get account by its address"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.GetAccountRequest, base_url, '/api/ledger/{ledger}/accounts/{address}', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetAccountResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -221,23 +231,23 @@
                 res.error_response = out
 
         return res
 
     
     def get_balances(self, request: operations.GetBalancesRequest) -> operations.GetBalancesResponse:
         r"""Get the balances from a ledger's account"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.GetBalancesRequest, base_url, '/api/ledger/{ledger}/balances', request)
         headers = {}
         query_params = utils.get_query_params(operations.GetBalancesRequest, request)
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, params=query_params, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetBalancesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -250,23 +260,23 @@
                 res.error_response = out
 
         return res
 
     
     def get_balances_aggregated(self, request: operations.GetBalancesAggregatedRequest) -> operations.GetBalancesAggregatedResponse:
         r"""Get the aggregated balances from selected accounts"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.GetBalancesAggregatedRequest, base_url, '/api/ledger/{ledger}/aggregate/balances', request)
         headers = {}
         query_params = utils.get_query_params(operations.GetBalancesAggregatedRequest, request)
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, params=query_params, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetBalancesAggregatedResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -279,22 +289,22 @@
                 res.error_response = out
 
         return res
 
     
     def get_info(self) -> operations.GetInfoResponse:
         r"""Show server information"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
-        url = base_url + '/api/ledger/_info'
+        url = base_url.removesuffix('/') + '/api/ledger/_info'
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetInfoResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -307,22 +317,22 @@
                 res.error_response = out
 
         return res
 
     
     def get_ledger_info(self, request: operations.GetLedgerInfoRequest) -> operations.GetLedgerInfoResponse:
         r"""Get information about a ledger"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.GetLedgerInfoRequest, base_url, '/api/ledger/{ledger}/_info', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetLedgerInfoResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -335,22 +345,22 @@
                 res.error_response = out
 
         return res
 
     
     def get_mapping(self, request: operations.GetMappingRequest) -> operations.GetMappingResponse:
         r"""Get the mapping of a ledger"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.GetMappingRequest, base_url, '/api/ledger/{ledger}/mapping', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetMappingResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -363,22 +373,22 @@
                 res.error_response = out
 
         return res
 
     
     def get_transaction(self, request: operations.GetTransactionRequest) -> operations.GetTransactionResponse:
         r"""Get transaction from a ledger by its ID"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.GetTransactionRequest, base_url, '/api/ledger/{ledger}/transactions/{txid}', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetTransactionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -393,23 +403,23 @@
         return res
 
     
     def list_accounts(self, request: operations.ListAccountsRequest) -> operations.ListAccountsResponse:
         r"""List accounts from a ledger
         List accounts from a ledger, sorted by address in descending order.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.ListAccountsRequest, base_url, '/api/ledger/{ledger}/accounts', request)
         headers = {}
         query_params = utils.get_query_params(operations.ListAccountsRequest, request)
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, params=query_params, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListAccountsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -424,23 +434,23 @@
         return res
 
     
     def list_logs(self, request: operations.ListLogsRequest) -> operations.ListLogsResponse:
         r"""List the logs from a ledger
         List the logs from a ledger, sorted by ID in descending order.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.ListLogsRequest, base_url, '/api/ledger/{ledger}/logs', request)
         headers = {}
         query_params = utils.get_query_params(operations.ListLogsRequest, request)
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, params=query_params, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListLogsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -455,23 +465,23 @@
         return res
 
     
     def list_transactions(self, request: operations.ListTransactionsRequest) -> operations.ListTransactionsResponse:
         r"""List transactions from a ledger
         List transactions from a ledger, sorted by txid in descending order.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.ListTransactionsRequest, base_url, '/api/ledger/{ledger}/transactions', request)
         headers = {}
         query_params = utils.get_query_params(operations.ListTransactionsRequest, request)
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, params=query_params, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListTransactionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -486,22 +496,22 @@
         return res
 
     
     def read_stats(self, request: operations.ReadStatsRequest) -> operations.ReadStatsResponse:
         r"""Get statistics from a ledger
         Get statistics from a ledger. (aggregate metrics on accounts and transactions)
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.ReadStatsRequest, base_url, '/api/ledger/{ledger}/stats', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ReadStatsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -514,22 +524,22 @@
                 res.error_response = out
 
         return res
 
     
     def revert_transaction(self, request: operations.RevertTransactionRequest) -> operations.RevertTransactionResponse:
         r"""Revert a ledger transaction by its ID"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.RevertTransactionRequest, base_url, '/api/ledger/{ledger}/transactions/{txid}/revert', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.RevertTransactionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -543,31 +553,31 @@
 
         return res
 
     
     def run_script(self, request: operations.RunScriptRequest) -> operations.RunScriptResponse:
         r"""Execute a Numscript
         This route is deprecated, and has been merged into `POST /{ledger}/transactions`.
-
+        
         Deprecated: this method will be removed in a future release, please migrate away from it as soon as possible
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.RunScriptRequest, base_url, '/api/ledger/{ledger}/script', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "script", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
         query_params = utils.get_query_params(operations.RunScriptRequest, request)
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.RunScriptResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -576,27 +586,27 @@
                 res.script_response = out
 
         return res
 
     
     def update_mapping(self, request: operations.UpdateMappingRequest) -> operations.UpdateMappingResponse:
         r"""Update the mapping of a ledger"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.UpdateMappingRequest, base_url, '/api/ledger/{ledger}/mapping', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "mapping", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('PUT', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.UpdateMappingResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/__init__.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,8 +89,8 @@
 from .updatemapping import *
 from .updatemetadata import *
 from .updatescope import *
 from .updatewallet import *
 from .voidhold import *
 from .walletsgetserverinfo import *
 
-__all__ = ["ActivateConfigRequest","ActivateConfigResponse","AddMetadataOnTransactionRequest","AddMetadataOnTransactionResponse","AddMetadataToAccountRequest","AddMetadataToAccountResponse","AddScopeToClientRequest","AddScopeToClientResponse","AddTransientScopeRequest","AddTransientScopeResponse","CancelEventRequest","CancelEventResponse","ChangeConfigSecretRequest","ChangeConfigSecretResponse","ConfirmHoldRequest","ConfirmHoldResponse","ConnectorsStripeTransferResponse","ConnectorsTransferRequest","ConnectorsTransferResponse","CountAccountsMetadata","CountAccountsRequest","CountAccountsResponse","CountTransactionsMetadata","CountTransactionsRequest","CountTransactionsResponse","CreateBalanceRequest","CreateBalanceResponse","CreateClientResponse","CreateScopeResponse","CreateSecretRequest","CreateSecretResponse","CreateTransactionRequest","CreateTransactionResponse","CreateTransactionsRequest","CreateTransactionsResponse","CreateWalletResponse","CreateWorkflowResponse","CreditWalletRequest","CreditWalletResponse","DeactivateConfigRequest","DeactivateConfigResponse","DebitWalletRequest","DebitWalletResponse","DeleteClientRequest","DeleteClientResponse","DeleteConfigRequest","DeleteConfigResponse","DeleteScopeFromClientRequest","DeleteScopeFromClientResponse","DeleteScopeRequest","DeleteScopeResponse","DeleteSecretRequest","DeleteSecretResponse","DeleteTransientScopeRequest","DeleteTransientScopeResponse","FlowsgetServerInfoResponse","GetAccountRequest","GetAccountResponse","GetBalanceRequest","GetBalanceResponse","GetBalancesAggregatedRequest","GetBalancesAggregatedResponse","GetBalancesRequest","GetBalancesResponse","GetConnectorTaskRequest","GetConnectorTaskResponse","GetHoldRequest","GetHoldResponse","GetHoldsRequest","GetHoldsResponse","GetInfoResponse","GetInstanceHistoryRequest","GetInstanceHistoryResponse","GetInstanceRequest","GetInstanceResponse","GetInstanceStageHistoryRequest","GetInstanceStageHistoryResponse","GetLedgerInfoRequest","GetLedgerInfoResponse","GetManyConfigsRequest","GetManyConfigsResponse","GetMappingRequest","GetMappingResponse","GetPaymentRequest","GetPaymentResponse","GetServerInfoResponse","GetTransactionRequest","GetTransactionResponse","GetTransactionsRequest","GetTransactionsResponse","GetVersionsResponse","GetWalletRequest","GetWalletResponse","GetWalletSummaryRequest","GetWalletSummaryResponse","GetWorkflowRequest","GetWorkflowResponse","InsertConfigResponse","InstallConnectorRequest","InstallConnectorResponse","ListAccountsBalanceOperator","ListAccountsMetadata","ListAccountsRequest","ListAccountsResponse","ListAllConnectorsResponse","ListBalancesRequest","ListBalancesResponse","ListClientsResponse","ListConfigsAvailableConnectorsResponse","ListConnectorTasksRequest","ListConnectorTasksResponse","ListConnectorsTransfersRequest","ListConnectorsTransfersResponse","ListInstancesRequest","ListInstancesResponse","ListLogsRequest","ListLogsResponse","ListPaymentsRequest","ListPaymentsResponse","ListScopesResponse","ListTransactionsMetadata","ListTransactionsRequest","ListTransactionsResponse","ListUsersResponse","ListWalletsRequest","ListWalletsResponse","ListWorkflowsResponse","PaymentsgetServerInfoResponse","PaymentslistAccountsRequest","PaymentslistAccountsResponse","ReadClientRequest","ReadClientResponse","ReadConnectorConfigRequest","ReadConnectorConfigResponse","ReadScopeRequest","ReadScopeResponse","ReadStatsRequest","ReadStatsResponse","ReadUserRequest","ReadUserResponse","ResetConnectorRequest","ResetConnectorResponse","RevertTransactionRequest","RevertTransactionResponse","RunScriptRequest","RunScriptResponse","RunWorkflowRequest","RunWorkflowResponse","SearchResponse","SearchgetServerInfoResponse","SendEventRequest","SendEventRequestBody","SendEventResponse","TestConfigRequest","TestConfigResponse","UninstallConnectorRequest","UninstallConnectorResponse","UpdateClientRequest","UpdateClientResponse","UpdateMappingRequest","UpdateMappingResponse","UpdateMetadataRequest","UpdateMetadataResponse","UpdateScopeRequest","UpdateScopeResponse","UpdateWalletRequest","UpdateWalletRequestBody","UpdateWalletResponse","VoidHoldRequest","VoidHoldResponse","WalletsgetServerInfoResponse"]
+__all__ = ["ActivateConfigRequest","ActivateConfigResponse","AddMetadataOnTransactionRequest","AddMetadataOnTransactionResponse","AddMetadataToAccountRequest","AddMetadataToAccountResponse","AddScopeToClientRequest","AddScopeToClientResponse","AddTransientScopeRequest","AddTransientScopeResponse","CancelEventRequest","CancelEventResponse","ChangeConfigSecretRequest","ChangeConfigSecretResponse","ConfirmHoldRequest","ConfirmHoldResponse","ConnectorsStripeTransferResponse","ConnectorsTransferRequest","ConnectorsTransferResponse","CountAccountsRequest","CountAccountsResponse","CountTransactionsRequest","CountTransactionsResponse","CreateBalanceRequest","CreateBalanceResponse","CreateClientResponse","CreateScopeResponse","CreateSecretRequest","CreateSecretResponse","CreateTransactionRequest","CreateTransactionResponse","CreateTransactionsRequest","CreateTransactionsResponse","CreateWalletResponse","CreateWorkflowResponse","CreditWalletRequest","CreditWalletResponse","DeactivateConfigRequest","DeactivateConfigResponse","DebitWalletRequest","DebitWalletResponse","DeleteClientRequest","DeleteClientResponse","DeleteConfigRequest","DeleteConfigResponse","DeleteScopeFromClientRequest","DeleteScopeFromClientResponse","DeleteScopeRequest","DeleteScopeResponse","DeleteSecretRequest","DeleteSecretResponse","DeleteTransientScopeRequest","DeleteTransientScopeResponse","FlowsgetServerInfoResponse","GetAccountRequest","GetAccountResponse","GetBalanceRequest","GetBalanceResponse","GetBalancesAggregatedRequest","GetBalancesAggregatedResponse","GetBalancesRequest","GetBalancesResponse","GetConnectorTaskRequest","GetConnectorTaskResponse","GetHoldRequest","GetHoldResponse","GetHoldsRequest","GetHoldsResponse","GetInfoResponse","GetInstanceHistoryRequest","GetInstanceHistoryResponse","GetInstanceRequest","GetInstanceResponse","GetInstanceStageHistoryRequest","GetInstanceStageHistoryResponse","GetLedgerInfoRequest","GetLedgerInfoResponse","GetManyConfigsRequest","GetManyConfigsResponse","GetMappingRequest","GetMappingResponse","GetPaymentRequest","GetPaymentResponse","GetServerInfoResponse","GetTransactionRequest","GetTransactionResponse","GetTransactionsRequest","GetTransactionsResponse","GetVersionsResponse","GetWalletRequest","GetWalletResponse","GetWalletSummaryRequest","GetWalletSummaryResponse","GetWorkflowRequest","GetWorkflowResponse","InsertConfigResponse","InstallConnectorRequest","InstallConnectorResponse","ListAccountsBalanceOperator","ListAccountsRequest","ListAccountsResponse","ListAllConnectorsResponse","ListBalancesRequest","ListBalancesResponse","ListClientsResponse","ListConfigsAvailableConnectorsResponse","ListConnectorTasksRequest","ListConnectorTasksResponse","ListConnectorsTransfersRequest","ListConnectorsTransfersResponse","ListInstancesRequest","ListInstancesResponse","ListLogsRequest","ListLogsResponse","ListPaymentsRequest","ListPaymentsResponse","ListScopesResponse","ListTransactionsRequest","ListTransactionsResponse","ListUsersResponse","ListWalletsRequest","ListWalletsResponse","ListWorkflowsResponse","PaymentsgetServerInfoResponse","PaymentslistAccountsRequest","PaymentslistAccountsResponse","ReadClientRequest","ReadClientResponse","ReadConnectorConfigRequest","ReadConnectorConfigResponse","ReadScopeRequest","ReadScopeResponse","ReadStatsRequest","ReadStatsResponse","ReadUserRequest","ReadUserResponse","ResetConnectorRequest","ResetConnectorResponse","RevertTransactionRequest","RevertTransactionResponse","RunScriptRequest","RunScriptResponse","RunWorkflowRequest","RunWorkflowResponse","SearchResponse","SearchgetServerInfoResponse","SendEventRequest","SendEventRequestBody","SendEventResponse","TestConfigRequest","TestConfigResponse","UninstallConnectorRequest","UninstallConnectorResponse","UpdateClientRequest","UpdateClientResponse","UpdateMappingRequest","UpdateMappingResponse","UpdateMetadataRequest","UpdateMetadataResponse","UpdateScopeRequest","UpdateScopeResponse","UpdateWalletRequest","UpdateWalletRequestBody","UpdateWalletResponse","VoidHoldRequest","VoidHoldResponse","WalletsgetServerInfoResponse"]
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/activateconfig.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/deactivateconfig.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,25 @@
 import dataclasses
 import requests as requests_http
 from ..shared import configresponse as shared_configresponse
 from ..shared import webhookserrorresponse as shared_webhookserrorresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
-class ActivateConfigRequest:
+class DeactivateConfigRequest:
+    
     id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'id', 'style': 'simple', 'explode': False }})
     r"""Config ID"""
     
 
-
-
-
 @dataclasses.dataclass
-class ActivateConfigResponse:
+class DeactivateConfigResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     config_response: Optional[shared_configresponse.ConfigResponse] = dataclasses.field(default=None)
-    r"""Config successfully activated."""
+    r"""Config successfully deactivated."""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     webhooks_error_response: Optional[shared_webhookserrorresponse.WebhooksErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/addmetadataontransaction.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/addmetadataontransaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,30 +3,27 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import errorresponse as shared_errorresponse
 from typing import Any, Optional
 
 
-
 @dataclasses.dataclass
 class AddMetadataOnTransactionRequest:
+    
     ledger: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ledger', 'style': 'simple', 'explode': False }})
     r"""Name of the ledger."""
     txid: int = dataclasses.field(metadata={'path_param': { 'field_name': 'txid', 'style': 'simple', 'explode': False }})
     r"""Transaction ID."""
     request_body: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     r"""metadata"""
     
 
-
-
-
 @dataclasses.dataclass
 class AddMetadataOnTransactionResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     error_response: Optional[shared_errorresponse.ErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/addmetadatatoaccount.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/addmetadatatoaccount.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,34 +3,31 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import errorresponse as shared_errorresponse
 from typing import Any, Optional
 
 
-
 @dataclasses.dataclass
 class AddMetadataToAccountRequest:
+    
     address: str = dataclasses.field(metadata={'path_param': { 'field_name': 'address', 'style': 'simple', 'explode': False }})
     r"""Exact address of the account. It must match the following regular expressions pattern:
     ```
     ^\w+(:\w+)*$
     ```
     """
     ledger: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ledger', 'style': 'simple', 'explode': False }})
     r"""Name of the ledger."""
     request_body: dict[str, Any] = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
     r"""metadata"""
     
 
-
-
-
 @dataclasses.dataclass
 class AddMetadataToAccountResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     error_response: Optional[shared_errorresponse.ErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/addscopetoclient.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/deleteclient.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,26 +2,21 @@
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from typing import Optional
 
 
-
 @dataclasses.dataclass
-class AddScopeToClientRequest:
+class DeleteClientRequest:
+    
     client_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'clientId', 'style': 'simple', 'explode': False }})
     r"""Client ID"""
-    scope_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'scopeId', 'style': 'simple', 'explode': False }})
-    r"""Scope ID"""
     
 
-
-
-
 @dataclasses.dataclass
-class AddScopeToClientResponse:
+class DeleteClientResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/addtransientscope.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/addtransientscope.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,26 +2,23 @@
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class AddTransientScopeRequest:
+    
     scope_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'scopeId', 'style': 'simple', 'explode': False }})
     r"""Scope ID"""
     transient_scope_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'transientScopeId', 'style': 'simple', 'explode': False }})
     r"""Transient scope ID"""
     
 
-
-
-
 @dataclasses.dataclass
 class AddTransientScopeResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/cancelevent.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/cancelevent.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,23 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import error as shared_error
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class CancelEventRequest:
+    
     instance_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'instanceID', 'style': 'simple', 'explode': False }})
     r"""The instance id"""
     
 
-
-
-
 @dataclasses.dataclass
 class CancelEventResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     error: Optional[shared_error.Error] = dataclasses.field(default=None)
     r"""General error"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/changeconfigsecret.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/changeconfigsecret.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,29 +5,26 @@
 import requests as requests_http
 from ..shared import configchangesecret as shared_configchangesecret
 from ..shared import configresponse as shared_configresponse
 from ..shared import webhookserrorresponse as shared_webhookserrorresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class ChangeConfigSecretRequest:
+    
     id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'id', 'style': 'simple', 'explode': False }})
     r"""Config ID"""
     config_change_secret: Optional[shared_configchangesecret.ConfigChangeSecret] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
-
-
-
 @dataclasses.dataclass
 class ChangeConfigSecretResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     config_response: Optional[shared_configresponse.ConfigResponse] = dataclasses.field(default=None)
     r"""Secret successfully changed."""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     webhooks_error_response: Optional[shared_webhookserrorresponse.WebhooksErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/confirmhold.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/confirmhold.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,26 +4,23 @@
 import dataclasses
 import requests as requests_http
 from ..shared import confirmholdrequest as shared_confirmholdrequest
 from ..shared import walletserrorresponse as shared_walletserrorresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class ConfirmHoldRequest:
+    
     hold_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'hold_id', 'style': 'simple', 'explode': False }})
     confirm_hold_request: Optional[shared_confirmholdrequest.ConfirmHoldRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
-
-
-
 @dataclasses.dataclass
 class ConfirmHoldResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     wallets_error_response: Optional[shared_walletserrorresponse.WalletsErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/connectorsstripetransfer.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/createworkflow.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import stripetransferresponse as shared_stripetransferresponse
+from ..shared import createworkflowresponse as shared_createworkflowresponse
+from ..shared import error as shared_error
 from typing import Optional
 
 
-
 @dataclasses.dataclass
-class ConnectorsStripeTransferResponse:
+class CreateWorkflowResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    create_workflow_response: Optional[shared_createworkflowresponse.CreateWorkflowResponse] = dataclasses.field(default=None)
+    r"""Created workflow"""
+    error: Optional[shared_error.Error] = dataclasses.field(default=None)
+    r"""General error"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    stripe_transfer_response: Optional[shared_stripetransferresponse.StripeTransferResponse] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/connectorstransfer.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/connectorstransfer.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,27 +5,24 @@
 import requests as requests_http
 from ..shared import connector as shared_connector
 from ..shared import transferrequest as shared_transferrequest
 from ..shared import transferresponse as shared_transferresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class ConnectorsTransferRequest:
+    
     connector: shared_connector.Connector = dataclasses.field(metadata={'path_param': { 'field_name': 'connector', 'style': 'simple', 'explode': False }})
     r"""The name of the connector."""
     transfer_request: shared_transferrequest.TransferRequest = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
     
 
-
-
-
 @dataclasses.dataclass
 class ConnectorsTransferResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     transfer_response: Optional[shared_transferresponse.TransferResponse] = dataclasses.field(default=None)
     r"""OK"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/countaccounts.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/countaccounts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,30 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import errorresponse as shared_errorresponse
-from typing import Optional
-
-
-
-@dataclasses.dataclass
-class CountAccountsMetadata:
-    r"""Filter accounts by metadata key value pairs. The filter can be used like this metadata[key]=value1&metadata[a.nested.key]=value2"""
-    
-
-
+from typing import Any, Optional
 
 
 @dataclasses.dataclass
 class CountAccountsRequest:
+    
     ledger: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ledger', 'style': 'simple', 'explode': False }})
     r"""Name of the ledger."""
     address: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'address', 'style': 'form', 'explode': True }})
     r"""Filter accounts by address pattern (regular expression placed between ^ and $)."""
-    metadata: Optional[CountAccountsMetadata] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'metadata', 'style': 'deepObject', 'explode': True }})
+    metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'metadata', 'style': 'deepObject', 'explode': True }})
     r"""Filter accounts by metadata key value pairs. The filter can be used like this metadata[key]=value1&metadata[a.nested.key]=value2"""
     
 
-
-
-
 @dataclasses.dataclass
 class CountAccountsResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     error_response: Optional[shared_errorresponse.ErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
     headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/counttransactions.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/counttransactions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,45 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import errorresponse as shared_errorresponse
 from datetime import datetime
-from typing import Optional
-
-
-
-@dataclasses.dataclass
-class CountTransactionsMetadata:
-    r"""Filter transactions by metadata key value pairs. Nested objects can be used as seen in the example below."""
-    
-
-
+from typing import Any, Optional
 
 
 @dataclasses.dataclass
 class CountTransactionsRequest:
+    
     ledger: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ledger', 'style': 'simple', 'explode': False }})
     r"""Name of the ledger."""
     account: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'account', 'style': 'form', 'explode': True }})
     r"""Filter transactions with postings involving given account, either as source or destination (regular expression placed between ^ and $)."""
     destination: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'destination', 'style': 'form', 'explode': True }})
     r"""Filter transactions with postings involving given account at destination (regular expression placed between ^ and $)."""
     end_time: Optional[datetime] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'endTime', 'style': 'form', 'explode': True }})
     r"""Filter transactions that occurred before this timestamp.
     The format is RFC3339 and is exclusive (for example, \"2023-01-02T15:04:01Z\" excludes the first second of 4th minute).
     """
-    metadata: Optional[CountTransactionsMetadata] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'metadata', 'style': 'deepObject', 'explode': True }})
+    metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'metadata', 'style': 'deepObject', 'explode': True }})
     r"""Filter transactions by metadata key value pairs. Nested objects can be used as seen in the example below."""
     reference: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'reference', 'style': 'form', 'explode': True }})
     r"""Filter transactions by reference field."""
     source: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'source', 'style': 'form', 'explode': True }})
     r"""Filter transactions with postings involving given account at source (regular expression placed between ^ and $)."""
     start_time: Optional[datetime] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'startTime', 'style': 'form', 'explode': True }})
     r"""Filter transactions that occurred after this timestamp.
     The format is RFC3339 and is inclusive (for example, \"2023-01-02T15:04:01Z\" includes the first second of 4th minute).
     """
     
 
-
-
-
 @dataclasses.dataclass
 class CountTransactionsResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     error_response: Optional[shared_errorresponse.ErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
     headers: Optional[dict[str, list[str]]] = dataclasses.field(default=None)
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/createbalance.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/createbalance.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,28 +5,25 @@
 import requests as requests_http
 from ..shared import createbalancerequest as shared_createbalancerequest
 from ..shared import createbalanceresponse as shared_createbalanceresponse
 from ..shared import walletserrorresponse as shared_walletserrorresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class CreateBalanceRequest:
+    
     id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'id', 'style': 'simple', 'explode': False }})
     create_balance_request: Optional[shared_createbalancerequest.CreateBalanceRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
-
-
-
 @dataclasses.dataclass
 class CreateBalanceResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     create_balance_response: Optional[shared_createbalanceresponse.CreateBalanceResponse] = dataclasses.field(default=None)
     r"""Created balance"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     wallets_error_response: Optional[shared_walletserrorresponse.WalletsErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/createclient.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/createclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import createclientresponse as shared_createclientresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class CreateClientResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     create_client_response: Optional[shared_createclientresponse.CreateClientResponse] = dataclasses.field(default=None)
     r"""Client created"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/createscope.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/createscope.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import createscoperesponse as shared_createscoperesponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class CreateScopeResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     create_scope_response: Optional[shared_createscoperesponse.CreateScopeResponse] = dataclasses.field(default=None)
     r"""Created scope"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/createsecret.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/updateclient.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import createsecretrequest as shared_createsecretrequest
-from ..shared import createsecretresponse as shared_createsecretresponse
+from ..shared import updateclientrequest as shared_updateclientrequest
+from ..shared import updateclientresponse as shared_updateclientresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
-class CreateSecretRequest:
+class UpdateClientRequest:
+    
     client_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'clientId', 'style': 'simple', 'explode': False }})
     r"""Client ID"""
-    create_secret_request: Optional[shared_createsecretrequest.CreateSecretRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    update_client_request: Optional[shared_updateclientrequest.UpdateClientRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
-
-
-
 @dataclasses.dataclass
-class CreateSecretResponse:
+class UpdateClientResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    create_secret_response: Optional[shared_createsecretresponse.CreateSecretResponse] = dataclasses.field(default=None)
-    r"""Created secret"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+    update_client_response: Optional[shared_updateclientresponse.UpdateClientResponse] = dataclasses.field(default=None)
+    r"""Updated client"""
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/createtransaction.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/createtransaction.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,35 +5,32 @@
 import requests as requests_http
 from ..shared import errorresponse as shared_errorresponse
 from ..shared import posttransaction as shared_posttransaction
 from ..shared import transactionsresponse as shared_transactionsresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class CreateTransactionRequest:
+    
     ledger: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ledger', 'style': 'simple', 'explode': False }})
     r"""Name of the ledger."""
     post_transaction: shared_posttransaction.PostTransaction = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
     r"""The request body must contain at least one of the following objects:
       - `postings`: suitable for simple transactions
       - `script`: enabling more complex transactions with Numscript
     """
     preview: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'preview', 'style': 'form', 'explode': True }})
     r"""Set the preview mode. Preview mode doesn't add the logs to the database or publish a message to the message broker."""
     
 
-
-
-
 @dataclasses.dataclass
 class CreateTransactionResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     error_response: Optional[shared_errorresponse.ErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     transactions_response: Optional[shared_transactionsresponse.TransactionsResponse] = dataclasses.field(default=None)
     r"""OK"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/createtransactions.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/createtransactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,29 +5,26 @@
 import requests as requests_http
 from ..shared import errorresponse as shared_errorresponse
 from ..shared import transactions as shared_transactions
 from ..shared import transactionsresponse as shared_transactionsresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class CreateTransactionsRequest:
+    
     ledger: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ledger', 'style': 'simple', 'explode': False }})
     r"""Name of the ledger."""
     transactions: shared_transactions.Transactions = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
     
 
-
-
-
 @dataclasses.dataclass
 class CreateTransactionsResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     error_response: Optional[shared_errorresponse.ErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     transactions_response: Optional[shared_transactionsresponse.TransactionsResponse] = dataclasses.field(default=None)
     r"""OK"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/createwallet.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/createwallet.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 import dataclasses
 import requests as requests_http
 from ..shared import createwalletresponse as shared_createwalletresponse
 from ..shared import walletserrorresponse as shared_walletserrorresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class CreateWalletResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     create_wallet_response: Optional[shared_createwalletresponse.CreateWalletResponse] = dataclasses.field(default=None)
     r"""Wallet created"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     wallets_error_response: Optional[shared_walletserrorresponse.WalletsErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/createworkflow.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/readconnectorconfig.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import createworkflowresponse as shared_createworkflowresponse
-from ..shared import error as shared_error
+from ..shared import connector as shared_connector
+from ..shared import connectorconfigresponse as shared_connectorconfigresponse
 from typing import Optional
 
 
+@dataclasses.dataclass
+class ReadConnectorConfigRequest:
+    
+    connector: shared_connector.Connector = dataclasses.field(metadata={'path_param': { 'field_name': 'connector', 'style': 'simple', 'explode': False }})
+    r"""The name of the connector."""
+    
 
 @dataclasses.dataclass
-class CreateWorkflowResponse:
+class ReadConnectorConfigResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    create_workflow_response: Optional[shared_createworkflowresponse.CreateWorkflowResponse] = dataclasses.field(default=None)
-    r"""Created workflow"""
-    error: Optional[shared_error.Error] = dataclasses.field(default=None)
-    r"""General error"""
+    connector_config_response: Optional[shared_connectorconfigresponse.ConnectorConfigResponse] = dataclasses.field(default=None)
+    r"""OK"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/creditwallet.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/creditwallet.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,23 @@
 import dataclasses
 import requests as requests_http
 from ..shared import creditwalletrequest as shared_creditwalletrequest
 from ..shared import walletserrorresponse as shared_walletserrorresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class CreditWalletRequest:
+    
     id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'id', 'style': 'simple', 'explode': False }})
     credit_wallet_request: Optional[shared_creditwalletrequest.CreditWalletRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
-
-
-
 @dataclasses.dataclass
 class CreditWalletResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     wallets_error_response: Optional[shared_walletserrorresponse.WalletsErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/deactivateconfig.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/deleteconfig.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import configresponse as shared_configresponse
 from ..shared import webhookserrorresponse as shared_webhookserrorresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
-class DeactivateConfigRequest:
+class DeleteConfigRequest:
+    
     id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'id', 'style': 'simple', 'explode': False }})
     r"""Config ID"""
     
 
-
-
-
 @dataclasses.dataclass
-class DeactivateConfigResponse:
+class DeleteConfigResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    config_response: Optional[shared_configresponse.ConfigResponse] = dataclasses.field(default=None)
-    r"""Config successfully deactivated."""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     webhooks_error_response: Optional[shared_webhookserrorresponse.WebhooksErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/debitwallet.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/debitwallet.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,25 @@
 import requests as requests_http
 from ..shared import debitwalletrequest as shared_debitwalletrequest
 from ..shared import debitwalletresponse as shared_debitwalletresponse
 from ..shared import walletserrorresponse as shared_walletserrorresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class DebitWalletRequest:
+    
     id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'id', 'style': 'simple', 'explode': False }})
     debit_wallet_request: Optional[shared_debitwalletrequest.DebitWalletRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
-
-
-
 @dataclasses.dataclass
 class DebitWalletResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     debit_wallet_response: Optional[shared_debitwalletresponse.DebitWalletResponse] = dataclasses.field(default=None)
     r"""Wallet successfully debited as a pending hold"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     wallets_error_response: Optional[shared_walletserrorresponse.WalletsErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/deleteclient.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/connectorsstripetransfer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from typing import Optional
-
+from typing import Any, Optional
 
 
 @dataclasses.dataclass
-class DeleteClientRequest:
-    client_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'clientId', 'style': 'simple', 'explode': False }})
-    r"""Client ID"""
+class ConnectorsStripeTransferResponse:
     
-
-
-
-
-@dataclasses.dataclass
-class DeleteClientResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+    stripe_transfer_response: Optional[dict[str, Any]] = dataclasses.field(default=None)
+    r"""OK"""
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/deleteconfig.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/activateconfig.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ..shared import configresponse as shared_configresponse
 from ..shared import webhookserrorresponse as shared_webhookserrorresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
-class DeleteConfigRequest:
+class ActivateConfigRequest:
+    
     id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'id', 'style': 'simple', 'explode': False }})
     r"""Config ID"""
     
 
-
-
-
 @dataclasses.dataclass
-class DeleteConfigResponse:
+class ActivateConfigResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    config_response: Optional[shared_configresponse.ConfigResponse] = dataclasses.field(default=None)
+    r"""Config successfully activated."""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     webhooks_error_response: Optional[shared_webhookserrorresponse.WebhooksErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/deletescope.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/deletescopefromclient.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from typing import Optional
 
 
-
 @dataclasses.dataclass
-class DeleteScopeRequest:
+class DeleteScopeFromClientRequest:
+    
+    client_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'clientId', 'style': 'simple', 'explode': False }})
+    r"""Client ID"""
     scope_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'scopeId', 'style': 'simple', 'explode': False }})
     r"""Scope ID"""
     
 
-
-
-
 @dataclasses.dataclass
-class DeleteScopeResponse:
+class DeleteScopeFromClientResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/deletescopefromclient.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/voidhold.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ..shared import walletserrorresponse as shared_walletserrorresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
-class DeleteScopeFromClientRequest:
-    client_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'clientId', 'style': 'simple', 'explode': False }})
-    r"""Client ID"""
-    scope_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'scopeId', 'style': 'simple', 'explode': False }})
-    r"""Scope ID"""
+class VoidHoldRequest:
+    
+    hold_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'hold_id', 'style': 'simple', 'explode': False }})
     
-
-
-
 
 @dataclasses.dataclass
-class DeleteScopeFromClientResponse:
+class VoidHoldResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+    wallets_error_response: Optional[shared_walletserrorresponse.WalletsErrorResponse] = dataclasses.field(default=None)
+    r"""Error"""
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/deletesecret.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getpayment.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ..shared import paymentresponse as shared_paymentresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
-class DeleteSecretRequest:
-    client_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'clientId', 'style': 'simple', 'explode': False }})
-    r"""Client ID"""
-    secret_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'secretId', 'style': 'simple', 'explode': False }})
-    r"""Secret ID"""
+class GetPaymentRequest:
+    
+    payment_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'paymentId', 'style': 'simple', 'explode': False }})
+    r"""The payment ID."""
     
-
-
-
 
 @dataclasses.dataclass
-class DeleteSecretResponse:
+class GetPaymentResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    payment_response: Optional[shared_paymentresponse.PaymentResponse] = dataclasses.field(default=None)
+    r"""OK"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/deletetransientscope.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/deletetransientscope.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,26 +2,23 @@
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class DeleteTransientScopeRequest:
+    
     scope_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'scopeId', 'style': 'simple', 'explode': False }})
     r"""Scope ID"""
     transient_scope_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'transientScopeId', 'style': 'simple', 'explode': False }})
     r"""Transient scope ID"""
     
 
-
-
-
 @dataclasses.dataclass
 class DeleteTransientScopeResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/flowsgetserverinfo.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/flowsgetserverinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 import dataclasses
 import requests as requests_http
 from ..shared import error as shared_error
 from ..shared import serverinfo as shared_serverinfo
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class FlowsgetServerInfoResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     error: Optional[shared_error.Error] = dataclasses.field(default=None)
     r"""General error"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     server_info: Optional[shared_serverinfo.ServerInfo] = dataclasses.field(default=None)
     r"""Server information"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/getaccount.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getaccount.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,34 +4,31 @@
 import dataclasses
 import requests as requests_http
 from ..shared import accountresponse as shared_accountresponse
 from ..shared import errorresponse as shared_errorresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class GetAccountRequest:
+    
     address: str = dataclasses.field(metadata={'path_param': { 'field_name': 'address', 'style': 'simple', 'explode': False }})
     r"""Exact address of the account. It must match the following regular expressions pattern:
     ```
     ^\w+(:\w+)*$
     ```
     """
     ledger: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ledger', 'style': 'simple', 'explode': False }})
     r"""Name of the ledger."""
     
 
-
-
-
 @dataclasses.dataclass
 class GetAccountResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     account_response: Optional[shared_accountresponse.AccountResponse] = dataclasses.field(default=None)
     r"""OK"""
     error_response: Optional[shared_errorresponse.ErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/getbalance.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getbalance.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,28 +4,25 @@
 import dataclasses
 import requests as requests_http
 from ..shared import getbalanceresponse as shared_getbalanceresponse
 from ..shared import walletserrorresponse as shared_walletserrorresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class GetBalanceRequest:
+    
     balance_name: str = dataclasses.field(metadata={'path_param': { 'field_name': 'balanceName', 'style': 'simple', 'explode': False }})
     id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'id', 'style': 'simple', 'explode': False }})
     
 
-
-
-
 @dataclasses.dataclass
 class GetBalanceResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     get_balance_response: Optional[shared_getbalanceresponse.GetBalanceResponse] = dataclasses.field(default=None)
     r"""Balance summary"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     wallets_error_response: Optional[shared_walletserrorresponse.WalletsErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/getbalances.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getbalances.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import dataclasses
 import requests as requests_http
 from ..shared import balancescursorresponse as shared_balancescursorresponse
 from ..shared import errorresponse as shared_errorresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class GetBalancesRequest:
+    
     ledger: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ledger', 'style': 'simple', 'explode': False }})
     r"""Name of the ledger."""
     address: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'address', 'style': 'form', 'explode': True }})
     r"""Filter balances involving given account, either as source or destination."""
     after: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'after', 'style': 'form', 'explode': True }})
     r"""Pagination cursor, will return accounts after given address, in descending order."""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
@@ -24,26 +24,23 @@
     No other parameters can be set when this parameter is set.
     """
     pagination_token: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'pagination_token', 'style': 'form', 'explode': True }})
     r"""Parameter used in pagination requests.
     Set to the value of next for the next page of results.
     Set to the value of previous for the previous page of results.
     Deprecated, please use `cursor` instead.
-
+    
     Deprecated: this field will be removed in a future release, please migrate away from it as soon as possible
     """
     
 
-
-
-
 @dataclasses.dataclass
 class GetBalancesResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     balances_cursor_response: Optional[shared_balancescursorresponse.BalancesCursorResponse] = dataclasses.field(default=None)
     r"""OK"""
     error_response: Optional[shared_errorresponse.ErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/getbalancesaggregated.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getbalancesaggregated.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,30 +4,27 @@
 import dataclasses
 import requests as requests_http
 from ..shared import aggregatebalancesresponse as shared_aggregatebalancesresponse
 from ..shared import errorresponse as shared_errorresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class GetBalancesAggregatedRequest:
+    
     ledger: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ledger', 'style': 'simple', 'explode': False }})
     r"""Name of the ledger."""
     address: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'address', 'style': 'form', 'explode': True }})
     r"""Filter balances involving given account, either as source or destination."""
     
 
-
-
-
 @dataclasses.dataclass
 class GetBalancesAggregatedResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     aggregate_balances_response: Optional[shared_aggregatebalancesresponse.AggregateBalancesResponse] = dataclasses.field(default=None)
     r"""OK"""
     error_response: Optional[shared_errorresponse.ErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/getconnectortask.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getconnectortask.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,28 +4,25 @@
 import dataclasses
 import requests as requests_http
 from ..shared import connector as shared_connector
 from ..shared import taskresponse as shared_taskresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class GetConnectorTaskRequest:
+    
     connector: shared_connector.Connector = dataclasses.field(metadata={'path_param': { 'field_name': 'connector', 'style': 'simple', 'explode': False }})
     r"""The name of the connector."""
     task_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'taskId', 'style': 'simple', 'explode': False }})
     r"""The task ID."""
     
 
-
-
-
 @dataclasses.dataclass
 class GetConnectorTaskResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     task_response: Optional[shared_taskresponse.TaskResponse] = dataclasses.field(default=None)
     r"""OK"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/gethold.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/gethold.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,25 @@
 import dataclasses
 import requests as requests_http
 from ..shared import getholdresponse as shared_getholdresponse
 from ..shared import walletserrorresponse as shared_walletserrorresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class GetHoldRequest:
+    
     hold_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'holdID', 'style': 'simple', 'explode': False }})
     r"""The hold ID"""
     
 
-
-
-
 @dataclasses.dataclass
 class GetHoldResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     get_hold_response: Optional[shared_getholdresponse.GetHoldResponse] = dataclasses.field(default=None)
     r"""Holds"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     wallets_error_response: Optional[shared_walletserrorresponse.WalletsErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/getholds.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getholds.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,38 +4,35 @@
 import dataclasses
 import requests as requests_http
 from ..shared import getholdsresponse as shared_getholdsresponse
 from ..shared import walletserrorresponse as shared_walletserrorresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class GetHoldsRequest:
+    
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     r"""Parameter used in pagination requests.
     Set to the value of next for the next page of results.
     Set to the value of previous for the previous page of results.
     No other parameters can be set when the pagination token is set.
     """
     metadata: Optional[dict[str, str]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'metadata', 'style': 'deepObject', 'explode': True }})
     r"""Filter holds by metadata key value pairs. Nested objects can be used as seen in the example below."""
     page_size: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'pageSize', 'style': 'form', 'explode': True }})
     r"""The maximum number of results to return per page"""
     wallet_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'walletID', 'style': 'form', 'explode': True }})
     r"""The wallet to filter on"""
     
 
-
-
-
 @dataclasses.dataclass
 class GetHoldsResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     get_holds_response: Optional[shared_getholdsresponse.GetHoldsResponse] = dataclasses.field(default=None)
     r"""Holds"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     wallets_error_response: Optional[shared_walletserrorresponse.WalletsErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/getinfo.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getinfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 import dataclasses
 import requests as requests_http
 from ..shared import configinforesponse as shared_configinforesponse
 from ..shared import errorresponse as shared_errorresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class GetInfoResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     config_info_response: Optional[shared_configinforesponse.ConfigInfoResponse] = dataclasses.field(default=None)
     r"""OK"""
     error_response: Optional[shared_errorresponse.ErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/getinstance.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getinstance.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,28 +4,25 @@
 import dataclasses
 import requests as requests_http
 from ..shared import error as shared_error
 from ..shared import getworkflowinstanceresponse as shared_getworkflowinstanceresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class GetInstanceRequest:
+    
     instance_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'instanceID', 'style': 'simple', 'explode': False }})
     r"""The instance id"""
     
 
-
-
-
 @dataclasses.dataclass
 class GetInstanceResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     error: Optional[shared_error.Error] = dataclasses.field(default=None)
     r"""General error"""
     get_workflow_instance_response: Optional[shared_getworkflowinstanceresponse.GetWorkflowInstanceResponse] = dataclasses.field(default=None)
     r"""The workflow instance"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/getinstancehistory.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getinstancehistory.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,28 +4,25 @@
 import dataclasses
 import requests as requests_http
 from ..shared import error as shared_error
 from ..shared import getworkflowinstancehistoryresponse as shared_getworkflowinstancehistoryresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class GetInstanceHistoryRequest:
+    
     instance_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'instanceID', 'style': 'simple', 'explode': False }})
     r"""The instance id"""
     
 
-
-
-
 @dataclasses.dataclass
 class GetInstanceHistoryResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     error: Optional[shared_error.Error] = dataclasses.field(default=None)
     r"""General error"""
     get_workflow_instance_history_response: Optional[shared_getworkflowinstancehistoryresponse.GetWorkflowInstanceHistoryResponse] = dataclasses.field(default=None)
     r"""The workflow instance history"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/getinstancestagehistory.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getinstancestagehistory.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,30 +4,27 @@
 import dataclasses
 import requests as requests_http
 from ..shared import error as shared_error
 from ..shared import getworkflowinstancehistorystageresponse as shared_getworkflowinstancehistorystageresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class GetInstanceStageHistoryRequest:
+    
     instance_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'instanceID', 'style': 'simple', 'explode': False }})
     r"""The instance id"""
     number: int = dataclasses.field(metadata={'path_param': { 'field_name': 'number', 'style': 'simple', 'explode': False }})
     r"""The stage number"""
     
 
-
-
-
 @dataclasses.dataclass
 class GetInstanceStageHistoryResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     error: Optional[shared_error.Error] = dataclasses.field(default=None)
     r"""General error"""
     get_workflow_instance_history_stage_response: Optional[shared_getworkflowinstancehistorystageresponse.GetWorkflowInstanceHistoryStageResponse] = dataclasses.field(default=None)
     r"""The workflow instance stage history"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/getledgerinfo.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getledgerinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,28 +4,25 @@
 import dataclasses
 import requests as requests_http
 from ..shared import errorresponse as shared_errorresponse
 from ..shared import ledgerinforesponse as shared_ledgerinforesponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class GetLedgerInfoRequest:
+    
     ledger: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ledger', 'style': 'simple', 'explode': False }})
     r"""Name of the ledger."""
     
 
-
-
-
 @dataclasses.dataclass
 class GetLedgerInfoResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     error_response: Optional[shared_errorresponse.ErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
     ledger_info_response: Optional[shared_ledgerinforesponse.LedgerInfoResponse] = dataclasses.field(default=None)
     r"""OK"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/getmanyconfigs.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/updatemapping.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import configsresponse as shared_configsresponse
-from ..shared import webhookserrorresponse as shared_webhookserrorresponse
+from ..shared import errorresponse as shared_errorresponse
+from ..shared import mapping as shared_mapping
+from ..shared import mappingresponse as shared_mappingresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
-class GetManyConfigsRequest:
-    endpoint: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'endpoint', 'style': 'form', 'explode': True }})
-    r"""Optional filter by endpoint URL"""
-    id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
-    r"""Optional filter by Config ID"""
+class UpdateMappingRequest:
+    
+    ledger: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ledger', 'style': 'simple', 'explode': False }})
+    r"""Name of the ledger."""
+    mapping: shared_mapping.Mapping = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
     
-
-
-
 
 @dataclasses.dataclass
-class GetManyConfigsResponse:
+class UpdateMappingResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    configs_response: Optional[shared_configsresponse.ConfigsResponse] = dataclasses.field(default=None)
+    error_response: Optional[shared_errorresponse.ErrorResponse] = dataclasses.field(default=None)
+    r"""Error"""
+    mapping_response: Optional[shared_mappingresponse.MappingResponse] = dataclasses.field(default=None)
     r"""OK"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    webhooks_error_response: Optional[shared_webhookserrorresponse.WebhooksErrorResponse] = dataclasses.field(default=None)
-    r"""Error"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/getmapping.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getmapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,25 @@
 import dataclasses
 import requests as requests_http
 from ..shared import errorresponse as shared_errorresponse
 from ..shared import mappingresponse as shared_mappingresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class GetMappingRequest:
+    
     ledger: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ledger', 'style': 'simple', 'explode': False }})
     r"""Name of the ledger."""
     
 
-
-
-
 @dataclasses.dataclass
 class GetMappingResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     error_response: Optional[shared_errorresponse.ErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
     mapping_response: Optional[shared_mappingresponse.MappingResponse] = dataclasses.field(default=None)
     r"""OK"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/getpayment.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/readstats.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import paymentresponse as shared_paymentresponse
+from ..shared import errorresponse as shared_errorresponse
+from ..shared import statsresponse as shared_statsresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
-class GetPaymentRequest:
-    payment_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'paymentId', 'style': 'simple', 'explode': False }})
-    r"""The payment ID."""
+class ReadStatsRequest:
+    
+    ledger: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ledger', 'style': 'simple', 'explode': False }})
+    r"""name of the ledger"""
     
-
-
-
 
 @dataclasses.dataclass
-class GetPaymentResponse:
+class ReadStatsResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    payment_response: Optional[shared_paymentresponse.PaymentResponse] = dataclasses.field(default=None)
-    r"""OK"""
+    error_response: Optional[shared_errorresponse.ErrorResponse] = dataclasses.field(default=None)
+    r"""Error"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+    stats_response: Optional[shared_statsresponse.StatsResponse] = dataclasses.field(default=None)
+    r"""OK"""
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/getserverinfo.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getserverinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import serverinfo as shared_serverinfo
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class GetServerInfoResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     server_info: Optional[shared_serverinfo.ServerInfo] = dataclasses.field(default=None)
     r"""Server information"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/gettransaction.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/gettransaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,30 +4,27 @@
 import dataclasses
 import requests as requests_http
 from ..shared import errorresponse as shared_errorresponse
 from ..shared import transactionresponse as shared_transactionresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class GetTransactionRequest:
+    
     ledger: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ledger', 'style': 'simple', 'explode': False }})
     r"""Name of the ledger."""
     txid: int = dataclasses.field(metadata={'path_param': { 'field_name': 'txid', 'style': 'simple', 'explode': False }})
     r"""Transaction ID."""
     
 
-
-
-
 @dataclasses.dataclass
 class GetTransactionResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     error_response: Optional[shared_errorresponse.ErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     transaction_response: Optional[shared_transactionresponse.TransactionResponse] = dataclasses.field(default=None)
     r"""OK"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/gettransactions.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/gettransactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,36 +4,33 @@
 import dataclasses
 import requests as requests_http
 from ..shared import gettransactionsresponse as shared_gettransactionsresponse
 from ..shared import walletserrorresponse as shared_walletserrorresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class GetTransactionsRequest:
+    
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     r"""Parameter used in pagination requests.
     Set to the value of next for the next page of results.
     Set to the value of previous for the previous page of results.
     No other parameters can be set when the cursor is set.
     """
     page_size: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'pageSize', 'style': 'form', 'explode': True }})
     r"""The maximum number of results to return per page"""
     wallet_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'walletID', 'style': 'form', 'explode': True }})
     r"""A wallet ID to filter on"""
     
 
-
-
-
 @dataclasses.dataclass
 class GetTransactionsResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     get_transactions_response: Optional[shared_gettransactionsresponse.GetTransactionsResponse] = dataclasses.field(default=None)
     r"""OK"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     wallets_error_response: Optional[shared_walletserrorresponse.WalletsErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/getversions.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getversions.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import getversionsresponse as shared_getversionsresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class GetVersionsResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     get_versions_response: Optional[shared_getversionsresponse.GetVersionsResponse] = dataclasses.field(default=None)
     r"""OK"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/getwallet.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getwalletsummary.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import getwalletresponse as shared_getwalletresponse
+from ..shared import getwalletsummaryresponse as shared_getwalletsummaryresponse
 from ..shared import walletserrorresponse as shared_walletserrorresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
-class GetWalletRequest:
+class GetWalletSummaryRequest:
+    
     id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'id', 'style': 'simple', 'explode': False }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetWalletResponse:
+class GetWalletSummaryResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    get_wallet_response: Optional[shared_getwalletresponse.GetWalletResponse] = dataclasses.field(default=None)
-    r"""Wallet"""
+    get_wallet_summary_response: Optional[shared_getwalletsummaryresponse.GetWalletSummaryResponse] = dataclasses.field(default=None)
+    r"""Wallet summary"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     wallets_error_response: Optional[shared_walletserrorresponse.WalletsErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/getwalletsummary.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getwallet.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import getwalletsummaryresponse as shared_getwalletsummaryresponse
+from ..shared import getwalletresponse as shared_getwalletresponse
 from ..shared import walletserrorresponse as shared_walletserrorresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
-class GetWalletSummaryRequest:
+class GetWalletRequest:
+    
     id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'id', 'style': 'simple', 'explode': False }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetWalletSummaryResponse:
+class GetWalletResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    get_wallet_summary_response: Optional[shared_getwalletsummaryresponse.GetWalletSummaryResponse] = dataclasses.field(default=None)
-    r"""Wallet summary"""
+    get_wallet_response: Optional[shared_getwalletresponse.GetWalletResponse] = dataclasses.field(default=None)
+    r"""Wallet"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     wallets_error_response: Optional[shared_walletserrorresponse.WalletsErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/getworkflow.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getworkflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,25 @@
 import dataclasses
 import requests as requests_http
 from ..shared import error as shared_error
 from ..shared import getworkflowresponse as shared_getworkflowresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class GetWorkflowRequest:
+    
     flow_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'flowId', 'style': 'simple', 'explode': False }})
     r"""The flow id"""
     
 
-
-
-
 @dataclasses.dataclass
 class GetWorkflowResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     error: Optional[shared_error.Error] = dataclasses.field(default=None)
     r"""General error"""
     get_workflow_response: Optional[shared_getworkflowresponse.GetWorkflowResponse] = dataclasses.field(default=None)
     r"""The workflow"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/insertconfig.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/insertconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 import dataclasses
 import requests as requests_http
 from ..shared import configresponse as shared_configresponse
 from ..shared import webhookserrorresponse as shared_webhookserrorresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class InsertConfigResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     config_response: Optional[shared_configresponse.ConfigResponse] = dataclasses.field(default=None)
     r"""Config created successfully."""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     webhooks_error_response: Optional[shared_webhookserrorresponse.WebhooksErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/installconnector.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/installconnector.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,25 +3,22 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import connector as shared_connector
 from typing import Any, Optional
 
 
-
 @dataclasses.dataclass
 class InstallConnectorRequest:
+    
     connector: shared_connector.Connector = dataclasses.field(metadata={'path_param': { 'field_name': 'connector', 'style': 'simple', 'explode': False }})
     r"""The name of the connector."""
     request_body: Any = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
     
 
-
-
-
 @dataclasses.dataclass
 class InstallConnectorResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/listaccounts.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listaccounts.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,37 +2,29 @@
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import accountscursorresponse as shared_accountscursorresponse
 from ..shared import errorresponse as shared_errorresponse
 from enum import Enum
-from typing import Optional
+from typing import Any, Optional
 
 class ListAccountsBalanceOperator(str, Enum):
     r"""Operator used for the filtering of balances can be greater than/equal, less than/equal, greater than, less than, equal or not."""
     GTE = 'gte'
     LTE = 'lte'
     GT = 'gt'
     LT = 'lt'
     E = 'e'
     NE = 'ne'
 
 
-
-@dataclasses.dataclass
-class ListAccountsMetadata:
-    r"""Filter accounts by metadata key value pairs. Nested objects can be used as seen in the example below."""
-    
-
-
-
-
 @dataclasses.dataclass
 class ListAccountsRequest:
+    
     ledger: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ledger', 'style': 'simple', 'explode': False }})
     r"""Name of the ledger."""
     address: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'address', 'style': 'form', 'explode': True }})
     r"""Filter accounts by address pattern (regular expression placed between ^ and $)."""
     after: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'after', 'style': 'form', 'explode': True }})
     r"""Pagination cursor, will return accounts after given address, in descending order."""
     balance: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'balance', 'style': 'form', 'explode': True }})
@@ -41,36 +33,33 @@
     r"""Operator used for the filtering of balances can be greater than/equal, less than/equal, greater than, less than, equal or not."""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     r"""Parameter used in pagination requests. Maximum page size is set to 15.
     Set to the value of next for the next page of results.
     Set to the value of previous for the previous page of results.
     No other parameters can be set when this parameter is set.
     """
-    metadata: Optional[ListAccountsMetadata] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'metadata', 'style': 'deepObject', 'explode': True }})
+    metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'metadata', 'style': 'deepObject', 'explode': True }})
     r"""Filter accounts by metadata key value pairs. Nested objects can be used as seen in the example below."""
     page_size: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'pageSize', 'style': 'form', 'explode': True }})
     r"""The maximum number of results to return per page."""
     pagination_token: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'pagination_token', 'style': 'form', 'explode': True }})
     r"""Parameter used in pagination requests. Maximum page size is set to 15.
     Set to the value of next for the next page of results.
     Set to the value of previous for the previous page of results.
     No other parameters can be set when this parameter is set.
     Deprecated, please use `cursor` instead.
-
+    
     Deprecated: this field will be removed in a future release, please migrate away from it as soon as possible
     """
     
 
-
-
-
 @dataclasses.dataclass
 class ListAccountsResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     accounts_cursor_response: Optional[shared_accountscursorresponse.AccountsCursorResponse] = dataclasses.field(default=None)
     r"""OK"""
     error_response: Optional[shared_errorresponse.ErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/listallconnectors.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listallconnectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import connectorsresponse as shared_connectorsresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class ListAllConnectorsResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     connectors_response: Optional[shared_connectorsresponse.ConnectorsResponse] = dataclasses.field(default=None)
     r"""OK"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/listbalances.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listbalances.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,25 +3,22 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import listbalancesresponse as shared_listbalancesresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class ListBalancesRequest:
+    
     id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'id', 'style': 'simple', 'explode': False }})
     
 
-
-
-
 @dataclasses.dataclass
 class ListBalancesResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     list_balances_response: Optional[shared_listbalancesresponse.ListBalancesResponse] = dataclasses.field(default=None)
     r"""Balances list"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/listclients.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listclients.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import listclientsresponse as shared_listclientsresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class ListClientsResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     list_clients_response: Optional[shared_listclientsresponse.ListClientsResponse] = dataclasses.field(default=None)
     r"""List of clients"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/listconfigsavailableconnectors.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listconfigsavailableconnectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import connectorsconfigsresponse as shared_connectorsconfigsresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class ListConfigsAvailableConnectorsResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     connectors_configs_response: Optional[shared_connectorsconfigsresponse.ConnectorsConfigsResponse] = dataclasses.field(default=None)
     r"""OK"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/listconnectorstransfers.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listconnectorstransfers.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,26 +4,23 @@
 import dataclasses
 import requests as requests_http
 from ..shared import connector as shared_connector
 from ..shared import transfersresponse as shared_transfersresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class ListConnectorsTransfersRequest:
+    
     connector: shared_connector.Connector = dataclasses.field(metadata={'path_param': { 'field_name': 'connector', 'style': 'simple', 'explode': False }})
     r"""The name of the connector."""
     
 
-
-
-
 @dataclasses.dataclass
 class ListConnectorsTransfersResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     transfers_response: Optional[shared_transfersresponse.TransfersResponse] = dataclasses.field(default=None)
     r"""OK"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/listconnectortasks.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listconnectortasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,34 +4,31 @@
 import dataclasses
 import requests as requests_http
 from ..shared import connector as shared_connector
 from ..shared import taskscursor as shared_taskscursor
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class ListConnectorTasksRequest:
+    
     connector: shared_connector.Connector = dataclasses.field(metadata={'path_param': { 'field_name': 'connector', 'style': 'simple', 'explode': False }})
     r"""The name of the connector."""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     r"""Parameter used in pagination requests. Maximum page size is set to 15.
     Set to the value of next for the next page of results.
     Set to the value of previous for the previous page of results.
     No other parameters can be set when this parameter is set.
     """
     page_size: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'pageSize', 'style': 'form', 'explode': True }})
     r"""The maximum number of results to return per page."""
     
 
-
-
-
 @dataclasses.dataclass
 class ListConnectorTasksResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     tasks_cursor: Optional[shared_taskscursor.TasksCursor] = dataclasses.field(default=None)
     r"""OK"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/listinstances.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listinstances.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,27 @@
 import dataclasses
 import requests as requests_http
 from ..shared import error as shared_error
 from ..shared import listrunsresponse as shared_listrunsresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class ListInstancesRequest:
+    
     running: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'running', 'style': 'form', 'explode': True }})
     r"""Filter running instances"""
     workflow_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'workflowID', 'style': 'form', 'explode': True }})
     r"""A workflow id"""
     
 
-
-
-
 @dataclasses.dataclass
 class ListInstancesResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     error: Optional[shared_error.Error] = dataclasses.field(default=None)
     r"""General error"""
     list_runs_response: Optional[shared_listrunsresponse.ListRunsResponse] = dataclasses.field(default=None)
     r"""List of workflow instances"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/listlogs.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listlogs.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import requests as requests_http
 from ..shared import errorresponse as shared_errorresponse
 from ..shared import logscursorresponse as shared_logscursorresponse
 from datetime import datetime
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class ListLogsRequest:
+    
     ledger: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ledger', 'style': 'simple', 'explode': False }})
     r"""Name of the ledger."""
     after: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'after', 'style': 'form', 'explode': True }})
     r"""Pagination cursor, will return the logs after a given ID. (in descending order)."""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     r"""Parameter used in pagination requests. Maximum page size is set to 15.
     Set to the value of next for the next page of results.
@@ -30,30 +30,27 @@
     r"""The maximum number of results to return per page."""
     pagination_token: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'pagination_token', 'style': 'form', 'explode': True }})
     r"""Parameter used in pagination requests. Maximum page size is set to 15.
     Set to the value of next for the next page of results.
     Set to the value of previous for the previous page of results.
     No other parameters can be set when this parameter is set.
     Deprecated, please use `cursor` instead.
-
+    
     Deprecated: this field will be removed in a future release, please migrate away from it as soon as possible
     """
     start_time: Optional[datetime] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'startTime', 'style': 'form', 'explode': True }})
     r"""Filter transactions that occurred after this timestamp.
     The format is RFC3339 and is inclusive (for example, \"2023-01-02T15:04:01Z\" includes the first second of 4th minute).
     """
     
 
-
-
-
 @dataclasses.dataclass
 class ListLogsResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     error_response: Optional[shared_errorresponse.ErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
     logs_cursor_response: Optional[shared_logscursorresponse.LogsCursorResponse] = dataclasses.field(default=None)
     r"""OK"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/listpayments.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listpayments.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,34 +3,31 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import paymentscursor as shared_paymentscursor
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class ListPaymentsRequest:
+    
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     r"""Parameter used in pagination requests. Maximum page size is set to 15.
     Set to the value of next for the next page of results.
     Set to the value of previous for the previous page of results.
     No other parameters can be set when this parameter is set.
     """
     page_size: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'pageSize', 'style': 'form', 'explode': True }})
     r"""The maximum number of results to return per page."""
     sort: Optional[list[str]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sort', 'style': 'form', 'explode': True }})
     r"""Fields used to sort payments (default is date:desc)."""
     
 
-
-
-
 @dataclasses.dataclass
 class ListPaymentsResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     payments_cursor: Optional[shared_paymentscursor.PaymentsCursor] = dataclasses.field(default=None)
     r"""OK"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/listscopes.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listscopes.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import listscopesresponse as shared_listscopesresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class ListScopesResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     list_scopes_response: Optional[shared_listscopesresponse.ListScopesResponse] = dataclasses.field(default=None)
     r"""List of scopes"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/listtransactions.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listtransactions.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,28 +2,20 @@
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import errorresponse as shared_errorresponse
 from ..shared import transactionscursorresponse as shared_transactionscursorresponse
 from datetime import datetime
-from typing import Optional
-
-
-
-@dataclasses.dataclass
-class ListTransactionsMetadata:
-    r"""Filter transactions by metadata key value pairs. Nested objects can be used as seen in the example below."""
-    
-
-
+from typing import Any, Optional
 
 
 @dataclasses.dataclass
 class ListTransactionsRequest:
+    
     ledger: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ledger', 'style': 'simple', 'explode': False }})
     r"""Name of the ledger."""
     account: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'account', 'style': 'form', 'explode': True }})
     r"""Filter transactions with postings involving given account, either as source or destination (regular expression placed between ^ and $)."""
     after: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'after', 'style': 'form', 'explode': True }})
     r"""Pagination cursor, will return transactions after given txid (in descending order)."""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
@@ -34,44 +26,41 @@
     """
     destination: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'destination', 'style': 'form', 'explode': True }})
     r"""Filter transactions with postings involving given account at destination (regular expression placed between ^ and $)."""
     end_time: Optional[datetime] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'endTime', 'style': 'form', 'explode': True }})
     r"""Filter transactions that occurred before this timestamp.
     The format is RFC3339 and is exclusive (for example, \"2023-01-02T15:04:01Z\" excludes the first second of 4th minute).
     """
-    metadata: Optional[ListTransactionsMetadata] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'metadata', 'style': 'deepObject', 'explode': True }})
+    metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'metadata', 'style': 'deepObject', 'explode': True }})
     r"""Filter transactions by metadata key value pairs. Nested objects can be used as seen in the example below."""
     page_size: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'pageSize', 'style': 'form', 'explode': True }})
     r"""The maximum number of results to return per page."""
     pagination_token: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'pagination_token', 'style': 'form', 'explode': True }})
     r"""Parameter used in pagination requests. Maximum page size is set to 15.
     Set to the value of next for the next page of results.
     Set to the value of previous for the previous page of results.
     No other parameters can be set when this parameter is set.
     Deprecated, please use `cursor` instead.
-
+    
     Deprecated: this field will be removed in a future release, please migrate away from it as soon as possible
     """
     reference: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'reference', 'style': 'form', 'explode': True }})
     r"""Find transactions by reference field."""
     source: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'source', 'style': 'form', 'explode': True }})
     r"""Filter transactions with postings involving given account at source (regular expression placed between ^ and $)."""
     start_time: Optional[datetime] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'startTime', 'style': 'form', 'explode': True }})
     r"""Filter transactions that occurred after this timestamp.
     The format is RFC3339 and is inclusive (for example, \"2023-01-02T15:04:01Z\" includes the first second of 4th minute).
     """
     
 
-
-
-
 @dataclasses.dataclass
 class ListTransactionsResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     error_response: Optional[shared_errorresponse.ErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     transactions_cursor_response: Optional[shared_transactionscursorresponse.TransactionsCursorResponse] = dataclasses.field(default=None)
     r"""OK"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/listusers.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listusers.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import listusersresponse as shared_listusersresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class ListUsersResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     list_users_response: Optional[shared_listusersresponse.ListUsersResponse] = dataclasses.field(default=None)
     r"""List of users"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/listwallets.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listwallets.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,36 +3,33 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import listwalletsresponse as shared_listwalletsresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class ListWalletsRequest:
+    
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     r"""Parameter used in pagination requests.
     Set to the value of next for the next page of results.
     Set to the value of previous for the previous page of results.
     No other parameters can be set when the pagination token is set.
     """
     metadata: Optional[dict[str, str]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'metadata', 'style': 'deepObject', 'explode': True }})
     r"""Filter wallets by metadata key value pairs. Nested objects can be used as seen in the example below."""
     name: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'name', 'style': 'form', 'explode': True }})
     r"""Filter on wallet name"""
     page_size: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'pageSize', 'style': 'form', 'explode': True }})
     r"""The maximum number of results to return per page"""
     
 
-
-
-
 @dataclasses.dataclass
 class ListWalletsResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     list_wallets_response: Optional[shared_listwalletsresponse.ListWalletsResponse] = dataclasses.field(default=None)
     r"""OK"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/listworkflows.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/listworkflows.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 import dataclasses
 import requests as requests_http
 from ..shared import error as shared_error
 from ..shared import listworkflowsresponse as shared_listworkflowsresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class ListWorkflowsResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     error: Optional[shared_error.Error] = dataclasses.field(default=None)
     r"""General error"""
     list_workflows_response: Optional[shared_listworkflowsresponse.ListWorkflowsResponse] = dataclasses.field(default=None)
     r"""List of workflows"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/paymentsgetserverinfo.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/paymentsgetserverinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import serverinfo as shared_serverinfo
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class PaymentsgetServerInfoResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     server_info: Optional[shared_serverinfo.ServerInfo] = dataclasses.field(default=None)
     r"""Server information"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/paymentslistaccounts.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/paymentslistaccounts.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,34 +3,31 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import accountscursor as shared_accountscursor
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class PaymentslistAccountsRequest:
+    
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     r"""Parameter used in pagination requests. Maximum page size is set to 15.
     Set to the value of next for the next page of results.
     Set to the value of previous for the previous page of results.
     No other parameters can be set when this parameter is set.
     """
     page_size: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'pageSize', 'style': 'form', 'explode': True }})
     r"""The maximum number of results to return per page."""
     sort: Optional[list[str]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sort', 'style': 'form', 'explode': True }})
     r"""Fields used to sort payments (default is date:desc)."""
     
 
-
-
-
 @dataclasses.dataclass
 class PaymentslistAccountsResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     accounts_cursor: Optional[shared_accountscursor.AccountsCursor] = dataclasses.field(default=None)
     r"""OK"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/readclient.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/readclient.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,26 +3,23 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import readclientresponse as shared_readclientresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class ReadClientRequest:
+    
     client_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'clientId', 'style': 'simple', 'explode': False }})
     r"""Client ID"""
     
 
-
-
-
 @dataclasses.dataclass
 class ReadClientResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     read_client_response: Optional[shared_readclientresponse.ReadClientResponse] = dataclasses.field(default=None)
     r"""Retrieved client"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/readconnectorconfig.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/resetconnector.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import connector as shared_connector
-from ..shared import connectorconfigresponse as shared_connectorconfigresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
-class ReadConnectorConfigRequest:
+class ResetConnectorRequest:
+    
     connector: shared_connector.Connector = dataclasses.field(metadata={'path_param': { 'field_name': 'connector', 'style': 'simple', 'explode': False }})
     r"""The name of the connector."""
     
 
-
-
-
 @dataclasses.dataclass
-class ReadConnectorConfigResponse:
+class ResetConnectorResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    connector_config_response: Optional[shared_connectorconfigresponse.ConnectorConfigResponse] = dataclasses.field(default=None)
-    r"""OK"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/readscope.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/readscope.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,26 +3,23 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import readscoperesponse as shared_readscoperesponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class ReadScopeRequest:
+    
     scope_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'scopeId', 'style': 'simple', 'explode': False }})
     r"""Scope ID"""
     
 
-
-
-
 @dataclasses.dataclass
 class ReadScopeResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     read_scope_response: Optional[shared_readscoperesponse.ReadScopeResponse] = dataclasses.field(default=None)
     r"""Retrieved scope"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/readstats.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/readuser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import errorresponse as shared_errorresponse
-from ..shared import statsresponse as shared_statsresponse
+from ..shared import readuserresponse as shared_readuserresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
-class ReadStatsRequest:
-    ledger: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ledger', 'style': 'simple', 'explode': False }})
-    r"""name of the ledger"""
+class ReadUserRequest:
+    
+    user_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'userId', 'style': 'simple', 'explode': False }})
+    r"""User ID"""
     
-
-
-
 
 @dataclasses.dataclass
-class ReadStatsResponse:
+class ReadUserResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    error_response: Optional[shared_errorresponse.ErrorResponse] = dataclasses.field(default=None)
-    r"""Error"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    stats_response: Optional[shared_statsresponse.StatsResponse] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    read_user_response: Optional[shared_readuserresponse.ReadUserResponse] = dataclasses.field(default=None)
+    r"""Retrieved user"""
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/readuser.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/uninstallconnector.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import readuserresponse as shared_readuserresponse
+from ..shared import connector as shared_connector
 from typing import Optional
 
 
-
 @dataclasses.dataclass
-class ReadUserRequest:
-    user_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'userId', 'style': 'simple', 'explode': False }})
-    r"""User ID"""
+class UninstallConnectorRequest:
+    
+    connector: shared_connector.Connector = dataclasses.field(metadata={'path_param': { 'field_name': 'connector', 'style': 'simple', 'explode': False }})
+    r"""The name of the connector."""
     
-
-
-
 
 @dataclasses.dataclass
-class ReadUserResponse:
+class UninstallConnectorResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    read_user_response: Optional[shared_readuserresponse.ReadUserResponse] = dataclasses.field(default=None)
-    r"""Retrieved user"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/resetconnector.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/search.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import connector as shared_connector
+from ..shared import response as shared_response
 from typing import Optional
 
 
-
 @dataclasses.dataclass
-class ResetConnectorRequest:
-    connector: shared_connector.Connector = dataclasses.field(metadata={'path_param': { 'field_name': 'connector', 'style': 'simple', 'explode': False }})
-    r"""The name of the connector."""
+class SearchResponse:
     
-
-
-
-
-@dataclasses.dataclass
-class ResetConnectorResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+    response: Optional[shared_response.Response] = dataclasses.field(default=None)
+    r"""Success"""
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/reverttransaction.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/reverttransaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,27 @@
 import dataclasses
 import requests as requests_http
 from ..shared import errorresponse as shared_errorresponse
 from ..shared import transactionresponse as shared_transactionresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class RevertTransactionRequest:
+    
     ledger: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ledger', 'style': 'simple', 'explode': False }})
     r"""Name of the ledger."""
     txid: int = dataclasses.field(metadata={'path_param': { 'field_name': 'txid', 'style': 'simple', 'explode': False }})
     r"""Transaction ID."""
     
 
-
-
-
 @dataclasses.dataclass
 class RevertTransactionResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     error_response: Optional[shared_errorresponse.ErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     transaction_response: Optional[shared_transactionresponse.TransactionResponse] = dataclasses.field(default=None)
     r"""OK"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/runscript.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/runscript.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,35 +4,32 @@
 import dataclasses
 import requests as requests_http
 from ..shared import script as shared_script
 from ..shared import scriptresponse as shared_scriptresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class RunScriptRequest:
+    
     ledger: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ledger', 'style': 'simple', 'explode': False }})
     r"""Name of the ledger."""
     script: shared_script.Script = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
     preview: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'preview', 'style': 'form', 'explode': True }})
     r"""Set the preview mode. Preview mode doesn't add the logs to the database or publish a message to the message broker."""
     
 
-
-
-
 @dataclasses.dataclass
 class RunScriptResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     script_response: Optional[shared_scriptresponse.ScriptResponse] = dataclasses.field(default=None)
     r"""On success, it will return a 200 status code, and the resulting transaction under the `transaction` field.
-
+    
     On failure, it will also return a 200 status code, and the following fields:
       - `details`: contains a URL. When there is an error parsing Numscript, the result can be difficult to read—the provided URL will render the error in an easy-to-read format.
       - `errorCode` and `error_code` (deprecated): contains the string code of the error
       - `errorMessage` and `error_message` (deprecated): contains a human-readable indication of what went wrong, for example that an account had insufficient funds, or that there was an error in the provided Numscript.
     """
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/runworkflow.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/runworkflow.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,31 +4,28 @@
 import dataclasses
 import requests as requests_http
 from ..shared import error as shared_error
 from ..shared import runworkflowresponse as shared_runworkflowresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class RunWorkflowRequest:
+    
     workflow_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'workflowID', 'style': 'simple', 'explode': False }})
     r"""The flow id"""
     request_body: Optional[dict[str, str]] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     wait: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'wait', 'style': 'form', 'explode': True }})
     r"""Wait end of the workflow before return"""
     
 
-
-
-
 @dataclasses.dataclass
 class RunWorkflowResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     error: Optional[shared_error.Error] = dataclasses.field(default=None)
     r"""General error"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     run_workflow_response: Optional[shared_runworkflowresponse.RunWorkflowResponse] = dataclasses.field(default=None)
     r"""The workflow instance"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/search.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/listrunsresponse.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-import requests as requests_http
-from ..shared import response as shared_response
-from typing import Optional
-
+from ..shared import workflowinstance as shared_workflowinstance
+from dataclasses_json import Undefined, dataclass_json
+from sdk import utils
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response: Optional[shared_response.Response] = dataclasses.field(default=None)
-    r"""Success"""
+class ListRunsResponse:
+    r"""List of workflow instances"""
     
-
+    data: list[shared_workflowinstance.WorkflowInstance] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/searchgetserverinfo.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/searchgetserverinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import serverinfo as shared_serverinfo
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class SearchgetServerInfoResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     server_info: Optional[shared_serverinfo.ServerInfo] = dataclasses.field(default=None)
     r"""Server information"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/sendevent.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/sendevent.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,35 +6,30 @@
 from ..shared import error as shared_error
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class SendEventRequestBody:
+    
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
     
 
-
-
-
 @dataclasses.dataclass
 class SendEventRequest:
+    
     instance_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'instanceID', 'style': 'simple', 'explode': False }})
     r"""The instance id"""
     request_body: Optional[SendEventRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
-
-
-
 @dataclasses.dataclass
 class SendEventResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     error: Optional[shared_error.Error] = dataclasses.field(default=None)
     r"""General error"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/testconfig.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/testconfig.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,28 +4,25 @@
 import dataclasses
 import requests as requests_http
 from ..shared import attemptresponse as shared_attemptresponse
 from ..shared import webhookserrorresponse as shared_webhookserrorresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class TestConfigRequest:
+    
     id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'id', 'style': 'simple', 'explode': False }})
     r"""Config ID"""
     
 
-
-
-
 @dataclasses.dataclass
 class TestConfigResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     attempt_response: Optional[shared_attemptresponse.AttemptResponse] = dataclasses.field(default=None)
     r"""OK"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     webhooks_error_response: Optional[shared_webhookserrorresponse.WebhooksErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/uninstallconnector.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/workflowconfig.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-import requests as requests_http
-from ..shared import connector as shared_connector
-from typing import Optional
-
-
-
-@dataclasses.dataclass
-class UninstallConnectorRequest:
-    connector: shared_connector.Connector = dataclasses.field(metadata={'path_param': { 'field_name': 'connector', 'style': 'simple', 'explode': False }})
-    r"""The name of the connector."""
-    
-
-
+from dataclasses_json import Undefined, dataclass_json
+from sdk import utils
+from typing import Any, Optional
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class UninstallConnectorResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+class WorkflowConfig:
     
-
+    stages: list[dict[str, Any]] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stages') }})
+    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/updateclient.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/createsecret.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import updateclientrequest as shared_updateclientrequest
-from ..shared import updateclientresponse as shared_updateclientresponse
+from ..shared import createsecretrequest as shared_createsecretrequest
+from ..shared import createsecretresponse as shared_createsecretresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
-class UpdateClientRequest:
+class CreateSecretRequest:
+    
     client_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'clientId', 'style': 'simple', 'explode': False }})
     r"""Client ID"""
-    update_client_request: Optional[shared_updateclientrequest.UpdateClientRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    create_secret_request: Optional[shared_createsecretrequest.CreateSecretRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
-
-
-
 @dataclasses.dataclass
-class UpdateClientResponse:
+class CreateSecretResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
+    create_secret_response: Optional[shared_createsecretresponse.CreateSecretResponse] = dataclasses.field(default=None)
+    r"""Created secret"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    update_client_response: Optional[shared_updateclientresponse.UpdateClientResponse] = dataclasses.field(default=None)
-    r"""Updated client"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/updatemapping.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/getmanyconfigs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import errorresponse as shared_errorresponse
-from ..shared import mapping as shared_mapping
-from ..shared import mappingresponse as shared_mappingresponse
+from ..shared import configsresponse as shared_configsresponse
+from ..shared import webhookserrorresponse as shared_webhookserrorresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
-class UpdateMappingRequest:
-    ledger: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ledger', 'style': 'simple', 'explode': False }})
-    r"""Name of the ledger."""
-    mapping: shared_mapping.Mapping = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
+class GetManyConfigsRequest:
+    
+    endpoint: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'endpoint', 'style': 'form', 'explode': True }})
+    r"""Optional filter by endpoint URL"""
+    id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
+    r"""Optional filter by Config ID"""
     
-
-
-
 
 @dataclasses.dataclass
-class UpdateMappingResponse:
+class GetManyConfigsResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    error_response: Optional[shared_errorresponse.ErrorResponse] = dataclasses.field(default=None)
-    r"""Error"""
-    mapping_response: Optional[shared_mappingresponse.MappingResponse] = dataclasses.field(default=None)
+    configs_response: Optional[shared_configsresponse.ConfigsResponse] = dataclasses.field(default=None)
     r"""OK"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+    webhooks_error_response: Optional[shared_webhookserrorresponse.WebhooksErrorResponse] = dataclasses.field(default=None)
+    r"""Error"""
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/updatemetadata.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/updatemetadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,25 +3,22 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import paymentmetadata as shared_paymentmetadata
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class UpdateMetadataRequest:
+    
     payment_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'paymentId', 'style': 'simple', 'explode': False }})
     r"""The payment ID."""
     payment_metadata: shared_paymentmetadata.PaymentMetadata = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
     
 
-
-
-
 @dataclasses.dataclass
 class UpdateMetadataResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/updatescope.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/updatescope.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,27 +4,24 @@
 import dataclasses
 import requests as requests_http
 from ..shared import updatescoperequest as shared_updatescoperequest
 from ..shared import updatescoperesponse as shared_updatescoperesponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class UpdateScopeRequest:
+    
     scope_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'scopeId', 'style': 'simple', 'explode': False }})
     r"""Scope ID"""
     update_scope_request: Optional[shared_updatescoperequest.UpdateScopeRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
-
-
-
 @dataclasses.dataclass
 class UpdateScopeResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     update_scope_response: Optional[shared_updatescoperesponse.UpdateScopeResponse] = dataclasses.field(default=None)
     r"""Updated scope"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/updatewallet.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/updatewallet.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,35 +6,30 @@
 from ..shared import walletserrorresponse as shared_walletserrorresponse
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class UpdateWalletRequestBody:
+    
     metadata: dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata') }})
     r"""Custom metadata to attach to this wallet."""
     
 
-
-
-
 @dataclasses.dataclass
 class UpdateWalletRequest:
+    
     id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'id', 'style': 'simple', 'explode': False }})
     request_body: Optional[UpdateWalletRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
-
-
-
 @dataclasses.dataclass
 class UpdateWalletResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     wallets_error_response: Optional[shared_walletserrorresponse.WalletsErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/voidhold.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/balance.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-import requests as requests_http
-from ..shared import walletserrorresponse as shared_walletserrorresponse
+import dateutil.parser
+from dataclasses_json import Undefined, dataclass_json
+from datetime import datetime
+from marshmallow import fields
+from sdk import utils
 from typing import Optional
 
 
-
-@dataclasses.dataclass
-class VoidHoldRequest:
-    hold_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'hold_id', 'style': 'simple', 'explode': False }})
-    
-
-
-
-
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class VoidHoldResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    wallets_error_response: Optional[shared_walletserrorresponse.WalletsErrorResponse] = dataclasses.field(default=None)
-    r"""Error"""
+class Balance:
     
-
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    expires_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expiresAt'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+    priority: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('priority'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/operations/walletsgetserverinfo.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/walletsgetserverinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 import dataclasses
 import requests as requests_http
 from ..shared import serverinfo as shared_serverinfo
 from ..shared import walletserrorresponse as shared_walletserrorresponse
 from typing import Optional
 
 
-
 @dataclasses.dataclass
 class WalletsgetServerInfoResponse:
+    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     server_info: Optional[shared_serverinfo.ServerInfo] = dataclasses.field(default=None)
     r"""Server information"""
     wallets_error_response: Optional[shared_walletserrorresponse.WalletsErrorResponse] = dataclasses.field(default=None)
     r"""Error"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/__init__.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -128,15 +128,14 @@
 from .stagesendsourcewallet import *
 from .stagestatus import *
 from .stagewaitevent import *
 from .stats import *
 from .statsresponse import *
 from .stripeconfig import *
 from .stripetransferrequest import *
-from .stripetransferresponse import *
 from .taskbankingcircle import *
 from .taskcurrencycloud import *
 from .taskdummypay import *
 from .taskmodulr import *
 from .taskresponse import *
 from .taskscursor import *
 from .taskstripe import *
@@ -171,8 +170,8 @@
 from .workflowconfig import *
 from .workflowinstance import *
 from .workflowinstancehistory import *
 from .workflowinstancehistorystage import *
 from .workflowinstancehistorystageinput import *
 from .workflowinstancehistorystageoutput import *
 
-__all__ = ["Account","AccountMetadata","AccountResponse","AccountWithVolumesAndBalances","AccountWithVolumesAndBalancesMetadata","AccountsCursor","AccountsCursorCursor","AccountsCursorResponse","AccountsCursorResponseCursor","ActivityConfirmHold","ActivityCreateTransaction","ActivityCreateTransactionOutput","ActivityCreditWallet","ActivityDebitWallet","ActivityDebitWalletOutput","ActivityGetAccount","ActivityGetAccountOutput","ActivityGetPayment","ActivityGetPaymentOutput","ActivityGetWallet","ActivityGetWalletOutput","ActivityRevertTransaction","ActivityRevertTransactionOutput","ActivityStripeTransfer","ActivityStripeTransferMetadata","ActivityVoidHold","AggregateBalancesResponse","AssetHolder","Attempt","AttemptResponse","Balance","BalanceWithAssets","BalancesCursorResponse","BalancesCursorResponseCursor","BankingCircleConfig","Client","ClientSecret","Config","ConfigChangeSecret","ConfigInfo","ConfigInfoResponse","ConfigResponse","ConfigUser","ConfigsResponse","ConfigsResponseCursor","ConfirmHoldRequest","Connector","ConnectorConfigResponse","ConnectorsConfigsResponse","ConnectorsConfigsResponseData","ConnectorsConfigsResponseDataConnector","ConnectorsConfigsResponseDataConnectorKey","ConnectorsResponse","ConnectorsResponseData","Contract","ContractExpr","CreateBalanceRequest","CreateBalanceResponse","CreateClientRequest","CreateClientResponse","CreateScopeRequest","CreateScopeResponse","CreateSecretRequest","CreateSecretResponse","CreateWalletRequest","CreateWalletResponse","CreateWorkflowRequest","CreateWorkflowResponse","CreditWalletRequest","CurrencyCloudConfig","DebitWalletRequest","DebitWalletResponse","DummyPayConfig","Error","ErrorErrorCode","ErrorResponse","ErrorsEnum","ExpandedDebitHold","GetBalanceResponse","GetHoldResponse","GetHoldsResponse","GetHoldsResponseCursor","GetTransactionsResponse","GetTransactionsResponseCursor","GetVersionsResponse","GetWalletResponse","GetWalletSummaryResponse","GetWorkflowInstanceHistoryResponse","GetWorkflowInstanceHistoryStageResponse","GetWorkflowInstanceResponse","GetWorkflowResponse","Hold","LedgerAccountSubject","LedgerInfo","LedgerInfoResponse","LedgerInfoStorage","LedgerStorage","ListBalancesResponse","ListBalancesResponseCursor","ListClientsResponse","ListRunsResponse","ListScopesResponse","ListUsersResponse","ListWalletsResponse","ListWalletsResponseCursor","ListWorkflowsResponse","Log","LogData","LogType","LogsCursorResponse","LogsCursorResponseCursor","Mapping","MappingResponse","MigrationInfo","MigrationInfoState","ModulrConfig","Monetary","Payment","PaymentAdjustment","PaymentAdjustmentRaw","PaymentMetadata","PaymentRaw","PaymentResponse","PaymentScheme","PaymentStatus","PaymentType","PaymentsAccount","PaymentsAccountType","PaymentsCursor","PaymentsCursorCursor","PostTransaction","PostTransactionScript","PostTransactionScriptVars","Posting","Query","QueryRaw","ReadClientResponse","ReadScopeResponse","ReadUserResponse","Response","ResponseCursor","ResponseCursorData","ResponseCursorTotal","ResponseData","RunWorkflowResponse","Scope","Script","ScriptResponse","ScriptVars","Secret","Security","ServerInfo","StageDelay","StageSend","StageSendDestination","StageSendDestinationAccount","StageSendDestinationPayment","StageSendDestinationWallet","StageSendSource","StageSendSourceAccount","StageSendSourcePayment","StageSendSourceWallet","StageStatus","StageWaitEvent","Stats","StatsResponse","StripeConfig","StripeTransferRequest","StripeTransferRequestMetadata","StripeTransferResponse","TaskBankingCircle","TaskBankingCircleDescriptor","TaskBankingCircleState","TaskCurrencyCloud","TaskCurrencyCloudDescriptor","TaskCurrencyCloudState","TaskDummyPay","TaskDummyPayDescriptor","TaskDummyPayState","TaskModulr","TaskModulrDescriptor","TaskModulrState","TaskResponse","TaskStripe","TaskStripeDescriptor","TaskStripeState","TaskWise","TaskWiseDescriptor","TaskWiseState","TasksCursor","TasksCursorCursor","Transaction","TransactionData","TransactionResponse","Transactions","TransactionsCursorResponse","TransactionsCursorResponseCursor","TransactionsResponse","TransferRequest","TransferResponse","TransfersResponse","TransfersResponseData","UpdateClientRequest","UpdateClientResponse","UpdateScopeRequest","UpdateScopeResponse","User","Version","Volume","Wallet","WalletSubject","WalletWithBalances","WalletWithBalancesBalances","WalletsErrorResponse","WalletsErrorResponseErrorCode","WalletsTransaction","WalletsVolume","WebhooksConfig","WebhooksErrorResponse","WebhooksErrorsEnum","WiseConfig","Workflow","WorkflowConfig","WorkflowInstance","WorkflowInstanceHistory","WorkflowInstanceHistoryStage","WorkflowInstanceHistoryStageInput","WorkflowInstanceHistoryStageOutput"]
+__all__ = ["Account","AccountResponse","AccountWithVolumesAndBalances","AccountsCursor","AccountsCursorCursor","AccountsCursorResponse","AccountsCursorResponseCursor","ActivityConfirmHold","ActivityCreateTransaction","ActivityCreateTransactionOutput","ActivityCreditWallet","ActivityDebitWallet","ActivityDebitWalletOutput","ActivityGetAccount","ActivityGetAccountOutput","ActivityGetPayment","ActivityGetPaymentOutput","ActivityGetWallet","ActivityGetWalletOutput","ActivityRevertTransaction","ActivityRevertTransactionOutput","ActivityStripeTransfer","ActivityVoidHold","AggregateBalancesResponse","AssetHolder","Attempt","AttemptResponse","Balance","BalanceWithAssets","BalancesCursorResponse","BalancesCursorResponseCursor","BankingCircleConfig","Client","ClientSecret","Config","ConfigChangeSecret","ConfigInfo","ConfigInfoResponse","ConfigResponse","ConfigUser","ConfigsResponse","ConfigsResponseCursor","ConfirmHoldRequest","Connector","ConnectorConfigResponse","ConnectorsConfigsResponse","ConnectorsConfigsResponseData","ConnectorsConfigsResponseDataConnector","ConnectorsConfigsResponseDataConnectorKey","ConnectorsResponse","ConnectorsResponseData","Contract","CreateBalanceRequest","CreateBalanceResponse","CreateClientRequest","CreateClientResponse","CreateScopeRequest","CreateScopeResponse","CreateSecretRequest","CreateSecretResponse","CreateWalletRequest","CreateWalletResponse","CreateWorkflowRequest","CreateWorkflowResponse","CreditWalletRequest","CurrencyCloudConfig","DebitWalletRequest","DebitWalletResponse","DummyPayConfig","Error","ErrorErrorCode","ErrorResponse","ErrorsEnum","ExpandedDebitHold","GetBalanceResponse","GetHoldResponse","GetHoldsResponse","GetHoldsResponseCursor","GetTransactionsResponse","GetTransactionsResponseCursor","GetVersionsResponse","GetWalletResponse","GetWalletSummaryResponse","GetWorkflowInstanceHistoryResponse","GetWorkflowInstanceHistoryStageResponse","GetWorkflowInstanceResponse","GetWorkflowResponse","Hold","LedgerAccountSubject","LedgerInfo","LedgerInfoResponse","LedgerInfoStorage","LedgerStorage","ListBalancesResponse","ListBalancesResponseCursor","ListClientsResponse","ListRunsResponse","ListScopesResponse","ListUsersResponse","ListWalletsResponse","ListWalletsResponseCursor","ListWorkflowsResponse","Log","LogType","LogsCursorResponse","LogsCursorResponseCursor","Mapping","MappingResponse","MigrationInfo","MigrationInfoState","ModulrConfig","Monetary","Payment","PaymentAdjustment","PaymentMetadata","PaymentResponse","PaymentScheme","PaymentStatus","PaymentType","PaymentsAccount","PaymentsAccountType","PaymentsCursor","PaymentsCursorCursor","PostTransaction","PostTransactionScript","Posting","Query","ReadClientResponse","ReadScopeResponse","ReadUserResponse","Response","ResponseCursor","ResponseCursorTotal","RunWorkflowResponse","Scope","Script","ScriptResponse","Secret","Security","ServerInfo","StageDelay","StageSend","StageSendDestination","StageSendDestinationAccount","StageSendDestinationPayment","StageSendDestinationWallet","StageSendSource","StageSendSourceAccount","StageSendSourcePayment","StageSendSourceWallet","StageStatus","StageWaitEvent","Stats","StatsResponse","StripeConfig","StripeTransferRequest","TaskBankingCircle","TaskBankingCircleDescriptor","TaskCurrencyCloud","TaskCurrencyCloudDescriptor","TaskDummyPay","TaskDummyPayDescriptor","TaskModulr","TaskModulrDescriptor","TaskResponse","TaskStripe","TaskStripeDescriptor","TaskWise","TaskWiseDescriptor","TasksCursor","TasksCursorCursor","Transaction","TransactionData","TransactionResponse","Transactions","TransactionsCursorResponse","TransactionsCursorResponseCursor","TransactionsResponse","TransferRequest","TransferResponse","TransfersResponse","TransfersResponseData","UpdateClientRequest","UpdateClientResponse","UpdateScopeRequest","UpdateScopeResponse","User","Version","Volume","Wallet","WalletSubject","WalletWithBalances","WalletWithBalancesBalances","WalletsErrorResponse","WalletsErrorResponseErrorCode","WalletsTransaction","WalletsVolume","WebhooksConfig","WebhooksErrorResponse","WebhooksErrorsEnum","WiseConfig","Workflow","WorkflowConfig","WorkflowInstance","WorkflowInstanceHistory","WorkflowInstanceHistoryStage","WorkflowInstanceHistoryStageInput","WorkflowInstanceHistoryStageOutput"]
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/account.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/creditwalletrequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from ..shared import monetary as shared_monetary
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
-from typing import Optional
-
-
-
-@dataclasses.dataclass
-class AccountMetadata:
-    pass
+from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class Account:
-    address: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address') }})
-    metadata: Optional[AccountMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
-    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
+class CreditWalletRequest:
     
-
+    amount: shared_monetary.Monetary = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount') }})
+    metadata: dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata') }})
+    r"""Metadata associated with the wallet."""
+    sources: list[Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sources') }})
+    balance: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balance'), 'exclude': lambda f: f is None }})
+    r"""The balance to credit"""
+    reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/accountresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/accountresponse.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,13 @@
 import dataclasses
 from ..shared import accountwithvolumesandbalances as shared_accountwithvolumesandbalances
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class AccountResponse:
     r"""OK"""
-    data: shared_accountwithvolumesandbalances.AccountWithVolumesAndBalances = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     
-
+    data: shared_accountwithvolumesandbalances.AccountWithVolumesAndBalances = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/accountscursor.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/accountscursor.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,27 +5,24 @@
 from ..shared import paymentsaccount as shared_paymentsaccount
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class AccountsCursorCursor:
+    
     data: list[shared_paymentsaccount.PaymentsAccount] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     has_more: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasMore') }})
     page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
     next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
     previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class AccountsCursor:
     r"""OK"""
-    cursor: AccountsCursorCursor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor') }})
     
-
+    cursor: AccountsCursorCursor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/accountscursorresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/balancescursorresponse.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import account as shared_account
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class AccountsCursorResponseCursor:
-    data: list[shared_account.Account] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+class BalancesCursorResponseCursor:
+    
+    data: list[dict[str, dict[str, int]]] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     has_more: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasMore') }})
     page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
     next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
     previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class AccountsCursorResponse:
+class BalancesCursorResponse:
     r"""OK"""
-    cursor: AccountsCursorResponseCursor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor') }})
     
-
+    cursor: BalancesCursorResponseCursor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/accountwithvolumesandbalances.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/accountwithvolumesandbalances.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
-from typing import Optional
-
-
-
-@dataclasses.dataclass
-class AccountWithVolumesAndBalancesMetadata:
-    pass
+from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class AccountWithVolumesAndBalances:
+    
     address: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address') }})
     balances: Optional[dict[str, int]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balances'), 'exclude': lambda f: f is None }})
-    metadata: Optional[AccountWithVolumesAndBalancesMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
+    metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
     volumes: Optional[dict[str, dict[str, int]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('volumes'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/activitycreatetransaction.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitycreatetransaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,13 @@
 from ..shared import posttransaction as shared_posttransaction
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ActivityCreateTransaction:
+    
     data: Optional[shared_posttransaction.PostTransaction] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
     ledger: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ledger'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/activitycreatetransactionoutput.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitycreatetransactionoutput.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,13 +4,12 @@
 import dataclasses
 from ..shared import transaction as shared_transaction
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ActivityCreateTransactionOutput:
-    data: list[shared_transaction.Transaction] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     
-
+    data: list[shared_transaction.Transaction] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/activitycreditwallet.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitycreditwallet.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,13 @@
 from ..shared import creditwalletrequest as shared_creditwalletrequest
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ActivityCreditWallet:
+    
     data: Optional[shared_creditwalletrequest.CreditWalletRequest] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/activitydebitwallet.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitydebitwallet.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,13 @@
 from ..shared import debitwalletrequest as shared_debitwalletrequest
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ActivityDebitWallet:
+    
     data: Optional[shared_debitwalletrequest.DebitWalletRequest] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/activitygetaccount.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitygetaccount.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,13 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ActivityGetAccount:
+    
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     ledger: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ledger') }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/activitygetaccountoutput.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitygetaccountoutput.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,13 +4,12 @@
 import dataclasses
 from ..shared import accountwithvolumesandbalances as shared_accountwithvolumesandbalances
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ActivityGetAccountOutput:
-    data: shared_accountwithvolumesandbalances.AccountWithVolumesAndBalances = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     
-
+    data: shared_accountwithvolumesandbalances.AccountWithVolumesAndBalances = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/activitygetwalletoutput.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitygetwalletoutput.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,13 +4,12 @@
 import dataclasses
 from ..shared import walletwithbalances as shared_walletwithbalances
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ActivityGetWalletOutput:
-    data: shared_walletwithbalances.WalletWithBalances = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     
-
+    data: shared_walletwithbalances.WalletWithBalances = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/activityreverttransaction.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/ledgeraccountsubject.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,13 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class ActivityRevertTransaction:
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    ledger: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ledger') }})
+class LedgerAccountSubject:
     
-
+    identifier: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('identifier') }})
+    type: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/activityreverttransactionoutput.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/activityreverttransactionoutput.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,13 +4,12 @@
 import dataclasses
 from ..shared import transaction as shared_transaction
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ActivityRevertTransactionOutput:
-    data: list[shared_transaction.Transaction] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     
-
+    data: list[shared_transaction.Transaction] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/activitystripetransfer.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/activitystripetransfer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,21 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
-from typing import Optional
-
-
-
-@dataclasses.dataclass
-class ActivityStripeTransferMetadata:
-    r"""A set of key/value pairs that you can attach to a transfer object.
-    It can be useful for storing additional information about the transfer in a structured format.
-    """
-    
-
+from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ActivityStripeTransfer:
+    
     amount: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount'), 'exclude': lambda f: f is None }})
     asset: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('asset'), 'exclude': lambda f: f is None }})
     destination: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destination'), 'exclude': lambda f: f is None }})
-    metadata: Optional[ActivityStripeTransferMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
+    metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     r"""A set of key/value pairs that you can attach to a transfer object.
     It can be useful for storing additional information about the transfer in a structured format.
     """
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/attempt.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/attempt.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,22 +8,21 @@
 from datetime import datetime
 from marshmallow import fields
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class Attempt:
+    
     config: shared_webhooksconfig.WebhooksConfig = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('config') }})
     created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     payload: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('payload') }})
     retry_attempt: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('retryAttempt') }})
     status: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
     status_code: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusCode') }})
     updated_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
     webhook_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhookID') }})
     next_retry_after: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextRetryAfter'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/balance.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/createbalancerequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from datetime import datetime
 from marshmallow import fields
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class Balance:
+class CreateBalanceRequest:
+    
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
     expires_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expiresAt'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
     priority: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('priority'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/balancescursorresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/logscursorresponse.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from ..shared import log as shared_log
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class BalancesCursorResponseCursor:
-    data: list[dict[str, dict[str, int]]] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+class LogsCursorResponseCursor:
+    
+    data: list[shared_log.Log] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     has_more: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasMore') }})
     page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
     next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
     previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class BalancesCursorResponse:
+class LogsCursorResponse:
     r"""OK"""
-    cursor: BalancesCursorResponseCursor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor') }})
     
-
+    cursor: LogsCursorResponseCursor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/balancewithassets.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/balancewithassets.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 from datetime import datetime
 from marshmallow import fields
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class BalanceWithAssets:
+    
     assets: dict[str, int] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('assets') }})
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
     expires_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expiresAt'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
     priority: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('priority'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/bankingcircleconfig.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/posting.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class BankingCircleConfig:
-    authorization_endpoint: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('authorizationEndpoint') }})
-    endpoint: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endpoint') }})
-    password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password') }})
-    username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
+class Posting:
     
-
+    amount: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount') }})
+    asset: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('asset') }})
+    destination: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destination') }})
+    source: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('source') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/client.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,22 +5,21 @@
 from ..shared import clientsecret as shared_clientsecret
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class Client:
+    
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
     description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
     metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     post_logout_redirect_uris: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postLogoutRedirectUris'), 'exclude': lambda f: f is None }})
     public: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('public'), 'exclude': lambda f: f is None }})
     redirect_uris: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('redirectUris'), 'exclude': lambda f: f is None }})
     scopes: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('scopes'), 'exclude': lambda f: f is None }})
     secrets: Optional[list[shared_clientsecret.ClientSecret]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secrets'), 'exclude': lambda f: f is None }})
     trusted: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trusted'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/clientsecret.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/clientsecret.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ClientSecret:
+    
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     last_digits: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastDigits') }})
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
     metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/configinfo.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/configinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import dataclasses
 from ..shared import config as shared_config
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ConfigInfo:
+    
     config: shared_config.Config = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('config') }})
     server: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('server') }})
     version: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('version') }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/configinforesponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesendsourceaccount.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import configinfo as shared_configinfo
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
+from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class ConfigInfoResponse:
-    r"""OK"""
-    data: shared_configinfo.ConfigInfo = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+class StageSendSourceAccount:
     
-
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    ledger: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ledger'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/configresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/configresponse.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,13 @@
 import dataclasses
 from ..shared import webhooksconfig as shared_webhooksconfig
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ConfigResponse:
     r"""Config created successfully."""
-    data: shared_webhooksconfig.WebhooksConfig = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     
-
+    data: shared_webhooksconfig.WebhooksConfig = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/configsresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/configsresponse.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,21 @@
 import dataclasses
 from ..shared import webhooksconfig as shared_webhooksconfig
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ConfigsResponseCursor:
+    
     data: list[shared_webhooksconfig.WebhooksConfig] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     has_more: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasMore') }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ConfigsResponse:
     r"""OK"""
-    cursor: ConfigsResponseCursor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor') }})
     
-
+    cursor: ConfigsResponseCursor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/configuser.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/configuser.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ConfigUser:
+    
     endpoint: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endpoint') }})
     event_types: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventTypes') }})
     secret: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secret'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/confirmholdrequest.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/confirmholdrequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ConfirmHoldRequest:
+    
     amount: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount'), 'exclude': lambda f: f is None }})
     r"""Define the amount to transfer."""
     final: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('final'), 'exclude': lambda f: f is None }})
     r"""Define a final confirmation. Remaining funds will be returned to the wallet."""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/connectorsconfigsresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/connectorsconfigsresponse.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,42 +3,35 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ConnectorsConfigsResponseDataConnectorKey:
+    
     data_type: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataType') }})
     required: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('required') }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ConnectorsConfigsResponseDataConnector:
+    
     key: ConnectorsConfigsResponseDataConnectorKey = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key') }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ConnectorsConfigsResponseData:
+    
     connector: ConnectorsConfigsResponseDataConnector = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connector') }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ConnectorsConfigsResponse:
     r"""OK"""
-    data: ConnectorsConfigsResponseData = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     
-
+    data: ConnectorsConfigsResponseData = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/connectorsresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/connectorsresponse.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,21 @@
 from ..shared import connector as shared_connector
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ConnectorsResponseData:
+    
     enabled: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('enabled'), 'exclude': lambda f: f is None }})
     provider: Optional[shared_connector.Connector] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('provider'), 'exclude': lambda f: f is None }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ConnectorsResponse:
     r"""OK"""
-    data: list[ConnectorsResponseData] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     
-
+    data: list[ConnectorsResponseData] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/contract.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/transferrequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,21 +3,16 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
-
-@dataclasses.dataclass
-class ContractExpr:
-    pass
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class Contract:
-    expr: ContractExpr = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expr') }})
-    account: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account'), 'exclude': lambda f: f is None }})
+class TransferRequest:
     
-
+    amount: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount') }})
+    asset: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('asset') }})
+    destination: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destination') }})
+    source: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('source'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/createbalancerequest.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagestatus.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from datetime import datetime
 from marshmallow import fields
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class CreateBalanceRequest:
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    expires_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expiresAt'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    priority: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('priority'), 'exclude': lambda f: f is None }})
+class StageStatus:
     
-
+    instance_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('instanceID') }})
+    stage: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stage') }})
+    started_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
+    terminated_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('terminatedAt'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/createbalanceresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/createbalanceresponse.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,13 @@
 import dataclasses
 from ..shared import balance as shared_balance
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class CreateBalanceResponse:
     r"""Created balance"""
-    data: shared_balance.Balance = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     
-
+    data: shared_balance.Balance = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/createclientrequest.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/updateclientrequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class CreateClientRequest:
+class UpdateClientRequest:
+    
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
     description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
     metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     post_logout_redirect_uris: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postLogoutRedirectUris'), 'exclude': lambda f: f is None }})
     public: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('public'), 'exclude': lambda f: f is None }})
     redirect_uris: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('redirectUris'), 'exclude': lambda f: f is None }})
     trusted: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trusted'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/createclientresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/createclientresponse.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,13 @@
 from ..shared import client as shared_client
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class CreateClientResponse:
     r"""Client created"""
-    data: Optional[shared_client.Client] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
     
-
+    data: Optional[shared_client.Client] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/createscoperequest.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/bankingcircleconfig.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
-from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class CreateScopeRequest:
-    label: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('label') }})
-    metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
+class BankingCircleConfig:
     
-
+    authorization_endpoint: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('authorizationEndpoint') }})
+    endpoint: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endpoint') }})
+    password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password') }})
+    username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/createscoperesponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/readscoperesponse.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,13 @@
 from ..shared import scope as shared_scope
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class CreateScopeResponse:
-    r"""Created scope"""
-    data: Optional[shared_scope.Scope] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+class ReadScopeResponse:
+    r"""Retrieved scope"""
     
-
+    data: Optional[shared_scope.Scope] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/createsecretrequest.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/createscoperequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,13 @@
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class CreateSecretRequest:
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
+class CreateScopeRequest:
     
-
+    label: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('label') }})
+    metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/createsecretresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/createsecretresponse.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,13 @@
 from ..shared import secret as shared_secret
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class CreateSecretResponse:
     r"""Created secret"""
-    data: Optional[shared_secret.Secret] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
     
-
+    data: Optional[shared_secret.Secret] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/createwalletrequest.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/createsecretrequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
+from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class CreateWalletRequest:
-    metadata: dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata') }})
-    r"""Custom metadata to attach to this wallet."""
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+class CreateSecretRequest:
     
-
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/createwalletresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/createwalletresponse.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,13 @@
 import dataclasses
 from ..shared import wallet as shared_wallet
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class CreateWalletResponse:
     r"""Wallet created"""
-    data: shared_wallet.Wallet = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     
-
+    data: shared_wallet.Wallet = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/createworkflowrequest.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/createworkflowrequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,13 @@
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class CreateWorkflowRequest:
+    
     stages: list[dict[str, Any]] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stages') }})
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/createworkflowresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/createworkflowresponse.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,13 @@
 import dataclasses
 from ..shared import workflow as shared_workflow
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class CreateWorkflowResponse:
     r"""Created workflow"""
-    data: shared_workflow.Workflow = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     
-
+    data: shared_workflow.Workflow = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/creditwalletrequest.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/getholdsresponse.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import monetary as shared_monetary
+from ..shared import hold as shared_hold
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
-from typing import Any, Optional
+from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class CreditWalletRequest:
-    amount: shared_monetary.Monetary = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount') }})
-    metadata: dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata') }})
-    r"""Metadata associated with the wallet."""
-    sources: list[Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sources') }})
-    balance: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balance'), 'exclude': lambda f: f is None }})
-    r"""The balance to credit"""
-    reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})
+class GetHoldsResponseCursor:
+    
+    data: list[shared_hold.Hold] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
+    has_more: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasMore'), 'exclude': lambda f: f is None }})
+    next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
+    previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
     
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class GetHoldsResponse:
+    r"""Holds"""
+    
+    cursor: GetHoldsResponseCursor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/currencycloudconfig.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/currencycloudconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class CurrencyCloudConfig:
+    
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('apiKey') }})
     login_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('loginID') }})
     r"""Username of the API Key holder"""
     endpoint: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endpoint'), 'exclude': lambda f: f is None }})
     r"""The endpoint to use for the API. Defaults to https://devapi.currencycloud.com"""
     polling_period: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pollingPeriod'), 'exclude': lambda f: f is None }})
     r"""The frequency at which the connector will fetch transactions"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/debitwalletrequest.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/debitwalletrequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,20 +5,19 @@
 from ..shared import monetary as shared_monetary
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class DebitWalletRequest:
+    
     amount: shared_monetary.Monetary = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount') }})
     metadata: dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata') }})
     r"""Metadata associated with the wallet."""
     balances: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balances'), 'exclude': lambda f: f is None }})
     description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
     destination: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destination'), 'exclude': lambda f: f is None }})
     pending: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pending'), 'exclude': lambda f: f is None }})
     r"""Set to true to create a pending hold. If false, the wallet will be debited immediately."""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/debitwalletresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/debitwalletresponse.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,13 @@
 import dataclasses
 from ..shared import hold as shared_hold
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class DebitWalletResponse:
     r"""Wallet successfully debited as a pending hold"""
-    data: shared_hold.Hold = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     
-
+    data: shared_hold.Hold = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/dummypayconfig.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/dummypayconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class DummyPayConfig:
+    
     directory: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('directory') }})
     file_generation_period: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fileGenerationPeriod'), 'exclude': lambda f: f is None }})
     r"""The frequency at which the connector will create new payment objects in the directory"""
     file_polling_period: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filePollingPeriod'), 'exclude': lambda f: f is None }})
     r"""The frequency at which the connector will try to fetch new payment objects from the directory"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/error.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/walletserrorresponse.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from sdk import utils
 
-class ErrorErrorCode(str, Enum):
+class WalletsErrorResponseErrorCode(str, Enum):
     VALIDATION = 'VALIDATION'
-    NOT_FOUND = 'NOT_FOUND'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class Error:
-    r"""General error"""
-    error_code: ErrorErrorCode = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorCode') }})
-    error_message: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage') }})
+class WalletsErrorResponse:
+    r"""Error"""
     
-
+    error_code: WalletsErrorResponseErrorCode = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorCode') }})
+    error_message: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/errorresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/errorresponse.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 from ..shared import errorsenum as shared_errorsenum
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ErrorResponse:
     r"""Error"""
+    
     details: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('details'), 'exclude': lambda f: f is None }})
     error_code: Optional[shared_errorsenum.ErrorsEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorCode'), 'exclude': lambda f: f is None }})
     error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/expandeddebithold.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/expandeddebithold.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,23 @@
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ExpandedDebitHold:
+    
     description: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description') }})
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     r"""The unique ID of the hold."""
     metadata: dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata') }})
     r"""Metadata associated with the hold."""
     original_amount: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('originalAmount') }})
     r"""Original amount on hold"""
     remaining: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('remaining') }})
     r"""Remaining amount on hold"""
     wallet_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('walletID') }})
     r"""The ID of the wallet the hold is associated with."""
     destination: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destination'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/getbalanceresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/getbalanceresponse.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,13 @@
 import dataclasses
 from ..shared import balancewithassets as shared_balancewithassets
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class GetBalanceResponse:
     r"""Balance summary"""
-    data: shared_balancewithassets.BalanceWithAssets = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     
-
+    data: shared_balancewithassets.BalanceWithAssets = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/getholdresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/getholdresponse.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,13 @@
 import dataclasses
 from ..shared import expandeddebithold as shared_expandeddebithold
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class GetHoldResponse:
     r"""Holds"""
-    data: shared_expandeddebithold.ExpandedDebitHold = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     
-
+    data: shared_expandeddebithold.ExpandedDebitHold = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/getholdsresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/listbalancesresponse.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import hold as shared_hold
+from ..shared import balance as shared_balance
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetHoldsResponseCursor:
-    data: list[shared_hold.Hold] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+class ListBalancesResponseCursor:
+    
+    data: list[shared_balance.Balance] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
     has_more: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasMore'), 'exclude': lambda f: f is None }})
     next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
     previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetHoldsResponse:
-    r"""Holds"""
-    cursor: GetHoldsResponseCursor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor') }})
+class ListBalancesResponse:
+    r"""Balances list"""
     
-
+    cursor: ListBalancesResponseCursor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/gettransactionsresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/gettransactionsresponse.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,27 +5,24 @@
 from ..shared import walletstransaction as shared_walletstransaction
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class GetTransactionsResponseCursor:
+    
     data: list[shared_walletstransaction.WalletsTransaction] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
     has_more: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasMore'), 'exclude': lambda f: f is None }})
     next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
     previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class GetTransactionsResponse:
     r"""OK"""
-    cursor: GetTransactionsResponseCursor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor') }})
     
-
+    cursor: GetTransactionsResponseCursor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/getversionsresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/getversionsresponse.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import dataclasses
 from ..shared import version as shared_version
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class GetVersionsResponse:
     r"""OK"""
+    
     env: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('env') }})
     region: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('region') }})
     versions: list[shared_version.Version] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('versions') }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/getwalletresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/getwalletresponse.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,13 @@
 import dataclasses
 from ..shared import walletwithbalances as shared_walletwithbalances
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class GetWalletResponse:
     r"""Wallet"""
-    data: shared_walletwithbalances.WalletWithBalances = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     
-
+    data: shared_walletwithbalances.WalletWithBalances = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/getwalletsummaryresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/getwalletsummaryresponse.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,18 +4,17 @@
 import dataclasses
 from ..shared import balancewithassets as shared_balancewithassets
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class GetWalletSummaryResponse:
     r"""Wallet summary"""
+    
     available_funds: dict[str, int] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('availableFunds') }})
     balances: list[shared_balancewithassets.BalanceWithAssets] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balances') }})
     expirable_funds: dict[str, int] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expirableFunds') }})
     expired_funds: dict[str, int] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expiredFunds') }})
     hold_funds: dict[str, int] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('holdFunds') }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/getworkflowinstancehistoryresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/getworkflowinstancehistoryresponse.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,13 @@
 import dataclasses
 from ..shared import workflowinstancehistory as shared_workflowinstancehistory
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class GetWorkflowInstanceHistoryResponse:
     r"""The workflow instance history"""
-    data: list[shared_workflowinstancehistory.WorkflowInstanceHistory] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     
-
+    data: list[shared_workflowinstancehistory.WorkflowInstanceHistory] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/getworkflowinstancehistorystageresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/getworkflowinstancehistorystageresponse.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,13 @@
 import dataclasses
 from ..shared import workflowinstancehistorystage as shared_workflowinstancehistorystage
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class GetWorkflowInstanceHistoryStageResponse:
     r"""The workflow instance stage history"""
-    data: list[shared_workflowinstancehistorystage.WorkflowInstanceHistoryStage] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     
-
+    data: list[shared_workflowinstancehistorystage.WorkflowInstanceHistoryStage] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/getworkflowinstanceresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/getworkflowinstanceresponse.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,13 @@
 import dataclasses
 from ..shared import workflowinstance as shared_workflowinstance
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class GetWorkflowInstanceResponse:
     r"""The workflow instance"""
-    data: shared_workflowinstance.WorkflowInstance = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     
-
+    data: shared_workflowinstance.WorkflowInstance = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/getworkflowresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/getworkflowresponse.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,13 @@
 import dataclasses
 from ..shared import workflow as shared_workflow
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class GetWorkflowResponse:
     r"""The workflow"""
-    data: shared_workflow.Workflow = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     
-
+    data: shared_workflow.Workflow = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/hold.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/hold.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,20 +4,19 @@
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class Hold:
+    
     description: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description') }})
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     r"""The unique ID of the hold."""
     metadata: dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata') }})
     r"""Metadata associated with the hold."""
     wallet_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('walletID') }})
     r"""The ID of the wallet the hold is associated with."""
     destination: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destination'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/ledgeraccountsubject.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/walletsubject.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
+from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class LedgerAccountSubject:
+class WalletSubject:
+    
     identifier: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('identifier') }})
     type: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-    
-
+    balance: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balance'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/ledgerinfo.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/ledgerinfo.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,23 +5,20 @@
 from ..shared import migrationinfo as shared_migrationinfo
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class LedgerInfoStorage:
+    
     migrations: Optional[list[shared_migrationinfo.MigrationInfo]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('migrations'), 'exclude': lambda f: f is None }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class LedgerInfo:
+    
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
     storage: Optional[LedgerInfoStorage] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('storage'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/ledgerinforesponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/listclientsresponse.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import ledgerinfo as shared_ledgerinfo
+from ..shared import client as shared_client
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class LedgerInfoResponse:
-    r"""OK"""
-    data: Optional[shared_ledgerinfo.LedgerInfo] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+class ListClientsResponse:
+    r"""List of clients"""
     
-
+    data: Optional[list[shared_client.Client]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/ledgerstorage.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/modulrconfig.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
+from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class LedgerStorage:
-    driver: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('driver') }})
-    ledgers: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ledgers') }})
+class ModulrConfig:
     
-
+    api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('apiKey') }})
+    api_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('apiSecret') }})
+    endpoint: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endpoint'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/listbalancesresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/accountscursorresponse.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import balance as shared_balance
+from ..shared import account as shared_account
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class ListBalancesResponseCursor:
-    data: list[shared_balance.Balance] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+class AccountsCursorResponseCursor:
+    
+    data: list[shared_account.Account] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+    has_more: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasMore') }})
     page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
-    has_more: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasMore'), 'exclude': lambda f: f is None }})
     next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
     previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class ListBalancesResponse:
-    r"""Balances list"""
-    cursor: ListBalancesResponseCursor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor') }})
+class AccountsCursorResponse:
+    r"""OK"""
     
-
+    cursor: AccountsCursorResponseCursor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/listclientsresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/mappingresponse.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import client as shared_client
+from ..shared import mapping as shared_mapping
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class ListClientsResponse:
-    r"""List of clients"""
-    data: Optional[list[shared_client.Client]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+class MappingResponse:
+    r"""OK"""
     
-
+    data: Optional[shared_mapping.Mapping] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/listrunsresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/listworkflowsresponse.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import workflowinstance as shared_workflowinstance
+from ..shared import workflow as shared_workflow
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class ListRunsResponse:
-    r"""List of workflow instances"""
-    data: list[shared_workflowinstance.WorkflowInstance] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+class ListWorkflowsResponse:
+    r"""List of workflows"""
     
-
+    data: list[shared_workflow.Workflow] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/listscopesresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/listscopesresponse.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,13 @@
 from ..shared import scope as shared_scope
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ListScopesResponse:
     r"""List of scopes"""
-    data: Optional[list[shared_scope.Scope]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
     
-
+    data: Optional[list[shared_scope.Scope]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/listusersresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/listusersresponse.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,13 @@
 from ..shared import user as shared_user
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ListUsersResponse:
     r"""List of users"""
-    data: Optional[list[shared_user.User]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
     
-
+    data: Optional[list[shared_user.User]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/listwalletsresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/listwalletsresponse.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,27 +5,24 @@
 from ..shared import wallet as shared_wallet
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ListWalletsResponseCursor:
+    
     data: list[shared_wallet.Wallet] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
     has_more: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasMore'), 'exclude': lambda f: f is None }})
     next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
     previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ListWalletsResponse:
     r"""OK"""
-    cursor: ListWalletsResponseCursor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor') }})
     
-
+    cursor: ListWalletsResponseCursor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/listworkflowsresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/transactionsresponse.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import workflow as shared_workflow
+from ..shared import transaction as shared_transaction
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class ListWorkflowsResponse:
-    r"""List of workflows"""
-    data: list[shared_workflow.Workflow] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+class TransactionsResponse:
+    r"""OK"""
     
-
+    data: list[shared_transaction.Transaction] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/log.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/log.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,30 +4,24 @@
 import dataclasses
 import dateutil.parser
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from marshmallow import fields
 from sdk import utils
-
-
-
-@dataclasses.dataclass
-class LogData:
-    pass
+from typing import Any
 
 class LogType(str, Enum):
     NEW_TRANSACTION = 'NEW_TRANSACTION'
     SET_METADATA = 'SET_METADATA'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class Log:
-    data: LogData = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+    
+    data: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     date_: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
     hash: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hash') }})
     id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     type: LogType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/logscursorresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/transactionscursorresponse.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import log as shared_log
+from ..shared import transaction as shared_transaction
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class LogsCursorResponseCursor:
-    data: list[shared_log.Log] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+class TransactionsCursorResponseCursor:
+    
+    data: list[shared_transaction.Transaction] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     has_more: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasMore') }})
     page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
     next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
     previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class LogsCursorResponse:
+class TransactionsCursorResponse:
     r"""OK"""
-    cursor: LogsCursorResponseCursor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor') }})
     
-
+    cursor: TransactionsCursorResponseCursor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/mappingresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/readuserresponse.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import mapping as shared_mapping
+from ..shared import user as shared_user
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class MappingResponse:
-    r"""OK"""
-    data: Optional[shared_mapping.Mapping] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+class ReadUserResponse:
+    r"""Retrieved user"""
     
-
+    data: Optional[shared_user.User] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/migrationinfo.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/migrationinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 
 class MigrationInfoState(str, Enum):
     TO_DO = 'to do'
     DONE = 'done'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class MigrationInfo:
+    
     date_: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('date'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
     state: Optional[MigrationInfoState] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state'), 'exclude': lambda f: f is None }})
     version: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('version'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/modulrconfig.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesenddestinationaccount.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,13 @@
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class ModulrConfig:
-    api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('apiKey') }})
-    api_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('apiSecret') }})
-    endpoint: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endpoint'), 'exclude': lambda f: f is None }})
+class StageSendDestinationAccount:
     
-
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    ledger: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ledger'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/monetary.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/monetary.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class Monetary:
+    
     amount: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount') }})
     r"""The amount of the monetary value."""
     asset: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('asset') }})
     r"""The asset of the monetary value."""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/payment.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/payment.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,15 @@
 from ..shared import paymentmetadata as shared_paymentmetadata
 from ..shared import paymentstatus as shared_paymentstatus
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from marshmallow import fields
 from sdk import utils
-
-
-
-@dataclasses.dataclass
-class PaymentRaw:
-    pass
+from typing import Any
 
 class PaymentScheme(str, Enum):
     VISA = 'visa'
     MASTERCARD = 'mastercard'
     AMEX = 'amex'
     DINERS = 'diners'
     DISCOVER = 'discover'
@@ -43,25 +38,24 @@
     PAY_IN = 'PAY-IN'
     PAYOUT = 'PAYOUT'
     TRANSFER = 'TRANSFER'
     OTHER = 'OTHER'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class Payment:
+    
     account_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountID') }})
     adjustments: list[shared_paymentadjustment.PaymentAdjustment] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('adjustments') }})
     asset: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('asset') }})
     created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     initial_amount: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('initialAmount') }})
     metadata: shared_paymentmetadata.PaymentMetadata = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata') }})
     provider: shared_connector.Connector = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('provider') }})
-    raw: PaymentRaw = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('raw') }})
+    raw: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('raw') }})
     reference: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference') }})
     scheme: PaymentScheme = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('scheme') }})
     status: shared_paymentstatus.PaymentStatus = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
     type: PaymentType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/paymentadjustment.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/paymentscursor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-from ..shared import paymentstatus as shared_paymentstatus
+from ..shared import payment as shared_payment
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from marshmallow import fields
 from sdk import utils
+from typing import Optional
 
 
-
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PaymentAdjustmentRaw:
-    pass
-
+class PaymentsCursorCursor:
+    
+    data: list[shared_payment.Payment] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+    has_more: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasMore') }})
+    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
+    next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
+    previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PaymentAdjustment:
-    absolute: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('absolute') }})
-    amount: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount') }})
-    date_: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    raw: PaymentAdjustmentRaw = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('raw') }})
-    status: shared_paymentstatus.PaymentStatus = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
+class PaymentsCursor:
+    r"""OK"""
     
-
+    cursor: PaymentsCursorCursor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/paymentsaccount.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/paymentsaccount.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,16 @@
 
 class PaymentsAccountType(str, Enum):
     TARGET = 'TARGET'
     SOURCE = 'SOURCE'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class PaymentsAccount:
+    
     created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     provider: shared_connector.Connector = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('provider') }})
     reference: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference') }})
     type: PaymentsAccountType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/paymentscursor.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/script.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,19 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import payment as shared_payment
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
-from typing import Optional
+from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PaymentsCursorCursor:
-    data: list[shared_payment.Payment] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
-    has_more: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasMore') }})
-    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
-    next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
-    previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
+class Script:
     
-
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-
-@dataclasses.dataclass
-class PaymentsCursor:
-    r"""OK"""
-    cursor: PaymentsCursorCursor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor') }})
-    
-
+    plain: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('plain') }})
+    metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
+    reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})
+    r"""Reference to attach to the generated transaction"""
+    vars: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('vars'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/posting.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/version.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class Posting:
-    amount: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount') }})
-    asset: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('asset') }})
-    destination: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destination') }})
-    source: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('source') }})
+class Version:
     
-
+    health: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('health') }})
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    version: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('version') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/posttransaction.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/posttransaction.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,38 +7,29 @@
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from marshmallow import fields
 from sdk import utils
 from typing import Any, Optional
 
 
-
-@dataclasses.dataclass
-class PostTransactionScriptVars:
-    pass
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class PostTransactionScript:
+    
     plain: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('plain') }})
-    vars: Optional[PostTransactionScriptVars] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('vars'), 'exclude': lambda f: f is None }})
+    vars: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('vars'), 'exclude': lambda f: f is None }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class PostTransaction:
     r"""The request body must contain at least one of the following objects:
       - `postings`: suitable for simple transactions
       - `script`: enabling more complex transactions with Numscript
     """
+    
     metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     postings: Optional[list[shared_posting.Posting]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postings'), 'exclude': lambda f: f is None }})
     reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})
     script: Optional[PostTransactionScript] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('script'), 'exclude': lambda f: f is None }})
     timestamp: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timestamp'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/query.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
-from typing import Optional
-
-
-
-@dataclasses.dataclass
-class QueryRaw:
-    pass
+from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class Query:
+    
     after: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('after'), 'exclude': lambda f: f is None }})
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor'), 'exclude': lambda f: f is None }})
     ledgers: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ledgers'), 'exclude': lambda f: f is None }})
     page_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize'), 'exclude': lambda f: f is None }})
     policy: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('policy'), 'exclude': lambda f: f is None }})
-    raw: Optional[QueryRaw] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('raw'), 'exclude': lambda f: f is None }})
+    raw: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('raw'), 'exclude': lambda f: f is None }})
     sort: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sort'), 'exclude': lambda f: f is None }})
     target: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('target'), 'exclude': lambda f: f is None }})
     terms: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('terms'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/readclientresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/readclientresponse.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,13 @@
 from ..shared import client as shared_client
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ReadClientResponse:
     r"""Retrieved client"""
-    data: Optional[shared_client.Client] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
     
-
+    data: Optional[shared_client.Client] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/readscoperesponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/updatescoperesponse.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,13 @@
 from ..shared import scope as shared_scope
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class ReadScopeResponse:
-    r"""Retrieved scope"""
-    data: Optional[shared_scope.Scope] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+class UpdateScopeResponse:
+    r"""Updated scope"""
     
-
+    data: Optional[shared_scope.Scope] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/readuserresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/ledgerinforesponse.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import user as shared_user
+from ..shared import ledgerinfo as shared_ledgerinfo
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class ReadUserResponse:
-    r"""Retrieved user"""
-    data: Optional[shared_user.User] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+class LedgerInfoResponse:
+    r"""OK"""
     
-
+    data: Optional[shared_ledgerinfo.LedgerInfo] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/response.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,57 +1,38 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
-from typing import Optional
-
-
-
-@dataclasses.dataclass
-class ResponseCursorData:
-    pass
+from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ResponseCursorTotal:
+    
     relation: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('relation'), 'exclude': lambda f: f is None }})
     value: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value'), 'exclude': lambda f: f is None }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ResponseCursor:
-    data: Optional[list[ResponseCursorData]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+    
+    data: Optional[list[dict[str, Any]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
     has_more: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasMore'), 'exclude': lambda f: f is None }})
     next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
     page_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize'), 'exclude': lambda f: f is None }})
     previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
     total: Optional[ResponseCursorTotal] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('total'), 'exclude': lambda f: f is None }})
     
 
-
-
-
-@dataclasses.dataclass
-class ResponseData:
-    r"""The payload"""
-    
-
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class Response:
     r"""Success"""
+    
     cursor: Optional[ResponseCursor] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor'), 'exclude': lambda f: f is None }})
-    data: Optional[ResponseData] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+    data: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
     r"""The payload"""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/runworkflowresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/runworkflowresponse.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,13 @@
 import dataclasses
 from ..shared import workflowinstance as shared_workflowinstance
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class RunWorkflowResponse:
     r"""The workflow instance"""
-    data: shared_workflowinstance.WorkflowInstance = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     
-
+    data: shared_workflowinstance.WorkflowInstance = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/scope.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/scope.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class Scope:
+    
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     label: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('label') }})
     metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     transient: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transient'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/script.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/paymentadjustment.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+import dateutil.parser
+from ..shared import paymentstatus as shared_paymentstatus
 from dataclasses_json import Undefined, dataclass_json
+from datetime import datetime
+from marshmallow import fields
 from sdk import utils
-from typing import Any, Optional
-
-
-
-@dataclasses.dataclass
-class ScriptVars:
-    pass
+from typing import Any
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class Script:
-    plain: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('plain') }})
-    metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
-    reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})
-    r"""Reference to attach to the generated transaction"""
-    vars: Optional[ScriptVars] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('vars'), 'exclude': lambda f: f is None }})
+class PaymentAdjustment:
     
-
+    absolute: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('absolute') }})
+    amount: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount') }})
+    date_: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    raw: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('raw') }})
+    status: shared_paymentstatus.PaymentStatus = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/scriptresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/scriptresponse.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,22 @@
 from ..shared import transaction as shared_transaction
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class ScriptResponse:
     r"""On success, it will return a 200 status code, and the resulting transaction under the `transaction` field.
-
+    
     On failure, it will also return a 200 status code, and the following fields:
       - `details`: contains a URL. When there is an error parsing Numscript, the result can be difficult to read—the provided URL will render the error in an easy-to-read format.
       - `errorCode` and `error_code` (deprecated): contains the string code of the error
       - `errorMessage` and `error_message` (deprecated): contains a human-readable indication of what went wrong, for example that an account had insufficient funds, or that there was an error in the provided Numscript.
     """
+    
     details: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('details'), 'exclude': lambda f: f is None }})
     error_code: Optional[shared_errorsenum.ErrorsEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorCode'), 'exclude': lambda f: f is None }})
     error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage'), 'exclude': lambda f: f is None }})
     transaction: Optional[shared_transaction.Transaction] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transaction'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/secret.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/secret.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class Secret:
+    
     clear: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('clear') }})
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     last_digits: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastDigits') }})
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
     metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/stagedelay.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagedelay.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,13 @@
 from datetime import datetime
 from marshmallow import fields
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class StageDelay:
+    
     duration: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
     until: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('until'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/stagesend.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesend.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from ..shared import stagesendsource as shared_stagesendsource
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class StageSend:
+    
     amount: Optional[shared_monetary.Monetary] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount'), 'exclude': lambda f: f is None }})
     destination: Optional[shared_stagesenddestination.StageSendDestination] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destination'), 'exclude': lambda f: f is None }})
     source: Optional[shared_stagesendsource.StageSendSource] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('source'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/stagesenddestination.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesenddestination.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from ..shared import stagesenddestinationwallet as shared_stagesenddestinationwallet
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class StageSendDestination:
+    
     account: Optional[shared_stagesenddestinationaccount.StageSendDestinationAccount] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account'), 'exclude': lambda f: f is None }})
     payment: Optional[shared_stagesenddestinationpayment.StageSendDestinationPayment] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('payment'), 'exclude': lambda f: f is None }})
     wallet: Optional[shared_stagesenddestinationwallet.StageSendDestinationWallet] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('wallet'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/stagesenddestinationaccount.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/ledgerstorage.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
-from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class StageSendDestinationAccount:
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    ledger: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ledger'), 'exclude': lambda f: f is None }})
+class LedgerStorage:
     
-
+    driver: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('driver') }})
+    ledgers: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ledgers') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/stagesenddestinationwallet.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesendsourcewallet.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,13 @@
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class StageSendDestinationWallet:
+class StageSendSourceWallet:
+    
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     balance: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balance'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/stagesendsource.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesendsource.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from ..shared import stagesendsourcewallet as shared_stagesendsourcewallet
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class StageSendSource:
+    
     account: Optional[shared_stagesendsourceaccount.StageSendSourceAccount] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account'), 'exclude': lambda f: f is None }})
     payment: Optional[shared_stagesendsourcepayment.StageSendSourcePayment] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('payment'), 'exclude': lambda f: f is None }})
     wallet: Optional[shared_stagesendsourcewallet.StageSendSourceWallet] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('wallet'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/stagesendsourceaccount.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/volume.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class StageSendSourceAccount:
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    ledger: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ledger'), 'exclude': lambda f: f is None }})
+class Volume:
     
-
+    input: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('input') }})
+    output: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('output') }})
+    balance: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balance'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/stagesendsourcewallet.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/account.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
-from typing import Optional
+from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class StageSendSourceWallet:
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    balance: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balance'), 'exclude': lambda f: f is None }})
+class Account:
     
-
+    address: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address') }})
+    metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
+    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/stagestatus.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/workflowinstancehistory.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from marshmallow import fields
 from sdk import utils
-from typing import Optional
+from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class StageStatus:
-    instance_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('instanceID') }})
-    stage: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stage') }})
+class WorkflowInstanceHistory:
+    
+    input: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('input') }})
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
     started_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    terminated: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('terminated') }})
     error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
     terminated_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('terminatedAt'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/stats.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/updatescoperequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
+from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class Stats:
-    accounts: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts') }})
-    transactions: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transactions') }})
+class UpdateScopeRequest:
     
-
+    label: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('label') }})
+    metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/stripeconfig.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/stripeconfig.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class StripeConfig:
+    
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('apiKey') }})
     page_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize'), 'exclude': lambda f: f is None }})
     r"""Number of BalanceTransaction to fetch at each polling interval."""
     polling_period: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pollingPeriod'), 'exclude': lambda f: f is None }})
     r"""The frequency at which the connector will try to fetch new BalanceTransaction objects from Stripe API."""
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/stripetransferrequest.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/stripetransferrequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,21 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
-from typing import Optional
-
-
-
-@dataclasses.dataclass
-class StripeTransferRequestMetadata:
-    r"""A set of key/value pairs that you can attach to a transfer object.
-    It can be useful for storing additional information about the transfer in a structured format.
-    """
-    
-
+from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class StripeTransferRequest:
+    
     amount: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount'), 'exclude': lambda f: f is None }})
     asset: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('asset'), 'exclude': lambda f: f is None }})
     destination: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destination'), 'exclude': lambda f: f is None }})
-    metadata: Optional[StripeTransferRequestMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
+    metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     r"""A set of key/value pairs that you can attach to a transfer object.
     It can be useful for storing additional information about the transfer in a structured format.
     """
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/taskbankingcircle.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskbankingcircle.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,40 +4,31 @@
 import dataclasses
 import dateutil.parser
 from ..shared import paymentstatus as shared_paymentstatus
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from marshmallow import fields
 from sdk import utils
-from typing import Optional
+from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class TaskBankingCircleDescriptor:
+    
     key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key'), 'exclude': lambda f: f is None }})
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
     
 
-
-
-
-@dataclasses.dataclass
-class TaskBankingCircleState:
-    pass
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class TaskBankingCircle:
+    
     connector_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectorId') }})
     created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
     descriptor: TaskBankingCircleDescriptor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('descriptor') }})
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    state: TaskBankingCircleState = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state') }})
+    state: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state') }})
     status: shared_paymentstatus.PaymentStatus = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
     updated_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
     error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/taskcurrencycloud.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskcurrencycloud.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,39 +4,30 @@
 import dataclasses
 import dateutil.parser
 from ..shared import paymentstatus as shared_paymentstatus
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from marshmallow import fields
 from sdk import utils
-from typing import Optional
+from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class TaskCurrencyCloudDescriptor:
+    
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
     
 
-
-
-
-@dataclasses.dataclass
-class TaskCurrencyCloudState:
-    pass
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class TaskCurrencyCloud:
+    
     connector_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectorId') }})
     created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
     descriptor: TaskCurrencyCloudDescriptor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('descriptor') }})
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    state: TaskCurrencyCloudState = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state') }})
+    state: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state') }})
     status: shared_paymentstatus.PaymentStatus = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
     updated_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
     error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/taskdummypay.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskdummypay.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,41 +4,32 @@
 import dataclasses
 import dateutil.parser
 from ..shared import paymentstatus as shared_paymentstatus
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from marshmallow import fields
 from sdk import utils
-from typing import Optional
+from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class TaskDummyPayDescriptor:
+    
     file_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fileName'), 'exclude': lambda f: f is None }})
     key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key'), 'exclude': lambda f: f is None }})
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
     
 
-
-
-
-@dataclasses.dataclass
-class TaskDummyPayState:
-    pass
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class TaskDummyPay:
+    
     connector_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectorId') }})
     created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
     descriptor: TaskDummyPayDescriptor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('descriptor') }})
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    state: TaskDummyPayState = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state') }})
+    state: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state') }})
     status: shared_paymentstatus.PaymentStatus = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
     updated_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
     error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/taskmodulr.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskmodulr.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,41 +4,32 @@
 import dataclasses
 import dateutil.parser
 from ..shared import paymentstatus as shared_paymentstatus
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from marshmallow import fields
 from sdk import utils
-from typing import Optional
+from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class TaskModulrDescriptor:
+    
     account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountID'), 'exclude': lambda f: f is None }})
     key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key'), 'exclude': lambda f: f is None }})
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
     
 
-
-
-
-@dataclasses.dataclass
-class TaskModulrState:
-    pass
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class TaskModulr:
+    
     connector_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectorId') }})
     created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
     descriptor: TaskModulrDescriptor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('descriptor') }})
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    state: TaskModulrState = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state') }})
+    state: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state') }})
     status: shared_paymentstatus.PaymentStatus = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
     updated_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
     error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/taskscursor.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskscursor.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,24 @@
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class TasksCursorCursor:
+    
     data: list[Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     has_more: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasMore') }})
     page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
     next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
     previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class TasksCursor:
     r"""OK"""
-    cursor: TasksCursorCursor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor') }})
     
-
+    cursor: TasksCursorCursor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/taskstripe.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskwise.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,41 +4,32 @@
 import dataclasses
 import dateutil.parser
 from ..shared import paymentstatus as shared_paymentstatus
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from marshmallow import fields
 from sdk import utils
-from typing import Optional
+from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class TaskStripeDescriptor:
-    account: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account') }})
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    main: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('main'), 'exclude': lambda f: f is None }})
+class TaskWiseDescriptor:
+    
+    key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key'), 'exclude': lambda f: f is None }})
+    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    profile_id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('profileID'), 'exclude': lambda f: f is None }})
     
-
-
-
-
-@dataclasses.dataclass
-class TaskStripeState:
-    pass
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class TaskStripe:
+class TaskWise:
+    
     connector_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectorId') }})
     created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    descriptor: TaskStripeDescriptor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('descriptor') }})
+    descriptor: TaskWiseDescriptor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('descriptor') }})
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    state: TaskStripeState = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state') }})
+    state: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state') }})
     status: shared_paymentstatus.PaymentStatus = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
     updated_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
     error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/taskwise.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/taskstripe.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,41 +4,32 @@
 import dataclasses
 import dateutil.parser
 from ..shared import paymentstatus as shared_paymentstatus
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from marshmallow import fields
 from sdk import utils
-from typing import Optional
+from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class TaskWiseDescriptor:
-    key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    profile_id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('profileID'), 'exclude': lambda f: f is None }})
+class TaskStripeDescriptor:
+    
+    account: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account') }})
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    main: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('main'), 'exclude': lambda f: f is None }})
     
-
-
-
-
-@dataclasses.dataclass
-class TaskWiseState:
-    pass
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class TaskWise:
+class TaskStripe:
+    
     connector_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectorId') }})
     created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    descriptor: TaskWiseDescriptor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('descriptor') }})
+    descriptor: TaskStripeDescriptor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('descriptor') }})
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    state: TaskWiseState = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state') }})
+    state: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state') }})
     status: shared_paymentstatus.PaymentStatus = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
     updated_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
     error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/transaction.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/walletstransaction.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
 from ..shared import posting as shared_posting
-from ..shared import volume as shared_volume
+from ..shared import walletsvolume as shared_walletsvolume
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from marshmallow import fields
 from sdk import utils
-from typing import Any, Optional
+from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class Transaction:
+class WalletsTransaction:
+    
+    metadata: dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata') }})
+    r"""Metadata associated with the wallet."""
     postings: list[shared_posting.Posting] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postings') }})
     timestamp: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timestamp'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
     txid: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('txid') }})
-    metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
-    post_commit_volumes: Optional[dict[str, dict[str, shared_volume.Volume]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postCommitVolumes'), 'exclude': lambda f: f is None }})
-    pre_commit_volumes: Optional[dict[str, dict[str, shared_volume.Volume]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('preCommitVolumes'), 'exclude': lambda f: f is None }})
+    ledger: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ledger'), 'exclude': lambda f: f is None }})
+    post_commit_volumes: Optional[dict[str, dict[str, shared_walletsvolume.WalletsVolume]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postCommitVolumes'), 'exclude': lambda f: f is None }})
+    pre_commit_volumes: Optional[dict[str, dict[str, shared_walletsvolume.WalletsVolume]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('preCommitVolumes'), 'exclude': lambda f: f is None }})
     reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/transactiondata.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/transactiondata.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 from datetime import datetime
 from marshmallow import fields
 from sdk import utils
 from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class TransactionData:
+    
     postings: list[shared_posting.Posting] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postings') }})
     metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})
     timestamp: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timestamp'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/transactionresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/transactionresponse.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,13 @@
 import dataclasses
 from ..shared import transaction as shared_transaction
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class TransactionResponse:
     r"""OK"""
-    data: shared_transaction.Transaction = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     
-
+    data: shared_transaction.Transaction = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/transactions.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/transactions.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,13 +4,12 @@
 import dataclasses
 from ..shared import transactiondata as shared_transactiondata
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class Transactions:
-    transactions: list[shared_transactiondata.TransactionData] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transactions') }})
     
-
+    transactions: list[shared_transactiondata.TransactionData] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transactions') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/transactionscursorresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/webhookserrorresponse.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,19 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import transaction as shared_transaction
+from ..shared import webhookserrorsenum as shared_webhookserrorsenum
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class TransactionsCursorResponseCursor:
-    data: list[shared_transaction.Transaction] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
-    has_more: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasMore') }})
-    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
-    next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
-    previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
+class WebhooksErrorResponse:
+    r"""Error"""
     
-
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-
-@dataclasses.dataclass
-class TransactionsCursorResponse:
-    r"""OK"""
-    cursor: TransactionsCursorResponseCursor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor') }})
-    
-
+    error_code: shared_webhookserrorsenum.WebhooksErrorsEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorCode') }})
+    error_message: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage') }})
+    details: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('details'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/transactionsresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/updateclientresponse.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import transaction as shared_transaction
+from ..shared import client as shared_client
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
+from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class TransactionsResponse:
-    r"""OK"""
-    data: list[shared_transaction.Transaction] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+class UpdateClientResponse:
+    r"""Updated client"""
     
-
+    data: Optional[shared_client.Client] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/transferrequest.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/stats.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
-from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class TransferRequest:
-    amount: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount') }})
-    asset: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('asset') }})
-    destination: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destination') }})
-    source: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('source'), 'exclude': lambda f: f is None }})
+class Stats:
     
-
+    accounts: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts') }})
+    transactions: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transactions') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/transferresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/transferresponse.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,13 @@
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class TransferResponse:
     r"""OK"""
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     
-
+    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/transfersresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/transfersresponse.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,27 @@
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class TransfersResponseData:
+    
     amount: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount'), 'exclude': lambda f: f is None }})
     asset: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('asset'), 'exclude': lambda f: f is None }})
     currency: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency'), 'exclude': lambda f: f is None }})
     destination: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destination'), 'exclude': lambda f: f is None }})
     error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     source: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('source'), 'exclude': lambda f: f is None }})
     status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class TransfersResponse:
     r"""OK"""
-    data: Optional[list[TransfersResponseData]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
     
-
+    data: Optional[list[TransfersResponseData]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/updateclientrequest.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/createclientrequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class UpdateClientRequest:
+class CreateClientRequest:
+    
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
     description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
     metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     post_logout_redirect_uris: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postLogoutRedirectUris'), 'exclude': lambda f: f is None }})
     public: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('public'), 'exclude': lambda f: f is None }})
     redirect_uris: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('redirectUris'), 'exclude': lambda f: f is None }})
     trusted: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trusted'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/updatescoperequest.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/error.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
+from enum import Enum
 from sdk import utils
-from typing import Any, Optional
 
+class ErrorErrorCode(str, Enum):
+    VALIDATION = 'VALIDATION'
+    NOT_FOUND = 'NOT_FOUND'
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class UpdateScopeRequest:
-    label: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('label') }})
-    metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
+class Error:
+    r"""General error"""
     
-
+    error_code: ErrorErrorCode = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorCode') }})
+    error_message: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/updatescoperesponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/createscoperesponse.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,13 @@
 from ..shared import scope as shared_scope
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class UpdateScopeResponse:
-    r"""Updated scope"""
-    data: Optional[shared_scope.Scope] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+class CreateScopeResponse:
+    r"""Created scope"""
     
-
+    data: Optional[shared_scope.Scope] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/user.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class User:
+    
     email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/volume.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/stagesenddestinationwallet.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,13 @@
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class Volume:
-    input: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('input') }})
-    output: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('output') }})
-    balance: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balance'), 'exclude': lambda f: f is None }})
+class StageSendDestinationWallet:
     
-
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    balance: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balance'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/wallet.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/walletwithbalances.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
+from ..shared import assetholder as shared_assetholder
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from marshmallow import fields
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class WalletWithBalancesBalances:
+    
+    main: shared_assetholder.AssetHolder = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('main') }})
+    
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Wallet:
+class WalletWithBalances:
+    
+    balances: WalletWithBalancesBalances = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balances') }})
     created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     r"""The unique ID of the wallet."""
     ledger: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ledger') }})
     metadata: dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata') }})
     r"""Metadata associated with the wallet."""
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/walletserrorresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/contract.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
 from sdk import utils
-
-class WalletsErrorResponseErrorCode(str, Enum):
-    VALIDATION = 'VALIDATION'
+from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class WalletsErrorResponse:
-    r"""Error"""
-    error_code: WalletsErrorResponseErrorCode = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorCode') }})
-    error_message: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage') }})
+class Contract:
     
-
+    expr: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expr') }})
+    account: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/walletstransaction.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/workflowinstance.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
-from ..shared import posting as shared_posting
-from ..shared import walletsvolume as shared_walletsvolume
+from ..shared import stagestatus as shared_stagestatus
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from marshmallow import fields
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class WalletsTransaction:
-    metadata: dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata') }})
-    r"""Metadata associated with the wallet."""
-    postings: list[shared_posting.Posting] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postings') }})
-    timestamp: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timestamp'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    txid: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('txid') }})
-    ledger: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ledger'), 'exclude': lambda f: f is None }})
-    post_commit_volumes: Optional[dict[str, dict[str, shared_walletsvolume.WalletsVolume]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postCommitVolumes'), 'exclude': lambda f: f is None }})
-    pre_commit_volumes: Optional[dict[str, dict[str, shared_walletsvolume.WalletsVolume]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('preCommitVolumes'), 'exclude': lambda f: f is None }})
-    reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})
+class WorkflowInstance:
     
-
+    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    terminated: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('terminated') }})
+    updated_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    workflow_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workflowID') }})
+    error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
+    status: Optional[list[shared_stagestatus.StageStatus]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
+    terminated_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('terminatedAt'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/walletsubject.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/activityreverttransaction.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
-from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class WalletSubject:
-    identifier: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('identifier') }})
-    type: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-    balance: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balance'), 'exclude': lambda f: f is None }})
+class ActivityRevertTransaction:
     
-
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    ledger: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ledger') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/walletsvolume.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/walletsvolume.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class WalletsVolume:
+    
     balance: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balance') }})
     input: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('input') }})
     output: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('output') }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/walletwithbalances.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/transaction.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,26 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
-from ..shared import assetholder as shared_assetholder
+from ..shared import posting as shared_posting
+from ..shared import volume as shared_volume
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from marshmallow import fields
 from sdk import utils
+from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class WalletWithBalancesBalances:
-    main: shared_assetholder.AssetHolder = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('main') }})
+class Transaction:
     
-
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-
-@dataclasses.dataclass
-class WalletWithBalances:
-    balances: WalletWithBalancesBalances = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balances') }})
-    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""The unique ID of the wallet."""
-    ledger: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ledger') }})
-    metadata: dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata') }})
-    r"""Metadata associated with the wallet."""
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    
-
+    postings: list[shared_posting.Posting] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postings') }})
+    timestamp: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timestamp'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    txid: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('txid') }})
+    metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
+    post_commit_volumes: Optional[dict[str, dict[str, shared_volume.Volume]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postCommitVolumes'), 'exclude': lambda f: f is None }})
+    pre_commit_volumes: Optional[dict[str, dict[str, shared_volume.Volume]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('preCommitVolumes'), 'exclude': lambda f: f is None }})
+    reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/webhooksconfig.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/webhooksconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,18 @@
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from marshmallow import fields
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class WebhooksConfig:
+    
     active: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('active') }})
     created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
     endpoint: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endpoint') }})
     event_types: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventTypes') }})
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secret') }})
     updated_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/webhookserrorresponse.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/wallet.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import webhookserrorsenum as shared_webhookserrorsenum
+import dateutil.parser
 from dataclasses_json import Undefined, dataclass_json
+from datetime import datetime
+from marshmallow import fields
 from sdk import utils
-from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class WebhooksErrorResponse:
-    r"""Error"""
-    error_code: shared_webhookserrorsenum.WebhooksErrorsEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorCode') }})
-    error_message: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage') }})
-    details: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('details'), 'exclude': lambda f: f is None }})
+class Wallet:
     
-
+    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    r"""The unique ID of the wallet."""
+    ledger: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ledger') }})
+    metadata: dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata') }})
+    r"""Metadata associated with the wallet."""
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/workflow.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from marshmallow import fields
 from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class Workflow:
+    
     config: shared_workflowconfig.WorkflowConfig = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('config') }})
     created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     updated_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/workflowconfig.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/operations/addscopetoclient.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from dataclasses_json import Undefined, dataclass_json
-from sdk import utils
-from typing import Any, Optional
+import requests as requests_http
+from typing import Optional
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class WorkflowConfig:
-    stages: list[dict[str, Any]] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stages') }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+class AddScopeToClientRequest:
+    
+    client_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'clientId', 'style': 'simple', 'explode': False }})
+    r"""Client ID"""
+    scope_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'scopeId', 'style': 'simple', 'explode': False }})
+    r"""Scope ID"""
     
 
+@dataclasses.dataclass
+class AddScopeToClientResponse:
+    
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/workflowinstance.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/workflowinstancehistorystageoutput.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-from ..shared import stagestatus as shared_stagestatus
+from ..shared import activitycreatetransactionoutput as shared_activitycreatetransactionoutput
+from ..shared import activitydebitwalletoutput as shared_activitydebitwalletoutput
+from ..shared import activitygetaccountoutput as shared_activitygetaccountoutput
+from ..shared import activitygetpaymentoutput as shared_activitygetpaymentoutput
+from ..shared import activitygetwalletoutput as shared_activitygetwalletoutput
+from ..shared import activityreverttransactionoutput as shared_activityreverttransactionoutput
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from marshmallow import fields
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class WorkflowInstance:
-    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    terminated: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('terminated') }})
-    updated_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    workflow_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workflowID') }})
-    error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
-    status: Optional[list[shared_stagestatus.StageStatus]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
-    terminated_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('terminatedAt'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+class WorkflowInstanceHistoryStageOutput:
     
-
+    create_transaction: Optional[shared_activitycreatetransactionoutput.ActivityCreateTransactionOutput] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('CreateTransaction'), 'exclude': lambda f: f is None }})
+    debit_wallet: Optional[shared_activitydebitwalletoutput.ActivityDebitWalletOutput] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('DebitWallet'), 'exclude': lambda f: f is None }})
+    get_account: Optional[shared_activitygetaccountoutput.ActivityGetAccountOutput] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('GetAccount'), 'exclude': lambda f: f is None }})
+    get_payment: Optional[shared_activitygetpaymentoutput.ActivityGetPaymentOutput] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('GetPayment'), 'exclude': lambda f: f is None }})
+    get_wallet: Optional[shared_activitygetwalletoutput.ActivityGetWalletOutput] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('GetWallet'), 'exclude': lambda f: f is None }})
+    revert_transaction: Optional[shared_activityreverttransactionoutput.ActivityRevertTransactionOutput] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('RevertTransaction'), 'exclude': lambda f: f is None }})
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/workflowinstancehistorystage.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/workflowinstancehistorystage.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,22 +9,21 @@
 from datetime import datetime
 from marshmallow import fields
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class WorkflowInstanceHistoryStage:
+    
     attempt: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('attempt') }})
     input: shared_workflowinstancehistorystageinput.WorkflowInstanceHistoryStageInput = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('input') }})
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
     started_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
     terminated: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('terminated') }})
     error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
     last_failure: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastFailure'), 'exclude': lambda f: f is None }})
     next_execution: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextExecution'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
     output: Optional[shared_workflowinstancehistorystageoutput.WorkflowInstanceHistoryStageOutput] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('output'), 'exclude': lambda f: f is None }})
     terminated_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('terminatedAt'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/models/shared/workflowinstancehistorystageinput.py` & `formance-sdk-python-1.0.20230718/src/sdk/models/shared/workflowinstancehistorystageinput.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,22 +14,21 @@
 from ..shared import activityvoidhold as shared_activityvoidhold
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class WorkflowInstanceHistoryStageInput:
+    
     confirm_hold: Optional[shared_activityconfirmhold.ActivityConfirmHold] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ConfirmHold'), 'exclude': lambda f: f is None }})
     create_transaction: Optional[shared_activitycreatetransaction.ActivityCreateTransaction] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('CreateTransaction'), 'exclude': lambda f: f is None }})
     credit_wallet: Optional[shared_activitycreditwallet.ActivityCreditWallet] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('CreditWallet'), 'exclude': lambda f: f is None }})
     debit_wallet: Optional[shared_activitydebitwallet.ActivityDebitWallet] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('DebitWallet'), 'exclude': lambda f: f is None }})
     get_account: Optional[shared_activitygetaccount.ActivityGetAccount] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('GetAccount'), 'exclude': lambda f: f is None }})
     get_payment: Optional[shared_activitygetpayment.ActivityGetPayment] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('GetPayment'), 'exclude': lambda f: f is None }})
     get_wallet: Optional[shared_activitygetwallet.ActivityGetWallet] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('GetWallet'), 'exclude': lambda f: f is None }})
     revert_transaction: Optional[shared_activityreverttransaction.ActivityRevertTransaction] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('RevertTransaction'), 'exclude': lambda f: f is None }})
     stripe_transfer: Optional[shared_activitystripetransfer.ActivityStripeTransfer] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('StripeTransfer'), 'exclude': lambda f: f is None }})
     void_hold: Optional[shared_activityvoidhold.ActivityVoidHold] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('VoidHold'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/payments.py` & `formance-sdk-python-1.0.20230718/src/sdk/payments.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,79 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-from .sdkconfiguration import SDKConfiguration
-from sdk import utils
+import requests as requests_http
+from . import utils
 from sdk.models import operations, shared
-from typing import Optional
+from typing import Any, Optional
 
 class Payments:
-    sdk_configuration: SDKConfiguration
-
-    def __init__(self, sdk_config: SDKConfiguration) -> None:
-        self.sdk_configuration = sdk_config
+    _client: requests_http.Session
+    _security_client: requests_http.Session
+    _server_url: str
+    _language: str
+    _sdk_version: str
+    _gen_version: str
+
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+        self._client = client
+        self._security_client = security_client
+        self._server_url = server_url
+        self._language = language
+        self._sdk_version = sdk_version
+        self._gen_version = gen_version
         
     
     def connectors_stripe_transfer(self, request: shared.StripeTransferRequest) -> operations.ConnectorsStripeTransferResponse:
         r"""Transfer funds between Stripe accounts
         Execute a transfer between two Stripe accounts.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
-        url = base_url + '/api/payments/connectors/stripe/transfers'
+        url = base_url.removesuffix('/') + '/api/payments/connectors/stripe/transfers'
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ConnectorsStripeTransferResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.StripeTransferResponse])
+                out = utils.unmarshal_json(http_res.text, Optional[dict[str, Any]])
                 res.stripe_transfer_response = out
 
         return res
 
     
     def connectors_transfer(self, request: operations.ConnectorsTransferRequest) -> operations.ConnectorsTransferResponse:
         r"""Transfer funds between Connector accounts
         Execute a transfer between two accounts.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.ConnectorsTransferRequest, base_url, '/api/payments/connectors/{connector}/transfers', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "transfer_request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ConnectorsTransferResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -74,22 +84,22 @@
         return res
 
     
     def get_connector_task(self, request: operations.GetConnectorTaskRequest) -> operations.GetConnectorTaskResponse:
         r"""Read a specific task of the connector
         Get a specific task associated to the connector.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.GetConnectorTaskRequest, base_url, '/api/payments/connectors/{connector}/tasks/{taskId}', request)
         headers = {}
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetConnectorTaskResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -98,22 +108,22 @@
                 res.task_response = out
 
         return res
 
     
     def get_payment(self, request: operations.GetPaymentRequest) -> operations.GetPaymentResponse:
         r"""Get a payment"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.GetPaymentRequest, base_url, '/api/payments/payments/{paymentId}', request)
         headers = {}
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetPaymentResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -124,49 +134,49 @@
         return res
 
     
     def install_connector(self, request: operations.InstallConnectorRequest) -> operations.InstallConnectorResponse:
         r"""Install a connector
         Install a connector by its name and config.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.InstallConnectorRequest, base_url, '/api/payments/connectors/{connector}', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = '*/*'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.InstallConnectorResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
 
         return res
 
     
     def list_all_connectors(self) -> operations.ListAllConnectorsResponse:
         r"""List all installed connectors
         List all installed connectors.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
-        url = base_url + '/api/payments/connectors'
+        url = base_url.removesuffix('/') + '/api/payments/connectors'
         headers = {}
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListAllConnectorsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -177,22 +187,22 @@
         return res
 
     
     def list_configs_available_connectors(self) -> operations.ListConfigsAvailableConnectorsResponse:
         r"""List the configs of each available connector
         List the configs of each available connector.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
-        url = base_url + '/api/payments/connectors/configs'
+        url = base_url.removesuffix('/') + '/api/payments/connectors/configs'
         headers = {}
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListConfigsAvailableConnectorsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -203,23 +213,23 @@
         return res
 
     
     def list_connector_tasks(self, request: operations.ListConnectorTasksRequest) -> operations.ListConnectorTasksResponse:
         r"""List tasks from a connector
         List all tasks associated with this connector.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.ListConnectorTasksRequest, base_url, '/api/payments/connectors/{connector}/tasks', request)
         headers = {}
         query_params = utils.get_query_params(operations.ListConnectorTasksRequest, request)
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, params=query_params, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListConnectorTasksResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -230,22 +240,22 @@
         return res
 
     
     def list_connectors_transfers(self, request: operations.ListConnectorsTransfersRequest) -> operations.ListConnectorsTransfersResponse:
         r"""List transfers and their statuses
         List transfers
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.ListConnectorsTransfersRequest, base_url, '/api/payments/connectors/{connector}/transfers', request)
         headers = {}
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListConnectorsTransfersResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -254,23 +264,23 @@
                 res.transfers_response = out
 
         return res
 
     
     def list_payments(self, request: operations.ListPaymentsRequest) -> operations.ListPaymentsResponse:
         r"""List payments"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
-        url = base_url + '/api/payments/payments'
+        url = base_url.removesuffix('/') + '/api/payments/payments'
         headers = {}
         query_params = utils.get_query_params(operations.ListPaymentsRequest, request)
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, params=query_params, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListPaymentsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -279,22 +289,22 @@
                 res.payments_cursor = out
 
         return res
 
     
     def paymentsget_server_info(self) -> operations.PaymentsgetServerInfoResponse:
         r"""Get server info"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
-        url = base_url + '/api/payments/_info'
+        url = base_url.removesuffix('/') + '/api/payments/_info'
         headers = {}
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.PaymentsgetServerInfoResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -303,23 +313,23 @@
                 res.server_info = out
 
         return res
 
     
     def paymentslist_accounts(self, request: operations.PaymentslistAccountsRequest) -> operations.PaymentslistAccountsResponse:
         r"""List accounts"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
-        url = base_url + '/api/payments/accounts'
+        url = base_url.removesuffix('/') + '/api/payments/accounts'
         headers = {}
         query_params = utils.get_query_params(operations.PaymentslistAccountsRequest, request)
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, params=query_params, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.PaymentslistAccountsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -330,22 +340,22 @@
         return res
 
     
     def read_connector_config(self, request: operations.ReadConnectorConfigRequest) -> operations.ReadConnectorConfigResponse:
         r"""Read the config of a connector
         Read connector config
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.ReadConnectorConfigRequest, base_url, '/api/payments/connectors/{connector}/config', request)
         headers = {}
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ReadConnectorConfigResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -357,69 +367,69 @@
 
     
     def reset_connector(self, request: operations.ResetConnectorRequest) -> operations.ResetConnectorResponse:
         r"""Reset a connector
         Reset a connector by its name.
         It will remove the connector and ALL PAYMENTS generated with it.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.ResetConnectorRequest, base_url, '/api/payments/connectors/{connector}/reset', request)
         headers = {}
         headers['Accept'] = '*/*'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ResetConnectorResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
 
         return res
 
     
     def uninstall_connector(self, request: operations.UninstallConnectorRequest) -> operations.UninstallConnectorResponse:
         r"""Uninstall a connector
         Uninstall a connector by its name.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.UninstallConnectorRequest, base_url, '/api/payments/connectors/{connector}', request)
         headers = {}
         headers['Accept'] = '*/*'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('DELETE', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.UninstallConnectorResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
 
         return res
 
     
     def update_metadata(self, request: operations.UpdateMetadataRequest) -> operations.UpdateMetadataResponse:
         r"""Update metadata"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.UpdateMetadataRequest, base_url, '/api/payments/payments/{paymentId}/metadata', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "payment_metadata", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = '*/*'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.UpdateMetadataResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/search.py` & `formance-sdk-python-1.0.20230718/src/sdk/search.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-from .sdkconfiguration import SDKConfiguration
-from sdk import utils
+import requests as requests_http
+from . import utils
 from sdk.models import operations, shared
 from typing import Optional
 
 class Search:
-    sdk_configuration: SDKConfiguration
-
-    def __init__(self, sdk_config: SDKConfiguration) -> None:
-        self.sdk_configuration = sdk_config
+    _client: requests_http.Session
+    _security_client: requests_http.Session
+    _server_url: str
+    _language: str
+    _sdk_version: str
+    _gen_version: str
+
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+        self._client = client
+        self._security_client = security_client
+        self._server_url = server_url
+        self._language = language
+        self._sdk_version = sdk_version
+        self._gen_version = gen_version
         
     
     def search(self, request: shared.Query) -> operations.SearchResponse:
         r"""Search
         ElasticSearch query engine
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
-        url = base_url + '/api/search/'
+        url = base_url.removesuffix('/') + '/api/search/'
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.SearchResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -43,22 +53,22 @@
             pass
 
         return res
 
     
     def searchget_server_info(self) -> operations.SearchgetServerInfoResponse:
         r"""Get server info"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
-        url = base_url + '/api/search/_info'
+        url = base_url.removesuffix('/') + '/api/search/_info'
         headers = {}
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.SearchgetServerInfoResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/utils/retries.py` & `formance-sdk-python-1.0.20230718/src/sdk/utils/retries.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,16 @@
 
 
 class RetryConfig:
     strategy: str
     backoff: BackoffStrategy
     retry_connection_errors: bool
 
-    def __init__(self, strategy: str, backoff: BackoffStrategy, retry_connection_errors: bool):
+    def __init__(self, strategy: str, retry_connection_errors: bool):
         self.strategy = strategy
-        self.backoff = backoff
         self.retry_connection_errors = retry_connection_errors
 
 
 class Retries:
     config: RetryConfig
     status_codes: list[str]
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/utils/utils.py` & `formance-sdk-python-1.0.20230718/src/sdk/utils/utils.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/wallets.py` & `formance-sdk-python-1.0.20230718/src/sdk/wallets.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-from .sdkconfiguration import SDKConfiguration
-from sdk import utils
+import requests as requests_http
+from . import utils
 from sdk.models import operations, shared
 from typing import Optional
 
 class Wallets:
-    sdk_configuration: SDKConfiguration
-
-    def __init__(self, sdk_config: SDKConfiguration) -> None:
-        self.sdk_configuration = sdk_config
+    _client: requests_http.Session
+    _security_client: requests_http.Session
+    _server_url: str
+    _language: str
+    _sdk_version: str
+    _gen_version: str
+
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+        self._client = client
+        self._security_client = security_client
+        self._server_url = server_url
+        self._language = language
+        self._sdk_version = sdk_version
+        self._gen_version = gen_version
         
     
     def confirm_hold(self, request: operations.ConfirmHoldRequest) -> operations.ConfirmHoldResponse:
         r"""Confirm a hold"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.ConfirmHoldRequest, base_url, '/api/wallets/holds/{hold_id}/confirm', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "confirm_hold_request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ConfirmHoldResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 204:
@@ -39,25 +49,25 @@
                 res.wallets_error_response = out
 
         return res
 
     
     def create_balance(self, request: operations.CreateBalanceRequest) -> operations.CreateBalanceResponse:
         r"""Create a balance"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.CreateBalanceRequest, base_url, '/api/wallets/wallets/{id}/balances', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "create_balance_request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CreateBalanceResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 201:
@@ -70,25 +80,25 @@
                 res.wallets_error_response = out
 
         return res
 
     
     def create_wallet(self, request: shared.CreateWalletRequest) -> operations.CreateWalletResponse:
         r"""Create a new wallet"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
-        url = base_url + '/api/wallets/wallets'
+        url = base_url.removesuffix('/') + '/api/wallets/wallets'
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CreateWalletResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 201:
@@ -101,25 +111,25 @@
                 res.wallets_error_response = out
 
         return res
 
     
     def credit_wallet(self, request: operations.CreditWalletRequest) -> operations.CreditWalletResponse:
         r"""Credit a wallet"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.CreditWalletRequest, base_url, '/api/wallets/wallets/{id}/credit', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "credit_wallet_request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CreditWalletResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 204:
@@ -130,25 +140,25 @@
                 res.wallets_error_response = out
 
         return res
 
     
     def debit_wallet(self, request: operations.DebitWalletRequest) -> operations.DebitWalletResponse:
         r"""Debit a wallet"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.DebitWalletRequest, base_url, '/api/wallets/wallets/{id}/debit', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "debit_wallet_request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.DebitWalletResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 201:
@@ -163,22 +173,22 @@
                 res.wallets_error_response = out
 
         return res
 
     
     def get_balance(self, request: operations.GetBalanceRequest) -> operations.GetBalanceResponse:
         r"""Get detailed balance"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.GetBalanceRequest, base_url, '/api/wallets/wallets/{id}/balances/{balanceName}', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetBalanceResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -191,22 +201,22 @@
                 res.wallets_error_response = out
 
         return res
 
     
     def get_hold(self, request: operations.GetHoldRequest) -> operations.GetHoldResponse:
         r"""Get a hold"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.GetHoldRequest, base_url, '/api/wallets/holds/{holdID}', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetHoldResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -219,23 +229,23 @@
                 res.wallets_error_response = out
 
         return res
 
     
     def get_holds(self, request: operations.GetHoldsRequest) -> operations.GetHoldsResponse:
         r"""Get all holds for a wallet"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
-        url = base_url + '/api/wallets/holds'
+        url = base_url.removesuffix('/') + '/api/wallets/holds'
         headers = {}
         query_params = utils.get_query_params(operations.GetHoldsRequest, request)
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, params=query_params, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetHoldsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -247,23 +257,23 @@
                 out = utils.unmarshal_json(http_res.text, Optional[shared.WalletsErrorResponse])
                 res.wallets_error_response = out
 
         return res
 
     
     def get_transactions(self, request: operations.GetTransactionsRequest) -> operations.GetTransactionsResponse:
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
-        url = base_url + '/api/wallets/transactions'
+        url = base_url.removesuffix('/') + '/api/wallets/transactions'
         headers = {}
         query_params = utils.get_query_params(operations.GetTransactionsRequest, request)
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, params=query_params, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetTransactionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -276,22 +286,22 @@
                 res.wallets_error_response = out
 
         return res
 
     
     def get_wallet(self, request: operations.GetWalletRequest) -> operations.GetWalletResponse:
         r"""Get a wallet"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.GetWalletRequest, base_url, '/api/wallets/wallets/{id}', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetWalletResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -306,22 +316,22 @@
                 res.wallets_error_response = out
 
         return res
 
     
     def get_wallet_summary(self, request: operations.GetWalletSummaryRequest) -> operations.GetWalletSummaryResponse:
         r"""Get wallet summary"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.GetWalletSummaryRequest, base_url, '/api/wallets/wallets/{id}/summary', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetWalletSummaryResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -336,22 +346,22 @@
                 res.wallets_error_response = out
 
         return res
 
     
     def list_balances(self, request: operations.ListBalancesRequest) -> operations.ListBalancesResponse:
         r"""List balances of a wallet"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.ListBalancesRequest, base_url, '/api/wallets/wallets/{id}/balances', request)
         headers = {}
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListBalancesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -360,23 +370,23 @@
                 res.list_balances_response = out
 
         return res
 
     
     def list_wallets(self, request: operations.ListWalletsRequest) -> operations.ListWalletsResponse:
         r"""List all wallets"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
-        url = base_url + '/api/wallets/wallets'
+        url = base_url.removesuffix('/') + '/api/wallets/wallets'
         headers = {}
         query_params = utils.get_query_params(operations.ListWalletsRequest, request)
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, params=query_params, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListWalletsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -385,25 +395,25 @@
                 res.list_wallets_response = out
 
         return res
 
     
     def update_wallet(self, request: operations.UpdateWalletRequest) -> operations.UpdateWalletResponse:
         r"""Update a wallet"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.UpdateWalletRequest, base_url, '/api/wallets/wallets/{id}', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.UpdateWalletResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 204:
@@ -414,22 +424,22 @@
                 res.wallets_error_response = out
 
         return res
 
     
     def void_hold(self, request: operations.VoidHoldRequest) -> operations.VoidHoldResponse:
         r"""Cancel a hold"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.VoidHoldRequest, base_url, '/api/wallets/holds/{hold_id}/void', request)
         headers = {}
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.VoidHoldResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 204:
@@ -440,22 +450,22 @@
                 res.wallets_error_response = out
 
         return res
 
     
     def walletsget_server_info(self) -> operations.WalletsgetServerInfoResponse:
         r"""Get server info"""
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
-        url = base_url + '/api/wallets/_info'
+        url = base_url.removesuffix('/') + '/api/wallets/_info'
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.WalletsgetServerInfoResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
```

### Comparing `formance-sdk-python-1.0.20230714/src/sdk/webhooks.py` & `formance-sdk-python-1.0.20230718/src/sdk/webhooks.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-from .sdkconfiguration import SDKConfiguration
-from sdk import utils
+import requests as requests_http
+from . import utils
 from sdk.models import operations, shared
 from typing import Optional
 
 class Webhooks:
-    sdk_configuration: SDKConfiguration
-
-    def __init__(self, sdk_config: SDKConfiguration) -> None:
-        self.sdk_configuration = sdk_config
+    _client: requests_http.Session
+    _security_client: requests_http.Session
+    _server_url: str
+    _language: str
+    _sdk_version: str
+    _gen_version: str
+
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+        self._client = client
+        self._security_client = security_client
+        self._server_url = server_url
+        self._language = language
+        self._sdk_version = sdk_version
+        self._gen_version = gen_version
         
     
     def activate_config(self, request: operations.ActivateConfigRequest) -> operations.ActivateConfigResponse:
         r"""Activate one config
         Activate a webhooks config by ID, to start receiving webhooks to its endpoint.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.ActivateConfigRequest, base_url, '/api/webhooks/configs/{id}/activate', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('PUT', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ActivateConfigResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -41,29 +51,29 @@
 
         return res
 
     
     def change_config_secret(self, request: operations.ChangeConfigSecretRequest) -> operations.ChangeConfigSecretResponse:
         r"""Change the signing secret of a config
         Change the signing secret of the endpoint of a webhooks config.
-
+        
         If not passed or empty, a secret is automatically generated.
         The format is a random string of bytes of size 24, base64 encoded. (larger size after encoding)
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.ChangeConfigSecretRequest, base_url, '/api/webhooks/configs/{id}/secret/change', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "config_change_secret", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('PUT', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ChangeConfigSecretResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -78,22 +88,22 @@
         return res
 
     
     def deactivate_config(self, request: operations.DeactivateConfigRequest) -> operations.DeactivateConfigResponse:
         r"""Deactivate one config
         Deactivate a webhooks config by ID, to stop receiving webhooks to its endpoint.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.DeactivateConfigRequest, base_url, '/api/webhooks/configs/{id}/deactivate', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('PUT', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.DeactivateConfigResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -108,22 +118,22 @@
         return res
 
     
     def delete_config(self, request: operations.DeleteConfigRequest) -> operations.DeleteConfigResponse:
         r"""Delete one config
         Delete a webhooks config by ID.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.DeleteConfigRequest, base_url, '/api/webhooks/configs/{id}', request)
         headers = {}
         headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('DELETE', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.DeleteConfigResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -136,23 +146,23 @@
         return res
 
     
     def get_many_configs(self, request: operations.GetManyConfigsRequest) -> operations.GetManyConfigsResponse:
         r"""Get many configs
         Sorted by updated date descending
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
-        url = base_url + '/api/webhooks/configs'
+        url = base_url.removesuffix('/') + '/api/webhooks/configs'
         headers = {}
         query_params = utils.get_query_params(operations.GetManyConfigsRequest, request)
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, params=query_params, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetManyConfigsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -166,36 +176,36 @@
 
         return res
 
     
     def insert_config(self, request: shared.ConfigUser) -> operations.InsertConfigResponse:
         r"""Insert a new config
         Insert a new webhooks config.
-
+        
         The endpoint should be a valid https URL and be unique.
-
+        
         The secret is the endpoint's verification secret.
         If not passed or empty, a secret is automatically generated.
         The format is a random string of bytes of size 24, base64 encoded. (larger size after encoding)
-
+        
         All eventTypes are converted to lower-case when inserted.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
-        url = base_url + '/api/webhooks/configs'
+        url = base_url.removesuffix('/') + '/api/webhooks/configs'
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.InsertConfigResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
@@ -210,22 +220,22 @@
         return res
 
     
     def test_config(self, request: operations.TestConfigRequest) -> operations.TestConfigResponse:
         r"""Test one config
         Test a config by sending a webhook to its endpoint.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        base_url = self._server_url
         
         url = utils.generate_url(operations.TestConfigRequest, base_url, '/api/webhooks/configs/{id}/test', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('GET', url, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.TestConfigResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
```

