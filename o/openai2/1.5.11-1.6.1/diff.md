# Comparing `tmp/openai2-1.5.11.tar.gz` & `tmp/openai2-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai2-1.5.11.tar", last modified: Sat Jul 15 15:54:08 2023, max compression
+gzip compressed data, was "openai2-1.6.1.tar", last modified: Tue Jul 18 12:21:30 2023, max compression
```

## Comparing `openai2-1.5.11.tar` & `openai2-1.6.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11038 2023-07-14 17:01:09.603744 openai2-1.5.11/LICENSE
--rw-r--r--   0        0        0     8664 2023-07-15 15:35:15.008513 openai2-1.5.11/README.md
--rw-r--r--   0        0        0     1083 2020-12-22 18:45:03.000000 openai2-1.5.11/openai2/Dependent Packages/openai/LICENSE
--rw-r--r--   0        0        0       56 2023-07-15 11:05:31.162471 openai2-1.5.11/openai2/__init__.py
--rw-r--r--   0        0        0     5434 2023-07-15 14:06:17.992651 openai2-1.5.11/openai2/_core.py
--rw-r--r--   0        0        0      648 2023-07-15 15:36:52.162685 openai2-1.5.11/pyproject.toml
--rw-r--r--   0        0        0     8899 1970-01-01 00:00:00.000000 openai2-1.5.11/PKG-INFO
+-rw-r--r--   0        0        0    11038 2023-07-14 17:01:09.603744 openai2-1.6.1/LICENSE
+-rw-r--r--   0        0        0     9023 2023-07-18 12:05:20.684928 openai2-1.6.1/README.md
+-rw-r--r--   0        0        0     1083 2020-12-22 18:45:03.000000 openai2-1.6.1/openai2/Dependent Packages/openai/LICENSE
+-rw-r--r--   0        0        0       56 2023-07-18 11:42:34.392010 openai2-1.6.1/openai2/__init__.py
+-rw-r--r--   0        0        0     6277 2023-07-18 12:17:45.431993 openai2-1.6.1/openai2/_core.py
+-rw-r--r--   0        0        0      670 2023-07-18 12:21:08.408468 openai2-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     9265 1970-01-01 00:00:00.000000 openai2-1.6.1/PKG-INFO
```

### Comparing `openai2-1.5.11/LICENSE` & `openai2-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openai2-1.5.11/README.md` & `openai2-1.6.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # 项目描述
 
-一个用来调用 ChatGPT 的工具，支持连续对话、对话存档与载入、对话回滚、对话伪造、轮询 api_key 池。
+ChatGPT 工具包，支持连续对话、对话存档与载入、对话回滚、对话伪造、轮询 api_key 池、限制历史消息数量、异步请求。
 
 # 关于作者
 
 作者：lcctoor.com
 
 域名：lcctoor.com
 
@@ -111,29 +111,29 @@
 AK2 = AKPool(['sk-mf40...', 'sk-m6g7...', ...])
 AK3 = AKPool(['sk-affe...', 'sk-fam4...', ...])
 AK4 = AKPool(['sk-detg...', 'sk-adle...', ...])
 
 Duke = Chat(api_key=AK1, model="gpt-3.5-turbo")  # 令 Duke 使用固定的 api_key
 Carl = Chat(api_key=AK2, model="gpt-3.5-turbo")  # 令 Carl 和 Denny 使用同一个'api_key池', 系统将自动充分利用每个api_key
 Denny = Chat(api_key=AK2, model="gpt-3.5-turbo")
-Chris = Chat(api_key=AK3, model="gpt-3.5-turbo")  # 令 Chris 和 Dick 各自使用独立的'api_key池'
-Dick = Chat(api_key=AK4, model="gpt-3.5-turbo")
+Chris = Chat(api_key=AK3, model="gpt-3.5-turbo")  # 令 Chris 使用独立的'api_key池'
+Dick = Chat(api_key=AK4, model="gpt-3.5-turbo")  # 令 Dick 使用独立的'api_key池'
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
@@ -147,15 +147,15 @@
     assistant_msg('10+10=你大爷, 你提的这些问题真弱智!'),
 )
 
 answer = Mickey.request('哦吼, 你还敢骂我呀?')
 print(answer)  # >>> 非常抱歉，我刚才的回答有些不适当。1+1=2, 10+10=20。非常抱歉给你带来困扰！
 ```
 
-注：伪造对话不仅仅可以放在对话开头，也可以穿插在对话中的任何时刻。
+注：伪造对话可以穿插在对话中的任何时刻。
 
 #### 查看对话记录
 
 ```python
 Ariel = Chat(api_key=api_key, model="gpt-3.5-turbo")
 
 Ariel.request('自然数1的后面是几?')  # >>> 2
