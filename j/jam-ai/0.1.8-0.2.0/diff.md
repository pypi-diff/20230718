# Comparing `tmp/jam_ai-0.1.8.tar.gz` & `tmp/jam_ai-0.2.0.tar.gz`

## Comparing `jam_ai-0.1.8.tar` & `jam_ai-0.2.0.tar`

### file list

```diff
@@ -1,46 +1,50 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.8/cmd/__init__.py
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 jam_ai-0.1.8/cmd/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.8/example/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.8/example/personnel/__init__.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 jam_ai-0.1.8/example/personnel/albert-einstein.json
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 jam_ai-0.1.8/example/personnel/homer-simpson.json
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jam_ai-0.1.8/example/personnel/marie-curie.json
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 jam_ai-0.1.8/example/personnel/walter-white.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/__init__.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/base.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/core.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/version.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/instrument/__init__.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/instrument/base.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/instrument/image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/instrument/text.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/interface/__init__.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/interface/base.py
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/interface/openai.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/interface/stability_ai.py
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/interface/writesonic.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/persistence/__init__.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/persistence/base.py
--rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/persistence/memory.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/persistence/model.py
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/persistence/mysql.py
--rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/persistence/postgres.py
--rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/persistence/sqlite.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/personnel/__init__.py
--rw-r--r--   0        0        0     6954 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/personnel/base.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/personnel/personnel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/util/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/util/generate.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/util/search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.8/tests/instrument/__init__.py
--rw-r--r--   0        0        0    10211 2020-02-02 00:00:00.000000 jam_ai-0.1.8/tests/instrument/test_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.8/tests/interface/__init__.py
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 jam_ai-0.1.8/tests/interface/test_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.8/tests/test_persistence/__init__.py
--rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 jam_ai-0.1.8/tests/test_persistence/test_base.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 jam_ai-0.1.8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 jam_ai-0.1.8/LICENSE
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 jam_ai-0.1.8/README.md
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 jam_ai-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    16352 2020-02-02 00:00:00.000000 jam_ai-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.2.0/cmd/__init__.py
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 jam_ai-0.2.0/cmd/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.2.0/example/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.2.0/example/personnel/__init__.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 jam_ai-0.2.0/example/personnel/albert-einstein.json
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 jam_ai-0.2.0/example/personnel/claude-monet.json
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 jam_ai-0.2.0/example/personnel/homer-simpson.json
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jam_ai-0.2.0/example/personnel/marie-curie.json
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 jam_ai-0.2.0/example/personnel/pablo-picasso.json
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 jam_ai-0.2.0/example/personnel/vincent-van-gogh.json
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 jam_ai-0.2.0/example/personnel/walter-white.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jam_ai-0.2.0/jam/__init__.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jam_ai-0.2.0/jam/base.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 jam_ai-0.2.0/jam/core.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 jam_ai-0.2.0/jam/version.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 jam_ai-0.2.0/jam/instrument/__init__.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 jam_ai-0.2.0/jam/instrument/base.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 jam_ai-0.2.0/jam/instrument/image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.2.0/jam/instrument/text.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 jam_ai-0.2.0/jam/interface/__init__.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 jam_ai-0.2.0/jam/interface/base.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 jam_ai-0.2.0/jam/interface/openai.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 jam_ai-0.2.0/jam/interface/stability_ai.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 jam_ai-0.2.0/jam/interface/writesonic.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 jam_ai-0.2.0/jam/persistence/__init__.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 jam_ai-0.2.0/jam/persistence/base.py
+-rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 jam_ai-0.2.0/jam/persistence/memory.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 jam_ai-0.2.0/jam/persistence/model.py
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 jam_ai-0.2.0/jam/persistence/mysql.py
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 jam_ai-0.2.0/jam/persistence/postgres.py
+-rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 jam_ai-0.2.0/jam/persistence/sqlite.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 jam_ai-0.2.0/jam/personnel/__init__.py
+-rw-r--r--   0        0        0     8746 2020-02-02 00:00:00.000000 jam_ai-0.2.0/jam/personnel/base.py
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 jam_ai-0.2.0/jam/personnel/personnel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.2.0/jam/util/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 jam_ai-0.2.0/jam/util/generate.py
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 jam_ai-0.2.0/jam/util/prompt.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jam_ai-0.2.0/jam/util/search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.2.0/tests/instrument/__init__.py
+-rw-r--r--   0        0        0    10211 2020-02-02 00:00:00.000000 jam_ai-0.2.0/tests/instrument/test_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.2.0/tests/interface/__init__.py
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 jam_ai-0.2.0/tests/interface/test_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.2.0/tests/test_persistence/__init__.py
+-rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 jam_ai-0.2.0/tests/test_persistence/test_base.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 jam_ai-0.2.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 jam_ai-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 jam_ai-0.2.0/README.md
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 jam_ai-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    16591 2020-02-02 00:00:00.000000 jam_ai-0.2.0/PKG-INFO
```

