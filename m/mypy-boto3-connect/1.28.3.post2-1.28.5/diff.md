# Comparing `tmp/mypy-boto3-connect-1.28.3.post2.tar.gz` & `tmp/mypy-boto3-connect-1.28.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-connect-1.28.3.post2.tar", last modified: Sat Jul 15 06:38:32 2023, max compression
+gzip compressed data, was "mypy-boto3-connect-1.28.5.tar", last modified: Tue Jul 18 19:32:41 2023, max compression
```

## Comparing `mypy-boto3-connect-1.28.3.post2.tar` & `mypy-boto3-connect-1.28.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:32.314243 mypy-boto3-connect-1.28.3.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-15 06:35:49.000000 mypy-boto3-connect-1.28.3.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    47783 2023-07-15 06:38:32.314243 mypy-boto3-connect-1.28.3.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    46292 2023-07-15 06:35:49.000000 mypy-boto3-connect-1.28.3.post2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:32.290242 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/
--rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-07-15 06:35:49.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-07-15 06:35:49.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-15 06:35:49.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   151314 2023-07-15 06:35:51.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   151066 2023-07-15 06:35:50.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25344 2023-07-15 06:35:52.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    25342 2023-07-15 06:35:52.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    54314 2023-07-15 06:35:51.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    54267 2023-07-15 06:35:51.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 06:35:49.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   230292 2023-07-15 06:35:59.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   229979 2023-07-15 06:35:55.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-15 06:35:49.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:32.310243 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    47783 2023-07-15 06:38:32.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-15 06:38:32.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:38:32.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:38:32.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-15 06:38:32.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-15 06:38:32.000000 mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 06:38:32.314243 mypy-boto3-connect-1.28.3.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-15 06:35:49.000000 mypy-boto3-connect-1.28.3.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.734719 mypy-boto3-connect-1.28.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 19:32:01.000000 mypy-boto3-connect-1.28.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    47777 2023-07-18 19:32:41.734719 mypy-boto3-connect-1.28.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    46292 2023-07-18 19:32:01.000000 mypy-boto3-connect-1.28.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.734719 mypy-boto3-connect-1.28.5/mypy_boto3_connect/
+-rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-07-18 19:32:01.000000 mypy-boto3-connect-1.28.5/mypy_boto3_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-07-18 19:32:01.000000 mypy-boto3-connect-1.28.5/mypy_boto3_connect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-18 19:32:01.000000 mypy-boto3-connect-1.28.5/mypy_boto3_connect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151314 2023-07-18 19:32:02.000000 mypy-boto3-connect-1.28.5/mypy_boto3_connect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151066 2023-07-18 19:32:02.000000 mypy-boto3-connect-1.28.5/mypy_boto3_connect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25344 2023-07-18 19:32:03.000000 mypy-boto3-connect-1.28.5/mypy_boto3_connect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25342 2023-07-18 19:32:03.000000 mypy-boto3-connect-1.28.5/mypy_boto3_connect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    54314 2023-07-18 19:32:03.000000 mypy-boto3-connect-1.28.5/mypy_boto3_connect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54267 2023-07-18 19:32:03.000000 mypy-boto3-connect-1.28.5/mypy_boto3_connect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:01.000000 mypy-boto3-connect-1.28.5/mypy_boto3_connect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   230292 2023-07-18 19:32:09.000000 mypy-boto3-connect-1.28.5/mypy_boto3_connect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   229979 2023-07-18 19:32:06.000000 mypy-boto3-connect-1.28.5/mypy_boto3_connect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 19:32:01.000000 mypy-boto3-connect-1.28.5/mypy_boto3_connect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.734719 mypy-boto3-connect-1.28.5/mypy_boto3_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    47777 2023-07-18 19:32:41.000000 mypy-boto3-connect-1.28.5/mypy_boto3_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-18 19:32:41.000000 mypy-boto3-connect-1.28.5/mypy_boto3_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-connect-1.28.5/mypy_boto3_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-connect-1.28.5/mypy_boto3_connect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 19:32:41.000000 mypy-boto3-connect-1.28.5/mypy_boto3_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-18 19:32:41.000000 mypy-boto3-connect-1.28.5/mypy_boto3_connect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:32:41.734719 mypy-boto3-connect-1.28.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-18 19:32:01.000000 mypy-boto3-connect-1.28.5/setup.py
```

### Comparing `mypy-boto3-connect-1.28.3.post2/LICENSE` & `mypy-boto3-connect-1.28.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.3.post2/PKG-INFO` & `mypy-boto3-connect-1.28.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connect
-Version: 1.28.3.post2
-Summary: Type annotations for boto3.Connect 1.28.3 service generated with mypy-boto3-builder 7.15.0
+Version: 1.28.5
+Summary: Type annotations for boto3.Connect 1.28.5 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connect.svg?color=blue)](https://pypi.org/project/mypy-boto3-connect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connect?color=blue)](https://pypistats.org/packages/mypy-boto3-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Connect 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
+[boto3.Connect 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-connect-1.28.3.post2/README.md` & `mypy-boto3-connect-1.28.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connect.svg?color=blue)](https://pypi.org/project/mypy-boto3-connect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connect?color=blue)](https://pypistats.org/packages/mypy-boto3-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Connect 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
+[boto3.Connect 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/__init__.py` & `mypy-boto3-connect-1.28.5/mypy_boto3_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/__init__.pyi` & `mypy-boto3-connect-1.28.5/mypy_boto3_connect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/__main__.py` & `mypy-boto3-connect-1.28.5/mypy_boto3_connect/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Connect 1.28.3\nVersion:         1.28.3.post2\nBuilder version:"
-        " 7.15.0\nDocs:           "
+        "Type annotations for boto3.Connect 1.28.5\nVersion:         1.28.5\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.3.post2")
+    print("1.28.5")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/client.py` & `mypy-boto3-connect-1.28.5/mypy_boto3_connect/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/client.pyi` & `mypy-boto3-connect-1.28.5/mypy_boto3_connect/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/literals.py` & `mypy-boto3-connect-1.28.5/mypy_boto3_connect/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/literals.pyi` & `mypy-boto3-connect-1.28.5/mypy_boto3_connect/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/paginator.py` & `mypy-boto3-connect-1.28.5/mypy_boto3_connect/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/paginator.pyi` & `mypy-boto3-connect-1.28.5/mypy_boto3_connect/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/type_defs.py` & `mypy-boto3-connect-1.28.5/mypy_boto3_connect/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect/type_defs.pyi` & `mypy-boto3-connect-1.28.5/mypy_boto3_connect/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect.egg-info/PKG-INFO` & `mypy-boto3-connect-1.28.5/mypy_boto3_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connect
-Version: 1.28.3.post2
-Summary: Type annotations for boto3.Connect 1.28.3 service generated with mypy-boto3-builder 7.15.0
+Version: 1.28.5
+Summary: Type annotations for boto3.Connect 1.28.5 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connect.svg?color=blue)](https://pypi.org/project/mypy-boto3-connect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connect?color=blue)](https://pypistats.org/packages/mypy-boto3-connect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Connect 1.28.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
+[boto3.Connect 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-connect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-connect-1.28.3.post2/mypy_boto3_connect.egg-info/SOURCES.txt` & `mypy-boto3-connect-1.28.5/mypy_boto3_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connect-1.28.3.post2/setup.py` & `mypy-boto3-connect-1.28.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-connect",
-    version="1.28.3.post2",
+    version="1.28.5",
     packages=["mypy_boto3_connect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Connect 1.28.3 service generated with mypy-boto3-builder 7.15.0"
+        "Type annotations for boto3.Connect 1.28.5 service generated with mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

