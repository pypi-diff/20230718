# Comparing `tmp/pyminr-0.1.0-py3-none-win_amd64.whl.zip` & `tmp/pyminr-0.1.1-py3-none-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 30738 bytes, number of entries: 7
--rw-r--r--  2.0 unx      887 b- defN 23-Feb-15 18:47 pyminr/__init__.py
--rw-r--r--  2.0 unx    64000 b- defN 23-Jan-24 18:45 pyminr/lib/minr.dll
--rw-r--r--  2.0 unx    18092 b- defN 23-Feb-15 18:48 pyminr-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      318 b- defN 23-Feb-15 18:48 pyminr-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       98 b- defN 23-Feb-15 18:48 pyminr-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Feb-15 18:48 pyminr-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      531 b- defN 23-Feb-15 18:48 pyminr-0.1.0.dist-info/RECORD
-7 files, 83933 bytes uncompressed, 29802 bytes compressed:  64.5%
+Zip file size: 30211 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      775 b- defN 23-Jul-18 17:17 pyminr/__init__.py
+-rw-r--r--  2.0 unx    67144 b- defN 23-Jul-18 17:38 pyminr/lib/libminr.so
+-rw-r--r--  2.0 unx    18092 b- defN 23-Jul-18 17:38 pyminr-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      318 b- defN 23-Jul-18 17:38 pyminr-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      109 b- defN 23-Jul-18 17:38 pyminr-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-18 17:38 pyminr-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      534 b- defN 23-Jul-18 17:38 pyminr-0.1.1.dist-info/RECORD
+7 files, 86979 bytes uncompressed, 29271 bytes compressed:  66.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pyminr/__init__.py
 Comment: 
 
-Filename: pyminr/lib/minr.dll
+Filename: pyminr/lib/libminr.so
 Comment: 
 
-Filename: pyminr-0.1.0.dist-info/LICENSE
+Filename: pyminr-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: pyminr-0.1.0.dist-info/METADATA
+Filename: pyminr-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: pyminr-0.1.0.dist-info/WHEEL
+Filename: pyminr-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: pyminr-0.1.0.dist-info/top_level.txt
+Filename: pyminr-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pyminr-0.1.0.dist-info/RECORD
+Filename: pyminr-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyminr/__init__.py

```diff
@@ -9,24 +9,20 @@
 elif sys.platform == 'win32':
     _lib_name = 'minr.dll'
 else:
     _lib_name = 'libminr.so'
 
 _lib = ctypes.CDLL(os.path.join(os.path.dirname(__file__), 'lib', _lib_name))
 
-load_crypto_definitions = _lib.load_crypto_definitions
-clean_crypto_definitions = _lib.clean_crypto_definitions
-
-
 _report_result_t = ctypes.CFUNCTYPE(None, ctypes.c_char_p, ctypes.c_ushort)
 
 _find_crypto_algorithms = _lib.find_crypto_algorithms
 _find_crypto_algorithms.argtypes = [ctypes.c_char_p, ctypes.c_uint64, _report_result_t]
 
-def find_crypto_algorithms(src: str, report_result_callback: Callable[[str, str], None]):
+def find_crypto_algorithms(src: bytes, report_result_callback: Callable[[str, str], None]):
     def _report_result(a, c):
         report_result_callback(a.decode("utf-8"), c)
     _find_crypto_algorithms(src, len(src), _report_result_t(_report_result))
```

## Comparing `pyminr-0.1.0.dist-info/LICENSE` & `pyminr-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

