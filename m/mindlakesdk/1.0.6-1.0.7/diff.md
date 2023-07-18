# Comparing `tmp/mindlakesdk-1.0.6.tar.gz` & `tmp/mindlakesdk-1.0.7.tar.gz`

## Comparing `mindlakesdk-1.0.6.tar` & `mindlakesdk-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/requirements.txt
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/mindlakesdk/LICENSE
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/mindlakesdk/README.md
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/mindlakesdk/__init__.py
--rw-r--r--   0        0        0     9614 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/mindlakesdk/cryptor.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/mindlakesdk/datalake.py
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/mindlakesdk/keyhelper.py
--rw-r--r--   0        0        0     6813 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/mindlakesdk/message.py
--rw-r--r--   0        0        0     6229 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/mindlakesdk/permission.py
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/mindlakesdk/settings.py
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/mindlakesdk/utils.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/LICENSE
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/README.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 mindlakesdk-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 mindlakesdk-1.0.7/requirements.txt
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mindlakesdk-1.0.7/mindlakesdk/LICENSE
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mindlakesdk-1.0.7/mindlakesdk/README.md
+-rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 mindlakesdk-1.0.7/mindlakesdk/__init__.py
+-rw-r--r--   0        0        0     9614 2020-02-02 00:00:00.000000 mindlakesdk-1.0.7/mindlakesdk/cryptor.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 mindlakesdk-1.0.7/mindlakesdk/datalake.py
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 mindlakesdk-1.0.7/mindlakesdk/keyhelper.py
+-rw-r--r--   0        0        0     6813 2020-02-02 00:00:00.000000 mindlakesdk-1.0.7/mindlakesdk/message.py
+-rw-r--r--   0        0        0     6229 2020-02-02 00:00:00.000000 mindlakesdk-1.0.7/mindlakesdk/permission.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 mindlakesdk-1.0.7/mindlakesdk/settings.py
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 mindlakesdk-1.0.7/mindlakesdk/utils.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mindlakesdk-1.0.7/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mindlakesdk-1.0.7/LICENSE
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 mindlakesdk-1.0.7/README.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 mindlakesdk-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 mindlakesdk-1.0.7/PKG-INFO
```

### Comparing `mindlakesdk-1.0.6/mindlakesdk/LICENSE` & `mindlakesdk-1.0.7/mindlakesdk/LICENSE`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.6/mindlakesdk/__init__.py` & `mindlakesdk-1.0.7/mindlakesdk/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -38,70 +38,67 @@
         else:
             session.gateway = settings.GATEWAY
         logging.debug('gateway: %s'%session.gateway)
         logging.debug('walletAddress: %s'%session.walletAddress)
 
         result = mindlakesdk.message.getNounce(session)
         if not result:
-            self.code = result.code
-            self.message = result.message
-            self.data = result.data
+            self.__setResult(result)
             return 
         nounce = result.data
         logging.debug('getNounce: %s'%nounce)
             
         result = MindLake.__login(session, walletAccount, nounce)
         if not result:
-            self.code = result.code
-            self.message = result.message
-            self.data = result.data
+            self.__setResult(result)
             return 
         logging.debug('__login: %s'%result.data)
             
         session.mk, session.sk = mindlakesdk.keyhelper.prepareKeys(web3, walletAccount)
         logging.debug('getNounce: %s'%nounce)
 
         result = mindlakesdk.message.getAccountInfo(session)
         if not result:
-            self.code = result.code
-            self.message = result.message
-            self.data = result.data
+            self.__setResult(result)
             return 
-        
+
+        result = mindlakesdk.keyhelper.registerMK(session)
+        if not result:
+            self.__setResult(result)
+            return 
+
         if not session.isRegistered:
             result = MindLake.__registerAccount(session, self.permission)
             if not result:
-                self.code = result.code
-                self.message = result.message
-                self.data = result.data
+                self.__setResult(result)
                 return 
         else:
             result = mindlakesdk.message.getPKid(session)
             if not result:
-                self.code = result.code
-                self.message = result.message
-                self.data = result.data
+                self.__setResult(result)
                 return 
         self.code = 0
         self.message = "Success"
         self.data = None
 
     @staticmethod
     def __login(session: Session, walletAccount, nounce):
         msgToSign = encode_defunct(text=nounce)
         signature = walletAccount.sign_message(msgToSign)
         signatureHex = signature.signature.hex()
         return mindlakesdk.message.sendLogin(session, signatureHex)
 
     @staticmethod
     def __registerAccount(session: Session, permission: Permission):
-        result = mindlakesdk.keyhelper.registerMK(session)
-        if not result:
-            return result
         result = mindlakesdk.keyhelper.registerPK(session)
         if not result:
             return result
         result = permission.grantToSelf()
         return result
+    
+    def __setResult(self, result):
+        self.code = result.code
+        self.message = result.message
+        self.data = result.data
 
 connect = mindlakesdk.MindLake
```