@@ -167,29 +167,29 @@
 #     {'role': 'user', 'content': '自然数1的后面是几?'},
 #     {'role': 'assistant', 'content': '2'},
 #     {'role': 'user', 'content': '再往后是几?'},
 #     {'role': 'assistant', 'content': '3'}
 # ]
 ```
 
-#### 限定历史消息数量
+#### 限制历史消息数量
 
-##### 限定历史消息数量
+##### 限制历史消息数量
 
-随着对话次数越来越多，最终上下文长度就会超出 openai 接口限定的最大 token 数量，此时可使用 MsgMaxCount 参数来限定历史消息数量。当消息数量超出 MsgMaxCount 后，程序会自动移除最早的记录，使消息数量减少到恰好等于 MsgMaxCount 。
+随着对话次数越来越多，最终上下文长度就会超出 openai 接口限定的最大 token 数量，此时可使用 MsgMaxCount 参数来限制历史消息数量。当消息数量超出 MsgMaxCount 后，程序会自动移除最早的记录，使消息数量减少到恰好等于 MsgMaxCount 。
 
 ```python
 MsgMaxCount = 6  # 最多保留6条历史消息
 Ariel = Chat(api_key=api_key, model="gpt-3.5-turbo", MsgMaxCount=MsgMaxCount)
 
 Ariel.request('英国的首都是什么？')  # >>> '伦敦'
 Ariel.request('日本首都是什么？')  # >>> '东京'
 Ariel.request('意大利的首都是什么？')  # >>> '罗马'
 Ariel.request('美国的首都是什么？')  # >>> '华盛顿'
-Ariel.request('世界上国土面积最大的国家？')  # >>> '俄罗斯'
+Ariel.request('世界上国土面积最大的国家是哪个？')  # >>> '俄罗斯'
 Ariel.request('法国的首都叫什么？')  # >>> '巴黎'
 Ariel.request('青蛙的幼体叫什么？')  # >>> '蝌蚪'
 Ariel.request('世界上最大的海洋是什么？')  # >>> '太平洋'
 
 Ariel.fetch_messages()
 # 返回:
 # [
@@ -210,23 +210,23 @@
 MsgMaxCount = 6
 Ariel = Chat(api_key=api_key, model="gpt-3.5-turbo", MsgMaxCount=MsgMaxCount)
 
 Ariel.request('英国的首都是什么？')  # >>> '伦敦'  此时产生了2条消息, 索引分别为 0 和 1
 Ariel.request('日本首都是什么？')  # >>> '东京'
 Ariel.request('意大利的首都是什么？')  # >>> '罗马'
 
-# 锁定索引为 0、-1、-2 的消息
-# 索引风格与Python基本数据类型的风格相同: 0表示第1个元素, -1表示倒数第1个元素
-# 索引无须按顺序填写, pin(0, 1, 2) 与 pin(0, 2, 1) 等价.
-Ariel.pin(0, -1, -2)
+# 锁定索引为 0、-2、-1 的消息
+# 索引风格与Python基本数据类型的索引风格相同: 0表示第1个元素, -1表示倒数第1个元素
+# 索引无须按顺序填写: pin(0, 1, 2) 与 pin(0, 2, 1) 等价.
+Ariel.pin(0, -2, -1)
 
 Ariel.request('美国的首都是什么？')  # >>> '华盛顿'
 Ariel.pin(-2)  # 锁定索引为 -2 的消息
 
-Ariel.request('世界上国土面积最大的国家？')  # >>> '俄罗斯'
+Ariel.request('世界上国土面积最大的国家是哪个？')  # >>> '俄罗斯'
 Ariel.request('法国的首都叫什么？')  # >>> '巴黎'
 Ariel.request('青蛙的幼体叫什么？')  # >>> '蝌蚪'
 Ariel.request('世界上最大的海洋是什么？')  # >>> '太平洋'
 
 Ariel.fetch_messages()
 # 返回:
 # [
