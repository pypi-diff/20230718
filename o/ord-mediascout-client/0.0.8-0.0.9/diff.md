# Comparing `tmp/ord_mediascout_client-0.0.8.tar.gz` & `tmp/ord_mediascout_client-0.0.9.tar.gz`

## Comparing `ord_mediascout_client-0.0.8.tar` & `ord_mediascout_client-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,36 @@
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/Pipfile
--rw-r--r--   0        0        0    50707 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/Pipfile.lock
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/setup.cfg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/setup.py
--rw-r--r--   0        0        0    36170 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/.idea/workspace.xml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/.pytest_cache/README.md
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/docs/track_api_changes.md
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/examples/create_client.py
--rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/src/ord_mediascout_client/__init__.py
--rw-r--r--   0        0        0    10601 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/src/ord_mediascout_client/client.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/src/ord_mediascout_client/config.py
--rw-r--r--   0        0        0    22925 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/src/ord_mediascout_client/models.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/tests/.env.example.env
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/tests/client_test.py
--rw-r--r--   0        0        0     6635 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/tests/contract_test.py
--rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/tests/creative_test.py
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/tests/invoice_test.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/tests/ping_test.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/tests/platform_test.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/LICENSE.txt
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/README.md
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/Pipfile
+-rw-r--r--   0        0        0    79753 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/Pipfile.lock
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/setup.cfg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/setup.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/.idea/OrdMediascoutClientAPI.iml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/.idea/misc.xml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/.idea/vcs.xml
+-rw-r--r--   0        0        0    38989 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/.idea/workspace.xml
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/docs/track_api_changes.md
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/examples/create_client.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/scripts/.env.example.env
+-rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/scripts/api_monitor.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/scripts/models_gen.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/scripts/notes.txt
+-rw-r--r--   0        0        0   237556 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/scripts/data/swagger.json
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/src/ord_mediascout_client/.env.example.env
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/src/ord_mediascout_client/__init__.py
+-rw-r--r--   0        0        0    11261 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/src/ord_mediascout_client/client.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/src/ord_mediascout_client/config.py
+-rw-r--r--   0        0        0    28213 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/src/ord_mediascout_client/models.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/tests/.env.example.env
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/tests/client_test.py
+-rw-r--r--   0        0        0     6635 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/tests/contract_test.py
+-rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/tests/creative_test.py
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/tests/invoice_test.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/tests/ping_test.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/tests/platform_test.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/tests/statistics_test.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/README.md
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 ord_mediascout_client-0.0.9/PKG-INFO
```

### Comparing `ord_mediascout_client-0.0.8/.pre-commit-config.yaml` & `ord_mediascout_client-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ord_mediascout_client-0.0.8/Pipfile.lock` & `ord_mediascout_client-0.0.9/Pipfile.lock`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9079034391534391%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'efbc10f11d56fd7292401a9f052ab2a8ced2a72f86d33b2b3eb93428c05d23d0'}}",*

 * * "'default'": "{'certifi': {'hashes': "*

 * *              "['sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7', "*

 * *              "'sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716'], "*

 * *              "'version': '==2023.5.7'}, 'requests': {'hashes': "*

 * *              "['sha256:10e94cc4f3121ee6da529d358cdaeaff2f1c409cd377dbc72b825852f2f7e294', "*

 * *         […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "2035c4dab180b4dc51ef8d18753d487a4e36437e7045b771c7fd43d758f399b8"
+            "sha256": "efbc10f11d56fd7292401a9f052ab2a8ced2a72f86d33b2b3eb93428c05d23d0"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.11"
         },
         "sources": [
             {
@@ -14,19 +14,19 @@
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.12.7"
+            "version": "==2023.5.7"
         },
         "charset-normalizer": {
             "hashes": [
                 "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
                 "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
                 "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
                 "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
@@ -185,46 +185,101 @@
                 "sha256:f5971a9226b701070a4bf2c38c89e5a3f0d64de8debda981d1db98583009122a"
             ],
             "index": "pypi",
             "version": "==1.0.0"
         },
         "requests": {
             "hashes": [
-                "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
-                "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
+                "sha256:10e94cc4f3121ee6da529d358cdaeaff2f1c409cd377dbc72b825852f2f7e294",
+                "sha256:239d7d4458afcb28a692cdd298d87542235f4ca8d36d03a15bfc128a6559a2f4"
             ],
             "index": "pypi",
-            "version": "==2.28.2"
+            "version": "==2.30.0"
         },
         "rich": {
             "hashes": [
-                "sha256:22b74cae0278fd5086ff44144d3813be1cedc9115bdfabbfefd86400cb88b20a",
-                "sha256:b5d573e13605423ec80bdd0cd5f8541f7844a0e71a13f74cf454ccb2f490708b"
+                "sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c",
+                "sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704"
             ],
             "index": "pypi",
-            "version": "==13.3.4"
+            "version": "==13.3.5"
         },
         "typing-extensions": {
             "hashes": [
                 "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb",
                 "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.5.0"
         },
         "urllib3": {
             "hashes": [
-                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
-                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
+                "sha256:61717a1095d7e155cdb737ac7bb2f4324a858a1e2e6466f6d03ff630ca68d3cc",
+                "sha256:d055c2f9d38dc53c808f6fdc8eab7360b6fdbbde02340ed25cfbcd817c62469e"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.15"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.0.2"
         }
     },
     "develop": {
+        "anyio": {
+            "hashes": [
+                "sha256:25ea0d673ae30af41a0c442f81cf3b38c7e79fdc7b60335a4c14e05eb0947421",
+                "sha256:fbbe32bd270d2a2ef3ed1c5d45041250284e31fc0a4df4a5a6071842051a51e3"
+            ],
+            "markers": "python_full_version >= '3.6.2'",
+            "version": "==3.6.2"
+        },
+        "argcomplete": {
+            "hashes": [
+                "sha256:b9ca96448e14fa459d7450a4ab5a22bbf9cee4ba7adddf03e65c398b5daeea28",
+                "sha256:e36fd646839933cbec7941c662ecb65338248667358dd3d968405a4506a60d9b"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==3.0.8"
+        },
+        "attrs": {
+            "hashes": [
+                "sha256:1f28b4522cdc2fb4256ac1a020c78acf9cba2c6b461ccd2c126f3aa8e8335d04",
+                "sha256:6279836d581513a26f1bf235f9acd333bc9115683f14f7e8fae46c98fc50e015"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==23.1.0"
+        },
+        "black": {
+            "hashes": [
+                "sha256:064101748afa12ad2291c2b91c960be28b817c0c7eaa35bec09cc63aa56493c5",
+                "sha256:0945e13506be58bf7db93ee5853243eb368ace1c08a24c65ce108986eac65915",
+                "sha256:11c410f71b876f961d1de77b9699ad19f939094c3a677323f43d7a29855fe326",
+                "sha256:1c7b8d606e728a41ea1ccbd7264677e494e87cf630e399262ced92d4a8dac940",
+                "sha256:1d06691f1eb8de91cd1b322f21e3bfc9efe0c7ca1f0e1eb1db44ea367dff656b",
+                "sha256:3238f2aacf827d18d26db07524e44741233ae09a584273aa059066d644ca7b30",
+                "sha256:32daa9783106c28815d05b724238e30718f34155653d4d6e125dc7daec8e260c",
+                "sha256:35d1381d7a22cc5b2be2f72c7dfdae4072a3336060635718cc7e1ede24221d6c",
+                "sha256:3a150542a204124ed00683f0db1f5cf1c2aaaa9cc3495b7a3b5976fb136090ab",
+                "sha256:48f9d345675bb7fbc3dd85821b12487e1b9a75242028adad0333ce36ed2a6d27",
+                "sha256:50cb33cac881766a5cd9913e10ff75b1e8eb71babf4c7104f2e9c52da1fb7de2",
+                "sha256:562bd3a70495facf56814293149e51aa1be9931567474993c7942ff7d3533961",
+                "sha256:67de8d0c209eb5b330cce2469503de11bca4085880d62f1628bd9972cc3366b9",
+                "sha256:6b39abdfb402002b8a7d030ccc85cf5afff64ee90fa4c5aebc531e3ad0175ddb",
+                "sha256:6f3c333ea1dd6771b2d3777482429864f8e258899f6ff05826c3a4fcc5ce3f70",
+                "sha256:714290490c18fb0126baa0fca0a54ee795f7502b44177e1ce7624ba1c00f2331",
+                "sha256:7c3eb7cea23904399866c55826b31c1f55bbcd3890ce22ff70466b907b6775c2",
+                "sha256:92c543f6854c28a3c7f39f4d9b7694f9a6eb9d3c5e2ece488c327b6e7ea9b266",
+                "sha256:a6f6886c9869d4daae2d1715ce34a19bbc4b95006d20ed785ca00fa03cba312d",
+                "sha256:a8a968125d0a6a404842fa1bf0b349a568634f856aa08ffaff40ae0dfa52e7c6",
+                "sha256:c7ab5790333c448903c4b721b59c0d80b11fe5e9803d8703e84dcb8da56fec1b",
+                "sha256:e114420bf26b90d4b9daa597351337762b63039752bdf72bf361364c1aa05925",
+                "sha256:e198cf27888ad6f4ff331ca1c48ffc038848ea9f031a3b40ba36aced7e22f2c8",
+                "sha256:ec751418022185b0c1bb7d7736e6933d40bbb14c14a0abcf9123d1b159f98dd4",
+                "sha256:f0bd2f4a58d6666500542b26354978218a9babcdc972722f4bf90779524515f3"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==23.3.0"
+        },
         "bleach": {
             "hashes": [
                 "sha256:1a1a85c1595e07d8db14c5f09f09e6433502c51c595970edc090551f0db99414",
                 "sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==6.0.0"
@@ -235,19 +290,19 @@
                 "sha256:d5b71264afdb5951d6704482aac78de887c80691c52b88a9ad195983ca2c9269"
             ],
             "index": "pypi",
             "version": "==0.10.0"
         },
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.12.7"
+            "version": "==2023.5.7"
         },
         "cffi": {
             "hashes": [
                 "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
                 "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
                 "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
                 "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
@@ -318,14 +373,22 @@
             "hashes": [
                 "sha256:c6a0883f3917a037485059700b9e75da2464e6c27051014ad85ba6aaa5884426",
                 "sha256:f5a830efb9ce7a445376bb66ec94c638a9787422f96264c98edc6bdeed8ab736"
             ],
             "markers": "python_full_version >= '3.6.1'",
             "version": "==3.3.1"
         },
+        "chardet": {
+            "hashes": [
+                "sha256:0d62712b956bc154f85fb0a266e2a3c5913c2967e00348701b32411d6def31e5",
+                "sha256:362777fb014af596ad31334fde1e8c327dfdb076e1960d1694662d46a6917ab9"
+            ],
+            "index": "pypi",
+            "version": "==5.1.0"
+        },
         "charset-normalizer": {
             "hashes": [
                 "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
                 "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
                 "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
                 "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
                 "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62",
@@ -399,14 +462,22 @@
                 "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
                 "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
                 "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
             ],
             "markers": "python_full_version >= '3.7.0'",
             "version": "==3.1.0"
         },
+        "click": {
+            "hashes": [
+                "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
+                "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==8.1.3"
+        },
         "cryptography": {
             "hashes": [
                 "sha256:05dc219433b14046c476f6f09d7636b92a1c3e5808b9a6536adf4932b3b2c440",
                 "sha256:0dcca15d3a19a66e63662dc8d30f8036b07be851a8680eda92d079868f106288",
                 "sha256:142bae539ef28a1c76794cca7f49729e7c54423f615cfd9b0b1fa90ebe53244b",
                 "sha256:3daf9b114213f8ba460b829a02896789751626a2a4e7a43a28ee77c04b5e4958",
                 "sha256:48f388d0d153350f378c7f7b41497a54ff1513c816bcbbcafe5b829e59b9ce5b",
@@ -424,69 +495,148 @@
                 "sha256:c33c0d32b8594fa647d2e01dbccc303478e16fdd7cf98652d5b3ed11aa5e5c99",
                 "sha256:cbaba590180cba88cb99a5f76f90808a624f18b169b90a4abb40c1fd8c19420e",
                 "sha256:d5a1bd0e9e2031465761dfa920c16b0065ad77321d8a8c1f5ee331021fda65e9"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==40.0.2"
         },
+        "datamodel-code-generator": {
+            "extras": [
+                "http"
+            ],
+            "hashes": [
+                "sha256:082c8c0f72b42953fb04bd4a4e76bbd7b1cd4c07f3000fbd019c9a196e2bdf6b",
+                "sha256:13ca59944d6aa347dd5f674f90f5d7f1004626a65ecade6c364b90c1a47ef499"
+            ],
+            "index": "pypi",
+            "version": "==0.19.0"
+        },
         "distlib": {
             "hashes": [
                 "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
                 "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
             "version": "==0.3.6"
         },
+        "dnspython": {
+            "hashes": [
+                "sha256:224e32b03eb46be70e12ef6d64e0be123a64e621ab4c0822ff6d450d52a540b9",
+                "sha256:89141536394f909066cabd112e3e1a37e4e654db00a25308b0f130bc3152eb46"
+            ],
+            "markers": "python_version >= '3.7' and python_version < '4.0'",
+            "version": "==2.3.0"
+        },
         "docutils": {
             "hashes": [
-                "sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6",
-                "sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc"
+                "sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6",
+                "sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.19"
+            "version": "==0.20.1"
+        },
+        "email-validator": {
+            "hashes": [
+                "sha256:1ff6e86044200c56ae23595695c54e9614f4a9551e0e393614f764860b3d7900",
+                "sha256:2466ba57cda361fb7309fd3d5a225723c788ca4bbad32a0ebd5373b99730285c"
+            ],
+            "version": "==2.0.0.post2"
         },
         "filelock": {
             "hashes": [
                 "sha256:ad98852315c2ab702aeb628412cbf7e95b7ce8c3bf9565670b4eaecf1db370a9",
                 "sha256:fc03ae43288c013d2ea83c8597001b1129db351aad9c57fe2409327916b8e718"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.12.0"
         },
+        "genson": {
+            "hashes": [
+                "sha256:8caf69aa10af7aee0e1a1351d1d06801f4696e005f06cedef438635384346a16"
+            ],
+            "version": "==1.2.2"
+        },
+        "h11": {
+            "hashes": [
+                "sha256:8f19fbbe99e72420ff35c00b27a34cb9937e902a8b810e2c88300c6f0a3b699d",
+                "sha256:e3fe4ac4b851c468cc8363d500db52c2ead036020723024a109d37346efaa761"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==0.14.0"
+        },
+        "httpcore": {
+            "hashes": [
+                "sha256:628e768aaeec1f7effdc6408ba1c3cdbd7487c1fc570f7d66844ec4f003e1ca4",
+                "sha256:caf508597c525f9b8bfff187e270666309f63115af30f7d68b16143a403c8356"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==0.17.1"
+        },
+        "httpx": {
+            "hashes": [
+                "sha256:447556b50c1921c351ea54b4fe79d91b724ed2b027462ab9a329465d147d5a4e",
+                "sha256:507d676fc3e26110d41df7d35ebd8b3b8585052450f4097401c9be59d928c63e"
+            ],
+            "version": "==0.24.0"
+        },
         "identify": {
             "hashes": [
-                "sha256:f0faad595a4687053669c112004178149f6c326db71ee999ae4636685753ad2f",
-                "sha256:f7a93d6cf98e29bd07663c60728e7a4057615068d7a639d132dc883b2d54d31e"
+                "sha256:0aac67d5b4812498056d28a9a512a483f5085cc28640b02b258a59dac34301d4",
+                "sha256:986dbfb38b1140e763e413e6feb44cd731faf72d1909543178aa79b0e258265d"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.5.22"
+            "version": "==2.5.24"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==3.4"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:03ba783c3a2c69d751b109fc0c94a62c51f581b3d6acf8ed1331b6d5729321ff",
-                "sha256:7a8bdf1bc3a726297f5cfbc999e6e7ff6b4fa41b26bba4afc580448624460045"
+                "sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed",
+                "sha256:92501cdf9cc66ebd3e612f1b4f0c0765dfa42f0fa38ffb319b6bd84dd675d705"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==6.6.0"
+        },
+        "importlib-resources": {
+            "hashes": [
+                "sha256:4be82589bf5c1d7999aedf2a45159d10cb3ca4f19b2271f8792bc8e6da7b22f6",
+                "sha256:7b1deeebbf351c7578e09bf2f63fa2ce8b5ffec296e0d349139d43cca061a81a"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==5.12.0"
+        },
+        "inflect": {
+            "hashes": [
+                "sha256:aadc7ed73928f5e014129794bbac03058cca35d0a973a5fc4eb45c7fa26005f9",
+                "sha256:b45d91a4a28a4e617ff1821117439b06eaa86e2a4573154af0149e9be6687238"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==6.5.0"
+            "version": "==5.6.2"
         },
         "iniconfig": {
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
+        "isort": {
+            "hashes": [
+                "sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504",
+                "sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6"
+            ],
+            "index": "pypi",
+            "version": "==5.12.0"
+        },
         "jaraco.classes": {
             "hashes": [
                 "sha256:2353de3288bc6b82120752201c6b1c1a14b058267fa424ed5ce5984e3b922158",
                 "sha256:89559fa5c1d3c34eff6f631ad80bb21f378dbcbb35dd161fd2c6b93f5be2f98a"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.2.3"
@@ -495,30 +645,152 @@
             "hashes": [
                 "sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806",
                 "sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755"
             ],
             "markers": "sys_platform == 'linux'",
             "version": "==0.8.0"
         },
+        "jinja2": {
+            "hashes": [
+                "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852",
+                "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==3.1.2"
+        },
+        "jsonschema": {
+            "hashes": [
+                "sha256:0f864437ab8b6076ba6707453ef8f98a6a0d512a80e93f8abdb676f737ecb60d",
+                "sha256:a870ad254da1a8ca84b6a2905cac29d265f805acc57af304784962a2aa6508f6"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==4.17.3"
+        },
+        "jsonschema-spec": {
+            "hashes": [
+                "sha256:34471d8b60e1f06d174236c4d3cf9590fbf3cff1cc733b28d15cd83672bcd062",
+                "sha256:824c743197bbe2104fcc6dce114a4082bf7f7efdebf16683510cb0ec6d8d53d0"
+            ],
+            "markers": "python_full_version >= '3.7.0' and python_full_version < '4.0.0'",
+            "version": "==0.1.4"
+        },
         "keyring": {
             "hashes": [
                 "sha256:771ed2a91909389ed6148631de678f82ddc73737d85a927f382a8a1b157898cd",
                 "sha256:ba2e15a9b35e21908d0aaf4e0a47acc52d6ae33444df0da2b49d41a46ef6d678"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==23.13.1"
         },
+        "lazy-object-proxy": {
+            "hashes": [
+                "sha256:09763491ce220c0299688940f8dc2c5d05fd1f45af1e42e636b2e8b2303e4382",
+                "sha256:0a891e4e41b54fd5b8313b96399f8b0e173bbbfc03c7631f01efbe29bb0bcf82",
+                "sha256:189bbd5d41ae7a498397287c408617fe5c48633e7755287b21d741f7db2706a9",
+                "sha256:18b78ec83edbbeb69efdc0e9c1cb41a3b1b1ed11ddd8ded602464c3fc6020494",
+                "sha256:1aa3de4088c89a1b69f8ec0dcc169aa725b0ff017899ac568fe44ddc1396df46",
+                "sha256:212774e4dfa851e74d393a2370871e174d7ff0ebc980907723bb67d25c8a7c30",
+                "sha256:2d0daa332786cf3bb49e10dc6a17a52f6a8f9601b4cf5c295a4f85854d61de63",
+                "sha256:5f83ac4d83ef0ab017683d715ed356e30dd48a93746309c8f3517e1287523ef4",
+                "sha256:659fb5809fa4629b8a1ac5106f669cfc7bef26fbb389dda53b3e010d1ac4ebae",
+                "sha256:660c94ea760b3ce47d1855a30984c78327500493d396eac4dfd8bd82041b22be",
+                "sha256:66a3de4a3ec06cd8af3f61b8e1ec67614fbb7c995d02fa224813cb7afefee701",
+                "sha256:721532711daa7db0d8b779b0bb0318fa87af1c10d7fe5e52ef30f8eff254d0cd",
+                "sha256:7322c3d6f1766d4ef1e51a465f47955f1e8123caee67dd641e67d539a534d006",
+                "sha256:79a31b086e7e68b24b99b23d57723ef7e2c6d81ed21007b6281ebcd1688acb0a",
+                "sha256:81fc4d08b062b535d95c9ea70dbe8a335c45c04029878e62d744bdced5141586",
+                "sha256:8fa02eaab317b1e9e03f69aab1f91e120e7899b392c4fc19807a8278a07a97e8",
+                "sha256:9090d8e53235aa280fc9239a86ae3ea8ac58eff66a705fa6aa2ec4968b95c821",
+                "sha256:946d27deaff6cf8452ed0dba83ba38839a87f4f7a9732e8f9fd4107b21e6ff07",
+                "sha256:9990d8e71b9f6488e91ad25f322898c136b008d87bf852ff65391b004da5e17b",
+                "sha256:9cd077f3d04a58e83d04b20e334f678c2b0ff9879b9375ed107d5d07ff160171",
+                "sha256:9e7551208b2aded9c1447453ee366f1c4070602b3d932ace044715d89666899b",
+                "sha256:9f5fa4a61ce2438267163891961cfd5e32ec97a2c444e5b842d574251ade27d2",
+                "sha256:b40387277b0ed2d0602b8293b94d7257e17d1479e257b4de114ea11a8cb7f2d7",
+                "sha256:bfb38f9ffb53b942f2b5954e0f610f1e721ccebe9cce9025a38c8ccf4a5183a4",
+                "sha256:cbf9b082426036e19c6924a9ce90c740a9861e2bdc27a4834fd0a910742ac1e8",
+                "sha256:d9e25ef10a39e8afe59a5c348a4dbf29b4868ab76269f81ce1674494e2565a6e",
+                "sha256:db1c1722726f47e10e0b5fdbf15ac3b8adb58c091d12b3ab713965795036985f",
+                "sha256:e7c21c95cae3c05c14aafffe2865bbd5e377cfc1348c4f7751d9dc9a48ca4bda",
+                "sha256:e8c6cfb338b133fbdbc5cfaa10fe3c6aeea827db80c978dbd13bc9dd8526b7d4",
+                "sha256:ea806fd4c37bf7e7ad82537b0757999264d5f70c45468447bb2b91afdbe73a6e",
+                "sha256:edd20c5a55acb67c7ed471fa2b5fb66cb17f61430b7a6b9c3b4a1e40293b1671",
+                "sha256:f0117049dd1d5635bbff65444496c90e0baa48ea405125c088e93d9cf4525b11",
+                "sha256:f0705c376533ed2a9e5e97aacdbfe04cecd71e0aa84c7c0595d02ef93b6e4455",
+                "sha256:f12ad7126ae0c98d601a7ee504c1122bcef553d1d5e0c3bfa77b16b3968d2734",
+                "sha256:f2457189d8257dd41ae9b434ba33298aec198e30adf2dcdaaa3a28b9994f6adb",
+                "sha256:f699ac1c768270c9e384e4cbd268d6e67aebcfae6cd623b4d7c3bfde5a35db59"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==1.9.0"
+        },
         "markdown-it-py": {
             "hashes": [
                 "sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30",
                 "sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.2.0"
         },
+        "markupsafe": {
+            "hashes": [
+                "sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed",
+                "sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc",
+                "sha256:090376d812fb6ac5f171e5938e82e7f2d7adc2b629101cec0db8b267815c85e2",
+                "sha256:0b462104ba25f1ac006fdab8b6a01ebbfbce9ed37fd37fd4acd70c67c973e460",
+                "sha256:137678c63c977754abe9086a3ec011e8fd985ab90631145dfb9294ad09c102a7",
+                "sha256:1bea30e9bf331f3fef67e0a3877b2288593c98a21ccb2cf29b74c581a4eb3af0",
+                "sha256:22152d00bf4a9c7c83960521fc558f55a1adbc0631fbb00a9471e097b19d72e1",
+                "sha256:22731d79ed2eb25059ae3df1dfc9cb1546691cc41f4e3130fe6bfbc3ecbbecfa",
+                "sha256:2298c859cfc5463f1b64bd55cb3e602528db6fa0f3cfd568d3605c50678f8f03",
+                "sha256:28057e985dace2f478e042eaa15606c7efccb700797660629da387eb289b9323",
+                "sha256:2e7821bffe00aa6bd07a23913b7f4e01328c3d5cc0b40b36c0bd81d362faeb65",
+                "sha256:2ec4f2d48ae59bbb9d1f9d7efb9236ab81429a764dedca114f5fdabbc3788013",
+                "sha256:340bea174e9761308703ae988e982005aedf427de816d1afe98147668cc03036",
+                "sha256:40627dcf047dadb22cd25ea7ecfe9cbf3bbbad0482ee5920b582f3809c97654f",
+                "sha256:40dfd3fefbef579ee058f139733ac336312663c6706d1163b82b3003fb1925c4",
+                "sha256:4cf06cdc1dda95223e9d2d3c58d3b178aa5dacb35ee7e3bbac10e4e1faacb419",
+                "sha256:50c42830a633fa0cf9e7d27664637532791bfc31c731a87b202d2d8ac40c3ea2",
+                "sha256:55f44b440d491028addb3b88f72207d71eeebfb7b5dbf0643f7c023ae1fba619",
+                "sha256:608e7073dfa9e38a85d38474c082d4281f4ce276ac0010224eaba11e929dd53a",
+                "sha256:63ba06c9941e46fa389d389644e2d8225e0e3e5ebcc4ff1ea8506dce646f8c8a",
+                "sha256:65608c35bfb8a76763f37036547f7adfd09270fbdbf96608be2bead319728fcd",
+                "sha256:665a36ae6f8f20a4676b53224e33d456a6f5a72657d9c83c2aa00765072f31f7",
+                "sha256:6d6607f98fcf17e534162f0709aaad3ab7a96032723d8ac8750ffe17ae5a0666",
+                "sha256:7313ce6a199651c4ed9d7e4cfb4aa56fe923b1adf9af3b420ee14e6d9a73df65",
+                "sha256:7668b52e102d0ed87cb082380a7e2e1e78737ddecdde129acadb0eccc5423859",
+                "sha256:7df70907e00c970c60b9ef2938d894a9381f38e6b9db73c5be35e59d92e06625",
+                "sha256:7e007132af78ea9df29495dbf7b5824cb71648d7133cf7848a2a5dd00d36f9ff",
+                "sha256:835fb5e38fd89328e9c81067fd642b3593c33e1e17e2fdbf77f5676abb14a156",
+                "sha256:8bca7e26c1dd751236cfb0c6c72d4ad61d986e9a41bbf76cb445f69488b2a2bd",
+                "sha256:8db032bf0ce9022a8e41a22598eefc802314e81b879ae093f36ce9ddf39ab1ba",
+                "sha256:99625a92da8229df6d44335e6fcc558a5037dd0a760e11d84be2260e6f37002f",
+                "sha256:9cad97ab29dfc3f0249b483412c85c8ef4766d96cdf9dcf5a1e3caa3f3661cf1",
+                "sha256:a4abaec6ca3ad8660690236d11bfe28dfd707778e2442b45addd2f086d6ef094",
+                "sha256:a6e40afa7f45939ca356f348c8e23048e02cb109ced1eb8420961b2f40fb373a",
+                "sha256:a6f2fcca746e8d5910e18782f976489939d54a91f9411c32051b4aab2bd7c513",
+                "sha256:a806db027852538d2ad7555b203300173dd1b77ba116de92da9afbc3a3be3eed",
+                "sha256:abcabc8c2b26036d62d4c746381a6f7cf60aafcc653198ad678306986b09450d",
+                "sha256:b8526c6d437855442cdd3d87eede9c425c4445ea011ca38d937db299382e6fa3",
+                "sha256:bb06feb762bade6bf3c8b844462274db0c76acc95c52abe8dbed28ae3d44a147",
+                "sha256:c0a33bc9f02c2b17c3ea382f91b4db0e6cde90b63b296422a939886a7a80de1c",
+                "sha256:c4a549890a45f57f1ebf99c067a4ad0cb423a05544accaf2b065246827ed9603",
+                "sha256:ca244fa73f50a800cf8c3ebf7fd93149ec37f5cb9596aa8873ae2c1d23498601",
+                "sha256:cf877ab4ed6e302ec1d04952ca358b381a882fbd9d1b07cccbfd61783561f98a",
+                "sha256:d9d971ec1e79906046aa3ca266de79eac42f1dbf3612a05dc9368125952bd1a1",
+                "sha256:da25303d91526aac3672ee6d49a2f3db2d9502a4a60b55519feb1a4c7714e07d",
+                "sha256:e55e40ff0cc8cc5c07996915ad367fa47da6b3fc091fdadca7f5403239c5fec3",
+                "sha256:f03a532d7dee1bed20bc4884194a16160a2de9ffc6354b3878ec9682bb623c54",
+                "sha256:f1cd098434e83e656abf198f103a8207a8187c0fc110306691a2e94a78d0abb2",
+                "sha256:f2bfb563d0211ce16b63c7cb9395d2c682a23187f54c3d79bfec33e6705473c6",
+                "sha256:f8ffb705ffcf5ddd0e80b65ddf7bed7ee4f5a441ea7d3419e861a12eaf41af58"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==2.1.2"
+        },
         "mdurl": {
             "hashes": [
                 "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8",
                 "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.1.2"
@@ -529,107 +801,189 @@
                 "sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==9.1.0"
         },
         "mypy": {
             "hashes": [
-                "sha256:023fe9e618182ca6317ae89833ba422c411469156b690fde6a315ad10695a521",
-                "sha256:031fc69c9a7e12bcc5660b74122ed84b3f1c505e762cc4296884096c6d8ee140",
-                "sha256:2de7babe398cb7a85ac7f1fd5c42f396c215ab3eff731b4d761d68d0f6a80f48",
-                "sha256:2e93a8a553e0394b26c4ca683923b85a69f7ccdc0139e6acd1354cc884fe0128",
-                "sha256:390bc685ec209ada4e9d35068ac6988c60160b2b703072d2850457b62499e336",
-                "sha256:3a2d219775a120581a0ae8ca392b31f238d452729adbcb6892fa89688cb8306a",
-                "sha256:3efde4af6f2d3ccf58ae825495dbb8d74abd6d176ee686ce2ab19bd025273f41",
-                "sha256:4a99fe1768925e4a139aace8f3fb66db3576ee1c30b9c0f70f744ead7e329c9f",
-                "sha256:4b41412df69ec06ab141808d12e0bf2823717b1c363bd77b4c0820feaa37249e",
-                "sha256:4c8d8c6b80aa4a1689f2a179d31d86ae1367ea4a12855cc13aa3ba24bb36b2d8",
-                "sha256:4d19f1a239d59f10fdc31263d48b7937c585810288376671eaf75380b074f238",
-                "sha256:4e4a682b3f2489d218751981639cffc4e281d548f9d517addfd5a2917ac78119",
-                "sha256:695c45cea7e8abb6f088a34a6034b1d273122e5530aeebb9c09626cea6dca4cb",
-                "sha256:701189408b460a2ff42b984e6bd45c3f41f0ac9f5f58b8873bbedc511900086d",
-                "sha256:70894c5345bea98321a2fe84df35f43ee7bb0feec117a71420c60459fc3e1eed",
-                "sha256:8293a216e902ac12779eb7a08f2bc39ec6c878d7c6025aa59464e0c4c16f7eb9",
-                "sha256:8d26b513225ffd3eacece727f4387bdce6469192ef029ca9dd469940158bc89e",
-                "sha256:a197ad3a774f8e74f21e428f0de7f60ad26a8d23437b69638aac2764d1e06a6a",
-                "sha256:bea55fc25b96c53affab852ad94bf111a3083bc1d8b0c76a61dd101d8a388cf5",
-                "sha256:c9a084bce1061e55cdc0493a2ad890375af359c766b8ac311ac8120d3a472950",
-                "sha256:d0e9464a0af6715852267bf29c9553e4555b61f5904a4fc538547a4d67617937",
-                "sha256:d8e9187bfcd5ffedbe87403195e1fc340189a68463903c39e2b63307c9fa0394",
-                "sha256:eaeaa0888b7f3ccb7bcd40b50497ca30923dba14f385bde4af78fac713d6d6f6",
-                "sha256:f46af8d162f3d470d8ffc997aaf7a269996d205f9d746124a179d3abe05ac602",
-                "sha256:f70a40410d774ae23fcb4afbbeca652905a04de7948eaf0b1789c8d1426b72d1",
-                "sha256:fe91be1c51c90e2afe6827601ca14353bbf3953f343c2129fa1e247d55fd95ba"
+                "sha256:1c4c42c60a8103ead4c1c060ac3cdd3ff01e18fddce6f1016e08939647a0e703",
+                "sha256:44797d031a41516fcf5cbfa652265bb994e53e51994c1bd649ffcd0c3a7eccbf",
+                "sha256:473117e310febe632ddf10e745a355714e771ffe534f06db40702775056614c4",
+                "sha256:4c99c3ecf223cf2952638da9cd82793d8f3c0c5fa8b6ae2b2d9ed1e1ff51ba85",
+                "sha256:550a8b3a19bb6589679a7c3c31f64312e7ff482a816c96e0cecec9ad3a7564dd",
+                "sha256:658fe7b674769a0770d4b26cb4d6f005e88a442fe82446f020be8e5f5efb2fae",
+                "sha256:6e33bb8b2613614a33dff70565f4c803f889ebd2f859466e42b46e1df76018dd",
+                "sha256:6e42d29e324cdda61daaec2336c42512e59c7c375340bd202efa1fe0f7b8f8ca",
+                "sha256:74bc9b6e0e79808bf8678d7678b2ae3736ea72d56eede3820bd3849823e7f305",
+                "sha256:76ec771e2342f1b558c36d49900dfe81d140361dd0d2df6cd71b3db1be155409",
+                "sha256:7d23370d2a6b7a71dc65d1266f9a34e4cde9e8e21511322415db4b26f46f6b8c",
+                "sha256:87df44954c31d86df96c8bd6e80dfcd773473e877ac6176a8e29898bfb3501cb",
+                "sha256:8c5979d0deb27e0f4479bee18ea0f83732a893e81b78e62e2dda3e7e518c92ee",
+                "sha256:95d8d31a7713510685b05fbb18d6ac287a56c8f6554d88c19e73f724a445448a",
+                "sha256:a22435632710a4fcf8acf86cbd0d69f68ac389a3892cb23fbad176d1cddaf228",
+                "sha256:a8763e72d5d9574d45ce5881962bc8e9046bf7b375b0abf031f3e6811732a897",
+                "sha256:c1eb485cea53f4f5284e5baf92902cd0088b24984f4209e25981cc359d64448d",
+                "sha256:c5d2cc54175bab47011b09688b418db71403aefad07cbcd62d44010543fc143f",
+                "sha256:cbc07246253b9e3d7d74c9ff948cd0fd7a71afcc2b77c7f0a59c26e9395cb152",
+                "sha256:d0b6c62206e04061e27009481cb0ec966f7d6172b5b936f3ead3d74f29fe3dcf",
+                "sha256:ddae0f39ca146972ff6bb4399f3b2943884a774b8771ea0a8f50e971f5ea5ba8",
+                "sha256:e1f4d16e296f5135624b34e8fb741eb0eadedca90862405b1f1fde2040b9bd11",
+                "sha256:e86c2c6852f62f8f2b24cb7a613ebe8e0c7dc1402c61d36a609174f63e0ff017",
+                "sha256:ebc95f8386314272bbc817026f8ce8f4f0d2ef7ae44f947c4664efac9adec929",
+                "sha256:f9dca1e257d4cc129517779226753dbefb4f2266c4eaad610fc15c6a7e14283e",
+                "sha256:faff86aa10c1aa4a10e1a301de160f3d8fc8703b88c7e98de46b531ff1276a9a"
             ],
             "index": "pypi",
-            "version": "==1.2.0"
+            "version": "==1.3.0"
         },
         "mypy-extensions": {
             "hashes": [
                 "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
                 "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.0.0"
         },
         "nodeenv": {
             "hashes": [
-                "sha256:27083a7b96a25f2f5e1d8cb4b6317ee8aeda3bdd121394e5ac54e498028a042e",
-                "sha256:e0e7f7dfb85fc5394c6fe1e8fa98131a2473e04311a45afb6508f7cf1836fa2b"
+                "sha256:d51e0c37e64fbf47d017feac3145cdbb58836d7eee8c6f6d3b6880c5456227d2",
+                "sha256:df865724bb3c3adc86b3876fa209771517b0cfe596beff01a92700e0e8be4cec"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
-            "version": "==1.7.0"
+            "version": "==1.8.0"
+        },
+        "openapi-schema-validator": {
+            "hashes": [
+                "sha256:34fbd14b7501abe25e64d7b4624a9db02cde1a578d285b3da6f34b290cdf0b3a",
+                "sha256:7cf27585dd7970b7257cefe48e1a3a10d4e34421831bdb472d96967433bc27bd"
+            ],
+            "markers": "python_full_version >= '3.7.0' and python_full_version < '4.0.0'",
+            "version": "==0.3.4"
+        },
+        "openapi-spec-validator": {
+            "hashes": [
+                "sha256:4a8aee1e45b1ac868e07ab25e18828fe9837baddd29a8e20fdb3d3c61c8eea3d",
+                "sha256:8248634bad1f23cac5d5a34e193ab36e23914057ca69e91a1ede5af75552c465"
+            ],
+            "markers": "python_full_version >= '3.7.0' and python_full_version < '4.0.0'",
+            "version": "==0.5.1"
         },
         "packaging": {
             "hashes": [
                 "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
                 "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==23.1"
         },
+        "pathable": {
+            "hashes": [
+                "sha256:5c869d315be50776cc8a993f3af43e0c60dc01506b399643f919034ebf4cdcab",
+                "sha256:cdd7b1f9d7d5c8b8d3315dbf5a86b2596053ae845f056f57d97c0eefff84da14"
+            ],
+            "markers": "python_full_version >= '3.7.0' and python_full_version < '4.0.0'",
+            "version": "==0.4.3"
+        },
+        "pathspec": {
+            "hashes": [
+                "sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687",
+                "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==0.11.1"
+        },
         "pkginfo": {
             "hashes": [
                 "sha256:4b7a555a6d5a22169fcc9cf7bfd78d296b0361adad412a346c1226849af5e546",
                 "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.9.6"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:d5b638ca397f25f979350ff789db335903d7ea010ab28903f57b27e1b16c2b08",
-                "sha256:ebe11c0d7a805086e99506aa331612429a72ca7cd52a1f0d277dc4adc20cb10e"
+                "sha256:412dae91f52a6f84830f39a8078cecd0e866cb72294a5c66808e74d5e88d251f",
+                "sha256:e2378146f1964972c03c085bb5662ae80b2b8c06226c54b2ff4aa9483e8a13a5"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.2.0"
+            "version": "==3.5.1"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.0.0"
         },
+        "prance": {
+            "hashes": [
+                "sha256:57deeb67b7e93ef27c1c17845bf3ccb4af288ccfb5748c7e01779c01a8507f27",
+                "sha256:9a83f8a4f5fe0f2d896d238d4bec6b5788b10b94155414b3d88c21c1579b85bf"
+            ],
+            "markers": "python_version >= '3.8'",
+            "version": "==0.22.2.22.0"
+        },
         "pre-commit": {
             "hashes": [
-                "sha256:0b4210aea813fe81144e87c5a291f09ea66f199f367fa1df41b55e1d26e1e2b4",
-                "sha256:5b808fcbda4afbccf6d6633a56663fed35b6c2bc08096fd3d47ce197ac351d9d"
+                "sha256:66e37bec2d882de1f17f88075047ef8962581f83c234ac08da21a0c58953d1f0",
+                "sha256:8056bc52181efadf4aac792b1f4f255dfd2fb5a350ded7335d251a68561e8cb6"
             ],
             "index": "pypi",
-            "version": "==3.2.2"
+            "version": "==3.3.2"
         },
         "pycparser": {
             "hashes": [
                 "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
                 "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
             ],
             "version": "==2.21"
         },
+        "pydantic": {
+            "hashes": [
+                "sha256:01aea3a42c13f2602b7ecbbea484a98169fb568ebd9e247593ea05f01b884b2e",
+                "sha256:0cd181f1d0b1d00e2b705f1bf1ac7799a2d938cce3376b8007df62b29be3c2c6",
+                "sha256:10a86d8c8db68086f1e30a530f7d5f83eb0685e632e411dbbcf2d5c0150e8dcd",
+                "sha256:193924c563fae6ddcb71d3f06fa153866423ac1b793a47936656e806b64e24ca",
+                "sha256:464855a7ff7f2cc2cf537ecc421291b9132aa9c79aef44e917ad711b4a93163b",
+                "sha256:516f1ed9bc2406a0467dd777afc636c7091d71f214d5e413d64fef45174cfc7a",
+                "sha256:6434b49c0b03a51021ade5c4daa7d70c98f7a79e95b551201fff682fc1661245",
+                "sha256:64d34ab766fa056df49013bb6e79921a0265204c071984e75a09cbceacbbdd5d",
+                "sha256:670bb4683ad1e48b0ecb06f0cfe2178dcf74ff27921cdf1606e527d2617a81ee",
+                "sha256:68792151e174a4aa9e9fc1b4e653e65a354a2fa0fed169f7b3d09902ad2cb6f1",
+                "sha256:701daea9ffe9d26f97b52f1d157e0d4121644f0fcf80b443248434958fd03dc3",
+                "sha256:7d45fc99d64af9aaf7e308054a0067fdcd87ffe974f2442312372dfa66e1001d",
+                "sha256:80b1fab4deb08a8292d15e43a6edccdffa5377a36a4597bb545b93e79c5ff0a5",
+                "sha256:82dffb306dd20bd5268fd6379bc4bfe75242a9c2b79fec58e1041fbbdb1f7914",
+                "sha256:8c7f51861d73e8b9ddcb9916ae7ac39fb52761d9ea0df41128e81e2ba42886cd",
+                "sha256:950ce33857841f9a337ce07ddf46bc84e1c4946d2a3bba18f8280297157a3fd1",
+                "sha256:976cae77ba6a49d80f461fd8bba183ff7ba79f44aa5cfa82f1346b5626542f8e",
+                "sha256:9f6f0fd68d73257ad6685419478c5aece46432f4bdd8d32c7345f1986496171e",
+                "sha256:a7cd2251439988b413cb0a985c4ed82b6c6aac382dbaff53ae03c4b23a70e80a",
+                "sha256:abfb7d4a7cd5cc4e1d1887c43503a7c5dd608eadf8bc615413fc498d3e4645cd",
+                "sha256:ae150a63564929c675d7f2303008d88426a0add46efd76c3fc797cd71cb1b46f",
+                "sha256:b0f85904f73161817b80781cc150f8b906d521fa11e3cdabae19a581c3606209",
+                "sha256:b4a849d10f211389502059c33332e91327bc154acc1845f375a99eca3afa802d",
+                "sha256:c15582f9055fbc1bfe50266a19771bbbef33dd28c45e78afbe1996fd70966c2a",
+                "sha256:c230c0d8a322276d6e7b88c3f7ce885f9ed16e0910354510e0bae84d54991143",
+                "sha256:cc1dde4e50a5fc1336ee0581c1612215bc64ed6d28d2c7c6f25d2fe3e7c3e918",
+                "sha256:cf135c46099ff3f919d2150a948ce94b9ce545598ef2c6c7bf55dca98a304b52",
+                "sha256:cfc83c0678b6ba51b0532bea66860617c4cd4251ecf76e9846fa5a9f3454e97e",
+                "sha256:d2a5ebb48958754d386195fe9e9c5106f11275867051bf017a8059410e9abf1f",
+                "sha256:d71e69699498b020ea198468e2480a2f1e7433e32a3a99760058c6520e2bea7e",
+                "sha256:d75ae19d2a3dbb146b6f324031c24f8a3f52ff5d6a9f22f0683694b3afcb16fb",
+                "sha256:dfe2507b8ef209da71b6fb5f4e597b50c5a34b78d7e857c4f8f3115effaef5fe",
+                "sha256:e0cfe895a504c060e5d36b287ee696e2fdad02d89e0d895f83037245218a87fe",
+                "sha256:e79e999e539872e903767c417c897e729e015872040e56b96e67968c3b918b2d",
+                "sha256:ecbbc51391248116c0a055899e6c3e7ffbb11fb5e2a4cd6f2d0b93272118a209",
+                "sha256:f4a2b50e2b03d5776e7f21af73e2070e1b5c0d0df255a827e7c632962f8315af"
+            ],
+            "index": "pypi",
+            "version": "==1.10.7"
+        },
         "pygments": {
             "hashes": [
                 "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
                 "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.15.1"
@@ -638,14 +992,54 @@
             "hashes": [
                 "sha256:283c11acd6b928d2f6a7c73fa0d01cb2bdc5f07c57a2eeb6e83d5e56b97976f8",
                 "sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.0"
         },
+        "pyrsistent": {
+            "hashes": [
+                "sha256:016ad1afadf318eb7911baa24b049909f7f3bb2c5b1ed7b6a8f21db21ea3faa8",
+                "sha256:1a2994773706bbb4995c31a97bc94f1418314923bd1048c6d964837040376440",
+                "sha256:20460ac0ea439a3e79caa1dbd560344b64ed75e85d8703943e0b66c2a6150e4a",
+                "sha256:3311cb4237a341aa52ab8448c27e3a9931e2ee09561ad150ba94e4cfd3fc888c",
+                "sha256:3a8cb235fa6d3fd7aae6a4f1429bbb1fec1577d978098da1252f0489937786f3",
+                "sha256:3ab2204234c0ecd8b9368dbd6a53e83c3d4f3cab10ecaf6d0e772f456c442393",
+                "sha256:42ac0b2f44607eb92ae88609eda931a4f0dfa03038c44c772e07f43e738bcac9",
+                "sha256:49c32f216c17148695ca0e02a5c521e28a4ee6c5089f97e34fe24163113722da",
+                "sha256:4b774f9288dda8d425adb6544e5903f1fb6c273ab3128a355c6b972b7df39dcf",
+                "sha256:4c18264cb84b5e68e7085a43723f9e4c1fd1d935ab240ce02c0324a8e01ccb64",
+                "sha256:5a474fb80f5e0d6c9394d8db0fc19e90fa540b82ee52dba7d246a7791712f74a",
+                "sha256:64220c429e42a7150f4bfd280f6f4bb2850f95956bde93c6fda1b70507af6ef3",
+                "sha256:878433581fc23e906d947a6814336eee031a00e6defba224234169ae3d3d6a98",
+                "sha256:99abb85579e2165bd8522f0c0138864da97847875ecbd45f3e7e2af569bfc6f2",
+                "sha256:a2471f3f8693101975b1ff85ffd19bb7ca7dd7c38f8a81701f67d6b4f97b87d8",
+                "sha256:aeda827381f5e5d65cced3024126529ddc4289d944f75e090572c77ceb19adbf",
+                "sha256:b735e538f74ec31378f5a1e3886a26d2ca6351106b4dfde376a26fc32a044edc",
+                "sha256:c147257a92374fde8498491f53ffa8f4822cd70c0d85037e09028e478cababb7",
+                "sha256:c4db1bd596fefd66b296a3d5d943c94f4fac5bcd13e99bffe2ba6a759d959a28",
+                "sha256:c74bed51f9b41c48366a286395c67f4e894374306b197e62810e0fdaf2364da2",
+                "sha256:c9bb60a40a0ab9aba40a59f68214eed5a29c6274c83b2cc206a359c4a89fa41b",
+                "sha256:cc5d149f31706762c1f8bda2e8c4f8fead6e80312e3692619a75301d3dbb819a",
+                "sha256:ccf0d6bd208f8111179f0c26fdf84ed7c3891982f2edaeae7422575f47e66b64",
+                "sha256:e42296a09e83028b3476f7073fcb69ffebac0e66dbbfd1bd847d61f74db30f19",
+                "sha256:e8f2b814a3dc6225964fa03d8582c6e0b6650d68a232df41e3cc1b66a5d2f8d1",
+                "sha256:f0774bf48631f3a20471dd7c5989657b639fd2d285b861237ea9e82c36a415a9",
+                "sha256:f0e7c4b2f77593871e918be000b96c8107da48444d57005b6a6bc61fb4331b2c"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==0.19.3"
+        },
+        "pysnooper": {
+            "hashes": [
+                "sha256:378f13d731a3e04d3d0350e5f295bdd0f1b49fc8a8b8bf2067fe1e5290bd20be",
+                "sha256:d17dc91cca1593c10230dce45e46b1d3ff0f8910f0c38e941edf6ba1260b3820"
+            ],
+            "version": "==1.1.1"
+        },
         "pytest": {
             "hashes": [
                 "sha256:3799fa815351fea3a5e96ac7e503a96fa51cc9942c3753cda7651b93c1cfa362",
                 "sha256:434afafd78b1d78ed0addf160ad2b77a30d35d4bdf8af234fe621919d9ed15e3"
             ],
             "index": "pypi",
             "version": "==7.3.1"
@@ -718,114 +1112,180 @@
                 "sha256:f67a16caedfa71eef48a31b39708637a6f4664c4394801a7b0d6432d13907343"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==37.3"
         },
         "requests": {
             "hashes": [
-                "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
-                "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
+                "sha256:10e94cc4f3121ee6da529d358cdaeaff2f1c409cd377dbc72b825852f2f7e294",
+                "sha256:239d7d4458afcb28a692cdd298d87542235f4ca8d36d03a15bfc128a6559a2f4"
             ],
             "index": "pypi",
-            "version": "==2.28.2"
+            "version": "==2.30.0"
         },
         "requests-toolbelt": {
             "hashes": [
-                "sha256:18565aa58116d9951ac39baa288d3adb5b3ff975c4f25eee78555d89e8f247f7",
-                "sha256:62e09f7ff5ccbda92772a29f394a49c3ad6cb181d568b1337626b2abb628a63d"
+                "sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6",
+                "sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==0.10.1"
+            "version": "==1.0.0"
         },
         "rfc3986": {
             "hashes": [
                 "sha256:50b1502b60e289cb37883f3dfd34532b8873c7de9f49bb546641ce9cbd256ebd",
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
-                "sha256:22b74cae0278fd5086ff44144d3813be1cedc9115bdfabbfefd86400cb88b20a",
-                "sha256:b5d573e13605423ec80bdd0cd5f8541f7844a0e71a13f74cf454ccb2f490708b"
+                "sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c",
+                "sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704"
             ],
             "index": "pypi",
-            "version": "==13.3.4"
+            "version": "==13.3.5"
+        },
+        "ruamel.yaml": {
+            "hashes": [
+                "sha256:25d0ee82a0a9a6f44683dcf8c282340def4074a4562f3a24f55695bb254c1693",
+                "sha256:baa2d0a5aad2034826c439ce61c142c07082b76f4791d54145e131206e998059"
+            ],
+            "markers": "python_version >= '3'",
+            "version": "==0.17.26"
+        },
+        "ruamel.yaml.clib": {
+            "hashes": [
+                "sha256:045e0626baf1c52e5527bd5db361bc83180faaba2ff586e763d3d5982a876a9e",
+                "sha256:15910ef4f3e537eea7fe45f8a5d19997479940d9196f357152a09031c5be59f3",
+                "sha256:184faeaec61dbaa3cace407cffc5819f7b977e75360e8d5ca19461cd851a5fc5",
+                "sha256:1f08fd5a2bea9c4180db71678e850b995d2a5f4537be0e94557668cf0f5f9497",
+                "sha256:2aa261c29a5545adfef9296b7e33941f46aa5bbd21164228e833412af4c9c75f",
+                "sha256:3110a99e0f94a4a3470ff67fc20d3f96c25b13d24c6980ff841e82bafe827cac",
+                "sha256:3243f48ecd450eddadc2d11b5feb08aca941b5cd98c9b1db14b2fd128be8c697",
+                "sha256:370445fd795706fd291ab00c9df38a0caed0f17a6fb46b0f607668ecb16ce763",
+                "sha256:40d030e2329ce5286d6b231b8726959ebbe0404c92f0a578c0e2482182e38282",
+                "sha256:41d0f1fa4c6830176eef5b276af04c89320ea616655d01327d5ce65e50575c94",
+                "sha256:4a4d8d417868d68b979076a9be6a38c676eca060785abaa6709c7b31593c35d1",
+                "sha256:4b3a93bb9bc662fc1f99c5c3ea8e623d8b23ad22f861eb6fce9377ac07ad6072",
+                "sha256:5bc0667c1eb8f83a3752b71b9c4ba55ef7c7058ae57022dd9b29065186a113d9",
+                "sha256:721bc4ba4525f53f6a611ec0967bdcee61b31df5a56801281027a3a6d1c2daf5",
+                "sha256:763d65baa3b952479c4e972669f679fe490eee058d5aa85da483ebae2009d231",
+                "sha256:7bdb4c06b063f6fd55e472e201317a3bb6cdeeee5d5a38512ea5c01e1acbdd93",
+                "sha256:8831a2cedcd0f0927f788c5bdf6567d9dc9cc235646a434986a852af1cb54b4b",
+                "sha256:91a789b4aa0097b78c93e3dc4b40040ba55bef518f84a40d4442f713b4094acb",
+                "sha256:92460ce908546ab69770b2e576e4f99fbb4ce6ab4b245345a3869a0a0410488f",
+                "sha256:99e77daab5d13a48a4054803d052ff40780278240a902b880dd37a51ba01a307",
+                "sha256:a234a20ae07e8469da311e182e70ef6b199d0fbeb6c6cc2901204dd87fb867e8",
+                "sha256:a7b301ff08055d73223058b5c46c55638917f04d21577c95e00e0c4d79201a6b",
+                "sha256:be2a7ad8fd8f7442b24323d24ba0b56c51219513cfa45b9ada3b87b76c374d4b",
+                "sha256:bf9a6bc4a0221538b1a7de3ed7bca4c93c02346853f44e1cd764be0023cd3640",
+                "sha256:c3ca1fbba4ae962521e5eb66d72998b51f0f4d0f608d3c0347a48e1af262efa7",
+                "sha256:d000f258cf42fec2b1bbf2863c61d7b8918d31ffee905da62dede869254d3b8a",
+                "sha256:d5859983f26d8cd7bb5c287ef452e8aacc86501487634573d260968f753e1d71",
+                "sha256:d5e51e2901ec2366b79f16c2299a03e74ba4531ddcfacc1416639c557aef0ad8",
+                "sha256:da538167284de58a52109a9b89b8f6a53ff8437dd6dc26d33b57bf6699153122",
+                "sha256:debc87a9516b237d0466a711b18b6ebeb17ba9f391eb7f91c649c5c4ec5006c7",
+                "sha256:df5828871e6648db72d1c19b4bd24819b80a755c4541d3409f0f7acd0f335c80",
+                "sha256:ecdf1a604009bd35c674b9225a8fa609e0282d9b896c03dd441a91e5f53b534e",
+                "sha256:efa08d63ef03d079dcae1dfe334f6c8847ba8b645d08df286358b1f5293d24ab",
+                "sha256:f01da5790e95815eb5a8a138508c01c758e5f5bc0ce4286c4f7028b8dd7ac3d0",
+                "sha256:f34019dced51047d6f70cb9383b2ae2853b7fc4dce65129a5acd49f4f9256646",
+                "sha256:f6d3d39611ac2e4f62c3128a9eed45f19a6608670c5a2f4f07f24e8de3441d38"
+            ],
+            "markers": "platform_python_implementation == 'CPython' and python_version < '3.12'",
+            "version": "==0.2.7"
         },
         "secretstorage": {
             "hashes": [
                 "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77",
                 "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
             ],
             "markers": "sys_platform == 'linux'",
             "version": "==3.3.3"
         },
         "setuptools": {
             "hashes": [
-                "sha256:257de92a9d50a60b8e22abfcbb771571fde0dbf3ec234463212027a4eeecbe9a",
-                "sha256:e728ca814a823bf7bf60162daf9db95b93d532948c4c0bea762ce62f60189078"
+                "sha256:23aaf86b85ca52ceb801d32703f12d77517b2556af839621c641fca11287952b",
+                "sha256:f104fa03692a2602fa0fec6c6a9e63b6c8a968de13e17c026957dd1f53d80990"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==67.6.1"
+            "version": "==67.7.2"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2'",
             "version": "==1.16.0"
         },
+        "sniffio": {
+            "hashes": [
+                "sha256:e60305c5e5d314f5389259b7f22aaa33d8f7dee49763119234af3755c55b9101",
+                "sha256:eecefdce1e5bbfb7ad2eeaabf7c1eeb404d7757c379bd1f7e5cce9d8bf425384"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==1.3.0"
+        },
+        "toml": {
+            "hashes": [
+                "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b",
+                "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"
+            ],
+            "markers": "python_version >= '2.6' and python_version not in '3.0, 3.1, 3.2'",
+            "version": "==0.10.2"
+        },
         "twine": {
             "hashes": [
                 "sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8",
                 "sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8"
             ],
             "index": "pypi",
             "version": "==4.0.2"
         },
         "types-requests": {
             "hashes": [
-                "sha256:0d580652ce903f643f8c3b494dd01d29367ea57cea0c7ad7f65cf3169092edb0",
-                "sha256:cc1aba862575019306b2ed134eb1ea994cab1c887a22e18d3383e6dd42e9789b"
+                "sha256:c6cf08e120ca9f0dc4fa4e32c3f953c3fba222bcc1db6b97695bce8da1ba9864",
+                "sha256:dec781054324a70ba64430ae9e62e7e9c8e4618c185a5cb3f87a6738251b5a31"
             ],
             "index": "pypi",
-            "version": "==2.28.11.17"
+            "version": "==2.30.0.0"
         },
         "types-urllib3": {
             "hashes": [
-                "sha256:12c744609d588340a07e45d333bf870069fc8793bcf96bae7a96d4712a42591d",
-                "sha256:c44881cde9fc8256d05ad6b21f50c4681eb20092552351570ab0a8a0653286d6"
+                "sha256:3300538c9dc11dad32eae4827ac313f5d986b8b21494801f1bf97a1ac6c03ae5",
+                "sha256:5dbd1d2bef14efee43f5318b5d36d805a489f6600252bb53626d4bfafd95e27c"
             ],
-            "version": "==1.26.25.10"
+            "version": "==1.26.25.13"
         },
         "typing-extensions": {
             "hashes": [
                 "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb",
                 "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.5.0"
         },
         "urllib3": {
             "hashes": [
-                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
-                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
+                "sha256:61717a1095d7e155cdb737ac7bb2f4324a858a1e2e6466f6d03ff630ca68d3cc",
+                "sha256:d055c2f9d38dc53c808f6fdc8eab7360b6fdbbde02340ed25cfbcd817c62469e"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.15"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.0.2"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:278753c47aaef1a0f14e6db8a4c5e1e040e90aea654d0fc1dc7e0d8a42616cc3",
-                "sha256:48fd3b907b5149c5aab7c23d9790bea4cac6bc6b150af8635febc4cfeab1275a"
+                "sha256:6abec7670e5802a528357fdc75b26b9f57d5d92f29c5462ba0fbe45feacc685e",
+                "sha256:a85caa554ced0c0afbd0d638e7e2d7b5f92d23478d05d17a76daeac8f279f924"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==20.22.0"
+            "version": "==20.23.0"
         },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
```

