# Comparing `tmp/openai2-1.5.11.1.tar.gz` & `tmp/openai2-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai2-1.5.11.1.tar", last modified: Sat Jul 15 22:39:09 2023, max compression
+gzip compressed data, was "openai2-1.6.tar", last modified: Tue Jul 18 11:57:20 2023, max compression
```

## Comparing `openai2-1.5.11.1.tar` & `openai2-1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11038 2023-07-14 17:01:09.603744 openai2-1.5.11.1/LICENSE
--rw-r--r--   0        0        0     8727 2023-07-15 21:54:22.320236 openai2-1.5.11.1/README.md
--rw-r--r--   0        0        0     1083 2020-12-22 18:45:03.000000 openai2-1.5.11.1/openai2/Dependent Packages/openai/LICENSE
--rw-r--r--   0        0        0       56 2023-07-15 11:05:31.162471 openai2-1.5.11.1/openai2/__init__.py
--rw-r--r--   0        0        0     5434 2023-07-15 14:06:17.992651 openai2-1.5.11.1/openai2/_core.py
--rw-r--r--   0        0        0      677 2023-07-15 22:37:51.645148 openai2-1.5.11.1/pyproject.toml
--rw-r--r--   0        0        0     8991 1970-01-01 00:00:00.000000 openai2-1.5.11.1/PKG-INFO
+-rw-r--r--   0        0        0    11038 2023-07-14 17:01:09.603744 openai2-1.6/LICENSE
+-rw-r--r--   0        0        0     9020 2023-07-18 11:54:29.565377 openai2-1.6/README.md
+-rw-r--r--   0        0        0     1083 2020-12-22 18:45:03.000000 openai2-1.6/openai2/Dependent Packages/openai/LICENSE
+-rw-r--r--   0        0        0       56 2023-07-18 11:42:34.392010 openai2-1.6/openai2/__init__.py
+-rw-r--r--   0        0        0     6078 2023-07-18 11:43:42.876678 openai2-1.6/openai2/_core.py
+-rw-r--r--   0        0        0      668 2023-07-18 11:56:46.739518 openai2-1.6/pyproject.toml
+-rw-r--r--   0        0        0     9260 1970-01-01 00:00:00.000000 openai2-1.6/PKG-INFO
```

### Comparing `openai2-1.5.11.1/LICENSE` & `openai2-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `openai2-1.5.11.1/README.md` & `openai2-1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # 项目描述
 
-一个用来调用 ChatGPT 的工具，支持连续对话、对话存档与载入、对话回滚、对话伪造、轮询 api_key 池、限制历史消息数量。
+ChatGPT 工具包，支持连续对话、对话存档与载入、对话回滚、对话伪造、轮询 api_key 池、限制历史消息数量、异步请求。
 
 # 关于作者
 
 作者：lcctoor.com
 
 域名：lcctoor.com
 
@@ -117,23 +117,23 @@
 Denny = Chat(api_key=AK2, model="gpt-3.5-turbo")
 Chris = Chat(api_key=AK3, model="gpt-3.5-turbo")  # 令 Chris 使用独立的'api_key池'
 Dick = Chat(api_key=AK4, model="gpt-3.5-turbo")  # 令 Dick 使用独立的'api_key池'
 ```
 
 注：允许（而非不允许）同一个 api_key 投放到不同的 api_key 池中，但每个 api_key 池都是独立调度，不会互相通信。
 
