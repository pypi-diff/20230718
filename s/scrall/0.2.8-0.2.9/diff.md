# Comparing `tmp/scrall-0.2.8.tar.gz` & `tmp/scrall-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrall-0.2.8.tar", last modified: Tue Jul 11 16:35:59 2023, max compression
+gzip compressed data, was "scrall-0.2.9.tar", last modified: Tue Jul 11 20:15:40 2023, max compression
```

## Comparing `scrall-0.2.8.tar` & `scrall-0.2.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-11 16:35:59.141660 scrall-0.2.8/
--rw-r--r--   0 starr      (501) staff       (20)     1072 2023-07-04 22:05:28.000000 scrall-0.2.8/LICENSE
--rw-r--r--   0 starr      (501) staff       (20)       58 2023-07-11 00:01:55.000000 scrall-0.2.8/MANIFEST.in
--rw-r--r--   0 starr      (501) staff       (20)     4431 2023-07-11 16:35:59.141568 scrall-0.2.8/PKG-INFO
--rw-r--r--   0 starr      (501) staff       (20)     2509 2023-07-04 22:05:28.000000 scrall-0.2.8/README.md
--rw-r--r--   0 starr      (501) staff       (20)      977 2023-07-11 16:35:29.000000 scrall-0.2.8/pyproject.toml
--rw-r--r--   0 starr      (501) staff       (20)       38 2023-07-11 16:35:59.141691 scrall-0.2.8/setup.cfg
-drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-11 16:35:59.138965 scrall-0.2.8/src/
-drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-11 16:35:59.140123 scrall-0.2.8/src/scrall/
--rw-r--r--   0 starr      (501) staff       (20)       17 2023-07-11 16:35:29.000000 scrall-0.2.8/src/scrall/__init__.py
--rw-r--r--   0 starr      (501) staff       (20)     1779 2023-07-10 15:11:24.000000 scrall-0.2.8/src/scrall/__main__.py
--rw-r--r--   0 starr      (501) staff       (20)     1764 2023-07-09 14:59:46.000000 scrall-0.2.8/src/scrall/exceptions.py
--rw-r--r--   0 starr      (501) staff       (20)      827 2023-07-09 14:59:46.000000 scrall-0.2.8/src/scrall/log.conf
-drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-11 16:35:59.141211 scrall-0.2.8/src/scrall/parse/
--rw-r--r--   0 starr      (501) staff       (20)        0 2023-07-09 14:59:46.000000 scrall-0.2.8/src/scrall/parse/__init__.py
--rw-r--r--   0 starr      (501) staff       (20)     5014 2023-07-11 16:35:14.000000 scrall-0.2.8/src/scrall/parse/parser.py
--rw-r--r--   0 starr      (501) staff       (20)    34598 2023-07-11 00:01:55.000000 scrall-0.2.8/src/scrall/parse/visitor.py
--rw-r--r--   0 starr      (501) staff       (20)     7533 2023-07-11 00:01:55.000000 scrall-0.2.8/src/scrall/scrall.peg
-drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-11 16:35:59.140923 scrall-0.2.8/src/scrall.egg-info/
--rw-r--r--   0 starr      (501) staff       (20)     4431 2023-07-11 16:35:59.000000 scrall-0.2.8/src/scrall.egg-info/PKG-INFO
--rw-r--r--   0 starr      (501) staff       (20)      447 2023-07-11 16:35:59.000000 scrall-0.2.8/src/scrall.egg-info/SOURCES.txt
--rw-r--r--   0 starr      (501) staff       (20)        1 2023-07-11 16:35:59.000000 scrall-0.2.8/src/scrall.egg-info/dependency_links.txt
--rw-r--r--   0 starr      (501) staff       (20)       48 2023-07-11 16:35:59.000000 scrall-0.2.8/src/scrall.egg-info/entry_points.txt
--rw-r--r--   0 starr      (501) staff       (20)       91 2023-07-11 16:35:59.000000 scrall-0.2.8/src/scrall.egg-info/requires.txt
--rw-r--r--   0 starr      (501) staff       (20)        7 2023-07-11 16:35:59.000000 scrall-0.2.8/src/scrall.egg-info/top_level.txt
+drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-11 20:15:40.184344 scrall-0.2.9/
+-rw-r--r--   0 starr      (501) staff       (20)     1072 2023-07-04 22:05:28.000000 scrall-0.2.9/LICENSE
+-rw-r--r--   0 starr      (501) staff       (20)       58 2023-07-11 00:01:55.000000 scrall-0.2.9/MANIFEST.in
+-rw-r--r--   0 starr      (501) staff       (20)     6956 2023-07-11 20:15:40.184240 scrall-0.2.9/PKG-INFO
+-rw-r--r--   0 starr      (501) staff       (20)     5034 2023-07-11 19:56:35.000000 scrall-0.2.9/README.md
+-rw-r--r--   0 starr      (501) staff       (20)      977 2023-07-11 20:14:46.000000 scrall-0.2.9/pyproject.toml
+-rw-r--r--   0 starr      (501) staff       (20)       38 2023-07-11 20:15:40.184382 scrall-0.2.9/setup.cfg
+drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-11 20:15:40.180055 scrall-0.2.9/src/
+drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-11 20:15:40.180985 scrall-0.2.9/src/scrall/
+-rw-r--r--   0 starr      (501) staff       (20)       17 2023-07-11 20:14:46.000000 scrall-0.2.9/src/scrall/__init__.py
+-rw-r--r--   0 starr      (501) staff       (20)     1779 2023-07-10 15:11:24.000000 scrall-0.2.9/src/scrall/__main__.py
+-rw-r--r--   0 starr      (501) staff       (20)     1764 2023-07-09 14:59:46.000000 scrall-0.2.9/src/scrall/exceptions.py
+-rw-r--r--   0 starr      (501) staff       (20)      827 2023-07-09 14:59:46.000000 scrall-0.2.9/src/scrall/log.conf
+drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-11 20:15:40.183594 scrall-0.2.9/src/scrall/parse/
+-rw-r--r--   0 starr      (501) staff       (20)        0 2023-07-09 14:59:46.000000 scrall-0.2.9/src/scrall/parse/__init__.py
+-rw-r--r--   0 starr      (501) staff       (20)     5014 2023-07-11 16:35:14.000000 scrall-0.2.9/src/scrall/parse/parser.py
+-rw-r--r--   0 starr      (501) staff       (20)    34598 2023-07-11 00:01:55.000000 scrall-0.2.9/src/scrall/parse/visitor.py
+-rw-r--r--   0 starr      (501) staff       (20)     7533 2023-07-11 00:01:55.000000 scrall-0.2.9/src/scrall/scrall.peg
+drwxr-xr-x   0 starr      (501) staff       (20)        0 2023-07-11 20:15:40.181826 scrall-0.2.9/src/scrall.egg-info/
+-rw-r--r--   0 starr      (501) staff       (20)     6956 2023-07-11 20:15:40.000000 scrall-0.2.9/src/scrall.egg-info/PKG-INFO
+-rw-r--r--   0 starr      (501) staff       (20)      447 2023-07-11 20:15:40.000000 scrall-0.2.9/src/scrall.egg-info/SOURCES.txt
+-rw-r--r--   0 starr      (501) staff       (20)        1 2023-07-11 20:15:40.000000 scrall-0.2.9/src/scrall.egg-info/dependency_links.txt
+-rw-r--r--   0 starr      (501) staff       (20)       48 2023-07-11 20:15:40.000000 scrall-0.2.9/src/scrall.egg-info/entry_points.txt
+-rw-r--r--   0 starr      (501) staff       (20)       91 2023-07-11 20:15:40.000000 scrall-0.2.9/src/scrall.egg-info/requires.txt
+-rw-r--r--   0 starr      (501) staff       (20)        7 2023-07-11 20:15:40.000000 scrall-0.2.9/src/scrall.egg-info/top_level.txt
```

### Comparing `scrall-0.2.8/LICENSE` & `scrall-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scrall-0.2.8/PKG-INFO` & `scrall-0.2.9/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,82 @@
-Metadata-Version: 2.1
-Name: scrall
-Version: 0.2.8
-Summary: Starr's Concise Relational Action Language - For Shlaer-Mellor Executable UML
-Author-email: Leon Starr <leon_starr@modelint.com>
-License: MIT License
-        
-        Copyright (c) 2019-2023 Leon Starr
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: repository, https://github.com/modelint/scrall
-Project-URL: documentation, https://github.com/modelint/scrall/wiki
-Keywords: action language,executable uml,mbse,xuml,xtuml,platform independent,sysml
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: build
-Provides-Extra: dev
-License-File: LICENSE
-
 # Scrall Action Language
 Scrall = Starr's Concise Relational Action Language
 