### Comparing `jam_ai-0.1.8/cmd/main.py` & `jam_ai-0.2.0/cmd/main.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/example/personnel/albert-einstein.json` & `jam_ai-0.2.0/example/personnel/albert-einstein.json`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/example/personnel/homer-simpson.json` & `jam_ai-0.2.0/example/personnel/homer-simpson.json`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/example/personnel/marie-curie.json` & `jam_ai-0.2.0/example/personnel/marie-curie.json`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/example/personnel/walter-white.json` & `jam_ai-0.2.0/example/personnel/walter-white.json`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/jam/base.py` & `jam_ai-0.2.0/jam/base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/jam/core.py` & `jam_ai-0.2.0/jam/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 from multiprocessing.pool import ThreadPool
-from typing import List, Optional
+from typing import List, Optional, AnyStr
 
 from jam.base import BaseJam
 from jam.version import version
 from jam.instrument.base import BaseInstrument
 from jam.persistence.base import BasePersistence
 from jam.personnel.base import BasePersonnel
 from jam.util.search import search_mention
 
 
 class Jam(BaseJam):
-
     __version__ = version
 
     def __init__(self,
                  members: Optional[List[BasePersonnel]],
                  instruments: List[BaseInstrument] = None,
                  persistence: Optional[BasePersistence] = None):
         super(Jam, self).__init__(members, instruments, persistence)
         self.cache_output = []
 
     @staticmethod
     def _mention_filter(message: str, members: List[BasePersonnel]) -> List[BasePersonnel]:
         mention_filter = [member for member in members if member.uid in search_mention(message)]
         return mention_filter
 
-    def _assign(self, member: BasePersonnel, message: str):
-        call_output = member.call(message)
+    def _assign(self, member: BasePersonnel, cid: AnyStr = 'main'):
+        call_output = member.call(cid=cid)
         self.cache_output += call_output
         return
 
     def _multi_assign(self, args):
         self._assign(*args)
         return
 
-    def compose(self, message: str, multi=True):
+    def compose(self, message: str, multi: bool = True, cid: AnyStr = 'main'):
         self.cache_output = []
 
         prompt_member = self._mention_filter(
             message, self.members
         ) or [member for member in self.members if not member.mention_only]
         self.persistence.save(
+            cid=cid,
             role='user',
             author='user',
             content=message,
-            mentions=[member.uid for member in prompt_member]
+            mentions=[member.uid for member in prompt_member],
         )
 
         if multi:
-            tasks = [(member, message) for member in prompt_member]
+            tasks = [(member, cid) for member in prompt_member]
             with ThreadPool() as pool:
                 pool.map(self._multi_assign, tasks)
         else:
             for member in prompt_member:
-                self._assign(member, message)
+                self._assign(member, cid)
         return self.cache_output
 
     def history(self):
         result = self.persistence.all()
         return result
 
-    def clear(self, key: str = None,  value: List[str] = None):
+    def clear(self, key: str = None, value: List[str] = None):
         self.persistence.clear(key, value)
         return
```

### Comparing `jam_ai-0.1.8/jam/instrument/base.py` & `jam_ai-0.2.0/jam/instrument/base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/jam/instrument/image.py` & `jam_ai-0.2.0/jam/instrument/image.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/jam/interface/base.py` & `jam_ai-0.2.0/jam/interface/base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/jam/interface/openai.py` & `jam_ai-0.2.0/jam/interface/openai.py`

 * *Files 15% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                  model: str = DEFAULT_MODEL,
                  functions: List[Dict] = None):
         super(OpenAIChat, self).__init__(token, model)
         self.functions = functions
 
     def call(self, messages: List[Dict] = None, functional: bool = True) -> JIOutput:
         x_message = self.form_message(messages)
-        if functional:
+        if functional and self.functions:
             response = self.open_ai.ChatCompletion.create(
                 model=self.model,
                 messages=x_message,
                 functions=self.functions,
                 function_call='auto'
             )
             response_message = response['choices'][0]['message']
@@ -74,14 +74,35 @@
             if message.get('name'):
                 msg_obj['name'] = message.get('name')
 
             msg_objs.append(msg_obj)
         return msg_objs
 
 
+class OpenAIComplete(OpenAIBase):
+
+    DEFAULT_MODEL = 'text-davinci-003'
+
+    def __init__(self,
+                 token: str = None,
+                 model: str = DEFAULT_MODEL,
+                 max_tokens: int = 1000):
+        super(OpenAIComplete, self).__init__(token, model)
+        self.max_tokens = max_tokens
+
+    def call(self, x: AnyStr = None) -> JIOutput:
+        response = self.open_ai.Completion.create(
+            model=self.model,
+            prompt=x,
+            max_tokens=self.max_tokens
+        )
+        response_message = response['choices'][0]['text']
+        return JIOutput(output=response_message)
+
+
 class OpenAIImageGen(OpenAIBase):
 
     def __init__(self,
                  token: str = None,
                  model: str = None,
                  samples: int = 1,
                  dimension: Tuple[int, int] = (512, 512)):
```

