# Comparing `tmp/payload-api-0.4.3.tar.gz` & `tmp/payload-api-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payload-api-0.4.3.tar", last modified: Sat Aug 14 16:23:02 2021, max compression
+gzip compressed data, was "payload-api-0.4.4.tar", last modified: Mon Jul 17 22:22:24 2023, max compression
```

## Comparing `payload-api-0.4.3.tar` & `payload-api-0.4.4.tar`

### file list

```diff
@@ -1,34 +1,23 @@
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2021-08-14 16:23:02.403224 payload-api-0.4.3/
--rw-r--r--   0 ian       (1000) ian       (1000)     1089 2020-02-13 15:54:49.000000 payload-api-0.4.3/LICENSE
--rw-rw-r--   0 ian       (1000) ian       (1000)     4528 2021-08-14 16:23:02.403224 payload-api-0.4.3/PKG-INFO
--rw-rw-r--   0 ian       (1000) ian       (1000)     2458 2021-07-09 19:07:07.000000 payload-api-0.4.3/README.md
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2021-08-14 16:23:02.399224 payload-api-0.4.3/payload/
--rw-rw-r--   0 ian       (1000) ian       (1000)      673 2021-07-09 20:19:08.000000 payload-api-0.4.3/payload/__init__.py
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2021-08-14 16:23:02.403224 payload-api-0.4.3/payload/arm/
--rw-rw-r--   0 ian       (1000) ian       (1000)      122 2021-07-09 14:42:34.000000 payload-api-0.4.3/payload/arm/__init__.py
--rw-r--r--   0 ian       (1000) ian       (1000)     2104 2020-02-13 15:54:49.000000 payload-api-0.4.3/payload/arm/attr.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     3930 2021-07-09 14:42:34.000000 payload-api-0.4.3/payload/arm/object.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     7130 2021-08-14 16:22:06.000000 payload-api-0.4.3/payload/arm/request.py
--rw-rw-r--   0 ian       (1000) ian       (1000)      989 2021-07-09 20:19:32.000000 payload-api-0.4.3/payload/arm/session.py
--rw-r--r--   0 ian       (1000) ian       (1000)     1282 2020-09-06 16:12:56.000000 payload-api-0.4.3/payload/exceptions.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     2094 2021-06-02 23:16:37.000000 payload-api-0.4.3/payload/objects.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     3418 2021-07-09 14:42:34.000000 payload-api-0.4.3/payload/utils.py
--rw-rw-r--   0 ian       (1000) ian       (1000)       22 2021-08-14 16:22:25.000000 payload-api-0.4.3/payload/version.py
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2021-08-14 16:23:02.403224 payload-api-0.4.3/payload_api.egg-info/
--rw-r--r--   0 ian       (1000) ian       (1000)     4528 2021-08-14 16:23:02.000000 payload-api-0.4.3/payload_api.egg-info/PKG-INFO
--rw-r--r--   0 ian       (1000) ian       (1000)      615 2021-08-14 16:23:02.000000 payload-api-0.4.3/payload_api.egg-info/SOURCES.txt
--rw-r--r--   0 ian       (1000) ian       (1000)        1 2021-08-14 16:23:02.000000 payload-api-0.4.3/payload_api.egg-info/dependency_links.txt
--rw-r--r--   0 ian       (1000) ian       (1000)       13 2021-08-14 16:23:02.000000 payload-api-0.4.3/payload_api.egg-info/requires.txt
--rw-r--r--   0 ian       (1000) ian       (1000)       14 2021-08-14 16:23:02.000000 payload-api-0.4.3/payload_api.egg-info/top_level.txt
--rw-rw-r--   0 ian       (1000) ian       (1000)       38 2021-08-14 16:23:02.403224 payload-api-0.4.3/setup.cfg
--rw-r--r--   0 ian       (1000) ian       (1000)     1669 2020-02-13 15:54:49.000000 payload-api-0.4.3/setup.py
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2021-08-14 16:23:02.403224 payload-api-0.4.3/tests/
--rw-rw-r--   0 ian       (1000) ian       (1000)        0 2020-08-26 16:04:19.000000 payload-api-0.4.3/tests/__init__.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     3287 2021-07-09 14:42:34.000000 payload-api-0.4.3/tests/fixtures.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     3250 2021-07-09 14:42:34.000000 payload-api-0.4.3/tests/test_account.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     1162 2020-08-26 16:04:19.000000 payload-api-0.4.3/tests/test_billing.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     1364 2021-07-09 14:42:34.000000 payload-api-0.4.3/tests/test_invoice.py
--rw-rw-r--   0 ian       (1000) ian       (1000)      443 2020-08-26 16:04:19.000000 payload-api-0.4.3/tests/test_payment_link.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     3429 2021-07-09 14:42:34.000000 payload-api-0.4.3/tests/test_payment_method.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     3704 2021-07-09 14:42:34.000000 payload-api-0.4.3/tests/test_session.py
--rw-rw-r--   0 ian       (1000) ian       (1000)     1473 2021-07-09 14:42:34.000000 payload-api-0.4.3/tests/test_transaction.py
+-rw-r--r--   0        0        0     1089 2023-05-21 11:19:23.567686 payload-api-0.4.4/LICENSE
+-rw-r--r--   0        0        0      673 2023-05-21 11:19:23.567686 payload-api-0.4.4/payload/__init__.py
+-rw-r--r--   0        0        0      122 2023-05-21 11:19:23.567686 payload-api-0.4.4/payload/arm/__init__.py
+-rw-r--r--   0        0        0     2104 2023-05-21 11:19:23.567686 payload-api-0.4.4/payload/arm/attr.py
+-rw-r--r--   0        0        0     3930 2023-05-21 11:19:23.567686 payload-api-0.4.4/payload/arm/object.py
+-rw-r--r--   0        0        0     7131 2023-07-17 21:59:24.811514 payload-api-0.4.4/payload/arm/request.py
+-rw-r--r--   0        0        0      989 2023-05-21 11:19:23.567686 payload-api-0.4.4/payload/arm/session.py
+-rw-r--r--   0        0        0     1282 2023-05-21 11:19:23.567686 payload-api-0.4.4/payload/exceptions.py
+-rw-r--r--   0        0        0     2094 2023-05-21 11:19:23.567686 payload-api-0.4.4/payload/objects.py
+-rw-r--r--   0        0        0     3418 2023-05-21 11:19:23.567686 payload-api-0.4.4/payload/utils.py
+-rw-r--r--   0        0        0      531 2023-07-17 22:20:49.470374 payload-api-0.4.4/payload/version.py
+-rw-r--r--   0        0        0      615 2023-07-17 22:21:26.354105 payload-api-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-21 11:19:23.567686 payload-api-0.4.4/tests/__init__.py
+-rw-r--r--   0        0        0     4678 2023-07-17 21:59:24.811514 payload-api-0.4.4/tests/fixtures.py
+-rw-r--r--   0        0        0     3250 2023-05-21 11:19:23.567686 payload-api-0.4.4/tests/test_account.py
+-rw-r--r--   0        0        0     1419 2023-07-17 21:59:24.811514 payload-api-0.4.4/tests/test_billing.py
+-rw-r--r--   0        0        0     1568 2023-07-17 21:59:24.811514 payload-api-0.4.4/tests/test_invoice.py
+-rw-r--r--   0        0        0     1416 2023-07-17 21:59:24.811514 payload-api-0.4.4/tests/test_payment_link.py
+-rw-r--r--   0        0        0     3446 2023-07-17 21:59:24.811514 payload-api-0.4.4/tests/test_payment_method.py
+-rw-r--r--   0        0        0    27158 2023-07-17 21:59:24.811514 payload-api-0.4.4/tests/test_request.py
+-rw-r--r--   0        0        0     3704 2023-05-21 11:19:23.567686 payload-api-0.4.4/tests/test_session.py
+-rw-r--r--   0        0        0     1473 2023-05-21 11:19:23.567686 payload-api-0.4.4/tests/test_transaction.py
+-rw-r--r--   0        0        0      166 1970-01-01 00:00:00.000000 payload-api-0.4.4/PKG-INFO
```

### Comparing `payload-api-0.4.3/LICENSE` & `payload-api-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.3/payload/__init__.py` & `payload-api-0.4.4/payload/__init__.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.3/payload/arm/attr.py` & `payload-api-0.4.4/payload/arm/attr.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.3/payload/arm/object.py` & `payload-api-0.4.4/payload/arm/object.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.3/payload/arm/request.py` & `payload-api-0.4.4/payload/arm/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,28 +135,28 @@
 
     def delete(self, objects=None):
         if isinstance( objects, list ):
             if not objects:
                 raise ValueError('List must not be empty')
             for o in objects:
                 if not isinstance( o, ARMObject ):
