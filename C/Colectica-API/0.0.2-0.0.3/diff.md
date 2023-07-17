# Comparing `tmp/Colectica_API-0.0.2.tar.gz` & `tmp/Colectica_API-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Colectica_API-0.0.2.tar", last modified: Sun Jun 18 03:29:38 2023, max compression
+gzip compressed data, was "Colectica_API-0.0.3.tar", last modified: Mon Jul 17 22:18:41 2023, max compression
```

## Comparing `Colectica_API-0.0.2.tar` & `Colectica_API-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:29:38.135953 Colectica_API-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:29:38.135953 Colectica_API-0.0.2/Colectica_API.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-18 03:29:38.000000 Colectica_API-0.0.2/Colectica_API.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-18 03:29:38.000000 Colectica_API-0.0.2/Colectica_API.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 03:29:38.000000 Colectica_API-0.0.2/Colectica_API.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-18 03:29:38.000000 Colectica_API-0.0.2/Colectica_API.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-18 03:29:38.000000 Colectica_API-0.0.2/Colectica_API.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-18 03:29:25.000000 Colectica_API-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-18 03:29:38.135953 Colectica_API-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-18 03:29:25.000000 Colectica_API-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:29:38.135953 Colectica_API-0.0.2/colectica_api/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-18 03:29:25.000000 Colectica_API-0.0.2/colectica_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23926 2023-06-18 03:29:25.000000 Colectica_API-0.0.2/colectica_api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    55250 2023-06-18 03:29:25.000000 Colectica_API-0.0.2/colectica_api/colectica.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-18 03:29:25.000000 Colectica_API-0.0.2/colectica_api/test_items.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-18 03:29:25.000000 Colectica_API-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 03:29:38.135953 Colectica_API-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:41.005998 Colectica_API-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:41.005998 Colectica_API-0.0.3/Colectica_API.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-17 22:18:40.000000 Colectica_API-0.0.3/Colectica_API.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-17 22:18:41.000000 Colectica_API-0.0.3/Colectica_API.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:18:40.000000 Colectica_API-0.0.3/Colectica_API.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 22:18:40.000000 Colectica_API-0.0.3/Colectica_API.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-17 22:18:40.000000 Colectica_API-0.0.3/Colectica_API.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-17 22:18:26.000000 Colectica_API-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-17 22:18:41.005998 Colectica_API-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-17 22:18:26.000000 Colectica_API-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:41.005998 Colectica_API-0.0.3/colectica_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-17 22:18:26.000000 Colectica_API-0.0.3/colectica_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28108 2023-07-17 22:18:26.000000 Colectica_API-0.0.3/colectica_api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55927 2023-07-17 22:18:26.000000 Colectica_API-0.0.3/colectica_api/colectica.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-17 22:18:26.000000 Colectica_API-0.0.3/colectica_api/test_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-17 22:18:26.000000 Colectica_API-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 22:18:41.005998 Colectica_API-0.0.3/setup.cfg
```

### Comparing `Colectica_API-0.0.2/LICENSE` & `Colectica_API-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Colectica_API-0.0.2/colectica_api/api.py` & `Colectica_API-0.0.3/colectica_api/api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,562 +1,747 @@
 """
-    Colectica API
+Colectica API implementation details.
+
+In most cases you'll want to work with :class:`ColecticaObject` instead.
 """
 
-import requests
 import json
