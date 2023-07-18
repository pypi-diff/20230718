# Comparing `tmp/nonebot_adapter_villa-0.6.0.tar.gz` & `tmp/nonebot_adapter_villa-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_villa-0.6.0.tar", max compression
+gzip compressed data, was "nonebot_adapter_villa-0.6.1.tar", max compression
```

## Comparing `nonebot_adapter_villa-0.6.0.tar` & `nonebot_adapter_villa-0.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1062 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/LICENSE
--rw-r--r--   0        0        0     7323 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/README.md
--rw-r--r--   0        0        0      228 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/__init__.py
--rw-r--r--   0        0        0    12154 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/adapter.py
--rw-r--r--   0        0        0      114 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/api/__init__.py
--rw-r--r--   0        0        0       25 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/api/client.py
--rw-r--r--   0        0        0     3293 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/api/client.pyi
--rw-r--r--   0        0        0    13152 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/api/handle.py
--rw-r--r--   0        0        0     9488 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/api/models.py
--rw-r--r--   0        0        0     1734 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/api/request.py
--rw-r--r--   0        0        0    14561 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/bot.py
--rw-r--r--   0        0        0      713 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/config.py
--rw-r--r--   0        0        0    11808 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/event.py
--rw-r--r--   0        0        0     2717 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/exception.py
--rw-r--r--   0        0        0     9952 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/message.py
--rw-r--r--   0        0        0     1449 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/permission.py
--rw-r--r--   0        0        0       76 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/utils.py
--rw-r--r--   0        0        0     2125 2023-07-17 10:44:24.668774 nonebot_adapter_villa-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     8249 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-18 12:17:37.033620 nonebot_adapter_villa-0.6.1/LICENSE
+-rw-r--r--   0        0        0     7323 2023-07-18 12:17:37.033620 nonebot_adapter_villa-0.6.1/README.md
+-rw-r--r--   0        0        0      228 2023-07-18 12:17:37.033620 nonebot_adapter_villa-0.6.1/nonebot/adapters/villa/__init__.py
+-rw-r--r--   0        0        0    12154 2023-07-18 12:17:37.037620 nonebot_adapter_villa-0.6.1/nonebot/adapters/villa/adapter.py
+-rw-r--r--   0        0        0      114 2023-07-18 12:17:37.037620 nonebot_adapter_villa-0.6.1/nonebot/adapters/villa/api/__init__.py
+-rw-r--r--   0        0        0       25 2023-07-18 12:17:37.037620 nonebot_adapter_villa-0.6.1/nonebot/adapters/villa/api/client.py
+-rw-r--r--   0        0        0     3293 2023-07-18 12:17:37.037620 nonebot_adapter_villa-0.6.1/nonebot/adapters/villa/api/client.pyi
+-rw-r--r--   0        0        0    13152 2023-07-18 12:17:37.037620 nonebot_adapter_villa-0.6.1/nonebot/adapters/villa/api/handle.py
+-rw-r--r--   0        0        0     9488 2023-07-18 12:17:37.037620 nonebot_adapter_villa-0.6.1/nonebot/adapters/villa/api/models.py
+-rw-r--r--   0        0        0     1734 2023-07-18 12:17:37.037620 nonebot_adapter_villa-0.6.1/nonebot/adapters/villa/api/request.py
+-rw-r--r--   0        0        0    14467 2023-07-18 12:17:37.037620 nonebot_adapter_villa-0.6.1/nonebot/adapters/villa/bot.py
+-rw-r--r--   0        0        0     1168 2023-07-18 12:17:37.037620 nonebot_adapter_villa-0.6.1/nonebot/adapters/villa/config.py
+-rw-r--r--   0        0        0    12798 2023-07-18 12:17:37.037620 nonebot_adapter_villa-0.6.1/nonebot/adapters/villa/event.py
+-rw-r--r--   0        0        0     2717 2023-07-18 12:17:37.037620 nonebot_adapter_villa-0.6.1/nonebot/adapters/villa/exception.py
+-rw-r--r--   0        0        0     9952 2023-07-18 12:17:37.037620 nonebot_adapter_villa-0.6.1/nonebot/adapters/villa/message.py
+-rw-r--r--   0        0        0     1449 2023-07-18 12:17:37.037620 nonebot_adapter_villa-0.6.1/nonebot/adapters/villa/permission.py
+-rw-r--r--   0        0        0       76 2023-07-18 12:17:37.037620 nonebot_adapter_villa-0.6.1/nonebot/adapters/villa/utils.py
+-rw-r--r--   0        0        0     2125 2023-07-18 12:17:37.037620 nonebot_adapter_villa-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     8249 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.6.1/PKG-INFO
```

### Comparing `nonebot_adapter_villa-0.6.0/LICENSE` & `nonebot_adapter_villa-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.0/README.md` & `nonebot_adapter_villa-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/adapter.py` & `nonebot_adapter_villa-0.6.1/nonebot/adapters/villa/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/api/client.pyi` & `nonebot_adapter_villa-0.6.1/nonebot/adapters/villa/api/client.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/api/handle.py` & `nonebot_adapter_villa-0.6.1/nonebot/adapters/villa/api/handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/api/models.py` & `nonebot_adapter_villa-0.6.1/nonebot/adapters/villa/api/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/api/request.py` & `nonebot_adapter_villa-0.6.1/nonebot/adapters/villa/api/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/bot.py` & `nonebot_adapter_villa-0.6.1/nonebot/adapters/villa/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,24 +36,25 @@
 from .message import Message, MessageSegment
 from .utils import log
 
 if TYPE_CHECKING:
     from .adapter import Adapter
 
 
