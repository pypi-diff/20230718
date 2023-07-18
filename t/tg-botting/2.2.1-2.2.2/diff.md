# Comparing `tmp/tg-botting-2.2.1.tar.gz` & `tmp/tg-botting-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg-botting-2.2.1.tar", last modified: Tue Jul 18 13:54:12 2023, max compression
+gzip compressed data, was "tg-botting-2.2.2.tar", last modified: Tue Jul 18 13:55:20 2023, max compression
```

## Comparing `tg-botting-2.2.1.tar` & `tg-botting-2.2.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 13:54:12.274901 tg-botting-2.2.1/
--rw-rw-rw-   0        0        0     3407 2023-07-18 13:54:12.273904 tg-botting-2.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1709 2023-07-12 19:32:58.000000 tg-botting-2.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-18 13:54:12.274901 tg-botting-2.2.1/setup.cfg
--rw-rw-rw-   0        0        0     2624 2023-07-12 19:37:56.000000 tg-botting-2.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 13:54:12.267919 tg-botting-2.2.1/tg_botting/
--rw-rw-rw-   0        0        0      798 2023-07-18 13:53:57.000000 tg-botting-2.2.1/tg_botting/__init__.py
--rw-rw-rw-   0        0        0       39 2023-05-26 21:28:31.000000 tg-botting-2.2.1/tg_botting/_types.py
--rw-rw-rw-   0        0        0      730 2023-07-13 11:59:36.000000 tg-botting-2.2.1/tg_botting/abstract.py
--rw-rw-rw-   0        0        0    19269 2023-07-12 16:28:14.000000 tg-botting-2.2.1/tg_botting/bot.py
--rw-rw-rw-   0        0        0    31724 2023-07-18 13:44:21.000000 tg-botting-2.2.1/tg_botting/client.py
--rw-rw-rw-   0        0        0    12615 2023-05-26 21:34:31.000000 tg-botting-2.2.1/tg_botting/cog.py
--rw-rw-rw-   0        0        0    35621 2023-05-26 21:39:01.000000 tg-botting-2.2.1/tg_botting/commands.py
--rw-rw-rw-   0        0        0     3635 2023-07-13 11:59:36.000000 tg-botting-2.2.1/tg_botting/context.py
--rw-rw-rw-   0        0        0     1361 2023-05-26 21:43:21.000000 tg-botting-2.2.1/tg_botting/context_managers.py
--rw-rw-rw-   0        0        0     1410 2023-05-26 21:35:15.000000 tg-botting-2.2.1/tg_botting/conversions.py
--rw-rw-rw-   0        0        0     3679 2023-05-26 21:31:45.000000 tg-botting-2.2.1/tg_botting/cooldowns.py
--rw-rw-rw-   0        0        0    10433 2023-05-26 21:27:27.000000 tg-botting-2.2.1/tg_botting/exceptions.py
--rw-rw-rw-   0        0        0      902 2023-05-27 14:01:15.000000 tg-botting-2.2.1/tg_botting/general.py
--rw-rw-rw-   0        0        0     9737 2023-05-27 13:35:03.000000 tg-botting-2.2.1/tg_botting/group.py
--rw-rw-rw-   0        0        0      578 2023-07-14 23:30:00.000000 tg-botting-2.2.1/tg_botting/limiters.py
--rw-rw-rw-   0        0        0    18188 2023-07-18 13:53:57.000000 tg-botting-2.2.1/tg_botting/message.py
--rw-rw-rw-   0        0        0    33157 2023-07-18 13:53:57.000000 tg-botting-2.2.1/tg_botting/objects.py
--rw-rw-rw-   0        0        0     3037 2023-07-11 21:05:01.000000 tg-botting-2.2.1/tg_botting/permissions.py
--rw-rw-rw-   0        0        0     1919 2023-07-12 15:17:24.000000 tg-botting-2.2.1/tg_botting/user.py
--rw-rw-rw-   0        0        0     1023 2023-07-13 22:59:13.000000 tg-botting-2.2.1/tg_botting/utils.py
--rw-rw-rw-   0        0        0     4368 2023-05-26 21:44:26.000000 tg-botting-2.2.1/tg_botting/view.py
-drwxrwxrwx   0        0        0        0 2023-07-18 13:54:12.272931 tg-botting-2.2.1/tg_botting.egg-info/
--rw-rw-rw-   0        0        0     3407 2023-07-18 13:54:12.000000 tg-botting-2.2.1/tg_botting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      655 2023-07-18 13:54:12.000000 tg-botting-2.2.1/tg_botting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 13:54:12.000000 tg-botting-2.2.1/tg_botting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-07-18 13:54:12.000000 tg-botting-2.2.1/tg_botting.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-18 13:54:12.000000 tg-botting-2.2.1/tg_botting.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 13:55:20.609991 tg-botting-2.2.2/
+-rw-rw-rw-   0        0        0     3407 2023-07-18 13:55:20.609991 tg-botting-2.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1709 2023-07-12 19:32:58.000000 tg-botting-2.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-18 13:55:20.609991 tg-botting-2.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     2624 2023-07-12 19:37:56.000000 tg-botting-2.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:55:20.605006 tg-botting-2.2.2/tg_botting/
+-rw-rw-rw-   0        0        0      798 2023-07-18 13:55:17.000000 tg-botting-2.2.2/tg_botting/__init__.py
+-rw-rw-rw-   0        0        0       39 2023-05-26 21:28:31.000000 tg-botting-2.2.2/tg_botting/_types.py
+-rw-rw-rw-   0        0        0      730 2023-07-13 11:59:36.000000 tg-botting-2.2.2/tg_botting/abstract.py
+-rw-rw-rw-   0        0        0    19269 2023-07-12 16:28:14.000000 tg-botting-2.2.2/tg_botting/bot.py
+-rw-rw-rw-   0        0        0    31688 2023-07-18 13:55:11.000000 tg-botting-2.2.2/tg_botting/client.py
+-rw-rw-rw-   0        0        0    12615 2023-05-26 21:34:31.000000 tg-botting-2.2.2/tg_botting/cog.py
+-rw-rw-rw-   0        0        0    35621 2023-05-26 21:39:01.000000 tg-botting-2.2.2/tg_botting/commands.py
+-rw-rw-rw-   0        0        0     3635 2023-07-13 11:59:36.000000 tg-botting-2.2.2/tg_botting/context.py
+-rw-rw-rw-   0        0        0     1361 2023-05-26 21:43:21.000000 tg-botting-2.2.2/tg_botting/context_managers.py
+-rw-rw-rw-   0        0        0     1410 2023-05-26 21:35:15.000000 tg-botting-2.2.2/tg_botting/conversions.py
+-rw-rw-rw-   0        0        0     3679 2023-05-26 21:31:45.000000 tg-botting-2.2.2/tg_botting/cooldowns.py
+-rw-rw-rw-   0        0        0    10433 2023-05-26 21:27:27.000000 tg-botting-2.2.2/tg_botting/exceptions.py
+-rw-rw-rw-   0        0        0      902 2023-05-27 14:01:15.000000 tg-botting-2.2.2/tg_botting/general.py
+-rw-rw-rw-   0        0        0     9737 2023-05-27 13:35:03.000000 tg-botting-2.2.2/tg_botting/group.py
+-rw-rw-rw-   0        0        0      578 2023-07-14 23:30:00.000000 tg-botting-2.2.2/tg_botting/limiters.py
+-rw-rw-rw-   0        0        0    18188 2023-07-18 13:53:57.000000 tg-botting-2.2.2/tg_botting/message.py
+-rw-rw-rw-   0        0        0    33157 2023-07-18 13:53:57.000000 tg-botting-2.2.2/tg_botting/objects.py
+-rw-rw-rw-   0        0        0     3037 2023-07-11 21:05:01.000000 tg-botting-2.2.2/tg_botting/permissions.py
+-rw-rw-rw-   0        0        0     1919 2023-07-12 15:17:24.000000 tg-botting-2.2.2/tg_botting/user.py
+-rw-rw-rw-   0        0        0     1023 2023-07-13 22:59:13.000000 tg-botting-2.2.2/tg_botting/utils.py
+-rw-rw-rw-   0        0        0     4368 2023-05-26 21:44:26.000000 tg-botting-2.2.2/tg_botting/view.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:55:20.608995 tg-botting-2.2.2/tg_botting.egg-info/
+-rw-rw-rw-   0        0        0     3407 2023-07-18 13:55:20.000000 tg-botting-2.2.2/tg_botting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      655 2023-07-18 13:55:20.000000 tg-botting-2.2.2/tg_botting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 13:55:20.000000 tg-botting-2.2.2/tg_botting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-07-18 13:55:20.000000 tg-botting-2.2.2/tg_botting.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-18 13:55:20.000000 tg-botting-2.2.2/tg_botting.egg-info/top_level.txt
```

### Comparing `tg-botting-2.2.1/PKG-INFO` & `tg-botting-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 2.2.1
+Version: 2.2.2
 Summary: A basic package for building async TG bots
 Home-page: https://github.com/2sweetheart2/tg_botting
 Author: Sweetie (Roma Fomkin)
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `tg-botting-2.2.1/README.md` & `tg-botting-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `tg-botting-2.2.1/setup.py` & `tg-botting-2.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.2.1/tg_botting/__init__.py` & `tg-botting-2.2.2/tg_botting/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 _title__ = 'tg_botting'
 __author__ = 'Sweetie'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023-present Sweetie'
