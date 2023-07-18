# Comparing `tmp/alireza-0.0.4.tar.gz` & `tmp/alireza-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alireza-0.0.4.tar", last modified: Thu Jul  6 01:14:40 2023, max compression
+gzip compressed data, was "alireza-0.0.5.tar", last modified: Tue Jul 18 19:13:56 2023, max compression
```

## Comparing `alireza-0.0.4.tar` & `alireza-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-06 01:14:40.936100 alireza-0.0.4/
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     1775 2023-07-06 01:14:40.936100 alireza-0.0.4/PKG-INFO
--rw-rw-r--   0 alireza   (1000) alireza   (1000)        0 2023-06-14 12:34:33.000000 alireza-0.0.4/README.md
-drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-06 01:14:40.932100 alireza-0.0.4/alireza/
-drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-06 01:14:40.936100 alireza-0.0.4/alireza/DjangoTools/
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     1590 2023-07-05 21:36:04.000000 alireza-0.0.4/alireza/DjangoTools/__Error_Handler.py
--rw-rw-r--   0 alireza   (1000) alireza   (1000)       24 2023-07-04 07:20:15.000000 alireza-0.0.4/alireza/DjangoTools/__init__.py
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     3349 2023-07-06 00:52:33.000000 alireza-0.0.4/alireza/DjangoTools/__manager.py
-drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-06 01:14:40.936100 alireza-0.0.4/alireza/UsefulTools/
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     5256 2023-07-06 00:24:10.000000 alireza-0.0.4/alireza/UsefulTools/__Error_Handler.py
--rw-rw-r--   0 alireza   (1000) alireza   (1000)       24 2023-07-04 22:28:11.000000 alireza-0.0.4/alireza/UsefulTools/__init__.py
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     4117 2023-07-06 00:29:41.000000 alireza-0.0.4/alireza/UsefulTools/__manager.py
--rw-rw-r--   0 alireza   (1000) alireza   (1000)       52 2023-07-04 09:14:57.000000 alireza-0.0.4/alireza/__init__.py
-drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-06 01:14:40.936100 alireza-0.0.4/alireza.egg-info/
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     1775 2023-07-06 01:14:40.000000 alireza-0.0.4/alireza.egg-info/PKG-INFO
--rw-rw-r--   0 alireza   (1000) alireza   (1000)      383 2023-07-06 01:14:40.000000 alireza-0.0.4/alireza.egg-info/SOURCES.txt
--rw-rw-r--   0 alireza   (1000) alireza   (1000)        1 2023-07-06 01:14:40.000000 alireza-0.0.4/alireza.egg-info/dependency_links.txt
--rw-rw-r--   0 alireza   (1000) alireza   (1000)        8 2023-07-06 01:14:40.000000 alireza-0.0.4/alireza.egg-info/top_level.txt
--rw-rw-r--   0 alireza   (1000) alireza   (1000)       38 2023-07-06 01:14:40.936100 alireza-0.0.4/setup.cfg
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     2009 2023-07-06 01:14:05.000000 alireza-0.0.4/setup.py
-drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-06 01:14:40.936100 alireza-0.0.4/test/
--rw-rw-r--   0 alireza   (1000) alireza   (1000)        0 2023-07-06 01:09:15.000000 alireza-0.0.4/test/test.py
+drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-18 19:13:56.374467 alireza-0.0.5/
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     1800 2023-07-18 19:13:56.374467 alireza-0.0.5/PKG-INFO
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)        0 2023-06-14 12:34:33.000000 alireza-0.0.5/README.md
+drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-18 19:13:56.370466 alireza-0.0.5/alireza/
+drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-18 19:13:56.374467 alireza-0.0.5/alireza/DjangoTools/
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     1590 2023-07-05 21:36:04.000000 alireza-0.0.5/alireza/DjangoTools/__Error_Handler.py
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)       24 2023-07-04 07:20:15.000000 alireza-0.0.5/alireza/DjangoTools/__init__.py
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     3321 2023-07-06 01:32:31.000000 alireza-0.0.5/alireza/DjangoTools/__manager.py
+drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-18 19:13:56.374467 alireza-0.0.5/alireza/UsefulTools/
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     6294 2023-07-18 18:48:49.000000 alireza-0.0.5/alireza/UsefulTools/__Error_Handler.py
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)       24 2023-07-04 22:28:11.000000 alireza-0.0.5/alireza/UsefulTools/__init__.py
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     5620 2023-07-18 19:07:20.000000 alireza-0.0.5/alireza/UsefulTools/__manager.py
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)       52 2023-07-04 09:14:57.000000 alireza-0.0.5/alireza/__init__.py
+drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-18 19:13:56.370466 alireza-0.0.5/alireza.egg-info/
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     1800 2023-07-18 19:13:56.000000 alireza-0.0.5/alireza.egg-info/PKG-INFO
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)      383 2023-07-18 19:13:56.000000 alireza-0.0.5/alireza.egg-info/SOURCES.txt
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)        1 2023-07-18 19:13:56.000000 alireza-0.0.5/alireza.egg-info/dependency_links.txt
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)        8 2023-07-18 19:13:56.000000 alireza-0.0.5/alireza.egg-info/top_level.txt
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)       38 2023-07-18 19:13:56.374467 alireza-0.0.5/setup.cfg
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     2040 2023-07-18 19:09:27.000000 alireza-0.0.5/setup.py
+drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-18 19:13:56.374467 alireza-0.0.5/test/
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)        0 2023-07-06 01:09:15.000000 alireza-0.0.5/test/test.py
```

### Comparing `alireza-0.0.4/PKG-INFO` & `alireza-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: alireza
-Version: 0.0.4
-Summary: Comprehensive Toolkit for Boosting Productivity in Python Framework Development
+Version: 0.0.5
+Summary: Comprehensive Toolkit for Boosting Productivity in Python Frameworks Development
 Home-page: UNKNOWN
 Author: Alireza Soroush
 Author-email: alirezasoroush@hotmail.com
 License: UNKNOWN
 Keywords: python,tools,framework,django
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 This extensive toolkit is specifically designed to enhance productivity and streamline the development process 
 when working with Python frameworks. With a wide range of powerful and time-saving tools at your disposal, it empowers developers to tackle 
 complex challenges efficiently and effectively.From scaffolding projects to automating repetitive tasks, this toolkit offers an array of features that 
 simplify common development workflows. It provides seamless integration with popular Python frameworks, 
 offering an extensive collection of utilities, libraries, and modules tailored to enhance the capabilities of your chosen framework.
 Unlock the potential of this comprehensive toolkit and enjoy benefits such as code generation, 
 and much more. Whether you are working on web development, data science, or any other domain, this toolkit serves as a 
 valuable companion throughout the entire development lifecycle.
 Accelerate your Python framework projects, reduce development time, and increase code quality with this indispensable toolkit that caters 
 to the diverse needs of developers, allowing them to focus on delivering exceptional results.
 
