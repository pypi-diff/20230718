# Comparing `tmp/ubiq-security-1.0.8.tar.gz` & `tmp/ubiq-security-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ubiq-security-1.0.8.tar", last modified: Mon Jan 18 22:15:36 2021, max compression
+gzip compressed data, was "ubiq-security-2.1.0.tar", last modified: Tue Jul 18 15:36:50 2023, max compression
```

## Comparing `ubiq-security-1.0.8.tar` & `ubiq-security-2.1.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 gary      (1000) gary      (1000)        0 2021-01-18 22:15:36.000000 ubiq-security-1.0.8/
--rw-r--r--   0 gary      (1000) gary      (1000)       38 2021-01-18 22:15:36.000000 ubiq-security-1.0.8/setup.cfg
--rw-r--r--   0 gary      (1000) gary      (1000)     1742 2021-01-18 22:05:41.000000 ubiq-security-1.0.8/setup.py
--rw-r--r--   0 gary      (1000) gary      (1000)       27 2020-08-26 05:35:52.000000 ubiq-security-1.0.8/requirements.txt
--rw-r--r--   0 gary      (1000) gary      (1000)     7724 2021-01-18 22:15:36.000000 ubiq-security-1.0.8/PKG-INFO
--rw-r--r--   0 gary      (1000) gary      (1000)      448 2021-01-18 22:11:45.000000 ubiq-security-1.0.8/CHANGELOG.md
-drwxr-xr-x   0 gary      (1000) gary      (1000)        0 2021-01-18 22:15:36.000000 ubiq-security-1.0.8/examples/
--rw-r--r--   0 gary      (1000) gary      (1000)       77 2021-01-18 22:05:49.000000 ubiq-security-1.0.8/examples/credentials
--rw-r--r--   0 gary      (1000) gary      (1000)    11701 2021-01-18 22:05:41.000000 ubiq-security-1.0.8/examples/ubiq_sample.py
--rw-r--r--   0 gary      (1000) gary      (1000)     2575 2020-08-26 05:35:52.000000 ubiq-security-1.0.8/examples/README.md
--rw-r--r--   0 gary      (1000) gary      (1000)     1104 2021-01-18 22:05:41.000000 ubiq-security-1.0.8/LICENSE
-drwxr-xr-x   0 gary      (1000) gary      (1000)        0 2021-01-18 22:15:36.000000 ubiq-security-1.0.8/ubiq_security.egg-info/
--rw-r--r--   0 gary      (1000) gary      (1000)      483 2021-01-18 22:15:36.000000 ubiq-security-1.0.8/ubiq_security.egg-info/SOURCES.txt
--rw-r--r--   0 gary      (1000) gary      (1000)       14 2021-01-18 22:15:36.000000 ubiq-security-1.0.8/ubiq_security.egg-info/top_level.txt
--rw-r--r--   0 gary      (1000) gary      (1000)        1 2021-01-18 22:15:36.000000 ubiq-security-1.0.8/ubiq_security.egg-info/dependency_links.txt
--rw-r--r--   0 gary      (1000) gary      (1000)     7724 2021-01-18 22:15:36.000000 ubiq-security-1.0.8/ubiq_security.egg-info/PKG-INFO
--rw-r--r--   0 gary      (1000) gary      (1000)       26 2021-01-18 22:15:36.000000 ubiq-security-1.0.8/ubiq_security.egg-info/requires.txt
--rw-r--r--   0 gary      (1000) gary      (1000)     5259 2020-09-18 18:46:45.000000 ubiq-security-1.0.8/README.md
-drwxr-xr-x   0 gary      (1000) gary      (1000)        0 2021-01-18 22:15:36.000000 ubiq-security-1.0.8/ubiq_security/
--rw-r--r--   0 gary      (1000) gary      (1000)     5455 2021-01-18 22:05:41.000000 ubiq-security-1.0.8/ubiq_security/auth.py
--rw-r--r--   0 gary      (1000) gary      (1000)     8027 2021-01-18 22:05:41.000000 ubiq-security-1.0.8/ubiq_security/encrypt.py
--rw-r--r--   0 gary      (1000) gary      (1000)     3843 2021-01-18 22:05:41.000000 ubiq-security-1.0.8/ubiq_security/algorithm.py
--rw-r--r--   0 gary      (1000) gary      (1000)       18 2021-01-18 22:10:59.000000 ubiq-security-1.0.8/ubiq_security/version.py
--rw-r--r--   0 gary      (1000) gary      (1000)    13080 2021-01-18 22:05:41.000000 ubiq-security-1.0.8/ubiq_security/decrypt.py
--rw-r--r--   0 gary      (1000) gary      (1000)      226 2021-01-18 22:05:41.000000 ubiq-security-1.0.8/ubiq_security/__init__.py
--rw-r--r--   0 gary      (1000) gary      (1000)     4750 2021-01-18 22:05:41.000000 ubiq-security-1.0.8/ubiq_security/credentials.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:36:50.486871 ubiq-security-2.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1104 2022-11-21 21:22:47.000000 ubiq-security-2.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9019 2023-07-18 15:36:50.486220 ubiq-security-2.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8063 2023-05-23 20:56:07.000000 ubiq-security-2.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 15:36:50.487279 ubiq-security-2.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1742 2022-11-21 21:22:47.000000 ubiq-security-2.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:36:50.472869 ubiq-security-2.1.0/ubiq_security/
+-rw-r--r--   0 root         (0) root         (0)      226 2022-11-21 21:22:47.000000 ubiq-security-2.1.0/ubiq_security/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3843 2022-11-21 21:22:47.000000 ubiq-security-2.1.0/ubiq_security/algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     5455 2023-05-04 23:15:07.000000 ubiq-security-2.1.0/ubiq_security/auth.py
+-rw-r--r--   0 root         (0) root         (0)     3607 2023-06-15 19:59:00.000000 ubiq-security-2.1.0/ubiq_security/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5974 2023-06-15 19:59:00.000000 ubiq-security-2.1.0/ubiq_security/credentials.py
+-rw-r--r--   0 root         (0) root         (0)    13317 2023-06-15 19:59:00.000000 ubiq-security-2.1.0/ubiq_security/decrypt.py
+-rw-r--r--   0 root         (0) root         (0)     8317 2023-06-15 19:59:00.000000 ubiq-security-2.1.0/ubiq_security/encrypt.py
+-rw-r--r--   0 root         (0) root         (0)     5158 2023-06-15 19:59:00.000000 ubiq-security-2.1.0/ubiq_security/events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:36:50.484433 ubiq-security-2.1.0/ubiq_security/fpe/
+-rw-r--r--   0 root         (0) root         (0)      124 2023-06-15 19:59:00.000000 ubiq-security-2.1.0/ubiq_security/fpe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6452 2023-06-21 16:35:33.000000 ubiq-security-2.1.0/ubiq_security/fpe/common.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2023-06-15 19:59:00.000000 ubiq-security-2.1.0/ubiq_security/fpe/decrypt.py
+-rw-r--r--   0 root         (0) root         (0)     3611 2023-06-21 16:35:33.000000 ubiq-security-2.1.0/ubiq_security/fpe/encrypt.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-18 15:05:54.000000 ubiq-security-2.1.0/ubiq_security/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:36:50.479018 ubiq-security-2.1.0/ubiq_security.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9019 2023-07-18 15:36:50.000000 ubiq-security-2.1.0/ubiq_security.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      560 2023-07-18 15:36:50.000000 ubiq-security-2.1.0/ubiq_security.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 15:36:50.000000 ubiq-security-2.1.0/ubiq_security.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-18 15:36:50.000000 ubiq-security-2.1.0/ubiq_security.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-18 15:36:50.000000 ubiq-security-2.1.0/ubiq_security.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ubiq-security-1.0.8/setup.py` & `ubiq-security-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `ubiq-security-1.0.8/LICENSE` & `ubiq-security-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ubiq-security-1.0.8/README.md` & `ubiq-security-2.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 
 The Ubiq Security Python library provides convenient interaction with the
 Ubiq Security Platform API from applications written in the Python language.
 It includes a pre-defined set of classes that will provide simple interfaces
 to encrypt and decrypt data
 
+This library also incorporates Ubiq Format Preserving Encryption (eFPE).  eFPE allows encrypting so that the output cipher text is in the same format as the original plaintext. This includes preserving special characters and control over what characters are permitted in the cipher text. For example, consider encrypting a social security number '123-45-6789'. The cipher text will maintain the dashes and look something like: 'W$+-qF-oMMV'.
+
 ## Documentation
 
 See the [Python API docs](https://dev.ubiqsecurity.com/docs/api).
 
 ## Installation
 
 #### Using the package manager:
@@ -28,18 +30,21 @@
 
 #### Installing from source:
 From within the cloned git repository directory, Install from source with:
 
 
 ```
 cd ubiq-python