+import os
+
+import requests
 
 
 # item type dictionary
 #   See Item Type Identifiers for a list of identifiers for all item types.
 #   https://docs.colectica.com/repository/technical/item-type-identifiers/
 item_dict = {
-  "Action": "0b70f0ba-602a-4575-a15c-91f0915bae36",
-  "Archive": "ae8ee886-70a2-4c30-a879-b7d92605ba68",
-  "Category": "7e47c269-bcab-40f7-a778-af7bbc4e3d00",
-  "Category Group": "8a3ba89d-70da-4ba1-871a-b41954175453",
-  "Category Set": "1c11de94-a36d-4d80-95dc-950c6f37f624",
-  "ClassificationCorrespondenceTable": "D55A2705-0AB6-464F-92DD-8E78D10269D8",
-  "ClassificationFamily": "020B8B81-2CCD-4F1D-85BA-F724CE1724AC",
-  "ClassificationIndex": "F2C1F48C-A119-4576-9475-607E8E8A8A12",
-  "ClassificationItem": "E96C1674-C4D9-450A-877A-BD37C3060526",
-  "ClassificationLevel": "EF15C75E-FABA-4192-8FB0-19CF7A3436DB",
-  "ClassificationSeries": "3844452A-F213-4296-845A-2FC00835F97A",
-  "Code List Group": "394b9ff3-7248-4ede-b945-9bebdbf56bed",
-  "Code List Set": "4193d389-b5ae-4368-b399-cd5a7ee3653c",
-  "Code Set": "8b108ef8-b642-4484-9c49-f88e4bf7cf1d",
-  "Concept": "48b7d4b4-72bf-470a-a885-720f89bfbc40",
-  "Concept Group": "d38bfe75-60a9-460a-affa-61d643b5416b",
-  "Concept Set": "63c9f58d-1ea3-4239-99cf-e4418ec384c5",
-  "Conceptual Component": "d747d7db-ed2a-4339-a156-127f8786d5ec",
-  "Conceptual Variable": "75f63016-b4f8-45b6-953c-f7ac7364fc25",
-  "Conceptual Variable Group": "dceb4eb2-e7bb-46f8-804d-d9a86aa5ee9f",
-  "Conceptual Variable Set": "ce0f8af6-db9c-4fb3-a31a-e9523fc53668",
-  "Conditional": "2af9a279-89ee-4d06-b2d2-54563a6946ea",
-  "Control Construct Group": "6bcbb890-751d-41e5-a0c9-27d5c951cf93",
-  "Control Construct Set": "ed3801fe-6798-4ea6-808b-73052cc1c633",
-  "Data Collection": "c5084916-9936-47a9-a523-93be9fd816d8",
-  "Data File": "a51e85bb-6259-4488-8df2-f08cb43485f8",
-  "Data Layout": "f39ff278-8500-45fe-a850-3906da2d242b",
-  "DataCollection Methodology": "aa80eb80-c5a9-4215-a59f-4862c6b4009f",
-  "General Instruction": "723052be-35ac-4e63-84c6-743a0a693d85",
-  "Generation Instruction": "eca6afce-0840-421a-beae-d3283fae32b1",
-  "Individual": "1DD920A2-DED8-48B8-B085-D62E49DFC627",
-  "Instruction Group": "89688a09-e125-4b62-997e-18a14df90578",
-  "Instrument": "f196cc07-9c99-4725-ad55-5b34f479cf7d",
-  "Instrument Group": "27540e4f-9a3a-415e-8fb9-83c095dc7bcb",
-  "Instrument Set": "f152ee61-08ba-4fca-8a3a-daf8f87f972e",
-  "Interviewer Instruction": "f53f37b2-6f1b-4af3-b89a-4909d512dfb2",
-  "Interviewer Instruction Set": "5bf598a9-9333-4c84-8c10-46195776800a",
-  "Logical Product": "965c8d28-7d48-4950-bea7-04b27e52bb9b",
-  "Loop": "7482a1bf-fea5-4955-9fc0-f76c053e5b2d",
-  "Managed Representation Group": "68cac1f8-a2a6-49a7-9402-58b8df3d1921",
-  "Managed Representation Set": "16d4d829-41e1-4677-aa17-81190b6a0e66",
-  "MeasurementItem": "CF6FA3D8-3297-42D5-8922-0BA2D4B5C9FF",
-  "MeasurementConstruct": "44CB69AC-062C-4EC2-970B-AF73B42D3CB8",
-  "Metadata Package": "679a61f5-4246-4c89-b482-924dec09af98",
-  "NCube": "b771f5fd-3b29-4f4d-a4f5-6ccae1138c89",
-  "NCube Group": "47172a68-4b16-4f3b-b484-daace3f45bcc",
-  "NCube Set": "31e8515b-c0cc-4e88-9e00-ae4bb6d4ac25",
-  "Organization": "be33a54f-ca93-454f-9164-8c41df6212cb",
-  "Organization Group": "28455ff2-d6a9-4aa3-9c9f-f6b22b55b3a8",
-  "Organization Set": "08ed326a-8043-4da2-ace9-3f5bd19b6196",
-  "OtherMaterial": "EACCE1D3-011D-4980-BD4D-6CCFB9161B43",
-  "OtherMaterialGroup": "E24AFC19-5618-4050-84C7-1A464AF88485",
-  "OtherMaterialScheme": "D19C0898-743A-4AAC-A0ED-7BDF979E5957",
-  "Physical Data Product": "e27aac79-be4a-47d3-96e3-36da178f3923",
-  "Physical Structure": "b89d26c3-c9e1-4720-a6e4-3a1d8cdb10ce",
-  "PhysicalStructure Set": "19273b86-934a-4c2c-9b64-bd2b3bb07acd",
-  "Processing Event": "e99acc19-d127-413d-9cf9-aed786e62055",
-  "Processing Event Group": "a64a0ab6-5bfa-43dd-a3fb-e791f8f28c58",
-  "Processing Event Set": "dc15c74b-9b4a-492e-9ddd-4e02eca9d9d7",
-  "Processing Instruction Group": "c49e2c65-52fb-4948-a454-f3431b834fe7",
-  "Processing Instruction Scheme": "a1a5c54a-3a7b-4dfb-a5fa-46ed8ef465cc",
-  "Project": "f2b9352a-d976-4eac-8ee1-0c76da7cfca4",
-  "Quality Standard": "711e9487-82fd-4682-9309-22e1272bab2c",
-  "Quality Statement": "831a2d3f-7649-485d-90a4-359e2591e1df",
-  "Quality Statement Group": "a60d1016-3d44-4182-bbf7-a5812d817f71",
-  "Quality Statement Set": "4aa7ea9c-495d-4919-95f7-ac107c877f56",
-  "Question": "a1bb19bd-a24a-4443-8728-a6ad80eb42b8",
-  "Question Activity": "f433e43d-29a4-4c25-9610-9dd9819a0519",
-  "Question Block": "12d8f742-0433-4f12-88d1-eb9b77ceced5",
-  "Question Grid": "a1b8a30e-2f35-4056-8467-40e7ed0e7379",
-  "Question Group": "5cc915a1-23c9-4487-9613-779c62f8c205",
-  "Question Set": "0a63fcf6-ffdd-4214-b38c-147d6689d6a1",
-  "RecordLayout": "faddcfca-bedd-450f-9b4e-15c3f2458713",
-  "RecordLayout Set": "8e4d59db-e757-4e94-bb19-1ac72761566e",
-  "Repeat": "3a4e92c0-fd99-4d3f-9b66-471674ab7670",
-  "Represented Variable": "1044459c-8ae2-474a-ad96-6ec18b04953c",
-  "Represented Variable Group": "a8cecef5-4493-47b8-9c83-82a2f1cfb08e",
-  "Represented Variable Set": "14404696-2db3-45ac-a94d-139521de6e21",
-  "Reusable Missing Value": "c29c3125-2a53-4179-8fa6-aa3beb2bb5ed",
-  "Sequence": "df457731-a75c-47c3-aeb4-7969d55aa049",
-  "Series": "4bd6eef6-99df-40e6-9b11-5b8f64e5cb23",
-  "Statement": "4a8b1d85-a508-4b4f-8d56-798219f59689",
-  "StatisticalClassification": "9BACF643-4EF3-452B-8074-D12EE2404704",
-  "Study": "30ea0200-7121-4f01-8d21-a931a182b86d",
-  "SubSeries": "2d57296d-095c-485a-b970-8c63c215c1d0",
-  "UnitType": "897D4AA9-0C26-490B-B25E-F29D9FF721A5",
-  "UnitTypeScheme": "32E1427F-0B88-4FE5-9F2D-5D3EAF585EE8",
-  "UnitTypeGroup": "2B0A0A33-D233-40A3-993B-7CEDA290BC8D",
-  "Universe": "66dfcb67-4915-41ae-9b13-c8ebff6d8e00",
-  "Universe Group": "a80ecd09-7d81-4512-80bb-cdb60f9a95bf",
-  "Universe Set": "101f901a-2c28-4931-88d6-8f80b36d5650",
-  "Variable": "683889c6-f74b-4d5e-92ed-908c0a42bb2d",
-  "Variable Group": "91da6c62-c2c2-4173-8958-22c518d1d40d",
-  "Variable Set": "50907716-b67a-4dcd-8f9f-8a283cb5fee0",
-  "Variable Statistic": "3b438f9f-e039-4eac-a06d-3fa1aedf48bb",
-  "While": "0681e606-ba3f-453c-9fdd-10670e8e045c"
+    "Action": "0b70f0ba-602a-4575-a15c-91f0915bae36",
+    "Archive": "ae8ee886-70a2-4c30-a879-b7d92605ba68",
+    "Category": "7e47c269-bcab-40f7-a778-af7bbc4e3d00",
+    "Category Group": "8a3ba89d-70da-4ba1-871a-b41954175453",
+    "Category Set": "1c11de94-a36d-4d80-95dc-950c6f37f624",
+    "ClassificationCorrespondenceTable": "D55A2705-0AB6-464F-92DD-8E78D10269D8",
+    "ClassificationFamily": "020B8B81-2CCD-4F1D-85BA-F724CE1724AC",
+    "ClassificationIndex": "F2C1F48C-A119-4576-9475-607E8E8A8A12",
+    "ClassificationItem": "E96C1674-C4D9-450A-877A-BD37C3060526",
+    "ClassificationLevel": "EF15C75E-FABA-4192-8FB0-19CF7A3436DB",
+    "ClassificationSeries": "3844452A-F213-4296-845A-2FC00835F97A",
+    "Code List Group": "394b9ff3-7248-4ede-b945-9bebdbf56bed",
+    "Code List Set": "4193d389-b5ae-4368-b399-cd5a7ee3653c",
+    "Code Set": "8b108ef8-b642-4484-9c49-f88e4bf7cf1d",
+    "Concept": "48b7d4b4-72bf-470a-a885-720f89bfbc40",
+    "Concept Group": "d38bfe75-60a9-460a-affa-61d643b5416b",
+    "Concept Set": "63c9f58d-1ea3-4239-99cf-e4418ec384c5",
+    "Conceptual Component": "d747d7db-ed2a-4339-a156-127f8786d5ec",
+    "Conceptual Variable": "75f63016-b4f8-45b6-953c-f7ac7364fc25",
+    "Conceptual Variable Group": "dceb4eb2-e7bb-46f8-804d-d9a86aa5ee9f",
+    "Conceptual Variable Set": "ce0f8af6-db9c-4fb3-a31a-e9523fc53668",
+    "Conditional": "2af9a279-89ee-4d06-b2d2-54563a6946ea",
+    "Control Construct Group": "6bcbb890-751d-41e5-a0c9-27d5c951cf93",
+    "Control Construct Set": "ed3801fe-6798-4ea6-808b-73052cc1c633",
+    "Data Collection": "c5084916-9936-47a9-a523-93be9fd816d8",
+    "Data File": "a51e85bb-6259-4488-8df2-f08cb43485f8",
+    "Data Layout": "f39ff278-8500-45fe-a850-3906da2d242b",
+    "DataCollection Methodology": "aa80eb80-c5a9-4215-a59f-4862c6b4009f",
+    "General Instruction": "723052be-35ac-4e63-84c6-743a0a693d85",
+    "Generation Instruction": "eca6afce-0840-421a-beae-d3283fae32b1",
+    "Individual": "1DD920A2-DED8-48B8-B085-D62E49DFC627",
+    "Instruction Group": "89688a09-e125-4b62-997e-18a14df90578",
+    "Instrument": "f196cc07-9c99-4725-ad55-5b34f479cf7d",
+    "Instrument Group": "27540e4f-9a3a-415e-8fb9-83c095dc7bcb",
+    "Instrument Set": "f152ee61-08ba-4fca-8a3a-daf8f87f972e",
+    "Interviewer Instruction": "f53f37b2-6f1b-4af3-b89a-4909d512dfb2",
+    "Interviewer Instruction Set": "5bf598a9-9333-4c84-8c10-46195776800a",
+    "Logical Product": "965c8d28-7d48-4950-bea7-04b27e52bb9b",
+    "Loop": "7482a1bf-fea5-4955-9fc0-f76c053e5b2d",
+    "Managed Representation Group": "68cac1f8-a2a6-49a7-9402-58b8df3d1921",
+    "Managed Representation Set": "16d4d829-41e1-4677-aa17-81190b6a0e66",
+    "MeasurementItem": "CF6FA3D8-3297-42D5-8922-0BA2D4B5C9FF",
+    "MeasurementConstruct": "44CB69AC-062C-4EC2-970B-AF73B42D3CB8",
+    "Metadata Package": "679a61f5-4246-4c89-b482-924dec09af98",
+    "NCube": "b771f5fd-3b29-4f4d-a4f5-6ccae1138c89",
+    "NCube Group": "47172a68-4b16-4f3b-b484-daace3f45bcc",
+    "NCube Set": "31e8515b-c0cc-4e88-9e00-ae4bb6d4ac25",
+    "Organization": "be33a54f-ca93-454f-9164-8c41df6212cb",
+    "Organization Group": "28455ff2-d6a9-4aa3-9c9f-f6b22b55b3a8",
+    "Organization Set": "08ed326a-8043-4da2-ace9-3f5bd19b6196",
+    "OtherMaterial": "EACCE1D3-011D-4980-BD4D-6CCFB9161B43",
+    "OtherMaterialGroup": "E24AFC19-5618-4050-84C7-1A464AF88485",
+    "OtherMaterialScheme": "D19C0898-743A-4AAC-A0ED-7BDF979E5957",
+    "Physical Data Product": "e27aac79-be4a-47d3-96e3-36da178f3923",
+    "Physical Structure": "b89d26c3-c9e1-4720-a6e4-3a1d8cdb10ce",
+    "PhysicalStructure Set": "19273b86-934a-4c2c-9b64-bd2b3bb07acd",
+    "Processing Event": "e99acc19-d127-413d-9cf9-aed786e62055",
+    "Processing Event Group": "a64a0ab6-5bfa-43dd-a3fb-e791f8f28c58",
+    "Processing Event Set": "dc15c74b-9b4a-492e-9ddd-4e02eca9d9d7",
+    "Processing Instruction Group": "c49e2c65-52fb-4948-a454-f3431b834fe7",
+    "Processing Instruction Scheme": "a1a5c54a-3a7b-4dfb-a5fa-46ed8ef465cc",
+    "Project": "f2b9352a-d976-4eac-8ee1-0c76da7cfca4",
+    "Quality Standard": "711e9487-82fd-4682-9309-22e1272bab2c",
+    "Quality Statement": "831a2d3f-7649-485d-90a4-359e2591e1df",
+    "Quality Statement Group": "a60d1016-3d44-4182-bbf7-a5812d817f71",
+    "Quality Statement Set": "4aa7ea9c-495d-4919-95f7-ac107c877f56",
+    "Question": "a1bb19bd-a24a-4443-8728-a6ad80eb42b8",
+    "Question Activity": "f433e43d-29a4-4c25-9610-9dd9819a0519",
+    "Question Block": "12d8f742-0433-4f12-88d1-eb9b77ceced5",
+    "Question Grid": "a1b8a30e-2f35-4056-8467-40e7ed0e7379",
+    "Question Group": "5cc915a1-23c9-4487-9613-779c62f8c205",
+    "Question Set": "0a63fcf6-ffdd-4214-b38c-147d6689d6a1",
+    "RecordLayout": "faddcfca-bedd-450f-9b4e-15c3f2458713",
+    "RecordLayout Set": "8e4d59db-e757-4e94-bb19-1ac72761566e",
+    "Repeat": "3a4e92c0-fd99-4d3f-9b66-471674ab7670",
+    "Represented Variable": "1044459c-8ae2-474a-ad96-6ec18b04953c",
+    "Represented Variable Group": "a8cecef5-4493-47b8-9c83-82a2f1cfb08e",
+    "Represented Variable Set": "14404696-2db3-45ac-a94d-139521de6e21",
+    "Reusable Missing Value": "c29c3125-2a53-4179-8fa6-aa3beb2bb5ed",
+    "Sequence": "df457731-a75c-47c3-aeb4-7969d55aa049",
+    "Series": "4bd6eef6-99df-40e6-9b11-5b8f64e5cb23",
+    "Statement": "4a8b1d85-a508-4b4f-8d56-798219f59689",
+    "StatisticalClassification": "9BACF643-4EF3-452B-8074-D12EE2404704",
+    "Study": "30ea0200-7121-4f01-8d21-a931a182b86d",
+    "SubSeries": "2d57296d-095c-485a-b970-8c63c215c1d0",
+    "UnitType": "897D4AA9-0C26-490B-B25E-F29D9FF721A5",
+    "UnitTypeScheme": "32E1427F-0B88-4FE5-9F2D-5D3EAF585EE8",
+    "UnitTypeGroup": "2B0A0A33-D233-40A3-993B-7CEDA290BC8D",
+    "Universe": "66dfcb67-4915-41ae-9b13-c8ebff6d8e00",
+    "Universe Group": "a80ecd09-7d81-4512-80bb-cdb60f9a95bf",
+    "Universe Set": "101f901a-2c28-4931-88d6-8f80b36d5650",
+    "Variable": "683889c6-f74b-4d5e-92ed-908c0a42bb2d",
+    "Variable Group": "91da6c62-c2c2-4173-8958-22c518d1d40d",
+    "Variable Set": "50907716-b67a-4dcd-8f9f-8a283cb5fee0",
+    "Variable Statistic": "3b438f9f-e039-4eac-a06d-3fa1aedf48bb",
+    "While": "0681e606-ba3f-453c-9fdd-10670e8e045c",
 }
 
