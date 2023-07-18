# Comparing `tmp/mango-framework-0.6.7.tar.gz` & `tmp/mango-framework-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango-framework-0.6.7.tar", last modified: Mon Jul 17 13:52:55 2023, max compression
+gzip compressed data, was "mango-framework-0.7.0.tar", last modified: Tue Jul 18 01:47:25 2023, max compression
```

## Comparing `mango-framework-0.6.7.tar` & `mango-framework-0.7.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 13:52:55.037893 mango-framework-0.6.7/
--rw-r--r--   0 mohammed   (501) staff       (20)     1023 2023-07-17 05:13:07.000000 mango-framework-0.6.7/LICENSE
--rw-r--r--   0 mohammed   (501) staff       (20)     1920 2023-07-17 13:52:55.037776 mango-framework-0.6.7/PKG-INFO
--rw-r--r--   0 mohammed   (501) staff       (20)     1240 2023-07-17 12:32:59.000000 mango-framework-0.6.7/README.md
--rw-r--r--   0 mohammed   (501) staff       (20)     6351 2023-07-17 13:49:28.000000 mango-framework-0.6.7/mango.py
-drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-17 13:52:55.037612 mango-framework-0.6.7/mango_framework.egg-info/
--rw-r--r--   0 mohammed   (501) staff       (20)     1920 2023-07-17 13:52:55.000000 mango-framework-0.6.7/mango_framework.egg-info/PKG-INFO
--rw-r--r--   0 mohammed   (501) staff       (20)      191 2023-07-17 13:52:55.000000 mango-framework-0.6.7/mango_framework.egg-info/SOURCES.txt
--rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 13:52:55.000000 mango-framework-0.6.7/mango_framework.egg-info/dependency_links.txt
--rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-17 13:52:55.000000 mango-framework-0.6.7/mango_framework.egg-info/top_level.txt
--rw-r--r--   0 mohammed   (501) staff       (20)       38 2023-07-17 13:52:55.037933 mango-framework-0.6.7/setup.cfg
--rw-r--r--   0 mohammed   (501) staff       (20)      869 2023-07-17 13:52:22.000000 mango-framework-0.6.7/setup.py
+drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-18 01:47:25.001945 mango-framework-0.7.0/
+-rw-r--r--   0 mohammed   (501) staff       (20)     1023 2023-07-17 05:13:07.000000 mango-framework-0.7.0/LICENSE
+-rw-r--r--   0 mohammed   (501) staff       (20)     1920 2023-07-18 01:47:25.001841 mango-framework-0.7.0/PKG-INFO
+-rw-r--r--   0 mohammed   (501) staff       (20)     1240 2023-07-17 12:32:59.000000 mango-framework-0.7.0/README.md
+-rw-r--r--   0 mohammed   (501) staff       (20)     7202 2023-07-18 01:46:51.000000 mango-framework-0.7.0/mango.py
+drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-18 01:47:25.001672 mango-framework-0.7.0/mango_framework.egg-info/
+-rw-r--r--   0 mohammed   (501) staff       (20)     1920 2023-07-18 01:47:24.000000 mango-framework-0.7.0/mango_framework.egg-info/PKG-INFO
+-rw-r--r--   0 mohammed   (501) staff       (20)      191 2023-07-18 01:47:24.000000 mango-framework-0.7.0/mango_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-18 01:47:24.000000 mango-framework-0.7.0/mango_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-18 01:47:24.000000 mango-framework-0.7.0/mango_framework.egg-info/top_level.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)       38 2023-07-18 01:47:25.001984 mango-framework-0.7.0/setup.cfg
+-rw-r--r--   0 mohammed   (501) staff       (20)      869 2023-07-18 01:47:11.000000 mango-framework-0.7.0/setup.py
```

### Comparing `mango-framework-0.6.7/LICENSE` & `mango-framework-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mango-framework-0.6.7/PKG-INFO` & `mango-framework-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-framework
-Version: 0.6.7
+Version: 0.7.0
 Summary: A lightweight and highly customizable Python framework for building web applications
 Home-page: https://github.com/momo-AUX1/mango
 Author: Mohammed
 Author-email: fdlnaal@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `mango-framework-0.6.7/README.md` & `mango-framework-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `mango-framework-0.6.7/mango.py` & `mango-framework-0.7.0/mango.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from wsgiref.simple_server import make_server
 import json
 from os.path import join
 import sqlite3
 from urllib.parse import parse_qs
