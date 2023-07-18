# Comparing `tmp/slack-to-discord-1.1.4.tar.gz` & `tmp/slack-to-discord-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack-to-discord-1.1.4.tar", last modified: Tue Jun  6 05:01:26 2023, max compression
+gzip compressed data, was "slack-to-discord-1.1.5.tar", last modified: Tue Jul 18 01:54:49 2023, max compression
```

## Comparing `slack-to-discord-1.1.4.tar` & `slack-to-discord-1.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 carey      (501) staff       (20)        0 2023-06-06 05:01:26.726762 slack-to-discord-1.1.4/
--rw-r--r--   0 carey      (501) staff       (20)     4432 2023-06-06 05:01:26.726332 slack-to-discord-1.1.4/PKG-INFO
--rw-r--r--   0 carey      (501) staff       (20)     3702 2023-05-14 04:31:17.000000 slack-to-discord-1.1.4/README.md
--rw-r--r--   0 carey      (501) staff       (20)       38 2023-06-06 05:01:26.726879 slack-to-discord-1.1.4/setup.cfg
--rw-r--r--   0 carey      (501) staff       (20)     1359 2023-06-06 04:51:11.000000 slack-to-discord-1.1.4/setup.py
-drwxr-xr-x   0 carey      (501) staff       (20)        0 2023-06-06 05:01:26.721921 slack-to-discord-1.1.4/slack_to_discord/
--rw-r--r--   0 carey      (501) staff       (20)      132 2022-10-19 02:44:12.000000 slack-to-discord-1.1.4/slack_to_discord/__init__.py
--rw-r--r--   0 carey      (501) staff       (20)     1756 2023-05-14 04:28:19.000000 slack-to-discord-1.1.4/slack_to_discord/__main__.py
--rw-r--r--   0 carey      (501) staff       (20)     9096 2023-02-16 03:38:45.000000 slack-to-discord-1.1.4/slack_to_discord/emojis.py
--rw-r--r--   0 carey      (501) staff       (20)     8435 2023-06-06 04:50:08.000000 slack-to-discord-1.1.4/slack_to_discord/http_stream.py
--rw-r--r--   0 carey      (501) staff       (20)    20840 2023-06-06 04:50:08.000000 slack-to-discord-1.1.4/slack_to_discord/importer.py
--rwxr-xr-x   0 carey      (501) staff       (20)      754 2023-02-16 03:02:54.000000 slack-to-discord-1.1.4/slack_to_discord/script.py
-drwxr-xr-x   0 carey      (501) staff       (20)        0 2023-06-06 05:01:26.724991 slack-to-discord-1.1.4/slack_to_discord.egg-info/
--rw-r--r--   0 carey      (501) staff       (20)     4432 2023-06-06 05:01:26.000000 slack-to-discord-1.1.4/slack_to_discord.egg-info/PKG-INFO
--rw-r--r--   0 carey      (501) staff       (20)      490 2023-06-06 05:01:26.000000 slack-to-discord-1.1.4/slack_to_discord.egg-info/SOURCES.txt
--rw-r--r--   0 carey      (501) staff       (20)        1 2023-06-06 05:01:26.000000 slack-to-discord-1.1.4/slack_to_discord.egg-info/dependency_links.txt
--rw-r--r--   0 carey      (501) staff       (20)       68 2023-06-06 05:01:26.000000 slack-to-discord-1.1.4/slack_to_discord.egg-info/entry_points.txt
--rw-r--r--   0 carey      (501) staff       (20)       49 2023-06-06 05:01:26.000000 slack-to-discord-1.1.4/slack_to_discord.egg-info/requires.txt
--rw-r--r--   0 carey      (501) staff       (20)       17 2023-06-06 05:01:26.000000 slack-to-discord-1.1.4/slack_to_discord.egg-info/top_level.txt
-drwxr-xr-x   0 carey      (501) staff       (20)        0 2023-06-06 05:01:26.725757 slack-to-discord-1.1.4/tests/
--rw-r--r--   0 carey      (501) staff       (20)     2951 2023-06-06 04:50:08.000000 slack-to-discord-1.1.4/tests/test_bufferediterator.py
--rwxr-xr-x   0 carey      (501) staff       (20)     3924 2023-06-06 04:50:08.000000 slack-to-discord-1.1.4/tests/test_http_stream.py
+drwxr-xr-x   0 carey      (501) staff       (20)        0 2023-07-18 01:54:49.166765 slack-to-discord-1.1.5/
+-rw-r--r--   0 carey      (501) staff       (20)     4383 2023-07-18 01:54:49.166130 slack-to-discord-1.1.5/PKG-INFO
+-rw-r--r--   0 carey      (501) staff       (20)     3702 2023-05-14 04:31:17.000000 slack-to-discord-1.1.5/README.md
+-rw-r--r--   0 carey      (501) staff       (20)       38 2023-07-18 01:54:49.166881 slack-to-discord-1.1.5/setup.cfg
+-rw-r--r--   0 carey      (501) staff       (20)     1311 2023-07-18 01:53:09.000000 slack-to-discord-1.1.5/setup.py
+drwxr-xr-x   0 carey      (501) staff       (20)        0 2023-07-18 01:54:49.159023 slack-to-discord-1.1.5/slack_to_discord/
+-rw-r--r--   0 carey      (501) staff       (20)      132 2022-10-19 02:44:12.000000 slack-to-discord-1.1.5/slack_to_discord/__init__.py
+-rw-r--r--   0 carey      (501) staff       (20)     1756 2023-05-14 04:28:19.000000 slack-to-discord-1.1.5/slack_to_discord/__main__.py
+-rw-r--r--   0 carey      (501) staff       (20)     9096 2023-02-16 03:38:45.000000 slack-to-discord-1.1.5/slack_to_discord/emojis.py
+-rw-r--r--   0 carey      (501) staff       (20)     8435 2023-06-06 04:50:08.000000 slack-to-discord-1.1.5/slack_to_discord/http_stream.py
+-rw-r--r--   0 carey      (501) staff       (20)    20840 2023-06-06 04:50:08.000000 slack-to-discord-1.1.5/slack_to_discord/importer.py
+-rwxr-xr-x   0 carey      (501) staff       (20)      754 2023-02-16 03:02:54.000000 slack-to-discord-1.1.5/slack_to_discord/script.py
+drwxr-xr-x   0 carey      (501) staff       (20)        0 2023-07-18 01:54:49.163837 slack-to-discord-1.1.5/slack_to_discord.egg-info/
+-rw-r--r--   0 carey      (501) staff       (20)     4383 2023-07-18 01:54:49.000000 slack-to-discord-1.1.5/slack_to_discord.egg-info/PKG-INFO
+-rw-r--r--   0 carey      (501) staff       (20)      490 2023-07-18 01:54:49.000000 slack-to-discord-1.1.5/slack_to_discord.egg-info/SOURCES.txt
+-rw-r--r--   0 carey      (501) staff       (20)        1 2023-07-18 01:54:49.000000 slack-to-discord-1.1.5/slack_to_discord.egg-info/dependency_links.txt
+-rw-r--r--   0 carey      (501) staff       (20)       68 2023-07-18 01:54:49.000000 slack-to-discord-1.1.5/slack_to_discord.egg-info/entry_points.txt
+-rw-r--r--   0 carey      (501) staff       (20)       49 2023-07-18 01:54:49.000000 slack-to-discord-1.1.5/slack_to_discord.egg-info/requires.txt
+-rw-r--r--   0 carey      (501) staff       (20)       17 2023-07-18 01:54:49.000000 slack-to-discord-1.1.5/slack_to_discord.egg-info/top_level.txt
+drwxr-xr-x   0 carey      (501) staff       (20)        0 2023-07-18 01:54:49.165330 slack-to-discord-1.1.5/tests/
+-rw-r--r--   0 carey      (501) staff       (20)     2951 2023-06-06 04:50:08.000000 slack-to-discord-1.1.5/tests/test_bufferediterator.py
+-rwxr-xr-x   0 carey      (501) staff       (20)     3924 2023-06-06 04:50:08.000000 slack-to-discord-1.1.5/tests/test_http_stream.py
```

### Comparing `slack-to-discord-1.1.4/PKG-INFO` & `slack-to-discord-1.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: slack-to-discord
-Version: 1.1.4
+Version: 1.1.5
 Summary: Extract data from a Slack export and import it into Discord
 Home-page: https://github.com/pR0Ps/slack-to-discord
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Communications :: Chat
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.6.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 
 slack-to-discord
 ================
 
 This tool takes a Slack export file and imports it into a Discord server