-#### 修改 api_key
+#### 重置 api_key
 
 ```python
 AK5 = 'sk-jg93...'
 AK6 = AKPool(['sk-vb7l...', 'sk-d3lv...'])
 ...
 
-Carl.reset_api_key(AK5)  # 修改 api_key
-Carl.reset_api_key(AK6)  # 再次修改 api_key
+Carl.reset_api_key(AK5)  # 重置 api_key
+Carl.reset_api_key(AK6)  # 再次重置 api_key
 ...
 ```
 
 #### 伪造对话
 
 ```python
 from openai2 import Chat, user_msg, assistant_msg
@@ -247,10 +247,25 @@
 
 ```python
 Ariel.unpin(0, -2, -1)  # 解锁索引为 0、-2、-1 的消息
 ```
 
 注：unpin 方法也允许传入“未锁定的消息”的索引，这使得当不确定某些消息的状态时，可以放心地将它们的索引传进去。
 
+#### 异步请求
+
+```python
+import asyncio
+from openai2 import Chat
+
+Tony = Chat(api_key=api_key, model="gpt-3.5-turbo")
+
+async def main():
+    answer = await Tony.asy_request('世界最大的海洋是哪个')  # >>> 51
+    print(answer)
+
+asyncio.run(main())  # >>> 太平洋
+```
+
 #### 更多方法
 
 openai2.Chat 底层调用了 [openai.ChatCompletion.create](https://platform.openai.com/docs/api-reference/chat/create?lang=python)，在实例化时，支持 openai.ChatCompletion.create 的所有参数，例如：`Chat(api_key=api_key, model="gpt-3.5-turbo", max_tokens=100)` 。
```

### Comparing `openai2-1.5.11.1/openai2/Dependent Packages/openai/LICENSE` & `openai2-1.6/openai2/Dependent Packages/openai/LICENSE`

 * *Files identical despite different names*

### Comparing `openai2-1.5.11.1/openai2/_core.py` & `openai2-1.6/openai2/_core.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,31 @@
 from json import dumps as jsonDumps
 from json import loads as jsonLoads
 from pathlib import Path
 from typing import Union, List
 import openai
 
 
+import aiohttp
+try:
+    from openai import api_requestor
+    from contextlib import asynccontextmanager
+    @asynccontextmanager
+    async def aiohttp_session():
+        user_set_session = openai.aiosession.get()
+        if user_set_session:
+            yield user_set_session
+        else:
+            async with aiohttp.ClientSession(trust_env=True) as session:
+                yield session
+    api_requestor.aiohttp_session = aiohttp_session
+except:
+    pass
+
+
 class AKPool:
     ''' 轮询获取api_key '''
 
     def __init__(self, apikeys: list):
         self._pool = self._POOL(apikeys)
 
     def fetch_key(self):
@@ -98,14 +115,15 @@
     '''
     文档: https://pypi.org/project/openai2
     
     获取api_key:
         获取链接1: https://platform.openai.com/account/api-keys
         获取链接2: https://www.baidu.com/s?wd=%E8%8E%B7%E5%8F%96%20openai%20api_key
     '''
+    recently_used_apikey: str = ''
 
     def __init__(self,
                  api_key: Union[str, AKPool],
                  model: str="gpt-3.5-turbo",
                  MsgMaxCount=None,
                  **kwargs
                  ):
@@ -117,30 +135,32 @@
     def reset_api_key(self, api_key: Union[str, AKPool]):
         if isinstance(api_key, AKPool):
             self._akpool = api_key
         else:
             self._akpool = AKPool([api_key])
 
     def request(self, text:str):
+        self.recently_used_apikey = self._akpool.fetch_key()
         completion = openai.ChatCompletion.create(**{
-            'api_key': self._akpool.fetch_key(),
+            'api_key': self.recently_used_apikey,
             'model': self.model,
             'messages': list(self._messages + [{"role": "user", "content": text}]),
             **self.kwargs
         })
         answer:str = completion.choices[0].message['content']
         self._messages.add_many(
             {"role": "user", "content": text},
             {"role": "assistant", "content": answer}
         )
         return answer
 
     async def asy_request(self, text:str):
