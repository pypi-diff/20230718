# Comparing `tmp/hrbot-0.1.3.tar.gz` & `tmp/hrbot-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hrbot-0.1.3.tar", max compression
+gzip compressed data, was "hrbot-0.1.4.tar", max compression
```

## Comparing `hrbot-0.1.3.tar` & `hrbot-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      158 2023-06-15 08:01:29.191231 hrbot-0.1.3/hrbot/__init__.py
--rw-r--r--   0        0        0       31 2023-05-18 14:31:32.146814 hrbot-0.1.3/hrbot/bot/__init__.py
--rw-r--r--   0        0        0      988 2023-06-15 08:48:39.851385 hrbot-0.1.3/hrbot/bot/base.py
--rw-r--r--   0        0        0     3774 2023-07-01 12:31:29.301795 hrbot-0.1.3/hrbot/bot/bot.py
--rw-r--r--   0        0        0       59 2023-05-18 14:31:32.138854 hrbot-0.1.3/hrbot/dispatcher/__init__.py
--rw-r--r--   0        0        0     9653 2023-07-01 12:29:57.935681 hrbot-0.1.3/hrbot/dispatcher/__pycache__/dispatсher.cpython-311.pyc
--rw-r--r--   0        0        0     6433 2023-07-01 12:29:57.520228 hrbot-0.1.3/hrbot/dispatcher/dispatсher.py
--rw-r--r--   0        0        0    10692 2023-07-01 12:29:57.528779 hrbot-0.1.3/hrbot/dispatcher/filter.py
--rw-r--r--   0        0        0       30 2023-05-31 10:19:08.115326 hrbot-0.1.3/hrbot/dispatcher/fsm/__init__.py
--rw-r--r--   0        0        0     1972 2023-06-15 09:02:33.436860 hrbot-0.1.3/hrbot/dispatcher/fsm/state.py
--rw-r--r--   0        0        0     4675 2023-06-14 06:55:24.164338 hrbot-0.1.3/hrbot/dispatcher/fsm/storage.py
--rw-r--r--   0        0        0     1337 2023-06-14 07:07:30.601511 hrbot-0.1.3/hrbot/dispatcher/handler.py
--rw-r--r--   0        0        0      284 2023-06-11 09:43:38.740611 hrbot-0.1.3/hrbot/types/__init__.py
--rw-r--r--   0        0        0      402 2023-06-19 02:47:45.500862 hrbot-0.1.3/hrbot/types/handler.py
--rw-r--r--   0        0        0       31 2023-05-14 15:25:08.437975 hrbot-0.1.3/hrbot/types/hr.py
--rw-r--r--   0        0        0        0 2023-05-14 13:14:36.307325 hrbot-0.1.3/hrbot/utils/__init__.py
--rw-r--r--   0        0        0     1084 2023-06-18 13:15:36.011849 hrbot-0.1.3/LICENSE
--rw-r--r--   0        0        0      459 2023-07-01 05:33:00.474819 hrbot-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1612 2023-07-01 05:33:00.485987 hrbot-0.1.3/README.md
--rw-r--r--   0        0        0     2145 1970-01-01 00:00:00.000000 hrbot-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      158 2023-06-15 08:01:29.191231 hrbot-0.1.4/hrbot/__init__.py
+-rw-r--r--   0        0        0       31 2023-05-18 14:31:32.146814 hrbot-0.1.4/hrbot/bot/__init__.py
+-rw-r--r--   0        0        0      988 2023-06-15 08:48:39.851385 hrbot-0.1.4/hrbot/bot/base.py
+-rw-r--r--   0        0        0     3774 2023-07-01 12:31:29.301795 hrbot-0.1.4/hrbot/bot/bot.py
+-rw-r--r--   0        0        0       59 2023-05-18 14:31:32.138854 hrbot-0.1.4/hrbot/dispatcher/__init__.py
+-rw-r--r--   0        0        0     9653 2023-07-01 12:29:57.935681 hrbot-0.1.4/hrbot/dispatcher/__pycache__/dispatсher.cpython-311.pyc
+-rw-r--r--   0        0        0     6433 2023-07-01 12:29:57.520228 hrbot-0.1.4/hrbot/dispatcher/dispatсher.py
+-rw-r--r--   0        0        0    10692 2023-07-01 12:29:57.528779 hrbot-0.1.4/hrbot/dispatcher/filter.py
+-rw-r--r--   0        0        0       30 2023-05-31 10:19:08.115326 hrbot-0.1.4/hrbot/dispatcher/fsm/__init__.py
+-rw-r--r--   0        0        0     1972 2023-06-15 09:02:33.436860 hrbot-0.1.4/hrbot/dispatcher/fsm/state.py
+-rw-r--r--   0        0        0     4675 2023-06-14 06:55:24.164338 hrbot-0.1.4/hrbot/dispatcher/fsm/storage.py
+-rw-r--r--   0        0        0     1337 2023-06-14 07:07:30.601511 hrbot-0.1.4/hrbot/dispatcher/handler.py
+-rw-r--r--   0        0        0      284 2023-06-11 09:43:38.740611 hrbot-0.1.4/hrbot/types/__init__.py
+-rw-r--r--   0        0        0      402 2023-06-19 02:47:45.500862 hrbot-0.1.4/hrbot/types/handler.py
+-rw-r--r--   0        0        0       31 2023-05-14 15:25:08.437975 hrbot-0.1.4/hrbot/types/hr.py
+-rw-r--r--   0        0        0        0 2023-05-14 13:14:36.307325 hrbot-0.1.4/hrbot/utils/__init__.py
+-rw-r--r--   0        0        0     1084 2023-06-18 13:15:36.011849 hrbot-0.1.4/LICENSE
+-rw-r--r--   0        0        0      456 2023-07-18 05:59:03.515420 hrbot-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1612 2023-07-01 05:33:00.485987 hrbot-0.1.4/README.md
+-rw-r--r--   0        0        0     2142 1970-01-01 00:00:00.000000 hrbot-0.1.4/PKG-INFO
```

### Comparing `hrbot-0.1.3/hrbot/bot/base.py` & `hrbot-0.1.4/hrbot/bot/base.py`

 * *Files identical despite different names*

### Comparing `hrbot-0.1.3/hrbot/bot/bot.py` & `hrbot-0.1.4/hrbot/bot/bot.py`

 * *Files identical despite different names*

### Comparing `hrbot-0.1.3/hrbot/dispatcher/__pycache__/dispatсher.cpython-311.pyc` & `hrbot-0.1.4/hrbot/dispatcher/__pycache__/dispatсher.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hrbot-0.1.3/hrbot/dispatcher/dispatсher.py` & `hrbot-0.1.4/hrbot/dispatcher/dispatсher.py`

 * *Files identical despite different names*

### Comparing `hrbot-0.1.3/hrbot/dispatcher/filter.py` & `hrbot-0.1.4/hrbot/dispatcher/filter.py`

 * *Files identical despite different names*

### Comparing `hrbot-0.1.3/hrbot/dispatcher/fsm/state.py` & `hrbot-0.1.4/hrbot/dispatcher/fsm/state.py`

 * *Files identical despite different names*

### Comparing `hrbot-0.1.3/hrbot/dispatcher/fsm/storage.py` & `hrbot-0.1.4/hrbot/dispatcher/fsm/storage.py`

 * *Files identical despite different names*

### Comparing `hrbot-0.1.3/hrbot/dispatcher/handler.py` & `hrbot-0.1.4/hrbot/dispatcher/handler.py`

 * *Files identical despite different names*

### Comparing `hrbot-0.1.3/LICENSE` & `hrbot-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hrbot-0.1.3/README.md` & `hrbot-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `hrbot-0.1.3/PKG-INFO` & `hrbot-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: hrbot
-Version: 0.1.3
+Version: 0.1.4
 Summary: The hrbot is a wrapper on top of the HighRise Python Bot SDK that makes it easy to create bots in HighRise.
 License: MIT
 Author: MuoDosta
 Author-email: MuoDostaWork@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: highrise-bot-sdk (==23.1.0b15)
+Requires-Dist: highrise-bot-sdk (==23.3.0)
 Requires-Dist: redis (==4.5.5)
 Description-Content-Type: text/markdown
 
 
 # The hrbot  
 The hrbot is a wrapper on top of the [HighRise Python Bot SDK](https://github.com/pocketzworld/python-bot-sdk) that makes it easy to create bots in [HighRise](https://highrise.game/).
```

