# Comparing `tmp/lnauth_django-0.3.0.tar.gz` & `tmp/lnauth_django-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnauth_django-0.3.0.tar", max compression
+gzip compressed data, was "lnauth_django-0.4.0.tar", max compression
```

## Comparing `lnauth_django-0.3.0.tar` & `lnauth_django-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2023-06-24 22:25:50.420220 lnauth_django-0.3.0/LICENSE
--rw-r--r--   0        0        0     2708 2023-06-27 18:09:02.875869 lnauth_django-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-06-24 22:25:50.380220 lnauth_django-0.3.0/lnauth_django/__init__.py
--rw-r--r--   0        0        0      148 2023-06-24 22:34:51.066120 lnauth_django-0.3.0/lnauth_django/apps.py
--rw-r--r--   0        0        0     1826 2023-06-27 18:09:11.895982 lnauth_django-0.3.0/lnauth_django/django_auth.py
--rw-r--r--   0        0        0      141 2023-06-24 23:33:50.028248 lnauth_django-0.3.0/lnauth_django/exceptions.py
--rw-r--r--   0        0        0     1382 2023-06-24 22:50:06.437211 lnauth_django-0.3.0/lnauth_django/lnauth.py
--rw-r--r--   0        0        0      786 2023-06-26 23:23:58.916632 lnauth_django-0.3.0/lnauth_django/migrations/0000_initial.py
--rw-r--r--   0        0        0        0 2023-06-26 23:21:16.365884 lnauth_django-0.3.0/lnauth_django/migrations/__init__.py
--rw-r--r--   0        0        0      266 2023-06-24 23:33:50.044247 lnauth_django-0.3.0/lnauth_django/models.py
--rw-r--r--   0        0        0        0 2023-06-24 22:31:09.280965 lnauth_django-0.3.0/lnauth_django/tests/__init__.py
--rw-r--r--   0        0        0     1522 2023-06-24 23:33:21.865177 lnauth_django-0.3.0/lnauth_django/tests/test_service.py
--rw-r--r--   0        0        0      297 2023-06-24 22:33:44.897736 lnauth_django-0.3.0/lnauth_django/urls.py
--rw-r--r--   0        0        0     2578 2023-06-27 18:09:07.447926 lnauth_django-0.3.0/lnauth_django/views.py
--rw-r--r--   0        0        0      437 2023-06-27 17:53:36.859201 lnauth_django-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3256 1970-01-01 00:00:00.000000 lnauth_django-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-24 22:25:50.420220 lnauth_django-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2726 2023-06-27 18:15:34.056728 lnauth_django-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-24 22:25:50.380220 lnauth_django-0.4.0/lnauth_django/__init__.py
+-rw-r--r--   0        0        0      148 2023-06-24 22:34:51.066120 lnauth_django-0.4.0/lnauth_django/apps.py
+-rw-r--r--   0        0        0     3041 2023-07-18 12:14:53.656821 lnauth_django-0.4.0/lnauth_django/django_auth.py
+-rw-r--r--   0        0        0      141 2023-06-24 23:33:50.028248 lnauth_django-0.4.0/lnauth_django/exceptions.py
+-rw-r--r--   0        0        0     1445 2023-07-18 12:14:26.612514 lnauth_django-0.4.0/lnauth_django/lnauth.py
+-rw-r--r--   0        0        0      786 2023-06-26 23:23:58.916632 lnauth_django-0.4.0/lnauth_django/migrations/0000_initial.py
+-rw-r--r--   0        0        0        0 2023-06-26 23:21:16.365884 lnauth_django-0.4.0/lnauth_django/migrations/__init__.py
+-rw-r--r--   0        0        0      266 2023-06-24 23:33:50.044247 lnauth_django-0.4.0/lnauth_django/models.py
+-rw-r--r--   0        0        0        0 2023-06-24 22:31:09.280965 lnauth_django-0.4.0/lnauth_django/tests/__init__.py
+-rw-r--r--   0        0        0     1522 2023-06-24 23:33:21.865177 lnauth_django-0.4.0/lnauth_django/tests/test_service.py
+-rw-r--r--   0        0        0      297 2023-06-24 22:33:44.897736 lnauth_django-0.4.0/lnauth_django/urls.py
+-rw-r--r--   0        0        0     2789 2023-07-18 12:14:32.704583 lnauth_django-0.4.0/lnauth_django/views.py
+-rw-r--r--   0        0        0      437 2023-07-18 12:15:33.233271 lnauth_django-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3274 1970-01-01 00:00:00.000000 lnauth_django-0.4.0/PKG-INFO
```

### Comparing `lnauth_django-0.3.0/README.md` & `lnauth_django-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -48,17 +48,17 @@
 
 - `LNURL_AUTH_ROOT_DOMAIN`: This is used to specify the domain for your app. By default, it should be the domain where your Django project is hosted. Required.
 
 - `LNURL_AUTH_K1_TIMEOUT`: This is used to specify the timeout of the `k1` challenge in seconds. By default, it is set to `60 * 60` seconds (1 hour).
 
 - `LNURL_AUTH_REGISTER_CALLBACK` and `LNURL_AUTH_LOGIN_CALLBACK`: This is used to specify the import path of the callback function to be executed after user registration / login. Both are optional.
 
