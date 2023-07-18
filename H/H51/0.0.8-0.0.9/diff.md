# Comparing `tmp/H51-0.0.8.tar.gz` & `tmp/H51-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/H51-0.0.8.tar", last modified: Fri Dec  3 11:45:04 2021, max compression
+gzip compressed data, was "H51-0.0.9.tar", last modified: Tue Jul 18 15:35:37 2023, max compression
```

## Comparing `H51-0.0.8.tar` & `H51-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2021-12-03 11:45:04.000000 H51-0.0.8/
-drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2021-12-03 11:45:04.000000 H51-0.0.8/H51.egg-info/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2416 2021-12-03 11:45:03.000000 H51-0.0.8/H51.egg-info/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)      367 2021-12-03 11:45:04.000000 H51-0.0.8/H51.egg-info/SOURCES.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2021-12-03 11:45:03.000000 H51-0.0.8/H51.egg-info/dependency_links.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       17 2021-12-03 11:45:03.000000 H51-0.0.8/H51.egg-info/requires.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        4 2021-12-03 11:45:03.000000 H51-0.0.8/H51.egg-info/top_level.txt
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1101 2019-08-03 11:56:30.000000 H51-0.0.8/LICENSE
--rw-rw-r--   0 anthony   (1000) anthony   (1000)       61 2019-08-03 11:56:47.000000 H51-0.0.8/MANIFEST.in
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2416 2021-12-03 11:45:04.000000 H51-0.0.8/PKG-INFO
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1221 2019-11-25 13:29:57.000000 H51-0.0.8/README.md
-drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2021-12-03 11:45:04.000000 H51-0.0.8/h51/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      121 2019-08-03 11:42:54.000000 H51-0.0.8/h51/__init__.py
-drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2021-12-03 11:45:04.000000 H51-0.0.8/h51/analyzers/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      501 2019-08-02 23:48:05.000000 H51-0.0.8/h51/analyzers/__init__.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1072 2019-08-03 00:11:06.000000 H51-0.0.8/h51/analyzers/images.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3252 2019-11-25 13:31:45.000000 H51-0.0.8/h51/client.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     2813 2019-08-01 13:27:06.000000 H51-0.0.8/h51/exceptions.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     1076 2019-08-02 00:08:40.000000 H51-0.0.8/h51/pagination.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)    11713 2021-12-03 11:36:06.000000 H51-0.0.8/h51/resources.py
-drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2021-12-03 11:45:04.000000 H51-0.0.8/h51/transforms/
--rw-rw-r--   0 anthony   (1000) anthony   (1000)      523 2019-08-03 00:10:35.000000 H51-0.0.8/h51/transforms/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2405 2019-11-25 02:43:47.000000 H51-0.0.8/h51/transforms/images.py
--rw-rw-r--   0 anthony   (1000) anthony   (1000)       79 2021-12-03 11:45:04.000000 H51-0.0.8/setup.cfg
--rw-rw-r--   0 anthony   (1000) anthony   (1000)     3727 2021-12-03 11:36:19.000000 H51-0.0.8/setup.py
+drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2023-07-18 15:35:37.779190 H51-0.0.9/
+drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2023-07-18 15:35:37.723190 H51-0.0.9/H51.egg-info/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1987 2023-07-18 15:35:37.000000 H51-0.0.9/H51.egg-info/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      367 2023-07-18 15:35:37.000000 H51-0.0.9/H51.egg-info/SOURCES.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2023-07-18 15:35:37.000000 H51-0.0.9/H51.egg-info/dependency_links.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       17 2023-07-18 15:35:37.000000 H51-0.0.9/H51.egg-info/requires.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        4 2023-07-18 15:35:37.000000 H51-0.0.9/H51.egg-info/top_level.txt
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1101 2019-08-03 11:56:30.000000 H51-0.0.9/LICENSE
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)       61 2019-08-03 11:56:47.000000 H51-0.0.9/MANIFEST.in
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1987 2023-07-18 15:35:37.779190 H51-0.0.9/PKG-INFO
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1221 2019-11-25 13:29:57.000000 H51-0.0.9/README.md
+drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2023-07-18 15:35:37.755190 H51-0.0.9/h51/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      121 2019-08-03 11:42:54.000000 H51-0.0.9/h51/__init__.py
+drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2023-07-18 15:35:37.759190 H51-0.0.9/h51/analyzers/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      501 2019-08-02 23:48:05.000000 H51-0.0.9/h51/analyzers/__init__.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1072 2019-08-03 00:11:06.000000 H51-0.0.9/h51/analyzers/images.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3252 2019-11-25 13:31:45.000000 H51-0.0.9/h51/client.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     2813 2019-08-01 13:27:06.000000 H51-0.0.9/h51/exceptions.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     1076 2019-08-02 00:08:40.000000 H51-0.0.9/h51/pagination.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)    12228 2023-07-18 15:35:09.000000 H51-0.0.9/h51/resources.py
+drwxrwxr-x   0 anthony   (1000) anthony   (1000)        0 2023-07-18 15:35:37.767190 H51-0.0.9/h51/transforms/
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)      523 2019-08-03 00:10:35.000000 H51-0.0.9/h51/transforms/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2405 2019-11-25 02:43:47.000000 H51-0.0.9/h51/transforms/images.py
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)       79 2023-07-18 15:35:37.783190 H51-0.0.9/setup.cfg
+-rw-rw-r--   0 anthony   (1000) anthony   (1000)     3727 2023-07-18 15:34:36.000000 H51-0.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `H51-0.0.8/H51.egg-info/PKG-INFO` & `H51-0.0.9/H51.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,77 +1,80 @@
 Metadata-Version: 2.1
 Name: H51
-Version: 0.0.8
+Version: 0.0.9
 Summary: The H51 Python library provides a pythonic interface to the H51 API.
 Home-page: https://github.com/GetmeUK/h51-python
 Author: Anthony Blackshaw
 Author-email: ant@getme.co.uk
 Maintainer: Anthony Blackshaw
 Maintainer-email: ant@getme.co.uk
 License: MIT
-Description: # H51 Python Library
-        
-        The H51 Python library provides a pythonic interface to the H51 API. It includes an API client class, a set of resource classes and classes for configuring core analyzers and transforms.
-        
-        
-        ## Installation
-        
-        ```
-        pip install h51
-        ```
-        
-        ## Requirements
-        
-        - Python 3.7+
-        
-        
-        # Usage
-        
-        ```Python
-        
-        import h51
-        
-        
-        client = h51.Client('your_api_key...')
-        
-        # Create an asset
-        with open('image.bmp') as f:
-            asset = h51.resources.Asset.create(client, f)
-        
-        # Analyze the image asset to find its dominant colours and focal point
-        asset.analyze([
-            h51.analyzers.images.DominantColors(),
-            h51.analyzers.images.FocalPoint()
-        ])
-        
-        # Create web optimized variations of the image
-        h51.resources.Variation.create(
-            asset,
-            {
-                'x1': [
-                    h51.transforms.images.AutoOrient(),
-                    h51.transforms.images.FocalPointCrop(aspect_ratio=0.5),
-                    h51.transforms.images.Fit(640, 640),
-                    h51.transforms.images.Output('WebP')
-                ],
-                'x2': [
-                    h51.transforms.images.AutoOrient(),
-                    h51.transforms.images.FocalPointCrop(aspect_ratio=0.5),
-                    h51.transforms.images.Fit(1280, 1280),
-                    h51.transforms.images.Output('WebP')
-                ]
-            }
-        )
-        
-        ```
-        
 Keywords: api h51
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Database
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# H51 Python Library
+
+The H51 Python library provides a pythonic interface to the H51 API. It includes an API client class, a set of resource classes and classes for configuring core analyzers and transforms.
+
+
+## Installation
+
+```
+pip install h51
+```
+
+## Requirements
+
+- Python 3.7+
+
+
+# Usage
+
+```Python
+
+import h51
+
+
+client = h51.Client('your_api_key...')
+
+# Create an asset
+with open('image.bmp') as f:
+    asset = h51.resources.Asset.create(client, f)
+
+# Analyze the image asset to find its dominant colours and focal point
+asset.analyze([
+    h51.analyzers.images.DominantColors(),
+    h51.analyzers.images.FocalPoint()
+])
+
+# Create web optimized variations of the image
+h51.resources.Variation.create(
+    asset,
+    {
+        'x1': [
+            h51.transforms.images.AutoOrient(),
+            h51.transforms.images.FocalPointCrop(aspect_ratio=0.5),
+            h51.transforms.images.Fit(640, 640),
+            h51.transforms.images.Output('WebP')
+        ],
+        'x2': [
+            h51.transforms.images.AutoOrient(),
+            h51.transforms.images.FocalPointCrop(aspect_ratio=0.5),
+            h51.transforms.images.Fit(1280, 1280),
+            h51.transforms.images.Output('WebP')
+        ]
+    }
+)
+
+```
+
+
```