### Comparing `ord_mediascout_client-0.0.8/setup.cfg` & `ord_mediascout_client-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `ord_mediascout_client-0.0.8/.idea/workspace.xml` & `ord_mediascout_client-0.0.9/.idea/workspace.xml`

 * *Files 7% similar despite different names*

#### Comparing `ord_mediascout_client-0.0.8/.idea/workspace.xml` & `ord_mediascout_client-0.0.9/.idea/workspace.xml`

```diff
@@ -1,142 +1,169 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="ChangeListManager">
-    <list default="true" id="05a5941d-3a7a-4f00-8c25-56a959e7d84f" name="Default" comment="">
-      <change beforePath="$PROJECT_DIR$/Pipfile" beforeDir="false" afterPath="$PROJECT_DIR$/Pipfile" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/Pipfile.lock" beforeDir="false" afterPath="$PROJECT_DIR$/Pipfile.lock" afterDir="false"/>
-    </list>
+    <list default="true" id="05a5941d-3a7a-4f00-8c25-56a959e7d84f" name="Default" comment=""/>
     <option name="EXCLUDED_CONVERTED_TO_IGNORED" value="true"/>
     <option name="TRACKING_ENABLED" value="true"/>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileEditorManager">
     <leaf SIDE_TABS_SIZE_LIMIT_KEY="375">
       <file leaf-file-name="contract_test.py" pinned="false" current-in-tab="false">
         <entry file="file://$PROJECT_DIR$/tests/contract_test.py">
           <provider selected="true" editor-type-id="text-editor">
-            <state relative-caret-position="-2469">
-              <caret line="22" selection-start-line="22" selection-end-line="22"/>
+            <state relative-caret-position="675">
+              <caret line="108" column="18" selection-start-line="108" selection-start-column="18" selection-end-line="108" selection-end-column="18"/>
               <folding>
                 <element signature="e#0#13#0" expanded="true"/>
               </folding>
             </state>
           </provider>
         </entry>
       </file>
       <file leaf-file-name="creative_test.py" pinned="false" current-in-tab="false">
         <entry file="file://$PROJECT_DIR$/tests/creative_test.py">
           <provider selected="true" editor-type-id="text-editor">
-            <state relative-caret-position="648">
-              <caret line="27" column="19" selection-start-line="27" selection-start-column="19" selection-end-line="27" selection-end-column="19"/>
+            <state relative-caret-position="1584">
+              <caret line="66" column="28" selection-start-line="66" selection-start-column="28" selection-end-line="66" selection-end-column="39"/>
               <folding>
                 <element signature="e#0#13#0" expanded="true"/>
               </folding>
             </state>
           </provider>
         </entry>
       </file>
-      <file leaf-file-name="models.py" pinned="false" current-in-tab="true">
-        <entry file="file://$PROJECT_DIR$/src/ord_mediascout_client/models.py">
+      <file leaf-file-name="statistics_test.py" pinned="false" current-in-tab="false">
+        <entry file="file://$PROJECT_DIR$/tests/statistics_test.py">
           <provider selected="true" editor-type-id="text-editor">
-            <state relative-caret-position="-816">
-              <caret line="14" column="31" selection-start-line="14" selection-start-column="31" selection-end-line="14" selection-end-column="31"/>
+            <state relative-caret-position="723">
+              <caret line="55" column="40" lean-forward="true" selection-start-line="55" selection-start-column="40" selection-end-line="55" selection-end-column="40"/>
               <folding>
-                <element signature="e#142#176#0" expanded="true"/>
+                <element signature="e#0#13#0" expanded="true"/>
               </folding>
             </state>
           </provider>
         </entry>
       </file>
-      <file leaf-file-name="client.py" pinned="false" current-in-tab="false">
-        <entry file="file://$PROJECT_DIR$/src/ord_mediascout_client/client.py">
+      <file leaf-file-name="invoice_test.py" pinned="false" current-in-tab="false">
+        <entry file="file://$PROJECT_DIR$/tests/invoice_test.py">
           <provider selected="true" editor-type-id="text-editor">
-            <state relative-caret-position="796">
-              <caret line="96" column="24" selection-start-line="96" selection-start-column="24" selection-end-line="96" selection-end-column="24"/>
+            <state relative-caret-position="360">
+              <caret line="29" column="38" selection-start-line="29" selection-start-column="38" selection-end-line="29" selection-end-column="38"/>
               <folding>
-                <element signature="e#0#38#0" expanded="true"/>
+                <element signature="e#0#13#0" expanded="true"/>
               </folding>
             </state>
           </provider>
         </entry>
       </file>
-      <file leaf-file-name="ping_test.py" pinned="false" current-in-tab="false">
-        <entry file="file://$PROJECT_DIR$/tests/ping_test.py">
+      <file leaf-file-name="client.py" pinned="false" current-in-tab="true">
+        <entry file="file://$PROJECT_DIR$/src/ord_mediascout_client/client.py">
           <provider selected="true" editor-type-id="text-editor">
-            <state relative-caret-position="312">
-              <caret line="13" selection-start-line="13" selection-end-line="13"/>
+            <state relative-caret-position="2026">
+              <caret line="257" column="33" selection-start-line="257" selection-start-column="33" selection-end-line="257" selection-end-column="33"/>
               <folding>
-                <element signature="e#0#13#0" expanded="true"/>
+                <element signature="e#0#38#0" expanded="true"/>
               </folding>
             </state>
           </provider>
         </entry>
       </file>
-      <file leaf-file-name="client_test.py" pinned="false" current-in-tab="false">
-        <entry file="file://$PROJECT_DIR$/tests/client_test.py">
+      <file leaf-file-name="models.py" pinned="false" current-in-tab="false">
+        <entry file="file://$PROJECT_DIR$/src/ord_mediascout_client/models.py">
           <provider selected="true" editor-type-id="text-editor">
-            <state relative-caret-position="336">
-              <caret line="24" column="28" selection-start-line="24" selection-start-column="28" selection-end-line="24" selection-end-column="28"/>
+            <state relative-caret-position="874">
+              <caret line="263" column="31" lean-forward="true" selection-start-line="263" selection-start-column="31" selection-end-line="263" selection-end-column="31"/>
               <folding>
-                <element signature="e#0#13#0" expanded="true"/>
+                <element signature="e#142#176#0" expanded="true"/>
               </folding>
             </state>
           </provider>
         </entry>
       </file>
-      <file leaf-file-name="invoice_test.py" pinned="false" current-in-tab="false">
-        <entry file="file://$PROJECT_DIR$/tests/invoice_test.py">
+      <file leaf-file-name=".env" pinned="false" current-in-tab="false">
+        <entry file="file://$PROJECT_DIR$/scripts/.env">
+          <provider selected="true" editor-type-id="text-editor">
+            <state relative-caret-position="312">
+              <caret line="13" column="23" selection-start-line="13" selection-start-column="23" selection-end-line="13" selection-end-column="23"/>
+            </state>
+          </provider>
+        </entry>
+      </file>
+      <file leaf-file-name=".env" pinned="false" current-in-tab="false">
+        <entry file="file://$PROJECT_DIR$/tests/.env">
           <provider selected="true" editor-type-id="text-editor">
-            <state relative-caret-position="744">
-              <caret line="45" column="19" selection-start-line="45" selection-start-column="19" selection-end-line="45" selection-end-column="19"/>
+            <state relative-caret-position="72">
+              <caret line="3" lean-forward="true" selection-start-line="3" selection-end-line="3"/>
+            </state>
+          </provider>
+        </entry>
+      </file>
+      <file leaf-file-name="__init__.py" pinned="false" current-in-tab="false">
+        <entry file="file://$PROJECT_DIR$/src/ord_mediascout_client/__init__.py">
+          <provider selected="true" editor-type-id="text-editor">
+            <state relative-caret-position="1416">
+              <caret line="59" column="50" selection-start-line="59" selection-start-column="50" selection-end-line="59" selection-end-column="50"/>
               <folding>
-                <element signature="e#0#13#0" expanded="true"/>
+                <element signature="e#1794#1833#0" expanded="true"/>
               </folding>
             </state>
           </provider>
         </entry>
       </file>
-      <file leaf-file-name="pyproject.toml" pinned="false" current-in-tab="false">
-        <entry file="file://$PROJECT_DIR$/pyproject.toml">
+      <file leaf-file-name=".env" pinned="false" current-in-tab="false">
+        <entry file="file://$PROJECT_DIR$/src/ord_mediascout_client/.env">
           <provider selected="true" editor-type-id="text-editor">
             <state relative-caret-position="48">
-              <caret line="2" column="3" selection-start-line="2" selection-start-column="3" selection-end-line="2" selection-end-column="3"/>
+              <caret line="2" column="11" selection-start-line="2" selection-start-column="11" selection-end-line="2" selection-end-column="11"/>
             </state>
           </provider>
         </entry>
       </file>
-      <file leaf-file-name="platform_test.py" pinned="false" current-in-tab="false">
-        <entry file="file://$PROJECT_DIR$/tests/platform_test.py">
+      <file leaf-file-name="ping_test.py" pinned="false" current-in-tab="false">
+        <entry file="file://$PROJECT_DIR$/tests/ping_test.py">
           <provider selected="true" editor-type-id="text-editor">
-            <state relative-caret-position="240">
-              <caret line="10" selection-start-line="10" selection-end-line="10"/>
+            <state relative-caret-position="264">
+              <caret line="13" selection-start-line="13" selection-end-line="13"/>
               <folding>
                 <element signature="e#0#13#0" expanded="true"/>
               </folding>
             </state>
           </provider>
         </entry>
       </file>
-      <file leaf-file-name="main.py" pinned="false" current-in-tab="false">
-        <entry file="file://$PROJECT_DIR$/../kit_project/Envs/OrdMediascoutClientAPI-wpp3x_ga/lib/python3.11/site-packages/pydantic/main.py">
+      <file leaf-file-name="client_test.py" pinned="false" current-in-tab="false">
+        <entry file="file://$PROJECT_DIR$/tests/client_test.py">
           <provider selected="true" editor-type-id="text-editor">
-            <state relative-caret-position="9936">
-              <caret line="484" column="22" selection-start-line="484" selection-start-column="22" selection-end-line="484" selection-end-column="22"/>
+            <state relative-caret-position="336">
+              <caret line="24" column="28" selection-start-line="24" selection-start-column="28" selection-end-line="24" selection-end-column="28"/>
+              <folding>
+                <element signature="e#0#13#0" expanded="true"/>
+              </folding>
             </state>
           </provider>
         </entry>
       </file>
-      <file leaf-file-name="config.py" pinned="false" current-in-tab="false">
-        <entry file="file://$PROJECT_DIR$/src/ord_mediascout_client/config.py">
+      <file leaf-file-name="pyproject.toml" pinned="false" current-in-tab="false">
+        <entry file="file://$PROJECT_DIR$/pyproject.toml">
           <provider selected="true" editor-type-id="text-editor">
-            <state relative-caret-position="264">
-              <caret line="13" column="46" selection-end-line="14"/>
+            <state relative-caret-position="48">
+              <caret line="2" column="3" selection-start-line="2" selection-start-column="3" selection-end-line="2" selection-end-column="3"/>
+            </state>
+          </provider>
+        </entry>
+      </file>
+      <file leaf-file-name="platform_test.py" pinned="false" current-in-tab="false">
+        <entry file="file://$PROJECT_DIR$/tests/platform_test.py">
+          <provider selected="true" editor-type-id="text-editor">
+            <state relative-caret-position="624">
+              <caret line="26" selection-start-line="26" selection-end-line="26"/>
               <folding>
                 <element signature="e#0#13#0" expanded="true"/>
               </folding>
             </state>
           </provider>
         </entry>
       </file>
@@ -147,92 +174,125 @@
       <list>
         <option value="Python Script"/>
       </list>
     </option>
   </component>
   <component name="FindInProjectRecents">
     <findStrings>
-      <find>Invoice</find>
-      <find>Platform</find>
-      <find>CreativeTextDataItemWebApiDto</find>
-      <find>CreateCre</find>
-      <find>CreativeMediaDataItemWebApiDto</find>
-      <find>CreativeS</find>
-      <find>InvoiceInitialContractItemWebApiDto</find>
-      <find>WebApiDto</find>
-      <find>CreateInvoiceWebApiDto</find>
-      <find>Client</find>
-      <find>CreateInitialContractWebApiDto</find>
-      <find>CreatePlatformWebApiDto</find>
-      <find>CounterpartyStatus</find>
-      <find>Severity</find>
-      <find>Enum</find>
-      <find>CreateClientWebApiDto</find>
-      <find>create_outer_contract</find>
-      <find>dict[str, any]</find>
-      <find>test_get_self_promotion_contract</find>
-      <find>def</find>
-      <find>parse_raw_as</find>
-      <find>advertiserUrls</find>
       <find>CreateCreativeWebApiDto</find>
-      <find>EntityIdWebApiDto</find>
-      <find>AdvertiserUrl</find>
       <find>GetCrea</find>
-      <find>GetCreativesWebApiDto</find>
       <find>advertiserUrl</find>
-      <find>CreativeWebApiDto</find>
       <find>capitalize</find>
+      <find>PASSWORD</find>
+      <find>AdvertiserUrl</find>
+      <find>parse_raw_as</find>
+      <find>GetCreativesWebApiDto</find>
+      <find>InvoiceWebApiDto</find>
+      <find>CreateInvoiceWebApiDto</find>
+      <find>EntityIdWebApiDto</find>
+      <find>BadRequestWebApiDto</find>
+      <find>USERNAME</find>
+      <find>BadResponseError</find>
+      <find>case</find>
+      <find>Statistics</find>
+      <find>class CreativeWebApiDto(BaseModel):</find>
+      <find>CreativeWebApiDto</find>
+      <find>CreateStatistics</find>
+      <find>InitialContractWebApiDto</find>
+      <find>CreatedCreativeWebApiDto</find>
+      <find>InvoicelessStatisticsWebApiDto</find>
+      <find>GetInvoicelessPeriodsWebApiDto</find>
+      <find>FinalContractWebApiDto</find>
+      <find>erid</find>
+      <find>IActionResult</find>
+      <find>CreateInvoicelessStatisticsWebApiDto</find>
+      <find>InvoicelessStatisticsByPlatformsItemWebApiDto</find>
+      <find>CreateFinalContractWebApiDto</find>
+      <find>pass</find>
     </findStrings>
+    <dirStrings>
+      <dir>$PROJECT_DIR$</dir>
+    </dirStrings>
   </component>
   <component name="Git.Settings">
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
   </component>
   <component name="IdeDocumentHistory">
     <option name="CHANGED_PATHS">
       <list>
         <option value="$PROJECT_DIR$/tests/ping_test.py"/>
         <option value="$PROJECT_DIR$/tests/client_test.py"/>
-        <option value="$PROJECT_DIR$/tests/invoice_test.py"/>
         <option value="$PROJECT_DIR$/tests/platform_test.py"/>
-        <option value="$PROJECT_DIR$/src/ord_mediascout_client/config.py"/>
         <option value="$PROJECT_DIR$/tests/contract_test.py"/>
         <option value="$PROJECT_DIR$/tests/creative_test.py"/>
+        <option value="$PROJECT_DIR$/Pipfile"/>
+        <option value="$PROJECT_DIR$/scripts/.env"/>
+        <option value="$PROJECT_DIR$/scripts/api_monitor.py"/>
+        <option value="$PROJECT_DIR$/scripts/models_gen.py"/>
+        <option value="$PROJECT_DIR$/tests/.env"/>
+        <option value="$PROJECT_DIR$/src/ord_mediascout_client/config.py"/>
+        <option value="$PROJECT_DIR$/tests/.env.example.env"/>
+        <option value="$PROJECT_DIR$/tests/invoice_test.py"/>
+        <option value="$PROJECT_DIR$/src/ord_mediascout_client/.env"/>
+        <option value="$PROJECT_DIR$/src/ord_mediascout_client/__init__.py"/>
+        <option value="$PROJECT_DIR$/tests/statistics_test.py"/>
         <option value="$PROJECT_DIR$/src/ord_mediascout_client/models.py"/>
         <option value="$PROJECT_DIR$/src/ord_mediascout_client/client.py"/>
-        <option value="$PROJECT_DIR$/Pipfile"/>
       </list>
     </option>
   </component>
   <component name="JsBuildToolGruntFileManager" detection-done="true" sorting="DEFINITION_ORDER"/>
   <component name="JsBuildToolPackageJson" detection-done="true" sorting="DEFINITION_ORDER"/>
   <component name="JsGulpfileManager">
     <detection-done>true</detection-done>
     <sorting>DEFINITION_ORDER</sorting>
   </component>
   <component name="NodePackageJsonFileManager">
     <packageJsonPaths/>
   </component>
   <component name="ProjectFrameBounds" extendedState="6">
-    <option name="x" value="101"/>
-    <option name="y" value="34"/>
+    <option name="x" value="91"/>
+    <option name="y" value="71"/>
     <option name="width" value="3739"/>
-    <option name="height" value="2126"/>
+    <option name="height" value="2089"/>
   </component>
+  <component name="ProjectLevelVcsManager" settingsEditedManually="true"/>
   <component name="ProjectView">
     <navigator proportions="" version="1">
       <foldersAlwaysOnTop value="true"/>
     </navigator>
     <panes>
       <pane id="ProjectPane">
         <subPane>
           <expand>
             <path>
               <item name="OrdMediascoutClientAPI" type="b2602c69:ProjectViewProjectNode"/>
               <item name="OrdMediascoutClientAPI" type="462c0819:PsiDirectoryNode"/>
             </path>
+            <path>
+              <item name="OrdMediascoutClientAPI" type="b2602c69:ProjectViewProjectNode"/>
+              <item name="OrdMediascoutClientAPI" type="462c0819:PsiDirectoryNode"/>
+              <item name="scripts" type="462c0819:PsiDirectoryNode"/>
+            </path>
+            <path>
+              <item name="OrdMediascoutClientAPI" type="b2602c69:ProjectViewProjectNode"/>
+              <item name="OrdMediascoutClientAPI" type="462c0819:PsiDirectoryNode"/>
+              <item name="src" type="462c0819:PsiDirectoryNode"/>
+            </path>
+            <path>
+              <item name="OrdMediascoutClientAPI" type="b2602c69:ProjectViewProjectNode"/>
+              <item name="OrdMediascoutClientAPI" type="462c0819:PsiDirectoryNode"/>
+              <item name="src" type="462c0819:PsiDirectoryNode"/>
+              <item name="ord_mediascout_client" type="462c0819:PsiDirectoryNode"/>
+            </path>
+            <path>
+              <item name="OrdMediascoutClientAPI" type="b2602c69:ProjectViewProjectNode"/>
+              <item name="OrdMediascoutClientAPI" type="462c0819:PsiDirectoryNode"/>
+              <item name="tests" type="462c0819:PsiDirectoryNode"/>
+            </path>
           </expand>
           <select/>
         </subPane>
       </pane>
       <pane id="Scope"/>
     </panes>
   </component>
@@ -271,25 +331,25 @@
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1680273201412</updated>
     </task>
     <servers/>
   </component>
   <component name="ToolWindowManager">
-    <frame x="101" y="34" width="3739" height="2126" extended-state="6"/>
+    <frame x="91" y="71" width="3749" height="2089" extended-state="6"/>
     <editor active="true"/>
     <layout>
       <window_info anchor="bottom" id="TODO" order="6"/>
-      <window_info anchor="bottom" id="Event Log" order="7" sideWeight="0.5025794" side_tool="true" visible="true" weight="0.32971016"/>
+      <window_info active="true" anchor="bottom" id="Event Log" order="7" sideWeight="0.508525" side_tool="true" visible="true" weight="0.32971016"/>
       <window_info anchor="bottom" id="Database Changes" order="7" show_stripe_button="false"/>
-      <window_info anchor="bottom" id="Version Control" order="7" sideWeight="0.49742058" visible="true" weight="0.32971016"/>
+      <window_info anchor="bottom" id="Version Control" order="7" sideWeight="0.49147496" visible="true" weight="0.32971016"/>
       <window_info anchor="bottom" id="Python Console" order="7" sideWeight="0.49986425" weight="0.32953957"/>
       <window_info anchor="bottom" id="Run" order="2"/>
       <window_info anchor="bottom" id="Terminal" order="7" weight="0.45162958"/>
-      <window_info active="true" content_ui="combo" id="Project" order="0" visible="true" weight="0.26663047"/>
+      <window_info content_ui="combo" id="Project" order="0" visible="true" weight="0.3014885"/>
       <window_info anchor="bottom" id="Docker" order="7" sideWeight="0.49986425" weight="0.32953957"/>
       <window_info anchor="right" id="Database" order="3"/>
       <window_info anchor="right" id="SciView" order="3"/>
       <window_info id="Structure" order="1" side_tool="true" weight="0.25"/>
       <window_info id="Favorites" order="2" side_tool="true"/>
       <window_info anchor="bottom" id="Debug" order="3" weight="0.4"/>
       <window_info anchor="right" content_ui="combo" id="Hierarchy" order="2" weight="0.25"/>
@@ -303,89 +363,20 @@
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="1"/>
   </component>
   <component name="VcsContentAnnotationSettings">
     <option name="myLimit" value="2678400000"/>
   </component>
+  <component name="XDebuggerManager">
+    <breakpoint-manager>
+      <option name="time" value="1"/>
+    </breakpoint-manager>
+  </component>
   <component name="editorHistoryManager">
-    <entry file="file://$PROJECT_DIR$/Pipfile">
-      <provider selected="true" editor-type-id="text-editor">
-        <state relative-caret-position="408">
-          <caret line="17" column="10" selection-start-line="17" selection-start-column="10" selection-end-line="17" selection-end-column="10"/>
-        </state>
-      </provider>
-    </entry>
-    <entry file="file://$PROJECT_DIR$/tests/platform_test.py">
-      <provider selected="true" editor-type-id="text-editor">
-        <state relative-caret-position="144">
-          <caret line="10" selection-start-line="10" selection-end-line="10"/>
-          <folding>
-            <element signature="e#0#13#0" expanded="true"/>
-          </folding>
-        </state>
-      </provider>
-    </entry>
-    <entry file="file://$PROJECT_DIR$/tests/creative_test.py">
-      <provider selected="true" editor-type-id="text-editor">
-        <state relative-caret-position="144">
-          <caret line="18" selection-start-line="18" selection-end-line="18"/>
-          <folding>
-            <element signature="e#0#13#0" expanded="true"/>
-          </folding>
-        </state>
-      </provider>
-    </entry>
-    <entry file="file://$PROJECT_DIR$/src/ord_mediascout_client/models.py">
-      <provider selected="true" editor-type-id="text-editor">
-        <state relative-caret-position="12552">
-          <caret line="529" column="28" selection-start-line="529" selection-start-column="28" selection-end-line="529" selection-end-column="28"/>
-          <folding>
-            <element signature="e#142#176#0" expanded="true"/>
-          </folding>
-        </state>
-      </provider>
-    </entry>
-    <entry file="file://$PROJECT_DIR$/../kit_project/Envs/OrdMediascoutClientAPI-wpp3x_ga/lib/python3.11/site-packages/pydantic/main.py">
-      <provider selected="true" editor-type-id="text-editor">
-        <state relative-caret-position="9936">
-          <caret line="484" column="22" selection-start-line="484" selection-start-column="22" selection-end-line="484" selection-end-column="22"/>
-        </state>
-      </provider>
-    </entry>
-    <entry file="file://$PROJECT_DIR$/src/ord_mediascout_client/config.py">
-      <provider selected="true" editor-type-id="text-editor">
-        <state relative-caret-position="264">
-          <caret line="13" column="46" selection-end-line="14"/>
-          <folding>
-            <element signature="e#0#13#0" expanded="true"/>
-          </folding>
-        </state>
-      </provider>
-    </entry>
-    <entry file="file://$PROJECT_DIR$/src/ord_mediascout_client/client.py">
-      <provider selected="true" editor-type-id="text-editor">
-        <state relative-caret-position="912">
-          <caret line="81" column="68" lean-forward="true" selection-start-line="81" selection-start-column="68" selection-end-line="81" selection-end-column="68"/>
-          <folding>
-            <element signature="e#0#38#0" expanded="true"/>
-          </folding>
-        </state>
-      </provider>
-    </entry>
-    <entry file="file://$PROJECT_DIR$/tests/contract_test.py">
-      <provider selected="true" editor-type-id="text-editor">
-        <state relative-caret-position="3264">
-          <caret line="150" column="71" lean-forward="true" selection-start-line="150" selection-start-column="71" selection-end-line="150" selection-end-column="71"/>
-          <folding>
-            <element signature="e#0#13#0" expanded="true"/>
-          </folding>
-        </state>
-      </provider>
-    </entry>
     <entry file="file://$PROJECT_DIR$/tests/ping_test.py">
       <provider selected="true" editor-type-id="text-editor">
         <state relative-caret-position="144">
           <caret line="8" selection-start-line="8" selection-end-line="8"/>
           <folding>
             <element signature="e#0#13#0" expanded="true"/>
           </folding>
@@ -439,17 +430,14 @@
         </state>
       </provider>
     </entry>
     <entry file="file://$PROJECT_DIR$/src/ord_mediascout_client/models.py">
       <provider selected="true" editor-type-id="text-editor">
         <state relative-caret-position="12552">
           <caret line="529" column="28" selection-start-line="529" selection-start-column="28" selection-end-line="529" selection-end-column="28"/>
-          <folding>
-            <element signature="e#142#176#0" expanded="true"/>
-          </folding>
         </state>
       </provider>
     </entry>
     <entry file="file://$PROJECT_DIR$/../kit_project/Envs/OrdMediascoutClientAPI-wpp3x_ga/lib/python3.11/site-packages/pydantic/main.py">
       <provider selected="true" editor-type-id="text-editor">
         <state relative-caret-position="9936">
           <caret line="484" column="22" selection-start-line="484" selection-start-column="22" selection-end-line="484" selection-end-column="22"/>
@@ -466,17 +454,14 @@
         </state>
       </provider>
     </entry>
     <entry file="file://$PROJECT_DIR$/src/ord_mediascout_client/client.py">
       <provider selected="true" editor-type-id="text-editor">
         <state relative-caret-position="1488">
           <caret line="105" column="33" lean-forward="true" selection-start-line="105" selection-start-column="33" selection-end-line="105" selection-end-column="33"/>
-          <folding>
-            <element signature="e#0#38#0" expanded="true"/>
-          </folding>
         </state>
       </provider>
     </entry>
     <entry file="file://$PROJECT_DIR$/tests/contract_test.py">
       <provider selected="true" editor-type-id="text-editor">
         <state relative-caret-position="144">
           <caret line="20" selection-start-line="20" selection-end-line="20"/>
@@ -543,17 +528,14 @@
         </state>
       </provider>
     </entry>
     <entry file="file://$PROJECT_DIR$/src/ord_mediascout_client/models.py">
       <provider selected="true" editor-type-id="text-editor">
         <state relative-caret-position="12552">
           <caret line="529" column="28" lean-forward="true" selection-start-line="529" selection-start-column="28" selection-end-line="529" selection-end-column="28"/>
-          <folding>
-            <element signature="e#142#176#0" expanded="true"/>
-          </folding>
         </state>
       </provider>
     </entry>
     <entry file="file://$PROJECT_DIR$/../kit_project/Envs/OrdMediascoutClientAPI-wpp3x_ga/lib/python3.11/site-packages/pydantic/main.py">
       <provider selected="true" editor-type-id="text-editor">
         <state relative-caret-position="9936">
           <caret line="484" column="22" selection-start-line="484" selection-start-column="22" selection-end-line="484" selection-end-column="22"/>
@@ -570,17 +552,14 @@
         </state>
       </provider>
     </entry>
     <entry file="file://$PROJECT_DIR$/src/ord_mediascout_client/client.py">
       <provider selected="true" editor-type-id="text-editor">
         <state relative-caret-position="1584">
           <caret line="110" column="44" lean-forward="true" selection-start-line="110" selection-start-column="44" selection-end-line="110" selection-end-column="44"/>
-          <folding>
-            <element signature="e#0#38#0" expanded="true"/>
-          </folding>
         </state>
       </provider>
     </entry>
     <entry file="file://$PROJECT_DIR$/tests/contract_test.py">
       <provider selected="true" editor-type-id="text-editor">
         <state relative-caret-position="552">
           <caret line="23" column="22" selection-start-line="23" selection-start-column="22" selection-end-line="23" selection-end-column="22"/>
@@ -597,17 +576,14 @@
         </state>
       </provider>
     </entry>
     <entry file="file://$PROJECT_DIR$/src/ord_mediascout_client/client.py">
       <provider selected="true" editor-type-id="text-editor">
         <state relative-caret-position="1152">
           <caret line="91" column="29" selection-start-line="91" selection-start-column="29" selection-end-line="91" selection-end-column="29"/>
-          <folding>
-            <element signature="e#0#38#0" expanded="true"/>
-          </folding>
         </state>
       </provider>
     </entry>
     <entry file="file://$PROJECT_DIR$/src/ord_mediascout_client/config.py">
       <provider selected="true" editor-type-id="text-editor">
         <state relative-caret-position="216">
           <caret line="11" column="22" lean-forward="true" selection-start-line="11" selection-start-column="22" selection-end-line="11" selection-end-column="22"/>
@@ -626,144 +602,210 @@
           </folding>
         </state>
       </provider>
     </entry>
     <entry file="file://$PROJECT_DIR$/tests/__init__.py">
       <provider selected="true" editor-type-id="text-editor"/>
     </entry>
-    <entry file="file://$PROJECT_DIR$/src/ord_mediascout_client/.env">
-      <provider selected="true" editor-type-id="text-editor"/>
+    <entry file="file://$PROJECT_DIR$/../kit_project/Envs/OrdMediascoutClientAPI-wpp3x_ga/lib/python3.11/site-packages/pydantic/env_settings.py">
+      <provider selected="true" editor-type-id="text-editor">
+        <state relative-caret-position="288">
+          <caret line="21" column="6" selection-start-line="21" selection-start-column="6" selection-end-line="21" selection-end-column="6"/>
+        </state>
+      </provider>
     </entry>
-    <entry file="file://$PROJECT_DIR$/src/ord_mediascout_client/__init__.py">
+    <entry file="file://$APPLICATION_HOME_DIR$/helpers/typeshed/stdlib/3/builtins.pyi">
       <provider selected="true" editor-type-id="text-editor">
-        <state relative-caret-position="4200">
-          <caret line="175" column="28" lean-forward="true" selection-start-line="175" selection-start-column="28" selection-end-line="175" selection-end-column="28"/>
+        <state relative-caret-position="422">
+          <caret line="937" column="6" selection-start-line="937" selection-start-column="6" selection-end-line="937" selection-end-column="6"/>
         </state>
       </provider>
     </entry>
-    <entry file="file://$PROJECT_DIR$/../kit_project/Envs/OrdMediascoutClientAPI-wpp3x_ga/lib/python3.11/site-packages/pydantic/env_settings.py">
+    <entry file="file://$PROJECT_DIR$/tests/client_test.py">
       <provider selected="true" editor-type-id="text-editor">
-        <state relative-caret-position="288">
-          <caret line="21" column="6" selection-start-line="21" selection-start-column="6" selection-end-line="21" selection-end-column="6"/>
+        <state relative-caret-position="336">
+          <caret line="24" column="28" selection-start-line="24" selection-start-column="28" selection-end-line="24" selection-end-column="28"/>
+          <folding>
+            <element signature="e#0#13#0" expanded="true"/>
+          </folding>
         </state>
       </provider>
     </entry>
-    <entry file="file://$PROJECT_DIR$/src/ord_mediascout_client/config.py">
+    <entry file="file://$PROJECT_DIR$/tests/ping_test.py">
       <provider selected="true" editor-type-id="text-editor">
         <state relative-caret-position="264">
-          <caret line="13" column="46" selection-end-line="14"/>
+          <caret line="13" selection-start-line="13" selection-end-line="13"/>
           <folding>
             <element signature="e#0#13#0" expanded="true"/>
           </folding>
         </state>
       </provider>
     </entry>
-    <entry file="file://$APPLICATION_HOME_DIR$/helpers/typeshed/stdlib/3/builtins.pyi">
+    <entry file="file://$PROJECT_DIR$/Pipfile">
       <provider selected="true" editor-type-id="text-editor">
-        <state relative-caret-position="422">
-          <caret line="937" column="6" selection-start-line="937" selection-start-column="6" selection-end-line="937" selection-end-column="6"/>
+        <state relative-caret-position="216">
+          <caret line="9" lean-forward="true" selection-start-line="9" selection-end-line="9"/>
+        </state>
+      </provider>
+    </entry>
+    <entry file="file:///usr/lib/python3.10/difflib.py">
+      <provider selected="true" editor-type-id="text-editor">
+        <state relative-caret-position="24">
+          <caret line="1704" column="8" selection-start-line="1704" selection-start-column="8" selection-end-line="1704" selection-end-column="8"/>
+        </state>
+      </provider>
+    </entry>
+    <entry file="file:///usr/lib/python3.10/smtplib.py">
+      <provider selected="true" editor-type-id="text-editor">
+        <state relative-caret-position="421">
+          <caret line="807" column="8" selection-start-line="807" selection-start-column="8" selection-end-line="807" selection-end-column="8"/>
+        </state>
+      </provider>
+    </entry>
+    <entry file="file://$PROJECT_DIR$/scripts/api_monitor.py">
+      <provider selected="true" editor-type-id="text-editor">
+        <state relative-caret-position="672">
+          <caret line="28" column="56" selection-start-line="28" selection-start-column="36" selection-end-line="28" selection-end-column="56"/>
+        </state>
+      </provider>
+    </entry>
+    <entry file="file://$PROJECT_DIR$/pyproject.toml">
+      <provider selected="true" editor-type-id="text-editor">
+        <state relative-caret-position="48">
+          <caret line="2" column="3" selection-start-line="2" selection-start-column="3" selection-end-line="2" selection-end-column="3"/>
         </state>
       </provider>
     </entry>
     <entry file="file://$PROJECT_DIR$/../kit_project/Envs/OrdMediascoutClientAPI-wpp3x_ga/lib/python3.11/site-packages/pydantic/main.py">
       <provider selected="true" editor-type-id="text-editor">
-        <state relative-caret-position="9936">
+        <state relative-caret-position="7598">
           <caret line="484" column="22" selection-start-line="484" selection-start-column="22" selection-end-line="484" selection-end-column="22"/>
         </state>
       </provider>
     </entry>
-    <entry file="file://$PROJECT_DIR$/tests/client_test.py">
+    <entry file="file://$PROJECT_DIR$/tests/invoice_test.py">
       <provider selected="true" editor-type-id="text-editor">
-        <state relative-caret-position="336">
-          <caret line="24" column="28" selection-start-line="24" selection-start-column="28" selection-end-line="24" selection-end-column="28"/>
+        <state relative-caret-position="360">
+          <caret line="29" column="38" selection-start-line="29" selection-start-column="38" selection-end-line="29" selection-end-column="38"/>
           <folding>
             <element signature="e#0#13#0" expanded="true"/>
           </folding>
         </state>
       </provider>
     </entry>
-    <entry file="file://$PROJECT_DIR$/tests/platform_test.py">
+    <entry file="file://$PROJECT_DIR$/src/ord_mediascout_client/config.py">
       <provider selected="true" editor-type-id="text-editor">
-        <state relative-caret-position="240">
-          <caret line="10" selection-start-line="10" selection-end-line="10"/>
+        <state relative-caret-position="168">
+          <caret line="7" column="6" selection-start-line="7" selection-start-column="6" selection-end-line="7" selection-end-column="6"/>
           <folding>
             <element signature="e#0#13#0" expanded="true"/>
           </folding>
         </state>
       </provider>
     </entry>
-    <entry file="file://$PROJECT_DIR$/tests/ping_test.py">
+    <entry file="file://$PROJECT_DIR$/tests/.env.example.env">
+      <provider selected="true" editor-type-id="text-editor">
+        <state relative-caret-position="72">
+          <caret line="3" selection-start-line="3" selection-end-line="3"/>
+        </state>
+      </provider>
+    </entry>
+    <entry file="file://$PROJECT_DIR$/scripts/models_gen.py">
+      <provider selected="true" editor-type-id="text-editor">
+        <state relative-caret-position="925">
+          <caret line="39" column="21" selection-start-line="39" selection-start-column="21" selection-end-line="39" selection-end-column="21"/>
+        </state>
+      </provider>
+    </entry>
+    <entry file="file://$PROJECT_DIR$/src/ord_mediascout_client/.env">
+      <provider selected="true" editor-type-id="text-editor">
+        <state relative-caret-position="48">
+          <caret line="2" column="11" selection-start-line="2" selection-start-column="11" selection-end-line="2" selection-end-column="11"/>
+        </state>
+      </provider>
+    </entry>
+    <entry file="file://$PROJECT_DIR$/scripts/.env">
       <provider selected="true" editor-type-id="text-editor">
         <state relative-caret-position="312">
-          <caret line="13" selection-start-line="13" selection-end-line="13"/>
-          <folding>
-            <element signature="e#0#13#0" expanded="true"/>
-          </folding>
+          <caret line="13" column="23" selection-start-line="13" selection-start-column="23" selection-end-line="13" selection-end-column="23"/>
         </state>
       </provider>
     </entry>
-    <entry file="file://$PROJECT_DIR$/tests/contract_test.py">
+    <entry file="file://$PROJECT_DIR$/tests/.env">
+      <provider selected="true" editor-type-id="text-editor">
+        <state relative-caret-position="72">
+          <caret line="3" lean-forward="true" selection-start-line="3" selection-end-line="3"/>
+        </state>
+      </provider>
+    </entry>
+    <entry file="file://$PROJECT_DIR$/tests/platform_test.py">
       <provider selected="true" editor-type-id="text-editor">
-        <state relative-caret-position="-2469">
-          <caret line="22" selection-start-line="22" selection-end-line="22"/>
+        <state relative-caret-position="624">
+          <caret line="26" selection-start-line="26" selection-end-line="26"/>
           <folding>
             <element signature="e#0#13#0" expanded="true"/>
           </folding>
         </state>
       </provider>
     </entry>
-    <entry file="file://$PROJECT_DIR$/src/ord_mediascout_client/client.py">
+    <entry file="file://$PROJECT_DIR$/tests/contract_test.py">
       <provider selected="true" editor-type-id="text-editor">
-        <state relative-caret-position="796">
-          <caret line="96" column="24" selection-start-line="96" selection-start-column="24" selection-end-line="96" selection-end-column="24"/>
+        <state relative-caret-position="675">
+          <caret line="108" column="18" selection-start-line="108" selection-start-column="18" selection-end-line="108" selection-end-column="18"/>
           <folding>
-            <element signature="e#0#38#0" expanded="true"/>
+            <element signature="e#0#13#0" expanded="true"/>
           </folding>
         </state>
       </provider>
     </entry>
     <entry file="file://$PROJECT_DIR$/tests/creative_test.py">
       <provider selected="true" editor-type-id="text-editor">
-        <state relative-caret-position="648">
-          <caret line="27" column="19" selection-start-line="27" selection-start-column="19" selection-end-line="27" selection-end-column="19"/>
+        <state relative-caret-position="1584">
+          <caret line="66" column="28" selection-start-line="66" selection-start-column="28" selection-end-line="66" selection-end-column="39"/>
           <folding>
             <element signature="e#0#13#0" expanded="true"/>
           </folding>
         </state>
       </provider>
     </entry>
-    <entry file="file://$PROJECT_DIR$/Pipfile">
+    <entry file="file://$PROJECT_DIR$/src/ord_mediascout_client/__init__.py">
       <provider selected="true" editor-type-id="text-editor">
-        <state relative-caret-position="216">
-          <caret line="9" lean-forward="true" selection-start-line="9" selection-end-line="9"/>
+        <state relative-caret-position="1416">
+          <caret line="59" column="50" selection-start-line="59" selection-start-column="50" selection-end-line="59" selection-end-column="50"/>
+          <folding>
+            <element signature="e#1794#1833#0" expanded="true"/>
+          </folding>
         </state>
       </provider>
     </entry>
-    <entry file="file://$PROJECT_DIR$/tests/invoice_test.py">
+    <entry file="file://$PROJECT_DIR$/tests/statistics_test.py">
       <provider selected="true" editor-type-id="text-editor">
-        <state relative-caret-position="744">
-          <caret line="45" column="19" selection-start-line="45" selection-start-column="19" selection-end-line="45" selection-end-column="19"/>
+        <state relative-caret-position="723">
+          <caret line="55" column="40" lean-forward="true" selection-start-line="55" selection-start-column="40" selection-end-line="55" selection-end-column="40"/>
           <folding>
             <element signature="e#0#13#0" expanded="true"/>
           </folding>
         </state>
       </provider>
     </entry>
-    <entry file="file://$PROJECT_DIR$/pyproject.toml">
+    <entry file="file://$PROJECT_DIR$/src/ord_mediascout_client/models.py">
       <provider selected="true" editor-type-id="text-editor">
-        <state relative-caret-position="48">
-          <caret line="2" column="3" selection-start-line="2" selection-start-column="3" selection-end-line="2" selection-end-column="3"/>
+        <state relative-caret-position="874">
+          <caret line="263" column="31" lean-forward="true" selection-start-line="263" selection-start-column="31" selection-end-line="263" selection-end-column="31"/>
+          <folding>
+            <element signature="e#142#176#0" expanded="true"/>
+          </folding>
         </state>
       </provider>
     </entry>
-    <entry file="file://$PROJECT_DIR$/src/ord_mediascout_client/models.py">
+    <entry file="file://$PROJECT_DIR$/src/ord_mediascout_client/client.py">
       <provider selected="true" editor-type-id="text-editor">
-        <state relative-caret-position="-816">
-          <caret line="14" column="31" selection-start-line="14" selection-start-column="31" selection-end-line="14" selection-end-column="31"/>
+        <state relative-caret-position="2026">
+          <caret line="257" column="33" selection-start-line="257" selection-start-column="33" selection-end-line="257" selection-end-column="33"/>
           <folding>
-            <element signature="e#142#176#0" expanded="true"/>
+            <element signature="e#0#38#0" expanded="true"/>
           </folding>
         </state>
       </provider>
     </entry>
   </component>
 </project>
```

