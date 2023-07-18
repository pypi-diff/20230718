# Comparing `tmp/PyDeepLX-1.0.3.tar.gz` & `tmp/PyDeepLX-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDeepLX-1.0.3.tar", last modified: Sat May 20 20:12:20 2023, max compression
+gzip compressed data, was "PyDeepLX-1.0.4.tar", last modified: Tue Jul 18 04:59:14 2023, max compression
```

## Comparing `PyDeepLX-1.0.3.tar` & `PyDeepLX-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:12:20.717016 PyDeepLX-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-20 20:12:06.000000 PyDeepLX-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-20 20:12:20.717016 PyDeepLX-1.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:12:20.713016 PyDeepLX-1.0.3/PyDeepLX/
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-20 20:12:06.000000 PyDeepLX-1.0.3/PyDeepLX/PyDeepLX.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-20 20:12:06.000000 PyDeepLX-1.0.3/PyDeepLX/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:12:20.717016 PyDeepLX-1.0.3/PyDeepLX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-20 20:12:20.000000 PyDeepLX-1.0.3/PyDeepLX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-20 20:12:20.000000 PyDeepLX-1.0.3/PyDeepLX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 20:12:20.000000 PyDeepLX-1.0.3/PyDeepLX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 20:12:20.000000 PyDeepLX-1.0.3/PyDeepLX.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-20 20:12:20.000000 PyDeepLX-1.0.3/PyDeepLX.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-20 20:12:20.000000 PyDeepLX-1.0.3/PyDeepLX.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-20 20:12:06.000000 PyDeepLX-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 20:12:20.717016 PyDeepLX-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-20 20:12:06.000000 PyDeepLX-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:59:14.217773 PyDeepLX-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-18 04:59:01.000000 PyDeepLX-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-18 04:59:14.217773 PyDeepLX-1.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:59:14.217773 PyDeepLX-1.0.4/PyDeepLX/
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-18 04:59:01.000000 PyDeepLX-1.0.4/PyDeepLX/PyDeepLX.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-18 04:59:01.000000 PyDeepLX-1.0.4/PyDeepLX/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:59:14.217773 PyDeepLX-1.0.4/PyDeepLX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-18 04:59:14.000000 PyDeepLX-1.0.4/PyDeepLX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-18 04:59:14.000000 PyDeepLX-1.0.4/PyDeepLX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 04:59:14.000000 PyDeepLX-1.0.4/PyDeepLX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 04:59:14.000000 PyDeepLX-1.0.4/PyDeepLX.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-18 04:59:14.000000 PyDeepLX-1.0.4/PyDeepLX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 04:59:14.000000 PyDeepLX-1.0.4/PyDeepLX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-18 04:59:01.000000 PyDeepLX-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 04:59:14.217773 PyDeepLX-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-18 04:59:01.000000 PyDeepLX-1.0.4/setup.py
```

### Comparing `PyDeepLX-1.0.3/LICENSE` & `PyDeepLX-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyDeepLX-1.0.3/PKG-INFO` & `PyDeepLX-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDeepLX
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python package for unlimited DeepL translation
 Home-page: https://github.com/OwO-Network/PyDeepLX
 Author: missuo
 Author-email: i@yyt.moe
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
@@ -22,46 +22,53 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyDeepLX
+
 A Python package for unlimited DeepL translation
 
 ## API Version
