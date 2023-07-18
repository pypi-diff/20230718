# Comparing `tmp/adafri-0.0.19.42.tar.gz` & `tmp/adafri-0.0.19.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.19.42.tar", last modified: Mon Jul 17 02:53:26 2023, max compression
+gzip compressed data, was "adafri-0.0.19.43.tar", last modified: Tue Jul 18 00:37:00 2023, max compression
```

## Comparing `adafri-0.0.19.42.tar` & `adafri-0.0.19.43.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:53:26.638384 adafri-0.0.19.42/
--rw-r--r--   0 ibrahima   (502) staff       (20)      180 2023-07-17 02:53:26.638008 adafri-0.0.19.42/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:53:26.608317 adafri-0.0.19.42/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       83 2023-07-17 02:53:13.000000 adafri-0.0.19.42/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:53:26.613687 adafri-0.0.19.42/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.19.42/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.19.42/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    15213 2023-07-13 01:22:12.000000 adafri-0.0.19.42/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:53:26.614577 adafri-0.0.19.42/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.19.42/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:53:26.615518 adafri-0.0.19.42/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.19.42/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:53:26.618249 adafri-0.0.19.42/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.19.42/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.19.42/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.19.42/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:53:26.619337 adafri-0.0.19.42/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.19.42/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:53:26.620810 adafri-0.0.19.42/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.19.42/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.19.42/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:53:26.621806 adafri-0.0.19.42/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.19.42/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:53:26.622366 adafri-0.0.19.42/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-16 07:53:07.000000 adafri-0.0.19.42/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:53:26.629157 adafri-0.0.19.42/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.19.42/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6514 2023-07-17 02:30:36.000000 adafri-0.0.19.42/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.19.42/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    14105 2023-07-17 02:38:36.000000 adafri-0.0.19.42/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3219 2023-07-16 05:04:45.000000 adafri-0.0.19.42/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9139 2023-07-15 08:33:33.000000 adafri-0.0.19.42/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3212 2023-07-12 22:48:16.000000 adafri-0.0.19.42/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:53:26.631562 adafri-0.0.19.42/adafri/v1/auth/oauth/server/
--rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.19.42/adafri/v1/auth/oauth/server/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)      885 2023-07-17 02:53:04.000000 adafri-0.0.19.42/adafri/v1/auth/oauth/server/oidc_server.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2200 2023-07-16 05:37:41.000000 adafri-0.0.19.42/adafri/v1/auth/oauth/server/server.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:53:26.633365 adafri-0.0.19.42/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.19.42/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.19.42/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:53:26.634044 adafri-0.0.19.42/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.19.42/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:53:26.637029 adafri-0.0.19.42/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.19.42/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.19.42/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.19.42/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-17 02:53:26.611272 adafri-0.0.19.42/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      180 2023-07-17 02:53:26.000000 adafri-0.0.19.42/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1167 2023-07-17 02:53:26.000000 adafri-0.0.19.42/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-17 02:53:26.000000 adafri-0.0.19.42/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-17 02:53:26.000000 adafri-0.0.19.42/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-17 02:53:26.638533 adafri-0.0.19.42/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.19.42/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 00:37:00.113004 adafri-0.0.19.43/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      180 2023-07-18 00:37:00.112647 adafri-0.0.19.43/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 00:37:00.088630 adafri-0.0.19.43/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       83 2023-07-18 00:36:55.000000 adafri-0.0.19.43/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 00:37:00.093036 adafri-0.0.19.43/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.19.43/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.19.43/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    15213 2023-07-13 01:22:12.000000 adafri-0.0.19.43/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 00:37:00.093878 adafri-0.0.19.43/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.19.43/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 00:37:00.094669 adafri-0.0.19.43/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.19.43/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 00:37:00.097360 adafri-0.0.19.43/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.19.43/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.19.43/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.19.43/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 00:37:00.098150 adafri-0.0.19.43/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.19.43/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 00:37:00.099498 adafri-0.0.19.43/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.19.43/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.19.43/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 00:37:00.100317 adafri-0.0.19.43/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.19.43/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 00:37:00.100718 adafri-0.0.19.43/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-18 00:36:46.000000 adafri-0.0.19.43/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 00:37:00.105684 adafri-0.0.19.43/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.19.43/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6514 2023-07-17 02:30:36.000000 adafri-0.0.19.43/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.19.43/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    14112 2023-07-17 04:35:50.000000 adafri-0.0.19.43/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3219 2023-07-16 05:04:45.000000 adafri-0.0.19.43/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9130 2023-07-18 00:36:13.000000 adafri-0.0.19.43/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3212 2023-07-12 22:48:16.000000 adafri-0.0.19.43/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 00:37:00.107850 adafri-0.0.19.43/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.19.43/adafri/v1/auth/oauth/server/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1345 2023-07-18 00:33:08.000000 adafri-0.0.19.43/adafri/v1/auth/oauth/server/oidc_server.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2655 2023-07-18 00:34:16.000000 adafri-0.0.19.43/adafri/v1/auth/oauth/server/server.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 00:37:00.109150 adafri-0.0.19.43/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.19.43/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.19.43/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 00:37:00.109580 adafri-0.0.19.43/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.19.43/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 00:37:00.111805 adafri-0.0.19.43/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.19.43/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.19.43/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.19.43/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-18 00:37:00.090837 adafri-0.0.19.43/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      180 2023-07-18 00:36:59.000000 adafri-0.0.19.43/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1167 2023-07-18 00:37:00.000000 adafri-0.0.19.43/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-18 00:36:59.000000 adafri-0.0.19.43/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-18 00:36:59.000000 adafri-0.0.19.43/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-18 00:37:00.113160 adafri-0.0.19.43/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.19.43/setup.py
```

### Comparing `adafri-0.0.19.42/adafri/utils/response.py` & `adafri-0.0.19.43/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.42/adafri/utils/utils.py` & `adafri-0.0.19.43/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.42/adafri/v1/account/models/account.py` & `adafri-0.0.19.43/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.42/adafri/v1/account/models/account_fields.py` & `adafri-0.0.19.43/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.42/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.19.43/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.42/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.19.43/adafri/v1/auth/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.42/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.19.43/adafri/v1/auth/oauth/models/client.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.42/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.19.43/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.42/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.19.43/adafri/v1/auth/oauth/models/grant.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,8 +330,10 @@
     def exists_nonce(self, nonce, request):
         return exists_nonce(nonce, request)
 
     def get_jwt_config(self):
         return DUMMY_JWT_CONFIG
 
     def generate_user_info(self, user, scope):
