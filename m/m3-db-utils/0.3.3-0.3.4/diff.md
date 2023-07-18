# Comparing `tmp/m3_db_utils-0.3.3.tar.gz` & `tmp/m3_db_utils-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m3_db_utils-0.3.3.tar", last modified: Thu Oct 20 09:26:31 2022, max compression
+gzip compressed data, was "m3_db_utils-0.3.4.tar", last modified: Tue Jul 18 10:11:36 2023, max compression
```

## Comparing `m3_db_utils-0.3.3.tar` & `m3_db_utils-0.3.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-20 09:26:31.353463 m3_db_utils-0.3.3/
--rw-r--r--   0 root         (0) root         (0)     4028 2022-10-20 09:26:23.000000 m3_db_utils-0.3.3/CHANGES.md
--rw-r--r--   0 root         (0) root         (0)      134 2022-07-06 05:33:04.000000 m3_db_utils-0.3.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4986 2022-10-20 09:26:31.353463 m3_db_utils-0.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      100 2022-02-16 13:29:22.000000 m3_db_utils-0.3.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-20 09:26:31.339463 m3_db_utils-0.3.3/docs/
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-16 13:29:22.000000 m3_db_utils-0.3.3/docs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3517 2022-08-08 12:42:06.000000 m3_db_utils-0.3.3/docs/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-20 09:26:31.351463 m3_db_utils-0.3.3/m3_db_utils/
--rw-r--r--   0 root         (0) root         (0)       56 2022-02-16 13:29:22.000000 m3_db_utils-0.3.3/m3_db_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      340 2022-02-16 13:29:22.000000 m3_db_utils-0.3.3/m3_db_utils/api.py
--rw-r--r--   0 root         (0) root         (0)      546 2022-08-08 12:42:06.000000 m3_db_utils-0.3.3/m3_db_utils/apps.py
--rw-r--r--   0 root         (0) root         (0)      186 2022-08-09 06:48:57.000000 m3_db_utils-0.3.3/m3_db_utils/consts.py
--rw-r--r--   0 root         (0) root         (0)      800 2022-10-20 09:26:23.000000 m3_db_utils-0.3.3/m3_db_utils/decorators.py
--rw-r--r--   0 root         (0) root         (0)      300 2022-02-16 13:30:47.000000 m3_db_utils-0.3.3/m3_db_utils/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      760 2022-08-08 12:42:06.000000 m3_db_utils-0.3.3/m3_db_utils/excludes.py
--rw-r--r--   0 root         (0) root         (0)     6644 2022-07-25 11:46:40.000000 m3_db_utils-0.3.3/m3_db_utils/helpers.py
--rw-r--r--   0 root         (0) root         (0)     2203 2022-08-09 06:48:57.000000 m3_db_utils-0.3.3/m3_db_utils/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-20 09:26:31.353463 m3_db_utils-0.3.3/m3_db_utils/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-27 13:28:20.000000 m3_db_utils-0.3.3/m3_db_utils/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1002 2022-02-16 13:29:22.000000 m3_db_utils-0.3.3/m3_db_utils/mixins.py
--rw-r--r--   0 root         (0) root         (0)    32215 2022-10-20 09:26:23.000000 m3_db_utils-0.3.3/m3_db_utils/models.py
--rw-r--r--   0 root         (0) root         (0)     4455 2022-02-16 13:30:47.000000 m3_db_utils-0.3.3/m3_db_utils/options.py
--rw-r--r--   0 root         (0) root         (0)      330 2022-07-27 13:28:20.000000 m3_db_utils-0.3.3/m3_db_utils/receivers.py
--rw-r--r--   0 root         (0) root         (0)     1228 2022-08-09 06:48:57.000000 m3_db_utils-0.3.3/m3_db_utils/settings.py
--rw-r--r--   0 root         (0) root         (0)      279 2022-02-16 13:29:22.000000 m3_db_utils-0.3.3/m3_db_utils/strings.py
--rw-r--r--   0 root         (0) root         (0)     4687 2022-10-20 09:26:23.000000 m3_db_utils-0.3.3/m3_db_utils/wrappers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-20 09:26:31.352463 m3_db_utils-0.3.3/m3_db_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4986 2022-10-20 09:26:31.000000 m3_db_utils-0.3.3/m3_db_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      704 2022-10-20 09:26:31.000000 m3_db_utils-0.3.3/m3_db_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-20 09:26:31.000000 m3_db_utils-0.3.3/m3_db_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-16 13:29:30.000000 m3_db_utils-0.3.3/m3_db_utils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       48 2022-10-20 09:26:31.000000 m3_db_utils-0.3.3/m3_db_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-10-20 09:26:31.000000 m3_db_utils-0.3.3/m3_db_utils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       47 2022-08-08 12:42:06.000000 m3_db_utils-0.3.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-10-20 09:26:31.353463 m3_db_utils-0.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1988 2022-10-20 09:26:23.000000 m3_db_utils-0.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 10:11:36.634542 m3_db_utils-0.3.4/
+-rw-r--r--   0 root         (0) root         (0)     4196 2023-07-18 10:11:28.000000 m3_db_utils-0.3.4/CHANGES.md
+-rw-r--r--   0 root         (0) root         (0)      134 2022-07-06 05:33:04.000000 m3_db_utils-0.3.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5154 2023-07-18 10:11:36.633542 m3_db_utils-0.3.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      100 2022-02-16 13:29:22.000000 m3_db_utils-0.3.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 10:11:36.605542 m3_db_utils-0.3.4/docs/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-16 13:29:22.000000 m3_db_utils-0.3.4/docs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3517 2022-08-08 12:42:06.000000 m3_db_utils-0.3.4/docs/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 10:11:36.630542 m3_db_utils-0.3.4/m3_db_utils/
+-rw-r--r--   0 root         (0) root         (0)       56 2022-02-16 13:29:22.000000 m3_db_utils-0.3.4/m3_db_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      340 2022-02-16 13:29:22.000000 m3_db_utils-0.3.4/m3_db_utils/api.py
+-rw-r--r--   0 root         (0) root         (0)      546 2022-08-08 12:42:06.000000 m3_db_utils-0.3.4/m3_db_utils/apps.py
+-rw-r--r--   0 root         (0) root         (0)      186 2022-08-09 06:48:57.000000 m3_db_utils-0.3.4/m3_db_utils/consts.py
+-rw-r--r--   0 root         (0) root         (0)      800 2022-10-20 09:26:23.000000 m3_db_utils-0.3.4/m3_db_utils/decorators.py
+-rw-r--r--   0 root         (0) root         (0)      300 2022-02-16 13:30:47.000000 m3_db_utils-0.3.4/m3_db_utils/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      760 2022-08-08 12:42:06.000000 m3_db_utils-0.3.4/m3_db_utils/excludes.py
+-rw-r--r--   0 root         (0) root         (0)     6644 2022-07-25 11:46:40.000000 m3_db_utils-0.3.4/m3_db_utils/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     2203 2022-08-09 06:48:57.000000 m3_db_utils-0.3.4/m3_db_utils/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 10:11:36.633542 m3_db_utils-0.3.4/m3_db_utils/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-27 13:28:20.000000 m3_db_utils-0.3.4/m3_db_utils/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2022-02-16 13:29:22.000000 m3_db_utils-0.3.4/m3_db_utils/mixins.py
+-rw-r--r--   0 root         (0) root         (0)    33243 2023-07-18 10:11:28.000000 m3_db_utils-0.3.4/m3_db_utils/models.py
+-rw-r--r--   0 root         (0) root         (0)     4455 2022-02-16 13:30:47.000000 m3_db_utils-0.3.4/m3_db_utils/options.py
+-rw-r--r--   0 root         (0) root         (0)      330 2022-07-27 13:28:20.000000 m3_db_utils-0.3.4/m3_db_utils/receivers.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2022-08-09 06:48:57.000000 m3_db_utils-0.3.4/m3_db_utils/settings.py
+-rw-r--r--   0 root         (0) root         (0)      279 2022-02-16 13:29:22.000000 m3_db_utils-0.3.4/m3_db_utils/strings.py
+-rw-r--r--   0 root         (0) root         (0)     4687 2022-10-20 09:26:23.000000 m3_db_utils-0.3.4/m3_db_utils/wrappers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 10:11:36.633542 m3_db_utils-0.3.4/m3_db_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5154 2023-07-18 10:11:36.000000 m3_db_utils-0.3.4/m3_db_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      704 2023-07-18 10:11:36.000000 m3_db_utils-0.3.4/m3_db_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 10:11:36.000000 m3_db_utils-0.3.4/m3_db_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-02-16 13:29:30.000000 m3_db_utils-0.3.4/m3_db_utils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-18 10:11:36.000000 m3_db_utils-0.3.4/m3_db_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-18 10:11:36.000000 m3_db_utils-0.3.4/m3_db_utils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2022-08-08 12:42:06.000000 m3_db_utils-0.3.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 10:11:36.634542 m3_db_utils-0.3.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1988 2023-07-18 10:11:28.000000 m3_db_utils-0.3.4/setup.py
```

### Comparing `m3_db_utils-0.3.3/CHANGES.md` & `m3_db_utils-0.3.4/CHANGES.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+0.3.4
+
+* (EDUSCHL-19919) Добавлена возможность расширения модели-перечисления множеством элементов.
+
 0.3.3
 
 * (EDUSCHL-18423) Убрано кеширование.
 
 0.3.2
 
 * Отказ от m3_legacy.
