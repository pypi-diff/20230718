# Comparing `tmp/tokenmonster-1.1.6.tar.gz` & `tmp/tokenmonster-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokenmonster-1.1.6.tar", last modified: Mon Jul 17 03:36:01 2023, max compression
+gzip compressed data, was "tokenmonster-1.1.7.tar", last modified: Tue Jul 18 08:33:40 2023, max compression
```

## Comparing `tokenmonster-1.1.6.tar` & `tokenmonster-1.1.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 03:36:01.471752 tokenmonster-1.1.6/
--rw-r--r--   0 root         (0) root         (0)    15947 2023-07-17 03:36:01.471752 tokenmonster-1.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    16189 2023-07-17 03:31:00.000000 tokenmonster-1.1.6/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 03:36:01.471752 tokenmonster-1.1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      550 2023-07-17 03:30:42.000000 tokenmonster-1.1.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 03:36:01.471752 tokenmonster-1.1.6/tokenmonster.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15947 2023-07-17 03:36:01.000000 tokenmonster-1.1.6/tokenmonster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      178 2023-07-17 03:36:01.000000 tokenmonster-1.1.6/tokenmonster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 03:36:01.000000 tokenmonster-1.1.6/tokenmonster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 03:36:01.000000 tokenmonster-1.1.6/tokenmonster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    48319 2023-07-17 03:28:52.000000 tokenmonster-1.1.6/tokenmonster.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 08:33:40.403322 tokenmonster-1.1.7/
+-rw-r--r--   0 root         (0) root         (0)    15947 2023-07-18 08:33:40.403322 tokenmonster-1.1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    16189 2023-07-17 03:31:00.000000 tokenmonster-1.1.7/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 08:33:40.403322 tokenmonster-1.1.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      550 2023-07-18 08:29:59.000000 tokenmonster-1.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 08:33:40.403322 tokenmonster-1.1.7/tokenmonster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15947 2023-07-18 08:33:40.000000 tokenmonster-1.1.7/tokenmonster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      178 2023-07-18 08:33:40.000000 tokenmonster-1.1.7/tokenmonster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 08:33:40.000000 tokenmonster-1.1.7/tokenmonster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 08:33:40.000000 tokenmonster-1.1.7/tokenmonster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    48326 2023-07-18 08:29:28.000000 tokenmonster-1.1.7/tokenmonster.py
```

### Comparing `tokenmonster-1.1.6/PKG-INFO` & `tokenmonster-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokenmonster
-Version: 1.1.6
+Version: 1.1.7
 Summary: Tokenize and decode text with TokenMonster vocabularies.
 Home-page: https://github.com/alasdairforsythe/tokenmonster
 Author: Alasdair Forsythe
 Author-email: 77910352+alasdairforsythe@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `tokenmonster-1.1.6/README.md` & `tokenmonster-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `tokenmonster-1.1.6/setup.py` & `tokenmonster-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='tokenmonster',
-    version='1.1.6',
+    version='1.1.7',
     py_modules=['tokenmonster'],
     author='Alasdair Forsythe',
     author_email='77910352+alasdairforsythe@users.noreply.github.com',
     description='Tokenize and decode text with TokenMonster vocabularies.',
     url='https://github.com/alasdairforsythe/tokenmonster',
     license='MIT',
     long_description=long_description,
```

### Comparing `tokenmonster-1.1.6/tokenmonster.egg-info/PKG-INFO` & `tokenmonster-1.1.7/tokenmonster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokenmonster
-Version: 1.1.6
+Version: 1.1.7
 Summary: Tokenize and decode text with TokenMonster vocabularies.
 Home-page: https://github.com/alasdairforsythe/tokenmonster
 Author: Alasdair Forsythe
 Author-email: 77910352+alasdairforsythe@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `tokenmonster-1.1.6/tokenmonster.py` & `tokenmonster-1.1.7/tokenmonster.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
          vocab.unk = unk
     if vocab.vocab_size > 65536:
         vocab.encoding_length = 4
     else:
         vocab.encoding_length = 2
     vocab.fname = None
     vocab.dictionary = None
-    vocab.token_to_id = None
+    vocab._token_to_id = None
     vocab._modified_id = 0
     vocab._decoders = []
     return vocab
 
 class Vocab:
     """
     Main class for TokenMonster.
@@ -220,15 +220,15 @@
         self.fname = path
         path_encoded = path.encode("utf-8")
         if len(path_encoded) > 255:
             raise RuntimeError("TokenMonster: Vocabulary filepath is too long, it must be less than 256 characters")
         payload = _write_uint8(len(path_encoded)) + path_encoded
         self.id = Vocab._communicate(10, 0, len(payload), payload)
         self.dictionary = None
-        self.token_to_id = None
+        self._token_to_id = None
         self._modified_id = 0
         self._decoders = []
 
     def _unload(self):
         if hasattr(self, 'id'):
             if self.id is not None:
                 if self._modified_id != -1:
@@ -554,15 +554,15 @@
             raise RuntimeError("TokenMonster: Access denied to expired Vocab instance.")
         job_type = 15
         response = Vocab._communicate(job_type, self.id, 0)
         size = _read_uint32(response[0:4])
         self.vocab_size = size # it should be already the same
         offset = 4
         self.dictionary = {}
-        self.token_to_id = {}
+        self._token_to_id = {}
         self.unk = None
         types = ["regular", "single", "special", "unk"]
         for _ in range(size):
             id = _read_uint32(response[offset: offset + 4])
             offset += 4
             len_token = response[offset]
             len_token_decoded = response[offset + 1]
@@ -570,16 +570,16 @@
             score = _read_float32(response[offset + 3: offset + 7])
             offset += 7
             token = self._bytes_to_string(response[offset : offset + len_token])
             offset += len_token
             token_decoded = self._bytes_to_string(response[offset : offset + len_token_decoded])
             offset += len_token_decoded
             self.dictionary[id] = {'id': id, 'token': token, 'token_decoded': token_decoded, 'type': types[typ], 'score': score}
-            self.token_to_id[token] = id
-            self.token_to_id[token_decoded] = id
+            self._token_to_id[token] = id
+            self._token_to_id[token_decoded] = id
             if typ == 3:
                 self.unk = id
         return self.dictionary
     
     def id_to_token(self, id):
         """
         Get the token string from a single token ID, in it's capcode-encoded form.
@@ -624,15 +624,15 @@
             token: string
 
         Returns:
             int or None
         """
         if self.dictionary is None:
             self.get_dictionary()
-        return self.token_to_id.get(token, None)
+        return self._token_to_id.get(token, None)
     
     def unk_token_id(self):
         """
         Returns the ID of the UNK token, or 'None' type if there is no UNK token
 
         Parameters:
             token: string
@@ -952,15 +952,15 @@
                         raise ValueError("TokenMonster: Invalid input for vocabulary modification. Input should be string or bytes string, or list thereof.")
         else:
             raise ValueError("TokenMonster: Invalid input for vocabulary modification. Input should be string or bytes string, or list thereof.")
     
     def _modified(self):
         self._modified_id += 1
         self.dictionary = None
-        self.token_to_id = None
+        self._token_to_id = None
         self.unk = False
         if self.vocab_size > 65536:
             self.encoding_length = 4
         else:
             self.encoding_length = 2
         # Unload all the decoder objects
         for _, decoder_id in enumerate(self._decoders):
```

