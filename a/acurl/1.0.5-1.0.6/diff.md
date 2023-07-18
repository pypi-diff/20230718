# Comparing `tmp/acurl-1.0.5.tar.gz` & `tmp/acurl-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acurl-1.0.5.tar", last modified: Thu Mar 23 10:45:15 2023, max compression
+gzip compressed data, was "acurl-1.0.6.tar", last modified: Tue Jul 18 14:32:59 2023, max compression
```

## Comparing `acurl-1.0.5.tar` & `acurl-1.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:15.047080 acurl-1.0.5/
--rw-r--r--   0 root         (0) root         (0)       80 2023-03-23 10:44:49.000000 acurl-1.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2240 2023-03-23 10:45:15.047080 acurl-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1590 2023-03-23 10:44:49.000000 acurl-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:15.047080 acurl-1.0.5/acurl.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2240 2023-03-23 10:45:15.000000 acurl-1.0.5/acurl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      518 2023-03-23 10:45:15.000000 acurl-1.0.5/acurl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-23 10:45:15.000000 acurl-1.0.5/acurl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-03-23 10:45:15.000000 acurl-1.0.5/acurl.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-03-23 10:45:15.000000 acurl-1.0.5/acurl.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       60 2023-03-23 10:44:49.000000 acurl-1.0.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      861 2023-03-23 10:45:15.047080 acurl-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      914 2023-03-23 10:44:49.000000 acurl-1.0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:15.047080 acurl-1.0.5/src/
--rw-r--r--   0 root         (0) root         (0)  1400322 2023-03-23 10:45:14.000000 acurl-1.0.5/src/acurl.c
--rw-r--r--   0 root         (0) root         (0)     4904 2023-03-23 10:44:49.000000 acurl-1.0.5/src/acurl.pyx
--rw-r--r--   0 root         (0) root         (0)     2593 2023-03-23 10:44:49.000000 acurl-1.0.5/src/acurl_wrappers.h
--rw-r--r--   0 root         (0) root         (0)     3925 2023-03-23 10:44:49.000000 acurl-1.0.5/src/cookie.pyx
--rw-r--r--   0 root         (0) root         (0)     5311 2023-03-23 10:44:49.000000 acurl-1.0.5/src/curlinterface.pxd
--rw-r--r--   0 root         (0) root         (0)     3032 2023-03-23 10:44:49.000000 acurl-1.0.5/src/request.pyx
--rw-r--r--   0 root         (0) root         (0)     8514 2023-03-23 10:44:49.000000 acurl-1.0.5/src/response.pyx
--rw-r--r--   0 root         (0) root         (0)    13825 2023-03-23 10:44:49.000000 acurl-1.0.5/src/session.pyx
--rw-r--r--   0 root         (0) root         (0)     1451 2023-03-23 10:44:49.000000 acurl-1.0.5/src/utils.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:15.047080 acurl-1.0.5/tests/
--rw-r--r--   0 root         (0) root         (0)      520 2023-03-23 10:44:49.000000 acurl-1.0.5/tests/test_acurl.py
--rw-r--r--   0 root         (0) root         (0)     2563 2023-03-23 10:44:49.000000 acurl-1.0.5/tests/test_cookie.py
--rw-r--r--   0 root         (0) root         (0)     2259 2023-03-23 10:44:49.000000 acurl-1.0.5/tests/test_httpbin.py
--rw-r--r--   0 root         (0) root         (0)     2083 2023-03-23 10:44:49.000000 acurl-1.0.5/tests/test_request.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-03-23 10:44:49.000000 acurl-1.0.5/tests/test_response.py
--rw-r--r--   0 root         (0) root         (0)     3824 2023-03-23 10:44:49.000000 acurl-1.0.5/tests/test_session.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-03-23 10:44:49.000000 acurl-1.0.5/tests/test_to_curl.py
--rw-r--r--   0 root         (0) root         (0)     1892 2023-03-23 10:44:49.000000 acurl-1.0.5/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:59.785392 acurl-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-18 14:32:33.000000 acurl-1.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2240 2023-07-18 14:32:59.785392 acurl-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-07-18 14:32:33.000000 acurl-1.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:59.785392 acurl-1.0.6/acurl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2240 2023-07-18 14:32:59.000000 acurl-1.0.6/acurl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      518 2023-07-18 14:32:59.000000 acurl-1.0.6/acurl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 14:32:59.000000 acurl-1.0.6/acurl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-18 14:32:59.000000 acurl-1.0.6/acurl.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-18 14:32:59.000000 acurl-1.0.6/acurl.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-07-18 14:32:33.000000 acurl-1.0.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      861 2023-07-18 14:32:59.789392 acurl-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      914 2023-07-18 14:32:33.000000 acurl-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:59.785392 acurl-1.0.6/src/
+-rw-r--r--   0 root         (0) root         (0)  1403728 2023-07-18 14:32:59.000000 acurl-1.0.6/src/acurl.c
+-rw-r--r--   0 root         (0) root         (0)     4904 2023-07-18 14:32:33.000000 acurl-1.0.6/src/acurl.pyx
+-rw-r--r--   0 root         (0) root         (0)     2593 2023-07-18 14:32:33.000000 acurl-1.0.6/src/acurl_wrappers.h
+-rw-r--r--   0 root         (0) root         (0)     3925 2023-07-18 14:32:33.000000 acurl-1.0.6/src/cookie.pyx
+-rw-r--r--   0 root         (0) root         (0)     5311 2023-07-18 14:32:33.000000 acurl-1.0.6/src/curlinterface.pxd
+-rw-r--r--   0 root         (0) root         (0)     3032 2023-07-18 14:32:33.000000 acurl-1.0.6/src/request.pyx
+-rw-r--r--   0 root         (0) root         (0)     8514 2023-07-18 14:32:33.000000 acurl-1.0.6/src/response.pyx
+-rw-r--r--   0 root         (0) root         (0)    13825 2023-07-18 14:32:33.000000 acurl-1.0.6/src/session.pyx
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-07-18 14:32:33.000000 acurl-1.0.6/src/utils.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 14:32:59.785392 acurl-1.0.6/tests/
+-rw-r--r--   0 root         (0) root         (0)      520 2023-07-18 14:32:33.000000 acurl-1.0.6/tests/test_acurl.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2023-07-18 14:32:33.000000 acurl-1.0.6/tests/test_cookie.py
+-rw-r--r--   0 root         (0) root         (0)     2259 2023-07-18 14:32:33.000000 acurl-1.0.6/tests/test_httpbin.py
+-rw-r--r--   0 root         (0) root         (0)     2083 2023-07-18 14:32:33.000000 acurl-1.0.6/tests/test_request.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-07-18 14:32:33.000000 acurl-1.0.6/tests/test_response.py
+-rw-r--r--   0 root         (0) root         (0)     3824 2023-07-18 14:32:33.000000 acurl-1.0.6/tests/test_session.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-07-18 14:32:33.000000 acurl-1.0.6/tests/test_to_curl.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-07-18 14:32:33.000000 acurl-1.0.6/tests/test_utils.py
```

### Comparing `acurl-1.0.5/PKG-INFO` & `acurl-1.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acurl
-Version: 1.0.5
+Version: 1.0.6
 Summary: An async Curl library.
 Home-page: https://github.com/sky-uk/mite/tree/master/acurl
 Author: Aaron Ecay
 Author-email: aaron.ecay@sky.uk
 Maintainer: Sky Identity NFT team
 Maintainer-email: matthew.ellis@sky.uk
 License: MIT
