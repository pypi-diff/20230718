# Comparing `tmp/flask_protobuf-0.1.0.tar.gz` & `tmp/flask_protobuf-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_protobuf-0.1.0.tar", last modified: Mon Jul 17 04:19:30 2023, max compression
+gzip compressed data, was "flask_protobuf-0.1.3.tar", last modified: Tue Jul 18 00:01:14 2023, max compression
```

## Comparing `flask_protobuf-0.1.0.tar` & `flask_protobuf-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 jgutierrez   (503) staff       (20)        0 2023-07-17 04:19:30.364126 flask_protobuf-0.1.0/
--rw-r--r--   0 jgutierrez   (503) staff       (20)     1068 2023-07-17 03:34:07.000000 flask_protobuf-0.1.0/LICENSE.txt
--rw-r--r--   0 jgutierrez   (503) staff       (20)       84 2023-07-17 04:19:30.363728 flask_protobuf-0.1.0/PKG-INFO
-drwxr-xr-x   0 jgutierrez   (503) staff       (20)        0 2023-07-17 04:19:30.357657 flask_protobuf-0.1.0/flask_protobuf/
--rw-r--r--   0 jgutierrez   (503) staff       (20)      136 2023-07-16 10:00:26.000000 flask_protobuf-0.1.0/flask_protobuf/__init__.py
--rw-r--r--   0 jgutierrez   (503) staff       (20)     5650 2023-07-17 03:59:13.000000 flask_protobuf-0.1.0/flask_protobuf/extension.py
-drwxr-xr-x   0 jgutierrez   (503) staff       (20)        0 2023-07-17 04:19:30.362705 flask_protobuf-0.1.0/flask_protobuf.egg-info/
--rw-r--r--   0 jgutierrez   (503) staff       (20)       84 2023-07-17 04:19:30.000000 flask_protobuf-0.1.0/flask_protobuf.egg-info/PKG-INFO
--rw-r--r--   0 jgutierrez   (503) staff       (20)      264 2023-07-17 04:19:30.000000 flask_protobuf-0.1.0/flask_protobuf.egg-info/SOURCES.txt
--rw-r--r--   0 jgutierrez   (503) staff       (20)        1 2023-07-17 04:19:30.000000 flask_protobuf-0.1.0/flask_protobuf.egg-info/dependency_links.txt
--rw-r--r--   0 jgutierrez   (503) staff       (20)       30 2023-07-17 04:19:30.000000 flask_protobuf-0.1.0/flask_protobuf.egg-info/requires.txt
--rw-r--r--   0 jgutierrez   (503) staff       (20)       15 2023-07-17 04:19:30.000000 flask_protobuf-0.1.0/flask_protobuf.egg-info/top_level.txt
--rw-r--r--   0 jgutierrez   (503) staff       (20)       38 2023-07-17 04:19:30.364265 flask_protobuf-0.1.0/setup.cfg
--rw-r--r--   0 jgutierrez   (503) staff       (20)      201 2023-07-17 03:30:23.000000 flask_protobuf-0.1.0/setup.py
+drwxr-xr-x   0 jgutierrez   (503) staff       (20)        0 2023-07-18 00:01:14.997697 flask_protobuf-0.1.3/
+-rw-r--r--   0 jgutierrez   (503) staff       (20)     1068 2023-07-17 03:34:07.000000 flask_protobuf-0.1.3/LICENSE.txt
+-rw-r--r--   0 jgutierrez   (503) staff       (20)      431 2023-07-18 00:01:14.997333 flask_protobuf-0.1.3/PKG-INFO
+-rw-r--r--   0 jgutierrez   (503) staff       (20)     2819 2023-07-17 23:58:05.000000 flask_protobuf-0.1.3/README.md
+drwxr-xr-x   0 jgutierrez   (503) staff       (20)        0 2023-07-18 00:01:14.993552 flask_protobuf-0.1.3/flask_protobuf/
+-rw-r--r--   0 jgutierrez   (503) staff       (20)      136 2023-07-16 10:00:26.000000 flask_protobuf-0.1.3/flask_protobuf/__init__.py
+-rw-r--r--   0 jgutierrez   (503) staff       (20)     6346 2023-07-17 23:29:04.000000 flask_protobuf-0.1.3/flask_protobuf/extension.py
+drwxr-xr-x   0 jgutierrez   (503) staff       (20)        0 2023-07-18 00:01:14.996581 flask_protobuf-0.1.3/flask_protobuf.egg-info/
+-rw-r--r--   0 jgutierrez   (503) staff       (20)      431 2023-07-18 00:01:14.000000 flask_protobuf-0.1.3/flask_protobuf.egg-info/PKG-INFO
+-rw-r--r--   0 jgutierrez   (503) staff       (20)      274 2023-07-18 00:01:14.000000 flask_protobuf-0.1.3/flask_protobuf.egg-info/SOURCES.txt
+-rw-r--r--   0 jgutierrez   (503) staff       (20)        1 2023-07-18 00:01:14.000000 flask_protobuf-0.1.3/flask_protobuf.egg-info/dependency_links.txt
+-rw-r--r--   0 jgutierrez   (503) staff       (20)       30 2023-07-18 00:01:14.000000 flask_protobuf-0.1.3/flask_protobuf.egg-info/requires.txt
+-rw-r--r--   0 jgutierrez   (503) staff       (20)       15 2023-07-18 00:01:14.000000 flask_protobuf-0.1.3/flask_protobuf.egg-info/top_level.txt
+-rw-r--r--   0 jgutierrez   (503) staff       (20)       38 2023-07-18 00:01:14.997838 flask_protobuf-0.1.3/setup.cfg
+-rw-r--r--   0 jgutierrez   (503) staff       (20)      611 2023-07-18 00:01:12.000000 flask_protobuf-0.1.3/setup.py
```

### Comparing `flask_protobuf-0.1.0/LICENSE.txt` & `flask_protobuf-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flask_protobuf-0.1.0/flask_protobuf/extension.py` & `flask_protobuf-0.1.3/flask_protobuf/extension.py`

 * *Files 19% similar despite different names*

```diff
@@ -84,34 +84,39 @@
 
     def __call__(self, requestMessage=None,**decor_kwargs):
         def decorator(view_func):
             @wraps(view_func)
             def decorated_view(*args, **kwargs):
                 # Customizations using the 'param' before the request
                 #check if the request is a protobuf message before anything else