+
```

### Comparing `alireza-0.0.4/alireza/DjangoTools/__Error_Handler.py` & `alireza-0.0.5/alireza/DjangoTools/__Error_Handler.py`

 * *Files identical despite different names*

### Comparing `alireza-0.0.4/alireza/DjangoTools/__manager.py` & `alireza-0.0.5/alireza/DjangoTools/__manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 __all__= ['rename_file',]
 
 
 from uuid import uuid4
-from typing import Iterable
 from alireza.DjangoTools.__Error_Handler import _ErrorHandling
 
 
 
 
 
 def __format_finder(all_formats,filename):
```

### Comparing `alireza-0.0.4/alireza/UsefulTools/__manager.py` & `alireza-0.0.5/alireza/UsefulTools/__manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-__all__ = ['random_string','format_finder']
+__all__ = ['random_string','format_finder','string_validator']
 
 
 
 
 
 import secrets
 import string
 from urllib.parse import quote
 from alireza.DjangoTools import rename_file
 from typing import Iterable
 from alireza.UsefulTools.__Error_Handler import _ErrorHandling
-
+import re
 
 
 
 
 def random_string(length:int=15,url_safe:bool=False,regex:str=False,only_letters:bool=False,only_digits:bool=False,
-                  only_lowercase:bool=False,only_uppercase:bool=False,*args,**kwargs):
+                  only_lowercase:bool=False,only_uppercase:bool=False,*args,**kwargs) -> str:
     """
     Generate a random String .
     You can only choose one between regex and only_letters and only_digits .
     Regex must be a string.
     Example:
     >>> regex='AaBbCc123#'
     """
@@ -58,15 +58,15 @@
     return generated_string
 
 
 
 
 
 def format_finder(filenames:Iterable[str],customformats:Iterable[str]|None=None,find_formats:Iterable[str]|None=None,
-                  no_dot_filename:bool |None=False,rename_files:str|None=None,*args,**kwargs):
+                  no_dot_filename:bool |None=False,rename_files:str|None=None,*args,**kwargs) -> str:
     """
     Extract the format from given filenames and return it as a tuple of (filename, ext). 
     Specify a custom format using customformat=['custom.format'], and if that format exists in the filenames, it will be extracted.
     You can also search for a specific format using find_format. If none of the given formats are found, it will return None.
     To remove all dots in the filename, use no_dot_filename.
     Additionally, you can rename the filename with rename_files using a provided string."
     """
