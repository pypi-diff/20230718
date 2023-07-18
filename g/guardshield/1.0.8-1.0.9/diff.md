# Comparing `tmp/guardshield-1.0.8.tar.gz` & `tmp/guardshield-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\guardshield-1.0.8.tar", last modified: Tue Jul 18 01:22:26 2023, max compression
+gzip compressed data, was "dist\guardshield-1.0.9.tar", last modified: Tue Jul 18 15:56:45 2023, max compression
```

## Comparing `guardshield-1.0.8.tar` & `guardshield-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 01:22:26.659286 guardshield-1.0.8/
--rw-rw-rw-   0        0        0     1061 2023-05-18 23:20:40.000000 guardshield-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     4891 2023-07-18 01:22:26.658289 guardshield-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4464 2023-07-08 20:22:14.000000 guardshield-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 01:22:26.636836 guardshield-1.0.8/guardshield/
--rw-rw-rw-   0        0        0       89 2023-06-02 21:51:47.000000 guardshield-1.0.8/guardshield/__init__.py
--rw-rw-rw-   0        0        0    58627 2023-07-08 20:13:23.000000 guardshield-1.0.8/guardshield/dll_bytes.py
--rw-rw-rw-   0        0        0     3484 2023-07-18 01:20:38.000000 guardshield-1.0.8/guardshield/main.py
-drwxrwxrwx   0        0        0        0 2023-07-18 01:22:26.657291 guardshield-1.0.8/guardshield.egg-info/
--rw-rw-rw-   0        0        0     4891 2023-07-18 01:22:26.000000 guardshield-1.0.8/guardshield.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-07-18 01:22:26.000000 guardshield-1.0.8/guardshield.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 01:22:26.000000 guardshield-1.0.8/guardshield.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-18 01:22:26.000000 guardshield-1.0.8/guardshield.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2023-07-18 01:22:26.000000 guardshield-1.0.8/guardshield.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 01:22:26.660283 guardshield-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      585 2023-07-18 01:22:15.000000 guardshield-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 15:56:45.662160 guardshield-1.0.9/
+-rw-rw-rw-   0        0        0     1061 2023-05-18 23:20:40.000000 guardshield-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     5656 2023-07-18 15:56:45.662160 guardshield-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5195 2023-07-18 15:56:39.000000 guardshield-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 15:56:45.654152 guardshield-1.0.9/guardshield/
+-rw-rw-rw-   0        0        0       90 2023-07-18 15:33:04.000000 guardshield-1.0.9/guardshield/__init__.py
+-rw-rw-rw-   0        0        0    58627 2023-07-08 20:13:23.000000 guardshield-1.0.9/guardshield/dll_bytes.py
+-rw-rw-rw-   0        0        0     4840 2023-07-18 15:55:17.000000 guardshield-1.0.9/guardshield/main.py
+drwxrwxrwx   0        0        0        0 2023-07-18 15:56:45.660135 guardshield-1.0.9/guardshield.egg-info/
+-rw-rw-rw-   0        0        0     5656 2023-07-18 15:56:45.000000 guardshield-1.0.9/guardshield.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-07-18 15:56:45.000000 guardshield-1.0.9/guardshield.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 15:56:45.000000 guardshield-1.0.9/guardshield.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-18 15:56:45.000000 guardshield-1.0.9/guardshield.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2023-07-18 15:56:45.000000 guardshield-1.0.9/guardshield.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 15:56:45.663128 guardshield-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      585 2023-07-18 15:56:25.000000 guardshield-1.0.9/setup.py
```

### Comparing `guardshield-1.0.8/LICENSE` & `guardshield-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `guardshield-1.0.8/PKG-INFO` & `guardshield-1.0.9/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,137 +1,151 @@
-Metadata-Version: 2.1
-Name: guardshield
-Version: 1.0.8
-Summary: Security lib
-Home-page: https://github.com/OxynDev/ExcerSec
-Author: Oxyn
-Author-email: oxyn.dev@gmail.com
-License: MIT
-Keywords: python anti debugger security exe
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# GuardShield (Python security)
-
-GuardShield is a Python library that provides robust security measures to protect your Python projects. It offers various detection methods to prevent debugging attempts and ensure secure execution of your code.
-
-## Installation
-
-```python
-pip install guardshield
-```
-
-## Usage
-Import the library:
-```python
-import guardshield
-```
-
-Enable anti-debugger detection and define custom actions on detection:
-```python
-# Custom function to be executed on debugger detection
-def debugger_detected():
-    print("Debugger detected!")
-
-# Create a Security instance with desired settings
-module = guardshield.Security(
-    anti_debugger=True, # Enable debugger detection
-    kill_on_debug=True, # Kill the application on detection
-    custom_function_on_detection=debugger_detected # Execute custom function on detection
-)
-
-# Start the security check loop in a separate thread
-module.check_security()
-```
-
-Perform simple checks:
-```python
-# Check if the application is being debugged
-module.isDebugged()
-
-# Terminate the application
-module.kill()
-
-# Detect if the application is running within a sandbox environment (e.g., Sandboxie)
-module.isSandboxed()
-```
-
-## Secure Compilation and Protection Against Decompilation and Debugging Attacks
-
-To ensure the security of your executable (`.exe`) file, it is recommended to avoid using PyInstaller for compilation, as it can be easily reversed. Instead, you can use "Nuitka," a source-to-source compiler that compiles Python code into optimized C source code, making it harder for checkers and reverse engineers to understand and modify your code.
-
-Follow these steps to compile your code securely:
-
-1. Obfuscate your code using tools like the [Pyobfuscate](https://pyob.oxyry.com/) website, which can obfuscate variable names and enhance protection.
-2. Import GuardShield to prevent debugging during the execution of your code.
-3. Compile the code using Nuitka. Here's an example command:
-
-```python
-python -m nuitka --follow-imports --onefile --standalone --windows-icon-from-ico=icon.ico main.py
-```
-
-By following these steps, your code will be well-protected. However, for the utmost security, consider keeping sensitive parts of your code on the server-side as an API and perform critical operations there. This approach adds an extra layer of protection and makes your application almost unbreakable.
-
-## Request Encryption
-
-To enhance the security of your API requests, it is recommended to encrypt the requests or add a fingerprint (custom hash) to the request that can be checked in the application and on the server. Here's an example of AES encryption using the `AESCipher` class:
-
-```python
-import base64
-from Crypto.Cipher import AES
-from Crypto import Random
-import hashlib
-
-class AESCipher(object):
-    def __init__(self, key):
-        self.bs = AES.block_size
-        self.key = hashlib.sha256(key.encode()).digest()
-
-    def encrypt(self, raw):
-        raw = self._pad(raw)
-        iv = Random.new().read(AES.block_size)
-        cipher = AES.new(self.key, AES.MODE_CBC, iv)
-        return base64.b64encode(iv + cipher.encrypt(raw.encode()))
-
-    def decrypt(self, enc):
-        enc = base64.b64decode(enc)
-        iv = enc[:AES.block_size]
-        cipher = AES.new(self.key, AES.MODE_CBC, iv)
-        return self._unpad(cipher.decrypt(enc[AES.block_size:])).decode('utf-8')
-
-    def _pad(self, s):
-        return s + (self.bs - len(s) % self.bs) * chr(self.bs - len(s) % self.bs)
-
-    @staticmethod
-    def _unpad(s):
-        return s[:-ord(s[len(s)-1:])]
-
-class Aes:
-    def __init__(self):
-        self.key = "SecKey2115"
-
-    def decrypt(self, text, key=None):
-        if key is not None:
-            self.key = key
-        return AESCipher(self.key).decrypt(text)
-
-    def encrypt(self, text, key=None):
-        if key is not None:
-            self.key = key
-        return AESCipher(self.key).encrypt(text).decode()
-```
-
-You can use the `Aes` class to encrypt and decrypt your requests using AES encryption. Remember to use a strong and secure key for encryption.
-
-
-## Todo
-
-- [x] Add sandboxie detection
-- [ ] Add DLL injection protection
-
-## Tests
-
-![Test 1](https://github.com/OxynDev/guardshield/blob/ac9b56845ff0deb4de33363abe4025e119e830b7/temp/1.gif)
-
-![Test 2](https://github.com/OxynDev/guardshield/blob/4c971d7bebb2a04d54e7819561f5d850655a1881/temp/2.gif)
-
-![Test 3](https://github.com/OxynDev/guardshield/blob/bd7c082bf12272f35e63988267df144039d70873/temp/3.gif)
+# GuardShield (Python security)
+
+GuardShield is a Python library that provides robust security measures to protect your Python projects. It offers various detection methods to prevent debugging attempts and ensure secure execution of your code.
+
+## Installation
+
+```python
+pip install --force-reinstall guardshield
+```
+
+## Usage
+Import the library:
+```python
+import guardshield
+```
+
+Enable anti-debugger detection and define custom actions on detection:
+```python
+# Custom function to be executed on debugger detection
+def debugger_detected():
+    print("Debugger detected!")
+
+# Create a Security instance with desired settings
+module = guardshield.Security(
+    anti_debugger=True, # Enable debugger detection
+    kill_on_debug=True, # Kill the application on detection
+    custom_function_on_detection=debugger_detected # Execute custom function on detection
+)
+
+# Start the security check loop in a separate thread
+module.check_security() # -> dict { 'detected' : bool, 'description' : str }
+```
+
+Perform simple checks:
+```python
+# Check if the application is being debugged
+module.check_debug() # -> bool
+
+# Detect if the application is running within a sandbox environment (e.g., Sandboxie)
+module.check_sandbox() # -> bool
+
+# Terminate the application
+module.force_kill() # -> None
+
+# Detect if the application is running in vm and rdp
+module.check_vm() # -> bool
+
+# Crash user pc with Blue screen
+module.crash_pc() # -> None
+
+# Create pc fingerprint / hwid
+module.get_uuid() # -> str
+
+```
+
+## Change log
+```diff
+v1.0.9 ⋮ 18/07/2023
++ better cheat engine detection added
++ function names changed [ isSandboxed -> check_sandbox, isDebugged -> check_debug ]
++ added detect_vm and detect_sandbox to Security args
+
+v1.0.8 ⋮ 17/07/2023
++ crash_pc (Blue screen) function added
++ get_uuid (Create pc fingerprint / hwid) function added
+```
+
+
+## Secure Compilation and Protection Against Decompilation and Debugging Attacks
+
+To ensure the security of your executable (`.exe`) file, it is recommended to avoid using PyInstaller for compilation, as it can be easily reversed. Instead, you can use "Nuitka," a source-to-source compiler that compiles Python code into optimized C source code, making it harder for checkers and reverse engineers to understand and modify your code.
+
+Follow these steps to compile your code securely:
+
+1. Obfuscate your code using tools like the [Pyobfuscate](https://pyob.oxyry.com/) website, which can obfuscate variable names and enhance protection.
+2. Import GuardShield to prevent debugging during the execution of your code.
+3. Compile the code using Nuitka. Here's an example command:
+
+```python
+python -m nuitka --follow-imports --onefile --standalone --windows-icon-from-ico=icon.ico main.py
+```
+
+By following these steps, your code will be well-protected. However, for the utmost security, consider keeping sensitive parts of your code on the server-side as an API and perform critical operations there. This approach adds an extra layer of protection and makes your application almost unbreakable.
+
+## Request Encryption
+
+To enhance the security of your API requests, it is recommended to encrypt the requests or add a fingerprint (custom hash) to the request that can be checked in the application and on the server. Here's an example of AES encryption using the `AESCipher` class:
+
+```python
+import base64
+from Crypto.Cipher import AES
+from Crypto import Random
+import hashlib
+
+class AESCipher(object):
+    def __init__(self, key):
+        self.bs = AES.block_size
+        self.key = hashlib.sha256(key.encode()).digest()
+
+    def encrypt(self, raw):
+        raw = self._pad(raw)
+        iv = Random.new().read(AES.block_size)
+        cipher = AES.new(self.key, AES.MODE_CBC, iv)
+        return base64.b64encode(iv + cipher.encrypt(raw.encode()))
+
+    def decrypt(self, enc):
+        enc = base64.b64decode(enc)
+        iv = enc[:AES.block_size]
+        cipher = AES.new(self.key, AES.MODE_CBC, iv)
+        return self._unpad(cipher.decrypt(enc[AES.block_size:])).decode('utf-8')
+
+    def _pad(self, s):
+        return s + (self.bs - len(s) % self.bs) * chr(self.bs - len(s) % self.bs)
+
+    @staticmethod
+    def _unpad(s):
+        return s[:-ord(s[len(s)-1:])]
+
+class Aes:
+    def __init__(self):
+        self.key = "SecKey2115"
+
+    def decrypt(self, text, key=None):
+        if key is not None:
+            self.key = key
+        return AESCipher(self.key).decrypt(text)
+
+    def encrypt(self, text, key=None):
+        if key is not None:
+            self.key = key
+        return AESCipher(self.key).encrypt(text).decode()
+```
+
+You can use the `Aes` class to encrypt and decrypt your requests using AES encryption. Remember to use a strong and secure key for encryption.
+
+
+## Todo
+
+- [x] Add sandboxie detection
+- [x] Add Vm detection
+- [x] Add Better cheat engine detection
+- [ ] Add DLL injection protection
+
+      
+## Tests
+
+![Test 1](https://github.com/OxynDev/guardshield/blob/ac9b56845ff0deb4de33363abe4025e119e830b7/temp/1.gif)
+
+![Test 2](https://github.com/OxynDev/guardshield/blob/4c971d7bebb2a04d54e7819561f5d850655a1881/temp/2.gif)
+
+![Test 3](https://github.com/OxynDev/guardshield/blob/bd7c082bf12272f35e63988267df144039d70873/temp/3.gif)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `guardshield-1.0.8/README.md` & `guardshield-1.0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,125 +1,163 @@
-# GuardShield (Python security)
-
-GuardShield is a Python library that provides robust security measures to protect your Python projects. It offers various detection methods to prevent debugging attempts and ensure secure execution of your code.
-
-## Installation
-
-```python
-pip install guardshield
-```
-
-## Usage
-Import the library:
-```python
-import guardshield
-```
-
-Enable anti-debugger detection and define custom actions on detection:
-```python
-# Custom function to be executed on debugger detection
-def debugger_detected():
-    print("Debugger detected!")
-
-# Create a Security instance with desired settings
-module = guardshield.Security(
-    anti_debugger=True, # Enable debugger detection
-    kill_on_debug=True, # Kill the application on detection
-    custom_function_on_detection=debugger_detected # Execute custom function on detection
-)
-
-# Start the security check loop in a separate thread
-module.check_security()
-```
-
-Perform simple checks:
-```python
-# Check if the application is being debugged
-module.isDebugged()
-
-# Terminate the application
-module.kill()
-
-# Detect if the application is running within a sandbox environment (e.g., Sandboxie)
-module.isSandboxed()
-```
-
-## Secure Compilation and Protection Against Decompilation and Debugging Attacks
-
-To ensure the security of your executable (`.exe`) file, it is recommended to avoid using PyInstaller for compilation, as it can be easily reversed. Instead, you can use "Nuitka," a source-to-source compiler that compiles Python code into optimized C source code, making it harder for checkers and reverse engineers to understand and modify your code.
-
-Follow these steps to compile your code securely:
-
-1. Obfuscate your code using tools like the [Pyobfuscate](https://pyob.oxyry.com/) website, which can obfuscate variable names and enhance protection.
-2. Import GuardShield to prevent debugging during the execution of your code.
-3. Compile the code using Nuitka. Here's an example command:
-
-```python
-python -m nuitka --follow-imports --onefile --standalone --windows-icon-from-ico=icon.ico main.py
-```
-
-By following these steps, your code will be well-protected. However, for the utmost security, consider keeping sensitive parts of your code on the server-side as an API and perform critical operations there. This approach adds an extra layer of protection and makes your application almost unbreakable.
-
-## Request Encryption
-
-To enhance the security of your API requests, it is recommended to encrypt the requests or add a fingerprint (custom hash) to the request that can be checked in the application and on the server. Here's an example of AES encryption using the `AESCipher` class:
-
-```python
-import base64
-from Crypto.Cipher import AES
-from Crypto import Random
-import hashlib
-
-class AESCipher(object):
-    def __init__(self, key):
-        self.bs = AES.block_size
-        self.key = hashlib.sha256(key.encode()).digest()
-
-    def encrypt(self, raw):
-        raw = self._pad(raw)
-        iv = Random.new().read(AES.block_size)
-        cipher = AES.new(self.key, AES.MODE_CBC, iv)
-        return base64.b64encode(iv + cipher.encrypt(raw.encode()))
-
-    def decrypt(self, enc):
-        enc = base64.b64decode(enc)
-        iv = enc[:AES.block_size]
-        cipher = AES.new(self.key, AES.MODE_CBC, iv)
-        return self._unpad(cipher.decrypt(enc[AES.block_size:])).decode('utf-8')
-
-    def _pad(self, s):
-        return s + (self.bs - len(s) % self.bs) * chr(self.bs - len(s) % self.bs)
-
-    @staticmethod
-    def _unpad(s):
-        return s[:-ord(s[len(s)-1:])]
-
-class Aes:
-    def __init__(self):
-        self.key = "SecKey2115"
-
-    def decrypt(self, text, key=None):
-        if key is not None:
-            self.key = key
-        return AESCipher(self.key).decrypt(text)
-
-    def encrypt(self, text, key=None):
-        if key is not None:
-            self.key = key
-        return AESCipher(self.key).encrypt(text).decode()
-```
-
-You can use the `Aes` class to encrypt and decrypt your requests using AES encryption. Remember to use a strong and secure key for encryption.
-
-
-## Todo
-
-- [x] Add sandboxie detection
-- [ ] Add DLL injection protection
-
-## Tests
-
-![Test 1](https://github.com/OxynDev/guardshield/blob/ac9b56845ff0deb4de33363abe4025e119e830b7/temp/1.gif)
-
-![Test 2](https://github.com/OxynDev/guardshield/blob/4c971d7bebb2a04d54e7819561f5d850655a1881/temp/2.gif)
-
-![Test 3](https://github.com/OxynDev/guardshield/blob/bd7c082bf12272f35e63988267df144039d70873/temp/3.gif)
+Metadata-Version: 2.1
+Name: guardshield
+Version: 1.0.9
+Summary: Security lib
+Home-page: https://github.com/OxynDev/ExcerSec
+Author: Oxyn
+Author-email: oxyn.dev@gmail.com
+License: MIT
+Keywords: python anti debugger security exe
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# GuardShield (Python security)
+
+GuardShield is a Python library that provides robust security measures to protect your Python projects. It offers various detection methods to prevent debugging attempts and ensure secure execution of your code.
+
+## Installation
+
+```python
+pip install --force-reinstall guardshield
+```
+
+## Usage
+Import the library:
+```python
+import guardshield
+```
+
+Enable anti-debugger detection and define custom actions on detection:
+```python
+# Custom function to be executed on debugger detection
+def debugger_detected():
+    print("Debugger detected!")
+
+# Create a Security instance with desired settings
+module = guardshield.Security(
+    anti_debugger=True, # Enable debugger detection
+    kill_on_debug=True, # Kill the application on detection
+    custom_function_on_detection=debugger_detected # Execute custom function on detection
+)
+
+# Start the security check loop in a separate thread
+module.check_security() # -> dict { 'detected' : bool, 'description' : str }
+```
+
+Perform simple checks:
+```python
+# Check if the application is being debugged
+module.check_debug() # -> bool
+
+# Detect if the application is running within a sandbox environment (e.g., Sandboxie)
+module.check_sandbox() # -> bool
+
+# Terminate the application
+module.force_kill() # -> None
+
+# Detect if the application is running in vm and rdp
+module.check_vm() # -> bool
+
+# Crash user pc with Blue screen
+module.crash_pc() # -> None
+
+# Create pc fingerprint / hwid
+module.get_uuid() # -> str
+
+```
+
+## Change log
+```diff
+v1.0.9 â‹® 18/07/2023
++ better cheat engine detection added
++ function names changed [ isSandboxed -> check_sandbox, isDebugged -> check_debug ]
++ added detect_vm and detect_sandbox to Security args
+
+v1.0.8 â‹® 17/07/2023
++ crash_pc (Blue screen) function added
++ get_uuid (Create pc fingerprint / hwid) function added
+```
+
+
+## Secure Compilation and Protection Against Decompilation and Debugging Attacks
+
+To ensure the security of your executable (`.exe`) file, it is recommended to avoid using PyInstaller for compilation, as it can be easily reversed. Instead, you can use "Nuitka," a source-to-source compiler that compiles Python code into optimized C source code, making it harder for checkers and reverse engineers to understand and modify your code.
+
+Follow these steps to compile your code securely:
+
+1. Obfuscate your code using tools like the [Pyobfuscate](https://pyob.oxyry.com/) website, which can obfuscate variable names and enhance protection.
+2. Import GuardShield to prevent debugging during the execution of your code.
+3. Compile the code using Nuitka. Here's an example command:
+
+```python
+python -m nuitka --follow-imports --onefile --standalone --windows-icon-from-ico=icon.ico main.py
+```
+
+By following these steps, your code will be well-protected. However, for the utmost security, consider keeping sensitive parts of your code on the server-side as an API and perform critical operations there. This approach adds an extra layer of protection and makes your application almost unbreakable.
+
+## Request Encryption
+
+To enhance the security of your API requests, it is recommended to encrypt the requests or add a fingerprint (custom hash) to the request that can be checked in the application and on the server. Here's an example of AES encryption using the `AESCipher` class:
+
+```python
+import base64
+from Crypto.Cipher import AES
+from Crypto import Random
+import hashlib
+
+class AESCipher(object):
+    def __init__(self, key):
+        self.bs = AES.block_size
+        self.key = hashlib.sha256(key.encode()).digest()
+
+    def encrypt(self, raw):
+        raw = self._pad(raw)
+        iv = Random.new().read(AES.block_size)
+        cipher = AES.new(self.key, AES.MODE_CBC, iv)
+        return base64.b64encode(iv + cipher.encrypt(raw.encode()))
+
+    def decrypt(self, enc):
+        enc = base64.b64decode(enc)
+        iv = enc[:AES.block_size]
+        cipher = AES.new(self.key, AES.MODE_CBC, iv)
+        return self._unpad(cipher.decrypt(enc[AES.block_size:])).decode('utf-8')
+
+    def _pad(self, s):
+        return s + (self.bs - len(s) % self.bs) * chr(self.bs - len(s) % self.bs)
+
+    @staticmethod
+    def _unpad(s):
+        return s[:-ord(s[len(s)-1:])]
+
+class Aes:
+    def __init__(self):
+        self.key = "SecKey2115"
+
+    def decrypt(self, text, key=None):
+        if key is not None:
+            self.key = key
+        return AESCipher(self.key).decrypt(text)
+
+    def encrypt(self, text, key=None):
+        if key is not None:
+            self.key = key
+        return AESCipher(self.key).encrypt(text).decode()
+```
+
+You can use the `Aes` class to encrypt and decrypt your requests using AES encryption. Remember to use a strong and secure key for encryption.
+
+
+## Todo
+
+- [x] Add sandboxie detection
+- [x] Add Vm detection
+- [x] Add Better cheat engine detection
+- [ ] Add DLL injection protection
+
+      
+## Tests
+
+![Test 1](https://github.com/OxynDev/guardshield/blob/ac9b56845ff0deb4de33363abe4025e119e830b7/temp/1.gif)
+
+![Test 2](https://github.com/OxynDev/guardshield/blob/4c971d7bebb2a04d54e7819561f5d850655a1881/temp/2.gif)
+
+![Test 3](https://github.com/OxynDev/guardshield/blob/bd7c082bf12272f35e63988267df144039d70873/temp/3.gif)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `guardshield-1.0.8/guardshield/dll_bytes.py` & `guardshield-1.0.9/guardshield/dll_bytes.py`

 * *Files identical despite different names*

### Comparing `guardshield-1.0.8/guardshield/main.py` & `guardshield-1.0.9/guardshield/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,91 +1,127 @@
 import os, ctypes, threading, time, io, tempfile, platform, subprocess, hashlib
 from .dll_bytes import dll_bytes
+from .core import cheatengine
 
 timeout = 0.1
 
 
 class AntiDebugger:
 
     def __init__(self, dll, settings):
         self.settings = settings
         self.dll = dll
-        threading.Thread(target=self.start).start()
+        threading.Thread(target=self.dll_detector).start()
+        threading.Thread(target=self.file_monitor).start()
 
-    def start(self) -> None:
+    def dll_detector(self) -> None:
         while True:
 
             if self.dll.isDebugged() == 0:
                 pass
             else:
-                function_check = self.settings['custom_function_on_detection']
+                function_check = self.settings['on_detection']
                 if function_check != None:
                     function_check()
                 if self.settings['kill_on_debug'] == True:
                     self.dll.kill()
                 
 
             time.sleep(timeout)
 
+    def file_monitor(self):
+        res = cheatengine.monitor_dir(tempfile.gettempdir())
+        if res == True:
+            function_check = self.settings['on_detection']
+            if function_check != None:
+                function_check()
+            if self.settings['kill_on_debug'] == True:
+                self.dll.kill()
+
+
 class Security:
 
     dll = None
 
     def __init__(self,
                     anti_debugger: bool = True,
                     kill_on_debug: bool = True,
-                    custom_function_on_detection = None
+                    detect_vm: bool = False,
+                    detect_sandbox: bool = False,
+                    on_detection = None
                     
                  ):
         
         self.load_dll()
 
         self.settings = {
             "anti_debugger" : anti_debugger,
             "kill_on_debug" : kill_on_debug,
-            "custom_function_on_detection" : custom_function_on_detection
+            "on_detection" : on_detection,
+            "detect_vm" : detect_vm,
+            "detect_sandbox" : detect_sandbox,
         }
 
     def load_dll(self) -> None:
         #path = pkg_resources.resource_filename(__name__, 'lib.dll')
 
         temp_file = tempfile.NamedTemporaryFile(suffix='.dll', delete=False)
         temp_file.write(dll_bytes)
         temp_file.close()
         self.dll = ctypes.WinDLL(temp_file.name)
         
         
             
     def check_security(self) -> None:
 
+        if self.settings['detect_vm'] == True:
+            if self.check_vm() == True:
+                function_check = self.settings['on_detection']
+                if function_check != None:
+                    function_check()
+                return {
+                    "detected":True, 
+                    "description": "vm detected"
+                    }
+            
+        if self.settings['detect_sandbox'] == True:
+            if self.check_sandbox() == True:
+                function_check = self.settings['on_detection']
+                if function_check != None:
+                    function_check()
+                return {
+                    "detected":True, 
+                    "description": "sandbox detected"
+                    }
+
         if self.settings['anti_debugger'] == True:
             AntiDebugger(
                 dll = self.dll,
                 settings = self.settings
             )
-
+        
     def check_vm(self) -> bool:
         if self.dll.IsVm() == 0:
             return False
         else:
             return True
 
     def force_kill(self):
         self.dll.kill()
         os.close()
         exit()
         
-    def isDebugged(self) -> bool:
+    def check_debug(self) -> bool:
         if self.dll.isDebugged() == 0:
             return False
         else:
             return True
 
 
-    def isSandboxed(self) -> bool:
+    def check_sandbox(self) -> bool:
         if self.dll.isSandbox() == 0:
             return False
         else:
             return True
 
     def crash_pc(self) -> None:
```

### Comparing `guardshield-1.0.8/guardshield.egg-info/PKG-INFO` & `guardshield-1.0.9/guardshield.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guardshield
-Version: 1.0.8
+Version: 1.0.9
 Summary: Security lib
 Home-page: https://github.com/OxynDev/ExcerSec
 Author: Oxyn
 Author-email: oxyn.dev@gmail.com
 License: MIT
 Keywords: python anti debugger security exe
 Description-Content-Type: text/markdown
@@ -13,15 +13,15 @@
 # GuardShield (Python security)
 
 GuardShield is a Python library that provides robust security measures to protect your Python projects. It offers various detection methods to prevent debugging attempts and ensure secure execution of your code.
 
 ## Installation
 
 ```python
-pip install guardshield
+pip install --force-reinstall guardshield
 ```
 
 ## Usage
 Import the library:
 ```python
 import guardshield
 ```
@@ -36,29 +36,52 @@
 module = guardshield.Security(
     anti_debugger=True, # Enable debugger detection
     kill_on_debug=True, # Kill the application on detection
     custom_function_on_detection=debugger_detected # Execute custom function on detection
 )
 
 # Start the security check loop in a separate thread
-module.check_security()
+module.check_security() # -> dict { 'detected' : bool, 'description' : str }
 ```
 
 Perform simple checks:
 ```python
 # Check if the application is being debugged
-module.isDebugged()
+module.check_debug() # -> bool
+
+# Detect if the application is running within a sandbox environment (e.g., Sandboxie)
+module.check_sandbox() # -> bool
 
 # Terminate the application
-module.kill()
+module.force_kill() # -> None
+
+# Detect if the application is running in vm and rdp
+module.check_vm() # -> bool
+
+# Crash user pc with Blue screen
+module.crash_pc() # -> None
+
+# Create pc fingerprint / hwid
+module.get_uuid() # -> str
 
-# Detect if the application is running within a sandbox environment (e.g., Sandboxie)
-module.isSandboxed()
 ```
 
+## Change log
+```diff
+v1.0.9 â‹® 18/07/2023
++ better cheat engine detection added
++ function names changed [ isSandboxed -> check_sandbox, isDebugged -> check_debug ]
++ added detect_vm and detect_sandbox to Security args
+
+v1.0.8 â‹® 17/07/2023
++ crash_pc (Blue screen) function added
++ get_uuid (Create pc fingerprint / hwid) function added
+```
+
+
 ## Secure Compilation and Protection Against Decompilation and Debugging Attacks
 
 To ensure the security of your executable (`.exe`) file, it is recommended to avoid using PyInstaller for compilation, as it can be easily reversed. Instead, you can use "Nuitka," a source-to-source compiler that compiles Python code into optimized C source code, making it harder for checkers and reverse engineers to understand and modify your code.
 
 Follow these steps to compile your code securely:
 
 1. Obfuscate your code using tools like the [Pyobfuscate](https://pyob.oxyry.com/) website, which can obfuscate variable names and enhance protection.
@@ -122,16 +145,19 @@
 
 You can use the `Aes` class to encrypt and decrypt your requests using AES encryption. Remember to use a strong and secure key for encryption.
 
 
 ## Todo
 
 - [x] Add sandboxie detection
+- [x] Add Vm detection
+- [x] Add Better cheat engine detection
 - [ ] Add DLL injection protection
 
+      
 ## Tests
 
 ![Test 1](https://github.com/OxynDev/guardshield/blob/ac9b56845ff0deb4de33363abe4025e119e830b7/temp/1.gif)
 
 ![Test 2](https://github.com/OxynDev/guardshield/blob/4c971d7bebb2a04d54e7819561f5d850655a1881/temp/2.gif)
 
 ![Test 3](https://github.com/OxynDev/guardshield/blob/bd7c082bf12272f35e63988267df144039d70873/temp/3.gif)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `guardshield-1.0.8/setup.py` & `guardshield-1.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, os
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setuptools.setup(
     name="guardshield",
-    version="1.0.8",
+    version="1.0.9",
     author="Oxyn",
     author_email="oxyn.dev@gmail.com",
     description="Security lib",
     keywords = "python anti debugger security exe",
     packages=setuptools.find_packages(),
     include_package_data=True,
     url='https://github.com/OxynDev/ExcerSec',
```