-                instance_parse_to_dict = decor_kwargs.get('parse_dict',self.parse_to_dict)
-                instance_strict_message_validation = decor_kwargs.get('strict_message_validation',self.strict_message_validation)
+                instance_parse_to_dict = decor_kwargs.get('parse_dict',None)
+                instance_strict_message_validation = decor_kwargs.get('strict_message_validation',None)
                 exception_message = None
                 d = requestMessage()
                 if requestMessage==None:
                     raise Exception("No protobuf message passed to decorator")
                 try:
                     '''
                     enforces a default behavior of returning a 500 error if the message received is not a protobuf message
                     '''
                     d.ParseFromString(request.data)
-                    if(self.strict_message_validation or instance_strict_message_validation):
+                    if((self.strict_message_validation or instance_strict_message_validation) and instance_strict_message_validation != False):
+                        #when the global values are set to true, the decorator will check if the message received is the expected message
+                        #the behavior can be overriden by passing strict_message_validation=False to the decorator
+                        #when the global is set to False, the behavior can be overriden by passing strict_message_validation=True to the decorator
                         if(self.__is_message_valid(d) == False):
                             exception_message = self.__create_protobuf_guide(d)
 
                 except:
                     exception_message = self.__create_protobuf_guide(d)
         
-                if(self.parse_to_dict or instance_parse_to_dict):
+                if((self.parse_to_dict or instance_parse_to_dict) and instance_parse_to_dict != False):
                     #some users might want to parse the protobuf to a dict, so they can use the data outside the protobuf schema
+                    #the behavior can be overriden by passing instance_parse_to_dict=False to the decorator
+                    #when the global is set to False, the behavior can be overriden by passing instance_parse_to_dict=True to the decorator
                     request.data = self.__parse_protobuf_to_dict(d)
                 # Call the original view function
 
                 #if there was an exception, return the guide to the user
                 if(exception_message):
                     return jsonify(exception_message),500
```