-        return generate_user_info(user, scope)
+        return generate_user_info(user, scope)
+    
+
```

### Comparing `adafri-0.0.19.42/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.19.43/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.42/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.19.43/adafri/v1/auth/oauth/models/token.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,16 +136,14 @@
 class TokenValidator(BearerTokenValidator):
     def authenticate_token(self, token_string):
         token_request = OAuthToken().query([{"key":"access_token", "comp": "==", "value": token_string}], True)
         return token_request
     
     def validate_token(self, token, scopes, request):
         token_scopes = scope_to_list(token.scope);
-        print('token_scopes', token_scopes)
-        print('scopes', scopes)
         insufficient = self.scope_insufficient(token_scopes, scopes);
         if insufficient:
             response = ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error("Insufficient privilegies","INVALID_REQUEST", 1)).to_json()
             return abort(Response(response=json.dumps(response), status=401, mimetype='application/json'))        
         return None
 
 class TokenRevocationEndpoint(RevocationEndpoint):
@@ -184,14 +182,17 @@
 
 DEFAULT_EXPIRES_IN = 3600
 class TokenGenerator(BearerTokenGenerator):
     @staticmethod
     def generate(grant_type, client, user=None, scope=None, expires_in=None, include_refresh_token=True):
         if expires_in is None:
             expires_in = DEFAULT_EXPIRES_IN
-        expires_at = datetime.now() + timedelta(seconds=DEFAULT_EXPIRES_IN)
-        token = {'token_type': 'Bearer', "client_id": client.client_id, "uid": client.uid, 'scope': scope, 'expires_in': expires_in, "grant_type": grant_type, 'expired_at': expires_at.isoformat()}
+        uid = client.uid;
+        if user is not None:
+            uid = user.uid
+        expires_at = datetime.now() + timedelta(seconds=expires_in)
+        token = {'token_type': 'Bearer', "client_id": client.client_id, "uid": uid, 'scope': scope, 'expires_in': expires_in, "grant_type": grant_type, 'expired_at': expires_at.isoformat()}
         access_token = Crypto().generate_token("access_token~"+json.dumps(token));
         token['access_token'] = access_token;
         if include_refresh_token:
             token['refresh_token'] = Crypto().generate_token("refresh_token~"+json.dumps(token));
         return token
```

### Comparing `adafri-0.0.19.42/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.19.43/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.42/adafri/v1/auth/oauth/server/server.py` & `adafri-0.0.19.43/adafri/v1/auth/oauth/server/server.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,27 +27,36 @@
 #     save_token=OAuthToken().save,
 # )
 authorization_server = AuthorizationServer()
 require_oauth = ResourceProtector()
 
 require_oauth = ResourceProtector()
 
-def config_oauth(app):
-    authorization_server.query_client = OAuthClient().get_by_client_id
-    authorization_server.save_token = OAuthToken().save
+def config_oauth(app, query_client=None, save_token=None, token_generator=None):
+    if query_client is None:
+        query_client = OAuthClient().get_by_client_id
+    if save_token is None:
+        save_token = OAuthToken().save
+    authorization_server.query_client = query_client
+    authorization_server.save_token = save_token
     authorization_server.init_app(app)
     
     authorization_server.register_grant(grants.ImplicitGrant)
     #authorization_server.register_grant(AccessTokenGrant, [CodeChallenge(required=True)])
     authorization_server.register_grant(grants.ClientCredentialsGrant)
     authorization_server.register_grant(AuthCodeGrant, [CodeChallenge(required=True)])
     
     # authorization_server.register_grant(PasswordGrant)
     authorization_server.register_grant(RefreshTokenGrant)
     # support revocation
     # revocation_cls = create_revocation_endpoint()
     authorization_server.register_endpoint(TokenRevocationEndpoint)
+    if token_generator is not None:
+        type = getattr(token_generator, 'type', None);
+        generator = getattr(token_generator, 'generator', None);
+        if None not in [type, generator]:
+            authorization_server.register_token_generator(type, generator)
     # authorization_server.register_token_generator("default", TokenGenerator.generate)
     # authorization_server.register_token_generator("client_credentials", TokenGenerator.generate)
     # protect resource
     #bearer_cls = create_bearer_token_validator(TokenValidator)
     require_oauth.register_token_validator(TokenValidator())
```

### Comparing `adafri-0.0.19.42/adafri/v1/base/firebase_collection.py` & `adafri-0.0.19.43/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.42/adafri/v1/user/models/user.py` & `adafri-0.0.19.43/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.42/adafri/v1/user/models/user_fields.py` & `adafri-0.0.19.43/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.42/adafri.egg-info/SOURCES.txt` & `adafri-0.0.19.43/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.42/setup.py` & `adafri-0.0.19.43/setup.py`

 * *Files identical despite different names*

