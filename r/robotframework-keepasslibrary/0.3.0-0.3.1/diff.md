# Comparing `tmp/robotframework-keepasslibrary-0.3.0.tar.gz` & `tmp/robotframework-keepasslibrary-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\robotframework-keepasslibrary-0.3.0.tar", last modified: Fri Oct 30 15:27:00 2020, max compression
+gzip compressed data, was "robotframework-keepasslibrary-0.3.1.tar", last modified: Fri Aug  5 14:41:42 2022, max compression
```

## Comparing `robotframework-keepasslibrary-0.3.0.tar` & `robotframework-keepasslibrary-0.3.1.tar`

### file list

```diff
@@ -1,28 +1,60 @@
-drwxrwxrwx   0        0        0        0 2020-10-30 15:27:00.683459 robotframework-keepasslibrary-0.3.0/
--rw-rw-rw-   0        0        0       15 2020-10-30 13:55:53.000000 robotframework-keepasslibrary-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4038 2020-10-30 15:27:00.682462 robotframework-keepasslibrary-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2463 2020-10-30 14:51:58.000000 robotframework-keepasslibrary-0.3.0/README.md
--rw-rw-rw-   0        0        0       76 2020-10-30 14:51:58.000000 robotframework-keepasslibrary-0.3.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2020-10-30 15:27:00.683459 robotframework-keepasslibrary-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2115 2020-10-30 14:51:58.000000 robotframework-keepasslibrary-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2020-10-30 15:27:00.596937 robotframework-keepasslibrary-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2020-10-30 15:27:00.607958 robotframework-keepasslibrary-0.3.0/src/KeePassLibrary/
--rw-rw-rw-   0        0        0     3728 2020-10-30 14:52:44.000000 robotframework-keepasslibrary-0.3.0/src/KeePassLibrary/__init__.py
-drwxrwxrwx   0        0        0        0 2020-10-30 15:27:00.617969 robotframework-keepasslibrary-0.3.0/src/KeePassLibrary/base/
--rw-rw-rw-   0        0        0      256 2020-10-30 14:51:58.000000 robotframework-keepasslibrary-0.3.0/src/KeePassLibrary/base/__init__.py
--rw-rw-rw-   0        0        0      484 2020-10-30 14:51:58.000000 robotframework-keepasslibrary-0.3.0/src/KeePassLibrary/base/context.py
--rw-rw-rw-   0        0        0     1023 2020-10-30 14:51:57.000000 robotframework-keepasslibrary-0.3.0/src/KeePassLibrary/base/librarycomponent.py
--rw-rw-rw-   0        0        0      444 2020-10-30 14:51:58.000000 robotframework-keepasslibrary-0.3.0/src/KeePassLibrary/errors.py
-drwxrwxrwx   0        0        0        0 2020-10-30 15:27:00.631931 robotframework-keepasslibrary-0.3.0/src/KeePassLibrary/keywords/
--rw-rw-rw-   0        0        0      213 2020-10-30 14:51:58.000000 robotframework-keepasslibrary-0.3.0/src/KeePassLibrary/keywords/__init__.py
--rw-rw-rw-   0        0        0     6250 2020-10-30 14:51:58.000000 robotframework-keepasslibrary-0.3.0/src/KeePassLibrary/keywords/keepassdatabase.py
--rw-rw-rw-   0        0        0    12239 2020-10-30 14:51:58.000000 robotframework-keepasslibrary-0.3.0/src/KeePassLibrary/keywords/keepassentries.py
--rw-rw-rw-   0        0        0    22793 2020-10-30 14:51:58.000000 robotframework-keepasslibrary-0.3.0/src/KeePassLibrary/keywords/keepassentry.py
--rw-rw-rw-   0        0        0    13553 2020-10-30 14:51:58.000000 robotframework-keepasslibrary-0.3.0/src/KeePassLibrary/keywords/keepassgroup.py
--rw-rw-rw-   0        0        0     7264 2020-10-30 14:51:58.000000 robotframework-keepasslibrary-0.3.0/src/KeePassLibrary/keywords/keepassgroups.py
-drwxrwxrwx   0        0        0        0 2020-10-30 15:27:00.679459 robotframework-keepasslibrary-0.3.0/src/robotframework_keepasslibrary.egg-info/
--rw-rw-rw-   0        0        0     4038 2020-10-30 15:27:00.000000 robotframework-keepasslibrary-0.3.0/src/robotframework_keepasslibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      772 2020-10-30 15:27:00.000000 robotframework-keepasslibrary-0.3.0/src/robotframework_keepasslibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-10-30 15:27:00.000000 robotframework-keepasslibrary-0.3.0/src/robotframework_keepasslibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2020-10-30 15:27:00.000000 robotframework-keepasslibrary-0.3.0/src/robotframework_keepasslibrary.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2020-10-30 15:27:00.000000 robotframework-keepasslibrary-0.3.0/src/robotframework_keepasslibrary.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-08-05 14:41:42.977516 robotframework-keepasslibrary-0.3.1/
+drwxrwxrwx   0        0        0        0 2022-08-05 14:41:42.789989 robotframework-keepasslibrary-0.3.1/.github/
+drwxrwxrwx   0        0        0        0 2022-08-05 14:41:42.805616 robotframework-keepasslibrary-0.3.1/.github/workflows/
+-rw-rw-rw-   0        0        0     2414 2022-08-05 14:27:24.000000 robotframework-keepasslibrary-0.3.1/.github/workflows/python-package.yml
+-rw-rw-rw-   0        0        0     1444 2022-02-13 08:47:38.000000 robotframework-keepasslibrary-0.3.1/.gitignore
+-rw-rw-rw-   0        0        0     1090 2022-02-13 08:47:38.000000 robotframework-keepasslibrary-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0       15 2022-02-13 08:47:38.000000 robotframework-keepasslibrary-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3810 2022-08-05 14:41:42.977516 robotframework-keepasslibrary-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2022-08-05 14:27:24.000000 robotframework-keepasslibrary-0.3.1/Pipfile
+-rw-rw-rw-   0        0        0     2590 2022-08-05 14:30:59.000000 robotframework-keepasslibrary-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2022-08-05 14:41:42.836867 robotframework-keepasslibrary-0.3.1/atests/
+-rw-rw-rw-   0        0        0     1266 2022-08-05 14:27:24.000000 robotframework-keepasslibrary-0.3.1/atests/Composite Master Key.robot
+drwxrwxrwx   0        0        0        0 2022-08-05 14:41:42.899369 robotframework-keepasslibrary-0.3.1/atests/Data/
+-rw-rw-rw-   0        0        0     3406 2022-02-13 08:47:58.000000 robotframework-keepasslibrary-0.3.1/atests/Data/test3.kdbx
+-rw-rw-rw-   0        0        0      187 2022-02-13 08:47:58.000000 robotframework-keepasslibrary-0.3.1/atests/Data/test3.key
+-rw-rw-rw-   0        0        0     3737 2022-02-13 08:47:58.000000 robotframework-keepasslibrary-0.3.1/atests/Data/test4.kdbx
+-rw-rw-rw-   0        0        0      128 2022-02-13 08:47:58.000000 robotframework-keepasslibrary-0.3.1/atests/Data/test4.key
+-rw-rw-rw-   0        0        0     1989 2022-02-13 08:47:58.000000 robotframework-keepasslibrary-0.3.1/atests/Data/test4_aes.kdbx
+-rw-rw-rw-   0        0        0     1982 2022-02-13 08:47:58.000000 robotframework-keepasslibrary-0.3.1/atests/Data/test4_chacha20.kdbx
+-rw-rw-rw-   0        0        0     2341 2022-02-13 08:47:58.000000 robotframework-keepasslibrary-0.3.1/atests/Data/test4_hex.kdbx
+-rw-rw-rw-   0        0        0       64 2022-02-13 08:47:58.000000 robotframework-keepasslibrary-0.3.1/atests/Data/test4_hex.key
+-rw-rw-rw-   0        0        0     3616 2022-02-13 08:47:58.000000 robotframework-keepasslibrary-0.3.1/atests/Data/test4_only_keyfile.kdbx
+-rw-rw-rw-   0        0        0     3623 2022-02-13 08:47:58.000000 robotframework-keepasslibrary-0.3.1/atests/Data/test4_only_password.kdbx
+-rw-rw-rw-   0        0        0     1989 2022-02-13 08:47:58.000000 robotframework-keepasslibrary-0.3.1/atests/Data/test4_twofish.kdbx
+-rw-rw-rw-   0        0        0     6807 2022-08-05 14:27:24.000000 robotframework-keepasslibrary-0.3.1/atests/Entries.robot
+-rw-rw-rw-   0        0        0    10960 2022-08-05 14:27:24.000000 robotframework-keepasslibrary-0.3.1/atests/Entry.robot
+-rw-rw-rw-   0        0        0     7106 2022-08-05 14:27:24.000000 robotframework-keepasslibrary-0.3.1/atests/Group.robot
+-rw-rw-rw-   0        0        0     3137 2022-08-05 14:27:24.000000 robotframework-keepasslibrary-0.3.1/atests/Groups.robot
+-rw-rw-rw-   0        0        0     2699 2022-08-05 14:27:24.000000 robotframework-keepasslibrary-0.3.1/atests/KDBX v3.robot
+-rw-rw-rw-   0        0        0     3491 2022-08-05 14:27:24.000000 robotframework-keepasslibrary-0.3.1/atests/KDBX v4.robot
+-rw-rw-rw-   0        0        0      104 2022-02-13 08:47:58.000000 robotframework-keepasslibrary-0.3.1/atests/__init__.robot
+drwxrwxrwx   0        0        0        0 2022-08-05 14:41:42.915003 robotframework-keepasslibrary-0.3.1/docs/
+-rw-rw-rw-   0        0        0     1940 2022-02-13 08:47:58.000000 robotframework-keepasslibrary-0.3.1/docs/KeePassLibrary-0.3.0.rst
+-rw-rw-rw-   0        0        0      231 2022-08-05 14:32:52.000000 robotframework-keepasslibrary-0.3.1/docs/KeePassLibrary-0.3.1.rst
+-rw-rw-rw-   0        0        0   184224 2022-08-05 14:27:24.000000 robotframework-keepasslibrary-0.3.1/docs/KeePassLibrary.html
+-rw-rw-rw-   0        0        0       28 2022-02-13 08:47:38.000000 robotframework-keepasslibrary-0.3.1/docs/_config.yml
+-rw-rw-rw-   0        0        0       76 2022-08-05 14:27:24.000000 robotframework-keepasslibrary-0.3.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2022-08-05 14:41:42.977516 robotframework-keepasslibrary-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     2194 2022-08-05 14:27:24.000000 robotframework-keepasslibrary-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2022-08-05 14:41:42.789989 robotframework-keepasslibrary-0.3.1/src/
+drwxrwxrwx   0        0        0        0 2022-08-05 14:41:42.930619 robotframework-keepasslibrary-0.3.1/src/KeePassLibrary/
+-rw-rw-rw-   0        0        0     3728 2022-08-05 14:31:52.000000 robotframework-keepasslibrary-0.3.1/src/KeePassLibrary/__init__.py
+drwxrwxrwx   0        0        0        0 2022-08-05 14:41:42.930619 robotframework-keepasslibrary-0.3.1/src/KeePassLibrary/base/
+-rw-rw-rw-   0        0        0      256 2022-02-13 08:47:58.000000 robotframework-keepasslibrary-0.3.1/src/KeePassLibrary/base/__init__.py
+-rw-rw-rw-   0        0        0      484 2022-02-13 08:47:58.000000 robotframework-keepasslibrary-0.3.1/src/KeePassLibrary/base/context.py
+-rw-rw-rw-   0        0        0     1023 2022-02-13 08:47:58.000000 robotframework-keepasslibrary-0.3.1/src/KeePassLibrary/base/librarycomponent.py
+-rw-rw-rw-   0        0        0      444 2022-08-05 14:27:24.000000 robotframework-keepasslibrary-0.3.1/src/KeePassLibrary/errors.py
+drwxrwxrwx   0        0        0        0 2022-08-05 14:41:42.946246 robotframework-keepasslibrary-0.3.1/src/KeePassLibrary/keywords/
+-rw-rw-rw-   0        0        0      213 2022-02-13 08:47:58.000000 robotframework-keepasslibrary-0.3.1/src/KeePassLibrary/keywords/__init__.py
+-rw-rw-rw-   0        0        0     6258 2022-08-05 14:27:24.000000 robotframework-keepasslibrary-0.3.1/src/KeePassLibrary/keywords/keepassdatabase.py
+-rw-rw-rw-   0        0        0    12239 2022-08-05 14:27:24.000000 robotframework-keepasslibrary-0.3.1/src/KeePassLibrary/keywords/keepassentries.py
+-rw-rw-rw-   0        0        0    22793 2022-02-13 08:47:58.000000 robotframework-keepasslibrary-0.3.1/src/KeePassLibrary/keywords/keepassentry.py
+-rw-rw-rw-   0        0        0    13553 2022-02-13 08:47:58.000000 robotframework-keepasslibrary-0.3.1/src/KeePassLibrary/keywords/keepassgroup.py
+-rw-rw-rw-   0        0        0     7264 2022-08-05 14:27:24.000000 robotframework-keepasslibrary-0.3.1/src/KeePassLibrary/keywords/keepassgroups.py
+drwxrwxrwx   0        0        0        0 2022-08-05 14:41:42.977516 robotframework-keepasslibrary-0.3.1/src/robotframework_keepasslibrary.egg-info/
+-rw-rw-rw-   0        0        0     3810 2022-08-05 14:41:42.000000 robotframework-keepasslibrary-0.3.1/src/robotframework_keepasslibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1421 2022-08-05 14:41:42.000000 robotframework-keepasslibrary-0.3.1/src/robotframework_keepasslibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-08-05 14:41:42.000000 robotframework-keepasslibrary-0.3.1/src/robotframework_keepasslibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2022-08-05 14:41:42.000000 robotframework-keepasslibrary-0.3.1/src/robotframework_keepasslibrary.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2022-08-05 14:41:42.000000 robotframework-keepasslibrary-0.3.1/src/robotframework_keepasslibrary.egg-info/top_level.txt
```

### Comparing `robotframework-keepasslibrary-0.3.0/PKG-INFO` & `robotframework-keepasslibrary-0.3.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,91 @@
 Metadata-Version: 2.1
 Name: robotframework-keepasslibrary