+        self.recently_used_apikey = self._akpool.fetch_key()
         completion = await openai.ChatCompletion.acreate(**{
-            'api_key': self._akpool.fetch_key(),
+            'api_key': self.recently_used_apikey,
             'model': self.model,
             'messages': list(self._messages + [{"role": "user", "content": text}]),
             **self.kwargs
         })
         answer:str = completion.choices[0].message['content']
         self._messages.add_many(
             {"role": "user", "content": text},
```

### Comparing `openai2-1.5.11.1/pyproject.toml` & `openai2-1.6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "openai2"
-version = "1.5.11.1"
-description = "一个用来调用 ChatGPT 的工具，支持连续对话、对话存档与载入、对话回滚、对话伪造、轮询 api_key 池、限制历史消息数量"
+version = "1.6"
+description = "ChatGPT 工具包，支持连续对话、对话存档与载入、对话回滚、对话伪造、轮询 api_key 池、限制历史消息数量、异步请求"
 dependencies = ["openai"]
 keywords = ["openai2", "openai"]
 
 readme = "README.md"
 authors = [{name = "lcctoor.com", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
```

### Comparing `openai2-1.5.11.1/PKG-INFO` & `openai2-1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: openai2
-Version: 1.5.11.1
-Summary: 一个用来调用 ChatGPT 的工具，支持连续对话、对话存档与载入、对话回滚、对话伪造、轮询 api_key 池、限制历史消息数量
+Version: 1.6
+Summary: ChatGPT 工具包，支持连续对话、对话存档与载入、对话回滚、对话伪造、轮询 api_key 池、限制历史消息数量、异步请求
 Keywords: openai2,openai
 Author-email: "lcctoor.com" <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: openai
 Project-URL: HomePage, https://lcctoor.github.io/lccpy/?package=openai2
 
 # 项目描述
 
-一个用来调用 ChatGPT 的工具，支持连续对话、对话存档与载入、对话回滚、对话伪造、轮询 api_key 池、限制历史消息数量。
+ChatGPT 工具包，支持连续对话、对话存档与载入、对话回滚、对话伪造、轮询 api_key 池、限制历史消息数量、异步请求。
 
 # 关于作者
 
 作者：lcctoor.com
 
 域名：lcctoor.com
 
@@ -129,23 +129,23 @@
 Denny = Chat(api_key=AK2, model="gpt-3.5-turbo")
 Chris = Chat(api_key=AK3, model="gpt-3.5-turbo")  # 令 Chris 使用独立的'api_key池'
 Dick = Chat(api_key=AK4, model="gpt-3.5-turbo")  # 令 Dick 使用独立的'api_key池'
 ```
 
 注：允许（而非不允许）同一个 api_key 投放到不同的 api_key 池中，但每个 api_key 池都是独立调度，不会互相通信。
 
-#### 修改 api_key
+#### 重置 api_key
 
 ```python
 AK5 = 'sk-jg93...'
 AK6 = AKPool(['sk-vb7l...', 'sk-d3lv...'])
 ...
 
-Carl.reset_api_key(AK5)  # 修改 api_key
-Carl.reset_api_key(AK6)  # 再次修改 api_key
+Carl.reset_api_key(AK5)  # 重置 api_key
+Carl.reset_api_key(AK6)  # 再次重置 api_key
 ...
 ```
 
 #### 伪造对话
 
 ```python
 from openai2 import Chat, user_msg, assistant_msg
@@ -259,11 +259,26 @@
 
 ```python
 Ariel.unpin(0, -2, -1)  # 解锁索引为 0、-2、-1 的消息
 ```
 
 注：unpin 方法也允许传入“未锁定的消息”的索引，这使得当不确定某些消息的状态时，可以放心地将它们的索引传进去。
 
+#### 异步请求
+
+```python
+import asyncio
+from openai2 import Chat
+
+Tony = Chat(api_key=api_key, model="gpt-3.5-turbo")
+
+async def main():
+    answer = await Tony.asy_request('世界最大的海洋是哪个')  # >>> 51
+    print(answer)
+
+asyncio.run(main())  # >>> 太平洋
+```
+
 #### 更多方法
 
 openai2.Chat 底层调用了 [openai.ChatCompletion.create](https://platform.openai.com/docs/api-reference/chat/create?lang=python)，在实例化时，支持 openai.ChatCompletion.create 的所有参数，例如：`Chat(api_key=api_key, model="gpt-3.5-turbo", max_tokens=100)` 。
```