### Comparing `H51-0.0.8/LICENSE` & `H51-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `H51-0.0.8/PKG-INFO` & `H51-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,77 +1,80 @@
 Metadata-Version: 2.1
 Name: H51
-Version: 0.0.8
+Version: 0.0.9
 Summary: The H51 Python library provides a pythonic interface to the H51 API.
 Home-page: https://github.com/GetmeUK/h51-python
 Author: Anthony Blackshaw
 Author-email: ant@getme.co.uk
 Maintainer: Anthony Blackshaw
 Maintainer-email: ant@getme.co.uk
 License: MIT
-Description: # H51 Python Library
-        
-        The H51 Python library provides a pythonic interface to the H51 API. It includes an API client class, a set of resource classes and classes for configuring core analyzers and transforms.
-        
-        
-        ## Installation
-        
-        ```
-        pip install h51
-        ```
-        
-        ## Requirements
-        
-        - Python 3.7+
-        
-        
-        # Usage
-        
-        ```Python
-        
-        import h51
-        
-        
-        client = h51.Client('your_api_key...')
-        
-        # Create an asset
-        with open('image.bmp') as f:
-            asset = h51.resources.Asset.create(client, f)
-        
-        # Analyze the image asset to find its dominant colours and focal point
-        asset.analyze([
-            h51.analyzers.images.DominantColors(),
-            h51.analyzers.images.FocalPoint()
-        ])
-        
-        # Create web optimized variations of the image
-        h51.resources.Variation.create(
-            asset,
-            {
-                'x1': [
-                    h51.transforms.images.AutoOrient(),
-                    h51.transforms.images.FocalPointCrop(aspect_ratio=0.5),
-                    h51.transforms.images.Fit(640, 640),
-                    h51.transforms.images.Output('WebP')
-                ],
-                'x2': [
-                    h51.transforms.images.AutoOrient(),
-                    h51.transforms.images.FocalPointCrop(aspect_ratio=0.5),
-                    h51.transforms.images.Fit(1280, 1280),
-                    h51.transforms.images.Output('WebP')
-                ]
-            }
-        )
-        
-        ```
-        
 Keywords: api h51
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Database
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# H51 Python Library
+
+The H51 Python library provides a pythonic interface to the H51 API. It includes an API client class, a set of resource classes and classes for configuring core analyzers and transforms.
+
+
+## Installation
+
+```
+pip install h51
+```
+
+## Requirements
+
+- Python 3.7+
+
+
+# Usage
+
+```Python
+
+import h51
+
+
+client = h51.Client('your_api_key...')
+
+# Create an asset
+with open('image.bmp') as f:
+    asset = h51.resources.Asset.create(client, f)
+
+# Analyze the image asset to find its dominant colours and focal point
+asset.analyze([
+    h51.analyzers.images.DominantColors(),
+    h51.analyzers.images.FocalPoint()
+])
+
+# Create web optimized variations of the image
+h51.resources.Variation.create(
+    asset,
+    {
+        'x1': [
+            h51.transforms.images.AutoOrient(),
+            h51.transforms.images.FocalPointCrop(aspect_ratio=0.5),
+            h51.transforms.images.Fit(640, 640),
+            h51.transforms.images.Output('WebP')
+        ],
+        'x2': [
+            h51.transforms.images.AutoOrient(),
+            h51.transforms.images.FocalPointCrop(aspect_ratio=0.5),
+            h51.transforms.images.Fit(1280, 1280),
+            h51.transforms.images.Output('WebP')
+        ]
+    }
+)
+
+```
+
+
```

### Comparing `H51-0.0.8/README.md` & `H51-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `H51-0.0.8/h51/analyzers/images.py` & `H51-0.0.9/h51/analyzers/images.py`

 * *Files identical despite different names*