### Comparing `jam_ai-0.1.8/jam/interface/stability_ai.py` & `jam_ai-0.2.0/jam/interface/stability_ai.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/jam/interface/writesonic.py` & `jam_ai-0.2.0/jam/interface/writesonic.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/jam/persistence/base.py` & `jam_ai-0.2.0/jam/persistence/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,27 @@
 from datetime import datetime
 from typing import Dict, AnyStr, List
 
-
-class BasePersistence(object):
-
-    def __init__(self):
-        pass
-
-    @staticmethod
-    def transform(data: Dict) -> Dict:
-        return {}
-
-    def save(self,
-             role: str,
-             author: str,
-             content: str,
-             mentions: List[str] = None,
-             function: str = None,
-             success: bool = True):
-        return []
-
-    def find(self, key: str, value: str = None, limit: int = 5):
-        return []
-
-    def all(self):
-        return []
-
-    def count(self):
-        return 0
-
-    def clear(self):
-        return
+from jam.persistence.model import ConversationHistory
 
 
 class PersistenceObject:
 
     def __init__(self,
                  uid: AnyStr,
+                 cid: AnyStr,
                  author: str,
                  role: str,
                  content: AnyStr,
                  mention: AnyStr,
                  function: AnyStr,
                  timestamp: datetime = None,
                  success: bool = True):
         self.uid = uid
+        self.cid = cid
         self.author = author
         self.role = role
         self.content = content
         self.mention = mention
         self.function = function
         self.timestamp = timestamp
         self.success = success
@@ -57,8 +30,51 @@
         return {
             'role': self.role,
             'content': self.content,
             'name': self.function
         }
 
     def __repr__(self):
-        return f'<PersistenceObject (author={self.author}, content={self.content}, mention={self.mention})'
+        return f'<PersistenceObject (cid={self.cid}, author={self.author}, content={self.content}, mention={self.mention})'
+
+
+class BasePersistence(object):
+
+    def __init__(self):
+        pass
+
+    @staticmethod
+    def transform(data: ConversationHistory) -> PersistenceObject:
+        data_obj = PersistenceObject(
+            uid=data.uid,
+            cid=data.cid,
+            role=data.role,
+            author=data.author,
+            content=data.content,
+            mention=data.mention,
+            function=data.function,
+            timestamp=data.timestamp,
+            success=data.success
+        )
+        return data_obj
+
+    def save(self,
+             cid: str,
+             role: str,
+             author: str,
+             content: str,
+             mentions: List[str] = None,
+             function: str = None,
+             success: bool = True):
+        return []
+
+    def find(self, conditions: Dict, limit: int = 5):
+        return []
+
+    def all(self):
+        return []
+
+    def count(self):
+        return 0
+
+    def clear(self):
+        return
```

### Comparing `jam_ai-0.1.8/jam/persistence/memory.py` & `jam_ai-0.2.0/jam/persistence/memory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import List, Optional
+from typing import List, Optional, Dict
 
 from jam.persistence.base import BasePersistence
 from jam.persistence.base import PersistenceObject
 from jam.util.generate import generate_id
 
 
 class Node:
@@ -23,34 +23,32 @@
 
     def append(self, data: PersistenceObject):
         new_node = Node(data)
         if not self.head:
             self.head = new_node
             self.tail = new_node
         else:
-            # current = self.head
-            # while current.next:
-            #     current = current.next
-            # current.next = new_node
-            # new_node.prev = current
-            # self.tail = new_node
             current = self.tail
             current.next = new_node
             new_node.prev = self.tail
             self.tail = new_node
         self.length += 1
 
-    def find(self, key: str, value: List[str], limit: int = 5):
+    def find(self, conditions: Dict, limit: int = 5):
         result = []
         current = self.tail
         if current is None:
             return result
 
         while current is not None and len(result) < limit:
-            if current.data.__dict__[key] in value and current.data.mention in value:
+            key_flag = 0
+            for key, value in conditions.items():
+                if current.data.__dict__[key] in value:
+                    key_flag += 1
+            if key_flag >= len(conditions):
                 result.insert(0, current.data)
             current = current.prev
         return result
 
     def all(self):
         result = []
         current = self.tail
@@ -84,41 +82,43 @@
 class MemoryPersistence(BasePersistence):
 
     def __init__(self):
         super(MemoryPersistence, self).__init__()
         self.db: DoubleLinkedList = DoubleLinkedList()
 
     def save(self,
+             cid: str,
              role: str,
              author: str,
              content: str,
              mentions: List[str] = None,
              function: str = None,
              success: bool = True):
         saved_objs = []
         if mentions is None:
             mentions = ['user']
 
         for mention in mentions:
             data_obj = PersistenceObject(
                 uid=generate_id(16),
+                cid=cid,
                 role=role,
                 author=author,
                 content=content,
                 mention=mention,
                 function=function,
                 timestamp=datetime.now(),
                 success=success
             )
             self.db.append(data_obj)
             saved_objs.append(data_obj)
         return saved_objs
 
