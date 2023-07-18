# Comparing `tmp/pp_project_pkg-1.0.202307180257-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202307180301-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 16203 bytes, number of entries: 21
+Zip file size: 16200 bytes, number of entries: 21
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 22:23 mlflow_pipelines/__init__.py
 -rw-rw-r--  2.0 unx     1635 b- defN 23-Jul-07 09:28 mlflow_pipelines/main.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 22:23 mlflow_pipelines/fetch_data/__init__.py
 -rw-rw-r--  2.0 unx     2203 b- defN 23-Jul-13 23:55 mlflow_pipelines/fetch_data/get_data.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 22:23 mlflow_pipelines/train_model/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 22:23 mlflow_pipelines/train_model/model_train.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 22:23 mlflow_pipelines/upload_data/__init__.py
 -rw-rw-r--  2.0 unx      669 b- defN 23-Jul-07 09:28 mlflow_pipelines/upload_data/data_upload.py
 -rw-rw-r--  2.0 unx       71 b- defN 23-Jun-07 11:24 pp_project_pkg/__init__.py
 -rw-rw-r--  2.0 unx     5130 b- defN 23-Jul-07 09:28 pp_project_pkg/extra.py
 -rw-rw-r--  2.0 unx      577 b- defN 23-Jun-07 11:24 pp_project_pkg/newsvendor.py
 -rw-rw-r--  2.0 unx     9252 b- defN 23-Jun-27 22:23 pp_project_pkg/pp_tables.py
 -rw-rw-r--  2.0 unx     7661 b- defN 23-Jul-07 09:28 pp_project_pkg/train_loop.py
 -rw-rw-r--  2.0 unx     7847 b- defN 23-Jul-07 09:28 pp_project_pkg/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jul-18 02:57 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jul-18 03:01 pp_project_pkg/version.py
 -rw-rw-r--  2.0 unx     5301 b- defN 23-Jul-07 09:28 pp_project_pkg/wrangling.py
--rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-07 11:24 pp_project_pkg-1.0.202307180257.data/scripts/pp_project_run.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jul-18 02:57 pp_project_pkg-1.0.202307180257.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-18 02:57 pp_project_pkg-1.0.202307180257.dist-info/WHEEL
--rw-rw-r--  2.0 unx       32 b- defN 23-Jul-18 02:57 pp_project_pkg-1.0.202307180257.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1883 b- defN 23-Jul-18 02:57 pp_project_pkg-1.0.202307180257.dist-info/RECORD
-21 files, 44256 bytes uncompressed, 13055 bytes compressed:  70.5%
+-rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-07 11:24 pp_project_pkg-1.0.202307180301.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jul-18 03:01 pp_project_pkg-1.0.202307180301.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-18 03:01 pp_project_pkg-1.0.202307180301.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       32 b- defN 23-Jul-18 03:01 pp_project_pkg-1.0.202307180301.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1883 b- defN 23-Jul-18 03:01 pp_project_pkg-1.0.202307180301.dist-info/RECORD
+21 files, 44256 bytes uncompressed, 13052 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307180257.data/scripts/pp_project_run.py
+Filename: pp_project_pkg-1.0.202307180301.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307180257.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202307180301.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307180257.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202307180301.dist-info/WHEEL
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307180257.dist-info/top_level.txt
+Filename: pp_project_pkg-1.0.202307180301.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307180257.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202307180301.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pp_project_pkg/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('07')
 VERSION_DAY = int('18')
-VERSION_HOUR = int('02')
-VERSION_MINUTE = int('57')
+VERSION_HOUR = int('03')
+VERSION_MINUTE = int('01')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202307180257
-version_date = '2023/07/18 02:57'
+PATCH_VERSION = 202307180301
+version_date = '2023/07/18 03:01'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `pp_project_pkg-1.0.202307180257.data/scripts/pp_project_run.py` & `pp_project_pkg-1.0.202307180301.data/scripts/pp_project_run.py`

 * *Files identical despite different names*

## Comparing `pp_project_pkg-1.0.202307180257.dist-info/RECORD` & `pp_project_pkg-1.0.202307180301.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,14 @@
 mlflow_pipelines/upload_data/data_upload.py,sha256=13sSSQBDWKgXSVJaHLy1sN_cUHuFvv4MwJaOJE0brXk,669
 pp_project_pkg/__init__.py,sha256=9idX2X6SQKZg--ziGy6Ii9OB-kz9hOX1nEG9a0xEW9g,71
 pp_project_pkg/extra.py,sha256=RreiMggIbiIxM4St8jtlyoUpW7hTxhwyJZ1M_w2UNqc,5130
 pp_project_pkg/newsvendor.py,sha256=E6JHp0Vtmq63toKM6bO3xTAdCgwmAZzRua-w10wrc5Y,577
 pp_project_pkg/pp_tables.py,sha256=aNBP-aExfiPWTINChNLIzIIgTUrVo-z26Oq8cLTky2w,9252
 pp_project_pkg/train_loop.py,sha256=w5h4JaroFvA_yYeU2VKe5K6XucSuE_vJs_kQYFzZKi8,7661
 pp_project_pkg/utils.py,sha256=4qIYSi8u7uO2HujXvkYnV4FQ8tyOUbH3Cri8N_aJsY4,7847
-pp_project_pkg/version.py,sha256=NmrYYImNr6L7Dj4gYpioyzIHYKoNqOoZ4-6mxZWJwTY,396
+pp_project_pkg/version.py,sha256=s2oUFciYhYoCgNWfPABObuBBhpC93suQEd8CAYuo3qs,396
 pp_project_pkg/wrangling.py,sha256=0l0_MMgUEyjNlwOmrYrEj7pNtvCT_LyZFXOiKSko3PM,5301
-pp_project_pkg-1.0.202307180257.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
-pp_project_pkg-1.0.202307180257.dist-info/METADATA,sha256=T1XR9R1qS3piadyav-3y9XICSMBsTkY_3RyRw1vl7mQ,191
-pp_project_pkg-1.0.202307180257.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-pp_project_pkg-1.0.202307180257.dist-info/top_level.txt,sha256=aTmpGcM2s0GVN0z4bWc23t0I3mXhHxeqKNzUWghwIRA,32
-pp_project_pkg-1.0.202307180257.dist-info/RECORD,,
+pp_project_pkg-1.0.202307180301.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
+pp_project_pkg-1.0.202307180301.dist-info/METADATA,sha256=FPVdSH5ugjDU5kM_dRzGtmPxMT7Wkek5wkfpl1ysa0A,191
+pp_project_pkg-1.0.202307180301.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+pp_project_pkg-1.0.202307180301.dist-info/top_level.txt,sha256=aTmpGcM2s0GVN0z4bWc23t0I3mXhHxeqKNzUWghwIRA,32
+pp_project_pkg-1.0.202307180301.dist-info/RECORD,,
```