### Comparing `ord_mediascout_client-0.0.8/docs/track_api_changes.md` & `ord_mediascout_client-0.0.9/docs/track_api_changes.md`

 * *Files identical despite different names*

### Comparing `ord_mediascout_client-0.0.8/examples/create_client.py` & `ord_mediascout_client-0.0.9/examples/create_client.py`

 * *Files identical despite different names*

### Comparing `ord_mediascout_client-0.0.8/src/ord_mediascout_client/__init__.py` & `ord_mediascout_client-0.0.9/src/ord_mediascout_client/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,14 +50,19 @@
     'OuterContractWebApiDto',
     'PlatformCardWebApiDto',
     'PlatformType',
     'SelfPromotionContractWebApiDto',
     'Severity',
     'SupplementInvoiceWebApiDto',
     'ValidationFailure',
+    'IActionResult',
+    'GetInvoicelessPeriodsWebApiDto',
+    'InvoicelessStatisticsWebApiDto',
+    'InvoicelessStatisticsByPlatformsItemWebApiDto',
+    'CreateInvoicelessStatisticsWebApiDto',
 ]
 
 from .client import ORDMediascoutClient
 from .config import ORDMediascoutConfig
 from .models import (
     BadRequestWebApiDto,
     ClearInvoiceDataWebApiDto,
@@ -110,8 +115,13 @@
     OuterContractWebApiDto,
     PlatformCardWebApiDto,
     PlatformType,
     SelfPromotionContractWebApiDto,
     Severity,
     SupplementInvoiceWebApiDto,
     ValidationFailure,
+    IActionResult,
+    GetInvoicelessPeriodsWebApiDto,
+    InvoicelessStatisticsWebApiDto,
+    InvoicelessStatisticsByPlatformsItemWebApiDto,
+    CreateInvoicelessStatisticsWebApiDto,
 )