+pip3 install -r requirements.txt
 python3 setup.py install
 ```
 You may need to run the python3 commands above using sudo.
 
+The Ubiq Security libraries are dependent on M2Crypto which has specific requirements as well which varies depending upon your actual environment.  If you encounter problems installing the Ubiq Security libraries, please see [M2Crypto](https://gitlab.com/m2crypto/m2crypto/-/blob/master/INSTALL.rst) for the latest notes and instructions.
+
 
 ### Requirements
 
 -   Python 3.5+
 
 ## Usage
 
@@ -181,10 +186,76 @@
             break
 
     # Make sure an additional plaintext data is retrieved and
     # release any allocated resources
     plaintext_data += decryption.end()
 
 ```
+## Ubiq Format Preserving Encryption
+
+This library incorporates Ubiq Format Preserving Encryption (eFPE).
+
+## Requirements
+
+-   Please follow the same requirements as described above for the non-eFPE functionality.
+-   This library has dependencies on ubiqsecurity-fpe library available for download in the Ubiq GitHub/GitLab repository.
+
+## Usage
+
+You will need to obtain account credentials in the same way as described above for conventional encryption/decryption. When
+you do this in your [Ubiq Dashboard][dashboard] [credentials][credentials], you'll need to enable the eFPE option.
+The credentials can be set using environment variables, loaded from an explicitly
+specified file, or read from the default location (~/.ubiq/credentials).
+
+
+Require the Security Client module in your Python class.
+
+```python
+import ubiq_security as ubiq
+import ubiq_security.fpe as ubiqfpe
+```
+
+
+### Encrypt a social security text field - simple interface
+Pass credentials, the name of a Field Format Specification, FFS, and data into the encryption function.
+The encrypted data will be returned.
+
+```python
+ffs_name = "SSN";
+plain_text = "123-45-6789";
+
+credentials = ubiq.ConfigCredentials('./credentials', 'default');
+
+encrypted_data = ubiqfpe.Encrypt(
+        credentials,
+        ffs_name,
+        plain_text);
+        
+print('ENCRYPTED ciphertext= ' + encrypted_data + '\n');
+```
+
+### Decrypt a social security text field - simple interface
+Pass credentials, the name of a Field Format Specification, FFS, and data into the decryption function.
+The decrypted data will be returned.
+
+```python
+ffs_name = "SSN";
+cipher_text = "300-0E-274t";
+
+credentials = ubiq.ConfigCredentials('./credentials', 'default');
+
+decrypted_text = ubiqfpe.Decrypt(
+        credentials,
+        ffs_name,
+        cipher_text);
+        
+print('DECRYPTED decrypted_text= ' + decrypted_text + '\n');
+```
+
+Additional information on how to use these FFS models in your own applications is available by contacting Ubiq.
+
+
+
+
 [dashboard]:https://dashboard.ubiqsecurity.com/
 [credentials]:https://dev.ubiqsecurity.com/docs/how-to-create-api-keys