-                    raise TypeError('Bulk create requires ARMObject object types')
+                    raise TypeError('Bulk delete requires ARMObject object types')
                 if not self.Object:
                     self.Object = o.__class__
                 elif not isinstance( o, self.Object ):
-                    raise TypeError('Bulk create requires all objects to be of the same type')
+                    raise TypeError('Bulk delete requires all objects to be of the same type')
             delete_query = '|'.join([ obj.id for obj in objects ])
             return self._request('delete', params={'id': delete_query, 'mode': 'query'})
         elif isinstance( objects, ARMObject ):
             self.Object = objects.__class__
-            return cls._request('delete', id=objects.id)
+            return self._request('delete', id=objects.id)
         elif objects is None and self.Object and self._filters:
             return self._request('delete', params={'mode':'query'})
         else:
-            raise TypeError('Bulk create requires ARMObject object types')
+            raise TypeError('Bulk delete requires ARMObject object types')
 
     def update(self, objects=None, **values):
         if objects:
             if not isinstance( objects, list ):
                 raise ValueError('first parameter must be a list of updates')
             if not objects or not isinstance( objects[0], (list, tuple) ):
                 raise ValueError('first parameter must be a list of updates')
```

### Comparing `payload-api-0.4.3/payload/arm/session.py` & `payload-api-0.4.4/payload/arm/session.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.3/payload/exceptions.py` & `payload-api-0.4.4/payload/exceptions.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.3/payload/objects.py` & `payload-api-0.4.4/payload/objects.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.3/payload/utils.py` & `payload-api-0.4.4/payload/utils.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.3/tests/test_account.py` & `payload-api-0.4.4/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.3/tests/test_billing.py` & `payload-api-0.4.4/tests/test_billing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 
 import payload as pl
 
 from .fixtures import Fixtures