```

### Comparing `ord_mediascout_client-0.0.8/src/ord_mediascout_client/client.py` & `ord_mediascout_client-0.0.9/src/ord_mediascout_client/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 from .config import ORDMediascoutConfig
 from .models import (
     BadRequestWebApiDto,
     ClearInvoiceDataWebApiDto,
     ClientWebApiDto,
     CreateClientWebApiDto,
     CreateCreativeWebApiDto,
+    CreatedCreativeWebApiDto,
     CreateFinalContractWebApiDto,
     CreateInitialContractWebApiDto,
+    CreateInvoicelessStatisticsWebApiDto,
     CreateInvoiceWebApiDto,
     CreateOuterContractWebApiDto,
     CreatePlatformWebApiDto,
     CreativeWebApiDto,
     EditCreativeWebApiDto,
     EditFinalContractWebApiDto,
     EditInitialContractWebApiDto,
@@ -28,17 +30,20 @@
     EditPlatformWebApiDto,
     EntityIdWebApiDto,
     FinalContractWebApiDto,
     GetClientsWebApiDto,
     GetCreativesWebApiDto,
     GetFinalContractsWebApiDto,
     GetInitialContractsWebApiDto,
+    GetInvoicelessPeriodsWebApiDto,
     GetInvoicesWebApiDto,
     GetOuterContractsWebApiDto,
+    IActionResult,
     InitialContractWebApiDto,
+    InvoicelessStatisticsWebApiDto,
     InvoiceSummaryWebApiDto,
     InvoiceWebApiDto,
     OuterContractWebApiDto,
     PlatformCardWebApiDto,
     SelfPromotionContractWebApiDto,
     SupplementInvoiceWebApiDto,
 )