-    def find(self, key: str, value: List[str] = None, limit: int = 5):
-        result = self.db.find(key, value, limit)
+    def find(self, conditions: Dict, limit: int = 5):
+        result = self.db.find(conditions, limit)
         return result
 
     def all(self):
         result = self.db.all()
         return result
 
     def count(self):
```

### Comparing `jam_ai-0.1.8/jam/persistence/model.py` & `jam_ai-0.2.0/jam/persistence/model.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,17 +8,32 @@
 from sqlalchemy.orm import mapped_column
 from sqlalchemy.ext.declarative import declarative_base
 
 Base = declarative_base()
 
 
 class ConversationHistory(Base):
+    """
+    ConversationHistory:
+
+    - uid: Unique ID
+    - cid: Conversation ID
+    - author: Message Author
+    - role: Message Role
+    - content: Message Content
+    - mention: Mention Author
+    - function: Function Called
+    - timestamp: Message Timestamp
+    - success: Message Status
+    """
+
     __tablename__ = "conversation_history"
 
     uid: Mapped[str] = mapped_column(String(16), primary_key=True)
+    cid: Mapped[str] = mapped_column(String(32), nullable=True, default='main')
     author: Mapped[str] = mapped_column(String(32))
     role: Mapped[str] = mapped_column(String(32))
     content: Mapped[str] = mapped_column(Text)
     mention: Mapped[str] = mapped_column(String(32), nullable=True)
     function: Mapped[str] = mapped_column(String(32), nullable=True)
     timestamp: Mapped[datetime] = mapped_column(DateTime, default=datetime.now)
     success: Mapped[bool] = mapped_column(Boolean, default=True)
```

### Comparing `jam_ai-0.1.8/jam/persistence/mysql.py` & `jam_ai-0.2.0/jam/persistence/mysql.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,65 +22,52 @@
 
         self.seed()
 
     def seed(self):
         if not self.db.dialect.has_table(self.db.connect(), 'conversation_history'):
             Base.metadata.create_all(self.db)
 
-    @staticmethod
-    def transform(data: ConversationHistory) -> PersistenceObject:
-        data_obj = PersistenceObject(
-            uid=data.uid,
-            role=data.role,
-            author=data.author,
-            content=data.content,
-            mention=data.mention,
-            function=data.function,
-            timestamp=data.timestamp,
-            success=data.success
-        )
-        return data_obj
-
     def save(self,
+             cid: str,
              role: str,
              author: str,
              content: str,
              mentions: List[str] = None,
              function: str = None,
              success: bool = True):
         saved_objs = []
         if mentions is None:
             mentions = ['user']
 
         with Session(self.db) as session:
             for mention in mentions:
                 conv_history = ConversationHistory(
                     uid=generate_id(16),
+                    cid=cid,
                     role=role,
                     author=author,
                     content=content,
                     mention=mention,
                     function=function,
                     success=success
                 )
                 session.add(conv_history)
                 saved_objs.append(conv_history)
             session.commit()
 
             return list(map(self.transform, saved_objs))
 
-    def find(self, key: str, value: List[str] = None, limit: int = 5):
+    def find(self, conditions: Dict, limit: int = 5):
         with Session(self.db) as session:
-            key_conditions = [getattr(ConversationHistory, key) == val for val in value]
-            key_conditions = or_(*key_conditions)
-
-            mention_conditions = [getattr(ConversationHistory, 'mention') == val for val in value]
-            mention_conditions = or_(*mention_conditions)
-
-            filter_conditions = and_(key_conditions, mention_conditions)
+            filter_conditions = []
+            for key, value in conditions.items():
+                temp_conditions = [getattr(ConversationHistory, key) == val for val in value]
+                temp_conditions = or_(*temp_conditions)
+                filter_conditions.append(temp_conditions)
+            filter_conditions = and_(*filter_conditions)
 
             result = session.query(
                 ConversationHistory
             ).filter(filter_conditions).order_by(ConversationHistory.timestamp.desc()).limit(limit).all()
 
             return list(map(self.transform, result[::-1]))
```

### Comparing `jam_ai-0.1.8/jam/persistence/postgres.py` & `jam_ai-0.2.0/jam/persistence/sqlite.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,86 +1,73 @@
-from typing import List, Dict
+from typing import List, Dict, AnyStr
 
 from jam.persistence.base import BasePersistence
 from jam.persistence.base import PersistenceObject
 from jam.persistence.model import Base
 from jam.persistence.model import ConversationHistory
 from jam.util.generate import generate_id
 
 from sqlalchemy import create_engine
 from sqlalchemy import MetaData
 from sqlalchemy import or_, and_
 from sqlalchemy.orm import Session
 
 
-class PostgresPersistence(BasePersistence):
+class SQLitePersistence(BasePersistence):
 
