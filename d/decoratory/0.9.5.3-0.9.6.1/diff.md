# Comparing `tmp/decoratory-0.9.5.3.tar.gz` & `tmp/decoratory-0.9.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoratory-0.9.5.3.tar", last modified: Mon Jul 17 13:54:14 2023, max compression
+gzip compressed data, was "decoratory-0.9.6.1.tar", last modified: Tue Jul 18 17:55:12 2023, max compression
```

## Comparing `decoratory-0.9.5.3.tar` & `decoratory-0.9.6.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 13:54:14.423078 decoratory-0.9.5.3/
--rw-rw-rw-   0        0        0     1257 2023-07-15 14:55:02.000000 decoratory-0.9.5.3/License.txt
--rw-rw-rw-   0        0        0    48576 2023-07-17 13:54:14.419076 decoratory-0.9.5.3/PKG-INFO
--rw-rw-rw-   0        0        0    46879 2023-07-17 13:53:35.000000 decoratory-0.9.5.3/Readme.rst
--rw-rw-rw-   0        0        0        0 2023-06-23 16:09:56.000000 decoratory-0.9.5.3/Requirements.txt
-drwxrwxrwx   0        0        0        0 2023-07-17 13:54:14.363360 decoratory-0.9.5.3/Sources/
-drwxrwxrwx   0        0        0        0 2023-07-17 13:54:14.392816 decoratory-0.9.5.3/Sources/decoratory/
--rw-rw-rw-   0        0        0      249 2023-07-04 05:40:20.000000 decoratory-0.9.5.3/Sources/decoratory/__init__.py
--rw-rw-rw-   0        0        0     7627 2023-07-17 13:53:35.000000 decoratory-0.9.5.3/Sources/decoratory/__main__.py
--rw-rw-rw-   0        0        0     5893 2023-07-17 13:43:02.000000 decoratory-0.9.5.3/Sources/decoratory/banner.py
--rw-rw-rw-   0        0        0    19694 2023-07-17 13:43:02.000000 decoratory-0.9.5.3/Sources/decoratory/basic.py
--rw-rw-rw-   0        0        0    12430 2023-07-17 13:43:02.000000 decoratory-0.9.5.3/Sources/decoratory/multiton.py
--rw-rw-rw-   0        0        0    36920 2023-07-17 13:43:02.000000 decoratory-0.9.5.3/Sources/decoratory/observer.py
--rw-rw-rw-   0        0        0     8011 2023-07-17 13:43:02.000000 decoratory-0.9.5.3/Sources/decoratory/singleton.py
--rw-rw-rw-   0        0        0    10871 2023-07-17 13:43:03.000000 decoratory-0.9.5.3/Sources/decoratory/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-07-17 13:54:14.400910 decoratory-0.9.5.3/Sources/decoratory.egg-info/
--rw-rw-rw-   0        0        0    48576 2023-07-17 13:54:14.000000 decoratory-0.9.5.3/Sources/decoratory.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      586 2023-07-17 13:54:14.000000 decoratory-0.9.5.3/Sources/decoratory.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 13:54:14.000000 decoratory-0.9.5.3/Sources/decoratory.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-17 13:54:14.000000 decoratory-0.9.5.3/Sources/decoratory.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-17 13:54:14.419076 decoratory-0.9.5.3/Unittest/
--rw-rw-rw-   0        0        0    29046 2023-07-17 13:43:03.000000 decoratory-0.9.5.3/Unittest/test_basic.py
--rw-rw-rw-   0        0        0    23872 2023-07-17 13:43:03.000000 decoratory-0.9.5.3/Unittest/test_multiton.py
--rw-rw-rw-   0        0        0    40121 2023-07-17 13:43:03.000000 decoratory-0.9.5.3/Unittest/test_observer.py
--rw-rw-rw-   0        0        0    10743 2023-07-17 13:43:03.000000 decoratory-0.9.5.3/Unittest/test_singleton.py
--rw-rw-rw-   0        0        0    10207 2023-07-17 13:43:03.000000 decoratory-0.9.5.3/Unittest/test_wrapper.py
--rw-rw-rw-   0        0        0       42 2023-07-17 13:54:14.423078 decoratory-0.9.5.3/setup.cfg
--rw-rw-rw-   0        0        0     4715 2023-07-17 13:53:35.000000 decoratory-0.9.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:55:12.706859 decoratory-0.9.6.1/
+-rw-rw-rw-   0        0        0     1262 2023-07-18 17:13:50.000000 decoratory-0.9.6.1/License.txt
+-rw-rw-rw-   0        0        0    48576 2023-07-18 17:55:12.705803 decoratory-0.9.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0    46879 2023-07-18 17:54:26.000000 decoratory-0.9.6.1/Readme.rst
+-rw-rw-rw-   0        0        0        0 2023-06-23 16:09:56.000000 decoratory-0.9.6.1/Requirements.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 17:55:11.821074 decoratory-0.9.6.1/Sources/
+drwxrwxrwx   0        0        0        0 2023-07-18 17:55:12.251697 decoratory-0.9.6.1/Sources/decoratory/
+-rw-rw-rw-   0        0        0      249 2023-07-04 05:40:20.000000 decoratory-0.9.6.1/Sources/decoratory/__init__.py
+-rw-rw-rw-   0        0        0     7627 2023-07-18 17:54:26.000000 decoratory-0.9.6.1/Sources/decoratory/__main__.py
+-rw-rw-rw-   0        0        0     5893 2023-07-18 17:54:26.000000 decoratory-0.9.6.1/Sources/decoratory/banner.py
+-rw-rw-rw-   0        0        0    19694 2023-07-18 17:54:26.000000 decoratory-0.9.6.1/Sources/decoratory/basic.py
+-rw-rw-rw-   0        0        0    12476 2023-07-18 17:54:26.000000 decoratory-0.9.6.1/Sources/decoratory/multiton.py
+-rw-rw-rw-   0        0        0    36921 2023-07-18 17:54:26.000000 decoratory-0.9.6.1/Sources/decoratory/observer.py
+-rw-rw-rw-   0        0        0     8187 2023-07-18 17:54:26.000000 decoratory-0.9.6.1/Sources/decoratory/singleton.py
+-rw-rw-rw-   0        0        0    10871 2023-07-18 17:54:26.000000 decoratory-0.9.6.1/Sources/decoratory/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:55:12.336816 decoratory-0.9.6.1/Sources/decoratory.egg-info/
+-rw-rw-rw-   0        0        0    48576 2023-07-18 17:55:11.000000 decoratory-0.9.6.1/Sources/decoratory.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      586 2023-07-18 17:55:11.000000 decoratory-0.9.6.1/Sources/decoratory.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 17:55:11.000000 decoratory-0.9.6.1/Sources/decoratory.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-18 17:55:11.000000 decoratory-0.9.6.1/Sources/decoratory.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 17:55:12.640119 decoratory-0.9.6.1/Unittest/
+-rw-rw-rw-   0        0        0    28998 2023-07-18 17:54:26.000000 decoratory-0.9.6.1/Unittest/test_basic.py
+-rw-rw-rw-   0        0        0    23872 2023-07-18 17:54:26.000000 decoratory-0.9.6.1/Unittest/test_multiton.py
+-rw-rw-rw-   0        0        0    40073 2023-07-18 17:54:26.000000 decoratory-0.9.6.1/Unittest/test_observer.py
+-rw-rw-rw-   0        0        0    10743 2023-07-18 17:54:27.000000 decoratory-0.9.6.1/Unittest/test_singleton.py
+-rw-rw-rw-   0        0        0    10207 2023-07-18 17:54:27.000000 decoratory-0.9.6.1/Unittest/test_wrapper.py
+-rw-rw-rw-   0        0        0       42 2023-07-18 17:55:12.707861 decoratory-0.9.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     4715 2023-07-18 17:54:27.000000 decoratory-0.9.6.1/setup.py
```

### Comparing `decoratory-0.9.5.3/License.txt` & `decoratory-0.9.6.1/License.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ===============================================================================
 MIT License
 ===============================================================================
 
