# Comparing `tmp/langful-0.35-py3-none-any.whl.zip` & `tmp/langful-0.36-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5610 bytes, number of entries: 7
+Zip file size: 5528 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat      166 b- defN 23-Jul-06 06:25 langful/__init__.py
--rw-rw-rw-  2.0 fat    10563 b- defN 23-Jul-16 01:14 langful/lang.py
--rw-rw-rw-  2.0 fat     1066 b- defN 23-Jul-16 01:18 langful-0.35.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3389 b- defN 23-Jul-16 01:18 langful-0.35.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-16 01:18 langful-0.35.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-16 01:18 langful-0.35.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      528 b- defN 23-Jul-16 01:18 langful-0.35.dist-info/RECORD
-7 files, 15812 bytes uncompressed, 4680 bytes compressed:  70.4%
+-rw-rw-rw-  2.0 fat     9860 b- defN 23-Jul-18 02:04 langful/lang.py
+-rw-rw-rw-  2.0 fat     1066 b- defN 23-Jul-18 02:05 langful-0.36.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3074 b- defN 23-Jul-18 02:05 langful-0.36.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-18 02:05 langful-0.36.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-18 02:05 langful-0.36.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      527 b- defN 23-Jul-18 02:05 langful-0.36.dist-info/RECORD
+7 files, 14793 bytes uncompressed, 4598 bytes compressed:  68.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: langful/__init__.py
 Comment: 
 
 Filename: langful/lang.py
 Comment: 
 
-Filename: langful-0.35.dist-info/LICENSE
+Filename: langful-0.36.dist-info/LICENSE
 Comment: 
 
-Filename: langful-0.35.dist-info/METADATA
+Filename: langful-0.36.dist-info/METADATA
 Comment: 
 
-Filename: langful-0.35.dist-info/WHEEL
+Filename: langful-0.36.dist-info/WHEEL
 Comment: 
 
-Filename: langful-0.35.dist-info/top_level.txt
+Filename: langful-0.36.dist-info/top_level.txt
 Comment: 
 
-Filename: langful-0.35.dist-info/RECORD
+Filename: langful-0.36.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langful/lang.py