```

### Comparing `m3_db_utils-0.3.3/PKG-INFO` & `m3_db_utils-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m3_db_utils
-Version: 0.3.3
+Version: 0.3.4
 Summary: m3_db_utils
 Home-page: https://stash.bars-open.ru/projects/M3/repos/m3_db_utils/browse
 Download-URL: http://nexus.budg.bars.group/#browse/browse:pypi-bars-private:m3-db-utils
 Author: Alexander Danilenko
 Author-email: a.danilenko@bars.group
 License: MIT
 Platform: Any
@@ -19,15 +19,19 @@
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Description-Content-Type: text/markdown
 
 # Кастомный инструментарий для работы с базой данных
 
 
- 0.3.3
+ 0.3.4
+
+* (EDUSCHL-19919) Добавлена возможность расширения модели-перечисления множеством элементов.
+
+0.3.3
 
 * (EDUSCHL-18423) Убрано кеширование.
 
 0.3.2
 
 * Отказ от m3_legacy.
```

### Comparing `m3_db_utils-0.3.3/docs/settings.py` & `m3_db_utils-0.3.4/docs/settings.py`

 * *Files identical despite different names*

### Comparing `m3_db_utils-0.3.3/m3_db_utils/apps.py` & `m3_db_utils-0.3.4/m3_db_utils/apps.py`

 * *Files identical despite different names*

### Comparing `m3_db_utils-0.3.3/m3_db_utils/decorators.py` & `m3_db_utils-0.3.4/m3_db_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `m3_db_utils-0.3.3/m3_db_utils/excludes.py` & `m3_db_utils-0.3.4/m3_db_utils/excludes.py`

 * *Files identical despite different names*