-Version: 0.3.0
+Version: 0.3.1
 Summary: Robot Framework library for working with KeePass Database
 Home-page: https://github.com/loomanw/robotframework-keepasslibrary
 Author: William Looman
 Author-email: wlooman@gmail.com
 License: UNKNOWN
-Description: 
-        # KeePass Library
-        
-        This library enables Robot Framework to interact with KeePass databases.
-        
-        [![Build Status](https://travis-ci.org/loomanw/robotframework-keepasslibrary.svg?branch=master)](https://travis-ci.org/loomanw/robotframework-keepasslibrary)
-        [![Version](https://img.shields.io/pypi/v/robotframework-keepasslibrary.svg?label=version)](https://github.com/loomanw/robotframework-keepasslibrary) 
-        ![PyPI - License](https://img.shields.io/pypi/l/robotframework-keepasslibrary) 
-        ![PyPI - Downloads](https://img.shields.io/pypi/dm/robotframework-keepasslibrary) 
-        [![Updates](https://pyup.io/repos/github/loomanw/robotframework-keepasslibrary/shield.svg)](https://pyup.io/repos/github/loomanw/robotframework-keepasslibrary)
-        
-        Supported KeePass versions:
-        - KDBX3
-        - KDBX4
-            
-        KeepassLibrary uses the [PyKeePass](https://pypi.org/project/pykeepass/) modules internally to access KeePass databases
-            
-        See https://keepass.info for more information about KeePass in general
-        
-        ---
-        ### Versions:
-         - `0.3.0` New keywords for accessing entry and group data, rebuild of code using [Python Library Core](https://github.com/robotframework/PythonLibCore).
-         - `0.2.5` Fix manifest, additional test cases
-         - `0.2.4` Update dependencies
-         - `0.2.3` Update dependencies, new travis builds
-         - `0.2.2` Update dependencies
-         - `0.2.1` KDBX v3 and v4 test cases
-         - `0.2.0` Group Support
-         - `0.1.0` Entry Support
-        ---
-        
-        ### Installation
-        The recommended approach to install KeePassLibrary, regardless the version, is using  [pip](http://pip-installer.org/).
-        
-        Install (or upgrade) the latest KeePassLibrary version:
-        
-            pip install --upgrade robotframework-keepasslibrary
-        
-        ---
-        ### Example
-        
-        ```robotframework
-        *** Settings ***
-        Documentation     A test suite with a single test for retrieving a password.
-        ...
-        ...               The test loads a KeePass database named Database.kdbx using 
-        ...               the keyfile Database.key. 
-        ...               It then retrieves the first entry that matches the Username "User Name"
-        ...               and logs the password from the returned KeePass database entry
-        Library           KeePassLibrary
-        
-        *** Test Cases ***
-        Get KeePass Database Entry
-            Load KeePass Database       Database.kdbx    keyfile=Database.key        
-            ${entry}=    Get Entries By Username    User Name    first=True
-            ${value}=    Get Entry Password    ${entry}  
-            Log     Password for User Name is ${value}
-        ```
-        
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License  
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Security :: Cryptography  
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Framework :: Robot Framework
 Classifier: Framework :: Robot Framework :: Library
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# KeePass Library
+
+This library enables Robot Framework to interact with KeePass databases.
+
+[![Python package](https://github.com/loomanw/robotframework-keepasslibrary/actions/workflows/python-package.yml/badge.svg)](https://github.com/loomanw/robotframework-keepasslibrary/actions/workflows/python-package.yml) 
+[![Version](https://img.shields.io/pypi/v/robotframework-keepasslibrary.svg?label=version)](https://github.com/loomanw/robotframework-keepasslibrary) 
+![PyPI - License](https://img.shields.io/pypi/l/robotframework-keepasslibrary) 
+![PyPI - Downloads](https://img.shields.io/pypi/dm/robotframework-keepasslibrary) 
+[![Updates](https://pyup.io/repos/github/loomanw/robotframework-keepasslibrary/shield.svg)](https://pyup.io/repos/github/loomanw/robotframework-keepasslibrary)
+
+Supported KeePass versions:
+- KDBX3
+- KDBX4
+    
+KeepassLibrary uses the [PyKeePass](https://pypi.org/project/pykeepass/) modules internally to access KeePass databases
+    
+See https://keepass.info for more information about KeePass in general
+
+---
+### Versions:
+ - `0.3.1` Update dependencies, tests moved to github actions 
+ - `0.3.0` New keywords for accessing entry and group data, rebuild of code using [Python Library Core](https://github.com/robotframework/PythonLibCore).
+ - `0.2.5` Fix manifest, additional test cases
+ - `0.2.4` Update dependencies
+ - `0.2.3` Update dependencies, new travis builds
+ - `0.2.2` Update dependencies
+ - `0.2.1` KDBX v3 and v4 test cases
+ - `0.2.0` Group Support
+ - `0.1.0` Entry Support
+---
+
+### Installation
+The recommended approach to install KeePassLibrary, regardless the version, is using  [pip](http://pip-installer.org/).
+
+Install (or upgrade) the latest KeePassLibrary version:
+
+    pip install --upgrade robotframework-keepasslibrary
+
+---
+### Example
+
+```robotframework
+*** Settings ***
+Documentation     A test suite with a single test for retrieving a password.
+...
+...               The test opens a KeePass database named Database.kdbx using 
+...               the keyfile Database.key. 
+...               It then retrieves the first entry that matches the Username "User Name"
+...               and logs the password from the returned KeePass database entry
+Library           KeePassLibrary
+
+*** Test Cases ***
+Get KeePass Database Entry
+    Open KeePass Database       Database.kdbx    keyfile=Database.key        
+    ${entry}=    Get Entries By Username    User Name    first=True
+    ${value}=    Get Entry Password    ${entry}  
+    Log     Password for User Name is ${value}
+```
+
+
+
```

### Comparing `robotframework-keepasslibrary-0.3.0/README.md` & `robotframework-keepasslibrary-0.3.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 # KeePass Library
 
 This library enables Robot Framework to interact with KeePass databases.
 
-[![Build Status](https://travis-ci.org/loomanw/robotframework-keepasslibrary.svg?branch=master)](https://travis-ci.org/loomanw/robotframework-keepasslibrary)
+[![Python package](https://github.com/loomanw/robotframework-keepasslibrary/actions/workflows/python-package.yml/badge.svg)](https://github.com/loomanw/robotframework-keepasslibrary/actions/workflows/python-package.yml) 
 [![Version](https://img.shields.io/pypi/v/robotframework-keepasslibrary.svg?label=version)](https://github.com/loomanw/robotframework-keepasslibrary) 
 ![PyPI - License](https://img.shields.io/pypi/l/robotframework-keepasslibrary) 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/robotframework-keepasslibrary) 
 [![Updates](https://pyup.io/repos/github/loomanw/robotframework-keepasslibrary/shield.svg)](https://pyup.io/repos/github/loomanw/robotframework-keepasslibrary)
 
 Supported KeePass versions:
 - KDBX3
@@ -15,14 +15,15 @@
     
 KeepassLibrary uses the [PyKeePass](https://pypi.org/project/pykeepass/) modules internally to access KeePass databases
     
 See https://keepass.info for more information about KeePass in general
 
 ---
 ### Versions:
+ - `0.3.1` Update dependencies, tests moved to github actions 
  - `0.3.0` New keywords for accessing entry and group data, rebuild of code using [Python Library Core](https://github.com/robotframework/PythonLibCore).
  - `0.2.5` Fix manifest, additional test cases
  - `0.2.4` Update dependencies
  - `0.2.3` Update dependencies, new travis builds
  - `0.2.2` Update dependencies
  - `0.2.1` KDBX v3 and v4 test cases
  - `0.2.0` Group Support
@@ -39,21 +40,21 @@
 ---
 ### Example
 
 ```robotframework
 *** Settings ***
 Documentation     A test suite with a single test for retrieving a password.
 ...
-...               The test loads a KeePass database named Database.kdbx using 
+...               The test opens a KeePass database named Database.kdbx using 
 ...               the keyfile Database.key. 
 ...               It then retrieves the first entry that matches the Username "User Name"
 ...               and logs the password from the returned KeePass database entry
 Library           KeePassLibrary
 
 *** Test Cases ***
 Get KeePass Database Entry
-    Load KeePass Database       Database.kdbx    keyfile=Database.key        
+    Open KeePass Database       Database.kdbx    keyfile=Database.key        
     ${entry}=    Get Entries By Username    User Name    first=True
     ${value}=    Get Entry Password    ${entry}  
     Log     Password for User Name is ${value}
 ```
```

### Comparing `robotframework-keepasslibrary-0.3.0/setup.py` & `robotframework-keepasslibrary-0.3.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 License :: OSI Approved :: MIT License  
 Operating System :: OS Independent
 Programming Language :: Python
 Programming Language :: Python :: 3
 Programming Language :: Python :: 3.6
 Programming Language :: Python :: 3.7
 Programming Language :: Python :: 3.8
+Programming Language :: Python :: 3.9
+Programming Language :: Python :: 3.10
 Programming Language :: Python :: 3 :: Only
 Topic :: Security :: Cryptography  
 Topic :: Software Development :: Quality Assurance
 Topic :: Software Development :: Testing
 Framework :: Robot Framework
 Framework :: Robot Framework :: Library
 '''.strip().splitlines()
```

### Comparing `robotframework-keepasslibrary-0.3.0/src/KeePassLibrary/__init__.py` & `robotframework-keepasslibrary-0.3.1/src/KeePassLibrary/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     KeePassDatabase,
     KeePassEntry,
     KeePassEntries,
     KeePassGroup,
     KeePassGroups
 )
 
-__version__ = '0.3.0'
+__version__ = '0.3.1'
 
 class KeePassLibrary(DynamicCore):
     """KeePassLibrary is a library for Robot Framework.
     
     KeePassLibrary uses the PyKeePass modules internally to access KeePass databases
     
     See https://keepass.info for more information about KeePass in general.
```

### Comparing `robotframework-keepasslibrary-0.3.0/src/KeePassLibrary/base/librarycomponent.py` & `robotframework-keepasslibrary-0.3.1/src/KeePassLibrary/base/librarycomponent.py`

 * *Files identical despite different names*

### Comparing `robotframework-keepasslibrary-0.3.0/src/KeePassLibrary/keywords/keepassdatabase.py` & `robotframework-keepasslibrary-0.3.1/src/KeePassLibrary/keywords/keepassdatabase.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Library components."""
 from KeePassLibrary.base import PyKeePass, keyword, LibraryComponent
-from KeePassLibrary.errors import DatabaseNotLoaded
+from KeePassLibrary.errors import DatabaseNotOpened
 
 class KeePassDatabase(LibraryComponent):
     
     @keyword 
     def load_database(self, filename, password=None, keyfile=None,
              transformed_key=None):
         """*DEPRECATED in KeePassLibrary 0.3.0*, Use `Open Keepass Database` instead.
@@ -52,117 +52,117 @@
                            transformed_key)
 
     @keyword 
     def close_database(self):
         """*DEPRECATED in KeePassLibrary 0.3.0*, Use `Close Keepass Database` instead.
         """
         if self.database is None:
-            raise DatabaseNotLoaded('No KeePass Database loaded.')
+            raise DatabaseNotOpened('No KeePass Database Opened.')
         else:
             self.database = None  
     
     @keyword    
     def close_keepass_database(self):
         """Closes the currently open KeePass database.
         """
         if self.database is None:
-            raise DatabaseNotLoaded('No KeePass Database loaded.')
+            raise DatabaseNotOpened('No KeePass Database Opened.')
         else:
             self.database = None
 
 
     
     @keyword 
     def save(self, filename=None, transformed_key=None):
         """*DEPRECATED in KeePassLibrary 0.3.0*, Use `Save Keepass Database` instead.
         """
         if self.database is None:
-            raise DatabaseNotLoaded('No KeePass Database loaded.')
+            raise DatabaseNotOpened('No KeePass Database Opened.')
         else:
             self.database.save(filename, transformed_key)        
 
     @keyword 
     def save_keepass_database(self, filename=None, transformed_key=None):
         """Save the content of the currently open KeePass database.
 
         | =Parameter=        | =Description=                              |
         | ``filename``       | specifies the path of the KeePass database |
         | ``tranformed_key`` | specifies the location of the keyfile      |
         """
         if self.database is None:
-            raise DatabaseNotLoaded('No KeePass Database loaded.')
+            raise DatabaseNotOpened('No KeePass Database Opened.')
         else:
             self.database.save(filename, transformed_key)        
 
     @keyword 
     def dump_xml(self, outfile):
         """Dump the content of the database to a xml file.
            NOTE: The resulting file is unencrypted!
 
         | =Parameter= | =Description=                        |
         | ``outfile`` | specifies the path of the dumped xml |
         """
         if self.database is None:
-            raise DatabaseNotLoaded('No KeePass Database loaded.')
+            raise DatabaseNotOpened('No KeePass Database Opened.')
         else:
             self.database.dump_xml(outfile)
     
     @keyword 
     def get_version(self):
-        """Returns the version of the KeePass database loaded with `Load Database`
+        """Returns the version of the KeePass database loaded with `Open Keepass Database`
         | =Return=   | =Description= |
         | ``(3, 1)`` | KDBX v3       |
         | ``(4, 0)`` | KDBX v4       |
         """
         if self.database is None:
-            raise DatabaseNotLoaded('No KeePass Database loaded.')
+            raise DatabaseNotOpened('No KeePass Database Opened.')
         else:
             return self.database.version
     
     # TODO: Add more documentation
     @keyword 
     def get_encryption_algorithm(self):
         """Returns the encryption algorithm used. 
         """
         if self.database is None:
-            raise DatabaseNotLoaded('No KeePass Database loaded.')
+            raise DatabaseNotOpened('No KeePass Database Opened.')
         else:
             return self.database.encryption_algorithm
     
     # TODO: Add more documentation
     @keyword 
     def get_kdf_algorithm(self):
         """Returns the key transformation algorithm used. 
         """
         if self.database is None:
-            raise DatabaseNotLoaded('No KeePass Database loaded.')
+            raise DatabaseNotOpened('No KeePass Database Opened.')
         else:
             return self.database.kdf_algorithm
     
     # TODO: Add more documentation
     @keyword 
     def get_transformed_key(self):
         """Returns the transformed key.
         """
         if self.database is None:
-            raise DatabaseNotLoaded('No KeePass Database loaded.')
+            raise DatabaseNotOpened('No KeePass Database Opened.')
         else:
             return self.database.transformed_key
 
     @keyword 
     def get_tree(self):
         """Returns the full xml tree.
         """
         if self.database is None:
-            raise DatabaseNotLoaded('No KeePass Database loaded.')
+            raise DatabaseNotOpened('No KeePass Database Opened.')
         else:
             return self.database.tree
 
     # TODO: Add more documentation
     @keyword 
     def get_root_group(self):
         """Returns the root group.
         """
         if self.database is None:
-            raise DatabaseNotLoaded('No KeePass Database loaded.')
+            raise DatabaseNotOpened('No KeePass Database Opened.')
         else:
             return self.database.root_group
```

### Comparing `robotframework-keepasslibrary-0.3.0/src/KeePassLibrary/keywords/keepassentries.py` & `robotframework-keepasslibrary-0.3.1/src/KeePassLibrary/keywords/keepassentries.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Library components."""
 from KeePassLibrary.base import keyword, LibraryComponent, UUID
-from KeePassLibrary.errors import DatabaseNotLoaded
+from KeePassLibrary.errors import DatabaseNotOpened
 from robot.utils import is_truthy
 
 class KeePassEntries(LibraryComponent):
     
     # FIXME: Catch uuid string and convert to class     
     @keyword
     def get_entries(self, history=False, first=False, recursive=True,
@@ -34,15 +34,15 @@
            | @{entries}= | `Get Entries` | title=.*entry | username=.*user     | regex=True |
            | @{entries}= | `Get Entries` | title=.*entry | notes=.*entry notes | regex=True |
            
            | ${group}=   | Get Groups By Name      | subgroup | first=True |   
            | ${entries}= | Get Entries By Username | foobar   | group=${group} | first=True |     
         """
         if self.database is None:
-            raise DatabaseNotLoaded('No KeePass Database loaded.')
+            raise DatabaseNotOpened('No KeePass Database Opened.')
         else:
             if 'regex' in kwargs:
                 kwargs['regex'] = is_truthy(kwargs['regex']) 
             return self.database.find_entries(recursive=recursive,
                                               path=path, 
                                               group=group,
                                               history=history, 
@@ -55,15 +55,15 @@
            
            See the `Entries and Groups` section for more information about Entries and Groups.\n 
            
            Example:
            | ${entries} = | `Get Entries All` | 
         """
         if self.database is None:
-            raise DatabaseNotLoaded('No KeePass Database loaded.')
+            raise DatabaseNotOpened('No KeePass Database Opened.')
         else:
             return self.database.find_entries_by_title('.*', 
                                                        regex=True)
     
     @keyword
     def get_entries_by_title(self, title, regex=False, flags=None,
                               group=None, history=False, first=False):
@@ -75,15 +75,15 @@
            | @{entries} = | `Get Entries By Title` | root_entry |
            => all entries with title: root_entry
         
            | ${entry} =   | `Get Entries By Title` | root_entry | first=True |
            => first entry with title: root_entry
         """        
         if self.database is None:
-            raise DatabaseNotLoaded('No KeePass Database loaded.')
+            raise DatabaseNotOpened('No KeePass Database Opened.')
         else:
             return self.database.find_entries_by_title(title, 
                                                        regex,
                                                        flags, 
                                                        group, 
                                                        history, 
                                                        first)
@@ -95,15 +95,15 @@
            
            See `Get Entries` for more details about optional arguments.
 
            Example:
            | @{entries} = | `Get Entries By Username` | foobar_user |
         """  
         if self.database is None:
-            raise DatabaseNotLoaded('No KeePass Database loaded.')
+            raise DatabaseNotOpened('No KeePass Database Opened.')
         else:
             return self.database.find_entries_by_username(username, 
                                                           regex, 
                                                           flags, 
                                                           group, 
                                                           history, 
                                                           first)
@@ -115,15 +115,15 @@
         
            See `Get Entries` for more details about optional arguments.
            
            Example:
            | @{entries} = | `Get Entries By Password` | passw0rd |
         """  
         if self.database is None:
-            raise DatabaseNotLoaded('No KeePass Database loaded.')
+            raise DatabaseNotOpened('No KeePass Database Opened.')
         else:
             return self.database.find_entries_by_password(password, 
                                                           regex, 
                                                           flags, 
                                                           group, 
                                                           history, 
                                                           first)
@@ -135,15 +135,15 @@
         
            See `Get Entries` for more details about optional arguments.
            
            Example:
            | @{entries} = | `Get Entries By Url` | http://example.com |
         """  
         if self.database is None:
-            raise DatabaseNotLoaded('No KeePass Database loaded.')
+            raise DatabaseNotOpened('No KeePass Database Opened.')
         else:
             return self.database.find_entries_by_url(url, 
                                                      regex, 
                                                      flags, 
                                                      group, 
                                                      history, 
                                                      first)
@@ -155,15 +155,15 @@
         
            See `Get Entries` for more details about optional arguments.
            
            Example:
            | @{entries} = | `Get Entries By Notes` | root entry notes |
         """  
         if self.database is None:
-            raise DatabaseNotLoaded('No KeePass Database loaded.')
+            raise DatabaseNotOpened('No KeePass Database Opened.')
         else:
             return self.database.find_entries_by_notes(notes,
                                          regex,
                                          flags,
                                          group,
                                          history,
                                          first)
@@ -178,15 +178,15 @@
            
            Note, only 1 entry can be selected by path
              
            Example:
            | ${entry} = | Get Entries By Path | foobar_group/group_entry |
         """  
         if self.database is None:
-            raise DatabaseNotLoaded('No KeePass Database loaded.')
+            raise DatabaseNotOpened('No KeePass Database Opened.')
         else:
             return self.database.find_entries_by_path(path,
                                          regex,
                                          flags,
                                          group,
                                          history,
                                          first)
@@ -198,15 +198,15 @@
 
            See `Get Entries` for more details about optional arguments.
 
            Example:
            | ${entries} = | Get Entries By Uuid | 12345678-1234-5678-1234-567812345678 |
         """  
         if self.database is None:
-            raise DatabaseNotLoaded('No KeePass Database loaded.')
+            raise DatabaseNotOpened('No KeePass Database Opened.')
         else:
             uuid = UUID('urn:uuid:'+ uuid)
             return self.database.find_entries_by_uuid(uuid,
                                          regex,
                                          flags,
                                          group,
                                          history,
@@ -230,15 +230,15 @@
            | URL |
            | Notes |
            | IconID |
            | Tags |
            | History |
         """  
         if self.database is None:
-            raise DatabaseNotLoaded('No KeePass Database loaded.')
+            raise DatabaseNotOpened('No KeePass Database Opened.')
         else:
             return self.database.find_entries_by_string(string,
                                          regex,
                                          flags,
                                          group,
                                          history,
                                          first)
```

### Comparing `robotframework-keepasslibrary-0.3.0/src/KeePassLibrary/keywords/keepassentry.py` & `robotframework-keepasslibrary-0.3.1/src/KeePassLibrary/keywords/keepassentry.py`

 * *Files identical despite different names*

### Comparing `robotframework-keepasslibrary-0.3.0/src/KeePassLibrary/keywords/keepassgroup.py` & `robotframework-keepasslibrary-0.3.1/src/KeePassLibrary/keywords/keepassgroup.py`

 * *Files identical despite different names*

### Comparing `robotframework-keepasslibrary-0.3.0/src/KeePassLibrary/keywords/keepassgroups.py` & `robotframework-keepasslibrary-0.3.1/src/KeePassLibrary/keywords/keepassgroups.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Library components."""
 from KeePassLibrary.base import keyword, LibraryComponent, UUID
-from KeePassLibrary.errors import DatabaseNotLoaded
+from KeePassLibrary.errors import DatabaseNotOpened
 from robot.utils import is_truthy
 
 class KeePassGroups(LibraryComponent):
     
     # FIXME: Catch uuid string and convert to class
     @keyword
     def get_groups(self, recursive=True, path=None, group=None, **kwargs):
@@ -28,15 +28,15 @@
            | @{groups}= | `Get Groups` | name=.*group | notes=^.{0}$ | regex=True |
            | ${groups}= | `Get Groups` | name=.*group | notes=^.{0}$ | regex=True | first=True |
 
            | ${group}=   | `Get Groups By Name` | subgroup  | first=True     |   
            | @{groups}= |  `Get Groups`         | subgroup2 | group=${group} |             
         """ 
         if self.database is None:
-            raise DatabaseNotLoaded('No KeePass Database loaded.')
+            raise DatabaseNotOpened('No KeePass Database Opened.')
         else:
             if 'regex' in kwargs:
                 kwargs['regex'] = is_truthy(kwargs['regex'])
             if 'first' in kwargs:
                 kwargs['first'] = is_truthy(kwargs['first'])    
             return self.database.find_groups(recursive, path, group, **kwargs)
     
@@ -46,15 +46,15 @@
         
            See the `Entries and Groups` section for more information about Entries and Groups.\n  
         
            Example:
            | ${groups} = | Get Groups All | 
         """ 
         if self.database is None:
-            raise DatabaseNotLoaded('No KeePass Database loaded.')
+            raise DatabaseNotOpened('No KeePass Database Opened.')
         else:
             return self.database.find_groups_by_name('.*', 
                                                      regex=True)
         
     @keyword
     def get_groups_by_name(self, group_name, regex=False, flags=None,
                             group=None, first=False):
@@ -64,15 +64,15 @@
            See `Get Groups` for more details about optional arguments.
            
            Examples:
            | ${groups} = | Get Groups By Name | subgroup |
            | ${groups} = | Get Groups By Name | .* | regex=True |
         """  
         if self.database is None:
-            raise DatabaseNotLoaded('No KeePass Database loaded.')
+            raise DatabaseNotOpened('No KeePass Database Opened.')
         else:
             return self.database.find_groups_by_name(group_name=group_name,
                                                      regex=regex,
                                                      flags=flags,
                                                      group=group,
                                                      first=first)
     
@@ -84,15 +84,15 @@
            
            See `Get Groups` for more details about optional arguments.
            
            Example:
            | ${groups} = | Get Groups By Path | foobar_group/subgroup |
         """  
         if self.database is None:
-            raise DatabaseNotLoaded('No KeePass Database loaded.')
+            raise DatabaseNotOpened('No KeePass Database Opened.')
         else:
             return self.database.find_groups_by_path(group_path_str=group_path_str,
                                                      regex=regex,
                                                      flags=flags,
                                                      group=group,
                                                      first=first)
  
@@ -104,15 +104,15 @@
            
            See `Get Groups` for more details about optional arguments.
            
            Example:
            | ${groups} = | Get Groups By Uuid | 12345678-1234-5678-1234-567812345678 |
         """ 
         if self.database is None:
-            raise DatabaseNotLoaded('No KeePass Database loaded.')
+            raise DatabaseNotOpened('No KeePass Database Opened.')
         else:
             uuid = UUID('urn:uuid:'+ uuid)
             return self.database.find_groups_by_uuid(uuid=uuid,
                                                      regex=regex,
                                                      flags=flags,
                                                      group=group,
                                                      history=history,
@@ -126,15 +126,15 @@
     
            See `Get Groups` for more details about optional arguments.
     
            Example:
            | ${groups} = | Get Groups By Notes | group notes |
         """ 
         if self.database is None:
-            raise DatabaseNotLoaded('No KeePass Database loaded.')
+            raise DatabaseNotOpened('No KeePass Database Opened.')
         else:
             return self.database.find_groups_by_notes(notes=notes,
                                                       regex=regex,
                                                       flags=flags,
                                                       group=group,
                                                       history=history,
                                                       first=first)
```

### Comparing `robotframework-keepasslibrary-0.3.0/src/robotframework_keepasslibrary.egg-info/PKG-INFO` & `robotframework-keepasslibrary-0.3.1/src/robotframework_keepasslibrary.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,91 @@
 Metadata-Version: 2.1
 Name: robotframework-keepasslibrary
-Version: 0.3.0
+Version: 0.3.1
 Summary: Robot Framework library for working with KeePass Database
 Home-page: https://github.com/loomanw/robotframework-keepasslibrary
 Author: William Looman
 Author-email: wlooman@gmail.com
 License: UNKNOWN
-Description: 
-        # KeePass Library
-        
-        This library enables Robot Framework to interact with KeePass databases.
-        
-        [![Build Status](https://travis-ci.org/loomanw/robotframework-keepasslibrary.svg?branch=master)](https://travis-ci.org/loomanw/robotframework-keepasslibrary)
-        [![Version](https://img.shields.io/pypi/v/robotframework-keepasslibrary.svg?label=version)](https://github.com/loomanw/robotframework-keepasslibrary) 
-        ![PyPI - License](https://img.shields.io/pypi/l/robotframework-keepasslibrary) 
-        ![PyPI - Downloads](https://img.shields.io/pypi/dm/robotframework-keepasslibrary) 
-        [![Updates](https://pyup.io/repos/github/loomanw/robotframework-keepasslibrary/shield.svg)](https://pyup.io/repos/github/loomanw/robotframework-keepasslibrary)
-        
-        Supported KeePass versions:
-        - KDBX3
-        - KDBX4
-            
-        KeepassLibrary uses the [PyKeePass](https://pypi.org/project/pykeepass/) modules internally to access KeePass databases
-            
-        See https://keepass.info for more information about KeePass in general
-        
-        ---
-        ### Versions:
-         - `0.3.0` New keywords for accessing entry and group data, rebuild of code using [Python Library Core](https://github.com/robotframework/PythonLibCore).
-         - `0.2.5` Fix manifest, additional test cases
-         - `0.2.4` Update dependencies
-         - `0.2.3` Update dependencies, new travis builds
-         - `0.2.2` Update dependencies
-         - `0.2.1` KDBX v3 and v4 test cases
-         - `0.2.0` Group Support
-         - `0.1.0` Entry Support
-        ---
-        
-        ### Installation
-        The recommended approach to install KeePassLibrary, regardless the version, is using  [pip](http://pip-installer.org/).
-        
-        Install (or upgrade) the latest KeePassLibrary version:
-        
-            pip install --upgrade robotframework-keepasslibrary
-        
-        ---
-        ### Example
-        
-        ```robotframework
-        *** Settings ***
-        Documentation     A test suite with a single test for retrieving a password.
-        ...
-        ...               The test loads a KeePass database named Database.kdbx using 
-        ...               the keyfile Database.key. 
-        ...               It then retrieves the first entry that matches the Username "User Name"
-        ...               and logs the password from the returned KeePass database entry
-        Library           KeePassLibrary
-        
-        *** Test Cases ***
-        Get KeePass Database Entry
-            Load KeePass Database       Database.kdbx    keyfile=Database.key        
-            ${entry}=    Get Entries By Username    User Name    first=True
-            ${value}=    Get Entry Password    ${entry}  
-            Log     Password for User Name is ${value}
-        ```
-        
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License  
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Security :: Cryptography  
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Framework :: Robot Framework
 Classifier: Framework :: Robot Framework :: Library
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# KeePass Library
+
+This library enables Robot Framework to interact with KeePass databases.
+
+[![Python package](https://github.com/loomanw/robotframework-keepasslibrary/actions/workflows/python-package.yml/badge.svg)](https://github.com/loomanw/robotframework-keepasslibrary/actions/workflows/python-package.yml) 
+[![Version](https://img.shields.io/pypi/v/robotframework-keepasslibrary.svg?label=version)](https://github.com/loomanw/robotframework-keepasslibrary) 
+![PyPI - License](https://img.shields.io/pypi/l/robotframework-keepasslibrary) 
+![PyPI - Downloads](https://img.shields.io/pypi/dm/robotframework-keepasslibrary) 
+[![Updates](https://pyup.io/repos/github/loomanw/robotframework-keepasslibrary/shield.svg)](https://pyup.io/repos/github/loomanw/robotframework-keepasslibrary)
+
+Supported KeePass versions:
+- KDBX3
+- KDBX4
+    
+KeepassLibrary uses the [PyKeePass](https://pypi.org/project/pykeepass/) modules internally to access KeePass databases
+    
+See https://keepass.info for more information about KeePass in general
+
+---
+### Versions:
+ - `0.3.1` Update dependencies, tests moved to github actions 
+ - `0.3.0` New keywords for accessing entry and group data, rebuild of code using [Python Library Core](https://github.com/robotframework/PythonLibCore).
+ - `0.2.5` Fix manifest, additional test cases
+ - `0.2.4` Update dependencies
+ - `0.2.3` Update dependencies, new travis builds
+ - `0.2.2` Update dependencies
+ - `0.2.1` KDBX v3 and v4 test cases
+ - `0.2.0` Group Support
+ - `0.1.0` Entry Support
+---
+
+### Installation
+The recommended approach to install KeePassLibrary, regardless the version, is using  [pip](http://pip-installer.org/).
+
+Install (or upgrade) the latest KeePassLibrary version:
+
+    pip install --upgrade robotframework-keepasslibrary
+
+---
+### Example
+
+```robotframework
+*** Settings ***
+Documentation     A test suite with a single test for retrieving a password.
+...
+...               The test opens a KeePass database named Database.kdbx using 
+...               the keyfile Database.key. 
+...               It then retrieves the first entry that matches the Username "User Name"
+...               and logs the password from the returned KeePass database entry
+Library           KeePassLibrary
+
+*** Test Cases ***
+Get KeePass Database Entry
+    Open KeePass Database       Database.kdbx    keyfile=Database.key        
+    ${entry}=    Get Entries By Username    User Name    first=True
+    ${value}=    Get Entry Password    ${entry}  
+    Log     Password for User Name is ${value}
+```
+
+
+
```

