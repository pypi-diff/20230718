# Comparing `tmp/tg-botting-2.1.7.tar.gz` & `tmp/tg-botting-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg-botting-2.1.7.tar", last modified: Tue Jul 18 12:12:12 2023, max compression
+gzip compressed data, was "tg-botting-2.1.8.tar", last modified: Tue Jul 18 13:24:23 2023, max compression
```

## Comparing `tg-botting-2.1.7.tar` & `tg-botting-2.1.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 12:12:12.388265 tg-botting-2.1.7/
--rw-rw-rw-   0        0        0     3407 2023-07-18 12:12:12.388265 tg-botting-2.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1709 2023-07-12 19:32:58.000000 tg-botting-2.1.7/README.md
--rw-rw-rw-   0        0        0       42 2023-07-18 12:12:12.388265 tg-botting-2.1.7/setup.cfg
--rw-rw-rw-   0        0        0     2624 2023-07-12 19:37:56.000000 tg-botting-2.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 12:12:12.383252 tg-botting-2.1.7/tg_botting/
--rw-rw-rw-   0        0        0      798 2023-07-18 12:11:27.000000 tg-botting-2.1.7/tg_botting/__init__.py
--rw-rw-rw-   0        0        0       39 2023-05-26 21:28:31.000000 tg-botting-2.1.7/tg_botting/_types.py
--rw-rw-rw-   0        0        0      730 2023-07-13 11:59:36.000000 tg-botting-2.1.7/tg_botting/abstract.py
--rw-rw-rw-   0        0        0    19269 2023-07-12 16:28:14.000000 tg-botting-2.1.7/tg_botting/bot.py
--rw-rw-rw-   0        0        0    31649 2023-07-18 12:11:06.000000 tg-botting-2.1.7/tg_botting/client.py
--rw-rw-rw-   0        0        0    12615 2023-05-26 21:34:31.000000 tg-botting-2.1.7/tg_botting/cog.py
--rw-rw-rw-   0        0        0    35621 2023-05-26 21:39:01.000000 tg-botting-2.1.7/tg_botting/commands.py
--rw-rw-rw-   0        0        0     3635 2023-07-13 11:59:36.000000 tg-botting-2.1.7/tg_botting/context.py
--rw-rw-rw-   0        0        0     1361 2023-05-26 21:43:21.000000 tg-botting-2.1.7/tg_botting/context_managers.py
--rw-rw-rw-   0        0        0     1410 2023-05-26 21:35:15.000000 tg-botting-2.1.7/tg_botting/conversions.py
--rw-rw-rw-   0        0        0     3679 2023-05-26 21:31:45.000000 tg-botting-2.1.7/tg_botting/cooldowns.py
--rw-rw-rw-   0        0        0    10433 2023-05-26 21:27:27.000000 tg-botting-2.1.7/tg_botting/exceptions.py
--rw-rw-rw-   0        0        0      902 2023-05-27 14:01:15.000000 tg-botting-2.1.7/tg_botting/general.py
--rw-rw-rw-   0        0        0     9737 2023-05-27 13:35:03.000000 tg-botting-2.1.7/tg_botting/group.py
--rw-rw-rw-   0        0        0      578 2023-07-14 23:30:00.000000 tg-botting-2.1.7/tg_botting/limiters.py
--rw-rw-rw-   0        0        0    18252 2023-07-15 15:34:44.000000 tg-botting-2.1.7/tg_botting/message.py
--rw-rw-rw-   0        0        0    33413 2023-07-14 22:47:31.000000 tg-botting-2.1.7/tg_botting/objects.py
--rw-rw-rw-   0        0        0     3037 2023-07-11 21:05:01.000000 tg-botting-2.1.7/tg_botting/permissions.py
--rw-rw-rw-   0        0        0     1919 2023-07-12 15:17:24.000000 tg-botting-2.1.7/tg_botting/user.py
--rw-rw-rw-   0        0        0     1023 2023-07-13 22:59:13.000000 tg-botting-2.1.7/tg_botting/utils.py
--rw-rw-rw-   0        0        0     4368 2023-05-26 21:44:26.000000 tg-botting-2.1.7/tg_botting/view.py
-drwxrwxrwx   0        0        0        0 2023-07-18 12:12:12.387243 tg-botting-2.1.7/tg_botting.egg-info/
--rw-rw-rw-   0        0        0     3407 2023-07-18 12:12:12.000000 tg-botting-2.1.7/tg_botting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      655 2023-07-18 12:12:12.000000 tg-botting-2.1.7/tg_botting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 12:12:12.000000 tg-botting-2.1.7/tg_botting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-07-18 12:12:12.000000 tg-botting-2.1.7/tg_botting.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-18 12:12:12.000000 tg-botting-2.1.7/tg_botting.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 13:24:23.681742 tg-botting-2.1.8/
+-rw-rw-rw-   0        0        0     3407 2023-07-18 13:24:23.680745 tg-botting-2.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1709 2023-07-12 19:32:58.000000 tg-botting-2.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-18 13:24:23.681742 tg-botting-2.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     2624 2023-07-12 19:37:56.000000 tg-botting-2.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:24:23.675758 tg-botting-2.1.8/tg_botting/
+-rw-rw-rw-   0        0        0      798 2023-07-18 13:24:02.000000 tg-botting-2.1.8/tg_botting/__init__.py
+-rw-rw-rw-   0        0        0       39 2023-05-26 21:28:31.000000 tg-botting-2.1.8/tg_botting/_types.py
+-rw-rw-rw-   0        0        0      730 2023-07-13 11:59:36.000000 tg-botting-2.1.8/tg_botting/abstract.py
+-rw-rw-rw-   0        0        0    19269 2023-07-12 16:28:14.000000 tg-botting-2.1.8/tg_botting/bot.py
+-rw-rw-rw-   0        0        0    31835 2023-07-18 13:24:02.000000 tg-botting-2.1.8/tg_botting/client.py
+-rw-rw-rw-   0        0        0    12615 2023-05-26 21:34:31.000000 tg-botting-2.1.8/tg_botting/cog.py
+-rw-rw-rw-   0        0        0    35621 2023-05-26 21:39:01.000000 tg-botting-2.1.8/tg_botting/commands.py
+-rw-rw-rw-   0        0        0     3635 2023-07-13 11:59:36.000000 tg-botting-2.1.8/tg_botting/context.py
+-rw-rw-rw-   0        0        0     1361 2023-05-26 21:43:21.000000 tg-botting-2.1.8/tg_botting/context_managers.py
+-rw-rw-rw-   0        0        0     1410 2023-05-26 21:35:15.000000 tg-botting-2.1.8/tg_botting/conversions.py
+-rw-rw-rw-   0        0        0     3679 2023-05-26 21:31:45.000000 tg-botting-2.1.8/tg_botting/cooldowns.py
+-rw-rw-rw-   0        0        0    10433 2023-05-26 21:27:27.000000 tg-botting-2.1.8/tg_botting/exceptions.py
+-rw-rw-rw-   0        0        0      902 2023-05-27 14:01:15.000000 tg-botting-2.1.8/tg_botting/general.py
+-rw-rw-rw-   0        0        0     9737 2023-05-27 13:35:03.000000 tg-botting-2.1.8/tg_botting/group.py
+-rw-rw-rw-   0        0        0      578 2023-07-14 23:30:00.000000 tg-botting-2.1.8/tg_botting/limiters.py
+-rw-rw-rw-   0        0        0    18252 2023-07-15 15:34:44.000000 tg-botting-2.1.8/tg_botting/message.py
+-rw-rw-rw-   0        0        0    33413 2023-07-14 22:47:31.000000 tg-botting-2.1.8/tg_botting/objects.py
+-rw-rw-rw-   0        0        0     3037 2023-07-11 21:05:01.000000 tg-botting-2.1.8/tg_botting/permissions.py
+-rw-rw-rw-   0        0        0     1919 2023-07-12 15:17:24.000000 tg-botting-2.1.8/tg_botting/user.py
+-rw-rw-rw-   0        0        0     1023 2023-07-13 22:59:13.000000 tg-botting-2.1.8/tg_botting/utils.py
+-rw-rw-rw-   0        0        0     4368 2023-05-26 21:44:26.000000 tg-botting-2.1.8/tg_botting/view.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:24:23.679748 tg-botting-2.1.8/tg_botting.egg-info/
+-rw-rw-rw-   0        0        0     3407 2023-07-18 13:24:23.000000 tg-botting-2.1.8/tg_botting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      655 2023-07-18 13:24:23.000000 tg-botting-2.1.8/tg_botting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 13:24:23.000000 tg-botting-2.1.8/tg_botting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-07-18 13:24:23.000000 tg-botting-2.1.8/tg_botting.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-18 13:24:23.000000 tg-botting-2.1.8/tg_botting.egg-info/top_level.txt
```

### Comparing `tg-botting-2.1.7/PKG-INFO` & `tg-botting-2.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 2.1.7
+Version: 2.1.8
 Summary: A basic package for building async TG bots
 Home-page: https://github.com/2sweetheart2/tg_botting
 Author: Sweetie (Roma Fomkin)
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `tg-botting-2.1.7/README.md` & `tg-botting-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.7/setup.py` & `tg-botting-2.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.7/tg_botting/__init__.py` & `tg-botting-2.1.8/tg_botting/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 _title__ = 'tg_botting'
 __author__ = 'Sweetie'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023-present Sweetie'
-__version__ = '2.1.7'
+__version__ = '2.1.8'
 
 from collections import namedtuple
 import logging
 
 from .bot import Bot
 from .limiters import *
 from .conversions import Converter
```

