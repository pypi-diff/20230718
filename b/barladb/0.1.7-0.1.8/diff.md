# Comparing `tmp/barladb-0.1.7.tar.gz` & `tmp/barladb-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barladb-0.1.7.tar", last modified: Mon Jul 17 12:14:55 2023, max compression
+gzip compressed data, was "barladb-0.1.8.tar", last modified: Tue Jul 18 06:26:50 2023, max compression
```

## Comparing `barladb-0.1.7.tar` & `barladb-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 12:14:55.624768 barladb-0.1.7/
--rw-rw-rw-   0        0        0     3456 2023-07-17 12:14:55.624768 barladb-0.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-17 12:14:55.619618 barladb-0.1.7/barladb/
--rw-rw-rw-   0        0        0     1085 2023-07-17 11:56:23.000000 barladb-0.1.7/barladb/classes.py
--rw-rw-rw-   0        0        0       13 2023-07-15 10:58:22.000000 barladb-0.1.7/barladb/config.py
--rw-rw-rw-   0        0        0     4307 2023-07-17 11:58:32.000000 barladb-0.1.7/barladb/db.py
-drwxrwxrwx   0        0        0        0 2023-07-17 12:14:55.623746 barladb-0.1.7/barladb.egg-info/
--rw-rw-rw-   0        0        0     3456 2023-07-17 12:14:55.000000 barladb-0.1.7/barladb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-07-17 12:14:55.000000 barladb-0.1.7/barladb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 12:14:55.000000 barladb-0.1.7/barladb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-17 12:14:55.000000 barladb-0.1.7/barladb.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-07-17 12:14:55.000000 barladb-0.1.7/barladb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 12:14:55.624768 barladb-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     3618 2023-07-17 12:14:09.000000 barladb-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 06:26:50.593745 barladb-0.1.8/
+-rw-rw-rw-   0        0        0     3419 2023-07-18 06:26:50.593745 barladb-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3027 2023-07-18 06:20:29.000000 barladb-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 06:26:50.593745 barladb-0.1.8/barladb/
+-rw-rw-rw-   0        0        0     1085 2023-07-17 11:56:23.000000 barladb-0.1.8/barladb/classes.py
+-rw-rw-rw-   0        0        0       13 2023-07-15 10:58:22.000000 barladb-0.1.8/barladb/config.py
+-rw-rw-rw-   0        0        0     4307 2023-07-17 11:58:32.000000 barladb-0.1.8/barladb/db.py
+drwxrwxrwx   0        0        0        0 2023-07-18 06:26:50.593745 barladb-0.1.8/barladb.egg-info/
+-rw-rw-rw-   0        0        0     3419 2023-07-18 06:26:50.000000 barladb-0.1.8/barladb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-07-18 06:26:50.000000 barladb-0.1.8/barladb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 06:26:50.000000 barladb-0.1.8/barladb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-18 06:26:50.000000 barladb-0.1.8/barladb.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-07-18 06:26:50.000000 barladb-0.1.8/barladb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 06:26:50.593745 barladb-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     3581 2023-07-18 06:25:29.000000 barladb-0.1.8/setup.py
```

### Comparing `barladb-0.1.7/PKG-INFO` & `barladb-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: barladb
-Version: 0.1.7
+Version: 0.1.8
 Summary: A very easy local database based on JSON
-Home-page: https://sites.google.com/view/barladb/
+Home-page: https://github.com/barlin41k/barladb
 Author: barlin41k
 Author-email: sasaigrypocta@gmail.com
 Project-URL: Documentation, https://sites.google.com/view/barladb/
+Project-URL: GitHub, https://github.com/barlin41k/barladb
 Description-Content-Type: text/markdown
 
 
 # Изменения:
-- Добавлены новые функции и документация - https://sites.google.com/view/barladb/
-```python
-db.remove_column(filepath, key)
-db.columns(filepath)
-```
+- Добавлен репозиторий на GitHub - https://github.com/barlin41k/barladb
 
 
 # Что такое barlaDB?
 - `barlaDB` - это легкая, простая библиотека для небольших проектов на `Python`, которая имеет очень лёгкий интерфейс. С ней смогут познакомиться даже чайники в `Python`!
 
 # Лёгкий пример использования
 ```python
```

### Comparing `barladb-0.1.7/barladb/classes.py` & `barladb-0.1.8/barladb/classes.py`

 * *Files identical despite different names*

### Comparing `barladb-0.1.7/barladb/db.py` & `barladb-0.1.8/barladb/db.py`

 * *Files identical despite different names*

### Comparing `barladb-0.1.7/barladb.egg-info/PKG-INFO` & `barladb-0.1.8/barladb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: barladb
-Version: 0.1.7
+Version: 0.1.8
 Summary: A very easy local database based on JSON
-Home-page: https://sites.google.com/view/barladb/
+Home-page: https://github.com/barlin41k/barladb
 Author: barlin41k
 Author-email: sasaigrypocta@gmail.com
 Project-URL: Documentation, https://sites.google.com/view/barladb/
+Project-URL: GitHub, https://github.com/barlin41k/barladb
 Description-Content-Type: text/markdown
 
 
 # Изменения:
-- Добавлены новые функции и документация - https://sites.google.com/view/barladb/
-```python
-db.remove_column(filepath, key)
-db.columns(filepath)
-```
+- Добавлен репозиторий на GitHub - https://github.com/barlin41k/barladb
 
 
 # Что такое barlaDB?
 - `barlaDB` - это легкая, простая библиотека для небольших проектов на `Python`, которая имеет очень лёгкий интерфейс. С ней смогут познакомиться даже чайники в `Python`!
 
 # Лёгкий пример использования
 ```python
```

### Comparing `barladb-0.1.7/setup.py` & `barladb-0.1.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 from setuptools import setup
 
 setup(
     name='barladb',
-    version='0.1.7',
+    version='0.1.8',
     description='A very easy local database based on JSON',
     packages=['barladb'],
     author_email='sasaigrypocta@gmail.com',
     author="barlin41k",
     zip_safe=False,
     long_description='''
 # Изменения:
-- Добавлены новые функции и документация - https://sites.google.com/view/barladb/
-```python
-db.remove_column(filepath, key)
-db.columns(filepath)
-```
+- Добавлен репозиторий на GitHub - https://github.com/barlin41k/barladb
 
 
 # Что такое barlaDB?
 - `barlaDB` - это легкая, простая библиотека для небольших проектов на `Python`, которая имеет очень лёгкий интерфейс. С ней смогут познакомиться даже чайники в `Python`!
 
 # Лёгкий пример использования
 ```python
@@ -52,11 +48,12 @@
 
 # Особенности barlaDB
 - Простота в использовании
 - Очень лёгкий интерфейс
 - Базирована на всеми известном `JSON`
     ''',
     long_description_content_type="text/markdown",
-    url="https://sites.google.com/view/barladb/",
+    url="https://github.com/barlin41k/barladb",
     project_urls={
         "Documentation": "https://sites.google.com/view/barladb/",
+        "GitHub": "https://github.com/barlin41k/barladb",
     })
```