```

### Comparing `ubiq-security-1.0.8/ubiq_security/auth.py` & `ubiq-security-2.1.0/ubiq_security/auth.py`

 * *Files identical despite different names*

### Comparing `ubiq-security-1.0.8/ubiq_security/encrypt.py` & `ubiq-security-2.1.0/ubiq_security/encrypt.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,18 +30,19 @@
         If the key was used less times than was requested, send an
         update to the server. This function is called automatically.
         """
         try:
             if self._key['uses'] < self._key['max_uses']:
                 requests.patch(
                     self._endpoint_base() +
-                    '/encryption/key/' + self._key['id'] + '/' + self._key['session'],
+                    '/encryption/key/' +
+                    self._key['id'] + '/' + self._key['session'],
                     data=json.dumps(
-                        { "requested": self._key['max_uses'],
-                          "actual": self._key['uses'] }).encode('utf-8'),
+                        {"requested": self._key['max_uses'],
+                         "actual": self._key['uses']}).encode('utf-8'),
                     auth=http_auth(self._papi, self._sapi))
         except:
             pass
 
     def __init__(self, creds, uses):
         """Initialize the encryption object
 
@@ -59,14 +60,17 @@
             with the key. This number may be limited by the server.
         host:
             A string of the form 'host[:port]' with the []'s denoting an
             optional portion of the string indicating the server to which
             to make the request.
         """
 
+        if not creds.set():
+            raise RuntimeError("credentials not set")
+
         # If the host does not begin with either http or https
         # insert https://
         self._host = creds.host
         if (not self._host.lower().startswith('http')):
             self._host = "https://" + self._host
 
         self._papi = creds.access_key_id
@@ -79,15 +83,15 @@
         # propagated back to the caller
         #
 
         url = self._endpoint_base() + '/encryption/key'
 
         response = requests.post(
             url,
-            data=json.dumps({ 'uses': uses }).encode('utf-8'),
+            data=json.dumps({'uses': uses}).encode('utf-8'),
             auth=http_auth(self._papi, self._sapi))
 
         if response.status_code != http.HTTPStatus.CREATED:
             raise urllib.error.HTTPError(
                 url, response.status_code,
                 http.HTTPStatus(response.status_code).phrase,
                 response.headers, response.content)
@@ -103,15 +107,16 @@
         content = json.loads(response.content.decode('utf-8'))
 
         #
         # decrypt the client's private key. if the decryption fails,
         # the function raises a ValueError which is propagated up.
         #
         prvkey = crypto.serialization.load_pem_private_key(
-            content['encrypted_private_key'].encode('utf-8'), creds.secret_crypto_access_key.encode('utf-8'),
+            content['encrypted_private_key'].encode(
+                'utf-8'), creds.secret_crypto_access_key.encode('utf-8'),
             crypto_backend())
 
         self._key = {}
         self._key['id'] = content['key_fingerprint']
         self._key['session'] = content['encryption_session']
         self._key['security_model'] = content['security_model']
         self._key['algorithm'] = self._key['security_model']['algorithm'].lower()
@@ -157,30 +162,31 @@
         # create a new encryption context
         self._enc, iv = self._algo.encryptor(self._key['raw'])
 
         # VER 0, Flags 1 bit means AAD
         hdr = struct.pack('!BBBBH',
                           0, algorithm.UBIQ_HEADER_V0_FLAG_AAD,
                           self._algo.id,
-                          len(iv), len(self._key['encrypted']));
+                          len(iv), len(self._key['encrypted']))
         hdr += iv + self._key['encrypted']
         self._enc.authenticate_additional_data(hdr)
 
         # create and return the header for the cipher text
         return (hdr)
 
     def update(self, data):
         """Encrypt some plain text -
         plain text value has to be contained in a bytes, bytearray or memoryview object.
 
         Any cipher text produced by the operation is returned
         """
 
         if not isinstance(data, (bytes, bytearray, memoryview)):
-            raise RuntimeError("Data must be bytes, bytearray, or memoryview objects")
+            raise RuntimeError(
+                "Data must be bytes, bytearray, or memoryview objects")
 
         return self._enc.update(data)
 
     def end(self):
         """Finalize an encryption
 
         This function finalizes the encryption (producing the final
@@ -194,14 +200,15 @@
         res = self._enc.finalize()
         if not self._algo.len['tag'] == 0:
             res += self._enc.tag
 
         del self._enc
         return res
 
+
 def encrypt(creds, data):
     """Simple encryption interface
     papi:
         The client's public API key (used to identify the
         client to the server)
     sapi:
         The client's secret API key (used to authenticate HTTP requests)
@@ -215,8 +222,10 @@
         optional portion of the string indicating the server to which
         to make the request.
 
     returns:
         the entire cipher text that can be passed to the decrypt function
     """
     enc = encryption(creds, 1)
+    creds.add_event(dataset_name="", dataset_group_name="", billing_action="encrypt",
+                    dataset_type="unstructured", key_number=0, count=1)
     return enc.begin() + enc.update(data) + enc.end()
```

### Comparing `ubiq-security-1.0.8/ubiq_security/algorithm.py` & `ubiq-security-2.1.0/ubiq_security/algorithm.py`

 * *Files identical despite different names*

### Comparing `ubiq-security-1.0.8/ubiq_security/decrypt.py` & `ubiq-security-2.1.0/ubiq_security/decrypt.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,14 +58,17 @@
             by this object.
         host:
             A string of the form 'host[:port]' with the []'s denoting an
             optional portion of the string indicating the server to which
             to make the request.
         """
 
+        if not creds.set():
+            raise RuntimeError("credentials not set")
+
         # If the host does not begin with either http or https
         # insert https://
         self._host = creds.host
         if (not self._host.lower().startswith('http')):
             self._host = "https://" + self._host
 
         self._papi = creds.access_key_id
@@ -312,8 +315,10 @@
         optional portion of the string indicating the server to which
         to make the request.
 
     returns:
         the entire cipher text that can be passed to the decrypt function
     """
     dec = decryption(creds)
+    creds.add_event(dataset_name="", dataset_group_name="", billing_action="decrypt",
+                dataset_type="unstructured", key_number=0, count=1)
     return dec.begin() + dec.update(data) + dec.end()
```

### Comparing `ubiq-security-1.0.8/ubiq_security/credentials.py` & `ubiq-security-2.1.0/ubiq_security/credentials.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 #!/usr/bin/env python3
 
+import atexit
 import configparser
 import os
 from . import UBIQ_HOST
+from .configuration import ubiqConfiguration
+from .events import events, eventsProcessor
 
 class credentialsInfo:
 
     def __init__(self, access_key_id, secret_signing_key, secret_crypto_access_key, host):
         self.__access_key_id = access_key_id
         self.__secret_signing_key = secret_signing_key
         self.__secret_crypto_access_key = secret_crypto_access_key
@@ -72,26 +75,46 @@
         if os.path.exists(config_file):
             self.load_config_file(config_file, profile)
 
         credentialsInfo.__init__(self, self.__access_key_id , self.__secret_signing_key, self.__secret_crypto_access_key, self.__host)
 
         if (not self.set()):
             if (self.__access_key_id == None or self.__access_key_id.strip() == ""):
-               raise RuntimeError("Unable to open credentials file '{0}' or unable to find 'acess_key_id' value in profile '{1}' or through environment variable for 'UBIQ_ACCESS_KEY_ID'.".format(config_file, profile))
+               raise RuntimeError("Unable to open credentials file '{0}' or unable to find 'access_key_id' value in profile '{1}' or through environment variable for 'UBIQ_ACCESS_KEY_ID'.".format(config_file, profile))
             elif (self.__secret_signing_key == None or self.__secret_signing_key.strip() == ""):
                raise RuntimeError("Unable to open credentials file '{0}' or unable to find 'secret_signing_key' value in profile '{1}' or through environment variable for 'UBIQ_SECRET_SIGNING_KEY'.".format(config_file, profile))
             elif(self.__secret_crypto_access_key == None or self.__secret_crypto_access_key.strip() == ""):
                raise RuntimeError("Unable to open credentials file '{0}' or unable to find 'secret_crypto_access_key' value in profile '{1}' or through environment variable for 'UBIQ_SECRET_CRYPTO_ACCESS_KEY'.".format(config_file, profile))
+        
+        # Event Tracking
+        self.__configuration = ubiqConfiguration()
+        self.__events = events(self, self.__configuration)
+        self.__eventsProcessor = eventsProcessor(self.__configuration, self.__events)
+        self.__eventsProcessor.start()
+
+    # Forward events to event queue
+    def add_event(self, dataset_name, dataset_group_name, billing_action, dataset_type, key_number, count):
+        return self.__events.add_event(self.__access_key_id, dataset_name, dataset_group_name, billing_action, dataset_type, key_number, count)
 
 
 class credentials(credentialsInfo):
 
     def __init__(self, access_key_id = None, secret_signing_key = None, secret_crypto_access_key = None, host = UBIQ_HOST):
         # If supplied value is None, use ENV variable, otherwise use supplied value.
         # If env value isn't set, use the supplied value anyways (None) but prevent an exception
         self.__access_key_id = (access_key_id, os.getenv('UBIQ_ACCESS_KEY_ID', access_key_id)) [access_key_id == None]
         self.__secret_signing_key = (secret_signing_key, os.getenv('UBIQ_SECRET_SIGNING_KEY', secret_signing_key)) [secret_signing_key == None]
         self.__secret_crypto_access_key = (secret_crypto_access_key, os.getenv('UBIQ_SECRET_CRYPTO_ACCESS_KEY', secret_crypto_access_key)) [secret_crypto_access_key == None]
 
         credentialsInfo.__init__(self, self.__access_key_id,
                                  self.__secret_signing_key,
                                  self.__secret_crypto_access_key, host)
+        
+        # Event Tracking
+        self.__configuration = ubiqConfiguration()
+        self.__events = events(self, self.__configuration)
+        self.__eventsProcessor = eventsProcessor(self.__configuration, self.__events)
+        self.__eventsProcessor.start()
+    
+    # Forward events to event queue
+    def add_event(self, dataset_name, dataset_group_name, billing_action, dataset_type, key_number, count):
+        return self.__events.add_event(self.__access_key_id, dataset_name, dataset_group_name, billing_action, dataset_type, key_number, count)
```