-item_dict_inv = {v:k for k,v in item_dict.items()} 
+item_dict_inv = {v: k for k, v in item_dict.items()}
 
 
 def get_jwtToken(hostname, username, password):
     """
-        First obtain a JWT access token
-        documented at https://docs.colectica.com/portal/technical/deployment/local-jwt-provider/#usage
+    First obtain a JWT access token
+    documented at https://docs.colectica.com/portal/technical/deployment/local-jwt-provider/#usage
     """
     tokenEndpoint = "https://" + hostname + "/token/createtoken"
-    response = requests.post(tokenEndpoint, json={'username': username, 'password': password}, allow_redirects=True, verify=False)
+    response = requests.post(
+        tokenEndpoint,
+        json={"username": username, "password": password},
+        allow_redirects=True,
+        verify=False,
+    )
 
     if response.ok is not True:
         print("Could not get token. Status code: ", response.status_code)
         quit()
 
     jsonResponse = response.json()
     jwtToken = jsonResponse["access_token"]
-    tokenHeader = {'Authorization': 'Bearer ' + jwtToken}
+    tokenHeader = {"Authorization": "Bearer " + jwtToken}
 
     # get Repository information
-    #response = requests.get("https://"+self.host+"/api/v1/repository/info", headers=tokenHeader, verify=False)
+    # response = requests.get("https://"+self.host+"/api/v1/repository/info", headers=tokenHeader, verify=False)
     return tokenHeader
 
 