-Copyright (c) 2020-2023, Martin Abel
+Copyright 2020-2023, Martin Abel, eVation
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `decoratory-0.9.5.3/PKG-INFO` & `decoratory-0.9.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoratory
-Version: 0.9.5.3
+Version: 0.9.6.1
 Summary: Decorators: Singleton, Multiton, Observer, Observable, generic Wrapper.
 Home-page: http://evation.eu/index.html
 Download-URL: http://evation.eu/Section/Download.html
 Author: Martin Abel
 Author-email: Martin Abel <python@evation.eu>
 Maintainer: Martin Abel
 Maintainer-email: Martin Abel <python@evation.eu>
@@ -49,17 +49,17 @@
     __maintainer__ = "Martin Abel"
     __credits__ = ["Martin Abel"]
     __company__ = "eVation"
     __email__ = "python@evation.eu"
     __url__ = "http://evation.eu"
     __copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
     __created__ = "2020-01-01"
-    __version__ = "0.9.5.2"
-    __date__ = "2023-07-17"
-    __time__ = "15:53:35"
+    __version__ = "0.9.6.1"
+    __date__ = "2023-07-18"
+    __time__ = "19:54:26"
     __state__ = "Beta"
     __license__ = "MIT"
     --------------------------------------------------------------------------
 
 
 ==============================================================================
 Decoratory
```