@@ -120,7 +120,47 @@
             renamed_result.append(renamed_file)
         return renamed_result
 
 
 
     return result
 
+
+
+
+def string_validator(input_string:str,filter_characters:str,is_allowed:bool=True) -> bool:
+    """
+        *Validates a string based on the filter_characters and is_allowed.*
+        
+        Args:
+        Input_string: The string to be validated.
+        Filter_characters: The set of characters that used to validate the string.
+        is_allowed: Determines the validation behavior.
+            >>> if is_allowed is True -> only allows strings that contain the filter_characters.
+            >>> if is_allowed is False -> only allows strings that does not contain the filter_characters.
+    """
+    _ErrorHandling._string_validator_error_handler(input_string,filter_characters,is_allowed)
+
+    input_string = repr(input_string)[1:-1]
+    filter_characters = repr(filter_characters)[1:-1]
+
+
+    #is allowed
+    if is_allowed:
+        # Define a regular expression pattern for allowed characters
+        pattern = f'^[{re.escape(filter_characters)}]+$'
+        # Check if the input_string matches the pattern
+        if re.match(pattern, input_string):
+            return True
+        else:
+            return False
+    
+
+    #is disallowed
+    elif not is_allowed:
+        # Define a regular expression pattern for disallowed characters
+        pattern = f'[{re.escape(filter_characters)}]'
+        # Check if the input_string matches the pattern
+        if re.search(pattern, input_string):
+            return False
+        else:
+            return True
```

### Comparing `alireza-0.0.4/alireza.egg-info/PKG-INFO` & `alireza-0.0.5/alireza.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: alireza
-Version: 0.0.4
-Summary: Comprehensive Toolkit for Boosting Productivity in Python Framework Development
+Version: 0.0.5
+Summary: Comprehensive Toolkit for Boosting Productivity in Python Frameworks Development
 Home-page: UNKNOWN
 Author: Alireza Soroush
 Author-email: alirezasoroush@hotmail.com
 License: UNKNOWN
 Keywords: python,tools,framework,django
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 This extensive toolkit is specifically designed to enhance productivity and streamline the development process 
 when working with Python frameworks. With a wide range of powerful and time-saving tools at your disposal, it empowers developers to tackle 
 complex challenges efficiently and effectively.From scaffolding projects to automating repetitive tasks, this toolkit offers an array of features that 
 simplify common development workflows. It provides seamless integration with popular Python frameworks, 
 offering an extensive collection of utilities, libraries, and modules tailored to enhance the capabilities of your chosen framework.
 Unlock the potential of this comprehensive toolkit and enjoy benefits such as code generation, 
 and much more. Whether you are working on web development, data science, or any other domain, this toolkit serves as a 
 valuable companion throughout the entire development lifecycle.
 Accelerate your Python framework projects, reduce development time, and increase code quality with this indispensable toolkit that caters 
 to the diverse needs of developers, allowing them to focus on delivering exceptional results.
 
+
```

### Comparing `alireza-0.0.4/setup.py` & `alireza-0.0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4'
-DESCRIPTION = 'Comprehensive Toolkit for Boosting Productivity in Python Framework Development'
+VERSION = '0.0.5'
+DESCRIPTION = 'Comprehensive Toolkit for Boosting Productivity in Python Frameworks Development'
 LONG_DESCRIPTION = """This extensive toolkit is specifically designed to enhance productivity and streamline the development process 
 when working with Python frameworks. With a wide range of powerful and time-saving tools at your disposal, it empowers developers to tackle 
 complex challenges efficiently and effectively.From scaffolding projects to automating repetitive tasks, this toolkit offers an array of features that 
 simplify common development workflows. It provides seamless integration with popular Python frameworks, 
 offering an extensive collection of utilities, libraries, and modules tailored to enhance the capabilities of your chosen framework.
 Unlock the potential of this comprehensive toolkit and enjoy benefits such as code generation, 
 and much more. Whether you are working on web development, data science, or any other domain, this toolkit serves as a 
 valuable companion throughout the entire development lifecycle.
 Accelerate your Python framework projects, reduce development time, and increase code quality with this indispensable toolkit that caters 
-to the diverse needs of developers, allowing them to focus on delivering exceptional results."""
+to the diverse needs of developers, allowing them to focus on delivering exceptional results.
+"""
 
 # Setting up
 setup(
     name="alireza",
     version=VERSION,
     author="Alireza Soroush",
     author_email="alirezasoroush@hotmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
+    python_requires='>=3.6',
     keywords=['python', 'tools', 'framework', 'django',],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