-class ColecticaLowLevelAPI():
+class ColecticaBasicAPI:
     """Acts as a frontend to a Colectica portal.
 
-    You can then make API calls to this.  It caches authentication credentials, etc.
+    This object communicates with a Colectica server.  In most cases, it can
+    use the newer JSON-based api but still has a deprecated implementation of
+    the older XML-based api.  The latter involves a lot of manual parsing of
+    data.
+
+    You make a new ColecticaBasicAPI by using:
+
+    >>> C = ColecticaBasicAPI(hostname, username, password)
+
+    If `hostname`, `username` or `password` are omitted, environment
+    variables `COLECTICA_HOSTNAME`, `COLECTICA_USERNAME` and `COLECTICA_PASSWORD`
+    will be used, if they are defined.
     """
-    def __init__(self, hostname, username, password):
+
+    def __init__(self, hostname=None, username=None, password=None):
+        if hostname is None:
+            hostname = os.environ.get("COLECTICA_HOSTNAME")
+        if username is None:
+            username = os.environ.get("COLECTICA_USERNAME")
+        if password is None:
+            password = os.environ.get("COLECTICA_PASSWORD")
+        print(f"Connecting to {hostname} as user {username}")
         self.host = hostname
         self.token = get_jwtToken(hostname, username, password)
 
     @classmethod
     def item_code(self, item):
         return item_dict[item]
 
     @classmethod
     def item_code_inv(self, item_type_id):
         return item_dict_inv[item_type_id]
 
     def get_item_xml(self, AgencyId, Identifier, *, version=None):
-        """
-        This request retrieves an item based on known identification information.
-        https://docs.colectica.com/repository/functionality/rest-api/examples/get-item/
-        Request Type: GET
-        URL: /api/v1/item/agenct/Id
+        """Gets an item
+
+        Frontend to Colectica GET: /api/v1/item/{agency}/{id}
+
+        https://docs.colectica.com/portal/technical/api/v1/#tag/Item
 
         Args:
             AgencyId (str):
             Identifier (str):
 
         Keyword Args:
             version (None/int): If omitted we get latest item or you can specify
                 a particular version.
 
+        Returns:
+            dict: with "Item" itself is in xml format
+
         Exceptions:
             ValueError: the request did not succeed.
         """
-        uri = "https://"+self.host+"/api/v1/item/"+AgencyId+"/"+Identifier
+        uri = "https://" + self.host + "/api/v1/item/" + AgencyId + "/" + Identifier
         # use explicit None check so that zero treated
         if version is not None:
             uri += f"/{version}"
         response = requests.get(uri, headers=self.token, verify=False)
         if not response.ok:
             raise ValueError(response.text)
         return response.json()
 
-
     def get_item_json(self, AgencyId, Identifier, *, version=None):
-        """
-        This request retrieves an item based on known identification information.
-        https://docs.colectica.com/repository/functionality/rest-api/examples/get-item/
-        Request Type: GET
-        URL: /api/v1/item/agenct/Id
+        """Gets an item
+
+        Frontend to Colectica GET: /api/v1/json/{agency}/{id}
+
+        https://docs.colectica.com/portal/technical/api/v1/#tag/Item
 
         Args:
             AgencyId (str):
             Identifier (str):
 
         Keyword Args:
             version (None/int): If omitted we get latest item or you can specify
                 a particular version.
 
+        Returns:
+            dict:
+
+
         Exceptions:
             ValueError: the request did not succeed.
         """
-        uri = "https://"+self.host+"/api/v1/json/"+AgencyId+"/"+Identifier
+
+        uri = "https://" + self.host + "/api/v1/json/" + AgencyId + "/" + Identifier
         # use explicit None check so that zero treated
         if version is not None:
             uri += f"/{version}"
         response = requests.get(uri, headers=self.token, verify=False)
         if not response.ok:
             raise ValueError(response.text)
         return response.json()
 
-
     # backwards compatibility for old calls without a warning
     # get_an_item = get_item_xml
 
     def get_an_item(self, *args, **kwargs):
-        print("Warning: this is a deprecated function: use get_item_json or get_item_xml instead")
+        print(
+            "Warning: this is a deprecated function: use get_item_json or get_item_xml instead"
+        )
         return self.get_item_xml(*args, **kwargs)
 
+    def get_item_jsonset(self, AgencyId, Identifier, *, version=None):
+        """Gets an item
 
-    def get_an_item_jsonset(self, AgencyId, Identifier):
-        """
-        This request retrieves the lastest version of an item based on known identification information.
-        https://docs.colectica.com/portal/api/examples/get-item/
-        Request Type: GET
-        URL: /api/v1/item/agenct/Id
-        """
-        response = requests.get("https://"+self.host+"/api/v1/jsonset/"+AgencyId+"/"+Identifier, headers=self.token, verify=False)
-        if response.ok:
-            if response.json() != []:
-                return response.json()
+        Frontend to Colectica GET: /api/v1/jsonset/{agency}/{id}
 
+        https://docs.colectica.com/portal/technical/api/v1/#tag/Item
 
-    def general_search(self, item_type, search_term, MaxResults=1, RankResults=True, SearchDepricatedItems=False, SearchLatestVersion=True):
-        """
-            Perform a general search: https://docs.colectica.com/portal/api/examples/search/
-            Request Type: POST
-            URL: /api/v1/_query
-        """
-        # MaxResults=0 returns all results
-        jsonquery =  {
-             "Cultures": [
-                 "en-US"
-             ],
-             "ItemTypes": [
-                 item_type
-             ],
-             "LanguageSortOrder": [
-                 "en-US"
-             ],
-             "MaxResults": MaxResults,
-             "RankResults": RankResults,
-             "ResultOffset": 0,
-             "ResultOrdering": "None",
-             "SearchDepricatedItems": SearchDepricatedItems,
-             "SearchTerms": [
-                 search_term
-             ],
-             "SearchLatestVersion": SearchLatestVersion
-         }
+        Args:
+            AgencyId (str):
+            Identifier (str):
 
-        response = requests.post("https://"+self.host+"/api/v1/_query/", headers=self.token, json=jsonquery, verify=False)
-        if response.ok:
-            return response.json()
+        Keyword Args:
+            version (None/int): If omitted we get latest item or you can specify
+                a particular version.
 
+        Returns:
+            dict: with set infomation
 
-    def relationship_search(self, item_type, AgencyId, Identifier, UseDistinctResultItem=True, UseDistinctTargetItem=True):
-        """
-            Option 1: retrieve identifiers only
-            https://docs.colectica.com/portal/api/examples/relationship-search/
-            Request Type: POST
-            URL: /api/v1/_query/relationship/bysubject
+        Exceptions:
+            ValueError: the request did not succeed.
         """
 
-        jsonquery = {
-             "ItemTypes": [
-                 item_type
-             ],
-             "TargetItem": {
-                 "AgencyId": AgencyId,
-                 "Identifier": Identifier,
-                 "Version": 1
-             },
-             "UseDistinctResultItem": UseDistinctResultItem,
-             "UseDistinctTargetItem": UseDistinctTargetItem
-        }
+        uri = "https://" + self.host + "/api/v1/jsonset/" + AgencyId + "/" + Identifier
+        # use explicit None check so that zero treated
+        if version is not None:
+            uri += f"/{version}"
+        response = requests.get(uri, headers=self.token, verify=False)
+        if not response.ok:
+            raise ValueError(response.text)
+        return response.json()
 
-        response = requests.post("https://"+self.host+"/api/v1/_query/relationship/bysubject/", headers=self.token, json=jsonquery, verify=False)
-        if response.ok:
-            if response.json() != []:
-                return(response.json())
+    def get_item_version_history(self, AgencyId, Identifier):
+        """Gets the version history of an item.
 
