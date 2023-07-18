# Comparing `tmp/payload-api-0.4.5.tar.gz` & `tmp/payload-api-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payload-api-0.4.5.tar", last modified: Tue Jul 18 15:59:12 2023, max compression
+gzip compressed data, was "payload-api-0.4.6.tar", last modified: Tue Jul 18 16:01:41 2023, max compression
```

## Comparing `payload-api-0.4.5.tar` & `payload-api-0.4.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1089 2023-05-21 11:19:23.567686 payload-api-0.4.5/LICENSE
--rw-r--r--   0        0        0      673 2023-05-21 11:19:23.567686 payload-api-0.4.5/payload/__init__.py
--rw-r--r--   0        0        0      122 2023-05-21 11:19:23.567686 payload-api-0.4.5/payload/arm/__init__.py
--rw-r--r--   0        0        0     2104 2023-05-21 11:19:23.567686 payload-api-0.4.5/payload/arm/attr.py
--rw-r--r--   0        0        0     3930 2023-05-21 11:19:23.567686 payload-api-0.4.5/payload/arm/object.py
--rw-r--r--   0        0        0     7131 2023-07-17 21:59:24.811514 payload-api-0.4.5/payload/arm/request.py
--rw-r--r--   0        0        0      989 2023-05-21 11:19:23.567686 payload-api-0.4.5/payload/arm/session.py
--rw-r--r--   0        0        0     1282 2023-05-21 11:19:23.567686 payload-api-0.4.5/payload/exceptions.py
--rw-r--r--   0        0        0     2094 2023-05-21 11:19:23.567686 payload-api-0.4.5/payload/objects.py
--rw-r--r--   0        0        0     3418 2023-05-21 11:19:23.567686 payload-api-0.4.5/payload/utils.py
--rw-r--r--   0        0        0      546 2023-07-18 15:58:21.266975 payload-api-0.4.5/payload/version.py
--rw-r--r--   0        0        0      615 2023-07-18 15:58:33.910794 payload-api-0.4.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-21 11:19:23.567686 payload-api-0.4.5/tests/__init__.py
--rw-r--r--   0        0        0     4678 2023-07-17 21:59:24.811514 payload-api-0.4.5/tests/fixtures.py
--rw-r--r--   0        0        0     3250 2023-05-21 11:19:23.567686 payload-api-0.4.5/tests/test_account.py
--rw-r--r--   0        0        0     1419 2023-07-17 21:59:24.811514 payload-api-0.4.5/tests/test_billing.py
--rw-r--r--   0        0        0     1568 2023-07-17 21:59:24.811514 payload-api-0.4.5/tests/test_invoice.py
--rw-r--r--   0        0        0     1416 2023-07-17 21:59:24.811514 payload-api-0.4.5/tests/test_payment_link.py
--rw-r--r--   0        0        0     3446 2023-07-17 21:59:24.811514 payload-api-0.4.5/tests/test_payment_method.py
--rw-r--r--   0        0        0    27158 2023-07-17 21:59:24.811514 payload-api-0.4.5/tests/test_request.py
--rw-r--r--   0        0        0     3704 2023-05-21 11:19:23.567686 payload-api-0.4.5/tests/test_session.py
--rw-r--r--   0        0        0     1473 2023-05-21 11:19:23.567686 payload-api-0.4.5/tests/test_transaction.py
--rw-r--r--   0        0        0      166 1970-01-01 00:00:00.000000 payload-api-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-05-21 11:19:23.567686 payload-api-0.4.6/LICENSE
+-rw-r--r--   0        0        0      673 2023-05-21 11:19:23.567686 payload-api-0.4.6/payload/__init__.py
+-rw-r--r--   0        0        0      122 2023-05-21 11:19:23.567686 payload-api-0.4.6/payload/arm/__init__.py
+-rw-r--r--   0        0        0     2104 2023-05-21 11:19:23.567686 payload-api-0.4.6/payload/arm/attr.py
+-rw-r--r--   0        0        0     3930 2023-05-21 11:19:23.567686 payload-api-0.4.6/payload/arm/object.py
+-rw-r--r--   0        0        0     7131 2023-07-17 21:59:24.811514 payload-api-0.4.6/payload/arm/request.py
+-rw-r--r--   0        0        0      989 2023-05-21 11:19:23.567686 payload-api-0.4.6/payload/arm/session.py
+-rw-r--r--   0        0        0     1282 2023-05-21 11:19:23.567686 payload-api-0.4.6/payload/exceptions.py
+-rw-r--r--   0        0        0     2094 2023-05-21 11:19:23.567686 payload-api-0.4.6/payload/objects.py
+-rw-r--r--   0        0        0     3418 2023-05-21 11:19:23.567686 payload-api-0.4.6/payload/utils.py
+-rw-r--r--   0        0        0      495 2023-07-18 16:01:06.820588 payload-api-0.4.6/payload/version.py
+-rw-r--r--   0        0        0      615 2023-07-18 16:01:21.664373 payload-api-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-21 11:19:23.567686 payload-api-0.4.6/tests/__init__.py
+-rw-r--r--   0        0        0     4678 2023-07-17 21:59:24.811514 payload-api-0.4.6/tests/fixtures.py
+-rw-r--r--   0        0        0     3250 2023-05-21 11:19:23.567686 payload-api-0.4.6/tests/test_account.py
+-rw-r--r--   0        0        0     1419 2023-07-17 21:59:24.811514 payload-api-0.4.6/tests/test_billing.py
+-rw-r--r--   0        0        0     1568 2023-07-17 21:59:24.811514 payload-api-0.4.6/tests/test_invoice.py
+-rw-r--r--   0        0        0     1416 2023-07-17 21:59:24.811514 payload-api-0.4.6/tests/test_payment_link.py
+-rw-r--r--   0        0        0     3446 2023-07-17 21:59:24.811514 payload-api-0.4.6/tests/test_payment_method.py
+-rw-r--r--   0        0        0    27158 2023-07-17 21:59:24.811514 payload-api-0.4.6/tests/test_request.py
+-rw-r--r--   0        0        0     3704 2023-05-21 11:19:23.567686 payload-api-0.4.6/tests/test_session.py
+-rw-r--r--   0        0        0     1473 2023-05-21 11:19:23.567686 payload-api-0.4.6/tests/test_transaction.py
+-rw-r--r--   0        0        0      166 1970-01-01 00:00:00.000000 payload-api-0.4.6/PKG-INFO
```

### Comparing `payload-api-0.4.5/LICENSE` & `payload-api-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.5/payload/__init__.py` & `payload-api-0.4.6/payload/__init__.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.5/payload/arm/attr.py` & `payload-api-0.4.6/payload/arm/attr.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.5/payload/arm/object.py` & `payload-api-0.4.6/payload/arm/object.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.5/payload/arm/request.py` & `payload-api-0.4.6/payload/arm/request.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.5/payload/arm/session.py` & `payload-api-0.4.6/payload/arm/session.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.5/payload/exceptions.py` & `payload-api-0.4.6/payload/exceptions.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.5/payload/objects.py` & `payload-api-0.4.6/payload/objects.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.5/payload/utils.py` & `payload-api-0.4.6/payload/utils.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.5/pyproject.toml` & `payload-api-0.4.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "payload-api"
-version = "0.4.5"
+version = "0.4.6"
 description = "Payload Python Library"
 authors = [
     { name = "Ian Halpern", email = "ian@payload.co" },
 ]
 dependencies = [
     "requests",
     "six",
```

### Comparing `payload-api-0.4.5/tests/fixtures.py` & `payload-api-0.4.6/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.5/tests/test_account.py` & `payload-api-0.4.6/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.5/tests/test_billing.py` & `payload-api-0.4.6/tests/test_billing.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.5/tests/test_invoice.py` & `payload-api-0.4.6/tests/test_invoice.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.5/tests/test_payment_link.py` & `payload-api-0.4.6/tests/test_payment_link.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.5/tests/test_payment_method.py` & `payload-api-0.4.6/tests/test_payment_method.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.5/tests/test_request.py` & `payload-api-0.4.6/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.5/tests/test_session.py` & `payload-api-0.4.6/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.5/tests/test_transaction.py` & `payload-api-0.4.6/tests/test_transaction.py`

 * *Files identical despite different names*