### Comparing `decoratory-0.9.5.3/Readme.rst` & `decoratory-0.9.6.1/Readme.rst`

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     __maintainer__ = "Martin Abel"
     __credits__ = ["Martin Abel"]
     __company__ = "eVation"
     __email__ = "python@evation.eu"
     __url__ = "http://evation.eu"
     __copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
     __created__ = "2020-01-01"
-    __version__ = "0.9.5.2"
-    __date__ = "2023-07-17"
-    __time__ = "15:53:35"
+    __version__ = "0.9.6.1"
+    __date__ = "2023-07-18"
+    __time__ = "19:54:26"
     __state__ = "Beta"
     __license__ = "MIT"
     --------------------------------------------------------------------------
 
 
 ==============================================================================
 Decoratory
```

### Comparing `decoratory-0.9.5.3/Sources/decoratory/__main__.py` & `decoratory-0.9.6.1/Sources/decoratory/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.5.3"
-__date__ = "2023-07-17"
-__time__ = "15:53:35"
+__version__ = "0.9.6.1"
+__date__ = "2023-07-18"
+__time__ = "19:54:26"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["get_file_location"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.5.3/Sources/decoratory/banner.py` & `decoratory-0.9.6.1/Sources/decoratory/banner.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.5.1"
-__date__ = "2023-07-17"
-__time__ = "15:43:02"
+__version__ = "0.9.6.1"
+__date__ = "2023-07-18"
+__time__ = "19:54:26"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["__banner"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.5.3/Sources/decoratory/basic.py` & `decoratory-0.9.6.1/Sources/decoratory/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,17 +37,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.5.1"
-__date__ = "2023-07-17"
-__time__ = "15:43:02"
+__version__ = "0.9.6.1"
+__date__ = "2023-07-18"
+__time__ = "19:54:26"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Activation", "Parser", "F", "X", "BaseDecorator"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.5.3/Sources/decoratory/multiton.py` & `decoratory-0.9.6.1/Sources/decoratory/multiton.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,17 +125,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.5.1"
-__date__ = "2023-07-17"
-__time__ = "15:43:02"
+__version__ = "0.9.6.1"
+__date__ = "2023-07-18"
+__time__ = "19:54:26"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Multiton"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
@@ -243,15 +243,16 @@
             try:
                 if isinstance(self.__key, F):  # classmethod or staticmethod
                     if callable(self.__key.callee):
                         d_key = F(self.__key.callee, *subst.callee_args,
                                   **subst.callee_kwargs).eval()
                     else:
                         d_key = F(
-                            getattr(self.substitute.callee, self.__key.callee),
+                            getattr(self.__get__substitute().callee,
+                                    self.__key.callee),
                             *subst.callee_args, **subst.callee_kwargs).eval()
                 elif callable(self.__key):  # function
                     d_key = F(self.__key, *subst.callee_args,
                               **subst.callee_kwargs).eval()
                 else:  # Value
                     d_key = self.__key
                 instance = self._instances.get(d_key, None)
```

### Comparing `decoratory-0.9.5.3/Sources/decoratory/observer.py` & `decoratory-0.9.6.1/Sources/decoratory/observer.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     Examples
     --------
 
     A) Observable Decoration
 
     The simplest and at the same time the most pythonic variant of decoration
-    is to decorate only the observed entities as a Observable.
+    is to decorate only the observed entities as an Observable.
 
     This is possible because all observer pattern functionalities are
     concentrated in the Observable.BaseClass = BaseObservable of the observable
     decorator, while the Observer.BaseClass = BaseObserver of the observer
     decorator remains empty here. If necessary, it is possible to inherit from
     both BaseClasses to modify their functionalities.
 
@@ -407,17 +407,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.5.1"
-__date__ = "2023-07-17"
-__time__ = "15:43:02"
+__version__ = "0.9.6.1"
+__date__ = "2023-07-18"
+__time__ = "19:54:26"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Observer", "BaseObserver", "Observable", "BaseObservable"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.5.3/Sources/decoratory/singleton.py` & `decoratory-0.9.6.1/Sources/decoratory/singleton.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,17 +84,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.5.1"
-__date__ = "2023-07-17"
-__time__ = "15:43:02"
+__version__ = "0.9.6.1"
+__date__ = "2023-07-18"
+__time__ = "19:54:26"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Singleton", "SemiSingleton"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
@@ -114,19 +114,19 @@
     ----------
     substitute (callable|type):
         A type to be made a singleton
 
     resettable (bool):
         If True exposes a reset() method
 
+    instance (object):              (property)
+        Gets/Sets a singleton instance
+
     Methods
     -------
-    get_instance(self) -> object:
-        Return the singleton instance (primary instance)
-
     reset(self) -> None:            (if resettable=True, only!)
         Resets the singleton instance (None)
     """
 
     def __init__(self,
                  substitute: Union[type, callable, None] = None,
                  *args: object,
@@ -140,21 +140,21 @@
 
         Returns:
             self (object): Singleton decorator instance
         """
         self.__set__substitute(substitute)
 
         # The unique instance
-        self.__instance = None
+        self._instance = None
 
         # If resettable == True exposes a reset() method
         if bool(resettable):
             def reset(s: object = self) -> None:
                 """Define reset method"""
-                s.__instance = None
+                s._instance = None
 
             # Add the reset method
             setattr(self, 'reset', reset)
 
         # --- Decorator Arguments Template (1/2)
         if self.__get__substitute() is not None:
             # Decoration without parameter(s)
@@ -169,35 +169,41 @@
         if self.__get__substitute() is None:
             # Decoration with parameter(s)
             self.__set__substitute(F(args[0], *args[1:], **kwargs))
             update_wrapper(self, self.__get__substitute().callee, updated=())
             return self
         else:  # *** Decorator ***
             # Create and store new or return existing instance
-            if self.__instance is None:
+            if self._instance is None:
                 if args or kwargs:
-                    self.__instance = F(self.__get__substitute().callee,
-                                        *args, **kwargs).eval()
+                    self._instance = F(self.__get__substitute().callee,
+                                       *args, **kwargs).eval()
                 else:
-                    self.__instance = self.__get__substitute().eval()
-            return self.__instance
+                    self._instance = self.__get__substitute().eval()
+            return self._instance
 
     # Getter, Setter, Properties
     def __get__substitute(self):
         return self.__substitute
 
     def __set__substitute(self, value):
         self.__substitute = value
 
     substitute = property(__get__substitute)
 
     # Methods
     def get_instance(self) -> object:
         """Returns the singleton instance"""
-        return self.__instance
+        return self._instance
+
+    def set_instance(self, value: dict = None) -> None:
+        """Sets the singleton instance"""
+        self._instance = value
+
+    instance = property(get_instance, set_instance)
 
 
 class SemiSingleton(Singleton):
     """SemiSingleton
 
     A subclass shortcut for a resettable singleton.
     """
```

### Comparing `decoratory-0.9.5.3/Sources/decoratory/wrapper.py` & `decoratory-0.9.6.1/Sources/decoratory/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,17 +136,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.5.1"
-__date__ = "2023-07-17"
-__time__ = "15:43:02"
+__version__ = "0.9.6.1"
+__date__ = "2023-07-18"
+__time__ = "19:54:26"
 __state__ = "Beta"
 __license__ = "MIT"
 
 __all__ = ["Wrapper"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.9.5.3/Sources/decoratory.egg-info/PKG-INFO` & `decoratory-0.9.6.1/Sources/decoratory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoratory
-Version: 0.9.5.3
+Version: 0.9.6.1
 Summary: Decorators: Singleton, Multiton, Observer, Observable, generic Wrapper.
 Home-page: http://evation.eu/index.html
 Download-URL: http://evation.eu/Section/Download.html
 Author: Martin Abel
 Author-email: Martin Abel <python@evation.eu>
 Maintainer: Martin Abel
 Maintainer-email: Martin Abel <python@evation.eu>
@@ -49,17 +49,17 @@
     __maintainer__ = "Martin Abel"
     __credits__ = ["Martin Abel"]
     __company__ = "eVation"
     __email__ = "python@evation.eu"
     __url__ = "http://evation.eu"
     __copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
     __created__ = "2020-01-01"
-    __version__ = "0.9.5.2"
-    __date__ = "2023-07-17"
-    __time__ = "15:53:35"
+    __version__ = "0.9.6.1"
+    __date__ = "2023-07-18"
+    __time__ = "19:54:26"
     __state__ = "Beta"
     __license__ = "MIT"
     --------------------------------------------------------------------------
 
 
 ==============================================================================
 Decoratory
```

### Comparing `decoratory-0.9.5.3/Sources/decoratory.egg-info/SOURCES.txt` & `decoratory-0.9.6.1/Sources/decoratory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decoratory-0.9.5.3/Unittest/test_basic.py` & `decoratory-0.9.6.1/Unittest/test_basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.5.1"
-__date__ = "2023-07-17"
-__time__ = "15:43:02"
+__version__ = "0.9.6.1"
+__date__ = "2023-07-18"
+__time__ = "19:54:26"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
 
@@ -51,16 +51,14 @@
         pass
 
     def test_activation(self):
         """Unittest: Activation"""
 
         # ---------------------------------------------------------------------
         # Test
-        self.assertEqual(len(Activation), 4)
-
         self.assertNotEqual(Activation.NONE, Activation.BEFORE)
         self.assertNotEqual(Activation.NONE, Activation.AFTER)
         self.assertNotEqual(Activation.NONE, Activation.BEFORE_AND_AFTER)
         self.assertNotEqual(Activation.BEFORE, Activation.AFTER)
         self.assertNotEqual(Activation.BEFORE, Activation.BEFORE_AND_AFTER)
         self.assertNotEqual(Activation.AFTER, Activation.BEFORE_AND_AFTER)
```

### Comparing `decoratory-0.9.5.3/Unittest/test_multiton.py` & `decoratory-0.9.6.1/Unittest/test_multiton.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.5.1"
-__date__ = "2023-07-17"
-__time__ = "15:43:02"
+__version__ = "0.9.6.1"
+__date__ = "2023-07-18"
+__time__ = "19:54:26"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.9.5.3/Unittest/test_observer.py` & `decoratory-0.9.6.1/Unittest/test_observer.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.5.1"
-__date__ = "2023-07-17"
-__time__ = "15:43:02"
+__version__ = "0.9.6.1"
+__date__ = "2023-07-18"
+__time__ = "19:54:26"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
 
@@ -462,16 +462,14 @@
         # Observer
         def person(say: str = "Hello?") -> None:
             """A person function"""
             res.append(f"{person.__name__} says '{say}'")
 
         # ---------------------------------------------------------------------
         # Test
-        self.assertEqual(len(Activation), 4)
-
         self.assertNotEqual(Activation.NONE, Activation.BEFORE)
         self.assertNotEqual(Activation.NONE, Activation.AFTER)
         self.assertNotEqual(Activation.NONE, Activation.BEFORE_AND_AFTER)
         self.assertNotEqual(Activation.BEFORE, Activation.AFTER)
         self.assertNotEqual(Activation.BEFORE, Activation.BEFORE_AND_AFTER)
         self.assertNotEqual(Activation.AFTER, Activation.BEFORE_AND_AFTER)
```

### Comparing `decoratory-0.9.5.3/Unittest/test_singleton.py` & `decoratory-0.9.6.1/Unittest/test_singleton.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.5.1"
-__date__ = "2023-07-17"
-__time__ = "15:43:02"
+__version__ = "0.9.6.1"
+__date__ = "2023-07-18"
+__time__ = "19:54:26"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.9.5.3/Unittest/test_wrapper.py` & `decoratory-0.9.6.1/Unittest/test_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.5.1"
-__date__ = "2023-07-17"
-__time__ = "15:43:02"
+__version__ = "0.9.6.1"
+__date__ = "2023-07-18"
+__time__ = "19:54:26"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.9.5.3/setup.py` & `decoratory-0.9.6.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__author__}, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.9.5.3"
-__date__ = "2023-07-17"
-__time__ = "15:53:35"
+__version__ = "0.9.6.1"
+__date__ = "2023-07-18"
+__time__ = "19:54:26"
 __state__ = "Beta"
 __license__ = "MIT"
 
 # -----------------------------------------------------------------------------
 # Libraries
 from os.path import join
 from setuptools import setup, find_packages
```