@@ -91,15 +96,15 @@
                     raise UnexpectedResponseError(response) from e
                 raise BadResponseError(response, bad_response)
             case 500:
                 raise BadResponseError(response)
             case 200 | 201:
                 if return_type is not None:
                     try:
-                        return parse_raw_as(return_type, response.text)
+                        return parse_raw_as(return_type, response.text or '{}')
                     except ValidationError as e:
                         raise UnexpectedResponseError(response) from e
             case _:
                 raise UnexpectedResponseError(response)
 
     # Clients
     def create_client(self, client: CreateClientWebApiDto) -> ClientWebApiDto:
@@ -178,18 +183,18 @@
     def get_self_promotion_contracts(self) -> list[SelfPromotionContractWebApiDto]:
         contracts: list[SelfPromotionContractWebApiDto] = self._call(
             'post', '/webapi/Contracts/GetSelfPromotionContracts', None, list[SelfPromotionContractWebApiDto]
         )
         return contracts
 
     # Creatives
-    def create_creative(self, creative: CreateCreativeWebApiDto) -> EntityIdWebApiDto:
-        # entity: EntityIdWebApiDto = self._call('post', '/webapi/creatives/CreateCreative', creative, EntityIdWebApiDto)
-        creative: CreativeWebApiDto = self._call('post', '/webapi/creatives/CreateCreative', creative, CreativeWebApiDto)
-        # return entity
+    def create_creative(self, creative: CreateCreativeWebApiDto) -> CreatedCreativeWebApiDto:
+        creative: CreatedCreativeWebApiDto = self._call(
+            'post', '/webapi/creatives/CreateCreative', creative, CreatedCreativeWebApiDto
+        )
         return creative
 
     def edit_creative(self, creative: EditCreativeWebApiDto) -> CreativeWebApiDto:
         updated_creative: CreativeWebApiDto = self._call(
             'post', '/webapi/creatives/EditCreative', creative, CreativeWebApiDto
         )
         return updated_creative