-```
-LNURL_AUTH_REGISTER_CALLBACK = 'myapp.users.ln_auth.register_callback'
-```
+    ```python
+    LNURL_AUTH_REGISTER_CALLBACK = 'myapp.users.ln_auth.register_callback'
+    ```
 
 - `LNURL_AUTH_BACKEND`: This is used to specify the authentication backend that the library should use for login. Only needed if you're using multiple authentication backends.
 
 - `LNURL_AUTH_LOGIN_AFTER_REGISTER`: Specify whether to automatically log in the user after registration. Default is `True`.
 
 
 ## Usage
```

### Comparing `lnauth_django-0.3.0/lnauth_django/django_auth.py` & `lnauth_django-0.4.0/lnauth_django/django_auth.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,21 @@
+import random
 from importlib import import_module
 from logging import getLogger
 
 from django.conf import settings
-from django.contrib.auth import get_user_model, login
+from django.contrib.auth import (
+    BACKEND_SESSION_KEY,
+    HASH_SESSION_KEY,
+    SESSION_KEY,
+    get_user_model,
+)
+from django.contrib.sessions.backends.db import SessionStore
+from django.contrib.sessions.models import Session
+from django.core.cache import cache
 from django.db import IntegrityError, transaction
 
 from . import exceptions, models
 
 logger = getLogger(__name__)
 User = get_user_model()
 
@@ -19,16 +28,16 @@
     # Call the callback function
     callback_function(*args, **kwargs)
 
 
 def app_register(request):
     try:
         with transaction.atomic():
-
-            user = User.objects.create_user(username="LNURL User", password=None)
+            temp_username = f"lnauth_{random.randint(0, 1000000)}"
+            user = User.objects.create_user(username=temp_username, password=None)
             lnauthkey = models.LnAuthKey.objects.create(
                 user=user, linking_key=request.GET["key"]
             )
             lnauthkey.save()
             user.save()
     except IntegrityError as e:
         logger.info(e)
@@ -36,23 +45,55 @@
 
     callback_path = getattr(settings, "LNURL_AUTH_REGISTER_CALLBACK", False)
 
     if callback_path:
         _perform_callback(callback_path, request, user)
 
     if getattr(settings, "LNURL_AUTH_LOGIN_AFTER_REGISTER", True):
-        login(request, user, backend=getattr(settings, "LNURL_AUTH_BACKEND", None))
+        login_after_action(request.GET["k1"], user, request)
 
 
 def app_login(request):
     try:
         user = User.objects.get(lnauthkey__linking_key=request.GET["key"])
     except User.DoesNotExist as e:
         logger.info(e)
         raise exceptions.DjangoAuthException("User not registered.")
 
     callback_path = getattr(settings, "LNURL_AUTH_LOGIN_CALLBACK", False)
 
     if callback_path:
         _perform_callback(callback_path, request, user)
 
-    login(request, user, backend=getattr(settings, "LNURL_AUTH_BACKEND", None))
+    login_after_action(request.GET["k1"], user, request)
+
+
+def login_after_action(k1, user, request):
+
+    session_key = cache.get(f"lnauth-k1-{k1}:session_key")
+
+    cache.delete(f"lnauth-k1-{k1}:session_key")
+
+    try:
+        Session.objects.get(session_key=session_key)
+    except Session.DoesNotExist:
+        raise exceptions.DjangoAuthException("Session does not exist.")
+
+    # Update the session with the authenticated user's details
+    session_data = SessionStore(session_key=session_key)
+    session_data[SESSION_KEY] = user.pk
+    session_data[BACKEND_SESSION_KEY] = getattr(settings, "LNURL_AUTH_BACKEND", None)
+    session_data[HASH_SESSION_KEY] = user.get_session_auth_hash()
+
+    session_data.save()
+
+
+def create_and_save_session(k1: str, request):
+    timeout = getattr(settings, "LNURL_AUTH_K1_TIMEOUT", 60 * 60)
+    request.session["init"] = True
+    request.session.save()
+
+    cache.set(
+        f"lnauth-k1-{k1.hex()}:session_key",
+        request.session.session_key,
+        timeout=timeout,
+    )
```

### Comparing `lnauth_django-0.3.0/lnauth_django/lnauth.py` & `lnauth_django-0.4.0/lnauth_django/lnauth.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,44 +6,47 @@
 from django.core.cache import cache
 from django.urls import reverse
 from secp256k1 import PublicKey
 
 from . import exceptions
 
 