+from payload.exceptions import NotFound
 
 
 @pytest.fixture()
 def billing_schedule(processing_account, customer_account):
     billing_schedule = pl.BillingSchedule.create(
         start_date="2019-01-01",
         end_date="2019-12-31",
@@ -32,7 +33,12 @@
     ):
         assert billing_schedule.processing_id == processing_account.id
         assert billing_schedule.charges[0].amount == 39.99
 
         billing_schedule.update(recurring_frequency="quarterly")
 
         assert billing_schedule.recurring_frequency == "quarterly"
+
+    def test_delete_billing_schedule(self, billing_schedule):
+        with pytest.raises(NotFound):
+            billing_schedule.delete()
+            billing_schedule_get = pl.BillingSchedule.get(billing_schedule.id)
```

### Comparing `payload-api-0.4.3/tests/test_invoice.py` & `payload-api-0.4.4/tests/test_invoice.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import datetime
 
 import pytest
 
 import payload as pl
 
 from .fixtures import Fixtures
+from payload.exceptions import NotFound
+
 
 
 @pytest.fixture
 def invoice(processing_account, customer_account):
     invoice = pl.Invoice.create(
         type="bill",
         processing_id=processing_account.id,
@@ -17,29 +19,34 @@
         items=[pl.ChargeItem(amount=29.99)],
     )
 
     return invoice
 
 
 class TestInvoice(Fixtures):
-    def test_create_invoice(self, api_key, invoice):
+    def test_create_invoice(self, invoice):
         assert invoice.due_date == datetime.datetime.today().strftime('%Y-%m-%d')
         assert invoice.status == "unpaid"
 
-    def test_pay_invoice(self, api_key, invoice, customer_account):
+    def test_pay_invoice(self, invoice, customer_account):
         assert invoice.due_date == datetime.datetime.today().strftime('%Y-%m-%d')
         assert invoice.status == "unpaid"
 
         card_payment = pl.Card.create(
-            account_id=customer_account.id, card_number="4242 4242 4242 4242", expiry='12/25'
+            account_id=customer_account.id, card_number="4242 4242 4242 4242", expiry='12/35', card_code='123'
         )
 
         if invoice.status != "paid":
             pl.Payment.create(
                 amount=invoice.amount_due,
                 customer_id=customer_account.id,
                 payment_method_id=card_payment.id,
                 allocations=[pl.PaymentItem(invoice_id=invoice.id)],
             )
 
         get_invoice = pl.Invoice.get(invoice.id)
         assert get_invoice.status == "paid"
+
+    def test_delete_invoice(self, invoice):
+        with pytest.raises(NotFound):
+            invoice.delete()
+            invoice_get = pl.Invoice.get(invoice.id)
```

### Comparing `payload-api-0.4.3/tests/test_payment_method.py` & `payload-api-0.4.4/tests/test_payment_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         rand_description = "".join(random.choice(letters) for i in range(10))
 
         card_payment = pl.Payment.create(
             amount=100.0,
             description=rand_description,
             processing_id=processing_account.id,
             payment_method=pl.Card(
-                card_number="4242 4242 4242 4242", expiry="05/22", card_code="123"
+                card_number="4242 4242 4242 4242", expiry="05/35", card_code="123"
             ),
         )
 
         payments = pl.Payment.filter_by(
             pl.attr.amount > 99,
             pl.attr.amount < (200),
             pl.attr.description.contains(rand_description),
@@ -69,15 +69,15 @@
         assert refund.amount == 10
         assert refund.status_code == "approved"
 
     def test_blind_refund_card_payment(self, api_key, processing_account):
         refund = pl.Refund.create(
             amount=10,
             processing_id=processing_account.id,
-            payment_method=pl.Card(card_number="4242 4242 4242 4242", expiry="12/25"),
+            payment_method=pl.Card(card_number="4242 4242 4242 4242", expiry="12/25", card_code='123'),
         )
 
         assert refund.type == "refund"
         assert refund.amount == 10
         assert refund.status_code == "approved"
 
     def test_refund_bank_payment(self, api_key, bank_payment):
```

### Comparing `payload-api-0.4.3/tests/test_session.py` & `payload-api-0.4.4/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.3/tests/test_transaction.py` & `payload-api-0.4.4/tests/test_transaction.py`

 * *Files identical despite different names*

