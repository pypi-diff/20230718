# Comparing `tmp/examon_beginners_package-0.0.7.tar.gz` & `tmp/examon_beginners_package-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "examon_beginners_package-0.0.7.tar", max compression
+gzip compressed data, was "examon_beginners_package-0.0.8.tar", max compression
```

## Comparing `examon_beginners_package-0.0.7.tar` & `examon_beginners_package-0.0.8.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       24 2023-07-16 20:33:56.622876 examon_beginners_package-0.0.7/examon_beginners_package/__init__.py
--rw-r--r--   0        0        0     1574 2023-07-18 20:18:25.770230 examon_beginners_package-0.0.7/examon_beginners_package/beginners.py
--rw-r--r--   0        0        0      338 2023-07-18 20:41:34.093501 examon_beginners_package-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 examon_beginners_package-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       24 2023-07-16 20:33:56.622876 examon_beginners_package-0.0.8/examon_beginners_package/__init__.py
+-rw-r--r--   0        0        0     1573 2023-07-18 20:43:28.888259 examon_beginners_package-0.0.8/examon_beginners_package/beginners.py
+-rw-r--r--   0        0        0      338 2023-07-18 20:43:58.512136 examon_beginners_package-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 examon_beginners_package-0.0.8/PKG-INFO
```

### Comparing `examon_beginners_package-0.0.7/examon_beginners_package/beginners.py` & `examon_beginners_package-0.0.8/examon_beginners_package/beginners.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,18 +46,18 @@
     [False, True],
     [True, False],
     [False, False],
 ], tags=['equality', 'dict', 'beginner'])
 def question():
     my_object = {'name': 'bob'}
     new_ref = my_object
-    return (
+    return [
         my_object is new_ref,
-        my_object is {'name': 'bob'},
-    )
+        my_object is {'name': 'bob'}
+    ]
 
 
 @examon_item(choices=[
     ['the', 'cat', 'in', 'the', 'hat'], []
 ], tags=['array', 'for', 'if', 'beginner'])
 def question():
     words = ['the', 'cat', 'in', 'the', 'hat']
```