```

### Comparing `slack-to-discord-1.1.4/README.md` & `slack-to-discord-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `slack-to-discord-1.1.4/setup.py` & `slack-to-discord-1.1.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,28 +10,27 @@
         long_description = f.read()
 except Exception:
     long_description=None
 
 
 setup(
     name="slack-to-discord",
-    version="1.1.4",
+    version="1.1.5",
     description="Extract data from a Slack export and import it into Discord",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pR0Ps/slack-to-discord",
     license="GPLv3",
-    python_requires=">=3.6.0",
+    python_requires=">=3.8.0",
     classifiers=[
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
         "Topic :: Communications :: Chat",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)"
     ],
     install_requires = [
         "discord.py>=2.0.0,<3.0.0",
         "urllib3>=1.26.12,<2.0.0",
```

### Comparing `slack-to-discord-1.1.4/slack_to_discord/__main__.py` & `slack-to-discord-1.1.5/slack_to_discord/__main__.py`

 * *Files identical despite different names*

### Comparing `slack-to-discord-1.1.4/slack_to_discord/emojis.py` & `slack-to-discord-1.1.5/slack_to_discord/emojis.py`

 * *Files identical despite different names*

### Comparing `slack-to-discord-1.1.4/slack_to_discord/http_stream.py` & `slack-to-discord-1.1.5/slack_to_discord/http_stream.py`

 * *Files identical despite different names*

### Comparing `slack-to-discord-1.1.4/slack_to_discord/importer.py` & `slack-to-discord-1.1.5/slack_to_discord/importer.py`

 * *Files identical despite different names*

### Comparing `slack-to-discord-1.1.4/slack_to_discord/script.py` & `slack-to-discord-1.1.5/slack_to_discord/script.py`

 * *Files identical despite different names*

### Comparing `slack-to-discord-1.1.4/slack_to_discord.egg-info/PKG-INFO` & `slack-to-discord-1.1.5/slack_to_discord.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: slack-to-discord
-Version: 1.1.4
+Version: 1.1.5
 Summary: Extract data from a Slack export and import it into Discord
 Home-page: https://github.com/pR0Ps/slack-to-discord
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Communications :: Chat
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.6.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 
 slack-to-discord
 ================
 
 This tool takes a Slack export file and imports it into a Discord server
```

### Comparing `slack-to-discord-1.1.4/tests/test_bufferediterator.py` & `slack-to-discord-1.1.5/tests/test_bufferediterator.py`

 * *Files identical despite different names*

### Comparing `slack-to-discord-1.1.4/tests/test_http_stream.py` & `slack-to-discord-1.1.5/tests/test_http_stream.py`

 * *Files identical despite different names*