-async def _check_reply(bot: "Bot", event: SendMessageEvent):
-    """检查事件是否有引用消息，如果有则设置 reply 字段。
-
-    但是目前并没有API能获取被引用的消息的内容，所以现在不做。
+def _check_reply(bot: "Bot", event: SendMessageEvent):
+    """检查事件是否有引用消息，如果有则删除。
 
     参数:
         bot: Bot对象
         event: 事件
     """
-    ...
+    if event.content.quote is not None:
+        event.message = event.message.exclude("quote")
+    if not event.message:
+        event.message.append(MessageSegment.text(""))
 
 
 def _check_at_me(bot: "Bot", event: SendMessageEvent):
     """检查事件是否和机器人有关，如果有关则设置 to_me 为 True，并删除消息中的 at 信息。
 
     参数:
         bot: Bot对象
@@ -167,15 +168,15 @@
             raise ValueError(f"Bot {self.self_id} hasn't received any events yet.")
         return self._bot_info.villa_id
 
     async def handle_event(self, event: Event):
         """处理事件"""
         if isinstance(event, SendMessageEvent):
             _check_at_me(self, event)
-            # await _check_reply(self, event)
+            _check_reply(self, event)
         await handle_event(self, event)
 
     def _verify_signature(
         self,
         body: str,
         bot_sign: str,
     ):
