# Comparing `tmp/nonebot_adapter_kaiheila-0.2.7.tar.gz` & `tmp/nonebot_adapter_kaiheila-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_kaiheila-0.2.7.tar", max compression
+gzip compressed data, was "nonebot_adapter_kaiheila-0.2.8.tar", max compression
```

## Comparing `nonebot_adapter_kaiheila-0.2.7.tar` & `nonebot_adapter_kaiheila-0.2.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1065 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/LICENSE
--rw-r--r--   0        0        0      296 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/README.md
--rw-r--r--   0        0        0      359 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/__init__.py
--rw-r--r--   0        0        0    15919 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/adapter.py
--rw-r--r--   0        0        0       66 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/api/__init__.py
--rw-r--r--   0        0        0       27 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/api/client.py
--rw-r--r--   0        0        0    13589 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/api/client.pyi
--rw-r--r--   0        0        0     4223 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/api/handle.py
--rw-r--r--   0        0        0    12976 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/api/model.py
--rw-r--r--   0        0        0    12338 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/bot.py
--rw-r--r--   0        0        0      833 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/config.py
--rw-r--r--   0        0        0    28176 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/event.py
--rw-r--r--   0        0        0     3504 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/exception.py
--rw-r--r--   0        0        0    12822 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/message.py
--rw-r--r--   0        0        0      494 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/permission.py
--rw-r--r--   0        0        0     2437 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/utils.py
--rw-r--r--   0        0        0      749 2023-07-09 15:52:52.653429 nonebot_adapter_kaiheila-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     1090 1970-01-01 00:00:00.000000 nonebot_adapter_kaiheila-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-18 15:10:46.052547 nonebot_adapter_kaiheila-0.2.8/LICENSE
+-rw-r--r--   0        0        0      296 2023-07-18 15:10:46.052547 nonebot_adapter_kaiheila-0.2.8/README.md
+-rw-r--r--   0        0        0      359 2023-07-18 15:10:46.056547 nonebot_adapter_kaiheila-0.2.8/nonebot/adapters/kaiheila/__init__.py
+-rw-r--r--   0        0        0    15919 2023-07-18 15:10:46.056547 nonebot_adapter_kaiheila-0.2.8/nonebot/adapters/kaiheila/adapter.py
+-rw-r--r--   0        0        0       66 2023-07-18 15:10:46.056547 nonebot_adapter_kaiheila-0.2.8/nonebot/adapters/kaiheila/api/__init__.py
+-rw-r--r--   0        0        0       27 2023-07-18 15:10:46.056547 nonebot_adapter_kaiheila-0.2.8/nonebot/adapters/kaiheila/api/client.py
+-rw-r--r--   0        0        0    13589 2023-07-18 15:10:46.056547 nonebot_adapter_kaiheila-0.2.8/nonebot/adapters/kaiheila/api/client.pyi
+-rw-r--r--   0        0        0     4223 2023-07-18 15:10:46.056547 nonebot_adapter_kaiheila-0.2.8/nonebot/adapters/kaiheila/api/handle.py
+-rw-r--r--   0        0        0    12976 2023-07-18 15:10:46.056547 nonebot_adapter_kaiheila-0.2.8/nonebot/adapters/kaiheila/api/model.py
+-rw-r--r--   0        0        0    12338 2023-07-18 15:10:46.056547 nonebot_adapter_kaiheila-0.2.8/nonebot/adapters/kaiheila/bot.py
+-rw-r--r--   0        0        0      833 2023-07-18 15:10:46.056547 nonebot_adapter_kaiheila-0.2.8/nonebot/adapters/kaiheila/config.py
+-rw-r--r--   0        0        0    28176 2023-07-18 15:10:46.056547 nonebot_adapter_kaiheila-0.2.8/nonebot/adapters/kaiheila/event.py
+-rw-r--r--   0        0        0     3504 2023-07-18 15:10:46.056547 nonebot_adapter_kaiheila-0.2.8/nonebot/adapters/kaiheila/exception.py
+-rw-r--r--   0        0        0    12727 2023-07-18 15:10:46.056547 nonebot_adapter_kaiheila-0.2.8/nonebot/adapters/kaiheila/message.py
+-rw-r--r--   0        0        0      494 2023-07-18 15:10:46.056547 nonebot_adapter_kaiheila-0.2.8/nonebot/adapters/kaiheila/permission.py
+-rw-r--r--   0        0        0     2437 2023-07-18 15:10:46.056547 nonebot_adapter_kaiheila-0.2.8/nonebot/adapters/kaiheila/utils.py
+-rw-r--r--   0        0        0      749 2023-07-18 15:10:46.056547 nonebot_adapter_kaiheila-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     1090 1970-01-01 00:00:00.000000 nonebot_adapter_kaiheila-0.2.8/PKG-INFO
```

### Comparing `nonebot_adapter_kaiheila-0.2.7/LICENSE` & `nonebot_adapter_kaiheila-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/adapter.py` & `nonebot_adapter_kaiheila-0.2.8/nonebot/adapters/kaiheila/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/api/client.pyi` & `nonebot_adapter_kaiheila-0.2.8/nonebot/adapters/kaiheila/api/client.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/api/handle.py` & `nonebot_adapter_kaiheila-0.2.8/nonebot/adapters/kaiheila/api/handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/api/model.py` & `nonebot_adapter_kaiheila-0.2.8/nonebot/adapters/kaiheila/api/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/bot.py` & `nonebot_adapter_kaiheila-0.2.8/nonebot/adapters/kaiheila/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/config.py` & `nonebot_adapter_kaiheila-0.2.8/nonebot/adapters/kaiheila/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/event.py` & `nonebot_adapter_kaiheila-0.2.8/nonebot/adapters/kaiheila/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/exception.py` & `nonebot_adapter_kaiheila-0.2.8/nonebot/adapters/kaiheila/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/message.py` & `nonebot_adapter_kaiheila-0.2.8/nonebot/adapters/kaiheila/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,18 +93,15 @@
         if len(msg) != 1:
             raise UnsupportedMessageOperation("必须为纯文本段或 KMarkdown 段")
         else:
             return msg[0]
 
     @overrides(BaseMessageSegment)
     def is_text(self) -> bool:
