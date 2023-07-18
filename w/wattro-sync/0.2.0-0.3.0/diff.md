# Comparing `tmp/wattro_sync-0.2.0.tar.gz` & `tmp/wattro_sync-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wattro_sync-0.2.0.tar", last modified: Thu Dec  8 12:33:40 2022, max compression
+gzip compressed data, was "wattro_sync-0.3.0.tar", last modified: Tue Jul 18 11:46:13 2023, max compression
```

## Comparing `wattro_sync-0.2.0.tar` & `wattro_sync-0.3.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2022-12-08 12:33:40.792211 wattro_sync-0.2.0/
--rw-r--r--   0 bastian   (1000) bastian   (1000)     1073 2022-11-11 16:56:53.000000 wattro_sync-0.2.0/LICENSE
--rw-r--r--   0 bastian   (1000) bastian   (1000)     2668 2022-12-08 12:33:40.792211 wattro_sync-0.2.0/PKG-INFO
--rw-r--r--   0 bastian   (1000) bastian   (1000)     2353 2022-12-06 15:07:31.000000 wattro_sync-0.2.0/README.md
--rw-r--r--   0 bastian   (1000) bastian   (1000)       38 2022-12-08 12:33:40.792211 wattro_sync-0.2.0/setup.cfg
--rw-r--r--   0 bastian   (1000) bastian   (1000)      585 2022-12-08 12:29:02.000000 wattro_sync-0.2.0/setup.py
-drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2022-12-08 12:33:40.785544 wattro_sync-0.2.0/tests/
--rw-r--r--   0 bastian   (1000) bastian   (1000)        0 2022-12-05 15:24:24.000000 wattro_sync-0.2.0/tests/__init__.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     7419 2022-12-05 15:24:24.000000 wattro_sync-0.2.0/tests/test_hash_history.py
-drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2022-12-08 12:33:40.785544 wattro_sync-0.2.0/wattro_sync/
--rw-r--r--   0 bastian   (1000) bastian   (1000)        0 2022-11-11 16:39:16.000000 wattro_sync-0.2.0/wattro_sync/__init__.py
-drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2022-12-08 12:33:40.788878 wattro_sync-0.2.0/wattro_sync/api/
--rw-r--r--   0 bastian   (1000) bastian   (1000)        0 2022-10-28 14:22:35.000000 wattro_sync-0.2.0/wattro_sync/api/__init__.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)      612 2022-12-07 15:21:33.000000 wattro_sync-0.2.0/wattro_sync/api/api_mapping.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     1770 2022-12-05 15:24:24.000000 wattro_sync-0.2.0/wattro_sync/api/mail.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     1840 2022-12-07 15:59:45.000000 wattro_sync-0.2.0/wattro_sync/api/mosaik_api.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     1790 2022-12-07 12:49:42.000000 wattro_sync-0.2.0/wattro_sync/api/odbc_api.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     4283 2022-12-07 13:54:46.000000 wattro_sync-0.2.0/wattro_sync/api/rest_api.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     2395 2022-12-08 12:32:12.000000 wattro_sync-0.2.0/wattro_sync/api/sqlite_api.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     3847 2022-12-07 13:48:19.000000 wattro_sync-0.2.0/wattro_sync/api/src_cli.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)      573 2022-12-06 14:41:42.000000 wattro_sync-0.2.0/wattro_sync/api/topkontor_api.py
-drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2022-12-08 12:33:40.788878 wattro_sync-0.2.0/wattro_sync/config_reader/
--rw-r--r--   0 bastian   (1000) bastian   (1000)        0 2022-10-28 12:45:32.000000 wattro_sync-0.2.0/wattro_sync/config_reader/__init__.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     3247 2022-12-08 12:32:12.000000 wattro_sync-0.2.0/wattro_sync/config_reader/access.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)      880 2022-12-05 15:24:36.000000 wattro_sync-0.2.0/wattro_sync/config_reader/types.py
-drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2022-12-08 12:33:40.792211 wattro_sync-0.2.0/wattro_sync/file_access/
--rw-r--r--   0 bastian   (1000) bastian   (1000)        0 2022-12-05 15:24:24.000000 wattro_sync-0.2.0/wattro_sync/file_access/__init__.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)      658 2022-12-05 15:24:36.000000 wattro_sync-0.2.0/wattro_sync/file_access/logging.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     3588 2022-12-07 14:01:37.000000 wattro_sync-0.2.0/wattro_sync/file_access/read_write.py
-drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2022-12-08 12:33:40.792211 wattro_sync-0.2.0/wattro_sync/hash_history/
--rw-r--r--   0 bastian   (1000) bastian   (1000)        0 2022-12-05 15:24:24.000000 wattro_sync-0.2.0/wattro_sync/hash_history/__init__.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     1567 2022-12-05 15:24:36.000000 wattro_sync-0.2.0/wattro_sync/hash_history/history.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     3187 2022-12-05 15:24:36.000000 wattro_sync-0.2.0/wattro_sync/helpers.py
--rwxr-xr-x   0 bastian   (1000) bastian   (1000)     9728 2022-12-08 12:30:30.000000 wattro_sync-0.2.0/wattro_sync/setup.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)    10475 2022-12-08 11:35:45.000000 wattro_sync-0.2.0/wattro_sync/sync.py
-drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2022-12-08 12:33:40.788878 wattro_sync-0.2.0/wattro_sync.egg-info/
--rw-r--r--   0 bastian   (1000) bastian   (1000)     2668 2022-12-08 12:33:40.000000 wattro_sync-0.2.0/wattro_sync.egg-info/PKG-INFO
--rw-r--r--   0 bastian   (1000) bastian   (1000)      883 2022-12-08 12:33:40.000000 wattro_sync-0.2.0/wattro_sync.egg-info/SOURCES.txt
--rw-r--r--   0 bastian   (1000) bastian   (1000)        1 2022-12-08 12:33:40.000000 wattro_sync-0.2.0/wattro_sync.egg-info/dependency_links.txt
--rw-r--r--   0 bastian   (1000) bastian   (1000)       42 2022-12-08 12:33:40.000000 wattro_sync-0.2.0/wattro_sync.egg-info/requires.txt
--rw-r--r--   0 bastian   (1000) bastian   (1000)       18 2022-12-08 12:33:40.000000 wattro_sync-0.2.0/wattro_sync.egg-info/top_level.txt
+drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2023-07-18 11:46:13.466155 wattro_sync-0.3.0/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     1073 2022-11-11 16:56:53.000000 wattro_sync-0.3.0/LICENSE
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     2570 2023-07-18 11:46:13.462821 wattro_sync-0.3.0/PKG-INFO
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     2255 2023-07-18 11:40:16.000000 wattro_sync-0.3.0/README.md
+-rw-r--r--   0 bastian   (1000) bastian   (1000)       38 2023-07-18 11:46:13.466155 wattro_sync-0.3.0/setup.cfg
+-rw-r--r--   0 bastian   (1000) bastian   (1000)      585 2023-07-18 11:45:36.000000 wattro_sync-0.3.0/setup.py
+drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2023-07-18 11:46:13.459488 wattro_sync-0.3.0/tests/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)        0 2022-12-05 15:24:24.000000 wattro_sync-0.3.0/tests/__init__.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     7419 2022-12-05 15:24:24.000000 wattro_sync-0.3.0/tests/test_hash_history.py
+drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2023-07-18 11:46:13.459488 wattro_sync-0.3.0/wattro_sync/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)        0 2022-11-11 16:39:16.000000 wattro_sync-0.3.0/wattro_sync/__init__.py
+drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2023-07-18 11:46:13.462821 wattro_sync-0.3.0/wattro_sync/api/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)        0 2022-10-28 14:22:35.000000 wattro_sync-0.3.0/wattro_sync/api/__init__.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)      612 2022-12-08 12:37:33.000000 wattro_sync-0.3.0/wattro_sync/api/api_mapping.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     1770 2022-12-05 15:24:24.000000 wattro_sync-0.3.0/wattro_sync/api/mail.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     2601 2023-07-18 11:40:16.000000 wattro_sync-0.3.0/wattro_sync/api/mosaik_api.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     1790 2022-12-08 12:37:33.000000 wattro_sync-0.3.0/wattro_sync/api/odbc_api.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     4283 2022-12-07 13:54:46.000000 wattro_sync-0.3.0/wattro_sync/api/rest_api.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     2395 2022-12-08 12:37:33.000000 wattro_sync-0.3.0/wattro_sync/api/sqlite_api.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     3847 2022-12-08 12:37:33.000000 wattro_sync-0.3.0/wattro_sync/api/src_cli.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)      573 2022-12-08 12:37:33.000000 wattro_sync-0.3.0/wattro_sync/api/topkontor_api.py
+drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2023-07-18 11:46:13.462821 wattro_sync-0.3.0/wattro_sync/config_reader/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)        0 2022-10-28 12:45:32.000000 wattro_sync-0.3.0/wattro_sync/config_reader/__init__.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     3247 2022-12-08 12:37:33.000000 wattro_sync-0.3.0/wattro_sync/config_reader/access.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)      880 2022-12-05 15:24:36.000000 wattro_sync-0.3.0/wattro_sync/config_reader/types.py
+drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2023-07-18 11:46:13.462821 wattro_sync-0.3.0/wattro_sync/file_access/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)        0 2022-12-05 15:24:24.000000 wattro_sync-0.3.0/wattro_sync/file_access/__init__.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)      658 2022-12-05 15:24:36.000000 wattro_sync-0.3.0/wattro_sync/file_access/logging.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     3567 2022-12-12 12:52:21.000000 wattro_sync-0.3.0/wattro_sync/file_access/read_write.py
+drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2023-07-18 11:46:13.462821 wattro_sync-0.3.0/wattro_sync/hash_history/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)        0 2022-12-05 15:24:24.000000 wattro_sync-0.3.0/wattro_sync/hash_history/__init__.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     1567 2022-12-05 15:24:36.000000 wattro_sync-0.3.0/wattro_sync/hash_history/history.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     3187 2022-12-05 15:24:36.000000 wattro_sync-0.3.0/wattro_sync/helpers.py
+-rwxr-xr-x   0 bastian   (1000) bastian   (1000)     9798 2022-12-12 12:54:13.000000 wattro_sync-0.3.0/wattro_sync/setup.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)    10475 2022-12-08 12:37:33.000000 wattro_sync-0.3.0/wattro_sync/sync.py
+drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2023-07-18 11:46:13.462821 wattro_sync-0.3.0/wattro_sync.egg-info/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     2570 2023-07-18 11:46:13.000000 wattro_sync-0.3.0/wattro_sync.egg-info/PKG-INFO
+-rw-r--r--   0 bastian   (1000) bastian   (1000)      883 2023-07-18 11:46:13.000000 wattro_sync-0.3.0/wattro_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 bastian   (1000) bastian   (1000)        1 2023-07-18 11:46:13.000000 wattro_sync-0.3.0/wattro_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 bastian   (1000) bastian   (1000)       42 2023-07-18 11:46:13.000000 wattro_sync-0.3.0/wattro_sync.egg-info/requires.txt
+-rw-r--r--   0 bastian   (1000) bastian   (1000)       18 2023-07-18 11:46:13.000000 wattro_sync-0.3.0/wattro_sync.egg-info/top_level.txt
```

### Comparing `wattro_sync-0.2.0/LICENSE` & `wattro_sync-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.2.0/PKG-INFO` & `wattro_sync-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,51 @@
 Metadata-Version: 2.1
 Name: wattro_sync
