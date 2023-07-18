# Comparing `tmp/Mensajes-angelus-1.5.tar.gz` & `tmp/Mensajes-angelus-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mensajes-angelus-1.5.tar", last modified: Mon Jul 17 22:20:35 2023, max compression
+gzip compressed data, was "Mensajes-angelus-1.6.tar", last modified: Tue Jul 18 03:28:12 2023, max compression
```

## Comparing `Mensajes-angelus-1.5.tar` & `Mensajes-angelus-1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 22:20:35.032573 Mensajes-angelus-1.5/
--rw-rw-rw-   0        0        0     1085 2023-07-17 21:40:21.000000 Mensajes-angelus-1.5/LICENSE
--rw-rw-rw-   0        0        0       60 2023-07-17 21:41:05.000000 Mensajes-angelus-1.5/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-07-17 22:20:35.016576 Mensajes-angelus-1.5/Mensajes_angelus.egg-info/
--rw-rw-rw-   0        0        0      368 2023-07-17 22:20:34.000000 Mensajes-angelus-1.5/Mensajes_angelus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      419 2023-07-17 22:20:34.000000 Mensajes-angelus-1.5/Mensajes_angelus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 22:20:34.000000 Mensajes-angelus-1.5/Mensajes_angelus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-17 22:20:34.000000 Mensajes-angelus-1.5/Mensajes_angelus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-17 22:20:34.000000 Mensajes-angelus-1.5/Mensajes_angelus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      368 2023-07-17 22:20:35.032573 Mensajes-angelus-1.5/PKG-INFO
--rw-rw-rw-   0        0        0       34 2023-07-17 21:26:31.000000 Mensajes-angelus-1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 22:20:35.016576 Mensajes-angelus-1.5/mensajes/
--rw-rw-rw-   0        0        0       37 2023-06-28 19:52:51.000000 Mensajes-angelus-1.5/mensajes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 22:20:35.024578 Mensajes-angelus-1.5/mensajes/adios/
--rw-rw-rw-   0        0        0       46 2023-06-28 19:44:17.000000 Mensajes-angelus-1.5/mensajes/adios/__init__.py
--rw-rw-rw-   0        0        0      160 2023-06-28 19:48:05.000000 Mensajes-angelus-1.5/mensajes/adios/despedidas.py
-drwxrwxrwx   0        0        0        0 2023-07-17 22:20:35.024578 Mensajes-angelus-1.5/mensajes/hola/
--rw-rw-rw-   0        0        0       45 2023-06-28 19:42:49.000000 Mensajes-angelus-1.5/mensajes/hola/__init__.py
--rw-rw-rw-   0        0        0      390 2023-07-17 00:48:09.000000 Mensajes-angelus-1.5/mensajes/hola/saludos.py
--rw-rw-rw-   0        0        0       13 2023-07-17 20:47:34.000000 Mensajes-angelus-1.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 22:20:35.032573 Mensajes-angelus-1.5/setup.cfg
--rw-rw-rw-   0        0        0      718 2023-07-17 22:16:01.000000 Mensajes-angelus-1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 22:20:35.032573 Mensajes-angelus-1.5/tests/
--rw-rw-rw-   0        0        0        0 2023-07-17 06:16:20.000000 Mensajes-angelus-1.5/tests/__init__.py
--rw-rw-rw-   0        0        0      269 2023-07-17 06:25:01.000000 Mensajes-angelus-1.5/tests/test_hola.py
+drwxrwxrwx   0        0        0        0 2023-07-18 03:28:12.064602 Mensajes-angelus-1.6/
+-rw-rw-rw-   0        0        0     1085 2023-07-17 21:40:21.000000 Mensajes-angelus-1.6/LICENSE
+-rw-rw-rw-   0        0        0       60 2023-07-17 21:41:05.000000 Mensajes-angelus-1.6/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-07-18 03:28:12.008611 Mensajes-angelus-1.6/Mensajes_angelus.egg-info/
+-rw-rw-rw-   0        0        0      368 2023-07-18 03:28:11.000000 Mensajes-angelus-1.6/Mensajes_angelus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      419 2023-07-18 03:28:11.000000 Mensajes-angelus-1.6/Mensajes_angelus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 03:28:11.000000 Mensajes-angelus-1.6/Mensajes_angelus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-18 03:28:11.000000 Mensajes-angelus-1.6/Mensajes_angelus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-18 03:28:11.000000 Mensajes-angelus-1.6/Mensajes_angelus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      368 2023-07-18 03:28:12.063594 Mensajes-angelus-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       34 2023-07-17 21:26:31.000000 Mensajes-angelus-1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 03:28:12.019611 Mensajes-angelus-1.6/mensajes/
+-rw-rw-rw-   0        0        0       37 2023-06-28 19:52:51.000000 Mensajes-angelus-1.6/mensajes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 03:28:12.027603 Mensajes-angelus-1.6/mensajes/adios/
+-rw-rw-rw-   0        0        0       46 2023-06-28 19:44:17.000000 Mensajes-angelus-1.6/mensajes/adios/__init__.py
+-rw-rw-rw-   0        0        0      160 2023-06-28 19:48:05.000000 Mensajes-angelus-1.6/mensajes/adios/despedidas.py
+drwxrwxrwx   0        0        0        0 2023-07-18 03:28:12.055602 Mensajes-angelus-1.6/mensajes/hola/
+-rw-rw-rw-   0        0        0       45 2023-06-28 19:42:49.000000 Mensajes-angelus-1.6/mensajes/hola/__init__.py
+-rw-rw-rw-   0        0        0      394 2023-07-18 03:20:01.000000 Mensajes-angelus-1.6/mensajes/hola/saludos.py
+-rw-rw-rw-   0        0        0       13 2023-07-17 20:47:34.000000 Mensajes-angelus-1.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 03:28:12.064602 Mensajes-angelus-1.6/setup.cfg
+-rw-rw-rw-   0        0        0      718 2023-07-18 03:20:21.000000 Mensajes-angelus-1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 03:28:12.061620 Mensajes-angelus-1.6/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-17 06:16:20.000000 Mensajes-angelus-1.6/tests/__init__.py
+-rw-rw-rw-   0        0        0      269 2023-07-17 06:25:01.000000 Mensajes-angelus-1.6/tests/test_hola.py
```

### Comparing `Mensajes-angelus-1.5/LICENSE` & `Mensajes-angelus-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Mensajes-angelus-1.5/setup.py` & `Mensajes-angelus-1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from struct import pack
 from setuptools import setup, find_packages
 
 setup(
     name = 'Mensajes-angelus',
-    version = '1.5',
+    version = '1.6',
     description = 'Paquete para saludar y despedir',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author = 'angelus',
     author_email = 'cloud.angelus@gmail.com',
     url = 'https://github.com/angelus',
     license_files=['LICENSE'],
```

