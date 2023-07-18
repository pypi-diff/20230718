# Comparing `tmp/azure-purview-sharing-1.0.0b2.zip` & `tmp/azure-purview-sharing-1.0.0b3.zip`

## zipinfo {}

```diff
@@ -1,54 +1,56 @@
-Zip file size: 87459 bytes, number of entries: 52
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 20:18 azure-purview-sharing-1.0.0b2/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 20:18 azure-purview-sharing-1.0.0b2/azure_purview_sharing.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 20:18 azure-purview-sharing-1.0.0b2/tests/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 20:18 azure-purview-sharing-1.0.0b2/azure/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 20:18 azure-purview-sharing-1.0.0b2/samples/
--rw-rw-r--  2.0 unx    13777 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/README.md
--rw-rw-r--  2.0 unx       38 b- defN 23-Jun-06 20:18 azure-purview-sharing-1.0.0b2/setup.cfg
--rw-rw-r--  2.0 unx    14679 b- defN 23-Jun-06 20:18 azure-purview-sharing-1.0.0b2/PKG-INFO
--rw-rw-r--  2.0 unx     1073 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/LICENSE
--rw-rw-r--  2.0 unx     2457 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/setup.py
--rw-rw-r--  2.0 unx      113 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/pyproject.toml
--rw-rw-r--  2.0 unx      192 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/MANIFEST.in
--rw-rw-r--  2.0 unx      194 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/CHANGELOG.md
--rw-rw-r--  2.0 unx    14679 b- defN 23-Jun-06 20:18 azure-purview-sharing-1.0.0b2/azure_purview_sharing.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx        1 b- defN 23-Jun-06 20:18 azure-purview-sharing-1.0.0b2/azure_purview_sharing.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx        1 b- defN 23-Jun-06 20:18 azure-purview-sharing-1.0.0b2/azure_purview_sharing.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx        6 b- defN 23-Jun-06 20:18 azure-purview-sharing-1.0.0b2/azure_purview_sharing.egg-info/top_level.txt
--rw-rw-r--  2.0 unx      102 b- defN 23-Jun-06 20:18 azure-purview-sharing-1.0.0b2/azure_purview_sharing.egg-info/requires.txt
--rw-rw-r--  2.0 unx     1287 b- defN 23-Jun-06 20:18 azure-purview-sharing-1.0.0b2/azure_purview_sharing.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx    12780 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/tests/test_sent_shares.py
--rw-rw-r--  2.0 unx     3050 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/tests/conftest.py
--rw-rw-r--  2.0 unx    12227 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/tests/test_received_shares.py
--rw-rw-r--  2.0 unx      777 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/tests/_util.py
--rw-rw-r--  2.0 unx     1972 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/tests/testcase.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 20:18 azure-purview-sharing-1.0.0b2/azure/purview/
--rw-rw-r--  2.0 unx       81 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 20:18 azure-purview-sharing-1.0.0b2/azure/purview/sharing/
--rw-rw-r--  2.0 unx       81 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/azure/purview/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 20:18 azure-purview-sharing-1.0.0b2/azure/purview/sharing/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 20:18 azure-purview-sharing-1.0.0b2/azure/purview/sharing/operations/
--rw-rw-r--  2.0 unx     3694 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/azure/purview/sharing/_configuration.py
--rw-rw-r--  2.0 unx     4247 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/azure/purview/sharing/_client.py
--rw-rw-r--  2.0 unx      884 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/azure/purview/sharing/__init__.py
--rw-rw-r--  2.0 unx      976 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/azure/purview/sharing/_vendor.py
--rw-rw-r--  2.0 unx      488 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/azure/purview/sharing/_version.py
--rw-rw-r--  2.0 unx       26 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/azure/purview/sharing/py.typed
--rw-rw-r--  2.0 unx    78858 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/azure/purview/sharing/_serialization.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/azure/purview/sharing/_patch.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-06 20:18 azure-purview-sharing-1.0.0b2/azure/purview/sharing/aio/operations/
--rw-rw-r--  2.0 unx     3737 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/azure/purview/sharing/aio/_configuration.py
--rw-rw-r--  2.0 unx     4386 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/azure/purview/sharing/aio/_client.py
--rw-rw-r--  2.0 unx      831 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/azure/purview/sharing/aio/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/azure/purview/sharing/aio/_patch.py
--rw-rw-r--  2.0 unx      863 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/azure/purview/sharing/aio/operations/__init__.py
--rw-rw-r--  2.0 unx   223242 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/azure/purview/sharing/aio/operations/_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/azure/purview/sharing/aio/operations/_patch.py
--rw-rw-r--  2.0 unx      863 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/azure/purview/sharing/operations/__init__.py
--rw-rw-r--  2.0 unx   244068 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/azure/purview/sharing/operations/_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/azure/purview/sharing/operations/_patch.py
--rw-rw-r--  2.0 unx     2111 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/samples/README.md
--rw-rw-r--  2.0 unx     4005 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/samples/sent_shares_examples.py
--rw-rw-r--  2.0 unx     2655 b- defN 23-Jun-06 20:17 azure-purview-sharing-1.0.0b2/samples/received_shares_examples.py
-52 files, 658197 bytes uncompressed, 77469 bytes compressed:  88.2%
+Zip file size: 95519 bytes, number of entries: 54
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-18 17:35 azure-purview-sharing-1.0.0b3/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-18 17:35 azure-purview-sharing-1.0.0b3/azure_purview_sharing.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-18 17:35 azure-purview-sharing-1.0.0b3/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-18 17:35 azure-purview-sharing-1.0.0b3/tests/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-18 17:35 azure-purview-sharing-1.0.0b3/samples/
+-rw-rw-r--  2.0 unx    20553 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/README.md
+-rw-rw-r--  2.0 unx     1073 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/LICENSE
+-rw-rw-r--  2.0 unx       38 b- defN 23-Jul-18 17:35 azure-purview-sharing-1.0.0b3/setup.cfg
+-rw-rw-r--  2.0 unx      113 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/pyproject.toml
+-rw-rw-r--  2.0 unx    21455 b- defN 23-Jul-18 17:35 azure-purview-sharing-1.0.0b3/PKG-INFO
+-rw-rw-r--  2.0 unx      192 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/MANIFEST.in
+-rw-rw-r--  2.0 unx      955 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/CHANGELOG.md
+-rw-rw-r--  2.0 unx     2457 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/setup.py
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-18 17:35 azure-purview-sharing-1.0.0b3/azure_purview_sharing.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-18 17:35 azure-purview-sharing-1.0.0b3/azure_purview_sharing.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx     1353 b- defN 23-Jul-18 17:35 azure-purview-sharing-1.0.0b3/azure_purview_sharing.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx    21455 b- defN 23-Jul-18 17:35 azure-purview-sharing-1.0.0b3/azure_purview_sharing.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx      102 b- defN 23-Jul-18 17:35 azure-purview-sharing-1.0.0b3/azure_purview_sharing.egg-info/requires.txt
+-rw-rw-r--  2.0 unx        6 b- defN 23-Jul-18 17:35 azure-purview-sharing-1.0.0b3/azure_purview_sharing.egg-info/top_level.txt
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-18 17:35 azure-purview-sharing-1.0.0b3/azure/purview/
+-rw-rw-r--  2.0 unx       81 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-18 17:35 azure-purview-sharing-1.0.0b3/azure/purview/sharing/
+-rw-rw-r--  2.0 unx       81 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/azure/purview/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-18 17:35 azure-purview-sharing-1.0.0b3/azure/purview/sharing/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-18 17:35 azure-purview-sharing-1.0.0b3/azure/purview/sharing/aio/
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/azure/purview/sharing/_patch.py
+-rw-rw-r--  2.0 unx       26 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/azure/purview/sharing/py.typed
+-rw-rw-r--  2.0 unx      884 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/azure/purview/sharing/__init__.py
+-rw-rw-r--  2.0 unx      488 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/azure/purview/sharing/_version.py
+-rw-rw-r--  2.0 unx     4544 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/azure/purview/sharing/_client.py
+-rw-rw-r--  2.0 unx    78824 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/azure/purview/sharing/_serialization.py
+-rw-rw-r--  2.0 unx     3694 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/azure/purview/sharing/_configuration.py
+-rw-rw-r--  2.0 unx      976 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/azure/purview/sharing/_vendor.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/azure/purview/sharing/operations/_patch.py
+-rw-rw-r--  2.0 unx      945 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/azure/purview/sharing/operations/__init__.py
+-rw-rw-r--  2.0 unx   249166 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/azure/purview/sharing/operations/_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-18 17:35 azure-purview-sharing-1.0.0b3/azure/purview/sharing/aio/operations/
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/azure/purview/sharing/aio/_patch.py
+-rw-rw-r--  2.0 unx      831 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/azure/purview/sharing/aio/__init__.py
+-rw-rw-r--  2.0 unx     4687 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/azure/purview/sharing/aio/_client.py
+-rw-rw-r--  2.0 unx     3737 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/azure/purview/sharing/aio/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/azure/purview/sharing/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx      945 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/azure/purview/sharing/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx   228056 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/azure/purview/sharing/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx    16660 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/tests/test_received_shares.py
+-rw-rw-r--  2.0 unx    16639 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/tests/test_sent_shares.py
+-rw-rw-r--  2.0 unx      777 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/tests/_util.py
+-rw-rw-r--  2.0 unx     1956 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/tests/testcase.py
+-rw-rw-r--  2.0 unx     1364 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/tests/test_share_resources.py
+-rw-rw-r--  2.0 unx     3637 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/tests/conftest.py
+-rw-rw-r--  2.0 unx     2316 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/samples/README.md
+-rw-rw-r--  2.0 unx     2655 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/samples/received_shares_examples.py
+-rw-rw-r--  2.0 unx     1285 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/samples/share_resources_examples.py
+-rw-rw-r--  2.0 unx     4628 b- defN 23-Jul-18 17:33 azure-purview-sharing-1.0.0b3/samples/sent_shares_examples.py
+54 files, 702332 bytes uncompressed, 85129 bytes compressed:  87.9%
```

## zipnote {}