-Version: 0.2.0
+Version: 0.3.0
 Summary: Script collection to sync data from local sources to a wattro node
 Home-page: https://github.com/wattro/wattro_sync
 Author: Wattro GmbH
 Author-email: admin@wattro.de
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Wattro Sync Helfer
+# Wattro Sync
 
-Scriptsammlung, um das Synchronisieren von Daten aus einer lokalen Quelle nach Wattro zu
-erleichtern.
+Ermöglicht es, Daten aus einer lokalen Quelle mit Wattro zu synchronisieren.
 
 ## Voraussetzung
 
 * Verbindung zu wattro (https) und Quellsystem
 * python >= 3.10 und pip
 
 ## Installation
 
 * `pip install wattro-sync`
 
-## Anwendung
-
-Nach der Installation können die Scripte
-mit `python -m wattro_sync.[script_name] [Argumente]` aufgerufen werden.
-Etwa: `python -m wattro_sync.setup asset SQLite`
+## Einrichten
 
 ### Die zentrale Konfigurationsdatei
 
-Die Synchronisation beruht auf einer Konfigurationsdatei, welche mit `setup` erzeugt
-oder aktualisiert werden kann.
-Die Konfigurationsdatei kann auch von Hand angepasst werden.
-Mit `sync --dry` kann geprüft werden, ob die Synchronisation wie erwartet arbeitet.
-
-`setup` erwartet zwei Argumente:
+Die Synchronisation beruht auf einer Konfigurationsdatei, welche mit `python -m wattro_sync.setup ZIEL QUELLE` erzeugt
+oder aktualisiert werden kann (siehe `python -m wattro_sync.setup --help` für alle gültigen Optionen).
 