+        Frontend to Colectica GET: /api/v1/item/{agency}/{id}/history
 
-    def get_an_item_version(self, AgencyId, Identifier, Version):
-        """
-            This request an item based on known identification information.
-            https://docs.colectica.com/portal/technical/api/v1/#operation/ApiV1ItemByAgencyByIdByVersionGet
-            Request Type: GET
-            URL: /api/v1/item/{agency}/{id}/{version}
-        """
-        response = requests.get("https://"+self.host+"/api/v1/item/"+AgencyId+"/"+Identifier+"/"+Version, headers=self.token, verify=False)
-        if response.ok:
-            if response.json() != []:
-                return response.json()
+        https://docs.colectica.com/portal/technical/api/v1/#operation/ApiV1ItemByAgencyByIdHistoryGet
 
+        Args:
+            AgencyId (str):
+            Identifier (str):
 
-    def get_item_version_history(self, AgencyId, Identifier):
-        """
-            Gets the version history of an item.
-            https://docs.colectica.com/portal/technical/api/v1/#operation/ApiV1ItemByAgencyByIdHistoryGet
-            Request Type: GET
-            URL: /api/v1/item/{agency}/{id}/history
+        Returns:
+            dict:
+
+        Exceptions:
+            ValueError: the request did not succeed.
         """
-        response = requests.get("https://"+self.host+"/api/v1/item/"+AgencyId+"/"+Identifier+"/history", headers=self.token, verify=False)
-        if response.ok:
-            if response.json() != []:
-                return response.json()
+        uri = f"https://{self.host}/api/v1/item/{AgencyId}/{Identifier}/history"
+        response = requests.get(uri, headers=self.token, verify=False)
+        if not response.ok:
+            raise ValueError(response.text)
+        return response.json()
 
+    def get_item_description(self, AgencyId, Identifier, Version):
+        """Gets a description of a repository item.
 
-    def colectica_get_api(self, url, hostname, tokenHeader):
-        """
-            Gets the version history of an item.
-            https://docs.colectica.com/portal/technical/api/v1/#operation/ApiV1ItemByAgencyByIdHistoryGet
-            Request Type: GET
-            URL: /api/v1/item/{agency}/{id}/history
-        """
-        response = requests.get("https://"+self.host+"/api/v1/"+url, headers=self.token, verify=False)
-        if response.ok:
-            if response.json() != []:
-                return response.json()
+        The description contains identification, naming, and summary information,
+        but not the entire contents of the item.
 
+        Frontend to Colectica GET: /api/v1/item/{agency}/{id}/{version}/description
 
-    def get_item_description(self, AgencyId, Identifier, Version):
-        """
-            Gets a description of a repository item. The description contains identification, naming, 
-            and summary information, but not the entire contents of the item.
-            https://docs.colectica.com/portal/technical/api/v1/#operation/ApiV1ItemByAgencyByIdByVersionDescriptionGet
-            Request Type: GET
-            URL: /api/v1/item/{agency}/{id}/{version}/description
-        """
-        response = requests.get("https://"+self.host+"/api/v1/item/"+AgencyId+"/"+Identifier+"/"+Version+"/description", headers=self.token, verify=False)
-        if response.ok:
-            if response.json() != []:
-                return response.json()
+        https://docs.colectica.com/portal/technical/api/v1/#operation/ApiV1ItemByAgencyByIdByVersionDescriptionGet
+
+        Args:
+            AgencyId (str):
+            Identifier (str):
+            Version (int):
 
+        Returns:
+            dict:
 
-    def relationship_bysubject_descriptions(self, item_type, AgencyId, Identifier, Version, UseDistinctResultItem=True, UseDistinctTargetItem=True):
-        """
-            Gets the repository item descriptions for items that match the specified relationship search parameters.
-            The search will query for items referenced by the target item specified in the search facet.
-            https://docs.colectica.com/portal/technical/api/v1/#operation/ApiV1_queryRelationshipBysubjectDescriptionsPost
-            Request Type: POST
-            URL: /api/v1/_query/relationship/bysubject/descriptions
+        Exceptions:
+            ValueError: the request did not succeed.
         """
 
-        jsonquery = {
-             "ItemTypes": [
-                 item_type
-             ],
-             "TargetItem": {
-                 "AgencyId": AgencyId,
-                 "Identifier": Identifier,
-                 "Version": Version
-             },
-             "UseDistinctResultItem": UseDistinctResultItem,
-             "UseDistinctTargetItem": UseDistinctTargetItem
-        }
+        response = requests.get(
+            "https://"
+            + self.host
+            + "/api/v1/item/"
+            + AgencyId
+            + "/"
+            + Identifier
+            + "/"
+            + str(Version)
+            + "/description",
+            headers=self.token,
+            verify=False,
+        )
+        if not response.ok:
+            raise ValueError(response.text)
+        return response.json()
 
-        response = requests.post("https://"+self.host+"/api/v1/_query/relationship/bysubject/descriptions", headers=self.token, json=jsonquery, verify=False)
-        if response.ok:
-            if response.json() != []:
-                return(response.json())
+    def search_item(
+        self,
+        item_type,
+        search_term,
+        MaxResults=1,
+        *,
+        RankResults=None,
+        SearchDepricatedItems=None,
+        SearchLatestVersion=None,
+        UsePrefixSearch=None,
+    ):
+        """Find all items that match certain criteria.
+
+        Args:
+            item_type (str): for example `C.item_type("Question")` or
+                `C.item_type("Variable")`.
+            search_term (list/str): for example "home" or a list
+                `["work", "home"]`.
+            MaxResults (int): how many results to return or 0 to return
+                all results.
 
+        Keyword Args:
+            RankResults (bool/None):
+            SearchDepricatedItems (bool/None):
+            SearchLatestVersion (bool/None): Whether to search only the
+                latest version.
+            UsePrefixSearch (bool/None): ???
 
-    def relationship_byobject_descriptions(self, item_type, AgencyId, Identifier, Version, UseDistinctResultItem=True, UseDistinctTargetItem=True):
-        """
-            Gets the repository item descriptions for items that match the specified relationship search parameters.
-            The search will query for items that reference the target item specified in the search facet.
-            https://docs.colectica.com/portal/technical/api/v1/#operation/ApiV1_queryRelationshipByobjectDescriptionsPost
-            Request Type: POST
-            URL: /api/v1/_query/relationship/byobject/descriptions
-        """
+        Returns:
+            dict: the results of the search, including list of matches,
+            how many matches, etc.
 