@@ -244,14 +249,25 @@
 
     def edit_platform(self, platform: EditPlatformWebApiDto) -> PlatformCardWebApiDto:
         updated_platform: PlatformCardWebApiDto = self._call(
             'post', '/webapi/Platforms/EditPlatform', platform, PlatformCardWebApiDto
         )
         return updated_platform
 
+    # Statistics
+    def create_statistics(self, statistics: CreateInvoicelessStatisticsWebApiDto) -> IActionResult:
+        statistics: IActionResult = self._call('post', '/webapi/Statistics/CreateStatistics', statistics, IActionResult)
+        return statistics
+
+    def get_statistics(self, parameters: GetInvoicelessPeriodsWebApiDto) -> list[InvoicelessStatisticsWebApiDto]:
+        statistics: list[InvoicelessStatisticsWebApiDto] = self._call(
+            'post', '/webapi/Statistics/GetStatistics', parameters, list[InvoicelessStatisticsWebApiDto]
+        )
+        return statistics
+
     # PING
     def ping(self) -> bool:
         tmp_auth, self.auth = self.auth, None
         self._call('get', '/webapi/Ping')
         self.auth = tmp_auth
         return True
```

### Comparing `ord_mediascout_client-0.0.8/src/ord_mediascout_client/models.py` & `ord_mediascout_client-0.0.9/src/ord_mediascout_client/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # generated by datamodel-codegen:
 #   filename:  https://demo.mediascout.ru/swagger/v1/swagger.json