-    def __init__(self, dbname: str = 'postgresql+psycopg2://localhost:5432/postgres'):
-        super(PostgresPersistence, self).__init__()
+    def __init__(self, dbname: str = 'sqlite:///jam.db'):
+        super(SQLitePersistence, self).__init__()
         self._dbname = dbname
-        self.db = create_engine(self._dbname)
+        self.db = create_engine(self._dbname, echo=False)
         self._metadata = MetaData()
 
         self.seed()
 
     def seed(self):
         if not self.db.dialect.has_table(self.db.connect(), 'conversation_history'):
             Base.metadata.create_all(self.db)
 
-    @staticmethod
-    def transform(data: ConversationHistory) -> PersistenceObject:
-        data_obj = PersistenceObject(
-            uid=data.uid,
-            role=data.role,
-            author=data.author,
-            content=data.content,
-            mention=data.mention,
-            function=data.function,
-            timestamp=data.timestamp,
-            success=data.success
-        )
-        return data_obj
-
     def save(self,
+             cid: str,
              role: str,
              author: str,
              content: str,
              mentions: List[str] = None,
              function: str = None,
              success: bool = True):
         saved_objs = []
         if mentions is None:
             mentions = ['user']
 
         with Session(self.db) as session:
             for mention in mentions:
-                conv_history = ConversationHistory(
+                conv_hist = ConversationHistory(
                     uid=generate_id(16),
+                    cid=cid,
                     role=role,
                     author=author,
                     content=content,
                     mention=mention,
                     function=function,
                     success=success
                 )
-                session.add(conv_history)
-                saved_objs.append(conv_history)
+                session.add(conv_hist)
+                saved_objs.append(conv_hist)
             session.commit()
 
             return list(map(self.transform, saved_objs))
 
-    def find(self, key: str, value: List[str] = None, limit: int = 5):
+    def find(self, conditions: Dict, limit: int = 5):
         with Session(self.db) as session:
-            key_conditions = [getattr(ConversationHistory, key) == val for val in value]
-            key_conditions = or_(*key_conditions)
-
-            mention_conditions = [getattr(ConversationHistory, 'mention') == val for val in value]
-            mention_conditions = or_(*mention_conditions)
-
-            filter_conditions = and_(key_conditions, mention_conditions)
+            filter_conditions = []
+            for key, value in conditions.items():
+                temp_conditions = [getattr(ConversationHistory, key) == val for val in value]
+                temp_conditions = or_(*temp_conditions)
+                filter_conditions.append(temp_conditions)
+            filter_conditions = and_(*filter_conditions)
 
             result = session.query(
                 ConversationHistory
             ).filter(filter_conditions).order_by(ConversationHistory.timestamp.desc()).limit(limit).all()
 
             return list(map(self.transform, result[::-1]))
 
@@ -104,7 +91,9 @@
             filter_conditions = [getattr(ConversationHistory, key) == val for val in value]
             filter_conditions = or_(*filter_conditions)
 
             session.query(ConversationHistory).filter(filter_conditions).delete()
             session.commit()
             return
 
+
+
```

### Comparing `jam_ai-0.1.8/jam/persistence/sqlite.py` & `jam_ai-0.2.0/jam/persistence/postgres.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,79 +8,66 @@
 
 from sqlalchemy import create_engine
 from sqlalchemy import MetaData
 from sqlalchemy import or_, and_
 from sqlalchemy.orm import Session
 
 
-class SQLitePersistence(BasePersistence):
+class PostgresPersistence(BasePersistence):
 
-    def __init__(self, dbname: str = 'sqlite:///jam.db'):
-        super(SQLitePersistence, self).__init__()
+    def __init__(self, dbname: str = 'postgresql+psycopg2://localhost:5432/postgres'):
+        super(PostgresPersistence, self).__init__()
         self._dbname = dbname
         self.db = create_engine(self._dbname)
         self._metadata = MetaData()
 
         self.seed()
 
     def seed(self):
         if not self.db.dialect.has_table(self.db.connect(), 'conversation_history'):
             Base.metadata.create_all(self.db)
 
-    @staticmethod
-    def transform(data: ConversationHistory) -> PersistenceObject:
-        data_obj = PersistenceObject(
-            uid=data.uid,
-            role=data.role,
-            author=data.author,
-            content=data.content,
-            mention=data.mention,
-            function=data.function,
-            timestamp=data.timestamp,
-            success=data.success
-        )
-        return data_obj
-
     def save(self,
+             cid: str,
              role: str,
              author: str,
              content: str,
              mentions: List[str] = None,
              function: str = None,
              success: bool = True):
         saved_objs = []
         if mentions is None:
             mentions = ['user']
 
         with Session(self.db) as session:
             for mention in mentions:
-                conv_hist = ConversationHistory(
+                conv_history = ConversationHistory(
                     uid=generate_id(16),
+                    cid=cid,
                     role=role,
                     author=author,
                     content=content,
                     mention=mention,
                     function=function,
                     success=success
                 )
-                session.add(conv_hist)
-                saved_objs.append(conv_hist)
+                session.add(conv_history)
+                saved_objs.append(conv_history)
             session.commit()
 
             return list(map(self.transform, saved_objs))
 
-    def find(self, key: str, value: List[str] = None, limit: int = 5):
+    def find(self, conditions: Dict, limit: int = 5):
         with Session(self.db) as session:
-            key_conditions = [getattr(ConversationHistory, key) == val for val in value]
-            key_conditions = or_(*key_conditions)
-
-            mention_conditions = [getattr(ConversationHistory, 'mention') == val for val in value]
-            mention_conditions = or_(*mention_conditions)
-
-            filter_conditions = and_(key_conditions, mention_conditions)
+            filter_conditions = []
+            for key, value in conditions.items():
+                temp_conditions = [getattr(ConversationHistory, key) == val for val in value]
+                temp_conditions = or_(*temp_conditions)
+                filter_conditions.append(temp_conditions)
+            filter_conditions = and_(*filter_conditions)
 
             result = session.query(
                 ConversationHistory
             ).filter(filter_conditions).order_by(ConversationHistory.timestamp.desc()).limit(limit).all()
 
             return list(map(self.transform, result[::-1]))
 
@@ -104,9 +91,7 @@
             filter_conditions = [getattr(ConversationHistory, key) == val for val in value]
             filter_conditions = or_(*filter_conditions)
 
             session.query(ConversationHistory).filter(filter_conditions).delete()
             session.commit()
             return
 
-
-
```

### Comparing `jam_ai-0.1.8/tests/instrument/test_base.py` & `jam_ai-0.2.0/tests/instrument/test_base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/tests/interface/test_base.py` & `jam_ai-0.2.0/tests/interface/test_base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/tests/test_persistence/test_base.py` & `jam_ai-0.2.0/tests/test_persistence/test_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,44 +8,48 @@
 from jam.util.generate import generate_id
 
 
 class TestPersistenceObject(unittest.TestCase):
 
     def setUp(self) -> None:
         self.uid_1 = generate_id(16)
+        self.cid_1 = generate_id(16)
         self.author_1 = generate_id(8)
         self.role_1 = generate_id(8)
         self.content_1 = generate_id(8)
         self.mention_1 = self.author_1
         self.function_1 = generate_id(8)
         self.timestamp_1 = datetime.now()
         self.success_1 = True
 
         self.uid_2 = generate_id(16)
+        self.cid_2 = generate_id(16)
         self.author_2 = generate_id(8)
         self.role_2 = generate_id(8)
         self.content_2 = generate_id(8)
         self.mention_2 = self.author_2
         self.function_2 = generate_id(8)
         self.timestamp_2 = datetime.now()
         self.success_2 = False
 
         self.po_1 = PersistenceObject(
             uid=self.uid_1,
+            cid=self.cid_1,
             author=self.author_1,
             role=self.role_1,
             content=self.content_1,
             mention=self.mention_1,
             function=self.function_1,
             timestamp=self.timestamp_1,
             success=self.success_1
         )
 
         self.po_2 = PersistenceObject(
             uid=self.uid_2,
+            cid=self.cid_2,
             author=self.author_2,
             role=self.role_2,
             content=self.content_2,
             mention=self.mention_2,
             function=self.function_2,
             timestamp=self.timestamp_2,
             success=self.success_2
@@ -55,14 +59,18 @@
         self.assertIsInstance(self.po_1, PersistenceObject)
         self.assertIsInstance(self.po_2, PersistenceObject)
 
     def test_class_attribute_uid(self):
         self.assertEqual(self.po_1.uid, self.uid_1)
         self.assertEqual(self.po_2.uid, self.uid_2)
 
+    def test_class_attribute_cid(self):
+        self.assertEqual(self.po_1.cid, self.cid_1)
+        self.assertEqual(self.po_2.cid, self.cid_2)
+
     def test_class_attribute_author(self):
         self.assertEqual(self.po_1.author, self.author_1)
         self.assertEqual(self.po_2.author, self.author_2)
 
     def test_class_attribute_role(self):
         self.assertEqual(self.po_1.role, self.role_1)
         self.assertEqual(self.po_2.role, self.role_2)
@@ -103,27 +111,29 @@
         self.assertEqual(self.po_2_m.get('content'), self.po_2.content)
         self.assertEqual(self.po_2_m.get('name'), self.po_2.function)
 
 
 class AlterPersistence(BasePersistence):
 
     def save(self,
+             cid: str,
              role: str,
              author: str,
              content: str,
              mentions: List[str] = None,
              function: str = None,
              success: bool = True):
         saved_objs = []
         if mentions is None:
             mentions = ['user']
 
         for mention in mentions:
             data_obj = PersistenceObject(
                 uid=generate_id(16),
+                cid=cid,
                 role=role,
                 author=author,
                 content=content,
                 mention=mention,
                 function=function,
                 timestamp=datetime.now(),
                 success=success
@@ -134,31 +144,34 @@
 
 class TestBasePersistence(unittest.TestCase):
 
     def setUp(self) -> None:
         self.per_1 = BasePersistence()
         self.per_2 = AlterPersistence()
 
+        self.cid_2 = generate_id(16)
         self.role_2 = generate_id(8)
         self.author_2 = generate_id(8)
         self.content_2 = generate_id(8)
         self.mention_2 = [self.author_2]
         self.function_2 = generate_id(8)
 
         self.per_2_saved = self.per_2.save(
+            cid=self.cid_2,
             role=self.role_2,
             author=self.author_2,
             content=self.content_2,
             mentions=self.mention_2,
             function=self.function_2
         )
 
         self.per_2_saved_mock = [
             PersistenceObject(
                 uid=generate_id(16),
+                cid=self.cid_2,
                 role=self.role_2,
                 author=self.author_2,
                 content=self.content_2,
                 mention=self.author_2,
                 function=self.function_2,
                 timestamp=datetime.now()
             )
@@ -166,17 +179,18 @@
 
     def test_class_identity(self):
         self.assertIsInstance(self.per_1, BasePersistence)
         self.assertIsInstance(self.per_2, AlterPersistence)
 
     def test_class_method_save(self):
         self.assertEqual(self.per_1.save(
-            role='', author='', content=''
+            cid=self.cid_2, role='', author='', content=''
         ), [])
 
         self.assertEqual(len(self.per_2_saved), len(self.per_2_saved_mock))
+        self.assertEqual(self.per_2_saved[0].cid, self.per_2_saved_mock[0].cid)
         self.assertEqual(self.per_2_saved[0].role, self.per_2_saved_mock[0].role)
         self.assertEqual(self.per_2_saved[0].author, self.per_2_saved_mock[0].author)
         self.assertEqual(self.per_2_saved[0].content, self.per_2_saved_mock[0].content)
         self.assertEqual(self.per_2_saved[0].mention, self.per_2_saved_mock[0].mention)
         self.assertEqual(self.per_2_saved[0].function, self.per_2_saved_mock[0].function)
         self.assertEqual(self.per_2_saved[0].success, self.per_2_saved_mock[0].success)
```

### Comparing `jam_ai-0.1.8/.gitignore` & `jam_ai-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/LICENSE` & `jam_ai-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.8/README.md` & `jam_ai-0.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 # Jam.AI
 
-> Create Jam session with AI
-
 Jam is an experimental collaboration tool to use multiple AI personnel together equipped with instructed function calls.
 
+> Create Jam session with AI
+
 [View Changelog](https://github.com/abhishtagatya/jam/blob/master/CHANGELOG.md)
 
 ![Demo](https://raw.githubusercontent.com/abhishtagatya/jam/master/docs/demo.png)
 
 ## Quick Start
 
 ```python
 from jam import Jam
-from jam.personnel import BasicPersonnel
+from jam.personnel import BasicPersonnel, AutoPersonnel
 from jam.instrument import PromptPainter
 
 jam_room = Jam(
     members=[
-        BasicPersonnel.from_json('albert-einstein.json'),
-        BasicPersonnel.from_json('stephen-hawking.json')
+        BasicPersonnel.from_json(filepath='example/personnel/claude-monet.json'),  # Using custom JSON
+        BasicPersonnel.from_preset(name='pablo-picasso'),  # Using example presets from Git
+        AutoPersonnel.from_prompt(uid='wkandinsky', prompt='Wassily Kandinsky')  # Using GPT to build prompt
     ],
     instruments=[PromptPainter()]
 )
 
 prompt = jam_room.compose(
-    message='Give me a question',
+    message='who are you!',
     multi=True
 )
 
+print(prompt) # List of Prompts from Characters
+
 ```
 
 Don't forget to use your credentials. Primarily for OpenAI, the core engine of this project. 
 https://platform.openai.com/account/api-keys
 
 ```bash
 export OPENAI_KEY=YOUR_KEY
@@ -53,14 +56,21 @@
 Extra Requirements for Function Calls
 * Psycopg2
 * PyMySQL
 * Stability SDK
 
 ### Extension
 
+Optional dependencies to fit any requirement needed.
+
+```bash
+pip install jam-ai[database] # Using Postgres, MySQL, Redis ...
+pip install jam-ai[function] # Using Extended Function Calls requiring SDKs / Packages
+```
+
 For the use of other libraries, please consider to always feed in your API Keys respectively. See below for example.
 
 ```bash
 export STABILITY_KEY=YOUR_STABILITY_AI_KEY # If you are using Stability SDK
 export WRITESONIC_KEY=YOUR_WRITE_SONIC_KEY # If you are using WriteSonic API
 export CUSTOM_KEY=YOUR_CUSTOM_KEY          # If there are any other added functionalities
 ```
```

### Comparing `jam_ai-0.1.8/pyproject.toml` & `jam_ai-0.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jam-ai"
-version = "0.1.8"
+version = "0.2.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 authors = [
   { name="Abhishta Gatya", email="abhishtagatya@yahoo.com" },
 ]
 description = "Engaging with Multiple AI Agents with Jam."
 keywords = ["openai", "multi agent", "chat engine", "collaboration", "machine learning", "data science"]
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
 dependencies = [
     'openai',
     'Pillow',
     'requests',
     'SQLAlchemy',
-    'psycopg2',
-    'pymysql',
-    'stability-sdk',
     'rich',
 ]
 classifiers = [
     'License :: OSI Approved :: Apache Software License',
     'Development Status :: 3 - Alpha',
     # 'Development Status :: 4 - Beta',
     # 'Development Status :: 5 - Production/Stable',
@@ -38,17 +35,14 @@
 
     'Topic :: Adaptive Technologies',
     'Topic :: Communications :: Chat',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'Topic :: Software Development :: Libraries',
     'Topic :: Software Development :: Libraries :: Python Modules',
 
-    'Programming Language :: Python :: 3.6',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
 
     'Natural Language :: English',
 ]
 
@@ -57,11 +51,21 @@
   "jam/*",
   "/jam/*/*",
   "/tests/*",
   "/example/*",
   "/cmd/*",
 ]
 
+[tool.hatch.extras]
+database = [
+    'pymysql',
+    'psycopg2',
+]
+
+function = [
+    'stability-sdk',
+]
+
 [project.urls]
 homepage = "https://github.com/abhishtagatya/jam"
 documentation = "https://github.com/abhishtagatya/jam"
 changelog = "https://github.com/abhishtagatya/jam/blob/master/CHANGELOG.md"
```

### Comparing `jam_ai-0.1.8/PKG-INFO` & `jam_ai-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jam-ai
-Version: 0.1.8
+Version: 0.2.0
 Summary: Engaging with Multiple AI Agents with Jam.
 Project-URL: homepage, https://github.com/abhishtagatya/jam
 Project-URL: documentation, https://github.com/abhishtagatya/jam
 Project-URL: changelog, https://github.com/abhishtagatya/jam/blob/master/CHANGELOG.md
 Author-email: Abhishta Gatya <abhishtagatya@yahoo.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
@@ -213,66 +213,63 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Adaptive Technologies
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Requires-Dist: openai
 Requires-Dist: pillow
-Requires-Dist: psycopg2
-Requires-Dist: pymysql
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: sqlalchemy
-Requires-Dist: stability-sdk
 Description-Content-Type: text/markdown
 
 # Jam.AI
 
-> Create Jam session with AI
-
 Jam is an experimental collaboration tool to use multiple AI personnel together equipped with instructed function calls.
 
+> Create Jam session with AI
+
 [View Changelog](https://github.com/abhishtagatya/jam/blob/master/CHANGELOG.md)
 
 ![Demo](https://raw.githubusercontent.com/abhishtagatya/jam/master/docs/demo.png)
 
 ## Quick Start
 
 ```python
 from jam import Jam
-from jam.personnel import BasicPersonnel
+from jam.personnel import BasicPersonnel, AutoPersonnel
 from jam.instrument import PromptPainter
 
 jam_room = Jam(
     members=[
-        BasicPersonnel.from_json('albert-einstein.json'),
-        BasicPersonnel.from_json('stephen-hawking.json')
+        BasicPersonnel.from_json(filepath='example/personnel/claude-monet.json'),  # Using custom JSON
+        BasicPersonnel.from_preset(name='pablo-picasso'),  # Using example presets from Git
+        AutoPersonnel.from_prompt(uid='wkandinsky', prompt='Wassily Kandinsky')  # Using GPT to build prompt
     ],
     instruments=[PromptPainter()]
 )
 
 prompt = jam_room.compose(
-    message='Give me a question',
+    message='who are you!',
     multi=True
 )
 
+print(prompt) # List of Prompts from Characters
+
 ```
 
 Don't forget to use your credentials. Primarily for OpenAI, the core engine of this project. 
 https://platform.openai.com/account/api-keys
 
 ```bash
 export OPENAI_KEY=YOUR_KEY
@@ -294,14 +291,21 @@
 Extra Requirements for Function Calls
 * Psycopg2
 * PyMySQL
 * Stability SDK
 
 ### Extension
 
+Optional dependencies to fit any requirement needed.
+
+```bash
+pip install jam-ai[database] # Using Postgres, MySQL, Redis ...
+pip install jam-ai[function] # Using Extended Function Calls requiring SDKs / Packages
+```
+
 For the use of other libraries, please consider to always feed in your API Keys respectively. See below for example.
 
 ```bash
 export STABILITY_KEY=YOUR_STABILITY_AI_KEY # If you are using Stability SDK
 export WRITESONIC_KEY=YOUR_WRITE_SONIC_KEY # If you are using WriteSonic API
 export CUSTOM_KEY=YOUR_CUSTOM_KEY          # If there are any other added functionalities
 ```
```

