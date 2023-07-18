# Comparing `tmp/zdatabase-0.5.5.tar.gz` & `tmp/zdatabase-0.5.6.tar.gz`

## Comparing `zdatabase-0.5.5.tar` & `zdatabase-0.5.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 zdatabase-0.5.5/src/zdatabase/__init__.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 zdatabase-0.5.5/src/zdatabase/model.py
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 zdatabase-0.5.5/src/zdatabase/utility.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 zdatabase-0.5.5/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zdatabase-0.5.5/LICENSE
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 zdatabase-0.5.5/README.md
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 zdatabase-0.5.5/pyproject.toml
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 zdatabase-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 zdatabase-0.5.6/src/zdatabase/__init__.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 zdatabase-0.5.6/src/zdatabase/model.py
+-rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 zdatabase-0.5.6/src/zdatabase/utility.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 zdatabase-0.5.6/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zdatabase-0.5.6/LICENSE
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 zdatabase-0.5.6/README.md
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 zdatabase-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 zdatabase-0.5.6/PKG-INFO
```

### Comparing `zdatabase-0.5.5/src/zdatabase/__init__.py` & `zdatabase-0.5.6/src/zdatabase/__init__.py`

 * *Files identical despite different names*

### Comparing `zdatabase-0.5.5/src/zdatabase/model.py` & `zdatabase-0.5.6/src/zdatabase/model.py`

 * *Files identical despite different names*

### Comparing `zdatabase-0.5.5/src/zdatabase/utility.py` & `zdatabase-0.5.6/src/zdatabase/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,20 +81,15 @@
 class MapperUtility:
     @staticmethod
     def jsonlize(items):
         return [item.to_json() for item in items]
 
     @classmethod
     def make_flts(cls, **kwargs):
-        flts = []
-        kwargs.pop('page_size', None)
-        kwargs.pop('page_num', None)
-        for k, v in kwargs.items():
-            flts += [getattr(cls, k) == v]
-        return flts
+        return [getattr(cls, k) == v for k, v in kwargs.items()]
 
     @classmethod
     def make_query(cls, **kwargs):
         flts = cls.make_flts(**kwargs)
         return cls.filter(*flts)
 
     @classmethod
@@ -143,25 +138,24 @@
 
     @classmethod
     def get_list_(cls, **kwargs):
         return cls.make_query(**kwargs).all()
 
     @classmethod
     def get_list(cls, **kwargs):
-        items = cls.get_list_(**kwargs)
-        return cls.jsonlize(items)
-
-    @classmethod
-    def get_page(cls, **kwargs):
-        pagination = {
-            'page_size': kwargs.pop('page_size', 20),
-            'page_num': kwargs.pop('page_num', 1)
-        }
-        query = cls.make_query(**kwargs)
-        return cls.paginate(query, pagination)
+        if 'page_num' in kwargs:
+            pagination = {
+                'page_size': kwargs.pop('page_size', 20),
+                'page_num': kwargs.pop('page_num', 1)
+            }
+            query = cls.make_query(**kwargs)
+            return cls.paginate(query, pagination)
+        else:
+            items = cls.get_list_(**kwargs)
+            return cls.jsonlize(items)
 
     @classmethod
     def get_all_(cls):
         return cls.filter().all()
 
     @classmethod
     def get_all(cls):
```

### Comparing `zdatabase-0.5.5/LICENSE` & `zdatabase-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `zdatabase-0.5.5/pyproject.toml` & `zdatabase-0.5.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zdatabase"
-version = "0.5.5"
+version = "0.5.6"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "zen database library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `zdatabase-0.5.5/PKG-INFO` & `zdatabase-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zdatabase
-Version: 0.5.5
+Version: 0.5.6
 Summary: zen database library
 Project-URL: Homepage, https://github.com/inspirare6/zdatabase
 Project-URL: Bug Tracker, https://github.com/inspirare6/zdatabase/issues
 Author-email: inspirare6 <inspirare6@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

