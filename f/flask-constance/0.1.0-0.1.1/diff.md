# Comparing `tmp/flask_constance-0.1.0.tar.gz` & `tmp/flask_constance-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_constance-0.1.0.tar", max compression
+gzip compressed data, was "flask_constance-0.1.1.tar", max compression
```

## Comparing `flask_constance-0.1.0.tar` & `flask_constance-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0     1074 2023-04-06 21:12:46.149054 flask_constance-0.1.0/LICENSE
--rw-r--r--   0        0        0       74 2023-04-07 02:21:03.779281 flask_constance-0.1.0/flask_constance/__init__.py
--rw-r--r--   0        0        0       45 2023-04-08 22:02:20.400431 flask_constance-0.1.0/flask_constance/admin/__init__.py
--rw-r--r--   0        0        0      891 2023-04-10 00:04:27.365898 flask_constance-0.1.0/flask_constance/admin/form.py
--rw-r--r--   0        0        0     1760 2023-04-09 19:45:32.742322 flask_constance-0.1.0/flask_constance/admin/templates/settings.html.j2
--rw-r--r--   0        0        0     2927 2023-04-09 23:55:49.485902 flask_constance-0.1.0/flask_constance/admin/view.py
--rw-r--r--   0        0        0      137 2023-04-06 22:16:26.219101 flask_constance-0.1.0/flask_constance/backends/__init__.py
--rw-r--r--   0        0        0      440 2023-04-07 00:28:06.619198 flask_constance-0.1.0/flask_constance/backends/base.py
--rw-r--r--   0        0        0     1941 2023-04-29 01:33:44.335698 flask_constance-0.1.0/flask_constance/backends/fsqla.py
--rw-r--r--   0        0        0     1032 2023-04-09 23:59:39.775900 flask_constance-0.1.0/flask_constance/backends/memory.py
--rw-r--r--   0        0        0     1880 2023-04-10 00:04:09.645898 flask_constance-0.1.0/flask_constance/cli.py
--rw-r--r--   0        0        0     2609 2023-04-09 16:18:17.472246 flask_constance-0.1.0/flask_constance/core.py
--rw-r--r--   0        0        0      685 2023-04-06 23:57:45.669176 flask_constance-0.1.0/flask_constance/globals.py
--rw-r--r--   0        0        0        0 2023-04-09 23:58:48.425901 flask_constance-0.1.0/flask_constance/py.typed
--rw-r--r--   0        0        0      826 2023-04-11 04:25:56.561849 flask_constance-0.1.0/flask_constance/signals.py
--rw-r--r--   0        0        0     3705 2023-04-09 16:32:38.632251 flask_constance-0.1.0/flask_constance/storage.py
--rw-r--r--   0        0        0      949 2023-04-10 00:06:13.735897 flask_constance-0.1.0/flask_constance/view.py
--rw-r--r--   0        0        0     2861 2023-04-10 00:03:40.505898 flask_constance-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      965 1970-01-01 00:00:00.000000 flask_constance-0.1.0/setup.py
--rw-r--r--   0        0        0     1418 1970-01-01 00:00:00.000000 flask_constance-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-10 13:58:01.870714 flask_constance-0.1.1/LICENSE
+-rw-r--r--   0        0        0       74 2023-04-10 13:58:01.870714 flask_constance-0.1.1/flask_constance/__init__.py
+-rw-r--r--   0        0        0       45 2023-04-10 13:58:01.870714 flask_constance-0.1.1/flask_constance/admin/__init__.py
+-rw-r--r--   0        0        0      891 2023-04-10 13:58:01.870714 flask_constance-0.1.1/flask_constance/admin/form.py
+-rw-r--r--   0        0        0     1760 2023-04-10 13:58:01.870714 flask_constance-0.1.1/flask_constance/admin/templates/settings.html.j2
+-rw-r--r--   0        0        0     2927 2023-04-10 13:58:01.870714 flask_constance-0.1.1/flask_constance/admin/view.py
+-rw-r--r--   0        0        0      137 2023-04-10 13:58:01.870714 flask_constance-0.1.1/flask_constance/backends/__init__.py
+-rw-r--r--   0        0        0      440 2023-04-10 13:58:01.870714 flask_constance-0.1.1/flask_constance/backends/base.py
+-rw-r--r--   0        0        0     1941 2023-04-10 13:58:01.870714 flask_constance-0.1.1/flask_constance/backends/fsqla.py
+-rw-r--r--   0        0        0     1032 2023-04-10 13:58:01.870714 flask_constance-0.1.1/flask_constance/backends/memory.py
+-rw-r--r--   0        0        0     1880 2023-04-10 13:58:01.870714 flask_constance-0.1.1/flask_constance/cli.py
+-rw-r--r--   0        0        0     2609 2023-04-10 13:58:01.870714 flask_constance-0.1.1/flask_constance/core.py
+-rw-r--r--   0        0        0      685 2023-04-10 13:58:01.870714 flask_constance-0.1.1/flask_constance/globals.py
+-rw-r--r--   0        0        0        0 2023-04-10 13:58:01.870714 flask_constance-0.1.1/flask_constance/py.typed
+-rw-r--r--   0        0        0      886 2023-07-18 02:34:18.543642 flask_constance-0.1.1/flask_constance/signals.py
+-rw-r--r--   0        0        0     3705 2023-04-10 13:58:01.870714 flask_constance-0.1.1/flask_constance/storage.py
+-rw-r--r--   0        0        0      949 2023-04-10 13:58:01.870714 flask_constance-0.1.1/flask_constance/view.py
+-rw-r--r--   0        0        0     2897 2023-07-18 02:25:01.088272 flask_constance-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1416 1970-01-01 00:00:00.000000 flask_constance-0.1.1/PKG-INFO
```

### Comparing `flask_constance-0.1.0/LICENSE` & `flask_constance-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_constance-0.1.0/flask_constance/admin/form.py` & `flask_constance-0.1.1/flask_constance/admin/form.py`

 * *Files identical despite different names*

### Comparing `flask_constance-0.1.0/flask_constance/admin/templates/settings.html.j2` & `flask_constance-0.1.1/flask_constance/admin/templates/settings.html.j2`

 * *Files identical despite different names*

### Comparing `flask_constance-0.1.0/flask_constance/admin/view.py` & `flask_constance-0.1.1/flask_constance/admin/view.py`

 * *Files identical despite different names*

### Comparing `flask_constance-0.1.0/flask_constance/backends/fsqla.py` & `flask_constance-0.1.1/flask_constance/backends/fsqla.py`

 * *Files identical despite different names*

### Comparing `flask_constance-0.1.0/flask_constance/backends/memory.py` & `flask_constance-0.1.1/flask_constance/backends/memory.py`

 * *Files identical despite different names*

### Comparing `flask_constance-0.1.0/flask_constance/cli.py` & `flask_constance-0.1.1/flask_constance/cli.py`

 * *Files identical despite different names*

### Comparing `flask_constance-0.1.0/flask_constance/core.py` & `flask_constance-0.1.1/flask_constance/core.py`

 * *Files identical despite different names*

### Comparing `flask_constance-0.1.0/flask_constance/globals.py` & `flask_constance-0.1.1/flask_constance/globals.py`

 * *Files identical despite different names*

### Comparing `flask_constance-0.1.0/flask_constance/signals.py` & `flask_constance-0.1.1/flask_constance/signals.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 try:
-    from blinker import Namespace  # type: ignore[import]
+    from blinker import Namespace
 
     signals = Namespace()
 
     #: Signal called after extension was initialized.
     constance_setup = signals.signal("constance-setup")
     #: Signal called after setting value was accessed.
     constance_get = signals.signal("constance-get")