-        if self.type == "kmarkdown":
-            return self.data["raw_content"] == self.data["content"]
-        else:
-            return self.type == "text"
+        return self.type == "text" or self.type == "kmarkdown"
 
     @staticmethod
     @deprecated("用 KMarkdown 语法 (met)用户id/here/all(met) 代替")
     def at(user_id: str) -> "MessageSegment":
         return MessageSegment.KMarkdown(f"(met){user_id}(met)", user_id)
 
     @staticmethod
```

### Comparing `nonebot_adapter_kaiheila-0.2.7/nonebot/adapters/kaiheila/utils.py` & `nonebot_adapter_kaiheila-0.2.8/nonebot/adapters/kaiheila/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.7/pyproject.toml` & `nonebot_adapter_kaiheila-0.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-kaiheila"
-version = "0.2.7"
+version = "0.2.8"
 description = "kaiheila adapter for nonebot2"
 authors = ["Tian-que <1605206150@qq.com>", "ssttkkl <huang.wen.long@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Tian-que/nonebot-adapter-kaiheila"
 keywords = ["bot", "khl", "kaiheila", "khlbot"]
```

### Comparing `nonebot_adapter_kaiheila-0.2.7/PKG-INFO` & `nonebot_adapter_kaiheila-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-kaiheila
-Version: 0.2.7
+Version: 0.2.8
 Summary: kaiheila adapter for nonebot2
 Home-page: https://github.com/Tian-que/nonebot-adapter-kaiheila
 License: MIT
 Keywords: bot,khl,kaiheila,khlbot
 Author: Tian-que
 Author-email: 1605206150@qq.com
 Requires-Python: >=3.9,<4.0
```