-#   timestamp: 2023-04-19T12:32:32+00:00
+#   timestamp: 2023-06-20T14:50:03+00:00
 
 from __future__ import annotations
 
 from datetime import date, datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional
+from uuid import UUID
 
 from pydantic import BaseModel, Extra
 
 
 def capitalize(s: str) -> str:
     return s[0].upper() + s[1:]
 
@@ -27,15 +28,18 @@
 class ClientRelationshipType(Enum):
     DirectClient = 'DirectClient'
     InitialContractClient = 'InitialContractClient'
 
 
 class ContractStatus(Enum):
     Created = 'Created'
+    RegistrationRequired = 'RegistrationRequired'
+    Registering = 'Registering'
     Active = 'Active'
+    RegistrationError = 'RegistrationError'
     Testing = 'Testing'
     Deleted = 'Deleted'
 
 
 class ContractSubjectTypeWebApi(Enum):
     Distribution = 'Distribution'
     OrgDistribution = 'OrgDistribution'
@@ -50,20 +54,25 @@
     AdditionalAgreement = 'AdditionalAgreement'
     SelfPromotionContract = 'SelfPromotionContract'
     VirtualFinalContract = 'VirtualFinalContract'
 
 
 class CounterpartyStatus(Enum):
     Created = 'Created'
+    RegistrationRequired = 'RegistrationRequired'
+    Registering = 'Registering'
     Active = 'Active'
+    RegistrationError = 'RegistrationError'
 
 
 class CreatedCreativeWebApiDto(BaseModel):
     class Config:
         extra = Extra.forbid
+        alias_generator = capitalize
+        allow_population_by_field_name = True
 
     id: Optional[str] = None
     erid: Optional[str] = None
     creativeGroupId: Optional[str] = None
     creativeGroupName: Optional[str] = None
 
 
@@ -89,15 +98,18 @@
     srcUrl: Optional[str] = None
     description: Optional[str] = None
     isArchive: Optional[bool] = None
 
 
 class CreativeStatus(Enum):
     Created = 'Created'
+    RegistrationRequired = 'RegistrationRequired'
+    Registering = 'Registering'
     Active = 'Active'
+    RegistrationError = 'RegistrationError'
 
 
 class CreativeTextDataItemWebApiDto(BaseModel):
     class Config:
         extra = Extra.forbid
         alias_generator = capitalize
         allow_population_by_field_name = True
@@ -108,60 +120,68 @@
 class CreativeType(Enum):
     CPM = 'CPM'
     CPC = 'CPC'
     CPA = 'CPA'
     Other = 'Other'
 
 
-class CreativeWebApiDto(BaseModel):
+class EditCreativeWebApiDto(BaseModel):
     class Config:
         extra = Extra.forbid
         alias_generator = capitalize
         allow_population_by_field_name = True
 
+    id: Optional[str] = None
+    erid: Optional[str] = None
     creativeGroupId: Optional[str] = None
     creativeGroupName: Optional[str] = None
-    finalContractId: Optional[str] = None
-    initialContractId: Optional[str] = None
-    type: Optional[CreativeType] = None
-    form: Optional[CreativeForm] = None
-    advertiserUrl: Optional[str] = None
+    creativeGroupStartDate: Optional[date] = None
+    creativeGroupEndDate: Optional[date] = None
     advertiserUrls: Optional[List[str]] = None
-    description: Optional[str] = None
-    targetAudience: Optional[str] = None
-    isNative: Optional[bool] = None
-    isSocial: Optional[bool] = None
-    okvedCodes: Optional[List[str]] = None
     mediaData: Optional[List[CreativeMediaDataItemWebApiDto]] = None
     textData: Optional[List[CreativeTextDataItemWebApiDto]] = None
-    id: Optional[str] = None
-    erid: Optional[str] = None
-    status: Optional[CreativeStatus] = None
 
 
-class EditCreativeWebApiDto(BaseModel):
+class EntityIdWebApiDto(BaseModel):
     class Config:
         extra = Extra.forbid
         alias_generator = capitalize
         allow_population_by_field_name = True
 
     id: Optional[str] = None
-    erid: Optional[str] = None
-    creativeGroupId: Optional[str] = None
-    creativeGroupName: Optional[str] = None
-    advertiserUrls: Optional[List[str]] = None
 
 
-class EntityIdWebApiDto(BaseModel):
+class ErirRequestType(Enum):
+    First = 'First'
+    Second = 'Second'
+
+
+class ErirValidationErrorWebApiDto(BaseModel):
+    class Config:
+        extra = Extra.forbid
+        alias_generator = capitalize
+        allow_population_by_field_name = True
+
+    stage: Optional[ErirRequestType] = None
+    code: Optional[str] = None
+    message: Optional[str] = None
+    responseDt: Optional[datetime] = None
+
+
+class FiasObjectWebApiDto(BaseModel):
     class Config:
         extra = Extra.forbid
         alias_generator = capitalize
         allow_population_by_field_name = True
 
     id: Optional[str] = None
+    parentId: Optional[str] = None
+    objectGuid: Optional[UUID] = None
+    name: Optional[str] = None
+    fullName: Optional[str] = None
 
 
 class GetClientsWebApiDto(BaseModel):
     class Config:
         extra = Extra.forbid
         alias_generator = capitalize
         allow_population_by_field_name = True
@@ -176,24 +196,28 @@
         extra = Extra.forbid
         alias_generator = capitalize
         allow_population_by_field_name = True
 
     initialContractId: Optional[str] = None
     finalContractId: Optional[str] = None
     creativeGroupName: Optional[str] = None
+    creativeGroupStartDate: Optional[date] = None
+    creativeGroupEndDate: Optional[date] = None
 
 
 class GetCreativesWebApiDto(BaseModel):
     class Config:
         extra = Extra.forbid
         alias_generator = capitalize
         allow_population_by_field_name = True
 
     creativeId: Optional[str] = None
     erid: Optional[str] = None
+    creativeGroupStartDate: Optional[date] = None
+    creativeGroupEndDate: Optional[date] = None
     initialContractId: Optional[str] = None
     initialContractNumber: Optional[str] = None
     finalContractId: Optional[str] = None
     finalContractNumber: Optional[str] = None
     status: Optional[CreativeStatus] = None
 
 
@@ -233,14 +257,23 @@
 
     outerContractId: Optional[str] = None
     status: Optional[ContractStatus] = None
     contractorId: Optional[str] = None
     clientId: Optional[str] = None
 
 
+class IActionResult(BaseModel):
+    pass
+
+    class Config:
+        extra = Extra.forbid
+        alias_generator = capitalize
+        allow_population_by_field_name = True
+
+
 class InvoiceInitialContractItemWebApiDto(BaseModel):
     class Config:
         extra = Extra.forbid
         alias_generator = capitalize
         allow_population_by_field_name = True
 
     initialContractId: Optional[str] = None