-* das Daten-Ziel (zum Beispiel 'asset': Geräte, die mit Wattro verwaltet werden)
-* der Daten Quelltyp (zum Beispiel 'Benning' für eine Benning Datenbank)
-
-Im Prozess werden je nach Ziel und Quelltyp verschiedene Eingaben abgefragt und die
+Im Prozess werden je nach Ziel- und Quelltyp verschiedene Eingaben abgefragt und die
 Datenverfügbarkeit geprüft.
 Nur gültige Werte werden in die Konfigurationsdatei geschrieben.
 
+*ACHTUNG* 
+
+Für Importe aus Mosaik muss aus technischen Gründen ein View angesporchen werden, welcher 
+* die Datensätze auf maximal 2k beschränkt und 
+* die Datensätze nach Änderungsdatum sortiert
+
+Die Konfigurationsdatei kann von Hand angepasst werden.
+Mit `python -m wattro_sync.sync --dry` kann geprüft werden, ob die Synchronisation wie erwartet arbeitet.
+
 #### Mail Infos
 
 Um Informationen zum Erfolg der Synchornisation zu bekommen, können Mails verschickt
 werden.
 Das "log_level" entspricht dabei einem numerischen Wert nach
 dem [Python Log Level Schema.](https://docs.python.org/3/library/logging.html#logging-levels)
 
@@ -56,20 +53,18 @@
 
 | Level | numerischer Wert | Mail wird versendet bei...  |
 |-------|------------------|-----------------------------|
 | ERROR | 40               | Fehler beim Synchronisieren |
 | INFO  | 20               | Änderung von Datensätzen    |
 | DEBUG | 10               | Aufruf des Scripts          |
 
-### Synchronisation
+## Synchronisation
 
-Mit `sync` werden die Daten synchronisiert.
-Die Synchronisation kann auch eingeschränkt, verbos oder als dry run durchgeführt
-werden.
-`sync --help` für mehr.
+Mit `python -m wattro_sync.sync` werden die Daten synchronisiert.
+Siehe `python -m wattro_sync.sync --help` für mehr.
 
 # Development
 
 ## Pre Commit tooling
 
 ```bash
 # requires black, mypy and bandit to be installed (via pip)
```

### Comparing `wattro_sync-0.2.0/README.md` & `wattro_sync-0.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,40 @@
-# Wattro Sync Helfer
+# Wattro Sync
 
-Scriptsammlung, um das Synchronisieren von Daten aus einer lokalen Quelle nach Wattro zu
-erleichtern.
+Ermöglicht es, Daten aus einer lokalen Quelle mit Wattro zu synchronisieren.
 
 ## Voraussetzung
 
 * Verbindung zu wattro (https) und Quellsystem
 * python >= 3.10 und pip
 
 ## Installation
 
 * `pip install wattro-sync`
 
-## Anwendung
-
-Nach der Installation können die Scripte
-mit `python -m wattro_sync.[script_name] [Argumente]` aufgerufen werden.
-Etwa: `python -m wattro_sync.setup asset SQLite`
+## Einrichten
 
 ### Die zentrale Konfigurationsdatei
 
-Die Synchronisation beruht auf einer Konfigurationsdatei, welche mit `setup` erzeugt
-oder aktualisiert werden kann.
-Die Konfigurationsdatei kann auch von Hand angepasst werden.
-Mit `sync --dry` kann geprüft werden, ob die Synchronisation wie erwartet arbeitet.
-
-`setup` erwartet zwei Argumente:
+Die Synchronisation beruht auf einer Konfigurationsdatei, welche mit `python -m wattro_sync.setup ZIEL QUELLE` erzeugt
+oder aktualisiert werden kann (siehe `python -m wattro_sync.setup --help` für alle gültigen Optionen).
 
-* das Daten-Ziel (zum Beispiel 'asset': Geräte, die mit Wattro verwaltet werden)
-* der Daten Quelltyp (zum Beispiel 'Benning' für eine Benning Datenbank)
-
-Im Prozess werden je nach Ziel und Quelltyp verschiedene Eingaben abgefragt und die
+Im Prozess werden je nach Ziel- und Quelltyp verschiedene Eingaben abgefragt und die
 Datenverfügbarkeit geprüft.
 Nur gültige Werte werden in die Konfigurationsdatei geschrieben.
 
+*ACHTUNG* 
+
+Für Importe aus Mosaik muss aus technischen Gründen ein View angesporchen werden, welcher 
+* die Datensätze auf maximal 2k beschränkt und 
+* die Datensätze nach Änderungsdatum sortiert
+
+Die Konfigurationsdatei kann von Hand angepasst werden.
+Mit `python -m wattro_sync.sync --dry` kann geprüft werden, ob die Synchronisation wie erwartet arbeitet.
+
 #### Mail Infos
 
 Um Informationen zum Erfolg der Synchornisation zu bekommen, können Mails verschickt
 werden.
 Das "log_level" entspricht dabei einem numerischen Wert nach
 dem [Python Log Level Schema.](https://docs.python.org/3/library/logging.html#logging-levels)
 
@@ -45,20 +42,18 @@
 
 | Level | numerischer Wert | Mail wird versendet bei...  |
 |-------|------------------|-----------------------------|
 | ERROR | 40               | Fehler beim Synchronisieren |
 | INFO  | 20               | Änderung von Datensätzen    |
 | DEBUG | 10               | Aufruf des Scripts          |
 
-### Synchronisation
+## Synchronisation
 
-Mit `sync` werden die Daten synchronisiert.
-Die Synchronisation kann auch eingeschränkt, verbos oder als dry run durchgeführt
-werden.
-`sync --help` für mehr.
+Mit `python -m wattro_sync.sync` werden die Daten synchronisiert.
+Siehe `python -m wattro_sync.sync --help` für mehr.
 
 # Development
 
 ## Pre Commit tooling
 
 ```bash
 # requires black, mypy and bandit to be installed (via pip)
```

### Comparing `wattro_sync-0.2.0/setup.py` & `wattro_sync-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="wattro_sync",
-    version="0.2.0",
+    version="0.3.0",
     description="Script collection to sync data from local sources to a wattro node",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wattro/wattro_sync",
     author="Wattro GmbH",
     author_email="admin@wattro.de",
     packages=setuptools.find_packages(),
```

### Comparing `wattro_sync-0.2.0/tests/test_hash_history.py` & `wattro_sync-0.3.0/tests/test_hash_history.py`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.2.0/wattro_sync/api/api_mapping.py` & `wattro_sync-0.3.0/wattro_sync/api/api_mapping.py`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.2.0/wattro_sync/api/mail.py` & `wattro_sync-0.3.0/wattro_sync/api/mail.py`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.2.0/wattro_sync/api/mosaik_api.py` & `wattro_sync-0.3.0/wattro_sync/api/sqlite_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,75 @@
-import dataclasses
-from typing import Any
-
-from wattro_sync.api.odbc_api import OdbcSyncInfo, OdbcSrcCliAltSample
-from wattro_sync.api.src_cli import CollectionInfo
+from __future__ import annotations
 
+import dataclasses
+import sqlite3
 
-@dataclasses.dataclass
-class MosaikConInfo:
-    Server: str
-    Database: str = "Mosaik"
-    Trusted_Connection: str = "Yes"
-    Driver: str = "{SQL Server}"
+from .src_cli import SrcCli, DBRes, CollectionInfo, SyncInfo
 
-    def to_connection_str(self) -> str:
-        return ";".join(f"{k}={v}" for k, v in dataclasses.asdict(self).items())
 
+class SQLiteSyncInfo(SyncInfo):
+    db_path: str
+    collection_info: CollectionInfo
 
-class MosaikSyncInfo(OdbcSyncInfo):
-    """branded ODBC Sync Info"""
+    def __init__(self, db_path: str, collection_info: CollectionInfo):
+        self.db_path = db_path
+        self.collection_info = collection_info
 
+    def asdict(self) -> dict:
+        return {
+            "db_path": str(self.db_path),
+            "collection_info": dataclasses.asdict(self.collection_info),
+        }
 
-class MosaikApi(OdbcSrcCliAltSample):
     @classmethod
-    def get_collections(cls, connection_info: Any) -> list[str]:
-        fake_api = cls(
-            MosaikSyncInfo(
-                odbc_connection_str=connection_info,
-                collection_info=CollectionInfo.empty(),
-            )
+    def from_dict(cls, info: dict) -> SQLiteSyncInfo:
+        return cls(
+            db_path=info["db_path"],
+            collection_info=CollectionInfo(**info["collection_info"]),
         )
-        db_res = fake_api._exec(
-            "SELECT name FROM SYSOBJECTS WHERE xtype='U' PO xtype='V';"
-        )
-        return sorted([x["name"] for x in db_res])
+
+
+class SQLiteApi(SrcCli):
+    def __init__(self, sync_info: SQLiteSyncInfo):
+        self.db_path = sync_info.db_path
+        self.collection_info = sync_info.collection_info
 
     @classmethod
     def get_fields(
-        cls, connection_info: Any, collection: str
+        cls, connection_info: str, collection: str
     ) -> tuple[list[str], dict[str, list]]:
-        fake_api = cls(
-            MosaikSyncInfo(
-                odbc_connection_str=connection_info,
-                collection_info=CollectionInfo.empty(),
-            )
-        )
-        meta_info = fake_api._exec(
-            "SELECT COLUMN_NAME FROM INFORMATION_SCHEMA.COLUMNS "
-            f"WHERE TABLE_NAME = '{collection}';"
-        )
-        field_names = sorted(list(str(x["COLUMN_NAME"]) for x in meta_info))
+        fake_api = cls(SQLiteSyncInfo(connection_info, CollectionInfo.empty()))
+        meta_info = fake_api._exec(f"PRAGMA table_info({collection})")
+        field_names = sorted(list([str(x["name"]) for x in meta_info]))
 
-        db_res = fake_api._exec(f"SELECT TOP 50 * FROM {collection}")
+        db_res = fake_api._exec(f"SELECT * FROM {collection} LIMIT 50")
         transposed_rows = list(map(list, zip(*db_res.rows)))
         sample_values = {
             field: val for field, val in zip(db_res.description, transposed_rows)
         }
         return field_names, sample_values
+
+    @classmethod
+    def get_collections(cls, connection_info: str) -> list[str]:
+        """
+        get_collections('/path/to/db')
+        """
+        fake_api = cls(
+            SQLiteSyncInfo(
+                db_path=connection_info, collection_info=CollectionInfo.empty()
+            )
+        )
+        db_res = fake_api._exec(f"PRAGMA table_list")
+        return sorted([x["name"] for x in db_res])
+
+    def _exec(self, qry: str, params=None) -> DBRes:
+        cnxn = sqlite3.connect(self.db_path)
+        cursr = cnxn.cursor()
+        if params is None:
+            params = tuple()
+        rows = cursr.execute(qry, params).fetchall()
+        if not rows:
+            res = DBRes([], [])
+        else:
+            res = DBRes([n[0] for n in cursr.description], rows)
+        cnxn.close()
+        return res
```

### Comparing `wattro_sync-0.2.0/wattro_sync/api/odbc_api.py` & `wattro_sync-0.3.0/wattro_sync/api/odbc_api.py`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.2.0/wattro_sync/api/rest_api.py` & `wattro_sync-0.3.0/wattro_sync/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.2.0/wattro_sync/api/src_cli.py` & `wattro_sync-0.3.0/wattro_sync/api/src_cli.py`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.2.0/wattro_sync/api/topkontor_api.py` & `wattro_sync-0.3.0/wattro_sync/api/topkontor_api.py`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.2.0/wattro_sync/config_reader/access.py` & `wattro_sync-0.3.0/wattro_sync/config_reader/access.py`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.2.0/wattro_sync/config_reader/types.py` & `wattro_sync-0.3.0/wattro_sync/config_reader/types.py`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.2.0/wattro_sync/file_access/logging.py` & `wattro_sync-0.3.0/wattro_sync/file_access/logging.py`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.2.0/wattro_sync/file_access/read_write.py` & `wattro_sync-0.3.0/wattro_sync/file_access/read_write.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 import os
 import pathlib
 import typing
 
 from wattro_sync.config_reader.types import ConfigDegenerated
 
 BASE_FOLDER = ".wattro_sync"
-FILE_NAMES = ["cfg.json", "history.json", "mail.json"]
+FILE_NAMES = ["cfg.json", "history.json"]
 CON_TYPE_KEY = "connection_type"
 CON_INFO_KEY = "connection_info"
 FIELD_MAP_KEY = "field_mapping"
 
-ShortType = typing.Literal["cfg", "history", "mail"]
+ShortType = typing.Literal["cfg", "history"]
 
 
 def exists(file_type: ShortType) -> bool:
     fp = _get_file_path(file_type)
     return fp.exists()
```

### Comparing `wattro_sync-0.2.0/wattro_sync/hash_history/history.py` & `wattro_sync-0.3.0/wattro_sync/hash_history/history.py`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.2.0/wattro_sync/helpers.py` & `wattro_sync-0.3.0/wattro_sync/helpers.py`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.2.0/wattro_sync/setup.py` & `wattro_sync-0.3.0/wattro_sync/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,15 +171,16 @@
         return None
     logging.info("Wattro API erreichbar unter %s", wattro_api.hostname)
     return wattro_api
 
 
 def get_mosaik_connnection_info() -> str:
     server_path = input("Server Pfad (z.B. SERVERNAME\\SQLMOSER):\t")
-    con_info = MosaikConInfo(server_path).to_connection_str()
+    db = input("Datenbank Name (z.B. Mosaik):\t")
+    con_info = MosaikConInfo(Server=server_path, Database=db).to_connection_str()
     return con_info
 
 
 def get_sqlite_connection_info() -> str:
     while True:
         db_path_str = input("Pfad zur Datenbank Datei (z.B. /path/to/db.sqlite3):\t")
         connection_info = pathlib.Path(db_path_str).resolve()
```

### Comparing `wattro_sync-0.2.0/wattro_sync/sync.py` & `wattro_sync-0.3.0/wattro_sync/sync.py`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.2.0/wattro_sync.egg-info/PKG-INFO` & `wattro_sync-0.3.0/wattro_sync.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,51 @@
 Metadata-Version: 2.1
 Name: wattro-sync
-Version: 0.2.0
+Version: 0.3.0
 Summary: Script collection to sync data from local sources to a wattro node
 Home-page: https://github.com/wattro/wattro_sync
 Author: Wattro GmbH
 Author-email: admin@wattro.de
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Wattro Sync Helfer
+# Wattro Sync
 
-Scriptsammlung, um das Synchronisieren von Daten aus einer lokalen Quelle nach Wattro zu
-erleichtern.
+Ermöglicht es, Daten aus einer lokalen Quelle mit Wattro zu synchronisieren.
 
 ## Voraussetzung
 
 * Verbindung zu wattro (https) und Quellsystem
 * python >= 3.10 und pip
 
 ## Installation
 
 * `pip install wattro-sync`
 
-## Anwendung
-
-Nach der Installation können die Scripte
-mit `python -m wattro_sync.[script_name] [Argumente]` aufgerufen werden.
-Etwa: `python -m wattro_sync.setup asset SQLite`
+## Einrichten
 
 ### Die zentrale Konfigurationsdatei
 
-Die Synchronisation beruht auf einer Konfigurationsdatei, welche mit `setup` erzeugt
-oder aktualisiert werden kann.
-Die Konfigurationsdatei kann auch von Hand angepasst werden.
-Mit `sync --dry` kann geprüft werden, ob die Synchronisation wie erwartet arbeitet.
-
-`setup` erwartet zwei Argumente:
+Die Synchronisation beruht auf einer Konfigurationsdatei, welche mit `python -m wattro_sync.setup ZIEL QUELLE` erzeugt
+oder aktualisiert werden kann (siehe `python -m wattro_sync.setup --help` für alle gültigen Optionen).
 
-* das Daten-Ziel (zum Beispiel 'asset': Geräte, die mit Wattro verwaltet werden)
-* der Daten Quelltyp (zum Beispiel 'Benning' für eine Benning Datenbank)
-
-Im Prozess werden je nach Ziel und Quelltyp verschiedene Eingaben abgefragt und die
+Im Prozess werden je nach Ziel- und Quelltyp verschiedene Eingaben abgefragt und die
 Datenverfügbarkeit geprüft.
 Nur gültige Werte werden in die Konfigurationsdatei geschrieben.
 
+*ACHTUNG* 
+
+Für Importe aus Mosaik muss aus technischen Gründen ein View angesporchen werden, welcher 
+* die Datensätze auf maximal 2k beschränkt und 
+* die Datensätze nach Änderungsdatum sortiert
+
+Die Konfigurationsdatei kann von Hand angepasst werden.
+Mit `python -m wattro_sync.sync --dry` kann geprüft werden, ob die Synchronisation wie erwartet arbeitet.
+
 #### Mail Infos
 
 Um Informationen zum Erfolg der Synchornisation zu bekommen, können Mails verschickt
 werden.
 Das "log_level" entspricht dabei einem numerischen Wert nach
 dem [Python Log Level Schema.](https://docs.python.org/3/library/logging.html#logging-levels)
 
@@ -56,20 +53,18 @@
 
 | Level | numerischer Wert | Mail wird versendet bei...  |
 |-------|------------------|-----------------------------|
 | ERROR | 40               | Fehler beim Synchronisieren |
 | INFO  | 20               | Änderung von Datensätzen    |
 | DEBUG | 10               | Aufruf des Scripts          |
 
-### Synchronisation
+## Synchronisation
 
-Mit `sync` werden die Daten synchronisiert.
-Die Synchronisation kann auch eingeschränkt, verbos oder als dry run durchgeführt
-werden.
-`sync --help` für mehr.
+Mit `python -m wattro_sync.sync` werden die Daten synchronisiert.
+Siehe `python -m wattro_sync.sync --help` für mehr.
 
 # Development
 
 ## Pre Commit tooling
 
 ```bash
 # requires black, mypy and bandit to be installed (via pip)
```

### Comparing `wattro_sync-0.2.0/wattro_sync.egg-info/SOURCES.txt` & `wattro_sync-0.3.0/wattro_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