### Comparing `H51-0.0.8/h51/client.py` & `H51-0.0.9/h51/client.py`

 * *Files identical despite different names*

### Comparing `H51-0.0.8/h51/exceptions.py` & `H51-0.0.9/h51/exceptions.py`

 * *Files identical despite different names*

### Comparing `H51-0.0.8/h51/pagination.py` & `H51-0.0.9/h51/pagination.py`

 * *Files identical despite different names*

### Comparing `H51-0.0.8/h51/resources.py` & `H51-0.0.9/h51/resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,14 +146,22 @@
         r = self._client(
             'post',
             f'assets/{self.uid}/persist'
         )
 
         self._document.update(r)
 
+    def shallow_copy(self):
+        """Shallow copy an asset (remove the expires time)"""
+
+        r = self._client(
+            'post',
+            f'assets/{self.uid}/shallow-copy'
+        )
+
     @classmethod
     def all(cls, client, secure=None, type=None, q=None, rate_buffer=0):
         """
         Get all assets.
 
         Setting the `rate_buffer` to a value greater than 0 ensures the method
         will wait before continuing to fetch results if the number of
@@ -302,14 +310,26 @@
         return client(
             'post',
             'assets/persist',
             data={'uids': uids}
         )
 
     @classmethod
+    def shallow_copy_many(cls, client, uids):
+        """
+        Find one or more assets matching the given uids and shallow copy them
+        (remove the expires time).
+        """
+        return client(
+            'post',
+            'assets/shallow-copy',
+            data={'uids': uids}
+        )
+
+    @classmethod
     def zip(
         cls,
         client,
         uids,
         name,
         expire=None,
         secure=False,
```

### Comparing `H51-0.0.8/h51/transforms/__init__.py` & `H51-0.0.9/h51/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `H51-0.0.8/h51/transforms/images.py` & `H51-0.0.9/h51/transforms/images.py`

 * *Files identical despite different names*

### Comparing `H51-0.0.8/setup.py` & `H51-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 setup(
     name='H51',
 
     # Versions should comply with PEP440. For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.8',
+    version='0.0.9',
     description=\
         'The H51 Python library provides a pythonic interface to the H51 API.',
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     # The project's main homepage.
     url='https://github.com/GetmeUK/h51-python',
```