@@ -254,18 +287,19 @@
     Rd = 'Rd'
     Ra = 'Ra'
 
 
 class InvoiceStatus(Enum):
     Creating = 'Creating'
     Created = 'Created'
-    Deleted = 'Deleted'
-    Registering = 'Registering'
     RegistrationRequired = 'RegistrationRequired'
+    Registering = 'Registering'
     Active = 'Active'
+    RegistrationError = 'RegistrationError'
+    Deleted = 'Deleted'
 
 
 class InvoiceSummaryWebApiDto(BaseModel):
     class Config:
         extra = Extra.forbid
         alias_generator = capitalize
         allow_population_by_field_name = True
@@ -278,14 +312,60 @@
     creativesCount: Optional[int] = None
     platformsCount: Optional[int] = None
     impsFactCount: Optional[int] = None
     impsPlanCount: Optional[int] = None
     impsAmount: Optional[float] = None
 
 
+class InvoiceWebApiDto(BaseModel):
+    class Config:
+        extra = Extra.forbid
+        alias_generator = capitalize
+        allow_population_by_field_name = True
+
+    id: Optional[str] = None
+    number: Optional[str] = None
+    date: Optional[date] = None
+    contractorRole: Optional[InvoicePartyRole] = None
+    clientRole: Optional[InvoicePartyRole] = None
+    amount: Optional[float] = None
+    vatIncluded: Optional[bool] = None
+    startDate: Optional[date] = None
+    endDate: Optional[date] = None
+    finalContractId: Optional[str] = None
+    status: Optional[InvoiceStatus] = None
+    erirValidationError: Optional[ErirValidationErrorWebApiDto] = None
+
+
+class InvoicelessPeriodStatus(Enum):
+    Creating = 'Creating'
+    RegistrationRequired = 'RegistrationRequired'
+    Registering = 'Registering'
+    Active = 'Active'
+    RegistrationError = 'RegistrationError'
+
+
+class InvoicelessStatisticsWebApiDto(BaseModel):
+    class Config:
+        extra = Extra.forbid
+        alias_generator = capitalize
+        allow_population_by_field_name = True
+
+    id: Optional[str] = None
+    status: Optional[InvoicelessPeriodStatus] = None
+    erirValidationError: Optional[ErirValidationErrorWebApiDto] = None
+    year: Optional[int] = None
+    month: Optional[int] = None
+    amount: Optional[float] = None
+    creativesCount: Optional[int] = None
+    platformsCount: Optional[int] = None
+    impsFactCount: Optional[int] = None
+    impsPlanCount: Optional[int] = None
+
+
 class LegalForm(Enum):
     JuridicalPerson = 'JuridicalPerson'
     IndividualEntrepreneur = 'IndividualEntrepreneur'
     PhysicalPerson = 'PhysicalPerson'
     InternationalJuridicalPerson = 'InternationalJuridicalPerson'
     InternationalPhysicalPerson = 'InternationalPhysicalPerson'
 
@@ -311,14 +391,15 @@
     type: Optional[ContractType] = None
     subjectType: Optional[ContractSubjectTypeWebApi] = None
     actionType: Optional[MediationActionType] = None
     parentMainContractId: Optional[str] = None
     contractorId: Optional[str] = None
     id: Optional[str] = None
     status: Optional[ContractStatus] = None
+    erirValidationError: Optional[ErirValidationErrorWebApiDto] = None
 
 
 class PlatformType(Enum):
     Site = 'Site'
     Application = 'Application'
     InformationSystem = 'InformationSystem'
 
@@ -336,40 +417,52 @@
     isAgentActingForPublisher: Optional[bool] = None
     type: Optional[ContractType] = None
     subjectType: Optional[ContractSubjectTypeWebApi] = None
     actionType: Optional[MediationActionType] = None
     parentMainContractId: Optional[str] = None
     id: Optional[str] = None
     status: Optional[ContractStatus] = None
+    erirValidationError: Optional[ErirValidationErrorWebApiDto] = None
 
 
 class Severity(Enum):
     Error = 'Error'
     Warning = 'Warning'
     Info = 'Info'
 
 
+class TargetAudienceParamsWebApiDto(BaseModel):
+    class Config:
+        extra = Extra.forbid
+        alias_generator = capitalize
+        allow_population_by_field_name = True
+
+    geo: Optional[List[str]] = None
+
+
 class ValidationFailure(BaseModel):
     class Config:
         extra = Extra.forbid
         alias_generator = capitalize
+        allow_population_by_field_name = True
 
     propertyName: Optional[str] = None
     errorMessage: Optional[str] = None
     attemptedValue: Optional[Any] = None
     customState: Optional[Any] = None
     severity: Optional[Severity] = None
     errorCode: Optional[str] = None
     formattedMessagePlaceholderValues: Optional[Dict[str, Any]] = None
 
 
 class BadRequestWebApiDto(BaseModel):
     class Config:
         extra = Extra.forbid
         alias_generator = capitalize
+        allow_population_by_field_name = True
 
     errorType: Optional[str] = None
     errorItems: Optional[List[ValidationFailure]] = None
 
 
 class ClientWebApiDto(BaseModel):
     class Config:
@@ -383,14 +476,15 @@
     name: Optional[str] = None
     mobilePhone: Optional[str] = None
     epayNumber: Optional[str] = None
     regNumber: Optional[str] = None
     oksmNumber: Optional[str] = None
     id: Optional[str] = None
     status: Optional[CounterpartyStatus] = None
+    erirValidationError: Optional[ErirValidationErrorWebApiDto] = None
 
 
 class CreateClientWebApiDto(BaseModel):
     class Config:
         extra = Extra.forbid
         alias_generator = capitalize
         allow_population_by_field_name = True
@@ -407,20 +501,25 @@
 
 class CreateCreativeWebApiDto(BaseModel):
     class Config:
         extra = Extra.forbid
         alias_generator = capitalize
         allow_population_by_field_name = True
 
+    creativeGroupId: Optional[str] = None
+    creativeGroupName: Optional[str] = None
+    creativeGroupStartDate: Optional[date] = None
+    creativeGroupEndDate: Optional[date] = None
     finalContractId: Optional[str] = None
     initialContractId: Optional[str] = None
     type: Optional[CreativeType] = None
     form: Optional[CreativeForm] = None
     advertiserUrls: Optional[List[str]] = None
     description: Optional[str] = None
+    targetAudienceParams: Optional[TargetAudienceParamsWebApiDto] = None
     targetAudience: Optional[str] = None
     isNative: Optional[bool] = None
     isSocial: Optional[bool] = None
     okvedCodes: Optional[List[str]] = None
     mediaData: Optional[List[CreativeMediaDataItemWebApiDto]] = None
     textData: Optional[List[CreativeTextDataItemWebApiDto]] = None
 
@@ -488,31 +587,67 @@
         allow_population_by_field_name = True
 
     name: Optional[str] = None
     type: Optional[PlatformType] = None
     url: Optional[str] = None
     isOwner: Optional[bool] = None
 
+
 class CreativeGroupWebApiDto(BaseModel):
     class Config:
         extra = Extra.forbid
+        alias_generator = capitalize
+        allow_population_by_field_name = True
 
     creativeGroupId: Optional[str] = None
     finalContractId: Optional[str] = None
     initialContractId: Optional[str] = None
     creativeGroupName: Optional[str] = None
+    startDate: Optional[date] = None
+    endDate: Optional[date] = None
     type: Optional[CreativeType] = None
     form: Optional[CreativeForm] = None
     isSocial: Optional[bool] = None
     isNative: Optional[bool] = None
+    targetAudienceParams: Optional[TargetAudienceParamsWebApiDto] = None
     targetAudience: Optional[str] = None
     description: Optional[str] = None
     okvedCodes: Optional[str] = None
 
 
+class CreativeWebApiDto(BaseModel):
+    class Config:
+        extra = Extra.forbid
+        alias_generator = capitalize
+        allow_population_by_field_name = True
+
+    creativeGroupId: Optional[str] = None
+    creativeGroupName: Optional[str] = None
+    creativeGroupStartDate: Optional[date] = None
+    creativeGroupEndDate: Optional[date] = None
+    finalContractId: Optional[str] = None
+    initialContractId: Optional[str] = None
+    type: Optional[CreativeType] = None
+    form: Optional[CreativeForm] = None
+    advertiserUrl: Optional[str] = None
+    advertiserUrls: Optional[List[str]] = None
+    description: Optional[str] = None
+    targetAudienceParams: Optional[TargetAudienceParamsWebApiDto] = None
+    targetAudience: Optional[str] = None
+    isNative: Optional[bool] = None
+    isSocial: Optional[bool] = None
+    okvedCodes: Optional[List[str]] = None
+    mediaData: Optional[List[CreativeMediaDataItemWebApiDto]] = None
+    textData: Optional[List[CreativeTextDataItemWebApiDto]] = None
+    id: Optional[str] = None
+    erid: Optional[str] = None
+    status: Optional[CreativeStatus] = None
+    erirValidationError: Optional[ErirValidationErrorWebApiDto] = None
+
+
 class EditFinalContractWebApiDto(BaseModel):
     class Config:
         extra = Extra.forbid
         alias_generator = capitalize
         allow_population_by_field_name = True
 
     number: Optional[str] = None
@@ -613,14 +748,26 @@
     type: Optional[ContractType] = None
     subjectType: Optional[ContractSubjectTypeWebApi] = None
     actionType: Optional[MediationActionType] = None
     parentMainContractId: Optional[str] = None
     clientId: Optional[str] = None
     id: Optional[str] = None
     status: Optional[ContractStatus] = None
+    erirValidationError: Optional[ErirValidationErrorWebApiDto] = None
+
+
+class GetInvoicelessPeriodsWebApiDto(BaseModel):
+    class Config:
+        extra = Extra.forbid
+        alias_generator = capitalize
+        allow_population_by_field_name = True
+
+    dateStart: Optional[date] = None
+    dateEnd: Optional[date] = None
+    status: Optional[InvoicelessPeriodStatus] = None
 
 
 class GetInvoicesWebApiDto(BaseModel):
     class Config:
         extra = Extra.forbid
         alias_generator = capitalize
         allow_population_by_field_name = True
@@ -649,62 +796,64 @@
     actionType: Optional[MediationActionType] = None
     parentMainContractId: Optional[str] = None
     contractorId: Optional[str] = None
     clientId: Optional[str] = None
     finalContractId: Optional[str] = None
     id: Optional[str] = None
     status: Optional[ContractStatus] = None
+    erirValidationError: Optional[ErirValidationErrorWebApiDto] = None
     contractorInn: Optional[str] = None
     contractorName: Optional[str] = None
     clientInn: Optional[str] = None
     clientName: Optional[str] = None
 
 
 class InvoiceStatisticsByPlatformsItemWebApiDto(BaseModel):
     class Config:
         extra = Extra.forbid
         alias_generator = capitalize
         allow_population_by_field_name = True
 
-    initialContractId: Optional[str] = None
     erid: Optional[str] = None
     platformUrl: Optional[str] = None
     platformName: Optional[str] = None
     platformType: Optional[PlatformType] = None
     platformOwnedByAgency: Optional[bool] = None
     impsPlan: Optional[int] = None
     impsFact: Optional[int] = None
     startDatePlan: Optional[date] = None
     startDateFact: Optional[date] = None
     endDatePlan: Optional[date] = None
     endDateFact: Optional[date] = None
     amount: Optional[float] = None
     price: Optional[float] = None
     vatIncluded: Optional[bool] = None
+    initialContractId: Optional[str] = None
 
 
-class InvoiceWebApiDto(BaseModel):
+class InvoicelessStatisticsByPlatformsItemWebApiDto(BaseModel):
     class Config:
         extra = Extra.forbid
         alias_generator = capitalize
         allow_population_by_field_name = True
 
-    number: Optional[str] = None
-    date: Optional[date] = None
-    contractorRole: Optional[InvoicePartyRole] = None
-    clientRole: Optional[InvoicePartyRole] = None
+    erid: Optional[str] = None
+    platformUrl: Optional[str] = None
+    platformName: Optional[str] = None
+    platformType: Optional[PlatformType] = None
+    platformOwnedByAgency: Optional[bool] = None
+    impsPlan: Optional[int] = None
+    impsFact: Optional[int] = None
+    startDatePlan: Optional[date] = None
+    startDateFact: Optional[date] = None
+    endDatePlan: Optional[date] = None
+    endDateFact: Optional[date] = None
     amount: Optional[float] = None
+    price: Optional[float] = None
     vatIncluded: Optional[bool] = None
-    startDate: Optional[date] = None
-    endDate: Optional[date] = None
-    finalContractId: Optional[str] = None
-    initialContractsData: Optional[List[InvoiceInitialContractItemWebApiDto]] = None
-    statisticsByPlatforms: Optional[List[InvoiceStatisticsByPlatformsItemWebApiDto]] = None
-    id: Optional[str] = None
-    status: Optional[InvoiceStatus] = None
 
 
 class PlatformCardWebApiDto(BaseModel):
     class Config:
         extra = Extra.forbid
         alias_generator = capitalize
         allow_population_by_field_name = True
@@ -742,14 +891,23 @@
     startDate: Optional[date] = None
     endDate: Optional[date] = None
     finalContractId: Optional[str] = None
     initialContractsData: Optional[List[InvoiceInitialContractItemWebApiDto]] = None
     statisticsByPlatforms: Optional[List[InvoiceStatisticsByPlatformsItemWebApiDto]] = None
 
 
+class CreateInvoicelessStatisticsWebApiDto(BaseModel):
+    class Config:
+        extra = Extra.forbid
+        alias_generator = capitalize
+        allow_population_by_field_name = True
+
+    statistics: Optional[List[InvoicelessStatisticsByPlatformsItemWebApiDto]] = None
+
+
 class EditInvoiceStatisticsWebApiDto(BaseModel):
     class Config:
         extra = Extra.forbid
         alias_generator = capitalize
         allow_population_by_field_name = True
 
     id: Optional[str] = None
```

### Comparing `ord_mediascout_client-0.0.8/tests/client_test.py` & `ord_mediascout_client-0.0.9/tests/client_test.py`

 * *Files identical despite different names*

### Comparing `ord_mediascout_client-0.0.8/tests/contract_test.py` & `ord_mediascout_client-0.0.9/tests/contract_test.py`

 * *Files identical despite different names*

### Comparing `ord_mediascout_client-0.0.8/tests/creative_test.py` & `ord_mediascout_client-0.0.9/tests/creative_test.py`

 * *Files identical despite different names*

### Comparing `ord_mediascout_client-0.0.8/tests/invoice_test.py` & `ord_mediascout_client-0.0.9/tests/invoice_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 # НЕ работает в режиме "get or create", только "create" с новым номером, потому number генерится
 def test_create_invoice(client: ORDMediascoutClient) -> None:
     request_data = CreateInvoiceWebApiDto(
         number='INV-{}'.format(random.randrange(11111111, 99999999)),
         date='2023-03-20',
         contractorRole=InvoicePartyRole.Rr,
-        clientRole=InvoicePartyRole.Rd,
+        clientRole=InvoicePartyRole.Ra,
         amount=20000.00,
         vatIncluded=True,
         startDate='2023-03-23',
         endDate='2023-03-23',
         finalContractId='CTiwhIpoQ_F0OEPpKj8vWKGg',
         initialContractsData=[
             InvoiceInitialContractItemWebApiDto(
```

### Comparing `ord_mediascout_client-0.0.8/tests/platform_test.py` & `ord_mediascout_client-0.0.9/tests/platform_test.py`

 * *Files identical despite different names*

### Comparing `ord_mediascout_client-0.0.8/LICENSE.txt` & `ord_mediascout_client-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ord_mediascout_client-0.0.8/README.md` & `ord_mediascout_client-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ord_mediascout_client-0.0.8/pyproject.toml` & `ord_mediascout_client-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ord_mediascout_client"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Alexey Ruzin", email="ruzin@me.com" },
   { name="Ilya Chegodayev", email="lighter97@gmail.com" },
 ]
 description = "API Client for Mediascout ORD"
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `ord_mediascout_client-0.0.8/PKG-INFO` & `ord_mediascout_client-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ord_mediascout_client
-Version: 0.0.8
+Version: 0.0.9
 Summary: API Client for Mediascout ORD
 Project-URL: Homepage, https://github.com/KokocGroup/OrdMediascoutClientAPI
 Project-URL: Bug Tracker, https://github.com/KokocGroup/OrdMediascoutClientAPI/issues
 Author-email: Alexey Ruzin <ruzin@me.com>, Ilya Chegodayev <lighter97@gmail.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