-__version__ = '2.2.1'
+__version__ = '2.2.2'
 
 from collections import namedtuple
 import logging
 
 from .bot import Bot
 from .limiters import *
 from .conversions import Converter
```

### Comparing `tg-botting-2.2.1/tg_botting/abstract.py` & `tg-botting-2.2.2/tg_botting/abstract.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.2.1/tg_botting/bot.py` & `tg-botting-2.2.2/tg_botting/bot.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.2.1/tg_botting/client.py` & `tg-botting-2.2.2/tg_botting/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,15 +328,14 @@
             action = "chat_member_left"
         elif msg.photo is not None:
             action = "photo_new"
         elif msg.new_chat_members is not None:
             action = 'new_chat_members'
         elif msg.successful_payment is not None:
             action = "successful_payment"
-        print(f'ACTION: {action}')
         if action is not None:
             return self.dispatch(action, msg)
         if msg.text is None:
             return self.dispatch("something_without_text",msg)
         return self.dispatch('message_new', msg)
 
     def handle_callback_query(self, t, obj):
```

### Comparing `tg-botting-2.2.1/tg_botting/cog.py` & `tg-botting-2.2.2/tg_botting/cog.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.2.1/tg_botting/commands.py` & `tg-botting-2.2.2/tg_botting/commands.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.2.1/tg_botting/context.py` & `tg-botting-2.2.2/tg_botting/context.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.2.1/tg_botting/context_managers.py` & `tg-botting-2.2.2/tg_botting/context_managers.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.2.1/tg_botting/conversions.py` & `tg-botting-2.2.2/tg_botting/conversions.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.2.1/tg_botting/cooldowns.py` & `tg-botting-2.2.2/tg_botting/cooldowns.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.2.1/tg_botting/exceptions.py` & `tg-botting-2.2.2/tg_botting/exceptions.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.2.1/tg_botting/general.py` & `tg-botting-2.2.2/tg_botting/general.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.2.1/tg_botting/group.py` & `tg-botting-2.2.2/tg_botting/group.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.2.1/tg_botting/limiters.py` & `tg-botting-2.2.2/tg_botting/limiters.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.2.1/tg_botting/message.py` & `tg-botting-2.2.2/tg_botting/message.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.2.1/tg_botting/objects.py` & `tg-botting-2.2.2/tg_botting/objects.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.2.1/tg_botting/permissions.py` & `tg-botting-2.2.2/tg_botting/permissions.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.2.1/tg_botting/user.py` & `tg-botting-2.2.2/tg_botting/user.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.2.1/tg_botting/utils.py` & `tg-botting-2.2.2/tg_botting/utils.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.2.1/tg_botting/view.py` & `tg-botting-2.2.2/tg_botting/view.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.2.1/tg_botting.egg-info/PKG-INFO` & `tg-botting-2.2.2/tg_botting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 2.2.1
+Version: 2.2.2
 Summary: A basic package for building async TG bots
 Home-page: https://github.com/2sweetheart2/tg_botting
 Author: Sweetie (Roma Fomkin)
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `tg-botting-2.2.1/tg_botting.egg-info/SOURCES.txt` & `tg-botting-2.2.2/tg_botting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

