# Comparing `tmp/jtim_enc-0.0.2.tar.gz` & `tmp/jtim_enc-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jtim_enc-0.0.2.tar", last modified: Tue Jul 18 13:56:58 2023, max compression
+gzip compressed data, was "jtim_enc-0.1.tar", last modified: Sun Jul 16 02:00:42 2023, max compression
```

## Comparing `jtim_enc-0.0.2.tar` & `jtim_enc-0.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 jeefy     (1000) jeefy     (1000)        0 2023-07-18 13:56:58.193198 jtim_enc-0.0.2/
--rw-rw-r--   0 jeefy     (1000) jeefy     (1000)      592 2023-07-18 13:56:58.193198 jtim_enc-0.0.2/PKG-INFO
--rw-rw-r--   0 jeefy     (1000) jeefy     (1000)      205 2023-07-18 13:51:52.000000 jtim_enc-0.0.2/README.md
-drwxrwxr-x   0 jeefy     (1000) jeefy     (1000)        0 2023-07-18 13:56:58.193198 jtim_enc-0.0.2/jtim_enc/
--rw-rw-r--   0 jeefy     (1000) jeefy     (1000)       95 2023-07-18 13:51:52.000000 jtim_enc-0.0.2/jtim_enc/__init__.py
--rw-rw-r--   0 jeefy     (1000) jeefy     (1000)     2623 2023-07-18 13:55:03.000000 jtim_enc-0.0.2/jtim_enc/encryptor.py
-drwxrwxr-x   0 jeefy     (1000) jeefy     (1000)        0 2023-07-18 13:56:58.193198 jtim_enc-0.0.2/jtim_enc.egg-info/
--rw-rw-r--   0 jeefy     (1000) jeefy     (1000)      592 2023-07-18 13:56:58.000000 jtim_enc-0.0.2/jtim_enc.egg-info/PKG-INFO
--rw-rw-r--   0 jeefy     (1000) jeefy     (1000)      205 2023-07-18 13:56:58.000000 jtim_enc-0.0.2/jtim_enc.egg-info/SOURCES.txt
--rw-rw-r--   0 jeefy     (1000) jeefy     (1000)        1 2023-07-18 13:56:58.000000 jtim_enc-0.0.2/jtim_enc.egg-info/dependency_links.txt
--rw-rw-r--   0 jeefy     (1000) jeefy     (1000)        9 2023-07-18 13:56:58.000000 jtim_enc-0.0.2/jtim_enc.egg-info/top_level.txt
--rw-rw-r--   0 jeefy     (1000) jeefy     (1000)      103 2023-07-18 13:51:52.000000 jtim_enc-0.0.2/pyproject.toml
--rw-rw-r--   0 jeefy     (1000) jeefy     (1000)      490 2023-07-18 13:56:58.193198 jtim_enc-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-16 02:00:42.455385 jtim_enc-0.1/
+-rw-rw-rw-   0        0        0      614 2023-07-16 02:00:42.457380 jtim_enc-0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-07-16 01:59:50.000000 jtim_enc-0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 02:00:42.431352 jtim_enc-0.1/jtim_enc/
+-rw-rw-rw-   0        0        0       98 2023-07-16 01:49:26.000000 jtim_enc-0.1/jtim_enc/__init__.py
+-rw-rw-rw-   0        0        0     2690 2023-07-14 23:45:49.000000 jtim_enc-0.1/jtim_enc/encryptor.py
+drwxrwxrwx   0        0        0        0 2023-07-16 02:00:42.450351 jtim_enc-0.1/jtim_enc.egg-info/
+-rw-rw-rw-   0        0        0      614 2023-07-16 02:00:42.000000 jtim_enc-0.1/jtim_enc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-07-16 02:00:42.000000 jtim_enc-0.1/jtim_enc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 02:00:42.000000 jtim_enc-0.1/jtim_enc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-16 02:00:42.000000 jtim_enc-0.1/jtim_enc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-07-16 01:50:31.000000 jtim_enc-0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      492 2023-07-16 02:00:42.475395 jtim_enc-0.1/setup.cfg
+-rw-rw-rw-   0        0        0      137 2023-07-15 13:44:47.000000 jtim_enc-0.1/setup.py
```

### Comparing `jtim_enc-0.0.2/PKG-INFO` & `jtim_enc-0.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
-Name: jtim_enc
-Version: 0.0.2
-Summary: Randomized Base64 codec
-Home-page: https://gitlab.com/jeefies/jtim-enc
-Author: Jeefy
-Author-email: jeefy163@163.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-# jtim-enc
-
-**Jeefy's time encryptor**....
-
-Would fucking use in nowhere...
-
-## Techniques
-
-采用随机化的类 base64 编码。思路很简单，实现也非常容易。
-
-具体内容见目录文件。
+Metadata-Version: 2.1
+Name: jtim_enc
+Version: 0.1
+Summary: Randomized Base64 codec
+Home-page: https://gitlab.com/jeefies/jtim-enc
+Author: Jeefy
+Author-email: jeefy163@163.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+# jtim-enc
+
+**Jeefy's time encryptor**....
+
+Would fucking use in nowhere...
+
+## Techniques
+
+采用随机化的类 base64 编码。思路很简单，实现也非常容易。
+
+具体内容见目录文件。
```

### Comparing `jtim_enc-0.0.2/jtim_enc/encryptor.py` & `jtim_enc-0.1/jtim_enc/encryptor.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,98 +1,96 @@
-import math
-import random
-
-from time import time
-from typing import Optional
-
-charSet = b"ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789.+-*/?,<>';:[]{}|_=!@#$%^&()"
-
-globalRandom = random.Random(time())
-
-class Encryptor:
-    timeSeed : int
-    baseCodes : list[int]
-    def __init__(self, seed: Optional[int] = None):
-        if seed is None:
-            seed = time()
-
-        self.timeSeed = int(seed) & 0xFFFFFFFF
-        rand = random.Random(self.timeSeed)
-
-        self.baseCodes = list(charSet)
-        rand.shuffle(self.baseCodes)
-
-    def _header(self) -> bytes:
-        offset = globalRandom.randint(20, 62)
-        head = offset.to_bytes(1, 'big')
-        for i in range(7):
-            head += (((self.timeSeed >> (i * 5)) & 0b11111) ^ offset).to_bytes(1, 'big')
-        return head
-    
-    def encrypt(self, text: bytes) -> bytes:
-        bin_str = ""
-        for ch in text:
-            bin_str += bin(ch)[2:].zfill(8)
-        
-        blocks = math.ceil(len(bin_str) / 6)
-        if len(bin_str) % 6 != 0:
-            bin_str += ''.join(['0'] * (blocks * 6 - len(bin_str)))
-        
-        enc_str = b""
-        for bi in range(int(blocks)):
-            idx = int(bin_str[bi * 6: bi * 6 + 6], base=2)
-            enc_str += self.baseCodes[idx].to_bytes(1, 'big')
-        
-        return self._header() + enc_str
-        
-class Decryptor:
-    baseCodes : list[int]
-    def __init__(self):
-        self.baseCodes = charSet
-        
-    def decrypt(self, text : bytes) -> bytes:
-        offset = text[0]
-        header = text[1:8]
-        
-        seed = 0
-        for i in range(7):
-            seed += (header[i] ^ offset) << (i * 5)
-        
-        baseCodes = list(self.baseCodes)
-        rand = random.Random(seed)
-        rand.shuffle(baseCodes)
-        
-        mapCodes = { code : bin(i)[2:].zfill(6) for i, code in enumerate(baseCodes) }
-        
-        bin_str = ""
-        for code in text[8:]:
-            bin_str += mapCodes[code]
-        
-        dec_str = b""
-        blocks = math.floor(len(bin_str) / 8)
-        for bi in range(blocks):
-            bs = bin_str[bi * 8 : bi * 8 + 8]
-            dec_str += int(bs, base=2).to_bytes(1, 'big')
-        
-        return dec_str
-        
-
-if __name__ == '__main__':
-    enc = Encryptor()
-    print(enc._header())
-    
-    pwd = enc.encrypt(b"Hello World")
-    print("encrypt result: ", pwd)
-    
-    dec = Decryptor()
-    ori = dec.decrypt(pwd)
-    print(ori)
-    
-    chtext = "你知道fyk是个傻逼吗？".encode()
-    
-    pwd = enc.encrypt(chtext)
-    print("encrypt result: ", pwd)
-    
-    ori = dec.decrypt(pwd)
-    print(ori.decode())
-    
-    
+import math
+import random
+
+from time import time
+from typing import Optional
+
+charSet = b"ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789.+-*/?,<>';:[]{}|_=!@#$%^&()"
+
+class Encryptor:
+    timeSeed : int
+    baseCodes : list[int]
+    def __init__(self, seed: Optional[int] = None):
+        if seed is None:
+            seed = time()
+
+        self.timeSeed = int(seed) & 0xFFFFFFFF
+        rand = random.Random(self.timeSeed)
+
+        self.baseCodes = list(charSet)
+        rand.shuffle(self.baseCodes)
+
+    def _header(self) -> bytes:
+        offset = random.Random(time()).randint(20, 62)
+        head = offset.to_bytes(1, 'big')
+        for i in range(7):
+            head += (((self.timeSeed >> (i * 5)) & 0b11111) + offset).to_bytes(1, 'big')
+        return head
+    
+    def encrypt(self, text: bytes) -> bytes:
+        bin_str = ""
+        for ch in text:
+            bin_str += bin(ch)[2:].zfill(8)
+        
+        blocks = math.ceil(len(bin_str) / 6)
+        if len(bin_str) % 6 != 0:
+            bin_str += ''.join(['0'] * (blocks * 6 - len(bin_str)))
+        
+        enc_str = b""
+        for bi in range(int(blocks)):
+            idx = int(bin_str[bi * 6: bi * 6 + 6], base=2)
+            enc_str += self.baseCodes[idx].to_bytes(1, 'big')
+        
+        return self._header() + enc_str
+        
+class Decryptor:
+    baseCodes : list[int]
+    def __init__(self):
+        self.baseCodes = charSet
+        
+    def decrypt(self, text : bytes) -> bytes:
+        offset = text[0]
+        header = text[1:8]
+        
+        seed = 0
+        for i in range(7):
+            seed += (header[i] - offset) << (i * 5)
+        
+        baseCodes = list(self.baseCodes)
+        rand = random.Random(seed)
+        rand.shuffle(baseCodes)
+        
+        mapCodes = { code : bin(i)[2:].zfill(6) for i, code in enumerate(baseCodes) }
+        
+        bin_str = ""
+        for code in text[8:]:
+            bin_str += mapCodes[code]
+        
+        dec_str = b""
+        blocks = math.floor(len(bin_str) / 8)
+        for bi in range(blocks):
+            bs = bin_str[bi * 8 : bi * 8 + 8]
+            dec_str += int(bs, base=2).to_bytes(1, 'big')
+        
+        return dec_str
+        
+
+if __name__ == '__main__':
+    enc = Encryptor()
+    print(enc._header())
+    
+    pwd = enc.encrypt(b"Hello World")
+    print("encrypt result: ", pwd)
+    
+    dec = Decryptor()
+    ori = dec.decrypt(pwd)
+    print(ori)
+    
+    chtext = "你知道fyk是个傻逼吗？".encode()
+    
+    pwd = enc.encrypt(chtext)
+    print("encrypt result: ", pwd)
+    
+    ori = dec.decrypt(pwd)
+    print(ori.decode())
+    
+
```

### Comparing `jtim_enc-0.0.2/jtim_enc.egg-info/PKG-INFO` & `jtim_enc-0.1/jtim_enc.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
-Name: jtim-enc
-Version: 0.0.2
-Summary: Randomized Base64 codec
-Home-page: https://gitlab.com/jeefies/jtim-enc
-Author: Jeefy
-Author-email: jeefy163@163.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-# jtim-enc
-
-**Jeefy's time encryptor**....
-
-Would fucking use in nowhere...
-
-## Techniques
-
-采用随机化的类 base64 编码。思路很简单，实现也非常容易。
-
-具体内容见目录文件。
+Metadata-Version: 2.1
+Name: jtim-enc
+Version: 0.1
+Summary: Randomized Base64 codec
+Home-page: https://gitlab.com/jeefies/jtim-enc
+Author: Jeefy
+Author-email: jeefy163@163.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+# jtim-enc
+
+**Jeefy's time encryptor**....
+
+Would fucking use in nowhere...
+
+## Techniques
+
+采用随机化的类 base64 编码。思路很简单，实现也非常容易。
+
+具体内容见目录文件。
```