@@ -235,22 +235,37 @@
 #     {'role': 'assistant', 'content': '罗马'},               # 被锁定的消息
 #     {'role': 'user', 'content': '美国的首都是什么？'},       # 被锁定的消息
 #     {'role': 'user', 'content': '世界上最大的海洋是什么？'},
 #     {'role': 'assistant', 'content': '太平洋'}
 # ]
 ```
 
-注：pin 方法也可传入“已锁定的消息”的索引，这使得当不确定某些消息的状态时，可以放心地将索引传进去。
+注：pin 方法也允许传入“已锁定的消息”的索引，这使得当不确定某些消息的状态时，可以放心地将它们的索引传进去。
 
 ##### 解锁消息
 
 可使用 unpin 方法将已锁定的消息解除锁定。
 
 ```python
-Ariel.pin(0, -1, -2)  # 解锁索引为 0、-1、-2 的消息
+Ariel.unpin(0, -2, -1)  # 解锁索引为 0、-2、-1 的消息
 ```
 
-注：unpin 方法也可传入“未锁定的消息”的索引，这使得当不确定某些消息的状态时，可以放心地将索引传进去。
+注：unpin 方法也允许传入“未锁定的消息”的索引，这使得当不确定某些消息的状态时，可以放心地将它们的索引传进去。
+
+#### 异步请求
+
+```python
+import asyncio
+from openai2 import Chat
+
+Tony = Chat(api_key=api_key, model="gpt-3.5-turbo")
+
+async def main():
+    answer = await Tony.asy_request('世界上最大的海洋是哪个')  # >>> 51
+    print(answer)
+
+asyncio.run(main())  # >>> 太平洋
+```
 
 #### 更多方法
 
 openai2.Chat 底层调用了 [openai.ChatCompletion.create](https://platform.openai.com/docs/api-reference/chat/create?lang=python)，在实例化时，支持 openai.ChatCompletion.create 的所有参数，例如：`Chat(api_key=api_key, model="gpt-3.5-turbo", max_tokens=100)` 。
```

### Comparing `openai2-1.5.11/openai2/Dependent Packages/openai/LICENSE` & `openai2-1.6.1/openai2/Dependent Packages/openai/LICENSE`

 * *Files identical despite different names*

### Comparing `openai2-1.5.11/openai2/_core.py` & `openai2-1.6.1/openai2/_core.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,14 +11,35 @@
 from json import dumps as jsonDumps
 from json import loads as jsonLoads
 from pathlib import Path
 from typing import Union, List
 import openai
 
 
+try:
+    import aiohttp
+    from openai import api_requestor
+    from contextlib import asynccontextmanager
+    @asynccontextmanager
+    async def aiohttp_session():
+        '''
+            该函数基于 PyPi包 "openai" 中的 aiohttp_session 函数改写,
+            "openai"包的版权声明为: Copyright (c) OpenAI (https://openai.com)
+        '''
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
@@ -98,14 +119,15 @@
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
@@ -117,30 +139,32 @@
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

