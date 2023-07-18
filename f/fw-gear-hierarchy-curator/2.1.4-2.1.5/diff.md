# Comparing `tmp/fw_gear_hierarchy_curator-2.1.4-py3-none-any.whl.zip` & `tmp/fw_gear_hierarchy_curator-2.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5880 bytes, number of entries: 7
+Zip file size: 5903 bytes, number of entries: 7
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 fw_gear_hierarchy_curator/__init__.py
 -rw-r--r--  2.0 unx     8512 b- defN 80-Jan-01 00:00 fw_gear_hierarchy_curator/curate.py
 -rw-r--r--  2.0 unx     1115 b- defN 80-Jan-01 00:00 fw_gear_hierarchy_curator/parser.py
 -rw-r--r--  2.0 unx     2664 b- defN 80-Jan-01 00:00 fw_gear_hierarchy_curator/utils.py
-?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 fw_gear_hierarchy_curator-2.1.4.dist-info/WHEEL
-?rw-r--r--  2.0 unx      897 b- defN 16-Jan-01 00:00 fw_gear_hierarchy_curator-2.1.4.dist-info/METADATA
-?rw-r--r--  2.0 unx      625 b- defN 16-Jan-01 00:00 fw_gear_hierarchy_curator-2.1.4.dist-info/RECORD
-7 files, 13896 bytes uncompressed, 4754 bytes compressed:  65.8%
+-rw-r--r--  2.0 unx      980 b- defN 80-Jan-01 00:00 fw_gear_hierarchy_curator-2.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_gear_hierarchy_curator-2.1.5.dist-info/WHEEL
+?rw-r--r--  2.0 unx      625 b- defN 16-Jan-01 00:00 fw_gear_hierarchy_curator-2.1.5.dist-info/RECORD
+7 files, 13984 bytes uncompressed, 4777 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -6,17 +6,17 @@
 
 Filename: fw_gear_hierarchy_curator/parser.py
 Comment: 
 
 Filename: fw_gear_hierarchy_curator/utils.py
 Comment: 
 
-Filename: fw_gear_hierarchy_curator-2.1.4.dist-info/WHEEL
+Filename: fw_gear_hierarchy_curator-2.1.5.dist-info/METADATA
 Comment: 
 
-Filename: fw_gear_hierarchy_curator-2.1.4.dist-info/METADATA
+Filename: fw_gear_hierarchy_curator-2.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: fw_gear_hierarchy_curator-2.1.4.dist-info/RECORD
+Filename: fw_gear_hierarchy_curator-2.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `fw_gear_hierarchy_curator-2.1.4.dist-info/METADATA` & `fw_gear_hierarchy_curator-2.1.5.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: fw-gear-hierarchy-curator
-Version: 2.1.4
+Version: 2.1.5
 Summary: Custom hierarchy curation gear
 License: MIT
 Author: Flywheel
 Author-email: support@flywheel.io
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=9,<10)
 Requires-Dist: backoff (>=1.11.1,<2.0.0)
-Requires-Dist: flywheel-gear-toolkit[all] (>=0.6.1,<0.7.0)
-Requires-Dist: flywheel-sdk (>=15.8.0,<16.0.0)
-Requires-Dist: fw-file (>=1,<2)
+Requires-Dist: flywheel-gear-toolkit (>=0.6.11,<0.7.0)
+Requires-Dist: flywheel-sdk (>=17.1.1,<18.0.0)
+Requires-Dist: fw-file (>=2.3.0,<3.0.0)
 Requires-Dist: lxml (>=4.6.1,<5.0.0)
-Requires-Dist: nibabel (>=3.2.0,<4.0.0)
+Requires-Dist: nibabel (>=5.1.0,<6.0.0)
+Requires-Dist: nipype (>=1.8.6,<2.0.0)
+Requires-Dist: numpy (>=1.25.1,<2.0.0)
 Requires-Dist: pandas (>=1.1.4,<2.0.0)
 Requires-Dist: piexif (>=1.1.3,<2.0.0)
 Requires-Dist: pydicom (>=2.1.1,<3.0.0)
 Requires-Dist: pypng (>=0.0.20,<0.0.21)
```

## Comparing `fw_gear_hierarchy_curator-2.1.4.dist-info/RECORD` & `fw_gear_hierarchy_curator-2.1.5.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 fw_gear_hierarchy_curator/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fw_gear_hierarchy_curator/curate.py,sha256=osaF6tx-Y5J17WV3Lk6nL1T8bxKcCaeT8CKEEkqjvBE,8512
 fw_gear_hierarchy_curator/parser.py,sha256=oFslq8m9JNqd98DzF5IACZE-xyhl4uZ4FIHa8eLmDBA,1115
 fw_gear_hierarchy_curator/utils.py,sha256=XS2yWutqknk3zWSY2YXn2qLOjr61qyaahog_kyQUX-4,2664
-fw_gear_hierarchy_curator-2.1.4.dist-info/WHEEL,sha256=y3eDiaFVSNTPbgzfNn0nYn5tEn1cX6WrdetDlQM4xWw,83
-fw_gear_hierarchy_curator-2.1.4.dist-info/METADATA,sha256=V2Fbk2LpuXg2ATiMGapcB_7uMMXaNIUQba9boZKLiY8,897
-fw_gear_hierarchy_curator-2.1.4.dist-info/RECORD,,
+fw_gear_hierarchy_curator-2.1.5.dist-info/METADATA,sha256=G2ZyNpciO2DEwcLeviu1pNB7oksIMddzU0mZQc9dmZE,980
+fw_gear_hierarchy_curator-2.1.5.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+fw_gear_hierarchy_curator-2.1.5.dist-info/RECORD,,
```