@@ -17,10 +17,10 @@
 
         def __repr__(self) -> str:
             return f"<MockedSignal {self.name}>"
 
         def send(self, *args, **kwargs):
             pass
 
-    constance_setup = MockedSignal("constance-setup")
-    constance_get = MockedSignal("constance-get")
-    constance_set = MockedSignal("constance-set")
+    constance_setup = MockedSignal("constance-setup")  # type: ignore[assignment]
+    constance_get = MockedSignal("constance-get")  # type: ignore[assignment]
+    constance_set = MockedSignal("constance-set")  # type: ignore[assignment]
```

### Comparing `flask_constance-0.1.0/flask_constance/storage.py` & `flask_constance-0.1.1/flask_constance/storage.py`

 * *Files identical despite different names*

### Comparing `flask_constance-0.1.0/flask_constance/view.py` & `flask_constance-0.1.1/flask_constance/view.py`

 * *Files identical despite different names*

### Comparing `flask_constance-0.1.0/pyproject.toml` & `flask_constance-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Flask-Constance"
-version = "0.1.0"
+version = "0.1.1"
 description = "Dynamic settings for Flask applications"
 authors = ["Ivan Fedorov <inbox@titaniumhocker.ru>"]
 license = "MIT"
 repository = "https://github.com/TitaniumHocker/Flask-Constance"
 documentation = "https://flask-constance.rtfd.io"
 keywords = ["flask", "extension"]
 classifiers = [
@@ -19,20 +19,20 @@
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/TitaniumHocker/Flask-Constance/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
-Flask = "^2.0.1"
-Flask-SQLAlchemy = {version = "^2.5.1", extras = ["fsqla"]}
+Flask = ">=2.0.1,<3.0"
+Flask-SQLAlchemy = {version = ">=2.5.1,<3.0.0", extras = ["fsqla"]}
 SQLAlchemy = {version = ">1.4,<2.0", extras = ["fsqla"]}
-Flask-Admin = {version = "^1.6.1", extras = ["admin"]}
-Flask-WTF = {version = "^1.1.1", extras = ["admin"]}
-blinker = {version = "^1.6", extras = ["signals"]}
+Flask-Admin = {version = ">=1.6.1,<2.0.0", extras = ["admin"]}
+Flask-WTF = {version = ">=1.1.1,<2.0.0", extras = ["admin"]}
+blinker = {version = ">=1.6,<2.0", extras = ["signals"]}
 
 [tool.poetry.group.dev.dependencies]
 mypy = "<=1.1.1"
 pytest = "^6.2.4"
 coverage = {extras = ["toml"], version = "^5.5"}
 pytest-cov = "^2.12.1"
 flake8 = "<5.0.0"
```

### Comparing `flask_constance-0.1.0/PKG-INFO` & `flask_constance-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-constance
-Version: 0.1.0
+Version: 0.1.1
 Summary: Dynamic settings for Flask applications
 Home-page: https://github.com/TitaniumHocker/Flask-Constance
 License: MIT
 Keywords: flask,extension
 Author: Ivan Fedorov
 Author-email: inbox@titaniumhocker.ru
 Requires-Python: >=3.8,<4.0
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: Flask (>=2.0.1,<3.0.0)
+Requires-Dist: Flask (>=2.0.1,<3.0)
 Requires-Dist: Flask-Admin[admin] (>=1.6.1,<2.0.0)
 Requires-Dist: Flask-SQLAlchemy[fsqla] (>=2.5.1,<3.0.0)
 Requires-Dist: Flask-WTF[admin] (>=1.1.1,<2.0.0)
 Requires-Dist: SQLAlchemy[fsqla] (>1.4,<2.0)
 Requires-Dist: blinker[signals] (>=1.6,<2.0)
 Project-URL: Bug Tracker, https://github.com/TitaniumHocker/Flask-Constance/issues
 Project-URL: Documentation, https://flask-constance.rtfd.io
```