+
 [OwO-Network/DeepLX](https://github.com/OwO-Network/DeepLX): Permanently free DeepL API written in Golang.
 
 ## Description
+
 This is a Python package for DeepL translation, I didn't limit the number of translations in the code, if there is a `429` error, it means your IP has been blocked by DeepL temporarily, please don't request it frequently in a short time.
 
 ## Usage
+
 ### Install Package
+
 ```bash
 pip install PyDeepLX
 ```
+
 ### Use in code
+
 ```python
 from PyDeepLX import PyDeepLX
 # By default, the source language is automatically recognized and translated into English without providing any alternative results.
 PyDeepLX.translate("你好世界") # Return String
 
 # Specify the source and target languages
 PyDeepLX.translate("你好世界", "ZH", "EN") # Return String
 
 # Need alternative results
-PyDeepLX.translate("毫无疑问的", "ZH", "EN", True) # Return List: ['Without a doubt', 'No doubt']
+PyDeepLX.translate("毫无疑问的", "ZH", "EN", 2) # Return List: ['Without a doubt', 'No doubt']
 
 # Print the results
 PyDeepLX.translate("毫无疑问的", "ZH", "EN", True, True)
 
 # Using proxy
-PyDeepLX.translate(text="毫无疑问的", sourceLang="ZH", targetLang="EN", needAlternative=False, printResult=False, proxies="socks5://127.0.0.1:7890")
+PyDeepLX.translate(text="毫无疑问的", sourceLang="ZH", targetLang="EN", numberAlternative=0, printResult=False, proxies="socks5://127.0.0.1:7890")
 ```
 
 ## PyPi
+
 <a href="https://pypi.org/project/PyDeepLX/"><img src="https://img.shields.io/badge/Pypi-000000?style=for-the-badge&logo=pypi&logoColor=red" /></a>
 
 ## Author
 
 **PyDeepLX** © [Vincent Young](https://github.com/missuo), Released under the [MIT](./LICENSE) License.<br>
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyDeepLX Version: 1.0.3 Summary: A Python package
+Metadata-Version: 2.1 Name: PyDeepLX Version: 1.0.4 Summary: A Python package
 for unlimited DeepL translation Home-page: https://github.com/OwO-Network/
 PyDeepLX Author: missuo Author-email: i@yyt.moe License: MIT Platform: any
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.3 Classifier: Programming
 Language :: Python :: 3.4 Classifier: Programming Language :: Python :: 3.5
@@ -19,15 +19,15 @@
 a `429` error, it means your IP has been blocked by DeepL temporarily, please
 don't request it frequently in a short time. ## Usage ### Install Package
 ```bash pip install PyDeepLX ``` ### Use in code ```python from PyDeepLX import
 PyDeepLX # By default, the source language is automatically recognized and
 translated into English without providing any alternative results.
 PyDeepLX.translate("ä½ å¥½ä¸ç") # Return String # Specify the source and
 target languages PyDeepLX.translate("ä½ å¥½ä¸ç", "ZH", "EN") # Return String
-# Need alternative results PyDeepLX.translate("æ¯«æ çé®ç", "ZH", "EN",
-True) # Return List: ['Without a doubt', 'No doubt'] # Print the results
+# Need alternative results PyDeepLX.translate("æ¯«æ çé®ç", "ZH", "EN", 2)
+# Return List: ['Without a doubt', 'No doubt'] # Print the results
 PyDeepLX.translate("æ¯«æ çé®ç", "ZH", "EN", True, True) # Using proxy
 PyDeepLX.translate(text="æ¯«æ çé®ç", sourceLang="ZH", targetLang="EN",
-needAlternative=False, printResult=False, proxies="socks5://127.0.0.1:7890")
-``` ## PyPi [https://img.shields.io/badge/Pypi-000000?style=for-the-
+numberAlternative=0, printResult=False, proxies="socks5://127.0.0.1:7890") ```
+## PyPi [https://img.shields.io/badge/Pypi-000000?style=for-the-
 badge&logo=pypi&logoColor=red] ## Author **PyDeepLX** Â© [Vincent Young](https:
 //github.com/missuo), Released under the [MIT](./LICENSE) License.
