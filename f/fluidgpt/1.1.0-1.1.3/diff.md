# Comparing `tmp/fluidgpt-1.1.0-cp39-cp39-win_amd64.whl.zip` & `tmp/fluidgpt-1.1.3-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 145880 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-10 11:01 fluidgpt/__init__.py
--rw-rw-rw-  2.0 fat      140 b- defN 23-Jul-10 11:01 fluidgpt/fluidai_gpt_sdk/__init__.py
--rw-rw-rw-  2.0 fat    55296 b- defN 23-Jul-10 11:01 fluidgpt/fluidai_gpt_sdk/endpoints.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat    89600 b- defN 23-Jul-10 11:01 fluidgpt/fluidai_gpt_sdk/jupyter_helper.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat    26624 b- defN 23-Jul-10 11:01 fluidgpt/fluidai_gpt_sdk/prompt_list.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      113 b- defN 23-Jul-10 11:01 fluidgpt/validation/__init__.py
--rw-rw-rw-  2.0 fat    68096 b- defN 23-Jul-10 11:01 fluidgpt/validation/authentication.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat    80896 b- defN 23-Jul-10 11:01 fluidgpt/validation/credentials_authentication.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      745 b- defN 23-Jul-10 11:01 fluidgpt-1.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-10 11:01 fluidgpt-1.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-10 11:01 fluidgpt-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1128 b- defN 23-Jul-10 11:01 fluidgpt-1.1.0.dist-info/RECORD
-12 files, 322747 bytes uncompressed, 143940 bytes compressed:  55.4%
+Zip file size: 172636 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-18 17:28 fluidgpt/__init__.py
+-rw-rw-rw-  2.0 fat      140 b- defN 23-Jul-18 17:28 fluidgpt/fluidai_gpt_sdk/__init__.py
+-rw-rw-rw-  2.0 fat    66560 b- defN 23-Jul-18 17:28 fluidgpt/fluidai_gpt_sdk/endpoints.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   104960 b- defN 23-Jul-18 17:28 fluidgpt/fluidai_gpt_sdk/jupyter_helper.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    31232 b- defN 23-Jul-18 17:28 fluidgpt/fluidai_gpt_sdk/prompt_list.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      113 b- defN 23-Jul-18 17:28 fluidgpt/validation/__init__.py
+-rw-rw-rw-  2.0 fat    77824 b- defN 23-Jul-18 17:28 fluidgpt/validation/authentication.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    93696 b- defN 23-Jul-18 17:28 fluidgpt/validation/credentials_authentication.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      745 b- defN 23-Jul-18 17:28 fluidgpt-1.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-18 17:28 fluidgpt-1.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-18 17:28 fluidgpt-1.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1129 b- defN 23-Jul-18 17:28 fluidgpt-1.1.3.dist-info/RECORD
+12 files, 376508 bytes uncompressed, 170696 bytes compressed:  54.7%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: fluidgpt/validation/authentication.cp39-win_amd64.pyd
 Comment: 
 
 Filename: fluidgpt/validation/credentials_authentication.cp39-win_amd64.pyd
 Comment: 
 
-Filename: fluidgpt-1.1.0.dist-info/METADATA
+Filename: fluidgpt-1.1.3.dist-info/METADATA
 Comment: 
 
-Filename: fluidgpt-1.1.0.dist-info/WHEEL
+Filename: fluidgpt-1.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: fluidgpt-1.1.0.dist-info/top_level.txt
+Filename: fluidgpt-1.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: fluidgpt-1.1.0.dist-info/RECORD
+Filename: fluidgpt-1.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `fluidgpt-1.1.0.dist-info/METADATA` & `fluidgpt-1.1.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluidgpt
-Version: 1.1.0
+Version: 1.1.3
 Summary: Run different validation tests on machine learning models.
 Home-page: https://github.com/
 Author: FluidAI
 Author-email: info@fluid.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `fluidgpt-1.1.0.dist-info/RECORD` & `fluidgpt-1.1.3.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 fluidgpt/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fluidgpt/fluidai_gpt_sdk/__init__.py,sha256=WLrw_3XJyBU5pQVS_BPF_VdMgGZw1u9ZUHvGlYbrD9I,140
-fluidgpt/fluidai_gpt_sdk/endpoints.cp39-win_amd64.pyd,sha256=ecdTEKHSMt7DRfjTCX1e6D3VooGLASC0vGwR0yrmYL8,55296
-fluidgpt/fluidai_gpt_sdk/jupyter_helper.cp39-win_amd64.pyd,sha256=K8aoX1_toy0wa_vIKmFtAAxfT5O8jS95kG6M7-dVHqM,89600
-fluidgpt/fluidai_gpt_sdk/prompt_list.cp39-win_amd64.pyd,sha256=XUdApNKoNfC5V01c0Y4QIwL3s-poLV7SvYnVwmx9TNg,26624
+fluidgpt/fluidai_gpt_sdk/endpoints.cp39-win_amd64.pyd,sha256=pTHzR3TbZnyCuJTE2cthUpHdUYC3BEZCH7Z3VZjO7zU,66560
+fluidgpt/fluidai_gpt_sdk/jupyter_helper.cp39-win_amd64.pyd,sha256=U2tBI7UDdnhXSrJ6A-0H6dFxWERIMZvSmcUI9sZm2yU,104960
+fluidgpt/fluidai_gpt_sdk/prompt_list.cp39-win_amd64.pyd,sha256=i4hvh_XAq73slDkeFK6htRW59LW43Mj9z1l8T2GIsOc,31232
 fluidgpt/validation/__init__.py,sha256=nVbp996PbMLxhSJE7rFMPxfogDTPEkatLimrwEc-nQs,113
-fluidgpt/validation/authentication.cp39-win_amd64.pyd,sha256=oGa8FSGMiE22puEpz9vqb2ukB_bemSU9g1h5W2hiQPs,68096
-fluidgpt/validation/credentials_authentication.cp39-win_amd64.pyd,sha256=SXNXvUwaXiNWz2W_ex0fTwOEvGiY0UcZ_-M_S9LgGc4,80896
-fluidgpt-1.1.0.dist-info/METADATA,sha256=T0AoXiXowkAe8znt6_ySbo9UHTpv2pBUjVSRiPK554A,745
-fluidgpt-1.1.0.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-fluidgpt-1.1.0.dist-info/top_level.txt,sha256=wvmCfKc--Y9YazKg9wWJeEF4Det2AAMEhjEEcm-nXT0,9
-fluidgpt-1.1.0.dist-info/RECORD,,
+fluidgpt/validation/authentication.cp39-win_amd64.pyd,sha256=pYSYhBImYbsnHgDnXM1kLMSnyg1kaV8Vau9cRox1h6g,77824
+fluidgpt/validation/credentials_authentication.cp39-win_amd64.pyd,sha256=7ljYgorFUMV238wIDwKUGslUa2ZGHVTU-8B7OaOHfGA,93696
+fluidgpt-1.1.3.dist-info/METADATA,sha256=RS1-H3BlRv5_87caKkd5Jfa1-9KCRlO1CY2VTdaUqdQ,745
+fluidgpt-1.1.3.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+fluidgpt-1.1.3.dist-info/top_level.txt,sha256=wvmCfKc--Y9YazKg9wWJeEF4Det2AAMEhjEEcm-nXT0,9
+fluidgpt-1.1.3.dist-info/RECORD,,
```