```diff
@@ -1,157 +1,163 @@
-Filename: azure-purview-sharing-1.0.0b2/
+Filename: azure-purview-sharing-1.0.0b3/
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure_purview_sharing.egg-info/
+Filename: azure-purview-sharing-1.0.0b3/azure_purview_sharing.egg-info/
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/tests/
+Filename: azure-purview-sharing-1.0.0b3/azure/
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure/
+Filename: azure-purview-sharing-1.0.0b3/tests/
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/samples/
+Filename: azure-purview-sharing-1.0.0b3/samples/
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/README.md
+Filename: azure-purview-sharing-1.0.0b3/README.md
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/setup.cfg
+Filename: azure-purview-sharing-1.0.0b3/LICENSE
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/PKG-INFO
+Filename: azure-purview-sharing-1.0.0b3/setup.cfg
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/LICENSE
+Filename: azure-purview-sharing-1.0.0b3/pyproject.toml
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/setup.py
+Filename: azure-purview-sharing-1.0.0b3/PKG-INFO
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/pyproject.toml
+Filename: azure-purview-sharing-1.0.0b3/MANIFEST.in
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/MANIFEST.in
+Filename: azure-purview-sharing-1.0.0b3/CHANGELOG.md
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/CHANGELOG.md
+Filename: azure-purview-sharing-1.0.0b3/setup.py
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure_purview_sharing.egg-info/PKG-INFO
+Filename: azure-purview-sharing-1.0.0b3/azure_purview_sharing.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure_purview_sharing.egg-info/not-zip-safe
+Filename: azure-purview-sharing-1.0.0b3/azure_purview_sharing.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure_purview_sharing.egg-info/dependency_links.txt
+Filename: azure-purview-sharing-1.0.0b3/azure_purview_sharing.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure_purview_sharing.egg-info/top_level.txt
+Filename: azure-purview-sharing-1.0.0b3/azure_purview_sharing.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure_purview_sharing.egg-info/requires.txt
+Filename: azure-purview-sharing-1.0.0b3/azure_purview_sharing.egg-info/requires.txt
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure_purview_sharing.egg-info/SOURCES.txt
+Filename: azure-purview-sharing-1.0.0b3/azure_purview_sharing.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/tests/test_sent_shares.py
+Filename: azure-purview-sharing-1.0.0b3/azure/purview/
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/tests/conftest.py
+Filename: azure-purview-sharing-1.0.0b3/azure/__init__.py
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/tests/test_received_shares.py
+Filename: azure-purview-sharing-1.0.0b3/azure/purview/sharing/
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/tests/_util.py
+Filename: azure-purview-sharing-1.0.0b3/azure/purview/__init__.py
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/tests/testcase.py
+Filename: azure-purview-sharing-1.0.0b3/azure/purview/sharing/operations/
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure/purview/
+Filename: azure-purview-sharing-1.0.0b3/azure/purview/sharing/aio/
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure/__init__.py
+Filename: azure-purview-sharing-1.0.0b3/azure/purview/sharing/_patch.py
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure/purview/sharing/
+Filename: azure-purview-sharing-1.0.0b3/azure/purview/sharing/py.typed
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure/purview/__init__.py
+Filename: azure-purview-sharing-1.0.0b3/azure/purview/sharing/__init__.py
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure/purview/sharing/aio/
+Filename: azure-purview-sharing-1.0.0b3/azure/purview/sharing/_version.py
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure/purview/sharing/operations/
+Filename: azure-purview-sharing-1.0.0b3/azure/purview/sharing/_client.py
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure/purview/sharing/_configuration.py
+Filename: azure-purview-sharing-1.0.0b3/azure/purview/sharing/_serialization.py
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure/purview/sharing/_client.py
+Filename: azure-purview-sharing-1.0.0b3/azure/purview/sharing/_configuration.py
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure/purview/sharing/__init__.py
+Filename: azure-purview-sharing-1.0.0b3/azure/purview/sharing/_vendor.py
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure/purview/sharing/_vendor.py
+Filename: azure-purview-sharing-1.0.0b3/azure/purview/sharing/operations/_patch.py
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure/purview/sharing/_version.py
+Filename: azure-purview-sharing-1.0.0b3/azure/purview/sharing/operations/__init__.py
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure/purview/sharing/py.typed
+Filename: azure-purview-sharing-1.0.0b3/azure/purview/sharing/operations/_operations.py
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure/purview/sharing/_serialization.py
+Filename: azure-purview-sharing-1.0.0b3/azure/purview/sharing/aio/operations/
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure/purview/sharing/_patch.py
+Filename: azure-purview-sharing-1.0.0b3/azure/purview/sharing/aio/_patch.py
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure/purview/sharing/aio/operations/
+Filename: azure-purview-sharing-1.0.0b3/azure/purview/sharing/aio/__init__.py
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure/purview/sharing/aio/_configuration.py
+Filename: azure-purview-sharing-1.0.0b3/azure/purview/sharing/aio/_client.py
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure/purview/sharing/aio/_client.py
+Filename: azure-purview-sharing-1.0.0b3/azure/purview/sharing/aio/_configuration.py
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure/purview/sharing/aio/__init__.py
+Filename: azure-purview-sharing-1.0.0b3/azure/purview/sharing/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure/purview/sharing/aio/_patch.py
+Filename: azure-purview-sharing-1.0.0b3/azure/purview/sharing/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure/purview/sharing/aio/operations/__init__.py
+Filename: azure-purview-sharing-1.0.0b3/azure/purview/sharing/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure/purview/sharing/aio/operations/_operations.py
+Filename: azure-purview-sharing-1.0.0b3/tests/test_received_shares.py
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure/purview/sharing/aio/operations/_patch.py
+Filename: azure-purview-sharing-1.0.0b3/tests/test_sent_shares.py
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure/purview/sharing/operations/__init__.py
+Filename: azure-purview-sharing-1.0.0b3/tests/_util.py
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure/purview/sharing/operations/_operations.py
+Filename: azure-purview-sharing-1.0.0b3/tests/testcase.py
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/azure/purview/sharing/operations/_patch.py
+Filename: azure-purview-sharing-1.0.0b3/tests/test_share_resources.py
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/samples/README.md
+Filename: azure-purview-sharing-1.0.0b3/tests/conftest.py
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/samples/sent_shares_examples.py
+Filename: azure-purview-sharing-1.0.0b3/samples/README.md
 Comment: 
 
-Filename: azure-purview-sharing-1.0.0b2/samples/received_shares_examples.py
+Filename: azure-purview-sharing-1.0.0b3/samples/received_shares_examples.py
+Comment: 
+
+Filename: azure-purview-sharing-1.0.0b3/samples/share_resources_examples.py
+Comment: 
+
+Filename: azure-purview-sharing-1.0.0b3/samples/sent_shares_examples.py
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-purview-sharing-1.0.0b2/README.md` & `azure-purview-sharing-1.0.0b3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Azure Purview Sharing client library for Python
 
 Microsoft Purview Share is a fully managed cloud service.
 
-**Please rely heavily on the [service's documentation][sharing_product_documentation] and our [protocol client docs][protocol_client_quickstart] to use this library**
+**Please rely heavily on the [service's documentation][sharing_product_documentation] and our [protocol client docs][request_builders_and_client] to use this library**
 
 [Source code][source_code] | [Package (PyPI)][client_pypi_package] | [Product documentation][sharing_product_documentation]
 
 ## Getting started
 
 ### Install the package
 
@@ -21,33 +21,60 @@
 - You must have an [Azure subscription][azure_subscription] and a [Purview resource][purview_resource] to use this package.
 - Python 3.6 or later is required to use this package.
 
 ### Authenticate the client
 
 #### Using Azure Active Directory
 
-This document demonstrates using [DefaultAzureCredential][default_cred_ref] to authenticate via Azure Active Directory. However, any of the credentials offered by the [azure_identity][azure_identity] will be accepted.  See the [azure_identity][azure_identity] documentation for more information about other credentials.
+This document demonstrates using [DefaultAzureCredential][default_azure_credential] to authenticate via Azure Active Directory. However, any of the credentials offered by the [azure-identity package][azure_identity_pip] will be accepted.  See the [azure-identity][azure_identity_credentials] documentation for more information about other credentials.
 
 Once you have chosen and configured your credential, you can create instances of the `PurviewSharingClient`.
 
 ```python
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
 credential = DefaultAzureCredential()
 client = PurviewSharingClient(endpoint="https://<my-account-name>.purview.azure.com", credential=credential)
 ```
 
 ## Key concepts
 
+**Data Provider:** A data provider is the individual who creates a share by selecting a data source, choosing which files and folders to share, and who to share them with. Microsoft Purview then sends an invitation to each data consumer.
+
+**Data Consumer:** A data consumer is the individual who accepts the invitation by specifying a target storage account in their own Azure subscription that they'll use to access the shared data.
+
 ## Examples
 
-The following section shows you how to initialize and authenticate your client and share data.
+Table of Contents: 
+- [Data Provider](#data-provider-examples)
+- [Data Consumer](#data-consumer-examples)
+- [Share Resource](#share-resource-examples)
+
+## Data Provider Examples
+
+The following code examples demonstrate how data providers can use the Microsoft Azure Python SDK for Purview Sharing to manage their sharing activity.
+
+### Create a Sent Share Client
+
+```python Snippet:create_a_sent_share_client
+import os, uuid, json
+
+from azure.purview.sharing import PurviewSharingClient
+from azure.identity import DefaultAzureCredential
+
+endpoint = os.environ["ENDPOINT"]
+credential = DefaultAzureCredential()
+
+client = PurviewSharingClient(endpoint=endpoint, credential=credential)
+```
+
+### Create Share
 
-### Create share
+To begin sharing data, the data provider must first create a sent share that identifies the data they would like to share.
 
 ```python Snippet:create_a_sent_share
 import os, uuid, json
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
@@ -88,15 +115,90 @@
     str(sent_share_id),
     sent_share=sent_share)
 
 response = request.result()
 print(response)
 ```
 
-### Get sent share
+### Send Share Invitation to a User
+
+After creating a sent share, the data provider can extend invitations to consumers who may then view the shared data. In this example, an invitation is extended to an individual by specifying their email address.
+
+```python Snippet:send_a_user_invitation
+import os, uuid
+
+from azure.purview.sharing import PurviewSharingClient
+from azure.identity import DefaultAzureCredential
+from datetime import date
+
+endpoint = os.environ["ENDPOINT"]
+credential = DefaultAzureCredential()
+
+client = PurviewSharingClient(endpoint=endpoint, credential=credential)
+
+sent_share_id = uuid.uuid4()
+sent_share_invitation_id = uuid.uuid4()
+
+consumerEmail = "consumer@contoso.com"
+today = date.today()
+invitation = {
+    "invitationKind": "User",
+    "properties": {
+        "targetEmail": consumerEmail,
+        "notify": "true",
+        "expirationDate": date(today.year+1,today.month,today.day).strftime("%Y-%m-%d") + " 00:00:00"
+    }
+}
+
+invitation_request = client.sent_shares.create_invitation(
+    sent_share_id=str(sent_share_id),
+    sent_share_invitation_id=str(sent_share_invitation_id),
+    sent_share_invitation=invitation)
+
+invitation_response = invitation_request.result()
+created_invitation = json.loads(invitation_response)
+print(created_invitation)
+```
+### Send Share Invitation to a Service
+
+Data providers can also extend invitations to services or applications by specifying the tenant id and object id of the service. _The object id used for sending an invitation to a service must be the object id associated with the Enterprise Application (not the application registration)._
+
+```python Snippet:send_a_service_invitation
+import os, uuid
+
+from azure.purview.sharing import PurviewSharingClient
+from azure.identity import DefaultAzureCredential
+
+endpoint = os.environ["ENDPOINT"]
+credential = DefaultAzureCredential()
+
+client = PurviewSharingClient(endpoint=endpoint, credential=credential)
+
+targetActiveDirectoryId = uuid.uuid4()
+targetObjectId = uuid.uuid4()
+
+sent_share_invitation = {
+    "invitationKind": "Service",
+    "properties": {
+        "targetActiveDirectoryId": str(targetActiveDirectoryId),
+        "targetObjectId": str(targetObjectId)
+    }
+}
+
+invitation_response = client.sent_shares.create_invitation(
+    sent_share_id=str(sent_share_id),
+    sent_share_invitation_id=str(sent_share_invitation_id),
+    sent_share_invitation=sent_share_invitation)
+
+print(invitation_response)
+```
+
+### Get Sent Share
+
+After creating a sent share, data providers can retrieve it.
 
 ```python Snippet:get_a_sent_share
 import os, uuid
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
@@ -106,15 +208,17 @@
 
 client = PurviewSharingClient(endpoint=endpoint, credential=credential)
 
 retrieved_sent_share = client.sent_shares.get(sent_share_id=str(sent_share_id))
 print(retrieved_sent_share)
 ```
 
-### List sent shares
+### List Sent Shares
+
+Data providers can also retrieve a list of the sent shares they have created.
 
 ```python Snippet:get_all_sent_shares
 import os
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
@@ -129,53 +233,65 @@
     reference_name=provider_storage_account_resource_id,
     orderby="properties/createdAt desc")
 
 for list_response in list_request:
     print(list_response)
 ```
 
-### Create sent share invitation
+### Delete Sent Share
 
-```python Snippet:send_a_user_invitation
+A sent share can be deleted by the data provider to stop sharing their data with all data consumers.
+
+```python Snippet:delete_a_sent_share
 import os
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
-from datetime import date
 
 endpoint = os.environ["ENDPOINT"]
 credential = DefaultAzureCredential()
 
-client = PurviewSharingClient(endpoint=endpoint, credential=credential)
+client = PurviewSharingClient(endpoint=endpoint,credential=credential)
 
 sent_share_id = uuid.uuid4()
-sent_share_invitation_id = uuid.uuid4()
 
-consumerEmail = "consumer@contoso.com"
-today = date.today()
-invitation = {
-    "invitationKind": "User",
-    "properties": {
-        "targetEmail": consumerEmail,
-        "notify": "true",
-        "expirationDate": date(today.year+1,today.month,today.day).strftime("%Y-%m-%d") + " 00:00:00"
-    }
-}
+delete_request = client.sent_shares.begin_delete(sent_share_id=str(sent_share_id))
+delete_response = delete_request.result()
+print(delete_response)
+```
 
-invitation_request = client.sent_shares.create_invitation(
-    sent_share_id=str(sent_share_id),
-    sent_share_invitation_id=str(sent_share_invitation_id),
-    sent_share_invitation=invitation)
+### Get Sent Share Invitation
 
-invitation_response = invitation_request.result()
-created_invitation = json.loads(invitation_response)
-print(created_invitation)
+After creating a sent share invitation, data providers can retrieve it.
+
+```python Snippet:get_a_sent_share_invitation
+import os, uuid, json
+
+from azure.purview.sharing import PurviewSharingClient
+from azure.identity import DefaultAzureCredential
+
+endpoint = os.environ["ENDPOINT"]
+credential = DefaultAzureCredential()
+
+client = PurviewSharingClient(endpoint=endpoint,credential=credential)
+
+sent_share_id = uuid.uuid4()
+sent_share_invitation_id = uuid.uuid4()
+
+get_invitation_response = client.sent_shares.get_invitation(
+    sent_share_id=str(sent_share_id), 
+    sent_share_invitation_id=str(sent_share_invitation_id))
+
+retrieved_share_invitation = json.loads(get_invitation_response)
+print(retrieved_share_invitation)
 ```
 
-### List sent share invitations
+### List Sent Share Invitations
+
+Data providers can also retrieve a list of the sent share invitations they have created.
 
 ```python Snippet:view_sent_invitations
 import os, uuid, json
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
@@ -188,15 +304,60 @@
 
 list_request = client.sent_shares.list_invitations(sent_share_id=str(sent_share_id))
 
 for list_response in list_request:
     print(list_response)
 ```
 
-### List received shares
+### Delete Sent Share Invitation
+
+An individual sent share invitation can be deleted by the data provider to stop sharing their data with the specific data consumer to whom the invitation was addressed.
+
+```python Snippet:delete_a_sent_share_invitation
+import os, uuid, json
+
+from azure.purview.sharing import PurviewSharingClient
+from azure.identity import DefaultAzureCredential
+
+endpoint = os.environ["ENDPOINT"]
+credential = DefaultAzureCredential()
+
+client = PurviewSharingClient(endpoint=endpoint,credential=credential)
+
+sent_share_id = uuid.uuid4()
+sent_share_invitation_id = uuid.uuid4()
+
+delete_invitation_request = client.sent_shares.begin_delete_invitation(
+    sent_share_id=str(sent_share_id),
+    sent_share_invitation_id=str(sent_share_invitation_id))
+delete_invitation_response = delete_invitation_request.result()
+print(delete_invitation_response)
+```
+
+## Data Consumer Examples
+
+The following code examples demonstrate how data consumers can use the Microsoft Azure Python SDK for Purview Sharing to manage their sharing activity.
+
+### Create a Received Share Client
+
+```python Snippet:create_received_share_client
+import os
+
+from azure.purview.sharing import PurviewSharingClient
+from azure.identity import DefaultAzureCredential
+
+endpoint = os.environ["ENDPOINT"]
+credential = DefaultAzureCredential()
+
+client = PurviewSharingClient(endpoint=endpoint,credential=credential)
+```
+
+### List Detached Received Shares
+
+To begin viewing data shared with them, a data consumer must first retrieve a list of detached received shares. Within this list, they can identify a detached received share to attach. A "detached" received share refers to a received share that has never been attached or has been detached.
 
 ```python Snippet:get_all_detached_received_shares
 import os
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
@@ -205,15 +366,17 @@
 
 client = PurviewSharingClient(endpoint=endpoint,credential=credential)
 
 list_detached_response = client.received_shares.list_detached(orderby="properties/createdAt desc")
 print(list_detached_response)
 ```
 
-### Attach a received share
+### Attach a Received Share
+
+Once the data consumer has identified a received share, they can attach the received share to a location where they can access the shared data. If the received share is already attached, the shared data will be made accessible at the new location specified.
 
 ```python Snippet:attach_a_received_share
 import os, json
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
@@ -249,15 +412,17 @@
     content_type="application/json",
     content=json.dumps(received_share))
 
 update_response = update_request.result()
 print(update_response)
 ```
 
-### Get received share
+### Get Received Share
+
+A data consumer can retrieve an individual received share.
 
 ```python Snippet:get_a_received_share
 import os
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
@@ -271,15 +436,17 @@
 received_share = list_detached[0]
 
 get_share_response = client.received_shares.get(received_share_id=received_share['id'])
 retrieved_share = json.loads(get_share_response)
 print(retrieved_share)
 ```
 
-### List attached shares
+### List Attached Received Shares
+
+Data consumers can also retrieve a list of their attached received shares.
 
 ```python Snippet:list_attached_received_shares
 import os
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
@@ -292,15 +459,17 @@
 
 list_attached_response = client.received_shares.list_attached(
     reference_name=consumer_storage_account_resource_id,
     orderby="properties/createdAt desc")
 print(list_attached_response)
 ```
 
-### Delete received share
+### Delete Received Share
+
+A received share can be deleted by the data consumer to terminate their access to shared data.
 
 ```python Snippet:delete_a_received_share
 import os
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
@@ -310,32 +479,39 @@
 client = PurviewSharingClient(endpoint=endpoint,credential=credential)
 
 delete_received_share_request = client.received_shares.begin_delete(received_share_id=received_share['id'])
 delete_received_share_response = delete_received_share_request.result()
 print(delete_received_share_response)
 ```
 
-### Delete sent share
+## Share Resource Examples
 
-```python Snippet:delete_a_sent_share
+The following code examples demonstrate how to use the Microsoft Azure Python SDK for Purview Sharing to view share resources. A share resource is the underlying resource from which a provider shares data or the destination where a consumer attaches data shared with them.
+
+### List Share Resources
+
+A list of share resources can be retrieved to view all resources within an account where sharing activities have taken place.
+
+```python Snippet:list_share_resources
 import os
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
 endpoint = os.environ["ENDPOINT"]
 credential = DefaultAzureCredential()
 
 client = PurviewSharingClient(endpoint=endpoint,credential=credential)
 
-sent_share_id="885E60CB-2001-4192-B95D-B98CE316C783"
+list_request = client.share_resources.list(
+    filter="properties/storeKind eq 'AdlsGen2Account'",
+    orderby="properties/createdAt desc")
 
-delete_request = client.sent_shares.begin_delete(sent_share_id=str(sent_share_id))
-delete_response = delete_request.result()
-print(delete_response)
+for list_response in list_request:
+    print(list_response)
 ```
 
 ## Troubleshooting
 
 ### General
 
 The Purview Catalog client will raise exceptions defined in [Azure Core][azure_core] if you call `.raise_for_status()` on your responses.
@@ -398,17 +574,17 @@
 [sharing_product_documentation]: https://azure.microsoft.com/services/purview/
 [azure_subscription]: https://azure.microsoft.com/free/
 [purview_resource]: https://docs.microsoft.com/azure/purview
 [pip]: https://pypi.org/project/pip/
 [authenticate_with_token]: https://docs.microsoft.com/azure/cognitive-services/authentication?tabs=powershell#authenticate-with-an-authentication-token
 [azure_identity_credentials]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/identity/azure-identity#credentials
 [azure_identity_pip]: https://pypi.org/project/azure-identity/
-[default_azure_credential]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/identity/azure-identity#defaultazurecredential
+[default_azure_credential]: https://azuresdkdocs.blob.core.windows.net/$web/python/azure-identity/latest/azure.identity.html#azure.identity.DefaultAzureCredential
 [request_builders_and_client]: https://aka.ms/azsdk/python/protocol/quickstart
 [enable_aad]: https://docs.microsoft.com/azure/purview/
 [azure_core]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/core/azure-core/README.md
 [python_logging]: https://docs.python.org/3.5/library/logging.html
 [cla]: https://cla.microsoft.com
 [code_of_conduct]: https://opensource.microsoft.com/codeofconduct/
 [coc_faq]: https://opensource.microsoft.com/codeofconduct/faq/
 [coc_contact]: mailto:opencode@microsoft.com
-[samples]: https://github.com/yamanwahsheh/azure-sdk-for-python/tree/yaman/share-v2-python-tests-and-samples/sdk/purview/azure-purview-sharing/samples
+[samples]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/purview/azure-purview-sharing/samples
```

## Comparing `azure-purview-sharing-1.0.0b2/PKG-INFO` & `azure-purview-sharing-1.0.0b3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-purview-sharing
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: Microsoft Azure Purview Sharing Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -21,15 +21,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Azure Purview Sharing client library for Python
 
 Microsoft Purview Share is a fully managed cloud service.
 