-        jsonquery = {
-             "ItemTypes": [
-                 item_type
-             ],
-             "TargetItem": {
-                 "AgencyId": AgencyId,
-                 "Identifier": Identifier,
-                 "Version": Version
-             },
-             "UseDistinctResultItem": UseDistinctResultItem,
-             "UseDistinctTargetItem": UseDistinctTargetItem
+        For the keyword arguments, if they are omitted (or set to None),
+        then the server chooses a default value.  This might be documented
+        elsewhere.
+
+        This uses the ``/api/v1/_query`` API call.
+
+        Documented here: https://docs.colectica.com/repository/functionality/rest-api/examples/search/
+        """
+        if not isinstance(search_term, list):
+            search_term = [search_term]
+        query = {
+            "ItemTypes": [item_type],
+            "searchTerms": [*search_term],
+            "MaxResults": MaxResults,
         }
-
-        response = requests.post("https://"+self.host+"/api/v1/_query/relationship/byobject/descriptions", headers=self.token, json=jsonquery, verify=False)
+        if RankResults is not None:
+            query.update({"RankResults": RankResults})
+        if SearchDepricatedItems is not None:
+            query.update({"SearchDepricatedItems": SearchDepricatedItems})
+        if SearchLatestVersion is not None:
+            query.update({"SearchLatestVersion": SearchLatestVersion})
+        if UsePrefixSearch is not None:
+            query["UsePrefixSearch"] = UsePrefixSearch
+
+        response = requests.post(
+            "https://" + self.host + "/api/v1/_query/",
+            headers=self.token,
+            json=query,
+            verify=False,
+        )
         if response.ok:
-            if response.json() != []:
-                return(response.json())
+            return response.json()
+        raise ValueError(
+            f"Server returned {response.status_code} error: {response.content}"
+        )
+
+    def search_relationship_bysubject(
+        self,
+        item_type,
+        AgencyId,
+        Identifier,
+        *,
+        Version=None,
+        Descriptions=False,
+        UseDistinctResultItem=True,
+        UseDistinctTargetItem=True,
+    ):
+        """Search for items that are related to a particular item.
+
+        Args:
+            item_type (str): for example `C.item_type("Question")` or
+                `C.item_type("Variable")`.
+            AgencyId (str): For example, ``"uk.cls.nextsteps"``.
+            Identifier (str): e.g., ``"a6f96245-5c00-4ad3-89e9-79afaefa0c28"``.
 
+        Keyword Args:
+            Version (int/None): if omitted, first make a call to
+                retrieve the latest version.
+            Descriptions (bool): if True, return less detail.
+                Default: False, so return full detail.
+            UseDistinctResultItem (bool/None): ???
+            UseDistinctTargetItem (bool/None): ???
 
-    def relationship_bysubject(self, item_type, AgencyId, Identifier, Version,  UseDistinctResultItem=True, UseDistinctTargetItem=True):
-        """
-            Gets a list of items referenced by the specified item, according to the provided search options.
-            https://docs.colectica.com/portal/technical/api/v1/#operation/ApiV1_queryRelationshipBysubjectPost
-            Request Type: POST
-            URL: /api/v1/_query/relationship/bysubject
-        """
+        Returns:
+            list: A list of dicts, each dict is a bit tricky to work with.
+            There are two top-level keys and other 2nd-level keys::
 
-        jsonquery = {
-             "ItemTypes": [
-                 item_type
-             ],
-             "TargetItem": {
-                 "AgencyId": AgencyId,
-                 "Identifier": Identifier,
-                 "Version": Version
-             },
-             "UseDistinctResultItem": UseDistinctResultItem,
-             "UseDistinctTargetItem": UseDistinctTargetItem
+                Item1 (outer property)
+                  - Item1: the UUID of the result
+                  - Item2: the version number of the result
+                  - Item3: the agency identifier of the result
+                Item2: an identifier that indicates the item type of the result.
+
+            This format is
+            `documented here <https://docs.colectica.com/repository/functionality/rest-api/examples/relationship-search/>`_.
+
+        For the keyword arguments, if they are omitted (or set to None),
+        then the server chooses a default value.  This might be documented
+        elsewhere.
+
+        This uses the ``/api/v1/_query/relationship/bysubject/`` API call.
+
+        Documented here: https://docs.colectica.com/repository/functionality/rest-api/examples/search/
+        """
+        if Version is None:
+            # print("getting the version...")
+            Version = self.get_item_json(AgencyId, Identifier)["Version"]
+            # print(f"the version is {Version}")
+        query = {
+            "ItemTypes": [item_type],
+            "TargetItem": {
+                "AgencyId": AgencyId,
+                "Identifier": Identifier,
+                "Version": Version,
+            },
         }
-
-        response = requests.post("https://"+self.host+"/api/v1/_query/relationship/bysubject", headers=self.token, json=jsonquery, verify=False)
+        if UseDistinctResultItem is not None:
+            query["UseDistinctResultItem"] = UseDistinctResultItem
+        if UseDistinctTargetItem is not None:
+            query["UseDistinctTargetItem"] = UseDistinctTargetItem
+
+        url = f"https://{self.host}/api/v1/_query/relationship/bysubject/"
+        if Descriptions:
+            url += "descriptions"
+        response = requests.post(url, headers=self.token, json=query, verify=False)
         if response.ok:
-            if response.json() != []:
-                return(response.json())
+            return response.json()
+        raise ValueError(
+            f"Server returned {response.status_code} error: {response.content}"
+        )
+
+    def search_relationship_byobject(
+        self,
+        item_type,
+        AgencyId,
+        Identifier,
+        *,
+        Version=None,
+        Descriptions=False,
+        UseDistinctResultItem=True,
+        UseDistinctTargetItem=True,
+    ):
+        """Search for items that are related to a particular item by object.
 
+        Args:
+            item_type (str): for example `C.item_type("Question")` or
+                `C.item_type("Variable")`.
+            AgencyId (str): For example, ``"uk.cls.nextsteps"``.
+            Identifier (str): e.g., ``"a6f96245-5c00-4ad3-89e9-79afaefa0c28"``.
 
-    def relationship_byobject(self, item_type, AgencyId, Identifier, Version, UseDistinctResultItem=True, UseDistinctTargetItem=True):
-        """
-            Gets a list of items that reference the specified item, according to the provided search options.
-            https://docs.colectica.com/portal/technical/api/v1/#operation/ApiV1_queryRelationshipByobjectPost
-            Request Type: POST
-            URL: /api/v1/_query/relationship/byobject
-        """
+        Keyword Args:
+            Version (int/None): if omitted, first make a call to
+                retrieve the latest version.
+            Descriptions (bool): if True, return less detail.
+                Default: False, so return full detail.
+            UseDistinctResultItem (bool/None): ???
+            UseDistinctTargetItem (bool/None): ???
 
-        jsonquery = {
-             "ItemTypes": [
-                 item_type
-             ],
-             "TargetItem": {
-                 "AgencyId": AgencyId,
-                 "Identifier": Identifier,
-                 "Version": Version
-             },
-             "UseDistinctResultItem": UseDistinctResultItem,
-             "UseDistinctTargetItem": UseDistinctTargetItem
-        }
+        Returns:
+            list: A list of dicts, each dict is a bit tricky to work with.
+            There are two top-level keys and other 2nd-level keys::
 
-        response = requests.post("https://"+self.host+"/api/v1/_query/relationship/byobject", headers=self.token, json=jsonquery, verify=False)
+                Item1 (outer property)
+                  - Item1: the UUID of the result
+                  - Item2: the version number of the result
+                  - Item3: the agency identifier of the result
+                Item2: an identifier that indicates the item type of the result.
+
+            This format is
+            `documented here <https://docs.colectica.com/repository/functionality/rest-api/examples/relationship-search/>`_.
+
+        For the keyword arguments, if they are omitted (or set to None),
+        then the server chooses a default value.  This might be documented
+        elsewhere.
+
+        This uses the ``/api/v1/_query/relationship/bysubject/`` API call.
+
+        Documented here: https://docs.colectica.com/repository/functionality/rest-api/examples/search/
+        """
+        if Version is None:
+            # print("getting the version...")
+            Version = self.get_item_json(AgencyId, Identifier)["Version"]
+            # print(f"the version is {Version}")
+        query = {
+            "ItemTypes": [item_type],
+            "TargetItem": {
+                "AgencyId": AgencyId,
+                "Identifier": Identifier,
+                "Version": Version,
+            },
+        }
+        if UseDistinctResultItem is not None:
+            query["UseDistinctResultItem"] = UseDistinctResultItem
+        if UseDistinctTargetItem is not None:
+            query["UseDistinctTargetItem"] = UseDistinctTargetItem
+
+        url = f"https://{self.host}/api/v1/_query/relationship/byobject/"
+        if Descriptions:
+            url += "descriptions"
+        response = requests.post(url, headers=self.token, json=query, verify=False)
         if response.ok:
-            if response.json() != []:
-                return(response.json())
+            return response.json()
+        raise ValueError(
+            f"Server returned {response.status_code} error: {response.content}"
+        )
+
+    def search_set(
+        self,
+        item_types,
+        AgencyId,
+        Identifier,
+        MaxResults=1,
+    ):
+        """Find all items that are somehow connected to a given item.
+
+        Args:
+            item_types (str/list[str]): the item types to search for.
+                or all types if empty.  You can omit the list if
+                searching for just one item type.
+            AgencyId (str):
+            Identifier (str):
+            MaxResults (int): how many results to return or 0 to return
+                all results.
 
+        Returns:
+            dict: the results of the search, including list of matches,
+            how many matches, etc.
 
-    def relationship_matrix(self, AgencyId, Identifier, Version, Predicate, ReverseTraversal=True):
-        """
-            Gets a matrix representing all items in a set and the relationships among those items.
-            https://docs.colectica.com/portal/technical/api/v1/#operation/ApiV1_queryRelationshipMatrixPost
-            Request Type: POST
-            URL: /api/v1/_query/relationship/matrix
+        For the keyword arguments, if they are omitted (or set to None),
+        then the server chooses a default value.  This might be documented
+        elsewhere.
+
+        This uses the ``/api/v1/_query`` API call.
+
+        Documented here: https://docs.colectica.com/repository/functionality/rest-api/examples/search/
+        """
+        if not isinstance(item_types, list):
+            item_types = [item_types]
+        query = {
+            "ItemTypes": item_types,
+            "MaxResults": MaxResults,
+            "searchSets": [
+                {"agencyId": AgencyId, "identifier": Identifier, "version": 1}
+            ],
+        }
+        response = requests.post(
+            "https://" + self.host + "/api/v1/_query/",
+            headers=self.token,
+            json=query,
+            verify=False,
+        )
+        if response.ok:
+            return response.json()
+        raise ValueError(
+            f"Server returned {response.status_code} error: {response.content}"
+        )
+
+    # ----------------------------------------
+
+    def relationship_matrix(
+        self, AgencyId, Identifier, Version, Predicate, ReverseTraversal=True
+    ):
+        """
+        Gets a matrix representing all items in a set and the relationships among those items.
+        https://docs.colectica.com/portal/technical/api/v1/#operation/ApiV1_queryRelationshipMatrixPost
+        Request Type: POST
+        URL: /api/v1/_query/relationship/matrix
         """
 
         jsonquery = {
             "RootItems": [
-                {
-                "AgencyId": AgencyId,
-                "Identifier": Identifier,
-                "Version": Version
-                }
+                {"AgencyId": AgencyId, "Identifier": Identifier, "Version": Version}
             ],
-            "Facet": {
-                "Predicate": Predicate,
-                "ReverseTraversal": ReverseTraversal
-            }
+            "Facet": {"Predicate": Predicate, "ReverseTraversal": ReverseTraversal},
         }
 
-        response = requests.post("https://"+self.host+"/api/v1/_query/relationship/matrix", headers=self.token, json=jsonquery, verify=False)
+        response = requests.post(
+            "https://" + self.host + "/api/v1/_query/relationship/matrix",
+            headers=self.token,
+            json=jsonquery,
+            verify=False,
+        )
         if response.ok:
             if response.json() != []:
-                return(response.json())
-
+                return response.json()
 
-    def relationship_matrix_typed(self, AgencyId, Identifier, Version, Predicate, ReverseTraversal=True):
-        """
-            Gets a matrix representing all items in a set and the relationships among those items.
-            https://docs.colectica.com/portal/technical/api/v1/#operation/ApiV1_queryRelationshipMatrixPost
-            Request Type: POST
-            URL: /api/v1/_query/relationship/matrix/typed
+    def relationship_matrix_typed(
+        self, AgencyId, Identifier, Version, Predicate, ReverseTraversal=True
+    ):
+        """
+        Gets a matrix representing all items in a set and the relationships among those items.
+        https://docs.colectica.com/portal/technical/api/v1/#operation/ApiV1_queryRelationshipMatrixPost
+        Request Type: POST
+        URL: /api/v1/_query/relationship/matrix/typed
         """
 
         jsonquery = {
             "RootItems": [
-                {
-                "AgencyId": AgencyId,
-                "Identifier": Identifier,
-                "Version": Version
-                }
+                {"AgencyId": AgencyId, "Identifier": Identifier, "Version": Version}
             ],
-            "Facet": {
-                "Predicate": Predicate,
-                "ReverseTraversal": ReverseTraversal
-            }
+            "Facet": {"Predicate": Predicate, "ReverseTraversal": ReverseTraversal},
         }
 
-        response = requests.post("https://"+self.host+"/api/v1/_query/relationship/matrix/typed", headers=self.token, json=jsonquery, verify=False)
+        response = requests.post(
+            "https://" + self.host + "/api/v1/_query/relationship/matrix/typed",
+            headers=self.token,
+            json=jsonquery,
+            verify=False,
+        )
         if response.ok:
             if response.json() != []:
-                return(response.json())
-
+                return response.json()
 
     def get_a_set(self, AgencyId, Identifier, Version):
         """Gets the set of all items under the specified root.
 
         Frontend to Colectica GET: /api/v1/set/{agency}/{id}/{version}
 
+        https://docs.colectica.com/portal/technical/api/v1/#operation/ApiV1SetByAgencyByIdByVersionGet
+
         Args:
-            AgencyId (str):  foo foo foo
+            AgencyId (str):
             Identifier (str):
-            Version (str): 
+            Version (str):
             hostname (str):
-            tokenHeader (str): 
+            tokenHeader (str):
 
         Returns:
-            dict: as documented at [1].
-
-        [1] https://docs.colectica.com/portal/technical/api/v1/#operation/ApiV1SetByAgencyByIdByVersionGet
+            dict:
         """
 
-        response = requests.get("https://" + self.host + "/api/v1/set/" + AgencyId + "/" + Identifier + "/" + Version , headers=self.token, verify=False)
+        response = requests.get(
+            "https://"
+            + self.host
+            + "/api/v1/set/"
+            + AgencyId
+            + "/"
+            + Identifier
+            + "/"
+            + Version,
+            headers=self.token,
+            verify=False,
+        )
         if response.ok:
             if response.json() != []:
                 return response.json()
 
-
     def get_a_set_typed(self, AgencyId, Identifier, Version):
         """
-            Gets the set of items defined by the specified root. Each item in the set will have the latest version number for that item.
-            https://docs.colectica.com/portal/technical/api/v1/#operation/ApiV1SetByAgencyByIdByVersionTypedGet
-            Request Type: GET
-            URL: /api/v1/set/{agency}/{id}/{version}/typed
+        Gets the set of items defined by the specified root. Each item in the set will have the latest version number for that item.
+        https://docs.colectica.com/portal/technical/api/v1/#operation/ApiV1SetByAgencyByIdByVersionTypedGet
+        Request Type: GET
+        URL: /api/v1/set/{agency}/{id}/{version}/typed
         """
 
-        response = requests.get("https://" + self.host + "/api/v1/set/" + AgencyId + "/" + Identifier + "/" + Version + "/typed", headers=self.token, verify=False)
+        response = requests.get(
+            "https://"
+            + self.host
+            + "/api/v1/set/"
+            + AgencyId
+            + "/"
+            + Identifier
+            + "/"
+            + Version
+            + "/typed",
+            headers=self.token,
+            verify=False,
+        )
         if response.ok:
             if response.json() != []:
                 return response.json()
 
-
     def get_a_set_lasted(self, AgencyId, Identifier):
         """
-            Gets the set of items defined by the specified root. Each item in the set will have the latest version number for that item.
-            https://docs.colectica.com/portal/technical/api/v1/#operation/ApiV1SetByAgencyByIdGet
-            Request Type: GET
-            URL: /api/v1/set/{agency}/{id}
+        Gets the set of items defined by the specified root. Each item in the set will have the latest version number for that item.
+        https://docs.colectica.com/portal/technical/api/v1/#operation/ApiV1SetByAgencyByIdGet
+        Request Type: GET
+        URL: /api/v1/set/{agency}/{id}
         """
 
-        response = requests.get("https://" + self.host + "/api/v1/set/" + AgencyId + "/" + Identifier, headers=self.token, verify=False)
+        response = requests.get(
+            "https://" + self.host + "/api/v1/set/" + AgencyId + "/" + Identifier,
+            headers=self.token,
+            verify=False,
+        )
         if response.ok:
             if response.json() != []:
                 return response.json()
 
 
 if __name__ == "__main__":
     raise RuntimeError("don't run this directly")
-
```

### Comparing `Colectica_API-0.0.2/colectica_api/colectica.py` & `Colectica_API-0.0.3/colectica_api/colectica.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 """
     Pull information using python ColecticaPortal api
 """
 
 from io import StringIO
+import json
+import os
 import xml.etree.ElementTree as ET
+
 import pandas as pd
-import json
-from .api import ColecticaLowLevelAPI
+import requests
+
+from .api import ColecticaBasicAPI
 
 
 def remove_xml_ns(xml):
     """
     Read xml from string, remove namespaces, return root
     """
     it = ET.iterparse(StringIO(xml))
@@ -1097,33 +1101,43 @@
     elif item_type == 'Data File':
         info = root_to_dict_data_file(root)
     else:
         info = {}
     return info
 
 
-class ColecticaObject(ColecticaLowLevelAPI):
-    """Ask practical questions to Colectica.
+class ColecticaObject(ColecticaBasicAPI):
+    """Ask practical questions to a Colectica server.
 
-    This object communicates with a Colectica server.  In most cases, it can
-    use the newer JSON-based api but still has a deprecated implementation of
-    the older XML-based api.  The latter involves a lot of manual parsing of
-    data.
+    This extends :class:`ColecticaBasicAPI` by adding additional useful
+    methods.
 
     You make a new ColecticaObject by using:
 
     >>> C = ColecticaObject(hostname, username, password)
+
+    If `hostname`, `username` or `password` are omitted, environment
+    variables `COLECTICA_HOSTNAME`, `COLECTICA_USERNAME` and `COLECTICA_PASSWORD`
+    will be used, if they are defined.
     """
 
-    def item_to_dict(self, AgencyId, Identifier, Version = None):
-        """
-        From an agency ID and an identifier, get information using get_an_item
-        Return a dictionary
+    def item_to_dict(self, AgencyId, Identifier, Version=None):
+        """From an agency ID and an identifier, get information using ``get_an_item``.
+
+        Args:
+            AgencyId (str): For example, ``"uk.cls.nextsteps"``.
+            Identifier (str): e.g., ``"a6f96245-5c00-4ad3-89e9-79afaefa0c28"``.
+
+        Keyword Args:
+            Version (int/None): if omitted, get the latest version.
+
+        Return:
+            dict: a dictionary of the item contents.
         """
-        if Version == None:
+        if Version is None:
             result = self.get_an_item(AgencyId, Identifier)
         else:
             result = self.get_an_item_version(AgencyId, Identifier, Version)
 
         info = {}
         item_info = None
         if not result is None:
@@ -1135,58 +1149,64 @@
                 else:
                     info[k] = v
             d = {**info, **item_info}
         else:
             d = {}
         return d
 
+    def get_a_set_to_df(self, AgencyId: str, Identifier: str, Version: int):
+        """Find all items that are somehow connected to a given item, using ``get_a_set_typed``
 
-    def get_a_set_to_df(self, AgencyId, Identifier, Version):
-        """
-        From a study, find all questions
-        Example:
-            'ItemType': 'f196cc07-9c99-4725-ad55-5b34f479cf7d', (Instrument)
-            'AgencyId': 'uk.cls.nextsteps',
-            'Version': 1,
-            'Identifier': 'a6f96245-5c00-4ad3-89e9-79afaefa0c28'
+        Args:
+            AgencyId (str):
+            Identifier (str):
+            Version (int):
+
+        Returns:
+            pandas dataframe: with columns ["ItemType", "Agency", "Identifier", "Version"]
+        
         """
 
         l = self.get_a_set_typed(AgencyId, Identifier, Version)
         # print(l)
         df = pd.DataFrame(
              [self.item_code_inv(l[i]["Item2"]), l[i]["Item1"]["Item3"], l[i]["Item1"]["Item1"], l[i]["Item1"]["Item2"]] for i in range(len(l))
          )
         df.columns = ["ItemType", "Agency", "Identifier", "Version"]
 
         return df
 
 
     def item_info_set(self, AgencyId, Identifier):
-        """
-        From an ID, find it's name and set
-        """
-        info = self.item_to_dict(AgencyId, Identifier)
-        df = self.get_a_set_to_df(AgencyId, Identifier, str(info['Version']))
-        return df, info
-
+        """Find latest version of an item and it's set
 
-    def item_info_set_json(self, AgencyId, Identifier):
+        Args:
+            AgencyId (str):
+            Identifier (str):
+
+        Returns:
+            tuple: A 2-tuple `(df, info)` consisting of a Pandas dataframe of a set
+            and a dict with info about the item.
         """
-        From an ID, find it's name and set
-        """
-        info = self.get_an_item_json(AgencyId, Identifier)
+        info = self.get_item_json(AgencyId, Identifier)
         df = self.get_a_set_to_df(AgencyId, Identifier, str(info['Version']))
         return df, info
 
-
     def get_question_info(self, AgencyId, Identifier):
         """
-        From a question identifier, get information about it
+        From a question identifier, get information about 
+        
+        Args:
+            AgencyId (str):
+            Identifier (str):
+
+        Returns:
+            dict: 
         """
-        question_info = self.get_an_item(AgencyId, Identifier)
+        question_info = self.get_item_xml(AgencyId, Identifier)
         root = remove_xml_ns(question_info["Item"])
 
         question = {}
         for k, v in question_info.items():
             if k == 'ItemType':
                 question[k] = self.item_code_inv(v)
             elif k == 'Item':
@@ -1198,14 +1218,21 @@
                 question[k] = v
         return question
 
 
     def get_question_all(self, AgencyId, Identifier):
         """
         From a question ID, return question info and it's response
+        
+        Args:
+            AgencyId (str):
+            Identifier (str):
+
+        Returns:
+            pandas dataframe: with column name ['QuestionURN', 'QuestionItemName', 'response_type', 'Label', 'DateTypeCode']
         """
         # print(AgencyId, Identifier)
         question_info = self.item_to_dict(AgencyId, Identifier)
         # print(question_info)
 
         if question_info['Response']== {}:
             QI_response_type = None
```

### Comparing `Colectica_API-0.0.2/pyproject.toml` & `Colectica_API-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Colectica_API"
-version = "0.0.2"
 authors = [
   { name="Jenny Li", email="jenny.li@ucl.ac.uk" },
 ]
 description = "Python interface to the Colectica API"
+dynamic = ['version']
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
@@ -23,7 +23,14 @@
 
 [project.urls]
 "Homepage" = "https://github.com/CLOSER-Cohorts/colectica_api"
 "Bug Tracker" = "https://github.com/CLOSER-Cohorts/colectica_api/issues"
 
 [tool.setuptools]
 packages = ["colectica_api"]
+
+[tool.setuptools.dynamic]
+version = {attr = 'colectica_api.__version__'}
+
+[tool.black]
+line-length = 88
+target-version = ['py38']
```