```diff
@@ -1,30 +1,30 @@
 """
 # lang
 """
 
 import json
 import os
+import re
+
+__all__ = [ "to_json" , "to_lang" , "getdefaultlocale" , "lang" ]
 
 def to_json( lang_file : str ) -> dict :
     """
     .lang -> .json
     """
-    import re
     ret = {}
     for line in lang_file.split( "\n" ) :
         text = re.split( "([^#^=^\\s]+|)(\\s+=\\s+|\\s+=|=\\s+|=|)([^#^\\n]+|)" , line )
-        n = 0
-        for s in text :
-            if "=" in s :
+        index = 0
+        for value in text :
+            if "=" in value :
+                ret[ "".join( text[ :index ] ) ] = "".join( text[ index + 1: ] )
                 break
-            n += 1
-        else :
-            continue
-        ret[ "".join( text[:n] ) ] = "".join( text[n + 1:] )
+            index += 1
     return ret
 
 def to_lang( dict_file : dict ) -> str :
     """
     .json -> .lang
     """
     ret = ""
@@ -37,15 +37,15 @@
     getdefaultlocale will deprecated so use this
     """
     import locale
     import sys
     if sys.platform == "win32" :
         code = __import__( "_locale" )._getdefaultlocale()[ 0 ]
         if code[ :2 ] == "0x" :
-            code = locale.windows_locale[ code ]
+            code = locale.windows_locale[ int( code , 0 ) ]
     else :
         code = locale.getlocale()[ 0 ]
     return code.replace( "-" , "_" ).lower()
 
 class lang :
     """
     # lang
@@ -108,20 +108,18 @@
         """
         init by a directory
         """
         self.is_file = True
         if not os.path.exists( path ) :
             raise FileNotFoundError( f"can't find '{ os.path.abspath( path ) }'" )
         loads = [ [ ".lang" , ".json" ] , [ ".json" , ".lang" ] ][ self.json_first ]
-        files = []
-        for i in os.listdir( path ) :
-            name , suffix = os.path.splitext( i )
-            if ( suffix in loads ) and ( ( suffix == loads[ 0 ] ) or ( name + loads[ 0 ] not in files ) ) :
-                files.append( i )
-                with open( os.path.join( path , i ) , "r" , encoding = "utf-8" ) as file :
+        for lang_file in os.listdir( path ) :
+            name , suffix = os.path.splitext( lang_file )
+            if ( suffix in loads ) and ( ( suffix == loads[ 0 ] ) or ( suffix not in self.locales ) ) :
+                with open( os.path.join( path , lang_file ) , "r" , encoding = "utf-8" ) as file :
                     if suffix == ".json" :
                         try :
                             data = json.load( file )
                         except json.decoder.JSONDecodeError :
                             raise SyntaxError( "can't to load .json file" )
                     elif suffix == ".lang" :
                         data = to_json( file.read() )
@@ -165,22 +163,18 @@
         return list( self.types.keys() )
 
     @property
     def locale( self ) -> str :
         """
         choose locale
         """
-        if self.use_locale and self.use_locale in self.locales :
-            return self.use_locale
-        elif self.system_locale in self.locales :
-            return self.system_locale
-        elif self.default_locale in self.locales :
-            return self.default_locale
-        else :
-            raise KeyError( f"no such locale '{ self.system_locale }' or '{ self.default_locale }'" )
+        for locale in [ self.use_locale , self.system_locale , self.default_locale ] :
+            if locale and locale in self.locales :
+                return locale
+        raise KeyError( f"no such locale '{ self.system_locale }' or '{ self.default_locale }'" )
 
     @property
     def language( self ) -> dict :
         """
         get now language
         """
         return self.lang_get( self.locale )
@@ -202,32 +196,32 @@
     @property
     def type( self ) -> str :
         """
         get type, ".json" or ".lang"
         """
         return self.types[ self.locale ]
 
-    def locale_get( self , locale : str = None ) -> str :
-        """
-        get locale, usually use in function
-        """
-        if locale :
-            return locale
-        else :
-            return self.locale
-
     def replace_letter_get( self , replace_letter : str = None ) -> str :
         """
         get replace letter, usually use in function
         """
         if replace_letter :
             return replace_letter
         else :
             return self.replace_letter
 
+    def locale_get( self , locale : str = None ) -> str :
+        """
+        get locale, usually use in function
+        """
+        if locale :
+            return locale
+        else :
+            return self.locale
+
     def locale_set( self , locale : str = None  ) -> None :
         """
         if give a locale then set that, else reset it
         """
         if locale and locale not in self.locales :
             raise KeyError( f"no such locale '{ locale }'" )
         self.use_locale = locale
@@ -236,22 +230,22 @@
         """
         get a lang
         """
         return self.languages[ locale ]
 
     def lang_set( self , locale : str , value : dict = {} , suffix : str = ".json" ) -> None :
         """
-        set a new lang
+        set a lang
         """
         self.languages[ locale ] = value
         self.types[ locale ] = suffix
 
-    def lang_del( self , locale : str ) -> None :
+    def lang_remove( self , locale : str ) -> None :
         """
-        del a lang
+        remove a lang
         """
         del self.languages[ locale ]
         del self.types[ locale ]
 
     def lang_merge( self , to : str , locale : str = None , args : str | list = [] ) -> None :
         """
         merge to a locale
@@ -275,73 +269,51 @@
     def remove( self , key : str , locale : str = None ) -> None :
         """
         remove a value by a locale dictionary
         """
         locale = self.locale_get( locale )
         del self.languages[ locale ][ key ]
 
-    def save( self , separators : list = [ " ," , ": " ] ) -> None :
+    def merge( self , locale : str = None , args : str | list = [] ) -> dict :
+        """
+        merge
+        """
+        if isinstance( args , str ) :
+            args = [ args ]
+        ret = self.lang_get( self.locale_get( locale ) )
+        for locale_key in args :
+            for key , value in self.lang_get( locale_key ).items() :
+                ret[ key ] = value
+        return ret
+
+    def save( self , separators : list = [ " ," , ": " ] ) -> dict :
         """
-        save file when is_file variable is true, else raise the error
+        save file when is_file variable is true
         """
         if isinstance( self.lang_dir , str ) :
             for key , value in self.languages.items() :
                 suffix = self.types[ key ]
                 with open( os.path.join( self.lang_dir , key + suffix ) , "w" , encoding = "utf-8" ) as file :
                     if suffix == ".json" :
                         file.write( json.dumps( value , indent = 4 , separators = separators , ensure_ascii = False ) )
                     elif suffix == ".lang" :
                         file.write( to_lang( value ) )
         return self.languages
 
-    def merge( self , locale : str = None , args : str | list = [] ) -> dict :
-        """
-        merge
-        """
-        if isinstance( args , str ) :
-            args = [ args ]
-        ret = self.lang_get( self.locale_get( locale ) )
-        for i in args :
-            for key , value in self.lang_get( i ).items() :
-                ret[ key ] = value
-        return ret
-
     def replace( self , key : str = None , args : str | list  = None , locale : str = None , replace_letter : str = None ) -> str :
         """
         replace
         """
         replace_letter = self.replace_letter_get( replace_letter )
         locale = self.locale_get( locale )
-        text = self.get( key , locale ).split( replace_letter )
         if isinstance( args , str ) :
             args = [ args ]
+        index = 0
         ret = ""
-        p = 0
-        for i in text :
-            ret += i
-            if ( p + 1 ) < len( text ) :
-                if p < len( args ) :
-                    ret += str( args[ p ] )
-                else :
-                    ret += str( args[ -1 ] )
-                p += 1
-        return ret
-
-    def replace_str( self , text : str , locale : str = None , replace_letter : str = None ) -> str :
-        """
-        replace by str
-        """
-        locale = self.locale_get( locale )
-        replace_letter = self.replace_letter_get( replace_letter )
-        text = text.split( replace_letter )
-        ret = ""
-        p = 0
-        for i in text :
-            if p % 2 :
-                if i :
-                    ret += self.get( i )
-                else :
-                    ret += replace_letter
+        for text in re.split( f"({ replace_letter }+)" , self.get( key , locale ) ) :
+            if text != replace_letter :
+                ret += text
             else :
-                ret += i
-            p += 1
+                ret += text.replace( replace_letter , str( args[ index ] ) )
+                if index + 1 < len( args ) :
+                    index += 1
         return ret
```

## Comparing `langful-0.35.dist-info/LICENSE` & `langful-0.36.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langful-0.35.dist-info/METADATA` & `langful-0.36.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langful
-Version: 0.35
+Version: 0.36
 Summary: Help to localization
 Home-page: https://github.com/cueavy/langful
 Author: cueavyqwp
 Author-email: cueavyqwp@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -122,32 +122,14 @@
     "en_us" : {
         "test" : "&.&%"
     }
 } )
 print( lang.replace( "test" , [ 33 , 3 ] ) )
 ```
 
-### replace str
-
-```python
-import langful
-lang = langful.lang( False )
-lang.init_dict( {
-    "en_us" : {
-        "hi" : "Hi" ,
-        "welcome" : "Welcome"
-    } ,
-    "zh_cn" : {
-        "hi" : "你好" ,
-        "welcome" : "欢迎"
-    }
-} )
-print(lang.replace_str( "%hi%, %welcome%!" ))
-```
-
 ### merge
 
 ```python
 import langful
 lang = langful.lang( False )
 lang.init_dict( {
     "en_us" : {
```