```

### Comparing `PyDeepLX-1.0.3/PyDeepLX/PyDeepLX.py` & `PyDeepLX-1.0.4/PyDeepLX/PyDeepLX.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-'''
+"""
 Author: Vincent Young
 Date: 2023-04-27 00:44:01
 LastEditors: Vincent Young
 LastEditTime: 2023-05-21 03:58:18
 FilePath: /PyDeepLX/PyDeepLX/PyDeepLX.py
 Telegram: https://t.me/missuo
 
 Copyright © 2023 by Vincent, All Rights Reserved. 
-'''
+"""
 import random
 import time
 import json
 import httpx
 from langdetect import detect
 
 
@@ -20,110 +20,121 @@
     "Content-Type": "application/json",
     "Accept": "*/*",
     "x-app-os-name": "iOS",
     "x-app-os-version": "16.3.0",
     "Accept-Language": "en-US,en;q=0.9",
     "Accept-Encoding": "gzip, deflate, br",
     "x-app-device": "iPhone13,2",
-    "User-Agent": "DeepL-iOS/2.6.0 iOS 16.3.0 (iPhone13,2)",
-    "x-app-build": "353933",
-    "x-app-version": "2.6",
-    "Connection": "keep-alive"
+    "User-Agent": "DeepL-iOS/2.9.1 iOS 16.3.0 (iPhone13,2)",
+    "x-app-build": "510265",
+    "x-app-version": "2.9.1",
+    "Connection": "keep-alive",
 }
 
 
 class TooManyRequestsException(Exception):
     "Raised when there is a 429 error"
+
     def __str__(self):
         return "PyDeepLX Error: Too many requests, your IP has been blocked by DeepL temporarily, please don't request it frequently in a short time."
 
 
 def detectLang(translateText) -> str:
     language = detect(translateText)
     return language.upper()
 
+
 def getICount(translateText) -> int:
-    return translateText.count('i')
+    return translateText.count("i")
 
 
 def getRandomNumber() -> int:
     random.seed(time.time())
     num = random.randint(8300000, 8399998)
     return num * 1000
 
 
 def getTimestamp(iCount: int) -> int:
     ts = int(time.time() * 1000)
-    if iCount != 0:
-        iCount += 1
-        return ts - ts % iCount + iCount
-    else:
+
+    if iCount == 0:
         return ts
 
+    iCount += 1
+    return ts - ts % iCount + iCount
+
 
-def translate(text, sourceLang=None, targetLang=None, needAlternative=False, printResult=False, proxies=None):
+def translate(
+    text,
+    sourceLang=None,
+    targetLang=None,
+    numberAlternative=0,
+    printResult=False,
+    proxies=None,
+):
     iCount = getICount(text)
     id = getRandomNumber()
-    if sourceLang == None:
+
+    if sourceLang is None:
         sourceLang = detectLang(text)
-    if targetLang == None:
+    if targetLang is None:
         targetLang = "EN"
 
+    numberAlternative = max(min(3, numberAlternative), 0)
+
     postData = {
         "jsonrpc": "2.0",
         "method": "LMT_handle_texts",
         "id": id,
         "params": {
-            "texts": [{
-                "text": text,
-                "requestAlternatives": 3
-            }],
+            "texts": [{"text": text, "requestAlternatives": numberAlternative}],
             "splitting": "newlines",
             "lang": {
                 "source_lang_user_selected": sourceLang,
                 "target_lang": targetLang,
             },
             "timestamp": getTimestamp(iCount),
             "commonJobParams": {
                 "wasSpoken": False,
                 "transcribe_as": "",
-            }}
+            },
+        },
     }
     postDataStr = json.dumps(postData, ensure_ascii=False)
 
-    if (id+5) % 29 == 0 or (id+3) % 13 == 0:
-        postDataStr = postDataStr.replace(
-            "\"method\":\"", "\"method\" : \"", -1)
+    if (id + 5) % 29 == 0 or (id + 3) % 13 == 0:
+        postDataStr = postDataStr.replace('"method":"', '"method" : "', -1)
     else:
-        postDataStr = postDataStr.replace(
-            "\"method\":\"", "\"method\": \"", -1)
-        
+        postDataStr = postDataStr.replace('"method":"', '"method": "', -1)
+
     # Add proxy (e.g. proxies='socks5://127.0.0.1:7890')
     with httpx.Client(proxies=proxies) as client:
         resp = client.post(url=deeplAPI, data=postDataStr, headers=headers)
         respStatusCode = resp.status_code
+
+        if respStatusCode == 429:
+            raise TooManyRequestsException
+
+        if respStatusCode != 200:
+            print("Error", respStatusCode)
+            return
+
         respText = resp.text
         respJson = json.loads(respText)
+
+        if numberAlternative <= 1:
+            targetText = respJson["result"]["texts"][0]["text"]
+            if printResult:
+                print(targetText)
+            return targetText
+
         targetTextArray = []
-        if respStatusCode == 200:
-            if needAlternative == True:
-                targetText = respJson["result"]["texts"][0]["text"]
-                if printResult == True:
-                    print(targetText)
-                for item in respJson["result"]["texts"][0]["alternatives"]:
-                    targetTextArray.append(item["text"])
-                    if printResult == True:
-                        print(item["text"])
-                return targetTextArray
-            else:
-                targetText = respJson["result"]["texts"][0]["text"]
-                if printResult == True:
-                    print(targetText)
-                return targetText
-        elif respStatusCode == 429:
-            raise TooManyRequestsException
-        else:
-            print("Error", respStatusCode)
-            return None
+        for item in respJson["result"]["texts"][0]["alternatives"]:
+            targetTextArray.append(item["text"])
+            if printResult:
+                print(item["text"])
+
+        return targetTextArray
+
 
 # Example Call
-# translate("明天你好", "ZH", "EN", True, True, "socks5://127.0.0.1:7890")
+# translate("明天你好", "ZH", "EN", True, True, "socks5://127.0.0.1:7890")
```

### Comparing `PyDeepLX-1.0.3/PyDeepLX.egg-info/PKG-INFO` & `PyDeepLX-1.0.4/PyDeepLX.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDeepLX
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python package for unlimited DeepL translation
 Home-page: https://github.com/OwO-Network/PyDeepLX
 Author: missuo
 Author-email: i@yyt.moe
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
@@ -22,46 +22,53 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyDeepLX
+
 A Python package for unlimited DeepL translation
 
 ## API Version
+
 [OwO-Network/DeepLX](https://github.com/OwO-Network/DeepLX): Permanently free DeepL API written in Golang.
 
 ## Description
+
 This is a Python package for DeepL translation, I didn't limit the number of translations in the code, if there is a `429` error, it means your IP has been blocked by DeepL temporarily, please don't request it frequently in a short time.
 
 ## Usage
+
 ### Install Package
+
 ```bash
 pip install PyDeepLX
 ```
+
 ### Use in code
+
 ```python
 from PyDeepLX import PyDeepLX
 # By default, the source language is automatically recognized and translated into English without providing any alternative results.
 PyDeepLX.translate("你好世界") # Return String
 
 # Specify the source and target languages
 PyDeepLX.translate("你好世界", "ZH", "EN") # Return String
 
 # Need alternative results
-PyDeepLX.translate("毫无疑问的", "ZH", "EN", True) # Return List: ['Without a doubt', 'No doubt']
+PyDeepLX.translate("毫无疑问的", "ZH", "EN", 2) # Return List: ['Without a doubt', 'No doubt']
 
 # Print the results
 PyDeepLX.translate("毫无疑问的", "ZH", "EN", True, True)
 
 # Using proxy
-PyDeepLX.translate(text="毫无疑问的", sourceLang="ZH", targetLang="EN", needAlternative=False, printResult=False, proxies="socks5://127.0.0.1:7890")
+PyDeepLX.translate(text="毫无疑问的", sourceLang="ZH", targetLang="EN", numberAlternative=0, printResult=False, proxies="socks5://127.0.0.1:7890")
 ```
 
 ## PyPi
+
 <a href="https://pypi.org/project/PyDeepLX/"><img src="https://img.shields.io/badge/Pypi-000000?style=for-the-badge&logo=pypi&logoColor=red" /></a>
 
 ## Author
 
 **PyDeepLX** © [Vincent Young](https://github.com/missuo), Released under the [MIT](./LICENSE) License.<br>
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyDeepLX Version: 1.0.3 Summary: A Python package
+Metadata-Version: 2.1 Name: PyDeepLX Version: 1.0.4 Summary: A Python package
 for unlimited DeepL translation Home-page: https://github.com/OwO-Network/
 PyDeepLX Author: missuo Author-email: i@yyt.moe License: MIT Platform: any
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.3 Classifier: Programming
 Language :: Python :: 3.4 Classifier: Programming Language :: Python :: 3.5
@@ -19,15 +19,15 @@
 a `429` error, it means your IP has been blocked by DeepL temporarily, please
 don't request it frequently in a short time. ## Usage ### Install Package
 ```bash pip install PyDeepLX ``` ### Use in code ```python from PyDeepLX import
 PyDeepLX # By default, the source language is automatically recognized and
 translated into English without providing any alternative results.
 PyDeepLX.translate("ä½ å¥½ä¸ç") # Return String # Specify the source and
 target languages PyDeepLX.translate("ä½ å¥½ä¸ç", "ZH", "EN") # Return String
-# Need alternative results PyDeepLX.translate("æ¯«æ çé®ç", "ZH", "EN",
-True) # Return List: ['Without a doubt', 'No doubt'] # Print the results
+# Need alternative results PyDeepLX.translate("æ¯«æ çé®ç", "ZH", "EN", 2)
+# Return List: ['Without a doubt', 'No doubt'] # Print the results
 PyDeepLX.translate("æ¯«æ çé®ç", "ZH", "EN", True, True) # Using proxy
 PyDeepLX.translate(text="æ¯«æ çé®ç", sourceLang="ZH", targetLang="EN",
-needAlternative=False, printResult=False, proxies="socks5://127.0.0.1:7890")
-``` ## PyPi [https://img.shields.io/badge/Pypi-000000?style=for-the-
+numberAlternative=0, printResult=False, proxies="socks5://127.0.0.1:7890") ```
+## PyPi [https://img.shields.io/badge/Pypi-000000?style=for-the-
 badge&logo=pypi&logoColor=red] ## Author **PyDeepLX** Â© [Vincent Young](https:
 //github.com/missuo), Released under the [MIT](./LICENSE) License.
```

### Comparing `PyDeepLX-1.0.3/README.md` & `PyDeepLX-1.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,47 @@
 # PyDeepLX
+
 A Python package for unlimited DeepL translation
 
 ## API Version
+
 [OwO-Network/DeepLX](https://github.com/OwO-Network/DeepLX): Permanently free DeepL API written in Golang.
 
 ## Description
+
 This is a Python package for DeepL translation, I didn't limit the number of translations in the code, if there is a `429` error, it means your IP has been blocked by DeepL temporarily, please don't request it frequently in a short time.
 
 ## Usage
+
 ### Install Package
+
 ```bash
 pip install PyDeepLX
 ```
+
 ### Use in code
+
 ```python
 from PyDeepLX import PyDeepLX
 # By default, the source language is automatically recognized and translated into English without providing any alternative results.
 PyDeepLX.translate("你好世界") # Return String
 
 # Specify the source and target languages
 PyDeepLX.translate("你好世界", "ZH", "EN") # Return String
 
 # Need alternative results
-PyDeepLX.translate("毫无疑问的", "ZH", "EN", True) # Return List: ['Without a doubt', 'No doubt']
+PyDeepLX.translate("毫无疑问的", "ZH", "EN", 2) # Return List: ['Without a doubt', 'No doubt']
 
 # Print the results
 PyDeepLX.translate("毫无疑问的", "ZH", "EN", True, True)
 
 # Using proxy
-PyDeepLX.translate(text="毫无疑问的", sourceLang="ZH", targetLang="EN", needAlternative=False, printResult=False, proxies="socks5://127.0.0.1:7890")
+PyDeepLX.translate(text="毫无疑问的", sourceLang="ZH", targetLang="EN", numberAlternative=0, printResult=False, proxies="socks5://127.0.0.1:7890")
 ```
 
 ## PyPi
+
 <a href="https://pypi.org/project/PyDeepLX/"><img src="https://img.shields.io/badge/Pypi-000000?style=for-the-badge&logo=pypi&logoColor=red" /></a>
 
 ## Author
 
 **PyDeepLX** © [Vincent Young](https://github.com/missuo), Released under the [MIT](./LICENSE) License.<br>
-
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 a `429` error, it means your IP has been blocked by DeepL temporarily, please
 don't request it frequently in a short time. ## Usage ### Install Package
 ```bash pip install PyDeepLX ``` ### Use in code ```python from PyDeepLX import
 PyDeepLX # By default, the source language is automatically recognized and
 translated into English without providing any alternative results.
 PyDeepLX.translate("ä½ å¥½ä¸ç") # Return String # Specify the source and
 target languages PyDeepLX.translate("ä½ å¥½ä¸ç", "ZH", "EN") # Return String
-# Need alternative results PyDeepLX.translate("æ¯«æ çé®ç", "ZH", "EN",
-True) # Return List: ['Without a doubt', 'No doubt'] # Print the results
+# Need alternative results PyDeepLX.translate("æ¯«æ çé®ç", "ZH", "EN", 2)
+# Return List: ['Without a doubt', 'No doubt'] # Print the results
 PyDeepLX.translate("æ¯«æ çé®ç", "ZH", "EN", True, True) # Using proxy
 PyDeepLX.translate(text="æ¯«æ çé®ç", sourceLang="ZH", targetLang="EN",
-needAlternative=False, printResult=False, proxies="socks5://127.0.0.1:7890")
-``` ## PyPi [https://img.shields.io/badge/Pypi-000000?style=for-the-
+numberAlternative=0, printResult=False, proxies="socks5://127.0.0.1:7890") ```
+## PyPi [https://img.shields.io/badge/Pypi-000000?style=for-the-
 badge&logo=pypi&logoColor=red] ## Author **PyDeepLX** Â© [Vincent Young](https:
 //github.com/missuo), Released under the [MIT](./LICENSE) License.
```

### Comparing `PyDeepLX-1.0.3/setup.py` & `PyDeepLX-1.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 '''
 Author: Vincent Young
 Date: 2023-04-27 00:42:10
 LastEditors: Vincent Young
-LastEditTime: 2023-05-21 04:10:41
+LastEditTime: 2023-07-18 12:55:54
 FilePath: /PyDeepLX/setup.py
 Telegram: https://t.me/missuo
 
 Copyright © 2023 by Vincent, All Rights Reserved. 
 '''
 from setuptools import setup, find_packages
 
 with open("README.md","r") as fh:
     long_description = fh.read()
 
 setup(
     name="PyDeepLX",
     author="missuo",
-    version="1.0.3",
+    version="1.0.4",
     license='MIT',
     long_description= long_description,
     long_description_content_type="text/markdown",
     author_email="i@yyt.moe",
     description="A Python package for unlimited DeepL translation",
     url='https://github.com/OwO-Network/PyDeepLX',
     packages=find_packages(),
     include_package_data=False,
     platforms='any',
     zip_safe=False,
 
     install_requires=[
-        'httpx[socks]',
+        'httpx[socks,brotli]',
         'langdetect'
     ],
     classifiers=[
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
```