```

### Comparing `acurl-1.0.5/README.md` & `acurl-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `acurl-1.0.5/acurl.egg-info/PKG-INFO` & `acurl-1.0.6/acurl.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acurl
-Version: 1.0.5
+Version: 1.0.6
 Summary: An async Curl library.
 Home-page: https://github.com/sky-uk/mite/tree/master/acurl
 Author: Aaron Ecay
 Author-email: aaron.ecay@sky.uk
 Maintainer: Sky Identity NFT team
 Maintainer-email: matthew.ellis@sky.uk
 License: MIT
```

### Comparing `acurl-1.0.5/acurl.egg-info/SOURCES.txt` & `acurl-1.0.6/acurl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acurl-1.0.5/setup.cfg` & `acurl-1.0.6/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 	Programming Language :: Python :: 3.11
 author = Aaron Ecay
 author_email = aaron.ecay@sky.uk
 maintainer = Sky Identity NFT team
 maintainer_email = matthew.ellis@sky.uk
 license = MIT
 url = https://github.com/sky-uk/mite/tree/master/acurl
-version = 1.0.5
+version = 1.0.6
 
 [options]
 install_requires = 
 	ujson>=4.1.0
 	uvloop
 tests_require = pytest
```

### Comparing `acurl-1.0.5/setup.py` & `acurl-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `acurl-1.0.5/src/acurl.c` & `acurl-1.0.6/src/acurl.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "libraries": [
             "curl"
@@ -21,16 +21,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -90,18 +90,22 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -215,15 +219,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -254,15 +258,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -377,17 +381,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -457,14 +458,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -2408,22 +2414,30 @@
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* SetVTable.proto */
 static int __Pyx_SetVtable(PyObject *dict, void *vtable);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
@@ -22521,15 +22535,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_5acurl_Cookie(PyObject *o) {
   struct __pyx_obj_5acurl_Cookie *p = (struct __pyx_obj_5acurl_Cookie *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   Py_CLEAR(p->domain);
   Py_CLEAR(p->name);
   Py_CLEAR(p->value);
   (*Py_TYPE(o)->tp_free)(o);
@@ -22623,15 +22637,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_5acurl__Cookie __pyx_vtable_5acurl__Cookie;
 
 static PyObject *__pyx_tp_new_5acurl__Cookie(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_5acurl__Cookie *p;
@@ -22654,15 +22668,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_5acurl__Cookie(PyObject *o) {
   struct __pyx_obj_5acurl__Cookie *p = (struct __pyx_obj_5acurl__Cookie *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   Py_CLEAR(p->domain);
   Py_CLEAR(p->path);
   Py_CLEAR(p->name);
   Py_CLEAR(p->value);
@@ -22788,15 +22802,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_5acurl_Request __pyx_vtable_5acurl_Request;
 
 static PyObject *__pyx_tp_new_5acurl_Request(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_5acurl_Request *p;
@@ -22823,15 +22837,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_5acurl_Request(PyObject *o) {
   struct __pyx_obj_5acurl_Request *p = (struct __pyx_obj_5acurl_Request *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -23008,15 +23022,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_5acurl__Response __pyx_vtable_5acurl__Response;
 
 static PyObject *__pyx_tp_new_5acurl__Response(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_5acurl__Response *p;
@@ -23039,15 +23053,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_5acurl__Response(PyObject *o) {
   struct __pyx_obj_5acurl__Response *p = (struct __pyx_obj_5acurl__Response *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -23290,15 +23304,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_5acurl_Session __pyx_vtable_5acurl_Session;
 
 static PyObject *__pyx_tp_new_5acurl_Session(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_5acurl_Session *p;
@@ -23319,15 +23333,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_5acurl_Session(PyObject *o) {
   struct __pyx_obj_5acurl_Session *p = (struct __pyx_obj_5acurl_Session *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -23451,15 +23465,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_5acurl_CurlWrapper __pyx_vtable_5acurl_CurlWrapper;
 
 static PyObject *__pyx_tp_new_5acurl_CurlWrapper(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_5acurl_CurlWrapper *p;
@@ -23480,15 +23494,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_5acurl_CurlWrapper(PyObject *o) {
   struct __pyx_obj_5acurl_CurlWrapper *p = (struct __pyx_obj_5acurl_CurlWrapper *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -23596,15 +23610,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5acurl___pyx_scope_struct__store_session_cookies *__pyx_freelist_5acurl___pyx_scope_struct__store_session_cookies[8];
 static int __pyx_freecount_5acurl___pyx_scope_struct__store_session_cookies = 0;
 
@@ -23721,15 +23735,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5acurl___pyx_scope_struct_1_genexpr *__pyx_freelist_5acurl___pyx_scope_struct_1_genexpr[8];
 static int __pyx_freecount_5acurl___pyx_scope_struct_1_genexpr = 0;
 
@@ -23838,15 +23852,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5acurl___pyx_scope_struct_2_genexpr *__pyx_freelist_5acurl___pyx_scope_struct_2_genexpr[8];
 static int __pyx_freecount_5acurl___pyx_scope_struct_2_genexpr = 0;
 
@@ -23955,15 +23969,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5acurl___pyx_scope_struct_3___get__ *__pyx_freelist_5acurl___pyx_scope_struct_3___get__[8];
 static int __pyx_freecount_5acurl___pyx_scope_struct_3___get__ = 0;
 
@@ -24073,15 +24087,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5acurl___pyx_scope_struct_4_genexpr *__pyx_freelist_5acurl___pyx_scope_struct_4_genexpr[8];
 static int __pyx_freecount_5acurl___pyx_scope_struct_4_genexpr = 0;
 
@@ -24190,15 +24204,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5acurl___pyx_scope_struct_5___get__ *__pyx_freelist_5acurl___pyx_scope_struct_5___get__[8];
 static int __pyx_freecount_5acurl___pyx_scope_struct_5___get__ = 0;
 
@@ -24308,15 +24322,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5acurl___pyx_scope_struct_6_genexpr *__pyx_freelist_5acurl___pyx_scope_struct_6_genexpr[8];
 static int __pyx_freecount_5acurl___pyx_scope_struct_6_genexpr = 0;
 
@@ -24425,15 +24439,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5acurl___pyx_scope_struct_7_to_curl *__pyx_freelist_5acurl___pyx_scope_struct_7_to_curl[8];
 static int __pyx_freecount_5acurl___pyx_scope_struct_7_to_curl = 0;
 
@@ -24543,15 +24557,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5acurl___pyx_scope_struct_8_genexpr *__pyx_freelist_5acurl___pyx_scope_struct_8_genexpr[8];
 static int __pyx_freecount_5acurl___pyx_scope_struct_8_genexpr = 0;
 
@@ -24660,15 +24674,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5acurl___pyx_scope_struct_9_genexpr *__pyx_freelist_5acurl___pyx_scope_struct_9_genexpr[8];
 static int __pyx_freecount_5acurl___pyx_scope_struct_9_genexpr = 0;
 
@@ -24777,15 +24791,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5acurl___pyx_scope_struct_10___get__ *__pyx_freelist_5acurl___pyx_scope_struct_10___get__[8];
 static int __pyx_freecount_5acurl___pyx_scope_struct_10___get__ = 0;
 
@@ -24895,15 +24909,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5acurl___pyx_scope_struct_11_genexpr *__pyx_freelist_5acurl___pyx_scope_struct_11_genexpr[8];
 static int __pyx_freecount_5acurl___pyx_scope_struct_11_genexpr = 0;
 
@@ -25012,15 +25026,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5acurl___pyx_scope_struct_12___get__ *__pyx_freelist_5acurl___pyx_scope_struct_12___get__[8];
 static int __pyx_freecount_5acurl___pyx_scope_struct_12___get__ = 0;
 
@@ -25130,15 +25144,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5acurl___pyx_scope_struct_13_genexpr *__pyx_freelist_5acurl___pyx_scope_struct_13_genexpr[8];
 static int __pyx_freecount_5acurl___pyx_scope_struct_13_genexpr = 0;
 
@@ -25247,15 +25261,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5acurl___pyx_scope_struct_14_cookies *__pyx_freelist_5acurl___pyx_scope_struct_14_cookies[8];
 static int __pyx_freecount_5acurl___pyx_scope_struct_14_cookies = 0;
 
@@ -25365,15 +25379,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5acurl___pyx_scope_struct_15_genexpr *__pyx_freelist_5acurl___pyx_scope_struct_15_genexpr[8];
 static int __pyx_freecount_5acurl___pyx_scope_struct_15_genexpr = 0;
 
@@ -25482,15 +25496,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5acurl___pyx_scope_struct_16__outer_request *__pyx_freelist_5acurl___pyx_scope_struct_16__outer_request[8];
 static int __pyx_freecount_5acurl___pyx_scope_struct_16__outer_request = 0;
 
@@ -25651,15 +25665,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5acurl___pyx_scope_struct_17_genexpr *__pyx_freelist_5acurl___pyx_scope_struct_17_genexpr[8];
 static int __pyx_freecount_5acurl___pyx_scope_struct_17_genexpr = 0;
 
@@ -25772,15 +25786,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5acurl___pyx_scope_struct_18_genexpr *__pyx_freelist_5acurl___pyx_scope_struct_18_genexpr[8];
 static int __pyx_freecount_5acurl___pyx_scope_struct_18_genexpr = 0;
 
@@ -25893,15 +25907,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5acurl___pyx_scope_struct_19_delete *__pyx_freelist_5acurl___pyx_scope_struct_19_delete[8];
 static int __pyx_freecount_5acurl___pyx_scope_struct_19_delete = 0;
 
@@ -26010,15 +26024,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5acurl___pyx_scope_struct_20_get *__pyx_freelist_5acurl___pyx_scope_struct_20_get[8];
 static int __pyx_freecount_5acurl___pyx_scope_struct_20_get = 0;
 
@@ -26127,15 +26141,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5acurl___pyx_scope_struct_21_head *__pyx_freelist_5acurl___pyx_scope_struct_21_head[8];
 static int __pyx_freecount_5acurl___pyx_scope_struct_21_head = 0;
 
@@ -26244,15 +26258,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5acurl___pyx_scope_struct_22_options *__pyx_freelist_5acurl___pyx_scope_struct_22_options[8];
 static int __pyx_freecount_5acurl___pyx_scope_struct_22_options = 0;
 
@@ -26361,15 +26375,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5acurl___pyx_scope_struct_23_patch *__pyx_freelist_5acurl___pyx_scope_struct_23_patch[8];
 static int __pyx_freecount_5acurl___pyx_scope_struct_23_patch = 0;
 
@@ -26478,15 +26492,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5acurl___pyx_scope_struct_24_post *__pyx_freelist_5acurl___pyx_scope_struct_24_post[8];
 static int __pyx_freecount_5acurl___pyx_scope_struct_24_post = 0;
 
@@ -26595,15 +26609,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5acurl___pyx_scope_struct_25_put *__pyx_freelist_5acurl___pyx_scope_struct_25_put[8];
 static int __pyx_freecount_5acurl___pyx_scope_struct_25_put = 0;
 
@@ -26712,15 +26726,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_void____object___to_py *__pyx_freelist___pyx_scope_struct____Pyx_CFunc_void____object___to_py[8];
 static int __pyx_freecount___pyx_scope_struct____Pyx_CFunc_void____object___to_py = 0;
 
@@ -26808,15 +26822,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_void____CurlWrapper____int___to_py *__pyx_freelist___pyx_scope_struct____Pyx_CFunc_void____CurlWrapper____int___to_py[8];
 static int __pyx_freecount___pyx_scope_struct____Pyx_CFunc_void____CurlWrapper____int___to_py = 0;
 
@@ -26904,15 +26918,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_void____CurlWrapper___to_py *__pyx_freelist___pyx_scope_struct____Pyx_CFunc_void____CurlWrapper___to_py[8];
 static int __pyx_freecount___pyx_scope_struct____Pyx_CFunc_void____CurlWrapper___to_py = 0;
 
@@ -27000,15 +27014,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {"session_cookie_for_url", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5acurl_1session_cookie_for_url, METH_VARARGS|METH_KEYWORDS, 0},
   {"parse_cookie_string", (PyCFunction)__pyx_pw_5acurl_3parse_cookie_string, METH_O, 0},
@@ -28199,37 +28213,33 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(8, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(8, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(8, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(9, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(9, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(10, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(10, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(10, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("array"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_5array_array = __Pyx_ImportType(__pyx_t_1, "array", "array", sizeof(arrayobject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_5array_array) __PYX_ERR(7, 58, __pyx_L1_error)
+  __pyx_ptype_7cpython_5array_array = __Pyx_ImportType_0_29_36(__pyx_t_1, "array", "array", sizeof(arrayobject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(arrayobject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_5array_array) __PYX_ERR(7, 58, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -29567,28 +29577,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -31883,15 +31893,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 #if PY_VERSION_HEX < 0x030500B1 || defined(__Pyx_IterableCoroutine_USED) || CYTHON_USE_ASYNC_SLOTS
 static CYTHON_INLINE PyObject *__Pyx__Coroutine_await(PyObject *coroutine) {
     __pyx_CoroutineAwaitObject *await = PyObject_GC_New(__pyx_CoroutineAwaitObject, __pyx_CoroutineAwaitType);
     if (unlikely(!await)) return NULL;
@@ -32035,15 +32048,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_Coroutine_init(void) {
     __pyx_CoroutineType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_CoroutineType = __Pyx_FetchCommonType(&__pyx_CoroutineType_type);
     if (unlikely(!__pyx_CoroutineType))
@@ -32110,15 +32126,19 @@
 #endif
 #if PY_VERSION_HEX >= 0x030500B2 || defined(PyCoro_CheckExact)
     if (PyCoro_CheckExact(obj)) {
         return __Pyx_NewRef(obj);
     } else
 #endif
 #if CYTHON_COMPILING_IN_CPYTHON && defined(CO_ITERABLE_COROUTINE)
+#if PY_VERSION_HEX >= 0x030C00A6
+    if (PyGen_CheckExact(obj) && (PyGen_GetCode((PyGenObject*)obj)->co_flags & CO_ITERABLE_COROUTINE)) {
+#else
     if (PyGen_CheckExact(obj) && ((PyGenObject*)obj)->gi_code && ((PyCodeObject *)((PyGenObject*)obj)->gi_code)->co_flags & CO_ITERABLE_COROUTINE) {
+#endif
         return __Pyx_NewRef(obj);
     } else
 #endif
     {
         PyObject *method = NULL;
         int is_method = __Pyx_PyObject_GetMethod(obj, __pyx_n_s_await, &method);
         if (likely(is_method)) {
@@ -32160,15 +32180,15 @@
                  "object %.100s can't be used in 'await' expression",
                  Py_TYPE(obj)->tp_name);
 bad:
     return NULL;
 }
 
 /* CoroutineYieldFrom */
-static PyObject* __Pyx__Coroutine_Yield_From_Generic(__pyx_CoroutineObject *gen, PyObject *source) {
+  static PyObject* __Pyx__Coroutine_Yield_From_Generic(__pyx_CoroutineObject *gen, PyObject *source) {
     PyObject *retval;
     PyObject *source_gen = __Pyx__Coroutine_GetAwaitableIter(source);
     if (unlikely(!source_gen)) {
         return NULL;
     }
     if (__Pyx_Coroutine_Check(source_gen)) {
         retval = __Pyx_Generator_Next(source_gen);
@@ -32207,15 +32227,15 @@
         Py_INCREF(source);
         gen->yieldfrom = source;
     }
     return retval;
 }
 
 /* PyIntBinop */
-#if !CYTHON_COMPILING_IN_PYPY
+  #if !CYTHON_COMPILING_IN_PYPY
 static PyObject* __Pyx_PyInt_SubtractObjC(PyObject *op1, PyObject *op2, CYTHON_UNUSED long intval, int inplace, int zerodivision_check) {
     (void)inplace;
     (void)zerodivision_check;
     #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_CheckExact(op1))) {
         const long b = intval;
         long x;
@@ -32331,15 +32351,15 @@
             return PyFloat_FromDouble(result);
     }
     return (inplace ? PyNumber_InPlaceSubtract : PyNumber_Subtract)(op1, op2);
 }
 #endif
 
 /* PyIntCompare */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_EqObjC(PyObject *op1, PyObject *op2, CYTHON_UNUSED long intval, CYTHON_UNUSED long inplace) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_EqObjC(PyObject *op1, PyObject *op2, CYTHON_UNUSED long intval, CYTHON_UNUSED long inplace) {
     if (op1 == op2) {
         Py_RETURN_TRUE;
     }
     #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_CheckExact(op1))) {
         const long b = intval;
         long a = PyInt_AS_LONG(op1);
@@ -32398,15 +32418,15 @@
         if ((double)a == (double)b) Py_RETURN_TRUE; else Py_RETURN_FALSE;
     }
     return (
         PyObject_RichCompare(op1, op2, Py_EQ));
 }
 
 /* ReturnWithStopIteration */
-static void __Pyx__ReturnWithStopIteration(PyObject* value) {
+  static void __Pyx__ReturnWithStopIteration(PyObject* value) {
     PyObject *exc, *args;
 #if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_PYSTON
     __Pyx_PyThreadState_declare
     if ((PY_VERSION_HEX >= 0x03030000 && PY_VERSION_HEX < 0x030500B1)
             || unlikely(PyTuple_Check(value) || PyExceptionInstance_Check(value))) {
         args = PyTuple_New(1);
         if (unlikely(!args)) return;
@@ -32440,15 +32460,15 @@
     if (unlikely(!exc)) return;
 #endif
     PyErr_SetObject(PyExc_StopIteration, exc);
     Py_DECREF(exc);
 }
 
 /* CythonFunctionShared */
-#include <structmember.h>
+  #include <structmember.h>
 static PyObject *
 __Pyx_CyFunction_get_doc(__pyx_CyFunctionObject *op, CYTHON_UNUSED void *closure)
 {
     if (unlikely(op->func_doc == NULL)) {
         if (op->func.m_ml->ml_doc) {
 #if PY_MAJOR_VERSION >= 3
             op->func_doc = PyUnicode_FromString(op->func.m_ml->ml_doc);
@@ -33018,15 +33038,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -33056,38 +33079,38 @@
 static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *func, PyObject *dict) {
     __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
     m->func_annotations = dict;
     Py_INCREF(dict);
 }
 
 /* CythonFunction */
-static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml, int flags, PyObject* qualname,
+  static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml, int flags, PyObject* qualname,
                                       PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
     PyObject *op = __Pyx_CyFunction_Init(
         PyObject_GC_New(__pyx_CyFunctionObject, __pyx_CyFunctionType),
         ml, flags, qualname, closure, module, globals, code
     );
     if (likely(op)) {
         PyObject_GC_Track(op);
     }
     return op;
 }
 
 /* PyObject_GenericGetAttr */
-#if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
+  #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject* __Pyx_PyObject_GenericGetAttr(PyObject* obj, PyObject* attr_name) {
     if (unlikely(Py_TYPE(obj)->tp_dictoffset)) {
         return PyObject_GenericGetAttr(obj, attr_name);
     }
     return __Pyx_PyObject_GenericGetAttrNoDict(obj, attr_name);
 }
 #endif
 
 /* PyErrExceptionMatches */
-#if CYTHON_FAST_THREAD_STATE
+  #if CYTHON_FAST_THREAD_STATE
 static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
     Py_ssize_t i, n;
     n = PyTuple_GET_SIZE(tuple);
 #if PY_MAJOR_VERSION >= 3
     for (i=0; i<n; i++) {
         if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
     }
@@ -33104,15 +33127,15 @@
     if (unlikely(PyTuple_Check(err)))
         return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
     return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
 }
 #endif
 
 /* PyObjectGetAttrStrNoError */
-static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
+  static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
         __Pyx_PyErr_Clear();
 }
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
     PyObject *result;
@@ -33126,15 +33149,15 @@
     if (unlikely(!result)) {
         __Pyx_PyObject_GetAttrStr_ClearAttributeError();
     }
     return result;
 }
 
 /* SetupReduce */
-static int __Pyx_setup_reduce_is_named(PyObject* meth, PyObject* name) {
+  static int __Pyx_setup_reduce_is_named(PyObject* meth, PyObject* name) {
   int ret;
   PyObject *name_attr;
   name_attr = __Pyx_PyObject_GetAttrStr(meth, __pyx_n_s_name_2);
   if (likely(name_attr)) {
       ret = PyObject_RichCompareBool(name_attr, name, Py_EQ);
   } else {
       ret = -1;
@@ -33230,15 +33253,15 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* SetVTable */
-static int __Pyx_SetVtable(PyObject *dict, void *vtable) {
+  static int __Pyx_SetVtable(PyObject *dict, void *vtable) {
 #if PY_VERSION_HEX >= 0x02070000
     PyObject *ob = PyCapsule_New(vtable, 0, 0);
 #else
     PyObject *ob = PyCObject_FromVoidPtr(vtable, 0);
 #endif
     if (!ob)
         goto bad;
@@ -33248,76 +33271,94 @@
     return 0;
 bad:
     Py_XDECREF(ob);
     return -1;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
 bad:
     Py_XDECREF(result);
     return NULL;
 }
 #endif
 
 /* Import */
-static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
+  static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
     PyObject *empty_list = 0;
     PyObject *module = 0;
     PyObject *global_dict = 0;
     PyObject *empty_dict = 0;
     PyObject *list;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_import;
@@ -33374,29 +33415,29 @@
     #endif
     Py_XDECREF(empty_list);
     Py_XDECREF(empty_dict);
     return module;
 }
 
 /* ImportFrom */
-static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name) {
+  static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name) {
     PyObject* value = __Pyx_PyObject_GetAttrStr(module, name);
     if (unlikely(!value) && PyErr_ExceptionMatches(PyExc_AttributeError)) {
         PyErr_Format(PyExc_ImportError,
         #if PY_MAJOR_VERSION < 3
             "cannot import name %.230s", PyString_AS_STRING(name));
         #else
             "cannot import name %S", name);
         #endif
     }
     return value;
 }
 
 /* CalculateMetaclass */
-static PyObject *__Pyx_CalculateMetaclass(PyTypeObject *metaclass, PyObject *bases) {
+  static PyObject *__Pyx_CalculateMetaclass(PyTypeObject *metaclass, PyObject *bases) {
     Py_ssize_t i, nbases = PyTuple_GET_SIZE(bases);
     for (i=0; i < nbases; i++) {
         PyTypeObject *tmptype;
         PyObject *tmp = PyTuple_GET_ITEM(bases, i);
         tmptype = Py_TYPE(tmp);
 #if PY_MAJOR_VERSION < 3
         if (tmptype == &PyClass_Type)
@@ -33427,15 +33468,15 @@
 #endif
     }
     Py_INCREF((PyObject*) metaclass);
     return (PyObject*) metaclass;
 }
 
 /* Py3ClassCreate */
-static PyObject *__Pyx_Py3MetaclassPrepare(PyObject *metaclass, PyObject *bases, PyObject *name,
+  static PyObject *__Pyx_Py3MetaclassPrepare(PyObject *metaclass, PyObject *bases, PyObject *name,
                                            PyObject *qualname, PyObject *mkw, PyObject *modname, PyObject *doc) {
     PyObject *ns;
     if (metaclass) {
         PyObject *prep = __Pyx_PyObject_GetAttrStr(metaclass, __pyx_n_s_prepare);
         if (prep) {
             PyObject *pargs = PyTuple_Pack(2, name, bases);
             if (unlikely(!pargs)) {
@@ -33494,15 +33535,15 @@
         Py_DECREF(margs);
     }
     Py_XDECREF(owned_metaclass);
     return result;
 }
 
 /* CyFunctionClassCell */
-static int __Pyx_CyFunction_InitClassCell(PyObject *cyfunctions, PyObject *classobj) {
+  static int __Pyx_CyFunction_InitClassCell(PyObject *cyfunctions, PyObject *classobj) {
     Py_ssize_t i, count = PyList_GET_SIZE(cyfunctions);
     for (i = 0; i < count; i++) {
         __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *)
 #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
             PyList_GET_ITEM(cyfunctions, i);
 #else
             PySequence_ITEM(cyfunctions, i);
@@ -33515,15 +33556,15 @@
         Py_DECREF((PyObject*)m);
 #endif
     }
     return 0;
 }
 
 /* CLineInTraceback */
-#ifndef CYTHON_CLINE_IN_TRACEBACK
+  #ifndef CYTHON_CLINE_IN_TRACEBACK
 static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
@@ -33557,15 +33598,15 @@
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
 #endif
 
 /* CodeObjectCache */
-static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
+  static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
     int start = 0, mid = 0, end = count - 1;
     if (end >= 0 && code_line > entries[end].code_line) {
         return count;
     }
     while (start < end) {
         mid = start + (end - start) / 2;
         if (code_line < entries[mid].code_line) {
@@ -33637,15 +33678,15 @@
     entries[pos].code_line = code_line;
     entries[pos].code_object = code_object;
     __pyx_code_cache.count++;
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
-#include "compile.h"
+  #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
 #if PY_VERSION_HEX >= 0x030b00a6
   #ifndef Py_BUILD_CORE
     #define Py_BUILD_CORE 1
   #endif
   #include "internal/pycore_frame.h"
@@ -33744,15 +33785,15 @@
     PyTraceBack_Here(py_frame);
 bad:
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
 
 /* CIntFromPyVerify */
-#define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
+  #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
 #define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
 #define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
     {\
         func_type value = func_value;\
         if (sizeof(target_type) < sizeof(func_type)) {\
@@ -33766,15 +33807,15 @@
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
 /* CIntFromPy */
-static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
+  static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -33825,15 +33866,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -33962,15 +34003,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -34000,15 +34041,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -34038,15 +34079,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_long(unsigned long value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_long(unsigned long value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const unsigned long neg_one = (unsigned long) -1, const_zero = (unsigned long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -34076,15 +34117,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(unsigned long),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_curl_socket_t(curl_socket_t value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_curl_socket_t(curl_socket_t value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const curl_socket_t neg_one = (curl_socket_t) -1, const_zero = (curl_socket_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -34114,15 +34155,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(curl_socket_t),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_CURLcode(CURLcode value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_CURLcode(CURLcode value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const CURLcode neg_one = (CURLcode) -1, const_zero = (CURLcode) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -34152,15 +34193,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(CURLcode),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
+  static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -34211,15 +34252,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -34348,15 +34389,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to long");
     return (long) -1;
 }
 
 /* FastTypeChecks */
-#if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
         a = a->tp_base;
         if (a == b)
             return 1;
     }
     return b == &PyBaseObject_Type;
@@ -34448,15 +34489,15 @@
         return __Pyx_inner_PyErr_GivenExceptionMatches2(err, exc_type1, exc_type2);
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* Generator */
-static PyMethodDef __pyx_Generator_methods[] = {
+  static PyMethodDef __pyx_Generator_methods[] = {
     {"send", (PyCFunction) __Pyx_Coroutine_Send, METH_O,
      (char*) PyDoc_STR("send(arg) -> send 'arg' into generator,\nreturn next yielded value or raise StopIteration.")},
     {"throw", (PyCFunction) __Pyx_Coroutine_Throw, METH_VARARGS,
      (char*) PyDoc_STR("throw(typ[,val[,tb]]) -> raise exception in generator,\nreturn next yielded value or raise StopIteration.")},
     {"close", (PyCFunction) __Pyx_Coroutine_Close_Method, METH_NOARGS,
      (char*) PyDoc_STR("close() -> raise GeneratorExit inside generator.")},
     {0, 0, 0, 0}
@@ -34536,30 +34577,33 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_Generator_init(void) {
     __pyx_GeneratorType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_GeneratorType_type.tp_iter = PyObject_SelfIter;
     __pyx_GeneratorType = __Pyx_FetchCommonType(&__pyx_GeneratorType_type);
     if (unlikely(!__pyx_GeneratorType)) {
         return -1;
     }
     return 0;
 }
 
 /* CheckBinaryVersion */
-static int __Pyx_check_binary_version(void) {
+  static int __Pyx_check_binary_version(void) {
     char ctversion[5];
     int same=1, i, found_dot;
     const char* rt_from_call = Py_GetVersion();
     PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
     found_dot = 0;
     for (i = 0; i < 4; i++) {
         if (!ctversion[i]) {
@@ -34589,15 +34633,15 @@
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
 /* InitStrings */
-static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
+  static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
     while (t->p) {
         #if PY_MAJOR_VERSION < 3
         if (t->is_unicode) {
             *t->p = PyUnicode_DecodeUTF8(t->s, t->n - 1, NULL);
         } else if (t->intern) {
             *t->p = PyString_InternFromString(t->s);
         } else {
```