### Comparing `m3_db_utils-0.3.3/m3_db_utils/helpers.py` & `m3_db_utils-0.3.4/m3_db_utils/helpers.py`

 * *Files identical despite different names*

### Comparing `m3_db_utils-0.3.3/m3_db_utils/logger.py` & `m3_db_utils-0.3.4/m3_db_utils/logger.py`

 * *Files identical despite different names*

### Comparing `m3_db_utils-0.3.3/m3_db_utils/mixins.py` & `m3_db_utils-0.3.4/m3_db_utils/mixins.py`

 * *Files identical despite different names*

### Comparing `m3_db_utils-0.3.3/m3_db_utils/models.py` & `m3_db_utils-0.3.4/m3_db_utils/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -630,14 +630,29 @@
 
         Args:
             key: ключ элемента перечисления, указывается заглавными буквами с разделителем нижнее подчеркивание
             order_number: порядковый номер значения модели перечисления используемый при сортировке
         """
         setattr(cls, key, ModelEnumValue(key=key, order_number=order_number, **kwargs))
 
+    @classmethod
+    def extends(cls, items: List[Dict[str, Any]]):
+        """
+        Метод расширения модели-перечисления множеством значений. Расширение производится, например, из плагина.
+        Необходимо, чтобы сама модель-перечисление была расширяемой. Для этого необходимо, чтобы был установлен
+        extensible = True в Meta.
+
+        Args:
+            items: список словарей со значениями для формирования значений модели-перечисления. Обязательным полем
+                является key, order_number заполняется в случае необходимости соблюдения порядка значений
+                модели-перечисления.
+        """
+        for item in items:
+            cls.extend(**item)
+
     @property
     def model_enum_value(self) -> ModelEnumValue:
         """
         Получение значения модели-перечисления у экземпляра модели.
         """
         return getattr(self, self.key)
```

### Comparing `m3_db_utils-0.3.3/m3_db_utils/options.py` & `m3_db_utils-0.3.4/m3_db_utils/options.py`

 * *Files identical despite different names*

### Comparing `m3_db_utils-0.3.3/m3_db_utils/settings.py` & `m3_db_utils-0.3.4/m3_db_utils/settings.py`

 * *Files identical despite different names*

### Comparing `m3_db_utils-0.3.3/m3_db_utils/wrappers.py` & `m3_db_utils-0.3.4/m3_db_utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `m3_db_utils-0.3.3/m3_db_utils.egg-info/PKG-INFO` & `m3_db_utils-0.3.4/m3_db_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m3-db-utils
-Version: 0.3.3
+Version: 0.3.4
 Summary: m3_db_utils
 Home-page: https://stash.bars-open.ru/projects/M3/repos/m3_db_utils/browse
 Download-URL: http://nexus.budg.bars.group/#browse/browse:pypi-bars-private:m3-db-utils
 Author: Alexander Danilenko
 Author-email: a.danilenko@bars.group
 License: MIT
 Platform: Any
@@ -19,15 +19,19 @@
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Description-Content-Type: text/markdown
 
 # Кастомный инструментарий для работы с базой данных
 
 
- 0.3.3
+ 0.3.4
+
+* (EDUSCHL-19919) Добавлена возможность расширения модели-перечисления множеством элементов.
+
+0.3.3
 
 * (EDUSCHL-18423) Убрано кеширование.
 
 0.3.2
 
 * Отказ от m3_legacy.
```

### Comparing `m3_db_utils-0.3.3/m3_db_utils.egg-info/SOURCES.txt` & `m3_db_utils-0.3.4/m3_db_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m3_db_utils-0.3.3/setup.py` & `m3_db_utils-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from setuptools import (
     find_packages,
     setup,
 )
 
 
-__version__ = '0.3.3'
+__version__ = '0.3.4'
 
 
 here = path.abspath(path.dirname(__file__))
 
 # Получение полного описание из README.md
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
```

