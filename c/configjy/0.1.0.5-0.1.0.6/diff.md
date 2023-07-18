# Comparing `tmp/configjy-0.1.0.5.tar.gz` & `tmp/configjy-0.1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configjy-0.1.0.5.tar", max compression
+gzip compressed data, was "configjy-0.1.0.6.tar", max compression
```

## Comparing `configjy-0.1.0.5.tar` & `configjy-0.1.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-03-02 12:32:21.093891 configjy-0.1.0.5/LICENSE
--rw-r--r--   0        0        0     1789 2023-03-02 12:32:21.093891 configjy-0.1.0.5/README.md
--rw-r--r--   0        0        0     2831 2023-03-02 12:32:21.093891 configjy-0.1.0.5/pyproject.toml
--rw-r--r--   0        0        0     7104 2023-03-02 12:32:21.093891 configjy-0.1.0.5/src/configjy/ConfigFile.py
--rw-r--r--   0        0        0       71 2023-03-02 12:32:21.093891 configjy-0.1.0.5/src/configjy/__init__.py
--rw-r--r--   0        0        0     2264 1970-01-01 00:00:00.000000 configjy-0.1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-18 17:19:10.570677 configjy-0.1.0.6/LICENSE
+-rw-r--r--   0        0        0     1789 2023-07-18 17:19:10.570677 configjy-0.1.0.6/README.md
+-rw-r--r--   0        0        0     2831 2023-07-18 17:19:10.570677 configjy-0.1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     7175 2023-07-18 17:19:10.570677 configjy-0.1.0.6/src/configjy/ConfigFile.py
+-rw-r--r--   0        0        0       71 2023-07-18 17:19:10.570677 configjy-0.1.0.6/src/configjy/__init__.py
+-rw-r--r--   0        0        0     2264 1970-01-01 00:00:00.000000 configjy-0.1.0.6/PKG-INFO
```

### Comparing `configjy-0.1.0.5/LICENSE` & `configjy-0.1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `configjy-0.1.0.5/README.md` & `configjy-0.1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `configjy-0.1.0.5/pyproject.toml` & `configjy-0.1.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configjy"
-version = "v0.1.0.5"
+version = "v0.1.0.6"
 description = "Loads a json or yaml config file"
 authors = ["henrique lino <henrique.lino97@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 "ruamel.yaml" = "^0.17.21"
```

### Comparing `configjy-0.1.0.5/src/configjy/ConfigFile.py` & `configjy-0.1.0.6/src/configjy/ConfigFile.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,18 +131,24 @@
         for key, value in config.items():
             value = self.__load(value, globals())
             value = self.__load(value, self.__dict__)
 
             self.loaded_vars[key] = value
 
             if self.print_when_create:
-                logger.critical(f"\n{'-'*60}\nVariavel criada:\nNome: '{key}'\nValor: '{json.dumps(value, indent = 4, default = str)}'\nTipo: '{type(value)}'\n{'-'*60}\n")
+                logger.debug(f"\n{'-'*60}\nVariavel criada:\nNome: '{key}'\nValor: '{json.dumps(value, indent = 4, default = str)}'\nTipo: '{type(value)}'\n{'-'*60}\n")
         return
 
-    def __init__(self, path: Union[str, Path], *, name="config", extensions=(".yaml", ".yml", ".json"), print_when_create=True):
+    def __init__(
+            self,
+            path: Union[str, Path],
+            *,
+            name="config",
+            extensions=(".yaml", ".yml", ".json"),
+            print_when_create=False):
         """Loads file content into a class
         If path to a file is given, uses the path, else searchs for name + extensions\n
         #### Usage:\n
         ---
         ```
         \n\n
         config_file = Path(__file__).parent.resolve()
```

### Comparing `configjy-0.1.0.5/PKG-INFO` & `configjy-0.1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configjy
-Version: 0.1.0.5
+Version: 0.1.0.6
 Summary: Loads a json or yaml config file
 Author: henrique lino
 Author-email: henrique.lino97@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