### Comparing `acurl-1.0.5/src/acurl.pyx` & `acurl-1.0.6/src/acurl.pyx`

 * *Files identical despite different names*

### Comparing `acurl-1.0.5/src/acurl_wrappers.h` & `acurl-1.0.6/src/acurl_wrappers.h`

 * *Files identical despite different names*

### Comparing `acurl-1.0.5/src/cookie.pyx` & `acurl-1.0.6/src/cookie.pyx`

 * *Files identical despite different names*

### Comparing `acurl-1.0.5/src/curlinterface.pxd` & `acurl-1.0.6/src/curlinterface.pxd`

 * *Files identical despite different names*

### Comparing `acurl-1.0.5/src/request.pyx` & `acurl-1.0.6/src/request.pyx`

 * *Files identical despite different names*

### Comparing `acurl-1.0.5/src/response.pyx` & `acurl-1.0.6/src/response.pyx`

 * *Files identical despite different names*

### Comparing `acurl-1.0.5/src/session.pyx` & `acurl-1.0.6/src/session.pyx`

 * *Files identical despite different names*

### Comparing `acurl-1.0.5/src/utils.pyx` & `acurl-1.0.6/src/utils.pyx`

 * *Files identical despite different names*

### Comparing `acurl-1.0.5/tests/test_acurl.py` & `acurl-1.0.6/tests/test_acurl.py`

 * *Files identical despite different names*

### Comparing `acurl-1.0.5/tests/test_cookie.py` & `acurl-1.0.6/tests/test_cookie.py`

 * *Files identical despite different names*

### Comparing `acurl-1.0.5/tests/test_httpbin.py` & `acurl-1.0.6/tests/test_httpbin.py`

 * *Files identical despite different names*

### Comparing `acurl-1.0.5/tests/test_request.py` & `acurl-1.0.6/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `acurl-1.0.5/tests/test_response.py` & `acurl-1.0.6/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `acurl-1.0.5/tests/test_session.py` & `acurl-1.0.6/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `acurl-1.0.5/tests/test_to_curl.py` & `acurl-1.0.6/tests/test_to_curl.py`

 * *Files identical despite different names*

### Comparing `acurl-1.0.5/tests/test_utils.py` & `acurl-1.0.6/tests/test_utils.py`

 * *Files identical despite different names*