### Comparing `tg-botting-2.1.7/tg_botting/abstract.py` & `tg-botting-2.1.8/tg_botting/abstract.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.7/tg_botting/bot.py` & `tg-botting-2.1.8/tg_botting/bot.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.7/tg_botting/client.py` & `tg-botting-2.1.8/tg_botting/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import asyncio
 import enum
+import json
 import sys
 import textwrap
 import traceback
 import typing
 from typing import TypeVar
 import datetime
 import aiohttp
 
 from tg_botting.exceptions import TGException, TGApiError, BadArgument
 from tg_botting.general import convert_params
-from tg_botting.message import Chat, Message, CallbackQuery
+from tg_botting.message import Chat, Message, CallbackQuery, ChatJoinRequest, ChatJoinRequest
 from tg_botting.objects import get_chat_member, MessageEntity, InlineKeyboardMarkup, ReplyKeyboardMarkup, \
-    ReplyKeyboardRemove
+    ReplyKeyboardRemove, InlineQuery, ChosenInlineResult, ShippingQuery, PreCheckoutQuery, Poll,PollAnswer
+
 from tg_botting.user import User
 from tg_botting.utils import to_json, maybe_coroutine
 
+
+
 String = TypeVar('String', bound=str)
 Integer = TypeVar('Integer', bound=int)
 Float = TypeVar('Float', bound=float)
 Boolean = TypeVar('Boolean', bound=bool)
 T = TypeVar('T')
 
 class UserMessageFlags(enum.IntFlag):