@@ -232,19 +233,15 @@
             raise RuntimeError("Event cannot be replied to!")
         message = MessageSegment.text(message) if isinstance(message, str) else message
         message = message if isinstance(message, Message) else Message(message)
         if kwargs.pop("mention_sender", False) or kwargs.pop("at_sender", False):
             message.insert(
                 0,
                 MessageSegment.mention_user(
-                    user_id=(
-                        event.from_user_id
-                        if isinstance(event, SendMessageEvent)
-                        else event.uid
-                    ),
+                    user_id=int(event.get_user_id()),
                     user_name=(
                         event.content.user.name
                         if isinstance(event, SendMessageEvent)
                         else None
                     ),
                     villa_id=event.villa_id,
                 ),
```

### Comparing `nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/event.py` & `nonebot_adapter_villa-0.6.1/nonebot/adapters/villa/event.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
     @override
     def get_user_id(self) -> str:
         raise ValueError("Event has no context!")
 
     @override
     def get_session_id(self) -> str:
-        raise ValueError("Event has no context!")
+        return f"{self.robot.villa_id}_{self.id}"
 
     @override
     def is_tome(self) -> bool:
         return False
 
 
 class NoticeEvent(Event):
@@ -125,15 +125,15 @@
 
     @override
     def get_user_id(self) -> str:
         return str(self.join_uid)
 
     @override
     def get_session_id(self) -> str:
-        return str(self.join_uid)
+        return f"{self.villa_id}_{self.join_uid}"
 
 
 class SendMessageEvent(MessageEvent):
     """用户@机器人发送消息事件
 
     see https://webstatic.mihoyo.com/vila/bot/doc/callback.html###SendMessage"""
 
@@ -192,15 +192,15 @@
     def get_user_id(self) -> str:
         """获取用户ID"""
         return str(self.from_user_id)
 
     @override
     def get_session_id(self) -> str:
         """获取会话ID"""
-        return f"{self.room_id}-{self.from_user_id}"
+        return f"{self.villa_id}_{self.room_id}_{self.from_user_id}"
 
     @root_validator(pre=True)
     @classmethod
     def _(cls, data: Dict[str, Any]):
         if not data.get("content"):
             return data
         msg = Message()
@@ -289,14 +289,22 @@
 
     @override
     def get_event_description(self) -> str:
         return escape_tag(
             f"Bot(id={self.bot_id}) was added to Villa(id={self.villa_id})",
         )
 
+    @override
+    def is_tome(self) -> bool:
+        return True
+
+    @override
+    def get_session_id(self) -> str:
+        return f"{self.villa_id}_{self.bot_id}"
+
 
 class DeleteRobotEvent(NoticeEvent):
     """大别野删除机器人实例事件
 
     see https://webstatic.mihoyo.com/vila/bot/doc/callback.html###DeleteRobot"""
 
     type: Literal[EventType.DeleteRobot] = EventType.DeleteRobot
@@ -305,14 +313,22 @@
 
     @override
     def get_event_description(self) -> str:
         return escape_tag(
             f"Bot(id={self.bot_id}) was removed from Villa(id={self.villa_id})",
         )
 
+    @override
+    def is_tome(self) -> bool:
+        return True
+
+    @override
+    def get_session_id(self) -> str:
+        return f"{self.villa_id}_{self.bot_id}"
+
 
 class AddQuickEmoticonEvent(NoticeEvent):
     """用户使用表情回复消息表态事件
 
     see https://webstatic.mihoyo.com/vila/bot/doc/callback.html#AddQuickEmoticon"""
 
     type: Literal[EventType.AddQuickEmoticon] = EventType.AddQuickEmoticon
@@ -330,14 +346,29 @@
     """被回复的消息 id"""
     bot_msg_id: Optional[str]
     """如果被回复的消息从属于机器人，则该字段不为空字符串"""
     is_cancel: bool = False
     """是否是取消表情"""
 
     @override
+    def get_user_id(self) -> str:
+        return str(self.uid)
+
+    @override
+    def is_tome(self) -> bool:
+        return True
+
+    @override
+    def get_session_id(self) -> str:
+        return (
+            f"{self.villa_id}_{self.room_id}_{self.uid}"
+            f"_{self.emoticon_id}_{self.is_cancel}"
+        )
+
+    @override
     def get_event_description(self) -> str:
         return escape_tag(
             (
                 f"Emoticon(name={self.emoticon}, id={self.emoticon_id}) was "
                 f"{'removed from' if self.is_cancel else 'added to'} "
                 f"Message(id={self.msg_uid}) by User(id={self.uid}) in "
                 f"Room(id=Villa(id={self.room_id}) of Villa(id={self.villa_id})"
@@ -363,14 +394,26 @@
     """用户 id（和审核接口调用方传入的值一致）"""
     pass_through: str
     """透传数据（和审核接口调用方传入的值一致）"""
     audit_result: AuditResult
     """审核结果"""
 
     @override
+    def get_user_id(self) -> str:
+        return str(self.user_id)
+
+    @override
+    def is_tome(self) -> bool:
+        return self.bot_id == self.bot_tpl_id
+
+    @override
+    def get_session_id(self) -> str:
+        return f"{self.villa_id}_{self.bot_tpl_id}_{self.audit_id}"
+
+    @override
     def get_event_description(self) -> str:
         return escape_tag(
             (
                 f"Audit(id={self.audit_id},result={self.audit_result}) of "
                 f"User(id={self.user_id}) in Room(id={self.room_id}) of "
                 f"Villa(id={self.villa_id})"
             ),
```

### Comparing `nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/exception.py` & `nonebot_adapter_villa-0.6.1/nonebot/adapters/villa/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/message.py` & `nonebot_adapter_villa-0.6.1/nonebot/adapters/villa/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.0/nonebot/adapters/villa/permission.py` & `nonebot_adapter_villa-0.6.1/nonebot/adapters/villa/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.6.0/pyproject.toml` & `nonebot_adapter_villa-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-villa"
-version = "0.6.0"
+version = "0.6.1"
 description = "NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 repository = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 documentation = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
```

### Comparing `nonebot_adapter_villa-0.6.0/PKG-INFO` & `nonebot_adapter_villa-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-villa
-Version: 0.6.0
+Version: 0.6.1
 Summary: NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa
 License: MIT
 Keywords: nonebot,mihoyo,bot
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.6.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.6.1 Summary:
 NoneBot2ç±³æ¸¸ç¤¾å¤§å«éBotééå¨ãMiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa License: MIT
 Keywords: nonebot,mihoyo,bot Author: CMHopeSunshine Author-email:
 277073121@qq.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

