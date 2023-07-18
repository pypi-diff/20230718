# Comparing `tmp/gordo_client-6.2.2-py3-none-any.whl.zip` & `tmp/gordo_client-6.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 44602 bytes, number of entries: 17
+Zip file size: 44601 bytes, number of entries: 17
 -rw-r--r--  2.0 unx    34282 b- defN 80-Jan-01 00:00 LICENSE
 -rw-r--r--  2.0 unx      497 b- defN 80-Jan-01 00:00 gordo_client/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 gordo_client/cli/__init__.py
 -rw-r--r--  2.0 unx     8256 b- defN 80-Jan-01 00:00 gordo_client/cli/client.py
 -rw-r--r--  2.0 unx     1282 b- defN 80-Jan-01 00:00 gordo_client/cli/custom_types.py
 -rw-r--r--  2.0 unx    22869 b- defN 80-Jan-01 00:00 gordo_client/client.py
 -rw-r--r--  2.0 unx     5351 b- defN 80-Jan-01 00:00 gordo_client/dataframe.py
 -rw-r--r--  2.0 unx      347 b- defN 80-Jan-01 00:00 gordo_client/dist.py
 -rw-r--r--  2.0 unx     8574 b- defN 80-Jan-01 00:00 gordo_client/forwarders.py
 -rw-r--r--  2.0 unx     3545 b- defN 80-Jan-01 00:00 gordo_client/io.py
 -rw-r--r--  2.0 unx     1741 b- defN 80-Jan-01 00:00 gordo_client/schemas.py
 -rw-r--r--  2.0 unx     2669 b- defN 80-Jan-01 00:00 gordo_client/utils.py
--rw-r--r--  2.0 unx    34282 b- defN 80-Jan-01 00:00 gordo_client-6.2.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     2544 b- defN 80-Jan-01 00:00 gordo_client-6.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 gordo_client-6.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       69 b- defN 80-Jan-01 00:00 gordo_client-6.2.2.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1368 b- defN 16-Jan-01 00:00 gordo_client-6.2.2.dist-info/RECORD
-17 files, 127764 bytes uncompressed, 42370 bytes compressed:  66.8%
+-rw-r--r--  2.0 unx    34282 b- defN 80-Jan-01 00:00 gordo_client-6.2.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2540 b- defN 80-Jan-01 00:00 gordo_client-6.2.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 gordo_client-6.2.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       69 b- defN 80-Jan-01 00:00 gordo_client-6.2.3.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1368 b- defN 16-Jan-01 00:00 gordo_client-6.2.3.dist-info/RECORD
+17 files, 127760 bytes uncompressed, 42369 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: gordo_client/schemas.py
 Comment: 
 
 Filename: gordo_client/utils.py
 Comment: 
 
-Filename: gordo_client-6.2.2.dist-info/LICENSE
+Filename: gordo_client-6.2.3.dist-info/LICENSE
 Comment: 
 
-Filename: gordo_client-6.2.2.dist-info/METADATA
+Filename: gordo_client-6.2.3.dist-info/METADATA
 Comment: 
 
-Filename: gordo_client-6.2.2.dist-info/WHEEL
+Filename: gordo_client-6.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: gordo_client-6.2.2.dist-info/entry_points.txt
+Filename: gordo_client-6.2.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: gordo_client-6.2.2.dist-info/RECORD
+Filename: gordo_client-6.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `gordo_client-6.2.2.dist-info/LICENSE` & `gordo_client-6.2.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gordo_client-6.2.2.dist-info/METADATA` & `gordo_client-6.2.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gordo-client
-Version: 6.2.2
+Version: 6.2.3
 Summary: Gordo client
 Home-page: https://github.com/equinor/gordo-client
 License: AGPL-3.0
 Keywords: gordo-client
 Author: Equinor ASA
 Author-email: fg_gpl@equinor.com
 Requires-Python: >=3.9,<4.0
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
-Requires-Dist: PyYAML (>=5.3.1,<6.0.0)
+Requires-Dist: PyYAML (>=5.3.1,<7)
 Requires-Dist: click (>=7.0.0,<9.0.0)
 Requires-Dist: gordo-core (>=0.3.0,<0.4.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: requests (>=2.20,<3.0)
 Requires-Dist: simplejson (>=3.17.2,<4.0.0)
 Requires-Dist: wrapt (>=1.11.0,<2.0.0)
 Project-URL: Repository, https://github.com/equinor/gordo-client
```

## Comparing `gordo_client-6.2.2.dist-info/RECORD` & `gordo_client-6.2.3.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -6,12 +6,12 @@
 gordo_client/client.py,sha256=WpCrHmOXLbsaFWkYhkVnDMbtfT1zYhkSUzsMhAM8sX0,22869
 gordo_client/dataframe.py,sha256=8JPreh239zndjFd6qE4wvLfQrzh1EaH1dArOwwf0UXQ,5351
 gordo_client/dist.py,sha256=y18r-Cl2oHsSgy92zCRP0AvbmV-JVhu264CvgWOeOZo,347
 gordo_client/forwarders.py,sha256=VF5BrfozoU1fDmifmJPGkOGFd7b39K_k1lbFUP61Y_g,8574
 gordo_client/io.py,sha256=7EPiLCC7YOcv7A02bW9SsdQ4_n-ZvGeGaKnhATK9_rI,3545
 gordo_client/schemas.py,sha256=FBwKLa8I-9Y0rJufF0rCqDKYuvSUUyBzXQ1Ndkr5piA,1741
 gordo_client/utils.py,sha256=nkuZfOZtORlN_KPP-ydY1lsWz7Mm8Muy8HCPdbxv3s8,2669
-gordo_client-6.2.2.dist-info/LICENSE,sha256=YiL99kco2RvveX-uHGEPl3N99n_QcCa3qD1mElL9reY,34282
-gordo_client-6.2.2.dist-info/METADATA,sha256=TAcN6UQIqACJvTEZL1WSeB7uE_PcgnGRyzlFMjfaXA0,2544
-gordo_client-6.2.2.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-gordo_client-6.2.2.dist-info/entry_points.txt,sha256=7RFsbTmjxqibiaeAOUHH6P7UEb_hkENjEIDShFVXF4k,69
-gordo_client-6.2.2.dist-info/RECORD,,
+gordo_client-6.2.3.dist-info/LICENSE,sha256=YiL99kco2RvveX-uHGEPl3N99n_QcCa3qD1mElL9reY,34282
+gordo_client-6.2.3.dist-info/METADATA,sha256=6MhdDmZ0COcJUdHeJxRFxCwQmlSNvZALH6Hfs2vvAM0,2540
+gordo_client-6.2.3.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+gordo_client-6.2.3.dist-info/entry_points.txt,sha256=7RFsbTmjxqibiaeAOUHH6P7UEb_hkENjEIDShFVXF4k,69
+gordo_client-6.2.3.dist-info/RECORD,,
```