@@ -292,15 +296,14 @@
         if self.offset is None:
             self.offset = 0
         payload = {'offset': self.offset}
         try:
             res = await self.general_request(self.generate_link("getUpdates"), **payload)
         except asyncio.TimeoutError:
             return self.offset, []
-
         if res['ok'] is False:
             self.offset = 0
         elif len(res['result']) != 0:
             self.offset = res['result'][len(res['result']) - 1]['update_id']+1
         updates = res['result']
         return self.offset, updates
 
@@ -323,19 +326,17 @@
             action = "poll_new"
         elif msg.left_chat_member is not None:
             action = "chat_member_left"
         elif msg.photo is not None:
             action = "photo_new"
         elif msg.new_chat_members is not None:
             action = 'new_chat_members'
-        elif msg.left_chat_member is not None:
-            action = 'left_chat_member'
         elif msg.successful_payment is not None:
             action = "successful_payment"
-
+        print(f'ACTION: {action}')
         if action is not None:
             return self.dispatch(action, msg)
         if msg.text is None:
             return self.dispatch("something_without_text",msg)
         return self.dispatch('message_new', msg)
 
     def handle_callback_query(self, t, obj):
@@ -352,22 +353,25 @@
         return self.dispatch(t, msg)
 
     def handle_message_edit(self, t, obj):
         msg = self.build_msg(obj)
         return self.dispatch(t, msg)
 
     def handle_custom_classes(self, t, obj, update):
+        print(t)
         names = t.split("_")
         name = [r.title() for r in names]
         class_name = ''.join(name)
-
+        print(class_name)
+        print()
         if class_name not in globals():
             return self.dispatch('unknown', update)
-
+        print('FIND CLASS')
         klass = globals()[class_name]
+        print(obj)
         instance = klass(obj)
         return self.dispatch(t, instance)
 
     def check_date(self, message):
         date = datetime.datetime.now() - datetime.timedelta(seconds=5)
         return message.date > date
```

### Comparing `tg-botting-2.1.7/tg_botting/cog.py` & `tg-botting-2.1.8/tg_botting/cog.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.7/tg_botting/commands.py` & `tg-botting-2.1.8/tg_botting/commands.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.7/tg_botting/context.py` & `tg-botting-2.1.8/tg_botting/context.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.7/tg_botting/context_managers.py` & `tg-botting-2.1.8/tg_botting/context_managers.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.7/tg_botting/conversions.py` & `tg-botting-2.1.8/tg_botting/conversions.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.7/tg_botting/cooldowns.py` & `tg-botting-2.1.8/tg_botting/cooldowns.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.7/tg_botting/exceptions.py` & `tg-botting-2.1.8/tg_botting/exceptions.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.7/tg_botting/general.py` & `tg-botting-2.1.8/tg_botting/general.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.7/tg_botting/group.py` & `tg-botting-2.1.8/tg_botting/group.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.7/tg_botting/limiters.py` & `tg-botting-2.1.8/tg_botting/limiters.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.7/tg_botting/message.py` & `tg-botting-2.1.8/tg_botting/message.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.7/tg_botting/objects.py` & `tg-botting-2.1.8/tg_botting/objects.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.7/tg_botting/permissions.py` & `tg-botting-2.1.8/tg_botting/permissions.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.7/tg_botting/user.py` & `tg-botting-2.1.8/tg_botting/user.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.7/tg_botting/utils.py` & `tg-botting-2.1.8/tg_botting/utils.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.7/tg_botting/view.py` & `tg-botting-2.1.8/tg_botting/view.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.7/tg_botting.egg-info/PKG-INFO` & `tg-botting-2.1.8/tg_botting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 2.1.7
+Version: 2.1.8
 Summary: A basic package for building async TG bots
 Home-page: https://github.com/2sweetheart2/tg_botting
 Author: Sweetie (Roma Fomkin)
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `tg-botting-2.1.7/tg_botting.egg-info/SOURCES.txt` & `tg-botting-2.1.8/tg_botting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