### Comparing `openai2-1.5.11/pyproject.toml` & `openai2-1.6.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "openai2"
-version = "1.5.11"
-description = "一个用来调用 ChatGPT 的工具，支持连续对话、对话存档与载入、对话回滚、对话伪造、轮询 api_key 池"
+version = "1.6.1"
+description = "ChatGPT 工具包，支持连续对话、对话存档与载入、对话回滚、对话伪造、轮询 api_key 池、限制历史消息数量、异步请求"
 dependencies = ["openai"]
 keywords = ["openai2", "openai"]
 
 readme = "README.md"
 authors = [{name = "lcctoor.com", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
```

### Comparing `openai2-1.5.11/PKG-INFO` & `openai2-1.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: openai2
-Version: 1.5.11
-Summary: 一个用来调用 ChatGPT 的工具，支持连续对话、对话存档与载入、对话回滚、对话伪造、轮询 api_key 池
+Version: 1.6.1
+Summary: ChatGPT 工具包，支持连续对话、对话存档与载入、对话回滚、对话伪造、轮询 api_key 池、限制历史消息数量、异步请求
 Keywords: openai2,openai
 Author-email: "lcctoor.com" <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: openai
 Project-URL: HomePage, https://lcctoor.github.io/lccpy/?package=openai2
 
 # 项目描述
 
-一个用来调用 ChatGPT 的工具，支持连续对话、对话存档与载入、对话回滚、对话伪造、轮询 api_key 池。
+ChatGPT 工具包，支持连续对话、对话存档与载入、对话回滚、对话伪造、轮询 api_key 池、限制历史消息数量、异步请求。
 
 # 关于作者
 
 作者：lcctoor.com
 
 域名：lcctoor.com
 
@@ -123,29 +123,29 @@
 AK2 = AKPool(['sk-mf40...', 'sk-m6g7...', ...])
 AK3 = AKPool(['sk-affe...', 'sk-fam4...', ...])
 AK4 = AKPool(['sk-detg...', 'sk-adle...', ...])
 
 Duke = Chat(api_key=AK1, model="gpt-3.5-turbo")  # 令 Duke 使用固定的 api_key
 Carl = Chat(api_key=AK2, model="gpt-3.5-turbo")  # 令 Carl 和 Denny 使用同一个'api_key池', 系统将自动充分利用每个api_key
 Denny = Chat(api_key=AK2, model="gpt-3.5-turbo")
-Chris = Chat(api_key=AK3, model="gpt-3.5-turbo")  # 令 Chris 和 Dick 各自使用独立的'api_key池'
-Dick = Chat(api_key=AK4, model="gpt-3.5-turbo")
+Chris = Chat(api_key=AK3, model="gpt-3.5-turbo")  # 令 Chris 使用独立的'api_key池'
+Dick = Chat(api_key=AK4, model="gpt-3.5-turbo")  # 令 Dick 使用独立的'api_key池'
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
@@ -159,15 +159,15 @@
     assistant_msg('10+10=你大爷, 你提的这些问题真弱智!'),
 )
 
 answer = Mickey.request('哦吼, 你还敢骂我呀?')
 print(answer)  # >>> 非常抱歉，我刚才的回答有些不适当。1+1=2, 10+10=20。非常抱歉给你带来困扰！
 ```
 
-注：伪造对话不仅仅可以放在对话开头，也可以穿插在对话中的任何时刻。
+注：伪造对话可以穿插在对话中的任何时刻。
 
 #### 查看对话记录
 
 ```python
 Ariel = Chat(api_key=api_key, model="gpt-3.5-turbo")
 
 Ariel.request('自然数1的后面是几?')  # >>> 2
@@ -179,29 +179,29 @@
 #     {'role': 'user', 'content': '自然数1的后面是几?'},
 #     {'role': 'assistant', 'content': '2'},
 #     {'role': 'user', 'content': '再往后是几?'},
 #     {'role': 'assistant', 'content': '3'}
 # ]
 ```
 
-#### 限定历史消息数量
+#### 限制历史消息数量
 
-##### 限定历史消息数量
+##### 限制历史消息数量
 
-随着对话次数越来越多，最终上下文长度就会超出 openai 接口限定的最大 token 数量，此时可使用 MsgMaxCount 参数来限定历史消息数量。当消息数量超出 MsgMaxCount 后，程序会自动移除最早的记录，使消息数量减少到恰好等于 MsgMaxCount 。
+随着对话次数越来越多，最终上下文长度就会超出 openai 接口限定的最大 token 数量，此时可使用 MsgMaxCount 参数来限制历史消息数量。当消息数量超出 MsgMaxCount 后，程序会自动移除最早的记录，使消息数量减少到恰好等于 MsgMaxCount 。
 
 ```python
 MsgMaxCount = 6  # 最多保留6条历史消息
 Ariel = Chat(api_key=api_key, model="gpt-3.5-turbo", MsgMaxCount=MsgMaxCount)
 
 Ariel.request('英国的首都是什么？')  # >>> '伦敦'
 Ariel.request('日本首都是什么？')  # >>> '东京'
 Ariel.request('意大利的首都是什么？')  # >>> '罗马'
 Ariel.request('美国的首都是什么？')  # >>> '华盛顿'
-Ariel.request('世界上国土面积最大的国家？')  # >>> '俄罗斯'
+Ariel.request('世界上国土面积最大的国家是哪个？')  # >>> '俄罗斯'
 Ariel.request('法国的首都叫什么？')  # >>> '巴黎'
 Ariel.request('青蛙的幼体叫什么？')  # >>> '蝌蚪'
 Ariel.request('世界上最大的海洋是什么？')  # >>> '太平洋'
 
 Ariel.fetch_messages()
 # 返回:
 # [
@@ -222,23 +222,23 @@
 MsgMaxCount = 6
 Ariel = Chat(api_key=api_key, model="gpt-3.5-turbo", MsgMaxCount=MsgMaxCount)
 
 Ariel.request('英国的首都是什么？')  # >>> '伦敦'  此时产生了2条消息, 索引分别为 0 和 1
 Ariel.request('日本首都是什么？')  # >>> '东京'
 Ariel.request('意大利的首都是什么？')  # >>> '罗马'
 
-# 锁定索引为 0、-1、-2 的消息
-# 索引风格与Python基本数据类型的风格相同: 0表示第1个元素, -1表示倒数第1个元素
-# 索引无须按顺序填写, pin(0, 1, 2) 与 pin(0, 2, 1) 等价.
-Ariel.pin(0, -1, -2)
+# 锁定索引为 0、-2、-1 的消息
+# 索引风格与Python基本数据类型的索引风格相同: 0表示第1个元素, -1表示倒数第1个元素
+# 索引无须按顺序填写: pin(0, 1, 2) 与 pin(0, 2, 1) 等价.
+Ariel.pin(0, -2, -1)
 
 Ariel.request('美国的首都是什么？')  # >>> '华盛顿'
 Ariel.pin(-2)  # 锁定索引为 -2 的消息
 
-Ariel.request('世界上国土面积最大的国家？')  # >>> '俄罗斯'
+Ariel.request('世界上国土面积最大的国家是哪个？')  # >>> '俄罗斯'
 Ariel.request('法国的首都叫什么？')  # >>> '巴黎'
 Ariel.request('青蛙的幼体叫什么？')  # >>> '蝌蚪'
 Ariel.request('世界上最大的海洋是什么？')  # >>> '太平洋'
 
 Ariel.fetch_messages()
 # 返回:
 # [
@@ -247,23 +247,38 @@
 #     {'role': 'assistant', 'content': '罗马'},               # 被锁定的消息
 #     {'role': 'user', 'content': '美国的首都是什么？'},       # 被锁定的消息
 #     {'role': 'user', 'content': '世界上最大的海洋是什么？'},
 #     {'role': 'assistant', 'content': '太平洋'}
 # ]
 ```
 
-注：pin 方法也可传入“已锁定的消息”的索引，这使得当不确定某些消息的状态时，可以放心地将索引传进去。
+注：pin 方法也允许传入“已锁定的消息”的索引，这使得当不确定某些消息的状态时，可以放心地将它们的索引传进去。
 
 ##### 解锁消息
 
 可使用 unpin 方法将已锁定的消息解除锁定。
 
 ```python
-Ariel.pin(0, -1, -2)  # 解锁索引为 0、-1、-2 的消息
+Ariel.unpin(0, -2, -1)  # 解锁索引为 0、-2、-1 的消息
 ```
 
-注：unpin 方法也可传入“未锁定的消息”的索引，这使得当不确定某些消息的状态时，可以放心地将索引传进去。
+注：unpin 方法也允许传入“未锁定的消息”的索引，这使得当不确定某些消息的状态时，可以放心地将它们的索引传进去。
+
+#### 异步请求
+
+```python
+import asyncio
+from openai2 import Chat
+
+Tony = Chat(api_key=api_key, model="gpt-3.5-turbo")
+
+async def main():
+    answer = await Tony.asy_request('世界上最大的海洋是哪个')  # >>> 51
+    print(answer)
+
+asyncio.run(main())  # >>> 太平洋
+```
 
 #### 更多方法
 
 openai2.Chat 底层调用了 [openai.ChatCompletion.create](https://platform.openai.com/docs/api-reference/chat/create?lang=python)，在实例化时，支持 openai.ChatCompletion.create 的所有参数，例如：`Chat(api_key=api_key, model="gpt-3.5-turbo", max_tokens=100)` 。
```