+import cgi
 
 templates_path = 'templates'
 
 files_path = 'files'
 
 # Default route
 
@@ -55,14 +56,31 @@
 
     elif req == 'application/x-www-form-urlencoded':
       length = int(environ.get('CONTENT_LENGTH', 0))
       body = environ['wsgi.input'].read(length).decode('utf-8')
       data = parse_qs(body)
       response = routes[path](data)
       start_response(*OK)
+    
+    elif req == 'multipart/form-data':
+      content_type = environ.get('CONTENT_TYPE','')
+      length = int(environ.get('CONTENT_LENGHT',0))
+      form_data = cgi.FieldStorage(fp=environ['wsgi.input'], environ=environ)
+      if 'file' in form_data:
+        file_item = form_data['file']
+        if file_item.filename:
+          file = {'file':file_item,'name':file_item.filename}
+          response = routes[path](file)
+          start_response(*OK)
+        else:
+          response = "<h1> NOT ALLOWED </h1>"
+          start_response(*NOT_ALLOWED)
+      else:
+        response = "<h1> NOT ALLOWED </h1>"
+        start_response(*NOT_ALLOWED)
 
     else:
       response = "<h1> NOT ALLOWED </h1>"
       start_response(*NOT_ALLOWED)
 
   elif path in routes and method == 'GET':
     try:
@@ -115,14 +133,21 @@
   return json.dumps(data), 'application/json'
 
 
 def get_data(info,query):
   data = info[query][0]
   return data
 
+def get_file(data,name):
+  try:
+    with open(name,'wb') as f:
+      f.write(data['file'].file.read())
+  except:
+    with open(data['name'],'wb') as f:
+      f.write(data['file'].file.read())
 
 def send_file(path):
   try:
     with open(join(files_path, path), 'rb') as f:
       response = f.read()
   except:
     with open(path, 'rb') as f:
@@ -177,15 +202,15 @@
         }
     </style>
 </head>
 <body>
     <h1>Server successfully started, but there are no routes or the "/" route is empty</h1>
     <img class="mango-img" src="https://th.bing.com/th/id/R.54bad49b520690f3858b1f396194779d?rik=QSeITH3EbHg4Vw&pid=ImgRaw&r=0" alt="Mango">
     <footer>
-        Version: 0.6.7
+        Version: 0.7.0
         <br>
         <a class="link" href="https://pypi.org/project/mango-framework/">Check out the development!</a>
     </footer>
 </body>
 </html>
 """
 
@@ -228,8 +253,8 @@
     
     def get_user_by_email(self, email):
         result = self.conn.execute('SELECT * FROM Users WHERE email = ?', (email,))
         return result.fetchone()
     
     def get_user_by_password(self, password):
         result = self.conn.execute('SELECT * FROM Users WHERE password = ?', (password,))
-        return result.fetchone()
+        return result.fetchone()
```

### Comparing `mango-framework-0.6.7/mango_framework.egg-info/PKG-INFO` & `mango-framework-0.7.0/mango_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-framework
-Version: 0.6.7
+Version: 0.7.0
 Summary: A lightweight and highly customizable Python framework for building web applications
 Home-page: https://github.com/momo-AUX1/mango
 Author: Mohammed
 Author-email: fdlnaal@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `mango-framework-0.6.7/setup.py` & `mango-framework-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='mango-framework',
-    version='0.6.7',
+    version='0.7.0',
     author='Mohammed',
     author_email='fdlnaal@gmail.com',
     description='A lightweight and highly customizable Python framework for building web applications',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/momo-AUX1/mango',
     packages=['.'],
```