### Comparing `mindlakesdk-1.0.6/mindlakesdk/cryptor.py` & `mindlakesdk-1.0.7/mindlakesdk/cryptor.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.6/mindlakesdk/datalake.py` & `mindlakesdk-1.0.7/mindlakesdk/datalake.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.6/mindlakesdk/keyhelper.py` & `mindlakesdk-1.0.7/mindlakesdk/keyhelper.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.6/mindlakesdk/message.py` & `mindlakesdk-1.0.7/mindlakesdk/message.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.6/mindlakesdk/permission.py` & `mindlakesdk-1.0.7/mindlakesdk/permission.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.6/mindlakesdk/settings.py` & `mindlakesdk-1.0.7/mindlakesdk/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,8 +66,8 @@
                                 "type": "bytes"
                         }
                 ],
                 "stateMutability": "view",
                 "type": "function"
         }
 ]
-VERSION = 'v1.0.6'
+VERSION = 'v1.0.7'
```

### Comparing `mindlakesdk-1.0.6/mindlakesdk/utils.py` & `mindlakesdk-1.0.7/mindlakesdk/utils.py`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.6/LICENSE` & `mindlakesdk-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mindlakesdk-1.0.6/README.md` & `mindlakesdk-1.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 * Cryptographic principles ensure that only the data owner can access their own plaintext data. 
 * Additionally, Mind Lake's powerful privacy computing capabilities enable the performance of calculations and querying of encrypted data.
 
 ## Getting Started
 
 ### Dependencies
 
-* Python > 3.10
+* Python > 3.8
 * pip
 * web3
 * pynacl
 
 ### Installing
 
 * pip install mindlakesdk
@@ -55,26 +55,28 @@
 
 ## Help
 
 Full doc: [https://mind-network.gitbook.io/mind-lake-sdk](https://mind-network.gitbook.io/mind-lake-sdk) 
 
 ## Authors
  
-* Dennis [@yuhaos](https://twitter.com/yuhaos)
+* Dennis [@NuIlPtr](https://twitter.com/nuilptr)
 * George [@georgemindnet](https://twitter.com/georgemindnet)
 
 ## Version History
 
 * v1.0
     * Initial Release
 * v1.0.1
     * Fix bug
 * v1.0.2
     * Improve performances
 * v1.0.5
     * Keep up the version number with TypeScript SDK
 * v1.0.6
     * Add support for Mind DataPack
+* v1.0.7
+    * Update the connect function
 
 ## License
 
 This project is licensed under the [MIT] License - see the LICENSE.md file for details
```

### Comparing `mindlakesdk-1.0.6/pyproject.toml` & `mindlakesdk-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mindlakesdk"
-version = "v1.0.6"
+version = "v1.0.7"
 authors = [
   { name="Mind Labs", email="biz@mindnetwork.xyz" },
 ]
 description = "A Python SDK to connect to Mind Lake"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = ["web3", "encryption", "datalake"]
 dependencies = [
```

### Comparing `mindlakesdk-1.0.6/PKG-INFO` & `mindlakesdk-1.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: mindlakesdk
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Python SDK to connect to Mind Lake
 Project-URL: Homepage, https://github.com/mind-network/mind-lake-sdk-python
 Project-URL: Bug Tracker, https://github.com/mind-network/mind-lake-sdk-python/issues
 Author-email: Mind Labs <biz@mindnetwork.xyz>
 License-File: LICENSE
 Keywords: datalake,encryption,web3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: eth-account
 Requires-Dist: pynacl
 Requires-Dist: web3
 Description-Content-Type: text/markdown
 
 # Mind Lake Python SDK
 
@@ -28,15 +28,15 @@
 * Cryptographic principles ensure that only the data owner can access their own plaintext data. 
 * Additionally, Mind Lake's powerful privacy computing capabilities enable the performance of calculations and querying of encrypted data.
 
 ## Getting Started
 
 ### Dependencies
 
-* Python > 3.10
+* Python > 3.8
 * pip
 * web3
 * pynacl
 
 ### Installing
 
 * pip install mindlakesdk
@@ -73,26 +73,28 @@
 
 ## Help
 
 Full doc: [https://mind-network.gitbook.io/mind-lake-sdk](https://mind-network.gitbook.io/mind-lake-sdk) 
 
 ## Authors
  
-* Dennis [@yuhaos](https://twitter.com/yuhaos)
+* Dennis [@NuIlPtr](https://twitter.com/nuilptr)
 * George [@georgemindnet](https://twitter.com/georgemindnet)
 
 ## Version History
 
 * v1.0
     * Initial Release
 * v1.0.1
     * Fix bug
 * v1.0.2
     * Improve performances
 * v1.0.5
     * Keep up the version number with TypeScript SDK
 * v1.0.6
     * Add support for Mind DataPack
+* v1.0.7
+    * Update the connect function
 
 ## License
 
 This project is licensed under the [MIT] License - see the LICENSE.md file for details
```