-def get_auth_url(action: str):
-    k1 = os.urandom(32)
+def generate_k1():
+    return os.urandom(32)
+
+
+def get_auth_url(k1: str, action: str):
     reverse_url = reverse("lnauth_django:ln_auth_url")
 
     cache.set(
-        f"lnauth-k1-{k1.hex()}",
+        f"lnauth-k1-{k1.hex()}:{action}",
         action,
         timeout=getattr(settings, "LNURL_AUTH_K1_TIMEOUT", 60 * 60),
     )
 
     url = f"{settings.LNURL_AUTH_ROOT_DOMAIN}{reverse_url}?tag=login&k1={k1.hex()}&action={action}"
 
     bech32_url = bech32.bech32_encode(
         "lnurl",
         bech32.convertbits(url.encode("utf-8"), 8, 5),
     )
 
     return bech32_url
 
 
-def verify_ln_auth(k1: str, sig: str, linking_key: str):
+def verify_ln_auth(k1: str, sig: str, linking_key: str, action: str):
 
     try:
         k1_bytes = binascii.unhexlify(k1)
         sig_bytes = binascii.unhexlify(sig)
         linking_key_bytes = binascii.unhexlify(linking_key)
     except binascii.Error:
         raise exceptions.LnAuthException("Invalid hex.")
 
-    if not cache.delete(f"lnauth-k1-{k1_bytes.hex()}"):
+    if not cache.delete(f"lnauth-k1-{k1_bytes.hex()}:{action}"):
         raise exceptions.LnAuthException("K1 does not exist.")
 
     linking_key_pubkey = PublicKey(linking_key_bytes, raw=True)
 
     sig_raw = linking_key_pubkey.ecdsa_deserialize(sig_bytes)
 
     if not linking_key_pubkey.ecdsa_verify(k1_bytes, sig_raw, raw=True):
```

### Comparing `lnauth_django-0.3.0/lnauth_django/migrations/0000_initial.py` & `lnauth_django-0.4.0/lnauth_django/migrations/0000_initial.py`

 * *Files identical despite different names*

### Comparing `lnauth_django-0.3.0/lnauth_django/tests/test_service.py` & `lnauth_django-0.4.0/lnauth_django/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `lnauth_django-0.3.0/lnauth_django/views.py` & `lnauth_django-0.4.0/lnauth_django/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,17 +10,21 @@
 
 class AuthURLProviderView(generic.View):
     def get(self, request):
         if not request.user.is_anonymous:
             return JsonResponse({"message": "User already authenticated."}, status=400)
 
         if request.GET and "action" in request.GET:
-            return JsonResponse(
-                {"url": lnauth.get_auth_url(request.GET["action"])}, status=200
-            )
+            action = request.GET["action"]
+            k1 = lnauth.generate_k1()
+
+            lnauth_url = lnauth.get_auth_url(k1, action)
+            django_auth.create_and_save_session(k1, request)
+
+            return JsonResponse({"url": lnauth_url}, status=200)
         else:
             return JsonResponse({"message": "Invalid request."}, status=400)
 
 
 class AuthURLView(generic.View):
     def get(self, request):
         if not request.user.is_anonymous:
@@ -39,15 +43,18 @@
             return JsonResponse(
                 {"status": "ERROR", "reason": "Invalid request. Invalid tag."},
                 status=400,
             )
 
         try:
             lnauth.verify_ln_auth(
-                request.GET["k1"], request.GET["sig"], request.GET["key"]
+                request.GET["k1"],
+                request.GET["sig"],
+                request.GET["key"],
+                request.GET["action"],
             )
         except exceptions.LnAuthException as e:
             return JsonResponse(
                 {"status": "ERROR", "reason": f"Invalid request. {e}"}, status=400
             )
 
         if request.GET["action"] == "login":
```

### Comparing `lnauth_django-0.3.0/PKG-INFO` & `lnauth_django-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnauth-django
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Author: zwx00
 Author-email: blaz@bolt.observer
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -65,17 +65,17 @@
 
 - `LNURL_AUTH_ROOT_DOMAIN`: This is used to specify the domain for your app. By default, it should be the domain where your Django project is hosted. Required.
 
 - `LNURL_AUTH_K1_TIMEOUT`: This is used to specify the timeout of the `k1` challenge in seconds. By default, it is set to `60 * 60` seconds (1 hour).
 
 - `LNURL_AUTH_REGISTER_CALLBACK` and `LNURL_AUTH_LOGIN_CALLBACK`: This is used to specify the import path of the callback function to be executed after user registration / login. Both are optional.
 
-```
-LNURL_AUTH_REGISTER_CALLBACK = 'myapp.users.ln_auth.register_callback'
-```
+    ```python
+    LNURL_AUTH_REGISTER_CALLBACK = 'myapp.users.ln_auth.register_callback'
+    ```
 
 - `LNURL_AUTH_BACKEND`: This is used to specify the authentication backend that the library should use for login. Only needed if you're using multiple authentication backends.
 
 - `LNURL_AUTH_LOGIN_AFTER_REGISTER`: Specify whether to automatically log in the user after registration. Default is `True`.
 
 
 ## Usage
```