-**Please rely heavily on the [service's documentation][sharing_product_documentation] and our [protocol client docs][protocol_client_quickstart] to use this library**
+**Please rely heavily on the [service's documentation][sharing_product_documentation] and our [protocol client docs][request_builders_and_client] to use this library**
 
 [Source code][source_code] | [Package (PyPI)][client_pypi_package] | [Product documentation][sharing_product_documentation]
 
 ## Getting started
 
 ### Install the package
 
@@ -44,33 +44,60 @@
 - You must have an [Azure subscription][azure_subscription] and a [Purview resource][purview_resource] to use this package.
 - Python 3.6 or later is required to use this package.
 
 ### Authenticate the client
 
 #### Using Azure Active Directory
 
-This document demonstrates using [DefaultAzureCredential][default_cred_ref] to authenticate via Azure Active Directory. However, any of the credentials offered by the [azure_identity][azure_identity] will be accepted.  See the [azure_identity][azure_identity] documentation for more information about other credentials.
+This document demonstrates using [DefaultAzureCredential][default_azure_credential] to authenticate via Azure Active Directory. However, any of the credentials offered by the [azure-identity package][azure_identity_pip] will be accepted.  See the [azure-identity][azure_identity_credentials] documentation for more information about other credentials.
 
 Once you have chosen and configured your credential, you can create instances of the `PurviewSharingClient`.
 
 ```python
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
 credential = DefaultAzureCredential()
 client = PurviewSharingClient(endpoint="https://<my-account-name>.purview.azure.com", credential=credential)
 ```
 
 ## Key concepts
 
+**Data Provider:** A data provider is the individual who creates a share by selecting a data source, choosing which files and folders to share, and who to share them with. Microsoft Purview then sends an invitation to each data consumer.
+
+**Data Consumer:** A data consumer is the individual who accepts the invitation by specifying a target storage account in their own Azure subscription that they'll use to access the shared data.
+
 ## Examples
 
-The following section shows you how to initialize and authenticate your client and share data.
+Table of Contents: 
+- [Data Provider](#data-provider-examples)
+- [Data Consumer](#data-consumer-examples)
+- [Share Resource](#share-resource-examples)
+
+## Data Provider Examples
+
+The following code examples demonstrate how data providers can use the Microsoft Azure Python SDK for Purview Sharing to manage their sharing activity.
+
+### Create a Sent Share Client
+
+```python Snippet:create_a_sent_share_client
+import os, uuid, json
+
+from azure.purview.sharing import PurviewSharingClient
+from azure.identity import DefaultAzureCredential
+
+endpoint = os.environ["ENDPOINT"]
+credential = DefaultAzureCredential()
+
+client = PurviewSharingClient(endpoint=endpoint, credential=credential)
+```
+
+### Create Share
 
-### Create share
+To begin sharing data, the data provider must first create a sent share that identifies the data they would like to share.
 
 ```python Snippet:create_a_sent_share
 import os, uuid, json
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
@@ -111,15 +138,90 @@
     str(sent_share_id),
     sent_share=sent_share)
 
 response = request.result()
 print(response)
 ```
 
-### Get sent share
+### Send Share Invitation to a User
+
+After creating a sent share, the data provider can extend invitations to consumers who may then view the shared data. In this example, an invitation is extended to an individual by specifying their email address.
+
+```python Snippet:send_a_user_invitation
+import os, uuid
+
+from azure.purview.sharing import PurviewSharingClient
+from azure.identity import DefaultAzureCredential
+from datetime import date
+
+endpoint = os.environ["ENDPOINT"]
+credential = DefaultAzureCredential()
+
+client = PurviewSharingClient(endpoint=endpoint, credential=credential)
+
+sent_share_id = uuid.uuid4()
+sent_share_invitation_id = uuid.uuid4()
+
+consumerEmail = "consumer@contoso.com"
+today = date.today()
+invitation = {
+    "invitationKind": "User",
+    "properties": {
+        "targetEmail": consumerEmail,
+        "notify": "true",
+        "expirationDate": date(today.year+1,today.month,today.day).strftime("%Y-%m-%d") + " 00:00:00"
+    }
+}
+
+invitation_request = client.sent_shares.create_invitation(
+    sent_share_id=str(sent_share_id),
+    sent_share_invitation_id=str(sent_share_invitation_id),
+    sent_share_invitation=invitation)
+
+invitation_response = invitation_request.result()
+created_invitation = json.loads(invitation_response)
+print(created_invitation)
+```
+### Send Share Invitation to a Service
+
+Data providers can also extend invitations to services or applications by specifying the tenant id and object id of the service. _The object id used for sending an invitation to a service must be the object id associated with the Enterprise Application (not the application registration)._
+
+```python Snippet:send_a_service_invitation
+import os, uuid
+
+from azure.purview.sharing import PurviewSharingClient
+from azure.identity import DefaultAzureCredential
+
+endpoint = os.environ["ENDPOINT"]
+credential = DefaultAzureCredential()
+
+client = PurviewSharingClient(endpoint=endpoint, credential=credential)
+
+targetActiveDirectoryId = uuid.uuid4()
+targetObjectId = uuid.uuid4()
+
+sent_share_invitation = {
+    "invitationKind": "Service",
+    "properties": {
+        "targetActiveDirectoryId": str(targetActiveDirectoryId),
+        "targetObjectId": str(targetObjectId)
+    }
+}
+
+invitation_response = client.sent_shares.create_invitation(
+    sent_share_id=str(sent_share_id),
+    sent_share_invitation_id=str(sent_share_invitation_id),
+    sent_share_invitation=sent_share_invitation)
+
+print(invitation_response)
+```
+
+### Get Sent Share
+
+After creating a sent share, data providers can retrieve it.
 
 ```python Snippet:get_a_sent_share
 import os, uuid
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
@@ -129,15 +231,17 @@
 
 client = PurviewSharingClient(endpoint=endpoint, credential=credential)
 
 retrieved_sent_share = client.sent_shares.get(sent_share_id=str(sent_share_id))
 print(retrieved_sent_share)
 ```
 
-### List sent shares
+### List Sent Shares
+
+Data providers can also retrieve a list of the sent shares they have created.
 
 ```python Snippet:get_all_sent_shares
 import os
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
@@ -152,53 +256,65 @@
     reference_name=provider_storage_account_resource_id,
     orderby="properties/createdAt desc")
 
 for list_response in list_request:
     print(list_response)
 ```
 
-### Create sent share invitation
+### Delete Sent Share
 
-```python Snippet:send_a_user_invitation
+A sent share can be deleted by the data provider to stop sharing their data with all data consumers.
+
+```python Snippet:delete_a_sent_share
 import os
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
-from datetime import date
 
 endpoint = os.environ["ENDPOINT"]
 credential = DefaultAzureCredential()
 
-client = PurviewSharingClient(endpoint=endpoint, credential=credential)
+client = PurviewSharingClient(endpoint=endpoint,credential=credential)
 
 sent_share_id = uuid.uuid4()
-sent_share_invitation_id = uuid.uuid4()
 
-consumerEmail = "consumer@contoso.com"
-today = date.today()
-invitation = {
-    "invitationKind": "User",
-    "properties": {
-        "targetEmail": consumerEmail,
-        "notify": "true",
-        "expirationDate": date(today.year+1,today.month,today.day).strftime("%Y-%m-%d") + " 00:00:00"
-    }
-}
+delete_request = client.sent_shares.begin_delete(sent_share_id=str(sent_share_id))
+delete_response = delete_request.result()
+print(delete_response)
+```
 
-invitation_request = client.sent_shares.create_invitation(
-    sent_share_id=str(sent_share_id),
-    sent_share_invitation_id=str(sent_share_invitation_id),
-    sent_share_invitation=invitation)
+### Get Sent Share Invitation
 
-invitation_response = invitation_request.result()
-created_invitation = json.loads(invitation_response)
-print(created_invitation)
+After creating a sent share invitation, data providers can retrieve it.
+
+```python Snippet:get_a_sent_share_invitation
+import os, uuid, json
+
+from azure.purview.sharing import PurviewSharingClient
+from azure.identity import DefaultAzureCredential
+
+endpoint = os.environ["ENDPOINT"]
+credential = DefaultAzureCredential()
+
+client = PurviewSharingClient(endpoint=endpoint,credential=credential)
+
+sent_share_id = uuid.uuid4()
+sent_share_invitation_id = uuid.uuid4()
+
+get_invitation_response = client.sent_shares.get_invitation(
+    sent_share_id=str(sent_share_id), 
+    sent_share_invitation_id=str(sent_share_invitation_id))
+
+retrieved_share_invitation = json.loads(get_invitation_response)
+print(retrieved_share_invitation)
 ```
 
-### List sent share invitations
+### List Sent Share Invitations
+
+Data providers can also retrieve a list of the sent share invitations they have created.
 
 ```python Snippet:view_sent_invitations
 import os, uuid, json
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
@@ -211,15 +327,60 @@
 
 list_request = client.sent_shares.list_invitations(sent_share_id=str(sent_share_id))
 
 for list_response in list_request:
     print(list_response)
 ```
 
-### List received shares
+### Delete Sent Share Invitation
+
+An individual sent share invitation can be deleted by the data provider to stop sharing their data with the specific data consumer to whom the invitation was addressed.
+
+```python Snippet:delete_a_sent_share_invitation
+import os, uuid, json
+
+from azure.purview.sharing import PurviewSharingClient
+from azure.identity import DefaultAzureCredential
+
+endpoint = os.environ["ENDPOINT"]
+credential = DefaultAzureCredential()
+
+client = PurviewSharingClient(endpoint=endpoint,credential=credential)
+
+sent_share_id = uuid.uuid4()
+sent_share_invitation_id = uuid.uuid4()
+
+delete_invitation_request = client.sent_shares.begin_delete_invitation(
+    sent_share_id=str(sent_share_id),
+    sent_share_invitation_id=str(sent_share_invitation_id))
+delete_invitation_response = delete_invitation_request.result()
+print(delete_invitation_response)
+```
+
+## Data Consumer Examples
+
+The following code examples demonstrate how data consumers can use the Microsoft Azure Python SDK for Purview Sharing to manage their sharing activity.
+
+### Create a Received Share Client
+
+```python Snippet:create_received_share_client
+import os
+
+from azure.purview.sharing import PurviewSharingClient
+from azure.identity import DefaultAzureCredential
+
+endpoint = os.environ["ENDPOINT"]
+credential = DefaultAzureCredential()
+
+client = PurviewSharingClient(endpoint=endpoint,credential=credential)
+```
+
+### List Detached Received Shares
+
+To begin viewing data shared with them, a data consumer must first retrieve a list of detached received shares. Within this list, they can identify a detached received share to attach. A "detached" received share refers to a received share that has never been attached or has been detached.
 
 ```python Snippet:get_all_detached_received_shares
 import os
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
@@ -228,15 +389,17 @@
 
 client = PurviewSharingClient(endpoint=endpoint,credential=credential)
 
 list_detached_response = client.received_shares.list_detached(orderby="properties/createdAt desc")
 print(list_detached_response)
 ```
 
-### Attach a received share
+### Attach a Received Share
+
+Once the data consumer has identified a received share, they can attach the received share to a location where they can access the shared data. If the received share is already attached, the shared data will be made accessible at the new location specified.
 
 ```python Snippet:attach_a_received_share
 import os, json
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
@@ -272,15 +435,17 @@
     content_type="application/json",
     content=json.dumps(received_share))
 
 update_response = update_request.result()
 print(update_response)
 ```
 
-### Get received share
+### Get Received Share
+
+A data consumer can retrieve an individual received share.
 
 ```python Snippet:get_a_received_share
 import os
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
@@ -294,15 +459,17 @@
 received_share = list_detached[0]
 
 get_share_response = client.received_shares.get(received_share_id=received_share['id'])
 retrieved_share = json.loads(get_share_response)
 print(retrieved_share)
 ```
 
-### List attached shares
+### List Attached Received Shares
+
+Data consumers can also retrieve a list of their attached received shares.
 
 ```python Snippet:list_attached_received_shares
 import os
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
@@ -315,15 +482,17 @@
 
 list_attached_response = client.received_shares.list_attached(
     reference_name=consumer_storage_account_resource_id,
     orderby="properties/createdAt desc")
 print(list_attached_response)
 ```
 
-### Delete received share
+### Delete Received Share
+
+A received share can be deleted by the data consumer to terminate their access to shared data.
 
 ```python Snippet:delete_a_received_share
 import os
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
@@ -333,32 +502,39 @@
 client = PurviewSharingClient(endpoint=endpoint,credential=credential)
 
 delete_received_share_request = client.received_shares.begin_delete(received_share_id=received_share['id'])
 delete_received_share_response = delete_received_share_request.result()
 print(delete_received_share_response)
 ```
 
-### Delete sent share
+## Share Resource Examples
 
-```python Snippet:delete_a_sent_share
+The following code examples demonstrate how to use the Microsoft Azure Python SDK for Purview Sharing to view share resources. A share resource is the underlying resource from which a provider shares data or the destination where a consumer attaches data shared with them.
+
+### List Share Resources
+
+A list of share resources can be retrieved to view all resources within an account where sharing activities have taken place.
+
+```python Snippet:list_share_resources
 import os
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
 endpoint = os.environ["ENDPOINT"]
 credential = DefaultAzureCredential()
 
 client = PurviewSharingClient(endpoint=endpoint,credential=credential)
 
-sent_share_id="885E60CB-2001-4192-B95D-B98CE316C783"
+list_request = client.share_resources.list(
+    filter="properties/storeKind eq 'AdlsGen2Account'",
+    orderby="properties/createdAt desc")
 
-delete_request = client.sent_shares.begin_delete(sent_share_id=str(sent_share_id))
-delete_response = delete_request.result()
-print(delete_response)
+for list_response in list_request:
+    print(list_response)
 ```
 
 ## Troubleshooting
 
 ### General
 
 The Purview Catalog client will raise exceptions defined in [Azure Core][azure_core] if you call `.raise_for_status()` on your responses.
@@ -421,17 +597,17 @@
 [sharing_product_documentation]: https://azure.microsoft.com/services/purview/
 [azure_subscription]: https://azure.microsoft.com/free/
 [purview_resource]: https://docs.microsoft.com/azure/purview
 [pip]: https://pypi.org/project/pip/
 [authenticate_with_token]: https://docs.microsoft.com/azure/cognitive-services/authentication?tabs=powershell#authenticate-with-an-authentication-token
 [azure_identity_credentials]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/identity/azure-identity#credentials
 [azure_identity_pip]: https://pypi.org/project/azure-identity/
-[default_azure_credential]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/identity/azure-identity#defaultazurecredential
+[default_azure_credential]: https://azuresdkdocs.blob.core.windows.net/$web/python/azure-identity/latest/azure.identity.html#azure.identity.DefaultAzureCredential
 [request_builders_and_client]: https://aka.ms/azsdk/python/protocol/quickstart
 [enable_aad]: https://docs.microsoft.com/azure/purview/
 [azure_core]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/core/azure-core/README.md
 [python_logging]: https://docs.python.org/3.5/library/logging.html
 [cla]: https://cla.microsoft.com
 [code_of_conduct]: https://opensource.microsoft.com/codeofconduct/
 [coc_faq]: https://opensource.microsoft.com/codeofconduct/faq/
 [coc_contact]: mailto:opencode@microsoft.com
-[samples]: https://github.com/yamanwahsheh/azure-sdk-for-python/tree/yaman/share-v2-python-tests-and-samples/sdk/purview/azure-purview-sharing/samples
+[samples]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/purview/azure-purview-sharing/samples
```

## Comparing `azure-purview-sharing-1.0.0b2/LICENSE` & `azure-purview-sharing-1.0.0b3/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-purview-sharing-1.0.0b2/setup.py` & `azure-purview-sharing-1.0.0b3/setup.py`

 * *Files identical despite different names*

## Comparing `azure-purview-sharing-1.0.0b2/azure_purview_sharing.egg-info/PKG-INFO` & `azure-purview-sharing-1.0.0b3/azure_purview_sharing.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-purview-sharing
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: Microsoft Azure Purview Sharing Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -21,15 +21,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Azure Purview Sharing client library for Python
 
 Microsoft Purview Share is a fully managed cloud service.
 
-**Please rely heavily on the [service's documentation][sharing_product_documentation] and our [protocol client docs][protocol_client_quickstart] to use this library**
+**Please rely heavily on the [service's documentation][sharing_product_documentation] and our [protocol client docs][request_builders_and_client] to use this library**
 
 [Source code][source_code] | [Package (PyPI)][client_pypi_package] | [Product documentation][sharing_product_documentation]
 
 ## Getting started
 
 ### Install the package
 
@@ -44,33 +44,60 @@
 - You must have an [Azure subscription][azure_subscription] and a [Purview resource][purview_resource] to use this package.
 - Python 3.6 or later is required to use this package.
 
 ### Authenticate the client
 
 #### Using Azure Active Directory
 
-This document demonstrates using [DefaultAzureCredential][default_cred_ref] to authenticate via Azure Active Directory. However, any of the credentials offered by the [azure_identity][azure_identity] will be accepted.  See the [azure_identity][azure_identity] documentation for more information about other credentials.
+This document demonstrates using [DefaultAzureCredential][default_azure_credential] to authenticate via Azure Active Directory. However, any of the credentials offered by the [azure-identity package][azure_identity_pip] will be accepted.  See the [azure-identity][azure_identity_credentials] documentation for more information about other credentials.
 
 Once you have chosen and configured your credential, you can create instances of the `PurviewSharingClient`.
 
 ```python
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
 credential = DefaultAzureCredential()
 client = PurviewSharingClient(endpoint="https://<my-account-name>.purview.azure.com", credential=credential)
 ```
 
 ## Key concepts
 
+**Data Provider:** A data provider is the individual who creates a share by selecting a data source, choosing which files and folders to share, and who to share them with. Microsoft Purview then sends an invitation to each data consumer.
+
+**Data Consumer:** A data consumer is the individual who accepts the invitation by specifying a target storage account in their own Azure subscription that they'll use to access the shared data.
+
 ## Examples
 
-The following section shows you how to initialize and authenticate your client and share data.
+Table of Contents: 
+- [Data Provider](#data-provider-examples)
+- [Data Consumer](#data-consumer-examples)
+- [Share Resource](#share-resource-examples)
+
+## Data Provider Examples
+
+The following code examples demonstrate how data providers can use the Microsoft Azure Python SDK for Purview Sharing to manage their sharing activity.
+
+### Create a Sent Share Client
+
+```python Snippet:create_a_sent_share_client
+import os, uuid, json
+
+from azure.purview.sharing import PurviewSharingClient
+from azure.identity import DefaultAzureCredential
+
+endpoint = os.environ["ENDPOINT"]
+credential = DefaultAzureCredential()
+
+client = PurviewSharingClient(endpoint=endpoint, credential=credential)
+```
+
+### Create Share
 
-### Create share
+To begin sharing data, the data provider must first create a sent share that identifies the data they would like to share.
 
 ```python Snippet:create_a_sent_share
 import os, uuid, json
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
@@ -111,15 +138,90 @@
     str(sent_share_id),
     sent_share=sent_share)
 
 response = request.result()
 print(response)
 ```
 
-### Get sent share
+### Send Share Invitation to a User
+
+After creating a sent share, the data provider can extend invitations to consumers who may then view the shared data. In this example, an invitation is extended to an individual by specifying their email address.
+
+```python Snippet:send_a_user_invitation
+import os, uuid
+
+from azure.purview.sharing import PurviewSharingClient
+from azure.identity import DefaultAzureCredential
+from datetime import date
+
+endpoint = os.environ["ENDPOINT"]
+credential = DefaultAzureCredential()
+
+client = PurviewSharingClient(endpoint=endpoint, credential=credential)
+
+sent_share_id = uuid.uuid4()
+sent_share_invitation_id = uuid.uuid4()
+
+consumerEmail = "consumer@contoso.com"
+today = date.today()
+invitation = {
+    "invitationKind": "User",
+    "properties": {
+        "targetEmail": consumerEmail,
+        "notify": "true",
+        "expirationDate": date(today.year+1,today.month,today.day).strftime("%Y-%m-%d") + " 00:00:00"
+    }
+}
+
+invitation_request = client.sent_shares.create_invitation(
+    sent_share_id=str(sent_share_id),
+    sent_share_invitation_id=str(sent_share_invitation_id),
+    sent_share_invitation=invitation)
+
+invitation_response = invitation_request.result()
+created_invitation = json.loads(invitation_response)
+print(created_invitation)
+```
+### Send Share Invitation to a Service
+
+Data providers can also extend invitations to services or applications by specifying the tenant id and object id of the service. _The object id used for sending an invitation to a service must be the object id associated with the Enterprise Application (not the application registration)._
+
+```python Snippet:send_a_service_invitation
+import os, uuid
+
+from azure.purview.sharing import PurviewSharingClient
+from azure.identity import DefaultAzureCredential
+
+endpoint = os.environ["ENDPOINT"]
+credential = DefaultAzureCredential()
+
+client = PurviewSharingClient(endpoint=endpoint, credential=credential)
+
+targetActiveDirectoryId = uuid.uuid4()
+targetObjectId = uuid.uuid4()
+
+sent_share_invitation = {
+    "invitationKind": "Service",
+    "properties": {
+        "targetActiveDirectoryId": str(targetActiveDirectoryId),
+        "targetObjectId": str(targetObjectId)
+    }
+}
+
+invitation_response = client.sent_shares.create_invitation(
+    sent_share_id=str(sent_share_id),
+    sent_share_invitation_id=str(sent_share_invitation_id),
+    sent_share_invitation=sent_share_invitation)
+
+print(invitation_response)
+```
+
+### Get Sent Share
+
+After creating a sent share, data providers can retrieve it.
 
 ```python Snippet:get_a_sent_share
 import os, uuid
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
@@ -129,15 +231,17 @@
 
 client = PurviewSharingClient(endpoint=endpoint, credential=credential)
 
 retrieved_sent_share = client.sent_shares.get(sent_share_id=str(sent_share_id))
 print(retrieved_sent_share)
 ```
 
-### List sent shares
+### List Sent Shares
+
+Data providers can also retrieve a list of the sent shares they have created.
 
 ```python Snippet:get_all_sent_shares
 import os
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
@@ -152,53 +256,65 @@
     reference_name=provider_storage_account_resource_id,
     orderby="properties/createdAt desc")
 
 for list_response in list_request:
     print(list_response)
 ```
 
-### Create sent share invitation
+### Delete Sent Share
 
-```python Snippet:send_a_user_invitation
+A sent share can be deleted by the data provider to stop sharing their data with all data consumers.
+
+```python Snippet:delete_a_sent_share
 import os
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
-from datetime import date
 
 endpoint = os.environ["ENDPOINT"]
 credential = DefaultAzureCredential()
 
-client = PurviewSharingClient(endpoint=endpoint, credential=credential)
+client = PurviewSharingClient(endpoint=endpoint,credential=credential)
 
 sent_share_id = uuid.uuid4()
-sent_share_invitation_id = uuid.uuid4()
 
-consumerEmail = "consumer@contoso.com"
-today = date.today()
-invitation = {
-    "invitationKind": "User",
-    "properties": {
-        "targetEmail": consumerEmail,
-        "notify": "true",
-        "expirationDate": date(today.year+1,today.month,today.day).strftime("%Y-%m-%d") + " 00:00:00"
-    }
-}
+delete_request = client.sent_shares.begin_delete(sent_share_id=str(sent_share_id))
+delete_response = delete_request.result()
+print(delete_response)
+```
 
-invitation_request = client.sent_shares.create_invitation(
-    sent_share_id=str(sent_share_id),
-    sent_share_invitation_id=str(sent_share_invitation_id),
-    sent_share_invitation=invitation)
+### Get Sent Share Invitation
 
-invitation_response = invitation_request.result()
-created_invitation = json.loads(invitation_response)
-print(created_invitation)
+After creating a sent share invitation, data providers can retrieve it.
+
+```python Snippet:get_a_sent_share_invitation
+import os, uuid, json
+
+from azure.purview.sharing import PurviewSharingClient
+from azure.identity import DefaultAzureCredential
+
+endpoint = os.environ["ENDPOINT"]
+credential = DefaultAzureCredential()
+
+client = PurviewSharingClient(endpoint=endpoint,credential=credential)
+
+sent_share_id = uuid.uuid4()
+sent_share_invitation_id = uuid.uuid4()
+
+get_invitation_response = client.sent_shares.get_invitation(
+    sent_share_id=str(sent_share_id), 
+    sent_share_invitation_id=str(sent_share_invitation_id))
+
+retrieved_share_invitation = json.loads(get_invitation_response)
+print(retrieved_share_invitation)
 ```
 
-### List sent share invitations
+### List Sent Share Invitations
+
+Data providers can also retrieve a list of the sent share invitations they have created.
 
 ```python Snippet:view_sent_invitations
 import os, uuid, json
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
@@ -211,15 +327,60 @@
 
 list_request = client.sent_shares.list_invitations(sent_share_id=str(sent_share_id))
 
 for list_response in list_request:
     print(list_response)
 ```
 
-### List received shares
+### Delete Sent Share Invitation
+
+An individual sent share invitation can be deleted by the data provider to stop sharing their data with the specific data consumer to whom the invitation was addressed.
+
+```python Snippet:delete_a_sent_share_invitation
+import os, uuid, json
+
+from azure.purview.sharing import PurviewSharingClient
+from azure.identity import DefaultAzureCredential
+
+endpoint = os.environ["ENDPOINT"]
+credential = DefaultAzureCredential()
+
+client = PurviewSharingClient(endpoint=endpoint,credential=credential)
+
+sent_share_id = uuid.uuid4()
+sent_share_invitation_id = uuid.uuid4()
+
+delete_invitation_request = client.sent_shares.begin_delete_invitation(
+    sent_share_id=str(sent_share_id),
+    sent_share_invitation_id=str(sent_share_invitation_id))
+delete_invitation_response = delete_invitation_request.result()
+print(delete_invitation_response)
+```
+
+## Data Consumer Examples
+
+The following code examples demonstrate how data consumers can use the Microsoft Azure Python SDK for Purview Sharing to manage their sharing activity.
+
+### Create a Received Share Client
+
+```python Snippet:create_received_share_client
+import os
+
+from azure.purview.sharing import PurviewSharingClient
+from azure.identity import DefaultAzureCredential
+
+endpoint = os.environ["ENDPOINT"]
+credential = DefaultAzureCredential()
+
+client = PurviewSharingClient(endpoint=endpoint,credential=credential)
+```
+
+### List Detached Received Shares
+
+To begin viewing data shared with them, a data consumer must first retrieve a list of detached received shares. Within this list, they can identify a detached received share to attach. A "detached" received share refers to a received share that has never been attached or has been detached.
 
 ```python Snippet:get_all_detached_received_shares
 import os
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
@@ -228,15 +389,17 @@
 
 client = PurviewSharingClient(endpoint=endpoint,credential=credential)
 
 list_detached_response = client.received_shares.list_detached(orderby="properties/createdAt desc")
 print(list_detached_response)
 ```
 
-### Attach a received share
+### Attach a Received Share
+
+Once the data consumer has identified a received share, they can attach the received share to a location where they can access the shared data. If the received share is already attached, the shared data will be made accessible at the new location specified.
 
 ```python Snippet:attach_a_received_share
 import os, json
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
@@ -272,15 +435,17 @@
     content_type="application/json",
     content=json.dumps(received_share))
 
 update_response = update_request.result()
 print(update_response)
 ```
 
-### Get received share
+### Get Received Share
+
+A data consumer can retrieve an individual received share.
 
 ```python Snippet:get_a_received_share
 import os
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
@@ -294,15 +459,17 @@
 received_share = list_detached[0]
 
 get_share_response = client.received_shares.get(received_share_id=received_share['id'])
 retrieved_share = json.loads(get_share_response)
 print(retrieved_share)
 ```
 
-### List attached shares
+### List Attached Received Shares
+
+Data consumers can also retrieve a list of their attached received shares.
 
 ```python Snippet:list_attached_received_shares
 import os
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
@@ -315,15 +482,17 @@
 
 list_attached_response = client.received_shares.list_attached(
     reference_name=consumer_storage_account_resource_id,
     orderby="properties/createdAt desc")
 print(list_attached_response)
 ```
 
-### Delete received share
+### Delete Received Share
+
+A received share can be deleted by the data consumer to terminate their access to shared data.
 
 ```python Snippet:delete_a_received_share
 import os
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
@@ -333,32 +502,39 @@
 client = PurviewSharingClient(endpoint=endpoint,credential=credential)
 
 delete_received_share_request = client.received_shares.begin_delete(received_share_id=received_share['id'])
 delete_received_share_response = delete_received_share_request.result()
 print(delete_received_share_response)
 ```
 
-### Delete sent share
+## Share Resource Examples
 
-```python Snippet:delete_a_sent_share
+The following code examples demonstrate how to use the Microsoft Azure Python SDK for Purview Sharing to view share resources. A share resource is the underlying resource from which a provider shares data or the destination where a consumer attaches data shared with them.
+
+### List Share Resources
+
+A list of share resources can be retrieved to view all resources within an account where sharing activities have taken place.
+
+```python Snippet:list_share_resources
 import os
 
 from azure.purview.sharing import PurviewSharingClient
 from azure.identity import DefaultAzureCredential
 
 endpoint = os.environ["ENDPOINT"]
 credential = DefaultAzureCredential()
 
 client = PurviewSharingClient(endpoint=endpoint,credential=credential)
 
-sent_share_id="885E60CB-2001-4192-B95D-B98CE316C783"
+list_request = client.share_resources.list(
+    filter="properties/storeKind eq 'AdlsGen2Account'",
+    orderby="properties/createdAt desc")
 
-delete_request = client.sent_shares.begin_delete(sent_share_id=str(sent_share_id))
-delete_response = delete_request.result()
-print(delete_response)
+for list_response in list_request:
+    print(list_response)
 ```
 
 ## Troubleshooting
 
 ### General
 
 The Purview Catalog client will raise exceptions defined in [Azure Core][azure_core] if you call `.raise_for_status()` on your responses.
@@ -421,17 +597,17 @@
 [sharing_product_documentation]: https://azure.microsoft.com/services/purview/
 [azure_subscription]: https://azure.microsoft.com/free/
 [purview_resource]: https://docs.microsoft.com/azure/purview
 [pip]: https://pypi.org/project/pip/
 [authenticate_with_token]: https://docs.microsoft.com/azure/cognitive-services/authentication?tabs=powershell#authenticate-with-an-authentication-token
 [azure_identity_credentials]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/identity/azure-identity#credentials
 [azure_identity_pip]: https://pypi.org/project/azure-identity/
-[default_azure_credential]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/identity/azure-identity#defaultazurecredential
+[default_azure_credential]: https://azuresdkdocs.blob.core.windows.net/$web/python/azure-identity/latest/azure.identity.html#azure.identity.DefaultAzureCredential
 [request_builders_and_client]: https://aka.ms/azsdk/python/protocol/quickstart
 [enable_aad]: https://docs.microsoft.com/azure/purview/
 [azure_core]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/core/azure-core/README.md
 [python_logging]: https://docs.python.org/3.5/library/logging.html
 [cla]: https://cla.microsoft.com
 [code_of_conduct]: https://opensource.microsoft.com/codeofconduct/
 [coc_faq]: https://opensource.microsoft.com/codeofconduct/faq/
 [coc_contact]: mailto:opencode@microsoft.com
-[samples]: https://github.com/yamanwahsheh/azure-sdk-for-python/tree/yaman/share-v2-python-tests-and-samples/sdk/purview/azure-purview-sharing/samples
+[samples]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/purview/azure-purview-sharing/samples
```

## Comparing `azure-purview-sharing-1.0.0b2/azure_purview_sharing.egg-info/SOURCES.txt` & `azure-purview-sharing-1.0.0b3/azure_purview_sharing.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -29,12 +29,14 @@
 azure_purview_sharing.egg-info/dependency_links.txt
 azure_purview_sharing.egg-info/not-zip-safe
 azure_purview_sharing.egg-info/requires.txt
 azure_purview_sharing.egg-info/top_level.txt
 samples/README.md
 samples/received_shares_examples.py
 samples/sent_shares_examples.py
+samples/share_resources_examples.py
 tests/_util.py
 tests/conftest.py
 tests/test_received_shares.py
 tests/test_sent_shares.py
+tests/test_share_resources.py
 tests/testcase.py
```

## Comparing `azure-purview-sharing-1.0.0b2/tests/test_sent_shares.py` & `azure-purview-sharing-1.0.0b3/tests/test_sent_shares.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 # coding: utf-8
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # -------------------------------------------------------------------------
 import json
+from uuid import uuid4
 
 from testcase import TestPurviewSharing, PurviewSharingPowerShellPreparer
 from devtools_testutils import recorded_by_proxy
 from azure.core.exceptions import HttpResponseError
 from azure.purview.sharing.operations._operations import (
     build_sent_shares_create_or_replace_request,
     build_sent_shares_create_invitation_request,
     build_sent_shares_get_request,
     build_sent_shares_list_request,
     build_sent_shares_delete_request,
-    build_sent_shares_list_invitations_request
+    build_sent_shares_delete_invitation_request,
+    build_sent_shares_list_invitations_request,
+    build_sent_shares_get_invitation_request
 )
 
 class TestSentShares(TestPurviewSharing):
-    
     @PurviewSharingPowerShellPreparer()
     @recorded_by_proxy
     def test_create_sent_share(self, purviewsharing_endpoint):
         client = self.create_client(endpoint=purviewsharing_endpoint)
-        sent_share_id = "80084f86-e411-4447-82d3-a98a84651bf8"
+        sent_share_id = "541fd873-afa4-4d41-8b67-70d2302154c4" # uuid4()
         sent_share = self.prepare_sent_share()
 
         request = build_sent_shares_create_or_replace_request(
             sent_share_id,
             content_type="application/json",
             content=json.dumps(sent_share))
         
@@ -43,16 +45,16 @@
         assert created_sent_share is not None
         assert created_sent_share['id'] == str(sent_share_id)
 
     @PurviewSharingPowerShellPreparer()
     @recorded_by_proxy
     def test_create_sent_share_user_invitation(self, purviewsharing_endpoint):
         client = self.create_client(endpoint=purviewsharing_endpoint)
-        sent_share_id = "9e27ea94-c7dd-4e45-9564-30e280c37d1e"
-        sent_share_invitation_id = "9fb3755e-2f13-4cea-9b65-e45ed9a3dd01"
+        sent_share_id = "37061299-7990-4edd-b14c-2edf02edf162" # uuid4()
+        sent_share_invitation_id = "f3275be4-b54d-4620-bf50-ec478f8c12a6" #uuid4()
         sent_share = self.prepare_sent_share()
 
         request = build_sent_shares_create_or_replace_request(
             sent_share_id,
             content_type="application/json",
             content=json.dumps(sent_share))
         
@@ -89,15 +91,15 @@
         assert created_invitation['id'] == str(sent_share_invitation_id)
         assert created_invitation['properties']['targetEmail'] == consumerEmail
 
     @PurviewSharingPowerShellPreparer()
     @recorded_by_proxy
     def test_get_sent_share(self, purviewsharing_endpoint):
         client = self.create_client(endpoint=purviewsharing_endpoint)
-        sent_share_id = "8b3af6c7-1935-4ae9-8940-46373253520c"
+        sent_share_id = "41211a38-0125-45a0-b748-b6008cf107c7" # uuid4()
         sent_share = self.prepare_sent_share()
 
         request = build_sent_shares_create_or_replace_request(
             sent_share_id,
             content_type="application/json",
             content=json.dumps(sent_share))
         
@@ -116,30 +118,30 @@
 
         assert retrieved_sent_share['id'] == str(sent_share_id)
 
     @PurviewSharingPowerShellPreparer()
     @recorded_by_proxy
     def test_get_all_sent_shares(self, purviewsharing_endpoint):
         client = self.create_client(endpoint=purviewsharing_endpoint)
-        sent_share_id = "37003772-812b-4b69-bea5-5c0a17163df5"
+        sent_share_id = "25fb1b10-8131-4610-84c4-181236fdd062" # uuid4()
         sent_share = self.prepare_sent_share()
 
         request = build_sent_shares_create_or_replace_request(
             sent_share_id,
             content_type="application/json",
             content=json.dumps(sent_share))
         
         response = client.send_request(request)
 
         assert response is not None
         assert response.status_code == 201, "Invalid Status Code " + str(response.status_code)
 
         list_request = build_sent_shares_list_request(
             reference_name=sent_share["properties"]["artifact"]["storeReference"]["referenceName"],
-            orderby="properties/createdAt desc")
+            order_by="properties/createdAt desc")
         
         list_response = client.send_request(list_request)
 
         assert list_response is not None
         assert list_response.content is not None
          
         list = json.loads(list_response.content)['value']
@@ -147,15 +149,15 @@
         assert len(list) > 0, "Invalid number of shares " + str(len(list))
         assert len([x for x in list if x["id"] == str(sent_share_id)]) == 1
 
     @PurviewSharingPowerShellPreparer()
     @recorded_by_proxy
     def test_delete_sent_share(self, purviewsharing_endpoint):
         client = self.create_client(endpoint=purviewsharing_endpoint)
-        sent_share_id = "a5fbfbe0-6303-4924-b9be-885d7e3af97f"
+        sent_share_id = "d857d382-b535-4b6e-bb5a-db59c42ed333" # uuid4()
         sent_share = self.prepare_sent_share()
 
         request = build_sent_shares_create_or_replace_request(
             sent_share_id,
             content_type="application/json",
             content=json.dumps(sent_share))
         
@@ -176,36 +178,36 @@
             print("Exception " + str(e))
             print("Response " + delete_response.text())
 
     @PurviewSharingPowerShellPreparer()
     @recorded_by_proxy
     def test_create_sent_share_service_invitation(self, purviewsharing_endpoint):
         client = self.create_client(endpoint=purviewsharing_endpoint)
-        sent_share_id = "81f34fe1-9bf1-4e9c-aff5-8687fe0a37c7"
-        sent_share_invitation_id = "d1dfa155-70a9-4397-96ff-594159dc3fa8"
+        sent_share_id = "c0a51c4e-6951-4fb6-a501-98034ab5b741" # uuid4()
+        sent_share_invitation_id = "840faa15-db43-46b5-9de0-842c0aa2db35" # uuid4()
         sent_share = self.prepare_sent_share()
         
         request = build_sent_shares_create_or_replace_request(
             sent_share_id,
             content_type="application/json",
             content=json.dumps(sent_share))
         
         response = client.send_request(request)
 
         assert response is not None
         assert response.status_code == 201, "Invalid Status Code 1 " + str(response.status_code)
 
-        targetActiveDirectoryId = "bc02d987-c010-4e4e-95d1-4bab99ed0ac2"
-        targetObjectId = "28b46e20-9847-4d41-8bae-28e17a76d3de"
+        targetActiveDirectoryId = "b73a405f-f2e4-40f9-a606-5562778074c6" # uuid4()
+        targetObjectId = "7cbeb37b-95ea-4a7a-8cb3-becc797b3b8d" # uuid4()
 
         invitation = {
             "invitationKind": "Service",
             "properties": {
-                "targetActiveDirectoryId": targetActiveDirectoryId,
-                "targetObjectId": targetObjectId
+                "targetActiveDirectoryId": str(targetActiveDirectoryId),
+                "targetObjectId": str(targetObjectId)
             }
         }
 
         invitation_request = build_sent_shares_create_invitation_request(
             sent_share_id=sent_share_id,
             sent_share_invitation_id=sent_share_invitation_id,
             content_type="application/json",
@@ -216,43 +218,43 @@
         assert invitation_response is not None
         assert invitation_response.status_code == 201, "Invalid status code 2 " + str(invitation_response.status_code)
         assert invitation_response.content is not None
 
         created_invitation = json.loads(invitation_response.content)
 
         assert created_invitation['id'] == str(sent_share_invitation_id)
-        assert created_invitation['properties']['targetActiveDirectoryId'] == targetActiveDirectoryId
-        assert created_invitation['properties']['targetObjectId'] == targetObjectId
+        assert created_invitation['properties']['targetActiveDirectoryId'] == str(targetActiveDirectoryId)
+        assert created_invitation['properties']['targetObjectId'] == str(targetObjectId)
 
     @PurviewSharingPowerShellPreparer()
     @recorded_by_proxy
     def test_get_all_sent_share_service_invitation(self, purviewsharing_endpoint):
         client = self.create_client(endpoint=purviewsharing_endpoint)
-        sent_share_id = "57734197-13dd-45f0-aa78-082bb55ed768"
-        sent_share_invitation_id = "8c35d372-a90d-4e5b-93cc-c18ad525bb44"
+        sent_share_id = "df189706-d347-4659-b7d9-62f8b7b974d2" # uuid4()
+        sent_share_invitation_id = "2d423d1e-b1b1-4b33-9960-2fd2dd3fe90c" #uuid4()
         sent_share = self.prepare_sent_share()
 
         request = build_sent_shares_create_or_replace_request(
             sent_share_id,
             content_type="application/json",
             content=json.dumps(sent_share))
         
         response = client.send_request(request)
 
         assert response is not None
         assert response.status_code == 201, "Invalid Status Code 1 " + str(response.status_code)
 
-        targetActiveDirectoryId = "19513734-8215-4190-bd7e-ff6cbed36fbe"
-        targetObjectId = "ebf435a4-3f8d-4ed1-843b-e598e2916a3e"
+        targetActiveDirectoryId = "2a040521-5776-4569-a788-bc9b66160f6b" # uuid4()
+        targetObjectId = "e86fe185-1f23-4518-ab7b-e887cca44933" #uuid4()
 
         sent_share_invitation = {
             "invitationKind": "Service",
             "properties": {
-                "targetActiveDirectoryId": targetActiveDirectoryId,
-                "targetObjectId": targetObjectId
+                "targetActiveDirectoryId": str(targetActiveDirectoryId),
+                "targetObjectId": str(targetObjectId)
             }
         }
 
         invitation_request = build_sent_shares_create_invitation_request(
             sent_share_id=sent_share_id,
             sent_share_invitation_id=sent_share_invitation_id,
             content_type="application/json",
@@ -263,47 +265,134 @@
         assert invitation_response is not None
         assert invitation_response.status_code == 201, "Invalid status code 2 " + str(invitation_response.status_code)
         assert invitation_response.content is not None
 
         created_invitation = json.loads(invitation_response.content)
 
         assert created_invitation['id'] == str(sent_share_invitation_id)
-        assert created_invitation['properties']['targetActiveDirectoryId'] == targetActiveDirectoryId
-        assert created_invitation['properties']['targetObjectId'] == targetObjectId
+        assert created_invitation['properties']['targetActiveDirectoryId'] == str(targetActiveDirectoryId)
+        assert created_invitation['properties']['targetObjectId'] == str(targetObjectId)
 
         list_request = build_sent_shares_list_invitations_request(sent_share_id=sent_share_id)
         list_response = client.send_request(list_request)
 
         assert list_response is not None
         assert list_response.content is not None
          
         list = json.loads(list_response.content)['value']
         assert len([x for x in list if x['id'] == str(sent_share_invitation_id)]) == 1
-
+    ###     ###
+    ### NEW ###
+    ###     ###
     @PurviewSharingPowerShellPreparer()
     @recorded_by_proxy
     def test_delete_sent_share_service_invitation(self, purviewsharing_endpoint):
         client = self.create_client(endpoint=purviewsharing_endpoint)
-        sent_share_id = "050bd22d-a09e-47d0-ac20-367266ffaa54"
+        sent_share_id = "03a166c3-f68d-41fe-9af1-83f5dcc8b83e" # uuid4()
+        sent_share_invitation_id = "0bea71cd-428b-4989-91e9-92f19b9e165c" # uuid4()
         sent_share = self.prepare_sent_share()
 
         request = build_sent_shares_create_or_replace_request(
             sent_share_id,
             content_type="application/json",
             content=json.dumps(sent_share))
 
         response = client.send_request(request)
 
         assert response is not None
         assert response.status_code == 201, "Invalid Status Code " + str(response.status_code)
 
-        delete_request = build_sent_shares_delete_request(sent_share_id=sent_share_id)
+        targetActiveDirectoryId = "746a6b35-6571-4688-9e52-d29451add6ed" # uuid4()
+        targetObjectId = "fb5b839c-1401-4a58-b956-2d42f5641039" #uuid4()
+
+        sent_share_invitation = {
+            "invitationKind": "Service",
+            "properties": {
+                "targetActiveDirectoryId": str(targetActiveDirectoryId),
+                "targetObjectId": str(targetObjectId)
+            }
+        }
+
+        invitation_request = build_sent_shares_create_invitation_request(
+            sent_share_id=sent_share_id,
+            sent_share_invitation_id=sent_share_invitation_id,
+            content_type="application/json",
+            content=json.dumps(sent_share_invitation))
+        
+        invitation_response = client.send_request(invitation_request)
+
+        assert invitation_response is not None
+        assert invitation_response.status_code == 201, "Invalid status code 2 " + str(invitation_response.status_code)
+        assert invitation_response.content is not None
+
+        delete_request = build_sent_shares_delete_invitation_request(
+            sent_share_id=sent_share_id, 
+            sent_share_invitation_id=sent_share_invitation_id)
+        
         delete_response = client.send_request(delete_request)
 
         assert delete_response is not None
         assert delete_response.status_code == 202, "Invalid Status Code " + str(response.status_code)
 
         try:
             delete_response.raise_for_status()
         except HttpResponseError as e:
             print("Exception " + str(e))
-            print("Response " + delete_response.text())
+            print("Response " + delete_response.text())
+
+    @PurviewSharingPowerShellPreparer()
+    @recorded_by_proxy
+    def test_get_sent_share_invitation(self, purviewsharing_endpoint):
+        client = self.create_client(endpoint=purviewsharing_endpoint)
+        sent_share_id = "1a82d02a-033c-4624-b8f2-243c0df06a9b" # uuid4()
+        sent_share_invitation_id = "23006055-336a-437d-9808-3793af9fc6a8" # uuid4()
+        sent_share = self.prepare_sent_share()
+
+        request = build_sent_shares_create_or_replace_request(
+            sent_share_id,
+            content_type="application/json",
+            content=json.dumps(sent_share))
+        
+        response = client.send_request(request)
+
+        assert response is not None
+        assert response.status_code == 201, "Invalid Status Code " + str(response.status_code)
+
+        consumerEmail = "consumer@contoso.com"
+
+        invitation = {
+            "invitationKind": "User",
+            "properties": {
+                "targetEmail": consumerEmail,
+                "notify": "true",
+                "expirationDate": "2024-03-02 00:00:00"
+            }
+        }
+
+        invitation_request = build_sent_shares_create_invitation_request(
+            sent_share_id=sent_share_id,
+            sent_share_invitation_id=sent_share_invitation_id,
+            content_type="application/json",
+            content=json.dumps(invitation))
+        
+        invitation_response = client.send_request(invitation_request)
+
+        assert invitation_response is not None
+        assert invitation_response.status_code == 201, "Invalid Status Code " + str(invitation_response.status_code)
+        assert invitation_response.content is not None
+
+        created_invitation = json.loads(invitation_response.content)
+
+        assert created_invitation['id'] == str(sent_share_invitation_id)
+        assert created_invitation['properties']['targetEmail'] == consumerEmail
+
+        get_request = build_sent_shares_get_invitation_request(sent_share_id=sent_share_id, sent_share_invitation_id=sent_share_invitation_id)
+        get_response = client.send_request(get_request)
+
+        assert get_response is not None
+        assert get_response.content is not None
+         
+        retrieved_sent_share_invitation = json.loads(get_response.content)
+
+        assert retrieved_sent_share_invitation['id'] == str(sent_share_invitation_id)
+
+
```

## Comparing `azure-purview-sharing-1.0.0b2/tests/conftest.py` & `azure-purview-sharing-1.0.0b3/tests/conftest.py`

 * *Files 23% similar despite different names*

```diff
@@ -41,17 +41,23 @@
 
 @pytest.fixture(scope="session", autouse=True)
 def add_sanitizers(test_proxy):
     subscription_id = os.environ.get("PURVIEWSHARING_SUBSCRIPTION_ID", "00000000-0000-0000-0000-000000000000")
     tenant_id = os.environ.get("PURVIEWSHARING_TENANT_ID", "00000000-0000-0000-0000-000000000000")
     client_id = os.environ.get("PURVIEWSHARING_CLIENT_ID", "00000000-0000-0000-0000-000000000000")
     client_secret = os.environ.get("PURVIEWSHARING_CLIENT_SECRET", "00000000-0000-0000-0000-000000000000")
+    resource_group_name = os.environ.get("PURVIEWSHARING_RESOURCEGROUP", "fakeResourceGroup")
+    storage_account_provider = os.environ.get("PURVIEWSHARING_STORAGEACCOUNT_PROVIDER", "fakeStorageAccount")
+    storage_account_receiver = os.environ.get("PURVIEWSHARING_STORAGEACCOUNT_RECEIVER", "fakeStorageAccountR")
     add_general_regex_sanitizer(regex=subscription_id, value="00000000-0000-0000-0000-000000000000")
     add_general_regex_sanitizer(regex=tenant_id, value="00000000-0000-0000-0000-000000000000")
     add_general_regex_sanitizer(regex=client_id, value="00000000-0000-0000-0000-000000000000")
     add_general_regex_sanitizer(regex=client_secret, value="00000000-0000-0000-0000-000000000000")
+    add_general_regex_sanitizer(regex=resource_group_name, value="fakeResourceGroup")
+    add_general_regex_sanitizer(regex=storage_account_provider, value="fakeStorageAccount")
+    add_general_regex_sanitizer(regex=storage_account_receiver, value="fakeStorageAccountR")
     add_header_regex_sanitizer(key="Set-Cookie", value="[set-cookie;]")
     add_header_regex_sanitizer(key="Cookie", value="cookie;")
     add_body_key_sanitizer(json_path="$..access_token", value="access_token")
     add_body_key_sanitizer(json_path="$..atlasKafkaPrimaryEndpoint", value="000")
     add_body_key_sanitizer(json_path="$..atlasKafkaSecondaryEndpoint", value="000")
-    add_body_key_sanitizer(json_path="$..systemData.createdBy", value="000")
+    add_body_key_sanitizer(json_path="$..systemData.createdBy", value="000")
```

## Comparing `azure-purview-sharing-1.0.0b2/tests/test_received_shares.py` & `azure-purview-sharing-1.0.0b3/tests/test_received_shares.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 # coding: utf-8
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 import json
+from uuid import uuid4
 
 from testcase import TestPurviewSharing, PurviewSharingPowerShellPreparer
 from devtools_testutils import recorded_by_proxy
 from azure.core.exceptions import HttpResponseError
 from azure.purview.sharing.operations._operations import (
     build_sent_shares_create_or_replace_request,
     build_sent_shares_create_invitation_request,
     build_received_shares_list_detached_request,
     build_received_shares_get_request,
     build_received_shares_delete_request,
-    build_received_shares_create_or_replace_request
+    build_received_shares_create_or_replace_request,
+    build_received_shares_list_attached_request
 )
 
 class TestReceivedShares(TestPurviewSharing):
 
     @PurviewSharingPowerShellPreparer()
     @recorded_by_proxy
     def test_get_all_detached_shares(self, purviewsharing_endpoint):
         client = self.create_client(endpoint=purviewsharing_endpoint)
-        sent_share_id = "1c63a285-4649-4a5b-b9aa-6e9c356f70fc"
-        sent_share_invitation_id = "4d4f6be0-addd-4d5b-98be-ed09c38cdf49"
+        sent_share_id = "4556ccb7-5d6a-45d4-8568-e1faa236e037" # uuid4()
+        sent_share_invitation_id = "554696cf-ddc7-46c0-b915-45face229cd3" # uuid4()
         sent_share = self.prepare_sent_share()
 
         request = build_sent_shares_create_or_replace_request(
             sent_share_id,
             content_type="application/json",
             content=json.dumps(sent_share))
         
@@ -62,33 +64,32 @@
         assert invitation_response.content is not None
 
         created_invitation = json.loads(invitation_response.content)
 
         assert created_invitation['id'] == str(sent_share_invitation_id)
         assert created_invitation['properties']['targetEmail'] == consumerEmail
 
-        list_detached_request = build_received_shares_list_detached_request(orderby="properties/createdAt desc")
+        list_detached_request = build_received_shares_list_detached_request(order_by="properties/createdAt desc")
         list_detached_response = client.send_request(list_detached_request)
 
         assert list_detached_response is not None
 
         list_detached = json.loads(list_detached_response.content)
 
         assert list_detached is not None
         assert len(list_detached['value']) > 0
-
         # is the number of items that has shareStatus "Detached" equal to the number of all results
         assert len([x for x in list_detached['value'] if x['properties']['shareStatus'] == "Detached"]) == len(list_detached['value'])
-    
+
     @PurviewSharingPowerShellPreparer()
     @recorded_by_proxy
     def test_get_received_share(self, purviewsharing_endpoint):
         client = self.create_client(endpoint=purviewsharing_endpoint)
-        sent_share_id = "1060e96e-a2df-483d-9919-317a3ab4ef49"
-        sent_share_invitation_id = "5bf02e34-ae34-48e5-8cc6-13aec7f15cd2"
+        sent_share_id = "34ede054-d6fc-49a1-a4e2-996433ed4b53" #uuid4()
+        sent_share_invitation_id = "b8307b9f-db8d-4023-b406-2e7f9f6d88c5" #uuid4()
         sent_share = self.prepare_sent_share()
 
         request = build_sent_shares_create_or_replace_request(
             sent_share_id,
             content_type="application/json",
             content=json.dumps(sent_share))
         
@@ -121,37 +122,37 @@
         assert invitation_response.content is not None
 
         created_invitation = json.loads(invitation_response.content)
 
         assert created_invitation['id'] == str(sent_share_invitation_id)
         assert created_invitation['properties']['targetEmail'] == consumerEmail
 
-        list_detached_request = build_received_shares_list_detached_request(orderby="properties/createdAt desc")
+        list_detached_request = build_received_shares_list_detached_request(order_by="properties/createdAt desc")
         list_detached_response = client.send_request(list_detached_request)
 
         assert list_detached_response is not None
 
         list_detached = json.loads(list_detached_response.content)
 
         received_share = list_detached['value'][0]
 
         get_share_request = build_received_shares_get_request(received_share_id=received_share['id'])
         get_share_response = client.send_request(get_share_request)
         
         retrieved_share = json.loads(get_share_response.content)
-
+        print(retrieved_share)
         assert retrieved_share is not None
         assert retrieved_share['id'] == received_share['id']
 
     @PurviewSharingPowerShellPreparer()
     @recorded_by_proxy
     def test_delete_received_share(self, purviewsharing_endpoint):
         client = self.create_client(endpoint=purviewsharing_endpoint)
-        sent_share_id = "50244d25-4359-4310-97be-99b1569ebcb4"
-        sent_share_invitation_id = "2c1560f9-7390-450d-b2ac-12cdaa94bb75"
+        sent_share_id = "2a7268a0-85d9-4c13-ba7b-a25ebba5faf3" #uuid4()
+        sent_share_invitation_id = "9a672068-d620-4492-9e20-3f686f768f29" #uuid4()
         sent_share = self.prepare_sent_share()
 
         request = build_sent_shares_create_or_replace_request(
             sent_share_id,
             content_type="application/json",
             content=json.dumps(sent_share))
         
@@ -184,15 +185,15 @@
         assert invitation_response.content is not None
 
         created_invitation = json.loads(invitation_response.content)
 
         assert created_invitation['id'] == str(sent_share_invitation_id)
         assert created_invitation['properties']['targetEmail'] == consumerEmail
 
-        list_detached_request = build_received_shares_list_detached_request(orderby="properties/createdAt desc")
+        list_detached_request = build_received_shares_list_detached_request(order_by="properties/createdAt desc")
         list_detached_response = client.send_request(list_detached_request)
 
         assert list_detached_response is not None
 
         list_detached = json.loads(list_detached_response.content)
 
         received_share = list_detached['value'][0]
@@ -206,20 +207,20 @@
             print("Exception " + str(e))
             print("Response " + delete_received_share_response.text())
 
     @PurviewSharingPowerShellPreparer()
     @recorded_by_proxy
     def test_attach_received_share(self, purviewsharing_endpoint):
         client = self.create_client(endpoint=purviewsharing_endpoint)
-        sent_share_id = "0c2a884a-5b4c-4b41-b4f8-d364d20c4ae1"
-        sent_share_invitation_id = "1118c292-a591-4b46-875b-2332e7a3d2b3"
+        sent_share_id = "b9d374c2-30d7-4e91-a750-a53238002652" # uuid4()
+        sent_share_invitation_id = "242f81b5-fe36-402b-9a27-5d2af7f33308" #uuid4()
         sent_share = self.prepare_sent_share()
 
         # cspell:disable-next-line
-        consumer_storage_account_resource_id = "/subscriptions/0f3dcfc3-18f8-4099-b381-8353e19d43a7/resourceGroups/faisalaltell/providers/Microsoft.Storage/storageAccounts/ftreceiversan"
+        consumer_storage_account_resource_id = "/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/fakeResourceGroup/providers/Microsoft.Storage/storageAccounts/fakeStorageAccountR"
 
         request = build_sent_shares_create_or_replace_request(
             sent_share_id,
             content_type="application/json",
             content=json.dumps(sent_share))
         
         response = client.send_request(request)
@@ -251,15 +252,15 @@
         assert invitation_response.content is not None
 
         created_invitation = json.loads(invitation_response.content)
 
         assert created_invitation['id'] == str(sent_share_invitation_id)
         assert created_invitation['properties']['targetEmail'] == consumerEmail
 
-        list_detached_request = build_received_shares_list_detached_request(orderby="properties/createdAt desc")
+        list_detached_request = build_received_shares_list_detached_request(order_by="properties/createdAt desc")
         list_detached_response = client.send_request(list_detached_request)
 
         assert list_detached_response is not None
 
         list_detached = json.loads(list_detached_response.content)
         received_share = list_detached['value'][0]
 
@@ -292,8 +293,111 @@
         assert update_response is not None
         assert update_response.status_code == 201, "Invalid Status Code " + str(update_response.status_code)
 
         try:
             update_response.raise_for_status()
         except HttpResponseError as e:
             print("Exception " + str(e))
-            print("Response " + update_response.text())
+            print("Response " + update_response.text())
+
+    ###     ###
+    ### NEW ###
+    ###     ###
+    @PurviewSharingPowerShellPreparer()
+    @recorded_by_proxy
+    def test_get_all_attached_shares(self, purviewsharing_endpoint):
+        client = self.create_client(endpoint=purviewsharing_endpoint)
+        sent_share_id = "6143851f-930b-4050-a437-00b6bfbf2b4e" #uuid4()
+        sent_share_invitation_id = "4430cf68-61db-4e05-af7b-297bad6d362b" #uuid4()
+        sent_share = self.prepare_sent_share()
+
+        # cspell:disable-next-line
+        consumer_storage_account_resource_id = "/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/fakeResourceGroup/providers/Microsoft.Storage/storageAccounts/fakeStorageAccountR"
+
+        request = build_sent_shares_create_or_replace_request(
+            sent_share_id,
+            content_type="application/json",
+            content=json.dumps(sent_share))
+        
+        response = client.send_request(request)
+
+        assert response is not None
+        assert response.status_code == 201, "Invalid Status Code " + str(response.status_code)
+
+        consumerEmail = "consumer@contoso.com"
+
+        invitation = {
+            "invitationKind": "User",
+            "properties": {
+                "targetEmail": consumerEmail,
+                "notify": "true",
+                "expirationDate": "2024-01-01 00:00:00"
+            }
+        }
+
+        invitation_request = build_sent_shares_create_invitation_request(
+            sent_share_id=sent_share_id,
+            sent_share_invitation_id=sent_share_invitation_id,
+            content_type="application/json",
+            content=json.dumps(invitation))
+        
+        invitation_response = client.send_request(invitation_request)
+
+        assert invitation_response is not None
+        assert invitation_response.status_code == 201, "Invalid Status Code " + str(invitation_response.status_code)
+        assert invitation_response.content is not None
+
+        created_invitation = json.loads(invitation_response.content)
+
+        assert created_invitation['id'] == str(sent_share_invitation_id)
+        assert created_invitation['properties']['targetEmail'] == consumerEmail
+
+        list_detached_request = build_received_shares_list_detached_request(order_by="properties/createdAt desc")
+        list_detached_response = client.send_request(list_detached_request)
+
+        assert list_detached_response is not None
+
+        list_detached = json.loads(list_detached_response.content)
+        received_share = list_detached['value'][0]
+
+        store_reference = {
+            "referenceName": consumer_storage_account_resource_id,
+            "type": "ArmResourceReference"
+        }
+
+        # cspell:disable
+        sink = {
+            "properties": {
+                "containerName": "containerellxvxonnlukvfzbwhlexfzqfs",
+                "folder": "folderpubhxhmiibnxcvqchnbi",
+                "mountPath": "mountPathciynxouybsqvfgmcfwtt",
+            },
+            "storeKind": "AdlsGen2Account",
+            "storeReference": store_reference
+        }
+        # cspell:enable
+
+        received_share['properties']['sink'] = sink
+
+        update_request = build_received_shares_create_or_replace_request(
+            received_share['id'],
+            content_type="application/json",
+            content=json.dumps(received_share))
+        
+        update_response = client.send_request(update_request)
+
+        assert update_response is not None
+        assert update_response.status_code == 201, "Invalid Status Code " + str(update_response.status_code)
+
+        list_attached_request = build_received_shares_list_attached_request(
+            reference_name=consumer_storage_account_resource_id,
+            order_by="properties/createdAt desc")
+        list_attached_response = client.send_request(list_attached_request)
+
+        assert list_attached_response is not None
+
+        list_attached = json.loads(list_attached_response.content)
+
+        assert list_attached is not None
+        assert len(list_attached['value']) > 0
+        # is the number of items that has shareStatus "Attached" equal to the number of all results
+        assert len([x for x in list_attached['value'] if x['properties']['shareStatus'] == "Attached"]) == len(list_attached['value'])
```

## Comparing `azure-purview-sharing-1.0.0b2/tests/_util.py` & `azure-purview-sharing-1.0.0b3/tests/_util.py`

 * *Files identical despite different names*

## Comparing `azure-purview-sharing-1.0.0b2/azure/purview/sharing/_configuration.py` & `azure-purview-sharing-1.0.0b3/azure/purview/sharing/_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,22 +31,22 @@
     attributes.
 
     :param endpoint: The sharing endpoint of your purview account. Example:
      https://{accountName}.purview.azure.com/share. Required.
     :type endpoint: str
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
-    :keyword api_version: Api Version. Default value is "2023-02-15-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2023-05-30-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, endpoint: str, credential: "TokenCredential", **kwargs: Any) -> None:
         super(PurviewSharingClientConfiguration, self).__init__(**kwargs)
-        api_version: Literal["2023-02-15-preview"] = kwargs.pop("api_version", "2023-02-15-preview")
+        api_version: Literal["2023-05-30-preview"] = kwargs.pop("api_version", "2023-05-30-preview")
 
         if endpoint is None:
             raise ValueError("Parameter 'endpoint' must not be None.")
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
 
         self.endpoint = endpoint
```

## Comparing `azure-purview-sharing-1.0.0b2/azure/purview/sharing/_client.py` & `azure-purview-sharing-1.0.0b3/azure/purview/sharing/_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,34 +10,36 @@
 from typing import Any, TYPE_CHECKING
 
 from azure.core import PipelineClient
 from azure.core.rest import HttpRequest, HttpResponse
 
 from ._configuration import PurviewSharingClientConfiguration
 from ._serialization import Deserializer, Serializer
-from .operations import ReceivedSharesOperations, SentSharesOperations
+from .operations import ReceivedSharesOperations, SentSharesOperations, ShareResourcesOperations
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
 
 
 class PurviewSharingClient:  # pylint: disable=client-accepts-api-version-keyword
     """Creates a data plane client for Purview Share.
 
     :ivar received_shares: ReceivedSharesOperations operations
     :vartype received_shares: azure.purview.sharing.operations.ReceivedSharesOperations
     :ivar sent_shares: SentSharesOperations operations
     :vartype sent_shares: azure.purview.sharing.operations.SentSharesOperations
+    :ivar share_resources: ShareResourcesOperations operations
+    :vartype share_resources: azure.purview.sharing.operations.ShareResourcesOperations
     :param endpoint: The sharing endpoint of your purview account. Example:
      https://{accountName}.purview.azure.com/share. Required.
     :type endpoint: str
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
-    :keyword api_version: Api Version. Default value is "2023-02-15-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2023-05-30-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(self, endpoint: str, credential: "TokenCredential", **kwargs: Any) -> None:
@@ -46,14 +48,15 @@
         self._client: PipelineClient = PipelineClient(base_url=_endpoint, config=self._config, **kwargs)
 
         self._serialize = Serializer()
         self._deserialize = Deserializer()
         self._serialize.client_side_validation = False
         self.received_shares = ReceivedSharesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.sent_shares = SentSharesOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.share_resources = ShareResourcesOperations(self._client, self._config, self._serialize, self._deserialize)
 
     def send_request(self, request: HttpRequest, **kwargs: Any) -> HttpResponse:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
```

## Comparing `azure-purview-sharing-1.0.0b2/azure/purview/sharing/__init__.py` & `azure-purview-sharing-1.0.0b3/azure/purview/sharing/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-purview-sharing-1.0.0b2/azure/purview/sharing/_vendor.py` & `azure-purview-sharing-1.0.0b3/azure/purview/sharing/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-purview-sharing-1.0.0b2/azure/purview/sharing/_serialization.py` & `azure-purview-sharing-1.0.0b3/azure/purview/sharing/_serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
 #
 # --------------------------------------------------------------------------
 
 # pylint: skip-file
 # pyright: reportUnnecessaryTypeIgnoreComment=false
-# cspell:disable
 
 from base64 import b64decode, b64encode
 import calendar
 import datetime
 import decimal
 import email
 from enum import Enum
@@ -890,15 +889,14 @@
         :param str iter_type: Type of object in the iterable.
         :param bool required: Whether the objects in the iterable must
          not be None or empty.
         :param str div: If set, this str will be used to combine the elements
          in the iterable into a combined string. Default is 'None'.
         :rtype: list, str
         """
-
         if isinstance(data, str):
             raise SerializationError("Refuse str type as a valid iter type.")
 
         serialization_ctxt = kwargs.get("serialization_ctxt", {})
         is_xml = kwargs.get("is_xml", False)
 
         serialized = []
@@ -1992,9 +1990,7 @@
         try:
             date_obj = datetime.datetime.fromtimestamp(attr, TZ_UTC)
         except ValueError as err:
             msg = "Cannot deserialize to unix datetime object."
             raise_with_traceback(DeserializationError, msg, err)
         else:
             return date_obj
-
-# cspell:enable
```

## Comparing `azure-purview-sharing-1.0.0b2/azure/purview/sharing/_patch.py` & `azure-purview-sharing-1.0.0b3/azure/purview/sharing/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-purview-sharing-1.0.0b2/azure/purview/sharing/aio/_configuration.py` & `azure-purview-sharing-1.0.0b3/azure/purview/sharing/aio/_configuration.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,22 +31,22 @@
     attributes.
 
     :param endpoint: The sharing endpoint of your purview account. Example:
      https://{accountName}.purview.azure.com/share. Required.
     :type endpoint: str
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
-    :keyword api_version: Api Version. Default value is "2023-02-15-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2023-05-30-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, endpoint: str, credential: "AsyncTokenCredential", **kwargs: Any) -> None:
         super(PurviewSharingClientConfiguration, self).__init__(**kwargs)
-        api_version: Literal["2023-02-15-preview"] = kwargs.pop("api_version", "2023-02-15-preview")
+        api_version: Literal["2023-05-30-preview"] = kwargs.pop("api_version", "2023-05-30-preview")
 
         if endpoint is None:
             raise ValueError("Parameter 'endpoint' must not be None.")
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
 
         self.endpoint = endpoint
```

## Comparing `azure-purview-sharing-1.0.0b2/azure/purview/sharing/aio/_client.py` & `azure-purview-sharing-1.0.0b3/azure/purview/sharing/aio/_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,34 +10,36 @@
 from typing import Any, Awaitable, TYPE_CHECKING
 
 from azure.core import AsyncPipelineClient
 from azure.core.rest import AsyncHttpResponse, HttpRequest
 
 from .._serialization import Deserializer, Serializer
 from ._configuration import PurviewSharingClientConfiguration
-from .operations import ReceivedSharesOperations, SentSharesOperations
+from .operations import ReceivedSharesOperations, SentSharesOperations, ShareResourcesOperations
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
 
 class PurviewSharingClient:  # pylint: disable=client-accepts-api-version-keyword
     """Creates a data plane client for Purview Share.
 
     :ivar received_shares: ReceivedSharesOperations operations
     :vartype received_shares: azure.purview.sharing.aio.operations.ReceivedSharesOperations
     :ivar sent_shares: SentSharesOperations operations
     :vartype sent_shares: azure.purview.sharing.aio.operations.SentSharesOperations
+    :ivar share_resources: ShareResourcesOperations operations
+    :vartype share_resources: azure.purview.sharing.aio.operations.ShareResourcesOperations
     :param endpoint: The sharing endpoint of your purview account. Example:
      https://{accountName}.purview.azure.com/share. Required.
     :type endpoint: str
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
-    :keyword api_version: Api Version. Default value is "2023-02-15-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2023-05-30-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(self, endpoint: str, credential: "AsyncTokenCredential", **kwargs: Any) -> None:
@@ -46,14 +48,15 @@
         self._client: AsyncPipelineClient = AsyncPipelineClient(base_url=_endpoint, config=self._config, **kwargs)
 
         self._serialize = Serializer()
         self._deserialize = Deserializer()
         self._serialize.client_side_validation = False
         self.received_shares = ReceivedSharesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.sent_shares = SentSharesOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.share_resources = ShareResourcesOperations(self._client, self._config, self._serialize, self._deserialize)
 
     def send_request(self, request: HttpRequest, **kwargs: Any) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
```

## Comparing `azure-purview-sharing-1.0.0b2/azure/purview/sharing/aio/__init__.py` & `azure-purview-sharing-1.0.0b3/azure/purview/sharing/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-purview-sharing-1.0.0b2/azure/purview/sharing/aio/_patch.py` & `azure-purview-sharing-1.0.0b3/azure/purview/sharing/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-purview-sharing-1.0.0b2/azure/purview/sharing/aio/operations/__init__.py` & `azure-purview-sharing-1.0.0b3/azure/purview/sharing/operations/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._operations import ReceivedSharesOperations
 from ._operations import SentSharesOperations
+from ._operations import ShareResourcesOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "ReceivedSharesOperations",
     "SentSharesOperations",
+    "ShareResourcesOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-purview-sharing-1.0.0b2/azure/purview/sharing/aio/operations/_operations.py` & `azure-purview-sharing-1.0.0b3/azure/purview/sharing/aio/operations/_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     build_sent_shares_delete_invitation_request,
     build_sent_shares_delete_request,
     build_sent_shares_get_invitation_request,
     build_sent_shares_get_request,
     build_sent_shares_list_invitations_request,
     build_sent_shares_list_request,
     build_sent_shares_notify_user_invitation_request,
+    build_share_resources_list_request,
 )
 
 if sys.version_info >= (3, 9):
     from collections.abc import MutableMapping
 else:
     from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 JSON = MutableMapping[str, Any]  # pylint: disable=unsubscriptable-object
@@ -1201,34 +1202,26 @@
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
         return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     @distributed_trace
     def list_attached(
-        self,
-        *,
-        reference_name: str,
-        skip_token: Optional[str] = None,
-        filter: Optional[str] = None,
-        orderby: Optional[str] = None,
-        **kwargs: Any
+        self, *, reference_name: str, filter: Optional[str] = None, order_by: Optional[str] = None, **kwargs: Any
     ) -> AsyncIterable[JSON]:
         """Get a list of attached received shares.
 
         List attached received shares.
 
         :keyword reference_name: A name that references a data store. Required.
         :paramtype reference_name: str
-        :keyword skip_token: The continuation token to list the next page. Default value is None.
-        :paramtype skip_token: str
         :keyword filter: Filters the results using OData syntax. Default value is None.
         :paramtype filter: str
-        :keyword orderby: Sorts the results using OData syntax. Default value is None.
-        :paramtype orderby: str
+        :keyword order_by: Sorts the results using OData syntax. Default value is None.
+        :paramtype order_by: str
         :return: An iterator like instance of JSON object
         :rtype: ~azure.core.async_paging.AsyncItemPaged[JSON]
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
                 # The response is polymorphic. The following are possible polymorphic responses based
@@ -1325,17 +1318,16 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
                 request = build_received_shares_list_attached_request(
                     reference_name=reference_name,
-                    skip_token=skip_token,
                     filter=filter,
-                    orderby=orderby,
+                    order_by=order_by,
                     api_version=self._config.api_version,
                     headers=_headers,
                     params=_params,
                 )
                 path_format_arguments = {
                     "endpoint": self._serialize.url(
                         "self._config.endpoint", self._config.endpoint, "str", skip_quote=True
@@ -1387,31 +1379,24 @@
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
     @distributed_trace
     def list_detached(
-        self,
-        *,
-        skip_token: Optional[str] = None,
-        filter: Optional[str] = None,
-        orderby: Optional[str] = None,
-        **kwargs: Any
+        self, *, filter: Optional[str] = None, order_by: Optional[str] = None, **kwargs: Any
     ) -> AsyncIterable[JSON]:
         """Get a list of detached received shares.
 
         List detached received shares.
 
-        :keyword skip_token: The continuation token to list the next page. Default value is None.
-        :paramtype skip_token: str
         :keyword filter: Filters the results using OData syntax. Default value is None.
         :paramtype filter: str
-        :keyword orderby: Sorts the results using OData syntax. Default value is None.
-        :paramtype orderby: str
+        :keyword order_by: Sorts the results using OData syntax. Default value is None.
+        :paramtype order_by: str
         :return: An iterator like instance of JSON object
         :rtype: ~azure.core.async_paging.AsyncItemPaged[JSON]
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
                 # The response is polymorphic. The following are possible polymorphic responses based
@@ -1507,17 +1492,16 @@
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
                 request = build_received_shares_list_detached_request(
-                    skip_token=skip_token,
                     filter=filter,
-                    orderby=orderby,
+                    order_by=order_by,
                     api_version=self._config.api_version,
                     headers=_headers,
                     params=_params,
                 )
                 path_format_arguments = {
                     "endpoint": self._serialize.url(
                         "self._config.endpoint", self._config.endpoint, "str", skip_quote=True
@@ -1929,34 +1913,26 @@
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(
-        self,
-        *,
-        reference_name: str,
-        skip_token: Optional[str] = None,
-        filter: Optional[str] = None,
-        orderby: Optional[str] = None,
-        **kwargs: Any
+        self, *, reference_name: str, filter: Optional[str] = None, order_by: Optional[str] = None, **kwargs: Any
     ) -> AsyncIterable[JSON]:
         """Get a list of sent shares.
 
         List sent shares.
 
         :keyword reference_name: A name that references a data store. Required.
         :paramtype reference_name: str
-        :keyword skip_token: The continuation token to list the next page. Default value is None.
-        :paramtype skip_token: str
         :keyword filter: Filters the results using OData syntax. Default value is None.
         :paramtype filter: str
-        :keyword orderby: Sorts the results using OData syntax. Default value is None.
-        :paramtype orderby: str
+        :keyword order_by: Sorts the results using OData syntax. Default value is None.
+        :paramtype order_by: str
         :return: An iterator like instance of JSON object
         :rtype: ~azure.core.async_paging.AsyncItemPaged[JSON]
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
                 # The response is polymorphic. The following are possible polymorphic responses based
@@ -2054,17 +2030,16 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
                 request = build_sent_shares_list_request(
                     reference_name=reference_name,
-                    skip_token=skip_token,
                     filter=filter,
-                    orderby=orderby,
+                    order_by=order_by,
                     api_version=self._config.api_version,
                     headers=_headers,
                     params=_params,
                 )
                 path_format_arguments = {
                     "endpoint": self._serialize.url(
                         "self._config.endpoint", self._config.endpoint, "str", skip_quote=True
@@ -3253,34 +3228,26 @@
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
         return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     @distributed_trace
     def list_invitations(
-        self,
-        sent_share_id: str,
-        *,
-        skip_token: Optional[str] = None,
-        filter: Optional[str] = None,
-        orderby: Optional[str] = None,
-        **kwargs: Any
+        self, sent_share_id: str, *, filter: Optional[str] = None, order_by: Optional[str] = None, **kwargs: Any
     ) -> AsyncIterable[JSON]:
         """List all sent share invitations in a sent share.
 
         List sent share recipients.
 
         :param sent_share_id: Id of the sent share. Required.
         :type sent_share_id: str
-        :keyword skip_token: The continuation token to list the next page. Default value is None.
-        :paramtype skip_token: str
         :keyword filter: Filters the results using OData syntax. Default value is None.
         :paramtype filter: str
-        :keyword orderby: Sorts the results using OData syntax. Default value is None.
-        :paramtype orderby: str
+        :keyword order_by: Sorts the results using OData syntax. Default value is None.
+        :paramtype order_by: str
         :return: An iterator like instance of JSON object
         :rtype: ~azure.core.async_paging.AsyncItemPaged[JSON]
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
                 # The response is polymorphic. The following are possible polymorphic responses based
@@ -3355,17 +3322,16 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
                 request = build_sent_shares_list_invitations_request(
                     sent_share_id=sent_share_id,
-                    skip_token=skip_token,
                     filter=filter,
-                    orderby=orderby,
+                    order_by=order_by,
                     api_version=self._config.api_version,
                     headers=_headers,
                     params=_params,
                 )
                 path_format_arguments = {
                     "endpoint": self._serialize.url(
                         "self._config.endpoint", self._config.endpoint, "str", skip_quote=True
@@ -4257,7 +4223,139 @@
         else:
             deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})
 
         return cast(JSON, deserialized)
+
+
+class ShareResourcesOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~azure.purview.sharing.aio.PurviewSharingClient`'s
+        :attr:`share_resources` attribute.
+    """
+
+    def __init__(self, *args, **kwargs) -> None:
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
+
+    @distributed_trace
+    def list(
+        self, *, filter: Optional[str] = None, order_by: Optional[str] = None, **kwargs: Any
+    ) -> AsyncIterable[JSON]:
+        """API operation to list ShareResources.
+
+        List share resources.
+
+        :keyword filter: Filters the results using OData syntax. Default value is None.
+        :paramtype filter: str
+        :keyword order_by: Sorts the results using OData syntax. Default value is None.
+        :paramtype order_by: str
+        :return: An iterator like instance of JSON object
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[JSON]
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "id": "str",  # Optional. The unique id of the resource.
+                    "receivedSharesCount": 0,  # Optional. A count of Received Shares associated
+                      with the
+                      Microsoft.Azure.Purview.Share.ApiService.V3.DataTransferObjects.ShareResource.
+                    "sentSharesCount": 0,  # Optional. A count of Sent Shares associated with the
+                      Microsoft.Azure.Purview.Share.ApiService.V3.DataTransferObjects.ShareResource.
+                    "storeKind": "str",  # Optional. The types of asset. Known values are:
+                      "AdlsGen2Account" and "BlobAccount".
+                    "storeReference": {
+                        "referenceName": "str",  # Optional. Reference name for resource
+                          associated with the sink or artifact.
+                        "type": "str"  # Optional. Defines the type of resource being shared.
+                          "ArmResourceReference"
+                    },
+                    "type": "str"  # Optional. Type of the resource.
+                }
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        def prepare_request(next_link=None):
+            if not next_link:
+
+                request = build_share_resources_list_request(
+                    filter=filter,
+                    order_by=order_by,
+                    api_version=self._config.api_version,
+                    headers=_headers,
+                    params=_params,
+                )
+                path_format_arguments = {
+                    "endpoint": self._serialize.url(
+                        "self._config.endpoint", self._config.endpoint, "str", skip_quote=True
+                    ),
+                }
+                request.url = self._client.format_url(request.url, **path_format_arguments)
+
+            else:
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
+                )
+                path_format_arguments = {
+                    "endpoint": self._serialize.url(
+                        "self._config.endpoint", self._config.endpoint, "str", skip_quote=True
+                    ),
+                }
+                request.url = self._client.format_url(request.url, **path_format_arguments)
+
+            return request
+
+        async def extract_data(pipeline_response):
+            deserialized = pipeline_response.http_response.json()
+            list_of_elem = deserialized["value"]
+            if cls:
+                list_of_elem = cls(list_of_elem)  # type: ignore
+            return deserialized.get("nextLink") or None, AsyncList(list_of_elem)
+
+        async def get_next(next_link=None):
+            request = prepare_request(next_link)
+
+            _stream = False
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
+            )
+            response = pipeline_response.http_response
+
+            if response.status_code not in [200]:
+                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                raise HttpResponseError(response=response)
+
+            return pipeline_response
+
+        return AsyncItemPaged(get_next, extract_data)
```

## Comparing `azure-purview-sharing-1.0.0b2/azure/purview/sharing/aio/operations/_patch.py` & `azure-purview-sharing-1.0.0b3/azure/purview/sharing/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-purview-sharing-1.0.0b2/azure/purview/sharing/operations/__init__.py` & `azure-purview-sharing-1.0.0b3/azure/purview/sharing/aio/operations/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._operations import ReceivedSharesOperations
 from ._operations import SentSharesOperations
+from ._operations import ShareResourcesOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "ReceivedSharesOperations",
     "SentSharesOperations",
+    "ShareResourcesOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-purview-sharing-1.0.0b2/azure/purview/sharing/operations/_operations.py` & `azure-purview-sharing-1.0.0b3/azure/purview/sharing/operations/_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,16 +46,16 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_received_shares_get_request(received_share_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-15-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-15-preview")
+    api_version: Literal["2023-05-30-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-05-30-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/receivedShares/{receivedShareId}"
     path_format_arguments = {
         "receivedShareId": _SERIALIZER.url(
@@ -79,16 +79,16 @@
 
 
 def build_received_shares_create_or_replace_request(received_share_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-    api_version: Literal["2023-02-15-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-15-preview")
+    api_version: Literal["2023-05-30-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-05-30-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/receivedShares/{receivedShareId}"
     path_format_arguments = {
         "receivedShareId": _SERIALIZER.url(
@@ -113,16 +113,16 @@
     return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_received_shares_delete_request(received_share_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-15-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-15-preview")
+    api_version: Literal["2023-05-30-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-05-30-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/receivedShares/{receivedShareId}"
     path_format_arguments = {
         "receivedShareId": _SERIALIZER.url(
@@ -142,86 +142,77 @@
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_received_shares_list_attached_request(
-    *,
-    reference_name: str,
-    skip_token: Optional[str] = None,
-    filter: Optional[str] = None,
-    orderby: Optional[str] = None,
-    **kwargs: Any
+    *, reference_name: str, filter: Optional[str] = None, order_by: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-15-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-15-preview")
+    api_version: Literal["2023-05-30-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-05-30-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/receivedShares/attached"
 
     # Construct parameters
     _params["referenceName"] = _SERIALIZER.query("reference_name", reference_name, "str")
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-    if skip_token is not None:
-        _params["skipToken"] = _SERIALIZER.query("skip_token", skip_token, "str")
     if filter is not None:
         _params["filter"] = _SERIALIZER.query("filter", filter, "str")
-    if orderby is not None:
-        _params["orderby"] = _SERIALIZER.query("orderby", orderby, "str")
+    if order_by is not None:
+        _params["orderby"] = _SERIALIZER.query("order_by", order_by, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_received_shares_list_detached_request(
-    *, skip_token: Optional[str] = None, filter: Optional[str] = None, orderby: Optional[str] = None, **kwargs: Any
+    *, filter: Optional[str] = None, order_by: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-15-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-15-preview")
+    api_version: Literal["2023-05-30-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-05-30-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/receivedShares/detached"
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-    if skip_token is not None:
-        _params["skipToken"] = _SERIALIZER.query("skip_token", skip_token, "str")
     if filter is not None:
         _params["filter"] = _SERIALIZER.query("filter", filter, "str")
-    if orderby is not None:
-        _params["orderby"] = _SERIALIZER.query("orderby", orderby, "str")
+    if order_by is not None:
+        _params["orderby"] = _SERIALIZER.query("order_by", order_by, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_received_shares_activate_tenant_email_registration_request(
     *, repeatability_request_id: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-    api_version: Literal["2023-02-15-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-15-preview")
+    api_version: Literal["2023-05-30-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-05-30-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/emails:activate"
 
     # Construct parameters
@@ -241,16 +232,16 @@
 
 def build_received_shares_register_tenant_email_registration_request(
     *, repeatability_request_id: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-15-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-15-preview")
+    api_version: Literal["2023-05-30-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-05-30-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/emails:register"
 
     # Construct parameters
@@ -263,54 +254,47 @@
         )
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_sent_shares_list_request(
-    *,
-    reference_name: str,
-    skip_token: Optional[str] = None,
-    filter: Optional[str] = None,
-    orderby: Optional[str] = None,
-    **kwargs: Any
+    *, reference_name: str, filter: Optional[str] = None, order_by: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-15-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-15-preview")
+    api_version: Literal["2023-05-30-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-05-30-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/sentShares"
 
     # Construct parameters
     _params["referenceName"] = _SERIALIZER.query("reference_name", reference_name, "str")
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-    if skip_token is not None:
-        _params["skipToken"] = _SERIALIZER.query("skip_token", skip_token, "str")
     if filter is not None:
         _params["filter"] = _SERIALIZER.query("filter", filter, "str")
-    if orderby is not None:
-        _params["orderby"] = _SERIALIZER.query("orderby", orderby, "str")
+    if order_by is not None:
+        _params["orderby"] = _SERIALIZER.query("order_by", order_by, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_sent_shares_get_request(sent_share_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-15-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-15-preview")
+    api_version: Literal["2023-05-30-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-05-30-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/sentShares/{sentShareId}"
     path_format_arguments = {
         "sentShareId": _SERIALIZER.url(
@@ -334,16 +318,16 @@
 
 
 def build_sent_shares_create_or_replace_request(sent_share_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-    api_version: Literal["2023-02-15-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-15-preview")
+    api_version: Literal["2023-05-30-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-05-30-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/sentShares/{sentShareId}"
     path_format_arguments = {
         "sentShareId": _SERIALIZER.url(
@@ -368,16 +352,16 @@
     return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_sent_shares_delete_request(sent_share_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-15-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-15-preview")
+    api_version: Literal["2023-05-30-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-05-30-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/sentShares/{sentShareId}"
     path_format_arguments = {
         "sentShareId": _SERIALIZER.url(
@@ -397,26 +381,21 @@
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_sent_shares_list_invitations_request(
-    sent_share_id: str,
-    *,
-    skip_token: Optional[str] = None,
-    filter: Optional[str] = None,
-    orderby: Optional[str] = None,
-    **kwargs: Any
+    sent_share_id: str, *, filter: Optional[str] = None, order_by: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-15-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-15-preview")
+    api_version: Literal["2023-05-30-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-05-30-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/sentShares/{sentShareId}/sentShareInvitations"
     path_format_arguments = {
         "sentShareId": _SERIALIZER.url(
@@ -428,35 +407,33 @@
         ),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-    if skip_token is not None:
-        _params["skipToken"] = _SERIALIZER.query("skip_token", skip_token, "str")
     if filter is not None:
         _params["filter"] = _SERIALIZER.query("filter", filter, "str")
-    if orderby is not None:
-        _params["orderby"] = _SERIALIZER.query("orderby", orderby, "str")
+    if order_by is not None:
+        _params["orderby"] = _SERIALIZER.query("order_by", order_by, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_sent_shares_get_invitation_request(
     sent_share_id: str, sent_share_invitation_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-15-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-15-preview")
+    api_version: Literal["2023-05-30-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-05-30-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/sentShares/{sentShareId}/sentShareInvitations/{sentShareInvitationId}"
     path_format_arguments = {
         "sentShareId": _SERIALIZER.url(
@@ -489,16 +466,16 @@
 def build_sent_shares_create_invitation_request(
     sent_share_id: str, sent_share_invitation_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-    api_version: Literal["2023-02-15-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-15-preview")
+    api_version: Literal["2023-05-30-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-05-30-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/sentShares/{sentShareId}/sentShareInvitations/{sentShareInvitationId}"
     path_format_arguments = {
         "sentShareId": _SERIALIZER.url(
@@ -532,16 +509,16 @@
 
 def build_sent_shares_delete_invitation_request(
     sent_share_id: str, sent_share_invitation_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-15-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-15-preview")
+    api_version: Literal["2023-05-30-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-05-30-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/sentShares/{sentShareId}/sentShareInvitations/{sentShareInvitationId}"
     path_format_arguments = {
         "sentShareId": _SERIALIZER.url(
@@ -573,16 +550,16 @@
 
 def build_sent_shares_notify_user_invitation_request(
     sent_share_id: str, sent_share_invitation_id: str, *, repeatability_request_id: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: Literal["2023-02-15-preview"] = kwargs.pop(
-        "api_version", _params.pop("api-version", "2023-02-15-preview")
+    api_version: Literal["2023-05-30-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-05-30-preview")
     )
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/sentShares/{sentShareId}/sentShareInvitations/{sentShareInvitationId}:notify"
     path_format_arguments = {
         "sentShareId": _SERIALIZER.url(
@@ -612,14 +589,41 @@
             "repeatability_request_id", repeatability_request_id, "str"
         )
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
+def build_share_resources_list_request(
+    *, filter: Optional[str] = None, order_by: Optional[str] = None, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: Literal["2023-05-30-preview"] = kwargs.pop(
+        "api_version", _params.pop("api-version", "2023-05-30-preview")
+    )
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/shareResources"
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+    if filter is not None:
+        _params["filter"] = _SERIALIZER.query("filter", filter, "str")
+    if order_by is not None:
+        _params["orderby"] = _SERIALIZER.query("order_by", order_by, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
 class ReceivedSharesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.purview.sharing.PurviewSharingClient`'s
@@ -1759,34 +1763,26 @@
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
         return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     @distributed_trace
     def list_attached(
-        self,
-        *,
-        reference_name: str,
-        skip_token: Optional[str] = None,
-        filter: Optional[str] = None,
-        orderby: Optional[str] = None,
-        **kwargs: Any
+        self, *, reference_name: str, filter: Optional[str] = None, order_by: Optional[str] = None, **kwargs: Any
     ) -> Iterable[JSON]:
         """Get a list of attached received shares.
 
         List attached received shares.
 
         :keyword reference_name: A name that references a data store. Required.
         :paramtype reference_name: str
-        :keyword skip_token: The continuation token to list the next page. Default value is None.
-        :paramtype skip_token: str
         :keyword filter: Filters the results using OData syntax. Default value is None.
         :paramtype filter: str
-        :keyword orderby: Sorts the results using OData syntax. Default value is None.
-        :paramtype orderby: str
+        :keyword order_by: Sorts the results using OData syntax. Default value is None.
+        :paramtype order_by: str
         :return: An iterator like instance of JSON object
         :rtype: ~azure.core.paging.ItemPaged[JSON]
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
                 # The response is polymorphic. The following are possible polymorphic responses based
@@ -1883,17 +1879,16 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
                 request = build_received_shares_list_attached_request(
                     reference_name=reference_name,
-                    skip_token=skip_token,
                     filter=filter,
-                    orderby=orderby,
+                    order_by=order_by,
                     api_version=self._config.api_version,
                     headers=_headers,
                     params=_params,
                 )
                 path_format_arguments = {
                     "endpoint": self._serialize.url(
                         "self._config.endpoint", self._config.endpoint, "str", skip_quote=True
@@ -1945,31 +1940,24 @@
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
     @distributed_trace
     def list_detached(
-        self,
-        *,
-        skip_token: Optional[str] = None,
-        filter: Optional[str] = None,
-        orderby: Optional[str] = None,
-        **kwargs: Any
+        self, *, filter: Optional[str] = None, order_by: Optional[str] = None, **kwargs: Any
     ) -> Iterable[JSON]:
         """Get a list of detached received shares.
 
         List detached received shares.
 
-        :keyword skip_token: The continuation token to list the next page. Default value is None.
-        :paramtype skip_token: str
         :keyword filter: Filters the results using OData syntax. Default value is None.
         :paramtype filter: str
-        :keyword orderby: Sorts the results using OData syntax. Default value is None.
-        :paramtype orderby: str
+        :keyword order_by: Sorts the results using OData syntax. Default value is None.
+        :paramtype order_by: str
         :return: An iterator like instance of JSON object
         :rtype: ~azure.core.paging.ItemPaged[JSON]
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
                 # The response is polymorphic. The following are possible polymorphic responses based
@@ -2065,17 +2053,16 @@
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
                 request = build_received_shares_list_detached_request(
-                    skip_token=skip_token,
                     filter=filter,
-                    orderby=orderby,
+                    order_by=order_by,
                     api_version=self._config.api_version,
                     headers=_headers,
                     params=_params,
                 )
                 path_format_arguments = {
                     "endpoint": self._serialize.url(
                         "self._config.endpoint", self._config.endpoint, "str", skip_quote=True
@@ -2487,34 +2474,26 @@
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(
-        self,
-        *,
-        reference_name: str,
-        skip_token: Optional[str] = None,
-        filter: Optional[str] = None,
-        orderby: Optional[str] = None,
-        **kwargs: Any
+        self, *, reference_name: str, filter: Optional[str] = None, order_by: Optional[str] = None, **kwargs: Any
     ) -> Iterable[JSON]:
         """Get a list of sent shares.
 
         List sent shares.
 
         :keyword reference_name: A name that references a data store. Required.
         :paramtype reference_name: str
-        :keyword skip_token: The continuation token to list the next page. Default value is None.
-        :paramtype skip_token: str
         :keyword filter: Filters the results using OData syntax. Default value is None.
         :paramtype filter: str
-        :keyword orderby: Sorts the results using OData syntax. Default value is None.
-        :paramtype orderby: str
+        :keyword order_by: Sorts the results using OData syntax. Default value is None.
+        :paramtype order_by: str
         :return: An iterator like instance of JSON object
         :rtype: ~azure.core.paging.ItemPaged[JSON]
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
                 # The response is polymorphic. The following are possible polymorphic responses based
@@ -2612,17 +2591,16 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
                 request = build_sent_shares_list_request(
                     reference_name=reference_name,
-                    skip_token=skip_token,
                     filter=filter,
-                    orderby=orderby,
+                    order_by=order_by,
                     api_version=self._config.api_version,
                     headers=_headers,
                     params=_params,
                 )
                 path_format_arguments = {
                     "endpoint": self._serialize.url(
                         "self._config.endpoint", self._config.endpoint, "str", skip_quote=True
@@ -3809,34 +3787,26 @@
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
         return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     @distributed_trace
     def list_invitations(
-        self,
-        sent_share_id: str,
-        *,
-        skip_token: Optional[str] = None,
-        filter: Optional[str] = None,
-        orderby: Optional[str] = None,
-        **kwargs: Any
+        self, sent_share_id: str, *, filter: Optional[str] = None, order_by: Optional[str] = None, **kwargs: Any
     ) -> Iterable[JSON]:
         """List all sent share invitations in a sent share.
 
         List sent share recipients.
 
         :param sent_share_id: Id of the sent share. Required.
         :type sent_share_id: str
-        :keyword skip_token: The continuation token to list the next page. Default value is None.
-        :paramtype skip_token: str
         :keyword filter: Filters the results using OData syntax. Default value is None.
         :paramtype filter: str
-        :keyword orderby: Sorts the results using OData syntax. Default value is None.
-        :paramtype orderby: str
+        :keyword order_by: Sorts the results using OData syntax. Default value is None.
+        :paramtype order_by: str
         :return: An iterator like instance of JSON object
         :rtype: ~azure.core.paging.ItemPaged[JSON]
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
                 # The response is polymorphic. The following are possible polymorphic responses based
@@ -3911,17 +3881,16 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
                 request = build_sent_shares_list_invitations_request(
                     sent_share_id=sent_share_id,
-                    skip_token=skip_token,
                     filter=filter,
-                    orderby=orderby,
+                    order_by=order_by,
                     api_version=self._config.api_version,
                     headers=_headers,
                     params=_params,
                 )
                 path_format_arguments = {
                     "endpoint": self._serialize.url(
                         "self._config.endpoint", self._config.endpoint, "str", skip_quote=True
@@ -4810,7 +4779,137 @@
         else:
             deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})
 
         return cast(JSON, deserialized)
+
+
+class ShareResourcesOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~azure.purview.sharing.PurviewSharingClient`'s
+        :attr:`share_resources` attribute.
+    """
+
+    def __init__(self, *args, **kwargs):
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
+
+    @distributed_trace
+    def list(self, *, filter: Optional[str] = None, order_by: Optional[str] = None, **kwargs: Any) -> Iterable[JSON]:
+        """API operation to list ShareResources.
+
+        List share resources.
+
+        :keyword filter: Filters the results using OData syntax. Default value is None.
+        :paramtype filter: str
+        :keyword order_by: Sorts the results using OData syntax. Default value is None.
+        :paramtype order_by: str
+        :return: An iterator like instance of JSON object
+        :rtype: ~azure.core.paging.ItemPaged[JSON]
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "id": "str",  # Optional. The unique id of the resource.
+                    "receivedSharesCount": 0,  # Optional. A count of Received Shares associated
+                      with the
+                      Microsoft.Azure.Purview.Share.ApiService.V3.DataTransferObjects.ShareResource.
+                    "sentSharesCount": 0,  # Optional. A count of Sent Shares associated with the
+                      Microsoft.Azure.Purview.Share.ApiService.V3.DataTransferObjects.ShareResource.
+                    "storeKind": "str",  # Optional. The types of asset. Known values are:
+                      "AdlsGen2Account" and "BlobAccount".
+                    "storeReference": {
+                        "referenceName": "str",  # Optional. Reference name for resource
+                          associated with the sink or artifact.
+                        "type": "str"  # Optional. Defines the type of resource being shared.
+                          "ArmResourceReference"
+                    },
+                    "type": "str"  # Optional. Type of the resource.
+                }
+        """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        def prepare_request(next_link=None):
+            if not next_link:
+
+                request = build_share_resources_list_request(
+                    filter=filter,
+                    order_by=order_by,
+                    api_version=self._config.api_version,
+                    headers=_headers,
+                    params=_params,
+                )
+                path_format_arguments = {
+                    "endpoint": self._serialize.url(
+                        "self._config.endpoint", self._config.endpoint, "str", skip_quote=True
+                    ),
+                }
+                request.url = self._client.format_url(request.url, **path_format_arguments)
+
+            else:
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
+                )
+                path_format_arguments = {
+                    "endpoint": self._serialize.url(
+                        "self._config.endpoint", self._config.endpoint, "str", skip_quote=True
+                    ),
+                }
+                request.url = self._client.format_url(request.url, **path_format_arguments)
+
+            return request
+
+        def extract_data(pipeline_response):
+            deserialized = pipeline_response.http_response.json()
+            list_of_elem = deserialized["value"]
+            if cls:
+                list_of_elem = cls(list_of_elem)  # type: ignore
+            return deserialized.get("nextLink") or None, iter(list_of_elem)
+
+        def get_next(next_link=None):
+            request = prepare_request(next_link)
+
+            _stream = False
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                request, stream=_stream, **kwargs
+            )
+            response = pipeline_response.http_response
+
+            if response.status_code not in [200]:
+                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                raise HttpResponseError(response=response)
+
+            return pipeline_response
+
+        return ItemPaged(get_next, extract_data)
```

## Comparing `azure-purview-sharing-1.0.0b2/azure/purview/sharing/operations/_patch.py` & `azure-purview-sharing-1.0.0b3/azure/purview/sharing/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-purview-sharing-1.0.0b2/samples/README.md` & `azure-purview-sharing-1.0.0b3/samples/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -9,32 +9,37 @@
 description: Samples for the Azure.Purview.Sharing client library.
 ---
 
 # Azure.Purview.Sharing Samples
 
 The following are code samples that show common scenario operations with the Azure Purview client library.
 
-* [sent_shares_examples.py](https://github.com/yamanwahsheh/azure-sdk-for-python/blob/yaman/share-v2-python-tests-and-samples/sdk/purview/azure-purview-sharing/samples/sent_shares_examples.py) - Examples of Sent Shares:
+* [sent_shares_examples.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/purview/azure-purview-sharing/samples/sent_shares_examples.py) - Examples of Sent Shares:
     * Create a share client
     * Create a sent share
-    * Get a sent share
-    * Delete a sent share
-    * Get all sent shares
     * Send a user invitation
     * Send a service invitation
+    * Get a sent share
+    * Get all sent shares
+    * Delete a sent share
+    * Get a sent share invitation
     * View sent invitations
+    * Delete a sent share invitation
 
-* [received_shares_examples.py](https://github.com/yamanwahsheh/azure-sdk-for-python/blob/yaman/share-v2-python-tests-and-samples/sdk/purview/azure-purview-sharing/samples/received_shares_examples.py) - Examples of Received Shares:
+* [received_shares_examples.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/purview/azure-purview-sharing/samples/received_shares_examples.py) - Examples of Received Shares:
     * Create a share client
     * Get all detached received shares
     * Attach a received share
     * Get a received share
     * List attached received shares
     * Delete a received share
 
+* [share_resources_examples.py](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/purview/azure-purview-sharing/samples/share_resources_examples.py) - Examples of Share Resources:
+    * List Share Resources
+
 ## Prerequisites
 * Python 3.6+
 * You must have an [Azure subscription](https://azure.microsoft.com/free/)
 
 ## Setup
 
 1. Install the latest beta version of Azure Purview Sharing that the samples use:
```

## Comparing `azure-purview-sharing-1.0.0b2/samples/received_shares_examples.py` & `azure-purview-sharing-1.0.0b3/samples/received_shares_examples.py`

 * *Files identical despite different names*