-This is an action language that supports Shlaer-Mellor executable UML. It allows you to specify computation
-inside states, methods, and external entity operations.
+### Why you need this
+
+You are building or exploring Executable UML models using the Shlaer-Mellor methodology and you need a text language
+for specifying actions that:
+
+* perform computations
+* access and traverse the class model
+* synchronize states
+* communicate internally and with external entities
+
+With these qualities:
+* platorm independent action sequencing
+* platform independent data types
+* ability to manipulate both instances and attributres as well as relations (tables)
+* conforms to Date and Darwen's formulation of relational and type theory
+
+Scroll down for more about these qualities.
+
+### Installation
+
+Create or use a python 3.10+ environment. Then
+
+% pip install scrall
+
+At this point you can invoke the parser via the command line or from your python script.
+
+#### From your python script
+
+You need this import statement at a minimum:
+
+    from scrall.parse.parser import ScrallParser
+
+You can then either specify a path or a text variable using the appropriate method:
+
+    result = ScrallParser.parse_text(scrall_text=action_text, debug=False)
+
+OR
+
+    result = ScrallParser.parse_file(file_input=path_to_file, debug=False)
+
+Check the code in `parser.py` to verify I haven't changed these parameters on you wihtout updating the readme.
+
+In either case, `result` will be a list of parsed scrall statements. You may find the header of the `visitor.py`
+file helpful in interpreting these results.
+
+#### From the command line
+
+This is not the intended usage scenario, but may be helpful for testing or exploration. Since scrall may generate
+some diagnostic info you may want to create a fresh working directory and cd into it first. From there...
+
+    % scrall -f somefile.scrall
+
+The .scrall extension is not necessary, but the file must contain scrall text. See this repository's wiki for
+more about the scrall language. The grammar is defined in the [scrall.peg](https://github.com/modelint/scrall/blob/master/src/scrall/scrall.peg) file. (if the link breaks after I do some update to the code, 
+just browse through the code looking for the scrall.peg file, and let me know so I can fix it)
+
+You can also specify a debug option like this:
+
+    % scrall -f somefile.scrall -D
+
+This will create a scrall-diagnostics folder in your current working directory and deposite a coupel of PDFs defining
+the parse of both the scrall grammar: `scrall_parse_tree.pdf` and your supplied text: `scrall_model.pdf`.
+
+You should also see a file named `scrall.log`
+
+### Compatibility
 
 This language is consistent with the [Shlaer Mellor Metamodel](https://github.com/modelint/shlaer-mellor-metamodel),
- another repository on this site.
+ another [repository](https://github.com/modelint/class-model-dsl/wiki) on this site. In that repository the metamodel
+is used to define a schema for a database where user models can be stored and accessed.
+
+### Older documentation
 
 NOTE: If you have the Scrall version 1.0.0 PDF, consider it superceded by the wiki on this site where the language spec is now maintained and updated.
 
 ### Platform independent action sequencing
 
 This language is designed to support data flow execution, so that there is no arbitrary sequencing built in. You can transform
 any chunk of action language (a method, operation, or state activity) into a data flow graph where each action may execute
@@ -72,8 +100,8 @@
 today, I am permanently moving all the latest scrall code back here to its proper home.
 
 When the migration is complete, you will be able to grab the latest Scrall parser from PyPI without having to
 download the whole Shlaer-Mellor metamodel database populator. This separation is essential since you might want
 to define your own action language and parser to use with the metamodel, or just play with Scrall on its own.
 
 I will post another update when it's ready here and on PyPI. The parser is currently in decent shape, so it's just
-a matter of putting a command line interface on it and a bit of packaging.
+a matter of putting a command line interface on it and a bit of packaging.
```

### Comparing `scrall-0.2.8/pyproject.toml` & `scrall-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scrall"
-version = "0.2.8"
+version = "0.2.9"
 description = "Starr's Concise Relational Action Language - For Shlaer-Mellor Executable UML"
 readme = "README.md"
 authors = [{ name = "Leon Starr", email = "leon_starr@modelint.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `scrall-0.2.8/src/scrall/__main__.py` & `scrall-0.2.9/src/scrall/__main__.py`

 * *Files identical despite different names*

### Comparing `scrall-0.2.8/src/scrall/exceptions.py` & `scrall-0.2.9/src/scrall/exceptions.py`

 * *Files identical despite different names*

### Comparing `scrall-0.2.8/src/scrall/log.conf` & `scrall-0.2.9/src/scrall/log.conf`

 * *Files identical despite different names*

### Comparing `scrall-0.2.8/src/scrall/parse/parser.py` & `scrall-0.2.9/src/scrall/parse/parser.py`

 * *Files identical despite different names*

### Comparing `scrall-0.2.8/src/scrall/parse/visitor.py` & `scrall-0.2.9/src/scrall/parse/visitor.py`

 * *Files identical despite different names*

### Comparing `scrall-0.2.8/src/scrall/scrall.peg` & `scrall-0.2.9/src/scrall/scrall.peg`

 * *Files identical despite different names*

