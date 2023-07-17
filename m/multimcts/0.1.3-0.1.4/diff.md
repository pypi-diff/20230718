# Comparing `tmp/multimcts-0.1.3.tar.gz` & `tmp/multimcts-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multimcts-0.1.3.tar", last modified: Mon Jul 17 19:25:38 2023, max compression
+gzip compressed data, was "multimcts-0.1.4.tar", last modified: Mon Jul 17 23:05:38 2023, max compression
```

## Comparing `multimcts-0.1.3.tar` & `multimcts-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-17 19:25:38.240318 multimcts-0.1.3/
--rw-r--r--   0 taylorvance   (501) staff       (20)      228 2023-07-17 19:25:38.240165 multimcts-0.1.3/PKG-INFO
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-17 19:25:38.237741 multimcts-0.1.3/multimcts/
--rw-r--r--   0 taylorvance   (501) staff       (20)       56 2023-07-17 17:45:55.000000 multimcts-0.1.3/multimcts/__init__.py
--rw-r--r--   0 taylorvance   (501) staff       (20)   257682 2023-07-17 17:46:23.000000 multimcts-0.1.3/multimcts/gamestate.c
--rw-r--r--   0 taylorvance   (501) staff       (20)   434959 2023-07-17 17:46:23.000000 multimcts-0.1.3/multimcts/mcts.c
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-17 19:25:38.239904 multimcts-0.1.3/multimcts.egg-info/
--rw-r--r--   0 taylorvance   (501) staff       (20)      228 2023-07-17 19:25:38.000000 multimcts-0.1.3/multimcts.egg-info/PKG-INFO
--rw-r--r--   0 taylorvance   (501) staff       (20)      248 2023-07-17 19:25:38.000000 multimcts-0.1.3/multimcts.egg-info/SOURCES.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-17 19:25:38.000000 multimcts-0.1.3/multimcts.egg-info/dependency_links.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-17 19:12:04.000000 multimcts-0.1.3/multimcts.egg-info/not-zip-safe
--rw-r--r--   0 taylorvance   (501) staff       (20)       10 2023-07-17 19:25:38.000000 multimcts-0.1.3/multimcts.egg-info/top_level.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)      100 2023-07-17 18:23:36.000000 multimcts-0.1.3/pyproject.toml
--rw-r--r--   0 taylorvance   (501) staff       (20)       38 2023-07-17 19:25:38.240387 multimcts-0.1.3/setup.cfg
--rw-r--r--   0 taylorvance   (501) staff       (20)      567 2023-07-17 19:25:25.000000 multimcts-0.1.3/setup.py
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-17 23:05:38.927591 multimcts-0.1.4/
+-rw-r--r--   0 taylorvance   (501) staff       (20)       24 2023-07-17 19:47:43.000000 multimcts-0.1.4/MANIFEST.in
+-rw-r--r--   0 taylorvance   (501) staff       (20)      228 2023-07-17 23:05:38.927327 multimcts-0.1.4/PKG-INFO
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-17 23:05:38.926192 multimcts-0.1.4/multimcts/
+-rw-r--r--   0 taylorvance   (501) staff       (20)       34 2023-07-17 20:09:40.000000 multimcts-0.1.4/multimcts/__init__.py
+-rw-r--r--   0 taylorvance   (501) staff       (20)   508596 2023-07-17 23:05:38.000000 multimcts-0.1.4/multimcts/mcts.c
+-rw-r--r--   0 taylorvance   (501) staff       (20)     9301 2023-07-17 20:09:14.000000 multimcts-0.1.4/multimcts/mcts.pyx
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-17 23:05:38.927055 multimcts-0.1.4/multimcts.egg-info/
+-rw-r--r--   0 taylorvance   (501) staff       (20)      228 2023-07-17 23:05:38.000000 multimcts-0.1.4/multimcts.egg-info/PKG-INFO
+-rw-r--r--   0 taylorvance   (501) staff       (20)      257 2023-07-17 23:05:38.000000 multimcts-0.1.4/multimcts.egg-info/SOURCES.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-17 23:05:38.000000 multimcts-0.1.4/multimcts.egg-info/dependency_links.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-17 23:05:38.000000 multimcts-0.1.4/multimcts.egg-info/not-zip-safe
+-rw-r--r--   0 taylorvance   (501) staff       (20)       10 2023-07-17 23:05:38.000000 multimcts-0.1.4/multimcts.egg-info/top_level.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)      100 2023-07-17 18:23:36.000000 multimcts-0.1.4/pyproject.toml
+-rw-r--r--   0 taylorvance   (501) staff       (20)       38 2023-07-17 23:05:38.927703 multimcts-0.1.4/setup.cfg
+-rw-r--r--   0 taylorvance   (501) staff       (20)      424 2023-07-17 23:05:11.000000 multimcts-0.1.4/setup.py
```

### Comparing `multimcts-0.1.3/multimcts/mcts.c` & `multimcts-0.1.4/multimcts/mcts.c`

 * *Files 10% similar despite different names*

```diff
@@ -973,28 +973,28 @@
   "multimcts/mcts.pyx",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child;
 struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct_1_genexpr;
 
-/* "multimcts/mcts.pyx":164
+/* "multimcts/mcts.pyx":211
  *             node = node.parent
  * 
  *     def get_best_child(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         cur_team = node.state.get_current_team()
  *         cdef float ln_parent_visits = log(node.num_visits)
  */
 struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child {
   PyObject_HEAD
   PyObject *__pyx_v_child;
 };
 
 
-/* "multimcts/mcts.pyx":177
+/* "multimcts/mcts.pyx":224
  *         for child in node.children.values():
  *             # Relative reward is this child's reward minus its siblings' rewards.
  *             reward = (2 * child.total_reward[cur_team]) - sum(x for x in child.total_reward.values())             # <<<<<<<<<<<<<<
  *             visits = child.num_visits
  * 
  */
 struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct_1_genexpr {
@@ -1077,81 +1077,75 @@
 #else
 #define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
 #endif
 
 /* GetBuiltinName.proto */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name);
 
-/* RaiseArgTupleInvalid.proto */
-static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
-    Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
+/* PyObjectCall.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
+#else
+#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
+#endif
+
+/* PyThreadStateGet.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
+#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
+#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
+#else
+#define __Pyx_PyThreadState_declare
+#define __Pyx_PyThreadState_assign
+#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
+#endif
+
+/* PyErrFetchRestore.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
+#else
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#endif
+#else
+#define __Pyx_PyErr_Clear() PyErr_Clear()
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
+#endif
+
+/* RaiseException.proto */
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
 /* RaiseDoubleKeywords.proto */
 static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
 
 /* ParseKeywords.proto */
 static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
     PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
     const char* function_name);
 
-/* PyObjectSetAttrStr.proto */
-#if CYTHON_USE_TYPE_SLOTS
-#define __Pyx_PyObject_DelAttrStr(o,n) __Pyx_PyObject_SetAttrStr(o, n, NULL)
-static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value);
-#else
-#define __Pyx_PyObject_DelAttrStr(o,n)   PyObject_DelAttr(o,n)
-#define __Pyx_PyObject_SetAttrStr(o,n,v) PyObject_SetAttr(o,n,v)
-#endif
-
-/* PyDictVersioning.proto */
-#if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
-#define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
-#define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
-#define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
-    (version_var) = __PYX_GET_DICT_VERSION(dict);\
-    (cache_var) = (value);
-#define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP) {\
-    static PY_UINT64_T __pyx_dict_version = 0;\
-    static PyObject *__pyx_dict_cached_value = NULL;\
-    if (likely(__PYX_GET_DICT_VERSION(DICT) == __pyx_dict_version)) {\
-        (VAR) = __pyx_dict_cached_value;\
-    } else {\
-        (VAR) = __pyx_dict_cached_value = (LOOKUP);\
-        __pyx_dict_version = __PYX_GET_DICT_VERSION(DICT);\
-    }\
-}
-static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj);
-static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj);
-static CYTHON_INLINE int __Pyx_object_dict_version_matches(PyObject* obj, PY_UINT64_T tp_dict_version, PY_UINT64_T obj_dict_version);
-#else
-#define __PYX_GET_DICT_VERSION(dict)  (0)
-#define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
-#define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
-#endif
+/* RaiseArgTupleInvalid.proto */
+static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
+    Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
-/* GetModuleGlobalName.proto */
-#if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  do {\
-    static PY_UINT64_T __pyx_dict_version = 0;\
-    static PyObject *__pyx_dict_cached_value = NULL;\
-    (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
-        (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
-        __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-} while(0)
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
-    PY_UINT64_T __pyx_dict_version;\
-    PyObject *__pyx_dict_cached_value;\
-    (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-} while(0)
-static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
-#else
-#define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
-static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
-#endif
+/* IterNext.proto */
+#define __Pyx_PyIter_Next(obj) __Pyx_PyIter_Next2(obj, NULL)
+static CYTHON_INLINE PyObject *__Pyx_PyIter_Next2(PyObject *, PyObject *);
 
 /* PyCFunctionFastCall.proto */
 #if CYTHON_FAST_PYCCALL
 static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
 #else
 #define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
 #endif
@@ -1183,21 +1177,14 @@
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
 #endif // CYTHON_FAST_PYCALL
 #endif
 
-/* PyObjectCall.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
-#else
-#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
-#endif
-
 /* PyObjectCall2Args.proto */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
 
 /* PyObjectCallMethO.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
 #endif
@@ -1208,52 +1195,101 @@
 /* PyObjectCallNoArg.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
 #else
 #define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
 #endif
 
-/* PyThreadStateGet.proto */
+/* GetTopmostException.proto */
+#if CYTHON_USE_EXC_INFO_STACK
+static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
+#endif
+
+/* SaveResetException.proto */
 #if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
-#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
-#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
+#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
 #else
-#define __Pyx_PyThreadState_declare
-#define __Pyx_PyThreadState_assign
-#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
+#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
+#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
 #endif
 
-/* PyErrFetchRestore.proto */
+/* PyErrExceptionMatches.proto */
 #if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#if CYTHON_COMPILING_IN_CPYTHON
-#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
+#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
 #else
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
 #endif
+
+/* GetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #else
-#define __Pyx_PyErr_Clear() PyErr_Clear()
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
 #endif
 
-/* RaiseException.proto */
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
+/* PyObjectSetAttrStr.proto */
+#if CYTHON_USE_TYPE_SLOTS
+#define __Pyx_PyObject_DelAttrStr(o,n) __Pyx_PyObject_SetAttrStr(o, n, NULL)
+static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value);
+#else
+#define __Pyx_PyObject_DelAttrStr(o,n)   PyObject_DelAttr(o,n)
+#define __Pyx_PyObject_SetAttrStr(o,n,v) PyObject_SetAttr(o,n,v)
+#endif
+
+/* PyDictVersioning.proto */
+#if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
+#define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
+#define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
+#define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
+    (version_var) = __PYX_GET_DICT_VERSION(dict);\
+    (cache_var) = (value);
+#define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP) {\
+    static PY_UINT64_T __pyx_dict_version = 0;\
+    static PyObject *__pyx_dict_cached_value = NULL;\
+    if (likely(__PYX_GET_DICT_VERSION(DICT) == __pyx_dict_version)) {\
+        (VAR) = __pyx_dict_cached_value;\
+    } else {\
+        (VAR) = __pyx_dict_cached_value = (LOOKUP);\
+        __pyx_dict_version = __PYX_GET_DICT_VERSION(DICT);\
+    }\
+}
+static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj);
+static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj);
+static CYTHON_INLINE int __Pyx_object_dict_version_matches(PyObject* obj, PY_UINT64_T tp_dict_version, PY_UINT64_T obj_dict_version);
+#else
+#define __PYX_GET_DICT_VERSION(dict)  (0)
+#define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
+#define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
+#endif
+
+/* GetModuleGlobalName.proto */
+#if CYTHON_USE_DICT_VERSIONS
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
+    static PY_UINT64_T __pyx_dict_version = 0;\
+    static PyObject *__pyx_dict_cached_value = NULL;\
+    (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
+        (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
+        __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
+    PY_UINT64_T __pyx_dict_version;\
+    PyObject *__pyx_dict_cached_value;\
+    (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
+} while(0)
+static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
+#else
+#define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
+static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
+#endif
 
 /* None.proto */
 static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname);
 
 /* PyIntBinop.proto */
 #if !CYTHON_COMPILING_IN_PYPY
 static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
@@ -1304,46 +1340,14 @@
                ((cfunc)->flag == METH_VARARGS ?  (*((cfunc)->func))(self, __pyx_empty_tuple) :\
                __Pyx__CallUnboundCMethod0(cfunc, self)))))) :\
         __Pyx__CallUnboundCMethod0(cfunc, self))
 #else
 #define __Pyx_CallUnboundCMethod0(cfunc, self)  __Pyx__CallUnboundCMethod0(cfunc, self)
 #endif
 
-/* GetTopmostException.proto */
-#if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
-#endif
-
-/* SaveResetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-#else
-#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
-#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
-#endif
-
-/* PyErrExceptionMatches.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
-#else
-#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
-#endif
-
-/* GetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
-#endif
-
 /* ArgTypeTest.proto */
 #define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
     ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
 /* py_dict_items.proto */
@@ -1697,45 +1701,51 @@
 static PyTypeObject *__pyx_ptype_9multimcts_4mcts___pyx_scope_struct_1_genexpr = 0;
 #define __Pyx_MODULE_NAME "multimcts.mcts"
 extern int __pyx_module_is_main_multimcts__mcts;
 int __pyx_module_is_main_multimcts__mcts = 0;
 
 /* Implementation of 'multimcts.mcts' */
 static PyObject *__pyx_builtin_staticmethod;
+static PyObject *__pyx_builtin_NotImplementedError;
+static PyObject *__pyx_builtin_StopIteration;
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_IndexError;
 static PyObject *__pyx_builtin_sum;
 static const char __pyx_k_i[] = "i";
 static const char __pyx_k_k[] = "k";
 static const char __pyx_k_v[] = "v";
+static const char __pyx_k_eq[] = "__eq__";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_inf[] = "-inf";
 static const char __pyx_k_int[] = "int";
 static const char __pyx_k_key[] = "key";
 static const char __pyx_k_pop[] = "pop";
 static const char __pyx_k_sum[] = "sum";
 static const char __pyx_k_Dict[] = "Dict";
 static const char __pyx_k_MCTS[] = "MCTS";
 static const char __pyx_k_Node[] = "Node";
 static const char __pyx_k_args[] = "args";
 static const char __pyx_k_best[] = "best";
 static const char __pyx_k_dict[] = "dict";
+static const char __pyx_k_hash[] = "__hash__";
 static const char __pyx_k_init[] = "__init__";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_move[] = "move";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_node[] = "node";
 static const char __pyx_k_self[] = "self";
 static const char __pyx_k_send[] = "send";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_time[] = "time";
+static const char __pyx_k_Union[] = "Union";
 static const char __pyx_k_child[] = "child";
 static const char __pyx_k_close[] = "close";
 static const char __pyx_k_float[] = "float";
 static const char __pyx_k_items[] = "items";
+static const char __pyx_k_other[] = "other";
 static const char __pyx_k_score[] = "score";
 static const char __pyx_k_state[] = "state";
 static const char __pyx_k_throw[] = "throw";
 static const char __pyx_k_expand[] = "expand";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_module[] = "__module__";
 static const char __pyx_k_parent[] = "parent";
@@ -1745,26 +1755,28 @@
 static const char __pyx_k_select[] = "select";
 static const char __pyx_k_typing[] = "typing";
 static const char __pyx_k_values[] = "values";
 static const char __pyx_k_visits[] = "visits";
 static const char __pyx_k_genexpr[] = "genexpr";
 static const char __pyx_k_prepare[] = "__prepare__";
 static const char __pyx_k_Hashable[] = "Hashable";
+static const char __pyx_k_Iterator[] = "Iterator";
 static const char __pyx_k_children[] = "children";
 static const char __pyx_k_cur_team[] = "cur_team";
 static const char __pyx_k_end_time[] = "end_time";
+static const char __pyx_k_has_move[] = "has_move";
 static const char __pyx_k_max_time[] = "max_time";
 static const char __pyx_k_qualname[] = "__qualname__";
 static const char __pyx_k_simulate[] = "simulate";
 static const char __pyx_k_GameState[] = "GameState";
-static const char __pyx_k_gamestate[] = "gamestate";
 static const char __pyx_k_heuristic[] = "heuristic";
 static const char __pyx_k_make_move[] = "make_move";
 static const char __pyx_k_max_score[] = "max_score";
 static const char __pyx_k_metaclass[] = "__metaclass__";
+static const char __pyx_k_randomize[] = "randomize";
 static const char __pyx_k_IndexError[] = "IndexError";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_get_reward[] = "get_reward";
 static const char __pyx_k_num_visits[] = "num_visits";
 static const char __pyx_k_MCTS___init[] = "MCTS.__init__";
 static const char __pyx_k_MCTS_expand[] = "MCTS.expand";
 static const char __pyx_k_MCTS_search[] = "MCTS.search";
@@ -1772,78 +1784,118 @@
 static const char __pyx_k_Node___init[] = "Node.__init__";
 static const char __pyx_k_collections[] = "collections";
 static const char __pyx_k_defaultdict[] = "defaultdict";
 static const char __pyx_k_is_terminal[] = "is_terminal";
 static const char __pyx_k_staticmethod[] = "staticmethod";
 static const char __pyx_k_total_reward[] = "total_reward";
 static const char __pyx_k_MCTS_simulate[] = "MCTS.simulate";
+static const char __pyx_k_StopIteration[] = "StopIteration";
 static const char __pyx_k_backpropagate[] = "backpropagate";
 static const char __pyx_k_terminal_team[] = "terminal_team";
+static const char __pyx_k_GameState___eq[] = "GameState.__eq__";
 static const char __pyx_k_get_best_child[] = "get_best_child";
 static const char __pyx_k_max_iterations[] = "max_iterations";
 static const char __pyx_k_multimcts_mcts[] = "multimcts.mcts";
 static const char __pyx_k_get_legal_moves[] = "get_legal_moves";
 static const char __pyx_k_get_random_move[] = "get_random_move";
 static const char __pyx_k_remaining_moves[] = "remaining_moves";
+static const char __pyx_k_GameState___hash[] = "GameState.__hash__";
 static const char __pyx_k_exploration_bias[] = "exploration_bias";
 static const char __pyx_k_get_current_team[] = "get_current_team";
 static const char __pyx_k_ln_parent_visits[] = "ln_parent_visits";
 static const char __pyx_k_is_fully_expanded[] = "is_fully_expanded";
+static const char __pyx_k_GameState_has_move[] = "GameState.has_move";
 static const char __pyx_k_MCTS_backpropagate[] = "MCTS.backpropagate";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_multimcts_mcts_pyx[] = "multimcts/mcts.pyx";
+static const char __pyx_k_GameState_make_move[] = "GameState.make_move";
 static const char __pyx_k_MCTS_get_best_child[] = "MCTS.get_best_child";
+static const char __pyx_k_NotImplementedError[] = "NotImplementedError";
+static const char __pyx_k_GameState_get_reward[] = "GameState.get_reward";
+static const char __pyx_k_GameState_is_terminal[] = "GameState.is_terminal";
+static const char __pyx_k_GameState_get_legal_moves[] = "GameState.get_legal_moves";
+static const char __pyx_k_GameState_get_random_move[] = "GameState.get_random_move";
+static const char __pyx_k_GameState_get_current_team[] = "GameState.get_current_team";
+static const char __pyx_k_GameStates_must_implement___eq[] = "GameStates must implement __eq__";
+static const char __pyx_k_GameState_must_implement___hash[] = "GameState must implement __hash__";
 static const char __pyx_k_Non_terminal_state_has_no_legal[] = "Non-terminal state has no legal moves.";
 static const char __pyx_k_Represents_a_game_state_node_in[] = "Represents a game state node in the MCTS search tree.\n\n    Args:\n        state (GameState): The game state at the current node.\n        parent (Node): The parent of the current node in the search tree.\n\n    Attributes:\n        children (dict): The children of the current node in the search tree. Keys are moves; values are Nodes.\n        num_visits (int): The number of times the node has been visited.\n        total_reward (dict): The total reward obtained from simulations through the node. Keys are teams; values are rewards.\n        is_terminal (bool): Whether the node represents a terminal state.\n        is_fully_expanded (bool): Whether all children of the node have been visited.\n        remaining_moves (list): A list of moves that have not yet been tried.\n    ";
+static const char __pyx_k_GameState_must_implement_get_cur[] = "GameState must implement get_current_team.";
+static const char __pyx_k_GameState_must_implement_get_leg[] = "GameState must implement get_legal_moves.";
+static const char __pyx_k_GameState_must_implement_get_rew[] = "GameState must implement get_reward.";
+static const char __pyx_k_GameState_must_implement_is_term[] = "GameState must implement is_terminal.";
+static const char __pyx_k_GameState_must_implement_make_mo[] = "GameState must implement make_move.";
 static const char __pyx_k_MCTS_get_best_child_locals_genex[] = "MCTS.get_best_child.<locals>.genexpr";
 static const char __pyx_k_One_or_more_of_max_time_max_iter[] = "One or more of max_time/max_iterations is required.";
 static const char __pyx_k_Tried_to_expand_a_fully_expanded[] = "Tried to expand a fully-expanded or terminal node.";
 static PyObject *__pyx_n_s_Dict;
 static PyObject *__pyx_n_s_GameState;
+static PyObject *__pyx_n_s_GameState___eq;
+static PyObject *__pyx_n_s_GameState___hash;
+static PyObject *__pyx_n_s_GameState_get_current_team;
+static PyObject *__pyx_n_s_GameState_get_legal_moves;
+static PyObject *__pyx_n_s_GameState_get_random_move;
+static PyObject *__pyx_n_s_GameState_get_reward;
+static PyObject *__pyx_n_s_GameState_has_move;
+static PyObject *__pyx_n_s_GameState_is_terminal;
+static PyObject *__pyx_n_s_GameState_make_move;
+static PyObject *__pyx_kp_s_GameState_must_implement___hash;
+static PyObject *__pyx_kp_s_GameState_must_implement_get_cur;
+static PyObject *__pyx_kp_s_GameState_must_implement_get_leg;
+static PyObject *__pyx_kp_s_GameState_must_implement_get_rew;
+static PyObject *__pyx_kp_s_GameState_must_implement_is_term;
+static PyObject *__pyx_kp_s_GameState_must_implement_make_mo;
+static PyObject *__pyx_kp_s_GameStates_must_implement___eq;
 static PyObject *__pyx_n_s_Hashable;
 static PyObject *__pyx_n_s_IndexError;
+static PyObject *__pyx_n_s_Iterator;
 static PyObject *__pyx_n_s_MCTS;
 static PyObject *__pyx_n_s_MCTS___init;
 static PyObject *__pyx_n_s_MCTS_backpropagate;
 static PyObject *__pyx_n_s_MCTS_expand;
 static PyObject *__pyx_n_s_MCTS_get_best_child;
 static PyObject *__pyx_n_s_MCTS_get_best_child_locals_genex;
 static PyObject *__pyx_n_s_MCTS_search;
 static PyObject *__pyx_n_s_MCTS_select;
 static PyObject *__pyx_n_s_MCTS_simulate;
 static PyObject *__pyx_n_s_Node;
 static PyObject *__pyx_n_s_Node___init;
 static PyObject *__pyx_kp_s_Non_terminal_state_has_no_legal;
+static PyObject *__pyx_n_s_NotImplementedError;
 static PyObject *__pyx_kp_s_One_or_more_of_max_time_max_iter;
 static PyObject *__pyx_kp_s_Represents_a_game_state_node_in;
+static PyObject *__pyx_n_s_StopIteration;
 static PyObject *__pyx_kp_s_Tried_to_expand_a_fully_expanded;
+static PyObject *__pyx_n_s_Union;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_args;
 static PyObject *__pyx_n_s_backpropagate;
 static PyObject *__pyx_n_s_best;
 static PyObject *__pyx_n_s_child;
 static PyObject *__pyx_n_s_children;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_close;
 static PyObject *__pyx_n_s_collections;
 static PyObject *__pyx_n_s_cur_team;
 static PyObject *__pyx_n_s_defaultdict;
 static PyObject *__pyx_n_u_dict;
 static PyObject *__pyx_n_s_doc;
 static PyObject *__pyx_n_s_end_time;
+static PyObject *__pyx_n_s_eq;
 static PyObject *__pyx_n_s_expand;
 static PyObject *__pyx_n_s_exploration_bias;
 static PyObject *__pyx_n_u_float;
-static PyObject *__pyx_n_s_gamestate;
 static PyObject *__pyx_n_s_genexpr;
 static PyObject *__pyx_n_s_get_best_child;
 static PyObject *__pyx_n_s_get_current_team;
 static PyObject *__pyx_n_s_get_legal_moves;
 static PyObject *__pyx_n_s_get_random_move;
 static PyObject *__pyx_n_s_get_reward;
+static PyObject *__pyx_n_s_has_move;
+static PyObject *__pyx_n_s_hash;
 static PyObject *__pyx_n_s_heuristic;
 static PyObject *__pyx_n_s_i;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_kp_s_inf;
 static PyObject *__pyx_n_s_init;
 static PyObject *__pyx_n_u_int;
 static PyObject *__pyx_n_s_is_fully_expanded;
@@ -1861,18 +1913,20 @@
 static PyObject *__pyx_n_s_module;
 static PyObject *__pyx_n_s_move;
 static PyObject *__pyx_n_s_multimcts_mcts;
 static PyObject *__pyx_kp_s_multimcts_mcts_pyx;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_node;
 static PyObject *__pyx_n_s_num_visits;
+static PyObject *__pyx_n_s_other;
 static PyObject *__pyx_n_s_parent;
 static PyObject *__pyx_n_s_pop;
 static PyObject *__pyx_n_s_prepare;
 static PyObject *__pyx_n_s_qualname;
+static PyObject *__pyx_n_s_randomize;
 static PyObject *__pyx_n_s_remaining_moves;
 static PyObject *__pyx_n_s_return;
 static PyObject *__pyx_n_s_reward;
 static PyObject *__pyx_n_s_score;
 static PyObject *__pyx_n_s_search;
 static PyObject *__pyx_n_s_select;
 static PyObject *__pyx_n_s_self;
@@ -1886,14 +1940,23 @@
 static PyObject *__pyx_n_s_throw;
 static PyObject *__pyx_n_s_time;
 static PyObject *__pyx_n_s_total_reward;
 static PyObject *__pyx_n_s_typing;
 static PyObject *__pyx_n_s_v;
 static PyObject *__pyx_n_s_values;
 static PyObject *__pyx_n_s_visits;
+static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_get_current_team(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_2get_legal_moves(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_randomize); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_4get_random_move(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_6has_move(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_8make_move(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_move); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_10is_terminal(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_12get_reward(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_14__hash__(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_16__eq__(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_other); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_4Node___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_state, PyObject *__pyx_v_parent); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, double __pyx_v_exploration_bias, PyObject *__pyx_v_heuristic, PyObject *__pyx_v_max_time, PyObject *__pyx_v_max_iterations); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_2search(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_state); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_4select(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_node); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_6expand(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_node); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_8simulate(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_node); /* proto */
 static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_10backpropagate(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_node, PyObject *__pyx_v_reward); /* proto */
@@ -1906,33 +1969,930 @@
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_2;
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
+static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_tuple__7;
+static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_tuple__9;
+static PyObject *__pyx_tuple__10;
 static PyObject *__pyx_tuple__11;
 static PyObject *__pyx_tuple__13;
 static PyObject *__pyx_tuple__15;
-static PyObject *__pyx_tuple__17;
-static PyObject *__pyx_tuple__19;
-static PyObject *__pyx_codeobj__5;
-static PyObject *__pyx_codeobj__8;
-static PyObject *__pyx_codeobj__10;
+static PyObject *__pyx_tuple__16;
+static PyObject *__pyx_tuple__18;
+static PyObject *__pyx_tuple__20;
+static PyObject *__pyx_tuple__22;
+static PyObject *__pyx_tuple__24;
+static PyObject *__pyx_tuple__26;
+static PyObject *__pyx_tuple__28;
+static PyObject *__pyx_tuple__30;
+static PyObject *__pyx_tuple__32;
+static PyObject *__pyx_tuple__33;
+static PyObject *__pyx_tuple__35;
+static PyObject *__pyx_tuple__37;
+static PyObject *__pyx_tuple__39;
+static PyObject *__pyx_tuple__41;
+static PyObject *__pyx_tuple__43;
+static PyObject *__pyx_tuple__45;
 static PyObject *__pyx_codeobj__12;
 static PyObject *__pyx_codeobj__14;
-static PyObject *__pyx_codeobj__16;
-static PyObject *__pyx_codeobj__18;
-static PyObject *__pyx_codeobj__20;
+static PyObject *__pyx_codeobj__17;
+static PyObject *__pyx_codeobj__19;
+static PyObject *__pyx_codeobj__21;
+static PyObject *__pyx_codeobj__23;
+static PyObject *__pyx_codeobj__25;
+static PyObject *__pyx_codeobj__27;
+static PyObject *__pyx_codeobj__29;
+static PyObject *__pyx_codeobj__31;
+static PyObject *__pyx_codeobj__34;
+static PyObject *__pyx_codeobj__36;
+static PyObject *__pyx_codeobj__38;
+static PyObject *__pyx_codeobj__40;
+static PyObject *__pyx_codeobj__42;
+static PyObject *__pyx_codeobj__44;
+static PyObject *__pyx_codeobj__46;
 /* Late includes */
 
-/* "multimcts/mcts.pyx":25
+/* "multimcts/mcts.pyx":9
+ * 
+ * class GameState():
+ *     def get_current_team(self) -> Union[int,str]:             # <<<<<<<<<<<<<<
+ *         """The identifier of the current player's team."""
+ *         raise NotImplementedError("GameState must implement get_current_team.")
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_1get_current_team(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
+static char __pyx_doc_9multimcts_4mcts_9GameState_get_current_team[] = "The identifier of the current player's team.";
+static PyMethodDef __pyx_mdef_9multimcts_4mcts_9GameState_1get_current_team = {"get_current_team", (PyCFunction)__pyx_pw_9multimcts_4mcts_9GameState_1get_current_team, METH_O, __pyx_doc_9multimcts_4mcts_9GameState_get_current_team};
+static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_1get_current_team(PyObject *__pyx_self, PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("get_current_team (wrapper)", 0);
+  __pyx_r = __pyx_pf_9multimcts_4mcts_9GameState_get_current_team(__pyx_self, ((PyObject *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_get_current_team(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("get_current_team", 0);
+
+  /* "multimcts/mcts.pyx":11
+ *     def get_current_team(self) -> Union[int,str]:
+ *         """The identifier of the current player's team."""
+ *         raise NotImplementedError("GameState must implement get_current_team.")             # <<<<<<<<<<<<<<
+ * 
+ *     def get_legal_moves(self, randomize:bool=False) -> Iterator[Hashable]:
+ */
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 11, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_Raise(__pyx_t_1, 0, 0, 0);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __PYX_ERR(0, 11, __pyx_L1_error)
+
+  /* "multimcts/mcts.pyx":9
+ * 
+ * class GameState():
+ *     def get_current_team(self) -> Union[int,str]:             # <<<<<<<<<<<<<<
+ *         """The identifier of the current player's team."""
+ *         raise NotImplementedError("GameState must implement get_current_team.")
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("multimcts.mcts.GameState.get_current_team", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "multimcts/mcts.pyx":13
+ *         raise NotImplementedError("GameState must implement get_current_team.")
+ * 
+ *     def get_legal_moves(self, randomize:bool=False) -> Iterator[Hashable]:             # <<<<<<<<<<<<<<
+ *         """An iterator of all legal moves in this state.
+ *         The randomize param instructs the method to yield moves in a random order.
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_3get_legal_moves(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_9multimcts_4mcts_9GameState_2get_legal_moves[] = "An iterator of all legal moves in this state.\n        The randomize param instructs the method to yield moves in a random order.\n        ";
+static PyMethodDef __pyx_mdef_9multimcts_4mcts_9GameState_3get_legal_moves = {"get_legal_moves", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_9GameState_3get_legal_moves, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_9GameState_2get_legal_moves};
+static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_3get_legal_moves(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  CYTHON_UNUSED PyObject *__pyx_v_self = 0;
+  CYTHON_UNUSED PyObject *__pyx_v_randomize = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("get_legal_moves (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_randomize,0};
+    PyObject* values[2] = {0,0};
+    values[1] = ((PyObject *)((PyObject *)Py_False));
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_randomize);
+          if (value) { values[1] = value; kw_args--; }
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_legal_moves") < 0)) __PYX_ERR(0, 13, __pyx_L3_error)
+      }
+    } else {
+      switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_self = values[0];
+    __pyx_v_randomize = values[1];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("get_legal_moves", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 13, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("multimcts.mcts.GameState.get_legal_moves", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_9multimcts_4mcts_9GameState_2get_legal_moves(__pyx_self, __pyx_v_self, __pyx_v_randomize);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_2get_legal_moves(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_randomize) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("get_legal_moves", 0);
+
+  /* "multimcts/mcts.pyx":17
+ *         The randomize param instructs the method to yield moves in a random order.
+ *         """
+ *         raise NotImplementedError("GameState must implement get_legal_moves.")             # <<<<<<<<<<<<<<
+ * 
+ *     def get_random_move(self) -> Hashable:
+ */
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_Raise(__pyx_t_1, 0, 0, 0);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __PYX_ERR(0, 17, __pyx_L1_error)
+
+  /* "multimcts/mcts.pyx":13
+ *         raise NotImplementedError("GameState must implement get_current_team.")
+ * 
+ *     def get_legal_moves(self, randomize:bool=False) -> Iterator[Hashable]:             # <<<<<<<<<<<<<<
+ *         """An iterator of all legal moves in this state.
+ *         The randomize param instructs the method to yield moves in a random order.
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("multimcts.mcts.GameState.get_legal_moves", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "multimcts/mcts.pyx":19
+ *         raise NotImplementedError("GameState must implement get_legal_moves.")
+ * 
+ *     def get_random_move(self) -> Hashable:             # <<<<<<<<<<<<<<
+ *         """Returns a random legal move from this state."""
+ *         return next(self.get_legal_moves(True))
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_5get_random_move(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
+static char __pyx_doc_9multimcts_4mcts_9GameState_4get_random_move[] = "Returns a random legal move from this state.";
+static PyMethodDef __pyx_mdef_9multimcts_4mcts_9GameState_5get_random_move = {"get_random_move", (PyCFunction)__pyx_pw_9multimcts_4mcts_9GameState_5get_random_move, METH_O, __pyx_doc_9multimcts_4mcts_9GameState_4get_random_move};
+static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_5get_random_move(PyObject *__pyx_self, PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("get_random_move (wrapper)", 0);
+  __pyx_r = __pyx_pf_9multimcts_4mcts_9GameState_4get_random_move(__pyx_self, ((PyObject *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_4get_random_move(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("get_random_move", 0);
+
+  /* "multimcts/mcts.pyx":21
+ *     def get_random_move(self) -> Hashable:
+ *         """Returns a random legal move from this state."""
+ *         return next(self.get_legal_moves(True))             # <<<<<<<<<<<<<<
+ * 
+ *     def has_move(self) -> bool:
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_get_legal_moves); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_3);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+    }
+  }
+  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, Py_True) : __Pyx_PyObject_CallOneArg(__pyx_t_2, Py_True);
+  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_PyIter_Next(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_r = __pyx_t_2;
+  __pyx_t_2 = 0;
+  goto __pyx_L0;
+
+  /* "multimcts/mcts.pyx":19
+ *         raise NotImplementedError("GameState must implement get_legal_moves.")
+ * 
+ *     def get_random_move(self) -> Hashable:             # <<<<<<<<<<<<<<
+ *         """Returns a random legal move from this state."""
+ *         return next(self.get_legal_moves(True))
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_AddTraceback("multimcts.mcts.GameState.get_random_move", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "multimcts/mcts.pyx":23
+ *         return next(self.get_legal_moves(True))
+ * 
+ *     def has_move(self) -> bool:             # <<<<<<<<<<<<<<
+ *         """Returns whether there are any legal moves in this state."""
+ *         try:
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_7has_move(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
+static char __pyx_doc_9multimcts_4mcts_9GameState_6has_move[] = "Returns whether there are any legal moves in this state.";
+static PyMethodDef __pyx_mdef_9multimcts_4mcts_9GameState_7has_move = {"has_move", (PyCFunction)__pyx_pw_9multimcts_4mcts_9GameState_7has_move, METH_O, __pyx_doc_9multimcts_4mcts_9GameState_6has_move};
+static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_7has_move(PyObject *__pyx_self, PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("has_move (wrapper)", 0);
+  __pyx_r = __pyx_pf_9multimcts_4mcts_9GameState_6has_move(__pyx_self, ((PyObject *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_6has_move(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_t_7;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("has_move", 0);
+
+  /* "multimcts/mcts.pyx":25
+ *     def has_move(self) -> bool:
+ *         """Returns whether there are any legal moves in this state."""
+ *         try:             # <<<<<<<<<<<<<<
+ *             next(self.get_legal_moves())
+ *             return True
+ */
+  {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
+    __Pyx_XGOTREF(__pyx_t_1);
+    __Pyx_XGOTREF(__pyx_t_2);
+    __Pyx_XGOTREF(__pyx_t_3);
+    /*try:*/ {
+
+      /* "multimcts/mcts.pyx":26
+ *         """Returns whether there are any legal moves in this state."""
+ *         try:
+ *             next(self.get_legal_moves())             # <<<<<<<<<<<<<<
+ *             return True
+ *         except StopIteration:
+ */
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_get_legal_moves); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 26, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_6 = NULL;
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
+        __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
+        if (likely(__pyx_t_6)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+          __Pyx_INCREF(__pyx_t_6);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_5, function);
+        }
+      }
+      __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
+      __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 26, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __pyx_t_5 = __Pyx_PyIter_Next(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 26, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+      /* "multimcts/mcts.pyx":27
+ *         try:
+ *             next(self.get_legal_moves())
+ *             return True             # <<<<<<<<<<<<<<
+ *         except StopIteration:
+ *             return False
+ */
+      __Pyx_XDECREF(__pyx_r);
+      __Pyx_INCREF(Py_True);
+      __pyx_r = Py_True;
+      goto __pyx_L7_try_return;
+
+      /* "multimcts/mcts.pyx":25
+ *     def has_move(self) -> bool:
+ *         """Returns whether there are any legal moves in this state."""
+ *         try:             # <<<<<<<<<<<<<<
+ *             next(self.get_legal_moves())
+ *             return True
+ */
+    }
+    __pyx_L3_error:;
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+
+    /* "multimcts/mcts.pyx":28
+ *             next(self.get_legal_moves())
+ *             return True
+ *         except StopIteration:             # <<<<<<<<<<<<<<
+ *             return False
+ * 
+ */
+    __pyx_t_7 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_StopIteration);
+    if (__pyx_t_7) {
+      __Pyx_AddTraceback("multimcts.mcts.GameState.has_move", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_4, &__pyx_t_6) < 0) __PYX_ERR(0, 28, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_GOTREF(__pyx_t_6);
+
+      /* "multimcts/mcts.pyx":29
+ *             return True
+ *         except StopIteration:
+ *             return False             # <<<<<<<<<<<<<<
+ * 
+ *     def make_move(self, move:Hashable) -> 'GameState':
+ */
+      __Pyx_XDECREF(__pyx_r);
+      __Pyx_INCREF(Py_False);
+      __pyx_r = Py_False;
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      goto __pyx_L6_except_return;
+    }
+    goto __pyx_L5_except_error;
+    __pyx_L5_except_error:;
+
+    /* "multimcts/mcts.pyx":25
+ *     def has_move(self) -> bool:
+ *         """Returns whether there are any legal moves in this state."""
+ *         try:             # <<<<<<<<<<<<<<
+ *             next(self.get_legal_moves())
+ *             return True
+ */
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    goto __pyx_L1_error;
+    __pyx_L7_try_return:;
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    goto __pyx_L0;
+    __pyx_L6_except_return:;
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    goto __pyx_L0;
+  }
+
+  /* "multimcts/mcts.pyx":23
+ *         return next(self.get_legal_moves(True))
+ * 
+ *     def has_move(self) -> bool:             # <<<<<<<<<<<<<<
+ *         """Returns whether there are any legal moves in this state."""
+ *         try:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_AddTraceback("multimcts.mcts.GameState.has_move", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "multimcts/mcts.pyx":31
+ *             return False
+ * 
+ *     def make_move(self, move:Hashable) -> 'GameState':             # <<<<<<<<<<<<<<
+ *         """Returns a new GameState, which is the result of applying the given move to this state.
+ *         This usually involves updating the board and advancing the player counter.
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_9make_move(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_9multimcts_4mcts_9GameState_8make_move[] = "Returns a new GameState, which is the result of applying the given move to this state.\n        This usually involves updating the board and advancing the player counter.\n        The current state object (self) should not be modified. Rather, modify a copy of it.\n        ";
+static PyMethodDef __pyx_mdef_9multimcts_4mcts_9GameState_9make_move = {"make_move", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_9GameState_9make_move, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9multimcts_4mcts_9GameState_8make_move};
+static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_9make_move(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  CYTHON_UNUSED PyObject *__pyx_v_self = 0;
+  CYTHON_UNUSED PyObject *__pyx_v_move = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("make_move (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_move,0};
+    PyObject* values[2] = {0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_move)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("make_move", 1, 2, 2, 1); __PYX_ERR(0, 31, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "make_move") < 0)) __PYX_ERR(0, 31, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+    }
+    __pyx_v_self = values[0];
+    __pyx_v_move = values[1];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("make_move", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 31, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("multimcts.mcts.GameState.make_move", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_9multimcts_4mcts_9GameState_8make_move(__pyx_self, __pyx_v_self, __pyx_v_move);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_8make_move(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_move) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("make_move", 0);
+
+  /* "multimcts/mcts.pyx":36
+ *         The current state object (self) should not be modified. Rather, modify a copy of it.
+ *         """
+ *         raise NotImplementedError("GameState must implement make_move.")             # <<<<<<<<<<<<<<
+ * 
+ *     def is_terminal(self) -> bool:
+ */
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_Raise(__pyx_t_1, 0, 0, 0);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __PYX_ERR(0, 36, __pyx_L1_error)
+
+  /* "multimcts/mcts.pyx":31
+ *             return False
+ * 
+ *     def make_move(self, move:Hashable) -> 'GameState':             # <<<<<<<<<<<<<<
+ *         """Returns a new GameState, which is the result of applying the given move to this state.
+ *         This usually involves updating the board and advancing the player counter.
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("multimcts.mcts.GameState.make_move", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "multimcts/mcts.pyx":38
+ *         raise NotImplementedError("GameState must implement make_move.")
+ * 
+ *     def is_terminal(self) -> bool:             # <<<<<<<<<<<<<<
+ *         """Checks if the game is over."""
+ *         raise NotImplementedError("GameState must implement is_terminal.")
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_11is_terminal(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
+static char __pyx_doc_9multimcts_4mcts_9GameState_10is_terminal[] = "Checks if the game is over.";
+static PyMethodDef __pyx_mdef_9multimcts_4mcts_9GameState_11is_terminal = {"is_terminal", (PyCFunction)__pyx_pw_9multimcts_4mcts_9GameState_11is_terminal, METH_O, __pyx_doc_9multimcts_4mcts_9GameState_10is_terminal};
+static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_11is_terminal(PyObject *__pyx_self, PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_terminal (wrapper)", 0);
+  __pyx_r = __pyx_pf_9multimcts_4mcts_9GameState_10is_terminal(__pyx_self, ((PyObject *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_10is_terminal(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("is_terminal", 0);
+
+  /* "multimcts/mcts.pyx":40
+ *     def is_terminal(self) -> bool:
+ *         """Checks if the game is over."""
+ *         raise NotImplementedError("GameState must implement is_terminal.")             # <<<<<<<<<<<<<<
+ * 
+ *     def get_reward(self) -> Union[float, Dict[Union[int,str], float]]:
+ */
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_Raise(__pyx_t_1, 0, 0, 0);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __PYX_ERR(0, 40, __pyx_L1_error)
+
+  /* "multimcts/mcts.pyx":38
+ *         raise NotImplementedError("GameState must implement make_move.")
+ * 
+ *     def is_terminal(self) -> bool:             # <<<<<<<<<<<<<<
+ *         """Checks if the game is over."""
+ *         raise NotImplementedError("GameState must implement is_terminal.")
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("multimcts.mcts.GameState.is_terminal", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "multimcts/mcts.pyx":42
+ *         raise NotImplementedError("GameState must implement is_terminal.")
+ * 
+ *     def get_reward(self) -> Union[float, Dict[Union[int,str], float]]:             # <<<<<<<<<<<<<<
+ *         """Returns the reward earned by the team that played the game-ending move.
+ *         Typically 1 for win, -1 for loss, 0 for draw.
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_13get_reward(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
+static char __pyx_doc_9multimcts_4mcts_9GameState_12get_reward[] = "Returns the reward earned by the team that played the game-ending move.\n        Typically 1 for win, -1 for loss, 0 for draw.\n        Alternatively, returns a dict of format {team:reward} or {team1:reward1, team2:reward2, ...}\n        Note: This method is only evaluated on terminal states.\n        ";
+static PyMethodDef __pyx_mdef_9multimcts_4mcts_9GameState_13get_reward = {"get_reward", (PyCFunction)__pyx_pw_9multimcts_4mcts_9GameState_13get_reward, METH_O, __pyx_doc_9multimcts_4mcts_9GameState_12get_reward};
+static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_13get_reward(PyObject *__pyx_self, PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("get_reward (wrapper)", 0);
+  __pyx_r = __pyx_pf_9multimcts_4mcts_9GameState_12get_reward(__pyx_self, ((PyObject *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_12get_reward(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("get_reward", 0);
+
+  /* "multimcts/mcts.pyx":48
+ *         Note: This method is only evaluated on terminal states.
+ *         """
+ *         raise NotImplementedError("GameState must implement get_reward.")             # <<<<<<<<<<<<<<
+ * 
+ *     def __hash__(self) -> int:
+ */
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_Raise(__pyx_t_1, 0, 0, 0);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __PYX_ERR(0, 48, __pyx_L1_error)
+
+  /* "multimcts/mcts.pyx":42
+ *         raise NotImplementedError("GameState must implement is_terminal.")
+ * 
+ *     def get_reward(self) -> Union[float, Dict[Union[int,str], float]]:             # <<<<<<<<<<<<<<
+ *         """Returns the reward earned by the team that played the game-ending move.
+ *         Typically 1 for win, -1 for loss, 0 for draw.
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("multimcts.mcts.GameState.get_reward", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "multimcts/mcts.pyx":50
+ *         raise NotImplementedError("GameState must implement get_reward.")
+ * 
+ *     def __hash__(self) -> int:             # <<<<<<<<<<<<<<
+ *         raise NotImplementedError("GameState must implement __hash__")
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_15__hash__(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
+static PyMethodDef __pyx_mdef_9multimcts_4mcts_9GameState_15__hash__ = {"__hash__", (PyCFunction)__pyx_pw_9multimcts_4mcts_9GameState_15__hash__, METH_O, 0};
+static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_15__hash__(PyObject *__pyx_self, PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__hash__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_9multimcts_4mcts_9GameState_14__hash__(__pyx_self, ((PyObject *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_14__hash__(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__hash__", 0);
+
+  /* "multimcts/mcts.pyx":51
+ * 
+ *     def __hash__(self) -> int:
+ *         raise NotImplementedError("GameState must implement __hash__")             # <<<<<<<<<<<<<<
+ * 
+ *     def __eq__(self, other:'GameState') -> bool:
+ */
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_Raise(__pyx_t_1, 0, 0, 0);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __PYX_ERR(0, 51, __pyx_L1_error)
+
+  /* "multimcts/mcts.pyx":50
+ *         raise NotImplementedError("GameState must implement get_reward.")
+ * 
+ *     def __hash__(self) -> int:             # <<<<<<<<<<<<<<
+ *         raise NotImplementedError("GameState must implement __hash__")
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("multimcts.mcts.GameState.__hash__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "multimcts/mcts.pyx":53
+ *         raise NotImplementedError("GameState must implement __hash__")
+ * 
+ *     def __eq__(self, other:'GameState') -> bool:             # <<<<<<<<<<<<<<
+ *         raise NotImplementedError("GameStates must implement __eq__")
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_17__eq__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_9multimcts_4mcts_9GameState_17__eq__ = {"__eq__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_9GameState_17__eq__, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_17__eq__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  CYTHON_UNUSED PyObject *__pyx_v_self = 0;
+  CYTHON_UNUSED PyObject *__pyx_v_other = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__eq__ (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_other,0};
+    PyObject* values[2] = {0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_other)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("__eq__", 1, 2, 2, 1); __PYX_ERR(0, 53, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__eq__") < 0)) __PYX_ERR(0, 53, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+    }
+    __pyx_v_self = values[0];
+    __pyx_v_other = values[1];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("__eq__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 53, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("multimcts.mcts.GameState.__eq__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_9multimcts_4mcts_9GameState_16__eq__(__pyx_self, __pyx_v_self, __pyx_v_other);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9multimcts_4mcts_9GameState_16__eq__(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_other) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__eq__", 0);
+
+  /* "multimcts/mcts.pyx":54
+ * 
+ *     def __eq__(self, other:'GameState') -> bool:
+ *         raise NotImplementedError("GameStates must implement __eq__")             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_Raise(__pyx_t_1, 0, 0, 0);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __PYX_ERR(0, 54, __pyx_L1_error)
+
+  /* "multimcts/mcts.pyx":53
+ *         raise NotImplementedError("GameState must implement __hash__")
+ * 
+ *     def __eq__(self, other:'GameState') -> bool:             # <<<<<<<<<<<<<<
+ *         raise NotImplementedError("GameStates must implement __eq__")
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("multimcts.mcts.GameState.__eq__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "multimcts/mcts.pyx":72
  *         remaining_moves (list): A list of moves that have not yet been tried.
  *     """
  *     def __init__(self, state:GameState, parent:'Node'=None):             # <<<<<<<<<<<<<<
  *         self.state = state
  *         self.parent = parent
  */
 
@@ -1971,25 +2931,25 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_state)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, 1); __PYX_ERR(0, 25, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, 1); __PYX_ERR(0, 72, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_parent);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 25, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 72, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
@@ -1999,15 +2959,15 @@
     }
     __pyx_v_self = values[0];
     __pyx_v_state = values[1];
     __pyx_v_parent = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 25, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 72, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.Node.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9multimcts_4mcts_4Node___init__(__pyx_self, __pyx_v_self, __pyx_v_state, __pyx_v_parent);
 
@@ -2025,169 +2985,169 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "multimcts/mcts.pyx":26
+  /* "multimcts/mcts.pyx":73
  *     """
  *     def __init__(self, state:GameState, parent:'Node'=None):
  *         self.state = state             # <<<<<<<<<<<<<<
  *         self.parent = parent
  * 
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_state, __pyx_v_state) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_state, __pyx_v_state) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":27
+  /* "multimcts/mcts.pyx":74
  *     def __init__(self, state:GameState, parent:'Node'=None):
  *         self.state = state
  *         self.parent = parent             # <<<<<<<<<<<<<<
  * 
  *         self.children:Dict[Hashable,'Node'] = {}
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_parent, __pyx_v_parent) < 0) __PYX_ERR(0, 27, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_parent, __pyx_v_parent) < 0) __PYX_ERR(0, 74, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":29
+  /* "multimcts/mcts.pyx":76
  *         self.parent = parent
  * 
  *         self.children:Dict[Hashable,'Node'] = {}             # <<<<<<<<<<<<<<
  *         self.num_visits = 0
  *         self.total_reward = defaultdict(float)
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_children, __pyx_t_1) < 0) __PYX_ERR(0, 29, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_children, __pyx_t_1) < 0) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":30
+  /* "multimcts/mcts.pyx":77
  * 
  *         self.children:Dict[Hashable,'Node'] = {}
  *         self.num_visits = 0             # <<<<<<<<<<<<<<
  *         self.total_reward = defaultdict(float)
  * 
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_num_visits, __pyx_int_0) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_num_visits, __pyx_int_0) < 0) __PYX_ERR(0, 77, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":31
+  /* "multimcts/mcts.pyx":78
  *         self.children:Dict[Hashable,'Node'] = {}
  *         self.num_visits = 0
  *         self.total_reward = defaultdict(float)             # <<<<<<<<<<<<<<
  * 
  *         self.is_terminal = self.state.is_terminal()
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_defaultdict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_defaultdict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, ((PyObject *)(&PyFloat_Type))) : __Pyx_PyObject_CallOneArg(__pyx_t_2, ((PyObject *)(&PyFloat_Type)));
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 31, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_total_reward, __pyx_t_1) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_total_reward, __pyx_t_1) < 0) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":33
+  /* "multimcts/mcts.pyx":80
  *         self.total_reward = defaultdict(float)
  * 
  *         self.is_terminal = self.state.is_terminal()             # <<<<<<<<<<<<<<
  *         self.is_fully_expanded = self.is_terminal
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_state); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_state); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_is_terminal, __pyx_t_1) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_is_terminal, __pyx_t_1) < 0) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":34
+  /* "multimcts/mcts.pyx":81
  * 
  *         self.is_terminal = self.state.is_terminal()
  *         self.is_fully_expanded = self.is_terminal             # <<<<<<<<<<<<<<
  * 
  *         self.remaining_moves = [] if self.is_fully_expanded else list(self.state.get_legal_moves(True))
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_is_fully_expanded, __pyx_t_1) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_is_fully_expanded, __pyx_t_1) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":36
+  /* "multimcts/mcts.pyx":83
  *         self.is_fully_expanded = self.is_terminal
  * 
  *         self.remaining_moves = [] if self.is_fully_expanded else list(self.state.get_legal_moves(True))             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_is_fully_expanded); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_is_fully_expanded); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_4) {
-    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 83, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_1 = __pyx_t_3;
     __pyx_t_3 = 0;
   } else {
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_state); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_state); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 83, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get_legal_moves); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 36, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get_legal_moves); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 83, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_3 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_2, Py_True) : __Pyx_PyObject_CallOneArg(__pyx_t_5, Py_True);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 83, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = PySequence_List(__pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 36, __pyx_L1_error)
+    __pyx_t_5 = PySequence_List(__pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 83, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_1 = __pyx_t_5;
     __pyx_t_5 = 0;
   }
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_remaining_moves, __pyx_t_1) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_remaining_moves, __pyx_t_1) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":25
+  /* "multimcts/mcts.pyx":72
  *         remaining_moves (list): A list of moves that have not yet been tried.
  *     """
  *     def __init__(self, state:GameState, parent:'Node'=None):             # <<<<<<<<<<<<<<
  *         self.state = state
  *         self.parent = parent
  */
 
@@ -2203,15 +3163,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":40
+/* "multimcts/mcts.pyx":87
  * 
  * class MCTS():
  *     def __init__(self, *, exploration_bias:float=1.414, heuristic=None, max_time:float=None, max_iterations:int=None):             # <<<<<<<<<<<<<<
  *         """Initializes an MCTS agent.
  * 
  */
 
@@ -2256,34 +3216,34 @@
         Py_ssize_t index;
         for (index = 1; index < 5 && kw_args > 0; index++) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, *__pyx_pyargnames[index]);
           if (value) { values[index] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 40, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 87, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
     if (values[1]) {
-      __pyx_v_exploration_bias = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_exploration_bias == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 40, __pyx_L3_error)
+      __pyx_v_exploration_bias = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_exploration_bias == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 87, __pyx_L3_error)
     } else {
       __pyx_v_exploration_bias = ((double)((double)1.414));
     }
     __pyx_v_heuristic = values[2];
     __pyx_v_max_time = values[3];
     __pyx_v_max_iterations = values[4];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 40, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 87, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.MCTS.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS___init__(__pyx_self, __pyx_v_self, __pyx_v_exploration_bias, __pyx_v_heuristic, __pyx_v_max_time, __pyx_v_max_iterations);
 
@@ -2300,15 +3260,15 @@
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "multimcts/mcts.pyx":53
+  /* "multimcts/mcts.pyx":100
  *             max_iterations (int): The maximum number of iterations that the search method should execute.
  *         """
  *         if max_iterations is None and max_time is None:             # <<<<<<<<<<<<<<
  *             raise ValueError("One or more of max_time/max_iterations is required.")
  * 
  */
   __pyx_t_2 = (__pyx_v_max_iterations == Py_None);
@@ -2320,76 +3280,76 @@
   }
   __pyx_t_3 = (__pyx_v_max_time == Py_None);
   __pyx_t_2 = (__pyx_t_3 != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
-    /* "multimcts/mcts.pyx":54
+    /* "multimcts/mcts.pyx":101
  *         """
  *         if max_iterations is None and max_time is None:
  *             raise ValueError("One or more of max_time/max_iterations is required.")             # <<<<<<<<<<<<<<
  * 
  *         self.exploration_bias = exploration_bias
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 54, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 101, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 54, __pyx_L1_error)
+    __PYX_ERR(0, 101, __pyx_L1_error)
 
-    /* "multimcts/mcts.pyx":53
+    /* "multimcts/mcts.pyx":100
  *             max_iterations (int): The maximum number of iterations that the search method should execute.
  *         """
  *         if max_iterations is None and max_time is None:             # <<<<<<<<<<<<<<
  *             raise ValueError("One or more of max_time/max_iterations is required.")
  * 
  */
   }
 
-  /* "multimcts/mcts.pyx":56
+  /* "multimcts/mcts.pyx":103
  *             raise ValueError("One or more of max_time/max_iterations is required.")
  * 
  *         self.exploration_bias = exploration_bias             # <<<<<<<<<<<<<<
  *         self.heuristic = heuristic
  * 
  */
-  __pyx_t_4 = PyFloat_FromDouble(__pyx_v_exploration_bias); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_t_4 = PyFloat_FromDouble(__pyx_v_exploration_bias); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_exploration_bias, __pyx_t_4) < 0) __PYX_ERR(0, 56, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_exploration_bias, __pyx_t_4) < 0) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "multimcts/mcts.pyx":57
+  /* "multimcts/mcts.pyx":104
  * 
  *         self.exploration_bias = exploration_bias
  *         self.heuristic = heuristic             # <<<<<<<<<<<<<<
  * 
  *         self.max_time = max_time
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_heuristic, __pyx_v_heuristic) < 0) __PYX_ERR(0, 57, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_heuristic, __pyx_v_heuristic) < 0) __PYX_ERR(0, 104, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":59
+  /* "multimcts/mcts.pyx":106
  *         self.heuristic = heuristic
  * 
  *         self.max_time = max_time             # <<<<<<<<<<<<<<
  *         self.max_iterations = max_iterations
  * 
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_max_time, __pyx_v_max_time) < 0) __PYX_ERR(0, 59, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_max_time, __pyx_v_max_time) < 0) __PYX_ERR(0, 106, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":60
+  /* "multimcts/mcts.pyx":107
  * 
  *         self.max_time = max_time
  *         self.max_iterations = max_iterations             # <<<<<<<<<<<<<<
  * 
  *     def search(self, state:GameState) -> GameState:
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_max_iterations, __pyx_v_max_iterations) < 0) __PYX_ERR(0, 60, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_max_iterations, __pyx_v_max_iterations) < 0) __PYX_ERR(0, 107, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":40
+  /* "multimcts/mcts.pyx":87
  * 
  * class MCTS():
  *     def __init__(self, *, exploration_bias:float=1.414, heuristic=None, max_time:float=None, max_iterations:int=None):             # <<<<<<<<<<<<<<
  *         """Initializes an MCTS agent.
  * 
  */
 
@@ -2402,15 +3362,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":62
+/* "multimcts/mcts.pyx":109
  *         self.max_iterations = max_iterations
  * 
  *     def search(self, state:GameState) -> GameState:             # <<<<<<<<<<<<<<
  *         """Searches for this state's best move until some limit has been reached.
  * 
  */
 
@@ -2446,32 +3406,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_state)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("search", 1, 2, 2, 1); __PYX_ERR(0, 62, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("search", 1, 2, 2, 1); __PYX_ERR(0, 109, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "search") < 0)) __PYX_ERR(0, 62, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "search") < 0)) __PYX_ERR(0, 109, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_state = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("search", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 62, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("search", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 109, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.MCTS.search", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_2search(__pyx_self, __pyx_v_self, __pyx_v_state);
 
@@ -2497,204 +3457,204 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("search", 0);
 
-  /* "multimcts/mcts.pyx":70
+  /* "multimcts/mcts.pyx":117
  *             GameState: A new game state which is the result of applying the best move to the given state.
  *         """
  *         node = Node(state)             # <<<<<<<<<<<<<<
  * 
  *         if self.max_time is not None:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Node); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Node); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 117, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_state) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_state);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 117, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_node = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":72
+  /* "multimcts/mcts.pyx":119
  *         node = Node(state)
  * 
  *         if self.max_time is not None:             # <<<<<<<<<<<<<<
  *             end_time = time.time() + self.max_time
  *         if self.max_iterations is not None:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_4 = (__pyx_t_1 != Py_None);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_5 = (__pyx_t_4 != 0);
   if (__pyx_t_5) {
 
-    /* "multimcts/mcts.pyx":73
+    /* "multimcts/mcts.pyx":120
  * 
  *         if self.max_time is not None:
  *             end_time = time.time() + self.max_time             # <<<<<<<<<<<<<<
  *         if self.max_iterations is not None:
  *             i = 0
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 120, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 120, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 120, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = PyNumber_Add(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_Add(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_end_time = __pyx_t_2;
     __pyx_t_2 = 0;
 
-    /* "multimcts/mcts.pyx":72
+    /* "multimcts/mcts.pyx":119
  *         node = Node(state)
  * 
  *         if self.max_time is not None:             # <<<<<<<<<<<<<<
  *             end_time = time.time() + self.max_time
  *         if self.max_iterations is not None:
  */
   }
 
-  /* "multimcts/mcts.pyx":74
+  /* "multimcts/mcts.pyx":121
  *         if self.max_time is not None:
  *             end_time = time.time() + self.max_time
  *         if self.max_iterations is not None:             # <<<<<<<<<<<<<<
  *             i = 0
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_iterations); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_iterations); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_5 = (__pyx_t_2 != Py_None);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = (__pyx_t_5 != 0);
   if (__pyx_t_4) {
 
-    /* "multimcts/mcts.pyx":75
+    /* "multimcts/mcts.pyx":122
  *             end_time = time.time() + self.max_time
  *         if self.max_iterations is not None:
  *             i = 0             # <<<<<<<<<<<<<<
  * 
  *         while True:
  */
     __Pyx_INCREF(__pyx_int_0);
     __pyx_v_i = __pyx_int_0;
 
-    /* "multimcts/mcts.pyx":74
+    /* "multimcts/mcts.pyx":121
  *         if self.max_time is not None:
  *             end_time = time.time() + self.max_time
  *         if self.max_iterations is not None:             # <<<<<<<<<<<<<<
  *             i = 0
  * 
  */
   }
 
-  /* "multimcts/mcts.pyx":77
+  /* "multimcts/mcts.pyx":124
  *             i = 0
  * 
  *         while True:             # <<<<<<<<<<<<<<
  *             child = self.select(node)
  *             reward = self.simulate(child)
  */
   while (1) {
 
-    /* "multimcts/mcts.pyx":78
+    /* "multimcts/mcts.pyx":125
  * 
  *         while True:
  *             child = self.select(node)             # <<<<<<<<<<<<<<
  *             reward = self.simulate(child)
  *             self.backpropagate(child, reward)
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_select); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 78, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_select); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 125, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_1 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_1)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_1);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_1, __pyx_v_node) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_node);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 125, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF_SET(__pyx_v_child, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "multimcts/mcts.pyx":79
+    /* "multimcts/mcts.pyx":126
  *         while True:
  *             child = self.select(node)
  *             reward = self.simulate(child)             # <<<<<<<<<<<<<<
  *             self.backpropagate(child, reward)
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_simulate); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 79, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_simulate); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 126, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_1 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_1)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_1);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_1, __pyx_v_child) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_child);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 126, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF_SET(__pyx_v_reward, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "multimcts/mcts.pyx":80
+    /* "multimcts/mcts.pyx":127
  *             child = self.select(node)
  *             reward = self.simulate(child)
  *             self.backpropagate(child, reward)             # <<<<<<<<<<<<<<
  * 
  *             if self.max_time is not None and time.time() >= end_time:
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_backpropagate); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 80, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_backpropagate); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 127, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_1 = NULL;
     __pyx_t_6 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_1)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -2703,214 +3663,214 @@
         __Pyx_DECREF_SET(__pyx_t_3, function);
         __pyx_t_6 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_3)) {
       PyObject *__pyx_temp[3] = {__pyx_t_1, __pyx_v_child, __pyx_v_reward};
-      __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 80, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 127, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_GOTREF(__pyx_t_2);
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
       PyObject *__pyx_temp[3] = {__pyx_t_1, __pyx_v_child, __pyx_v_reward};
-      __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 80, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 127, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_GOTREF(__pyx_t_2);
     } else
     #endif
     {
-      __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 80, __pyx_L1_error)
+      __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 127, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       if (__pyx_t_1) {
         __Pyx_GIVEREF(__pyx_t_1); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_1); __pyx_t_1 = NULL;
       }
       __Pyx_INCREF(__pyx_v_child);
       __Pyx_GIVEREF(__pyx_v_child);
       PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_v_child);
       __Pyx_INCREF(__pyx_v_reward);
       __Pyx_GIVEREF(__pyx_v_reward);
       PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_v_reward);
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 80, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 127, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "multimcts/mcts.pyx":82
+    /* "multimcts/mcts.pyx":129
  *             self.backpropagate(child, reward)
  * 
  *             if self.max_time is not None and time.time() >= end_time:             # <<<<<<<<<<<<<<
  *                 break
  *             if self.max_iterations is not None:
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_5 = (__pyx_t_2 != Py_None);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_8 = (__pyx_t_5 != 0);
     if (__pyx_t_8) {
     } else {
       __pyx_t_4 = __pyx_t_8;
       goto __pyx_L8_bool_binop_done;
     }
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 82, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_time); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 82, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_time); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
     __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_v_end_time)) { __Pyx_RaiseUnboundLocalError("end_time"); __PYX_ERR(0, 82, __pyx_L1_error) }
-    __pyx_t_7 = PyObject_RichCompare(__pyx_t_2, __pyx_v_end_time, Py_GE); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 82, __pyx_L1_error)
+    if (unlikely(!__pyx_v_end_time)) { __Pyx_RaiseUnboundLocalError("end_time"); __PYX_ERR(0, 129, __pyx_L1_error) }
+    __pyx_t_7 = PyObject_RichCompare(__pyx_t_2, __pyx_v_end_time, Py_GE); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 129, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 82, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 129, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_t_4 = __pyx_t_8;
     __pyx_L8_bool_binop_done:;
     if (__pyx_t_4) {
 
-      /* "multimcts/mcts.pyx":83
+      /* "multimcts/mcts.pyx":130
  * 
  *             if self.max_time is not None and time.time() >= end_time:
  *                 break             # <<<<<<<<<<<<<<
  *             if self.max_iterations is not None:
  *                 i += 1
  */
       goto __pyx_L6_break;
 
-      /* "multimcts/mcts.pyx":82
+      /* "multimcts/mcts.pyx":129
  *             self.backpropagate(child, reward)
  * 
  *             if self.max_time is not None and time.time() >= end_time:             # <<<<<<<<<<<<<<
  *                 break
  *             if self.max_iterations is not None:
  */
     }
 
-    /* "multimcts/mcts.pyx":84
+    /* "multimcts/mcts.pyx":131
  *             if self.max_time is not None and time.time() >= end_time:
  *                 break
  *             if self.max_iterations is not None:             # <<<<<<<<<<<<<<
  *                 i += 1
  *                 if i >= self.max_iterations:
  */
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_iterations); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 84, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_iterations); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 131, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_4 = (__pyx_t_7 != Py_None);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_t_8 = (__pyx_t_4 != 0);
     if (__pyx_t_8) {
 
-      /* "multimcts/mcts.pyx":85
+      /* "multimcts/mcts.pyx":132
  *                 break
  *             if self.max_iterations is not None:
  *                 i += 1             # <<<<<<<<<<<<<<
  *                 if i >= self.max_iterations:
  *                     break
  */
-      if (unlikely(!__pyx_v_i)) { __Pyx_RaiseUnboundLocalError("i"); __PYX_ERR(0, 85, __pyx_L1_error) }
-      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_v_i, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 85, __pyx_L1_error)
+      if (unlikely(!__pyx_v_i)) { __Pyx_RaiseUnboundLocalError("i"); __PYX_ERR(0, 132, __pyx_L1_error) }
+      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_v_i, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 132, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_7);
       __pyx_t_7 = 0;
 
-      /* "multimcts/mcts.pyx":86
+      /* "multimcts/mcts.pyx":133
  *             if self.max_iterations is not None:
  *                 i += 1
  *                 if i >= self.max_iterations:             # <<<<<<<<<<<<<<
  *                     break
  * 
  */
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_iterations); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 86, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_iterations); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 133, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_2 = PyObject_RichCompare(__pyx_v_i, __pyx_t_7, Py_GE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
+      __pyx_t_2 = PyObject_RichCompare(__pyx_v_i, __pyx_t_7, Py_GE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 133, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 86, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 133, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (__pyx_t_8) {
 
-        /* "multimcts/mcts.pyx":87
+        /* "multimcts/mcts.pyx":134
  *                 i += 1
  *                 if i >= self.max_iterations:
  *                     break             # <<<<<<<<<<<<<<
  * 
  *         return self.get_best_child(node).state
  */
         goto __pyx_L6_break;
 
-        /* "multimcts/mcts.pyx":86
+        /* "multimcts/mcts.pyx":133
  *             if self.max_iterations is not None:
  *                 i += 1
  *                 if i >= self.max_iterations:             # <<<<<<<<<<<<<<
  *                     break
  * 
  */
       }
 
-      /* "multimcts/mcts.pyx":84
+      /* "multimcts/mcts.pyx":131
  *             if self.max_time is not None and time.time() >= end_time:
  *                 break
  *             if self.max_iterations is not None:             # <<<<<<<<<<<<<<
  *                 i += 1
  *                 if i >= self.max_iterations:
  */
     }
   }
   __pyx_L6_break:;
 
-  /* "multimcts/mcts.pyx":89
+  /* "multimcts/mcts.pyx":136
  *                     break
  * 
  *         return self.get_best_child(node).state             # <<<<<<<<<<<<<<
  * 
  *     def select(self, node:Node) -> Node:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_get_best_child); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_get_best_child); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_7);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_7, function);
     }
   }
   __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_3, __pyx_v_node) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_v_node);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 89, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_state); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_state); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_7;
   __pyx_t_7 = 0;
   goto __pyx_L0;
 
-  /* "multimcts/mcts.pyx":62
+  /* "multimcts/mcts.pyx":109
  *         self.max_iterations = max_iterations
  * 
  *     def search(self, state:GameState) -> GameState:             # <<<<<<<<<<<<<<
  *         """Searches for this state's best move until some limit has been reached.
  * 
  */
 
@@ -2929,15 +3889,15 @@
   __Pyx_XDECREF(__pyx_v_child);
   __Pyx_XDECREF(__pyx_v_reward);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":91
+/* "multimcts/mcts.pyx":138
  *         return self.get_best_child(node).state
  * 
  *     def select(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 1: Selection
  *         Traverse the tree for the node we most want to simulate.
  */
 
@@ -2973,32 +3933,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("select", 1, 2, 2, 1); __PYX_ERR(0, 91, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("select", 1, 2, 2, 1); __PYX_ERR(0, 138, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "select") < 0)) __PYX_ERR(0, 91, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "select") < 0)) __PYX_ERR(0, 138, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_node = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("select", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 91, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("select", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 138, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.MCTS.select", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_4select(__pyx_self, __pyx_v_self, __pyx_v_node);
 
@@ -3017,124 +3977,124 @@
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("select", 0);
   __Pyx_INCREF(__pyx_v_node);
 
-  /* "multimcts/mcts.pyx":96
+  /* "multimcts/mcts.pyx":143
  *         Looks for an unexplored child of this node's best child's best child's...best child.
  *         """
  *         while not node.is_terminal:             # <<<<<<<<<<<<<<
  *             if not node.is_fully_expanded:
  *                 return self.expand(node)
  */
   while (1) {
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 96, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 143, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_3 = ((!__pyx_t_2) != 0);
     if (!__pyx_t_3) break;
 
-    /* "multimcts/mcts.pyx":97
+    /* "multimcts/mcts.pyx":144
  *         """
  *         while not node.is_terminal:
  *             if not node.is_fully_expanded:             # <<<<<<<<<<<<<<
  *                 return self.expand(node)
  *             else:
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_is_fully_expanded); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_is_fully_expanded); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 97, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 144, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_2 = ((!__pyx_t_3) != 0);
     if (__pyx_t_2) {
 
-      /* "multimcts/mcts.pyx":98
+      /* "multimcts/mcts.pyx":145
  *         while not node.is_terminal:
  *             if not node.is_fully_expanded:
  *                 return self.expand(node)             # <<<<<<<<<<<<<<
  *             else:
  *                 node = self.get_best_child(node)
  */
       __Pyx_XDECREF(__pyx_r);
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_expand); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 98, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_expand); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 145, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_5 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_5)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_node) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_node);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 98, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 145, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_r = __pyx_t_1;
       __pyx_t_1 = 0;
       goto __pyx_L0;
 
-      /* "multimcts/mcts.pyx":97
+      /* "multimcts/mcts.pyx":144
  *         """
  *         while not node.is_terminal:
  *             if not node.is_fully_expanded:             # <<<<<<<<<<<<<<
  *                 return self.expand(node)
  *             else:
  */
     }
 
-    /* "multimcts/mcts.pyx":100
+    /* "multimcts/mcts.pyx":147
  *                 return self.expand(node)
  *             else:
  *                 node = self.get_best_child(node)             # <<<<<<<<<<<<<<
  * 
  *         return node
  */
     /*else*/ {
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_get_best_child); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 100, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_get_best_child); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 147, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_5 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_5)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_node) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_node);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 100, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 147, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF_SET(__pyx_v_node, __pyx_t_1);
       __pyx_t_1 = 0;
     }
   }
 
-  /* "multimcts/mcts.pyx":102
+  /* "multimcts/mcts.pyx":149
  *                 node = self.get_best_child(node)
  * 
  *         return node             # <<<<<<<<<<<<<<
  * 
  *     @staticmethod
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_node);
   __pyx_r = __pyx_v_node;
   goto __pyx_L0;
 
-  /* "multimcts/mcts.pyx":91
+  /* "multimcts/mcts.pyx":138
  *         return self.get_best_child(node).state
  * 
  *     def select(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 1: Selection
  *         Traverse the tree for the node we most want to simulate.
  */
 
@@ -3148,15 +4108,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_node);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":105
+/* "multimcts/mcts.pyx":152
  * 
  *     @staticmethod
  *     def expand(node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 2: Expansion
  *         Add a new child to this node.
  */
 
@@ -3192,15 +4152,15 @@
   Py_ssize_t __pyx_t_10;
   int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("expand", 0);
 
-  /* "multimcts/mcts.pyx":109
+  /* "multimcts/mcts.pyx":156
  *         Add a new child to this node.
  *         """
  *         try:             # <<<<<<<<<<<<<<
  *             move = node.remaining_moves.pop()
  *             child = Node(node.state.make_move(move), node)
  */
   {
@@ -3208,56 +4168,56 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "multimcts/mcts.pyx":110
+      /* "multimcts/mcts.pyx":157
  *         """
  *         try:
  *             move = node.remaining_moves.pop()             # <<<<<<<<<<<<<<
  *             child = Node(node.state.make_move(move), node)
  *             node.children[move] = child
  */
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_remaining_moves); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 110, __pyx_L3_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_remaining_moves); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 157, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = __Pyx_PyObject_Pop(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 110, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyObject_Pop(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 157, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_v_move = __pyx_t_5;
       __pyx_t_5 = 0;
 
-      /* "multimcts/mcts.pyx":111
+      /* "multimcts/mcts.pyx":158
  *         try:
  *             move = node.remaining_moves.pop()
  *             child = Node(node.state.make_move(move), node)             # <<<<<<<<<<<<<<
  *             node.children[move] = child
  * 
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Node); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 111, __pyx_L3_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Node); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 158, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_state); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 111, __pyx_L3_error)
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_state); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 158, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_make_move); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 111, __pyx_L3_error)
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_make_move); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 158, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_t_7 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
         __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_8);
         if (likely(__pyx_t_7)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
           __Pyx_INCREF(__pyx_t_7);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_8, function);
         }
       }
       __pyx_t_6 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_7, __pyx_v_move) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_v_move);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 111, __pyx_L3_error)
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 158, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __pyx_t_8 = NULL;
       __pyx_t_9 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_8)) {
@@ -3267,152 +4227,152 @@
           __Pyx_DECREF_SET(__pyx_t_4, function);
           __pyx_t_9 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_4)) {
         PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_6, __pyx_v_node};
-        __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 111, __pyx_L3_error)
+        __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 158, __pyx_L3_error)
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
         PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_6, __pyx_v_node};
-        __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 111, __pyx_L3_error)
+        __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 158, __pyx_L3_error)
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       } else
       #endif
       {
-        __pyx_t_7 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 111, __pyx_L3_error)
+        __pyx_t_7 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 158, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_7);
         if (__pyx_t_8) {
           __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_8); __pyx_t_8 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_6);
         PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_9, __pyx_t_6);
         __Pyx_INCREF(__pyx_v_node);
         __Pyx_GIVEREF(__pyx_v_node);
         PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_9, __pyx_v_node);
         __pyx_t_6 = 0;
-        __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 111, __pyx_L3_error)
+        __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 158, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       }
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_v_child = __pyx_t_5;
       __pyx_t_5 = 0;
 
-      /* "multimcts/mcts.pyx":112
+      /* "multimcts/mcts.pyx":159
  *             move = node.remaining_moves.pop()
  *             child = Node(node.state.make_move(move), node)
  *             node.children[move] = child             # <<<<<<<<<<<<<<
  * 
  *             if len(node.remaining_moves) == 0:
  */
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_children); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 112, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_children); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 159, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
-      if (unlikely(PyObject_SetItem(__pyx_t_5, __pyx_v_move, __pyx_v_child) < 0)) __PYX_ERR(0, 112, __pyx_L3_error)
+      if (unlikely(PyObject_SetItem(__pyx_t_5, __pyx_v_move, __pyx_v_child) < 0)) __PYX_ERR(0, 159, __pyx_L3_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-      /* "multimcts/mcts.pyx":114
+      /* "multimcts/mcts.pyx":161
  *             node.children[move] = child
  * 
  *             if len(node.remaining_moves) == 0:             # <<<<<<<<<<<<<<
  *                 node.is_fully_expanded = True
  * 
  */
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_remaining_moves); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 114, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_remaining_moves); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 161, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_10 = PyObject_Length(__pyx_t_5); if (unlikely(__pyx_t_10 == ((Py_ssize_t)-1))) __PYX_ERR(0, 114, __pyx_L3_error)
+      __pyx_t_10 = PyObject_Length(__pyx_t_5); if (unlikely(__pyx_t_10 == ((Py_ssize_t)-1))) __PYX_ERR(0, 161, __pyx_L3_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_11 = ((__pyx_t_10 == 0) != 0);
       if (__pyx_t_11) {
 
-        /* "multimcts/mcts.pyx":115
+        /* "multimcts/mcts.pyx":162
  * 
  *             if len(node.remaining_moves) == 0:
  *                 node.is_fully_expanded = True             # <<<<<<<<<<<<<<
  * 
  *             return child
  */
-        if (__Pyx_PyObject_SetAttrStr(__pyx_v_node, __pyx_n_s_is_fully_expanded, Py_True) < 0) __PYX_ERR(0, 115, __pyx_L3_error)
+        if (__Pyx_PyObject_SetAttrStr(__pyx_v_node, __pyx_n_s_is_fully_expanded, Py_True) < 0) __PYX_ERR(0, 162, __pyx_L3_error)
 
-        /* "multimcts/mcts.pyx":114
+        /* "multimcts/mcts.pyx":161
  *             node.children[move] = child
  * 
  *             if len(node.remaining_moves) == 0:             # <<<<<<<<<<<<<<
  *                 node.is_fully_expanded = True
  * 
  */
       }
 
-      /* "multimcts/mcts.pyx":117
+      /* "multimcts/mcts.pyx":164
  *                 node.is_fully_expanded = True
  * 
  *             return child             # <<<<<<<<<<<<<<
  *         except IndexError:
  *             raise Exception("Tried to expand a fully-expanded or terminal node.")
  */
       __Pyx_XDECREF(__pyx_r);
       __Pyx_INCREF(__pyx_v_child);
       __pyx_r = __pyx_v_child;
       goto __pyx_L7_try_return;
 
-      /* "multimcts/mcts.pyx":109
+      /* "multimcts/mcts.pyx":156
  *         Add a new child to this node.
  *         """
  *         try:             # <<<<<<<<<<<<<<
  *             move = node.remaining_moves.pop()
  *             child = Node(node.state.make_move(move), node)
  */
     }
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "multimcts/mcts.pyx":118
+    /* "multimcts/mcts.pyx":165
  * 
  *             return child
  *         except IndexError:             # <<<<<<<<<<<<<<
  *             raise Exception("Tried to expand a fully-expanded or terminal node.")
  * 
  */
     __pyx_t_9 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_IndexError);
     if (__pyx_t_9) {
       __Pyx_AddTraceback("multimcts.mcts.MCTS.expand", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_4, &__pyx_t_7) < 0) __PYX_ERR(0, 118, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_4, &__pyx_t_7) < 0) __PYX_ERR(0, 165, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "multimcts/mcts.pyx":119
+      /* "multimcts/mcts.pyx":166
  *             return child
  *         except IndexError:
  *             raise Exception("Tried to expand a fully-expanded or terminal node.")             # <<<<<<<<<<<<<<
  * 
  *     def simulate(self, node:Node) -> dict:
  */
-      __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 119, __pyx_L5_except_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 166, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __PYX_ERR(0, 119, __pyx_L5_except_error)
+      __PYX_ERR(0, 166, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "multimcts/mcts.pyx":109
+    /* "multimcts/mcts.pyx":156
  *         Add a new child to this node.
  *         """
  *         try:             # <<<<<<<<<<<<<<
  *             move = node.remaining_moves.pop()
  *             child = Node(node.state.make_move(move), node)
  */
     __Pyx_XGIVEREF(__pyx_t_1);
@@ -3424,15 +4384,15 @@
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L0;
   }
 
-  /* "multimcts/mcts.pyx":105
+  /* "multimcts/mcts.pyx":152
  * 
  *     @staticmethod
  *     def expand(node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 2: Expansion
  *         Add a new child to this node.
  */
 
@@ -3449,15 +4409,15 @@
   __Pyx_XDECREF(__pyx_v_move);
   __Pyx_XDECREF(__pyx_v_child);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":121
+/* "multimcts/mcts.pyx":168
  *             raise Exception("Tried to expand a fully-expanded or terminal node.")
  * 
  *     def simulate(self, node:Node) -> dict:             # <<<<<<<<<<<<<<
  *         """Step 3: Simulation (aka playout, rollout)
  *         Play out a random game, from this node to termination, and return the final reward.
  */
 
@@ -3493,32 +4453,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("simulate", 1, 2, 2, 1); __PYX_ERR(0, 121, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("simulate", 1, 2, 2, 1); __PYX_ERR(0, 168, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "simulate") < 0)) __PYX_ERR(0, 121, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "simulate") < 0)) __PYX_ERR(0, 168, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_node = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("simulate", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 121, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("simulate", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 168, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.MCTS.simulate", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_8simulate(__pyx_self, __pyx_v_self, __pyx_v_node);
 
@@ -3545,114 +4505,114 @@
   int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("simulate", 0);
 
-  /* "multimcts/mcts.pyx":125
+  /* "multimcts/mcts.pyx":172
  *         Play out a random game, from this node to termination, and return the final reward.
  *         """
  *         state = node.state             # <<<<<<<<<<<<<<
  * 
  *         if node.is_terminal:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_state); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 125, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_state); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_state = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":127
+  /* "multimcts/mcts.pyx":174
  *         state = node.state
  * 
  *         if node.is_terminal:             # <<<<<<<<<<<<<<
  *             terminal_team = node.parent.state.get_current_team()
  *         else:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 127, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 174, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 127, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 174, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
-    /* "multimcts/mcts.pyx":128
+    /* "multimcts/mcts.pyx":175
  * 
  *         if node.is_terminal:
  *             terminal_team = node.parent.state.get_current_team()             # <<<<<<<<<<<<<<
  *         else:
  *             while not state.is_terminal():
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_parent); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 128, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_parent); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 175, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_state); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 128, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_state); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 175, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 128, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 175, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 128, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 175, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_terminal_team = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "multimcts/mcts.pyx":127
+    /* "multimcts/mcts.pyx":174
  *         state = node.state
  * 
  *         if node.is_terminal:             # <<<<<<<<<<<<<<
  *             terminal_team = node.parent.state.get_current_team()
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "multimcts/mcts.pyx":130
+  /* "multimcts/mcts.pyx":177
  *             terminal_team = node.parent.state.get_current_team()
  *         else:
  *             while not state.is_terminal():             # <<<<<<<<<<<<<<
  *                 try:
  *                     if self.heuristic is not None:
  */
   /*else*/ {
     while (1) {
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 130, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 177, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 130, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 130, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 177, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_5 = ((!__pyx_t_2) != 0);
       if (!__pyx_t_5) break;
 
-      /* "multimcts/mcts.pyx":131
+      /* "multimcts/mcts.pyx":178
  *         else:
  *             while not state.is_terminal():
  *                 try:             # <<<<<<<<<<<<<<
  *                     if self.heuristic is not None:
  *                         move = self.heuristic(state)
  */
       {
@@ -3660,96 +4620,96 @@
         __Pyx_PyThreadState_assign
         __Pyx_ExceptionSave(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8);
         __Pyx_XGOTREF(__pyx_t_6);
         __Pyx_XGOTREF(__pyx_t_7);
         __Pyx_XGOTREF(__pyx_t_8);
         /*try:*/ {
 
-          /* "multimcts/mcts.pyx":132
+          /* "multimcts/mcts.pyx":179
  *             while not state.is_terminal():
  *                 try:
  *                     if self.heuristic is not None:             # <<<<<<<<<<<<<<
  *                         move = self.heuristic(state)
  *                     else:
  */
-          __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_heuristic); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 132, __pyx_L6_error)
+          __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_heuristic); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L6_error)
           __Pyx_GOTREF(__pyx_t_1);
           __pyx_t_5 = (__pyx_t_1 != Py_None);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __pyx_t_2 = (__pyx_t_5 != 0);
           if (__pyx_t_2) {
 
-            /* "multimcts/mcts.pyx":133
+            /* "multimcts/mcts.pyx":180
  *                 try:
  *                     if self.heuristic is not None:
  *                         move = self.heuristic(state)             # <<<<<<<<<<<<<<
  *                     else:
  *                         move = state.get_random_move()
  */
-            __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_heuristic); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 133, __pyx_L6_error)
+            __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_heuristic); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 180, __pyx_L6_error)
             __Pyx_GOTREF(__pyx_t_3);
             __pyx_t_4 = NULL;
             if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
               __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
               if (likely(__pyx_t_4)) {
                 PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
                 __Pyx_INCREF(__pyx_t_4);
                 __Pyx_INCREF(function);
                 __Pyx_DECREF_SET(__pyx_t_3, function);
               }
             }
             __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_state) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_state);
             __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-            if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 133, __pyx_L6_error)
+            if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 180, __pyx_L6_error)
             __Pyx_GOTREF(__pyx_t_1);
             __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
             __Pyx_XDECREF_SET(__pyx_v_move, __pyx_t_1);
             __pyx_t_1 = 0;
 
-            /* "multimcts/mcts.pyx":132
+            /* "multimcts/mcts.pyx":179
  *             while not state.is_terminal():
  *                 try:
  *                     if self.heuristic is not None:             # <<<<<<<<<<<<<<
  *                         move = self.heuristic(state)
  *                     else:
  */
             goto __pyx_L14;
           }
 
-          /* "multimcts/mcts.pyx":135
+          /* "multimcts/mcts.pyx":182
  *                         move = self.heuristic(state)
  *                     else:
  *                         move = state.get_random_move()             # <<<<<<<<<<<<<<
  *                 except IndexError:#.forgot why this is an IndexError...
  *                     raise Exception("Non-terminal state has no legal moves.")
  */
           /*else*/ {
-            __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_random_move); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 135, __pyx_L6_error)
+            __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_random_move); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 182, __pyx_L6_error)
             __Pyx_GOTREF(__pyx_t_3);
             __pyx_t_4 = NULL;
             if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
               __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
               if (likely(__pyx_t_4)) {
                 PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
                 __Pyx_INCREF(__pyx_t_4);
                 __Pyx_INCREF(function);
                 __Pyx_DECREF_SET(__pyx_t_3, function);
               }
             }
             __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
             __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-            if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 135, __pyx_L6_error)
+            if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 182, __pyx_L6_error)
             __Pyx_GOTREF(__pyx_t_1);
             __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
             __Pyx_XDECREF_SET(__pyx_v_move, __pyx_t_1);
             __pyx_t_1 = 0;
           }
           __pyx_L14:;
 
-          /* "multimcts/mcts.pyx":131
+          /* "multimcts/mcts.pyx":178
  *         else:
  *             while not state.is_terminal():
  *                 try:             # <<<<<<<<<<<<<<
  *                     if self.heuristic is not None:
  *                         move = self.heuristic(state)
  */
         }
@@ -3758,192 +4718,192 @@
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
         goto __pyx_L13_try_end;
         __pyx_L6_error:;
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-        /* "multimcts/mcts.pyx":136
+        /* "multimcts/mcts.pyx":183
  *                     else:
  *                         move = state.get_random_move()
  *                 except IndexError:#.forgot why this is an IndexError...             # <<<<<<<<<<<<<<
  *                     raise Exception("Non-terminal state has no legal moves.")
  * 
  */
         __pyx_t_9 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_IndexError);
         if (__pyx_t_9) {
           __Pyx_AddTraceback("multimcts.mcts.MCTS.simulate", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_3, &__pyx_t_4) < 0) __PYX_ERR(0, 136, __pyx_L8_except_error)
+          if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_3, &__pyx_t_4) < 0) __PYX_ERR(0, 183, __pyx_L8_except_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_GOTREF(__pyx_t_4);
 
-          /* "multimcts/mcts.pyx":137
+          /* "multimcts/mcts.pyx":184
  *                         move = state.get_random_move()
  *                 except IndexError:#.forgot why this is an IndexError...
  *                     raise Exception("Non-terminal state has no legal moves.")             # <<<<<<<<<<<<<<
  * 
  *                 terminal_team = state.get_current_team()
  */
-          __pyx_t_10 = __Pyx_PyObject_Call(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 137, __pyx_L8_except_error)
+          __pyx_t_10 = __Pyx_PyObject_Call(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 184, __pyx_L8_except_error)
           __Pyx_GOTREF(__pyx_t_10);
           __Pyx_Raise(__pyx_t_10, 0, 0, 0);
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-          __PYX_ERR(0, 137, __pyx_L8_except_error)
+          __PYX_ERR(0, 184, __pyx_L8_except_error)
         }
         goto __pyx_L8_except_error;
         __pyx_L8_except_error:;
 
-        /* "multimcts/mcts.pyx":131
+        /* "multimcts/mcts.pyx":178
  *         else:
  *             while not state.is_terminal():
  *                 try:             # <<<<<<<<<<<<<<
  *                     if self.heuristic is not None:
  *                         move = self.heuristic(state)
  */
         __Pyx_XGIVEREF(__pyx_t_6);
         __Pyx_XGIVEREF(__pyx_t_7);
         __Pyx_XGIVEREF(__pyx_t_8);
         __Pyx_ExceptionReset(__pyx_t_6, __pyx_t_7, __pyx_t_8);
         goto __pyx_L1_error;
         __pyx_L13_try_end:;
       }
 
-      /* "multimcts/mcts.pyx":139
+      /* "multimcts/mcts.pyx":186
  *                     raise Exception("Non-terminal state has no legal moves.")
  * 
  *                 terminal_team = state.get_current_team()             # <<<<<<<<<<<<<<
  *                 state = state.make_move(move)
  * 
  */
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 139, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 186, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_1 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_1)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_1);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
       __pyx_t_4 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 139, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 186, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF_SET(__pyx_v_terminal_team, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "multimcts/mcts.pyx":140
+      /* "multimcts/mcts.pyx":187
  * 
  *                 terminal_team = state.get_current_team()
  *                 state = state.make_move(move)             # <<<<<<<<<<<<<<
  * 
  *         reward = state.get_reward()
  */
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_make_move); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 140, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_make_move); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 187, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_1 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_1)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_1);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
         }
       }
       __pyx_t_4 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_1, __pyx_v_move) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_move);
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 140, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 187, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF_SET(__pyx_v_state, __pyx_t_4);
       __pyx_t_4 = 0;
     }
   }
   __pyx_L3:;
 
-  /* "multimcts/mcts.pyx":142
+  /* "multimcts/mcts.pyx":189
  *                 state = state.make_move(move)
  * 
  *         reward = state.get_reward()             # <<<<<<<<<<<<<<
  *         if not isinstance(reward, dict):
  *             reward = {terminal_team: reward}
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_reward); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_reward); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_4 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 142, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_reward = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "multimcts/mcts.pyx":143
+  /* "multimcts/mcts.pyx":190
  * 
  *         reward = state.get_reward()
  *         if not isinstance(reward, dict):             # <<<<<<<<<<<<<<
  *             reward = {terminal_team: reward}
  * 
  */
   __pyx_t_2 = PyDict_Check(__pyx_v_reward); 
   __pyx_t_5 = ((!(__pyx_t_2 != 0)) != 0);
   if (__pyx_t_5) {
 
-    /* "multimcts/mcts.pyx":144
+    /* "multimcts/mcts.pyx":191
  *         reward = state.get_reward()
  *         if not isinstance(reward, dict):
  *             reward = {terminal_team: reward}             # <<<<<<<<<<<<<<
  * 
  *         return reward
  */
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 144, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 191, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (unlikely(!__pyx_v_terminal_team)) { __Pyx_RaiseUnboundLocalError("terminal_team"); __PYX_ERR(0, 144, __pyx_L1_error) }
-    if (PyDict_SetItem(__pyx_t_4, __pyx_v_terminal_team, __pyx_v_reward) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
+    if (unlikely(!__pyx_v_terminal_team)) { __Pyx_RaiseUnboundLocalError("terminal_team"); __PYX_ERR(0, 191, __pyx_L1_error) }
+    if (PyDict_SetItem(__pyx_t_4, __pyx_v_terminal_team, __pyx_v_reward) < 0) __PYX_ERR(0, 191, __pyx_L1_error)
     __Pyx_DECREF_SET(__pyx_v_reward, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "multimcts/mcts.pyx":143
+    /* "multimcts/mcts.pyx":190
  * 
  *         reward = state.get_reward()
  *         if not isinstance(reward, dict):             # <<<<<<<<<<<<<<
  *             reward = {terminal_team: reward}
  * 
  */
   }
 
-  /* "multimcts/mcts.pyx":146
+  /* "multimcts/mcts.pyx":193
  *             reward = {terminal_team: reward}
  * 
  *         return reward             # <<<<<<<<<<<<<<
  * 
  *     @staticmethod
  */
   __Pyx_XDECREF(__pyx_r);
-  if (!(likely(PyDict_CheckExact(__pyx_v_reward))||((__pyx_v_reward) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_v_reward)->tp_name), 0))) __PYX_ERR(0, 146, __pyx_L1_error)
+  if (!(likely(PyDict_CheckExact(__pyx_v_reward))||((__pyx_v_reward) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_v_reward)->tp_name), 0))) __PYX_ERR(0, 193, __pyx_L1_error)
   __Pyx_INCREF(__pyx_v_reward);
   __pyx_r = ((PyObject*)__pyx_v_reward);
   goto __pyx_L0;
 
-  /* "multimcts/mcts.pyx":121
+  /* "multimcts/mcts.pyx":168
  *             raise Exception("Tried to expand a fully-expanded or terminal node.")
  * 
  *     def simulate(self, node:Node) -> dict:             # <<<<<<<<<<<<<<
  *         """Step 3: Simulation (aka playout, rollout)
  *         Play out a random game, from this node to termination, and return the final reward.
  */
 
@@ -3961,15 +4921,15 @@
   __Pyx_XDECREF(__pyx_v_move);
   __Pyx_XDECREF(__pyx_v_reward);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":149
+/* "multimcts/mcts.pyx":196
  * 
  *     @staticmethod
  *     def backpropagate(node:Node, reward:dict):             # <<<<<<<<<<<<<<
  *         """Step 4: Backpropagation
  *         Update all ancestors with the reward from this terminal node.
  */
 
@@ -4005,38 +4965,38 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_reward)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("backpropagate", 1, 2, 2, 1); __PYX_ERR(0, 149, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("backpropagate", 1, 2, 2, 1); __PYX_ERR(0, 196, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "backpropagate") < 0)) __PYX_ERR(0, 149, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "backpropagate") < 0)) __PYX_ERR(0, 196, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_node = values[0];
     __pyx_v_reward = ((PyObject*)values[1]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("backpropagate", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 149, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("backpropagate", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 196, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.MCTS.backpropagate", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_reward), (&PyDict_Type), 1, "reward", 1))) __PYX_ERR(0, 149, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_reward), (&PyDict_Type), 1, "reward", 1))) __PYX_ERR(0, 196, __pyx_L1_error)
   __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_10backpropagate(__pyx_self, __pyx_v_node, __pyx_v_reward);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4067,126 +5027,126 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("backpropagate", 0);
   __Pyx_INCREF(__pyx_v_node);
   __Pyx_INCREF(__pyx_v_reward);
 
-  /* "multimcts/mcts.pyx":154
+  /* "multimcts/mcts.pyx":201
  *         """
  *         # Remove 0-values for efficiency
  *         reward = {k:v for k,v in reward.items() if v!=0}             # <<<<<<<<<<<<<<
  * 
  *         while node is not None:
  */
   { /* enter inner scope */
-    __pyx_t_1 = PyDict_New(); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L5_error)
+    __pyx_t_1 = PyDict_New(); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (unlikely(__pyx_v_reward == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-      __PYX_ERR(0, 154, __pyx_L5_error)
+      __PYX_ERR(0, 201, __pyx_L5_error)
     }
-    __pyx_t_2 = __Pyx_PyDict_Items(__pyx_v_reward); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 154, __pyx_L5_error)
+    __pyx_t_2 = __Pyx_PyDict_Items(__pyx_v_reward); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_2);
     if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
       __pyx_t_3 = __pyx_t_2; __Pyx_INCREF(__pyx_t_3); __pyx_t_4 = 0;
       __pyx_t_5 = NULL;
     } else {
-      __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 154, __pyx_L5_error)
+      __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 201, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_5 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 154, __pyx_L5_error)
+      __pyx_t_5 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 201, __pyx_L5_error)
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     for (;;) {
       if (likely(!__pyx_t_5)) {
         if (likely(PyList_CheckExact(__pyx_t_3))) {
           if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 154, __pyx_L5_error)
+          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 201, __pyx_L5_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 154, __pyx_L5_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         } else {
           if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 154, __pyx_L5_error)
+          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 201, __pyx_L5_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 154, __pyx_L5_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         }
       } else {
         __pyx_t_2 = __pyx_t_5(__pyx_t_3);
         if (unlikely(!__pyx_t_2)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 154, __pyx_L5_error)
+            else __PYX_ERR(0, 201, __pyx_L5_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_2);
       }
       if ((likely(PyTuple_CheckExact(__pyx_t_2))) || (PyList_CheckExact(__pyx_t_2))) {
         PyObject* sequence = __pyx_t_2;
         Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
         if (unlikely(size != 2)) {
           if (size > 2) __Pyx_RaiseTooManyValuesError(2);
           else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-          __PYX_ERR(0, 154, __pyx_L5_error)
+          __PYX_ERR(0, 201, __pyx_L5_error)
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         if (likely(PyTuple_CheckExact(sequence))) {
           __pyx_t_6 = PyTuple_GET_ITEM(sequence, 0); 
           __pyx_t_7 = PyTuple_GET_ITEM(sequence, 1); 
         } else {
           __pyx_t_6 = PyList_GET_ITEM(sequence, 0); 
           __pyx_t_7 = PyList_GET_ITEM(sequence, 1); 
         }
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_7);
         #else
-        __pyx_t_6 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 154, __pyx_L5_error)
+        __pyx_t_6 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_7 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 154, __pyx_L5_error)
+        __pyx_t_7 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_7);
         #endif
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       } else {
         Py_ssize_t index = -1;
-        __pyx_t_8 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 154, __pyx_L5_error)
+        __pyx_t_8 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 201, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_t_9 = Py_TYPE(__pyx_t_8)->tp_iternext;
         index = 0; __pyx_t_6 = __pyx_t_9(__pyx_t_8); if (unlikely(!__pyx_t_6)) goto __pyx_L8_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_6);
         index = 1; __pyx_t_7 = __pyx_t_9(__pyx_t_8); if (unlikely(!__pyx_t_7)) goto __pyx_L8_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_7);
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_8), 2) < 0) __PYX_ERR(0, 154, __pyx_L5_error)
+        if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_8), 2) < 0) __PYX_ERR(0, 201, __pyx_L5_error)
         __pyx_t_9 = NULL;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         goto __pyx_L9_unpacking_done;
         __pyx_L8_unpacking_failed:;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __pyx_t_9 = NULL;
         if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 154, __pyx_L5_error)
+        __PYX_ERR(0, 201, __pyx_L5_error)
         __pyx_L9_unpacking_done:;
       }
       __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_k, __pyx_t_6);
       __pyx_t_6 = 0;
       __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_v, __pyx_t_7);
       __pyx_t_7 = 0;
-      __pyx_t_2 = __Pyx_PyInt_NeObjC(__pyx_7genexpr__pyx_v_v, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 154, __pyx_L5_error)
+      __pyx_t_2 = __Pyx_PyInt_NeObjC(__pyx_7genexpr__pyx_v_v, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 154, __pyx_L5_error)
+      __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 201, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (__pyx_t_10) {
-        if (unlikely(PyDict_SetItem(__pyx_t_1, (PyObject*)__pyx_7genexpr__pyx_v_k, (PyObject*)__pyx_7genexpr__pyx_v_v))) __PYX_ERR(0, 154, __pyx_L5_error)
+        if (unlikely(PyDict_SetItem(__pyx_t_1, (PyObject*)__pyx_7genexpr__pyx_v_k, (PyObject*)__pyx_7genexpr__pyx_v_v))) __PYX_ERR(0, 201, __pyx_L5_error)
       }
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_k); __pyx_7genexpr__pyx_v_k = 0;
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_v); __pyx_7genexpr__pyx_v_v = 0;
     goto __pyx_L11_exit_scope;
     __pyx_L5_error:;
@@ -4194,102 +5154,102 @@
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_v); __pyx_7genexpr__pyx_v_v = 0;
     goto __pyx_L1_error;
     __pyx_L11_exit_scope:;
   } /* exit inner scope */
   __Pyx_DECREF_SET(__pyx_v_reward, ((PyObject*)__pyx_t_1));
   __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":156
+  /* "multimcts/mcts.pyx":203
  *         reward = {k:v for k,v in reward.items() if v!=0}
  * 
  *         while node is not None:             # <<<<<<<<<<<<<<
  *             node.num_visits += 1
  * 
  */
   while (1) {
     __pyx_t_10 = (__pyx_v_node != Py_None);
     __pyx_t_11 = (__pyx_t_10 != 0);
     if (!__pyx_t_11) break;
 
-    /* "multimcts/mcts.pyx":157
+    /* "multimcts/mcts.pyx":204
  * 
  *         while node is not None:
  *             node.num_visits += 1             # <<<<<<<<<<<<<<
  * 
  *             for key in reward:
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_num_visits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 157, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_num_visits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 204, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_t_1, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 157, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_t_1, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 204, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_node, __pyx_n_s_num_visits, __pyx_t_3) < 0) __PYX_ERR(0, 157, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_v_node, __pyx_n_s_num_visits, __pyx_t_3) < 0) __PYX_ERR(0, 204, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "multimcts/mcts.pyx":159
+    /* "multimcts/mcts.pyx":206
  *             node.num_visits += 1
  * 
  *             for key in reward:             # <<<<<<<<<<<<<<
  *                 node.total_reward[key] += reward[key]
  * 
  */
     __pyx_t_4 = 0;
-    __pyx_t_1 = __Pyx_dict_iterator(__pyx_v_reward, 1, ((PyObject *)NULL), (&__pyx_t_12), (&__pyx_t_13)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 159, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_dict_iterator(__pyx_v_reward, 1, ((PyObject *)NULL), (&__pyx_t_12), (&__pyx_t_13)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 206, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF(__pyx_t_3);
     __pyx_t_3 = __pyx_t_1;
     __pyx_t_1 = 0;
     while (1) {
       __pyx_t_14 = __Pyx_dict_iter_next(__pyx_t_3, __pyx_t_12, &__pyx_t_4, &__pyx_t_1, NULL, NULL, __pyx_t_13);
       if (unlikely(__pyx_t_14 == 0)) break;
-      if (unlikely(__pyx_t_14 == -1)) __PYX_ERR(0, 159, __pyx_L1_error)
+      if (unlikely(__pyx_t_14 == -1)) __PYX_ERR(0, 206, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "multimcts/mcts.pyx":160
+      /* "multimcts/mcts.pyx":207
  * 
  *             for key in reward:
  *                 node.total_reward[key] += reward[key]             # <<<<<<<<<<<<<<
  * 
  *             node = node.parent
  */
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_total_reward); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 160, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_total_reward); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_v_key);
       __pyx_t_2 = __pyx_v_key;
-      __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 160, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 207, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_6 = __Pyx_PyDict_GetItem(__pyx_v_reward, __pyx_v_key); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 160, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyDict_GetItem(__pyx_v_reward, __pyx_v_key); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 207, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_8 = PyNumber_InPlaceAdd(__pyx_t_7, __pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 160, __pyx_L1_error)
+      __pyx_t_8 = PyNumber_InPlaceAdd(__pyx_t_7, __pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 207, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_t_2, __pyx_t_8) < 0)) __PYX_ERR(0, 160, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_t_2, __pyx_t_8) < 0)) __PYX_ERR(0, 207, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "multimcts/mcts.pyx":162
+    /* "multimcts/mcts.pyx":209
  *                 node.total_reward[key] += reward[key]
  * 
  *             node = node.parent             # <<<<<<<<<<<<<<
  * 
  *     def get_best_child(self, node:Node) -> Node:
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_parent); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 162, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_parent); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 209, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF_SET(__pyx_v_node, __pyx_t_3);
     __pyx_t_3 = 0;
   }
 
-  /* "multimcts/mcts.pyx":149
+  /* "multimcts/mcts.pyx":196
  * 
  *     @staticmethod
  *     def backpropagate(node:Node, reward:dict):             # <<<<<<<<<<<<<<
  *         """Step 4: Backpropagation
  *         Update all ancestors with the reward from this terminal node.
  */
 
@@ -4312,15 +5272,15 @@
   __Pyx_XDECREF(__pyx_v_node);
   __Pyx_XDECREF(__pyx_v_reward);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":164
+/* "multimcts/mcts.pyx":211
  *             node = node.parent
  * 
  *     def get_best_child(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         cur_team = node.state.get_current_team()
  *         cdef float ln_parent_visits = log(node.num_visits)
  */
 
@@ -4355,46 +5315,46 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("get_best_child", 1, 2, 2, 1); __PYX_ERR(0, 164, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_best_child", 1, 2, 2, 1); __PYX_ERR(0, 211, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_best_child") < 0)) __PYX_ERR(0, 164, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_best_child") < 0)) __PYX_ERR(0, 211, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_node = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_best_child", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 164, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_best_child", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 211, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.MCTS.get_best_child", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_12get_best_child(__pyx_self, __pyx_v_self, __pyx_v_node);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_9multimcts_4mcts_4MCTS_14get_best_child_2generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "multimcts/mcts.pyx":177
+/* "multimcts/mcts.pyx":224
  *         for child in node.children.values():
  *             # Relative reward is this child's reward minus its siblings' rewards.
  *             reward = (2 * child.total_reward[cur_team]) - sum(x for x in child.total_reward.values())             # <<<<<<<<<<<<<<
  *             visits = child.num_visits
  * 
  */
 
@@ -4406,23 +5366,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct_1_genexpr *)__pyx_tp_new_9multimcts_4mcts___pyx_scope_struct_1_genexpr(__pyx_ptype_9multimcts_4mcts___pyx_scope_struct_1_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct_1_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 177, __pyx_L1_error)
+    __PYX_ERR(0, 224, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child *) __pyx_self;
   __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_outer_scope));
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_outer_scope);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_9multimcts_4mcts_4MCTS_14get_best_child_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_MCTS_get_best_child_locals_genex, __pyx_n_s_multimcts_mcts); if (unlikely(!gen)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_9multimcts_4mcts_4MCTS_14get_best_child_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_MCTS_get_best_child_locals_genex, __pyx_n_s_multimcts_mcts); if (unlikely(!gen)) __PYX_ERR(0, 224, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4452,71 +5412,71 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L6_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 177, __pyx_L1_error)
-  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_child)) { __Pyx_RaiseClosureNameError("child"); __PYX_ERR(0, 177, __pyx_L1_error) }
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_child, __pyx_n_s_total_reward); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 224, __pyx_L1_error)
+  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_child)) { __Pyx_RaiseClosureNameError("child"); __PYX_ERR(0, 224, __pyx_L1_error) }
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_child, __pyx_n_s_total_reward); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 224, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_values); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_values); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 224, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
     __pyx_t_3 = __pyx_t_1; __Pyx_INCREF(__pyx_t_3); __pyx_t_4 = 0;
     __pyx_t_5 = NULL;
   } else {
-    __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 224, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_5 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 224, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     if (likely(!__pyx_t_5)) {
       if (likely(PyList_CheckExact(__pyx_t_3))) {
         if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_3)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_1); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 177, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_1); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 224, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
         if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_1); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 177, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_1); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 224, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
       __pyx_t_1 = __pyx_t_5(__pyx_t_3);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 177, __pyx_L1_error)
+          else __PYX_ERR(0, 224, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_x);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_x, __pyx_t_1);
@@ -4536,15 +5496,15 @@
     return __pyx_r;
     __pyx_L6_resume_from_yield:;
     __pyx_t_3 = __pyx_cur_scope->__pyx_t_0;
     __pyx_cur_scope->__pyx_t_0 = 0;
     __Pyx_XGOTREF(__pyx_t_3);
     __pyx_t_4 = __pyx_cur_scope->__pyx_t_1;
     __pyx_t_5 = __pyx_cur_scope->__pyx_t_2;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 177, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 224, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
   /* function exit code */
   PyErr_SetNone(PyExc_StopIteration);
   goto __pyx_L0;
@@ -4560,15 +5520,15 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":164
+/* "multimcts/mcts.pyx":211
  *             node = node.parent
  * 
  *     def get_best_child(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         cur_team = node.state.get_current_team()
  *         cdef float ln_parent_visits = log(node.num_visits)
  */
 
@@ -4599,284 +5559,284 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_best_child", 0);
   __pyx_cur_scope = (struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child *)__pyx_tp_new_9multimcts_4mcts___pyx_scope_struct__get_best_child(__pyx_ptype_9multimcts_4mcts___pyx_scope_struct__get_best_child, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 164, __pyx_L1_error)
+    __PYX_ERR(0, 211, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
 
-  /* "multimcts/mcts.pyx":165
+  /* "multimcts/mcts.pyx":212
  * 
  *     def get_best_child(self, node:Node) -> Node:
  *         cur_team = node.state.get_current_team()             # <<<<<<<<<<<<<<
  *         cdef float ln_parent_visits = log(node.num_visits)
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_state); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_state); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 212, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 165, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 212, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 212, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_cur_team = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":166
+  /* "multimcts/mcts.pyx":213
  *     def get_best_child(self, node:Node) -> Node:
  *         cur_team = node.state.get_current_team()
  *         cdef float ln_parent_visits = log(node.num_visits)             # <<<<<<<<<<<<<<
  * 
  *         cdef float reward, score
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_num_visits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_num_visits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 213, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 166, __pyx_L1_error)
+  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 213, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_ln_parent_visits = log(__pyx_t_4);
 
-  /* "multimcts/mcts.pyx":170
+  /* "multimcts/mcts.pyx":217
  *         cdef float reward, score
  *         cdef int visits
  *         cdef float exploration_bias = self.exploration_bias             # <<<<<<<<<<<<<<
  * 
  *         cdef float max_score = float('-inf')
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_exploration_bias); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 170, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_exploration_bias); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 217, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __pyx_PyFloat_AsFloat(__pyx_t_1); if (unlikely((__pyx_t_5 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 170, __pyx_L1_error)
+  __pyx_t_5 = __pyx_PyFloat_AsFloat(__pyx_t_1); if (unlikely((__pyx_t_5 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 217, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_exploration_bias = __pyx_t_5;
 
-  /* "multimcts/mcts.pyx":172
+  /* "multimcts/mcts.pyx":219
  *         cdef float exploration_bias = self.exploration_bias
  * 
  *         cdef float max_score = float('-inf')             # <<<<<<<<<<<<<<
  *         best = None
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_AsDouble(__pyx_kp_s_inf); if (unlikely(__pyx_t_4 == ((double)((double)-1)) && PyErr_Occurred())) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_AsDouble(__pyx_kp_s_inf); if (unlikely(__pyx_t_4 == ((double)((double)-1)) && PyErr_Occurred())) __PYX_ERR(0, 219, __pyx_L1_error)
   __pyx_v_max_score = __pyx_t_4;
 
-  /* "multimcts/mcts.pyx":173
+  /* "multimcts/mcts.pyx":220
  * 
  *         cdef float max_score = float('-inf')
  *         best = None             # <<<<<<<<<<<<<<
  * 
  *         for child in node.children.values():
  */
   __Pyx_INCREF(Py_None);
   __pyx_v_best = Py_None;
 
-  /* "multimcts/mcts.pyx":175
+  /* "multimcts/mcts.pyx":222
  *         best = None
  * 
  *         for child in node.children.values():             # <<<<<<<<<<<<<<
  *             # Relative reward is this child's reward minus its siblings' rewards.
  *             reward = (2 * child.total_reward[cur_team]) - sum(x for x in child.total_reward.values())
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_children); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 175, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_children); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 222, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_values); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 175, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_values); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 222, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 175, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
     __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2); __pyx_t_6 = 0;
     __pyx_t_7 = NULL;
   } else {
-    __pyx_t_6 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 175, __pyx_L1_error)
+    __pyx_t_6 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 222, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_7 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 175, __pyx_L1_error)
+    __pyx_t_7 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 222, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     if (likely(!__pyx_t_7)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_1); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 175, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_1); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 222, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 175, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
         if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_1); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 175, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_1); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 222, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 175, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
       __pyx_t_1 = __pyx_t_7(__pyx_t_2);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 175, __pyx_L1_error)
+          else __PYX_ERR(0, 222, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_child);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_child, __pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "multimcts/mcts.pyx":177
+    /* "multimcts/mcts.pyx":224
  *         for child in node.children.values():
  *             # Relative reward is this child's reward minus its siblings' rewards.
  *             reward = (2 * child.total_reward[cur_team]) - sum(x for x in child.total_reward.values())             # <<<<<<<<<<<<<<
  *             visits = child.num_visits
  * 
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_child, __pyx_n_s_total_reward); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_child, __pyx_n_s_total_reward); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_cur_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_cur_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 224, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_Multiply(__pyx_int_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Multiply(__pyx_int_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __pyx_pf_9multimcts_4mcts_4MCTS_14get_best_child_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_3 = __pyx_pf_9multimcts_4mcts_4MCTS_14get_best_child_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 224, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_8 = __Pyx_PyObject_CallOneArg(__pyx_builtin_sum, __pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_CallOneArg(__pyx_builtin_sum, __pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 224, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyNumber_Subtract(__pyx_t_1, __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Subtract(__pyx_t_1, __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 224, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_5 = __pyx_PyFloat_AsFloat(__pyx_t_3); if (unlikely((__pyx_t_5 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_5 = __pyx_PyFloat_AsFloat(__pyx_t_3); if (unlikely((__pyx_t_5 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 224, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_reward = __pyx_t_5;
 
-    /* "multimcts/mcts.pyx":178
+    /* "multimcts/mcts.pyx":225
  *             # Relative reward is this child's reward minus its siblings' rewards.
  *             reward = (2 * child.total_reward[cur_team]) - sum(x for x in child.total_reward.values())
  *             visits = child.num_visits             # <<<<<<<<<<<<<<
  * 
  *             """UCB := (x / n) + C * sqrt(ln(N) / n)
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_child, __pyx_n_s_num_visits); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 178, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_child, __pyx_n_s_num_visits); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 225, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_9 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_9 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 178, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_9 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 225, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_visits = __pyx_t_9;
 
-    /* "multimcts/mcts.pyx":186
+    /* "multimcts/mcts.pyx":233
  *             C=exploration bias
  *             """
  *             score = (reward / visits) + exploration_bias * sqrt(ln_parent_visits / visits)             # <<<<<<<<<<<<<<
  * 
  *             if score > max_score:
  */
     if (unlikely(__pyx_v_visits == 0)) {
       PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 186, __pyx_L1_error)
+      __PYX_ERR(0, 233, __pyx_L1_error)
     }
     if (unlikely(__pyx_v_visits == 0)) {
       PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 186, __pyx_L1_error)
+      __PYX_ERR(0, 233, __pyx_L1_error)
     }
     __pyx_v_score = ((__pyx_v_reward / __pyx_v_visits) + (__pyx_v_exploration_bias * sqrt((__pyx_v_ln_parent_visits / __pyx_v_visits))));
 
-    /* "multimcts/mcts.pyx":188
+    /* "multimcts/mcts.pyx":235
  *             score = (reward / visits) + exploration_bias * sqrt(ln_parent_visits / visits)
  * 
  *             if score > max_score:             # <<<<<<<<<<<<<<
  *                 max_score = score
  *                 best = child
  */
     __pyx_t_10 = ((__pyx_v_score > __pyx_v_max_score) != 0);
     if (__pyx_t_10) {
 
-      /* "multimcts/mcts.pyx":189
+      /* "multimcts/mcts.pyx":236
  * 
  *             if score > max_score:
  *                 max_score = score             # <<<<<<<<<<<<<<
  *                 best = child
  * 
  */
       __pyx_v_max_score = __pyx_v_score;
 
-      /* "multimcts/mcts.pyx":190
+      /* "multimcts/mcts.pyx":237
  *             if score > max_score:
  *                 max_score = score
  *                 best = child             # <<<<<<<<<<<<<<
  * 
  *         return best
  */
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_child);
       __Pyx_DECREF_SET(__pyx_v_best, __pyx_cur_scope->__pyx_v_child);
 
-      /* "multimcts/mcts.pyx":188
+      /* "multimcts/mcts.pyx":235
  *             score = (reward / visits) + exploration_bias * sqrt(ln_parent_visits / visits)
  * 
  *             if score > max_score:             # <<<<<<<<<<<<<<
  *                 max_score = score
  *                 best = child
  */
     }
 
-    /* "multimcts/mcts.pyx":175
+    /* "multimcts/mcts.pyx":222
  *         best = None
  * 
  *         for child in node.children.values():             # <<<<<<<<<<<<<<
  *             # Relative reward is this child's reward minus its siblings' rewards.
  *             reward = (2 * child.total_reward[cur_team]) - sum(x for x in child.total_reward.values())
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "multimcts/mcts.pyx":192
+  /* "multimcts/mcts.pyx":239
  *                 best = child
  * 
  *         return best             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_best);
   __pyx_r = __pyx_v_best;
   goto __pyx_L0;
 
-  /* "multimcts/mcts.pyx":164
+  /* "multimcts/mcts.pyx":211
  *             node = node.parent
  * 
  *     def get_best_child(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         cur_team = node.state.get_current_team()
  *         cdef float ln_parent_visits = log(node.num_visits)
  */
 
@@ -5177,55 +6137,77 @@
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_n_s_Dict, __pyx_k_Dict, sizeof(__pyx_k_Dict), 0, 0, 1, 1},
   {&__pyx_n_s_GameState, __pyx_k_GameState, sizeof(__pyx_k_GameState), 0, 0, 1, 1},
+  {&__pyx_n_s_GameState___eq, __pyx_k_GameState___eq, sizeof(__pyx_k_GameState___eq), 0, 0, 1, 1},
+  {&__pyx_n_s_GameState___hash, __pyx_k_GameState___hash, sizeof(__pyx_k_GameState___hash), 0, 0, 1, 1},
+  {&__pyx_n_s_GameState_get_current_team, __pyx_k_GameState_get_current_team, sizeof(__pyx_k_GameState_get_current_team), 0, 0, 1, 1},
+  {&__pyx_n_s_GameState_get_legal_moves, __pyx_k_GameState_get_legal_moves, sizeof(__pyx_k_GameState_get_legal_moves), 0, 0, 1, 1},
+  {&__pyx_n_s_GameState_get_random_move, __pyx_k_GameState_get_random_move, sizeof(__pyx_k_GameState_get_random_move), 0, 0, 1, 1},
+  {&__pyx_n_s_GameState_get_reward, __pyx_k_GameState_get_reward, sizeof(__pyx_k_GameState_get_reward), 0, 0, 1, 1},
+  {&__pyx_n_s_GameState_has_move, __pyx_k_GameState_has_move, sizeof(__pyx_k_GameState_has_move), 0, 0, 1, 1},
+  {&__pyx_n_s_GameState_is_terminal, __pyx_k_GameState_is_terminal, sizeof(__pyx_k_GameState_is_terminal), 0, 0, 1, 1},
+  {&__pyx_n_s_GameState_make_move, __pyx_k_GameState_make_move, sizeof(__pyx_k_GameState_make_move), 0, 0, 1, 1},
+  {&__pyx_kp_s_GameState_must_implement___hash, __pyx_k_GameState_must_implement___hash, sizeof(__pyx_k_GameState_must_implement___hash), 0, 0, 1, 0},
+  {&__pyx_kp_s_GameState_must_implement_get_cur, __pyx_k_GameState_must_implement_get_cur, sizeof(__pyx_k_GameState_must_implement_get_cur), 0, 0, 1, 0},
+  {&__pyx_kp_s_GameState_must_implement_get_leg, __pyx_k_GameState_must_implement_get_leg, sizeof(__pyx_k_GameState_must_implement_get_leg), 0, 0, 1, 0},
+  {&__pyx_kp_s_GameState_must_implement_get_rew, __pyx_k_GameState_must_implement_get_rew, sizeof(__pyx_k_GameState_must_implement_get_rew), 0, 0, 1, 0},
+  {&__pyx_kp_s_GameState_must_implement_is_term, __pyx_k_GameState_must_implement_is_term, sizeof(__pyx_k_GameState_must_implement_is_term), 0, 0, 1, 0},
+  {&__pyx_kp_s_GameState_must_implement_make_mo, __pyx_k_GameState_must_implement_make_mo, sizeof(__pyx_k_GameState_must_implement_make_mo), 0, 0, 1, 0},
+  {&__pyx_kp_s_GameStates_must_implement___eq, __pyx_k_GameStates_must_implement___eq, sizeof(__pyx_k_GameStates_must_implement___eq), 0, 0, 1, 0},
   {&__pyx_n_s_Hashable, __pyx_k_Hashable, sizeof(__pyx_k_Hashable), 0, 0, 1, 1},
   {&__pyx_n_s_IndexError, __pyx_k_IndexError, sizeof(__pyx_k_IndexError), 0, 0, 1, 1},
+  {&__pyx_n_s_Iterator, __pyx_k_Iterator, sizeof(__pyx_k_Iterator), 0, 0, 1, 1},
   {&__pyx_n_s_MCTS, __pyx_k_MCTS, sizeof(__pyx_k_MCTS), 0, 0, 1, 1},
   {&__pyx_n_s_MCTS___init, __pyx_k_MCTS___init, sizeof(__pyx_k_MCTS___init), 0, 0, 1, 1},
   {&__pyx_n_s_MCTS_backpropagate, __pyx_k_MCTS_backpropagate, sizeof(__pyx_k_MCTS_backpropagate), 0, 0, 1, 1},
   {&__pyx_n_s_MCTS_expand, __pyx_k_MCTS_expand, sizeof(__pyx_k_MCTS_expand), 0, 0, 1, 1},
   {&__pyx_n_s_MCTS_get_best_child, __pyx_k_MCTS_get_best_child, sizeof(__pyx_k_MCTS_get_best_child), 0, 0, 1, 1},
   {&__pyx_n_s_MCTS_get_best_child_locals_genex, __pyx_k_MCTS_get_best_child_locals_genex, sizeof(__pyx_k_MCTS_get_best_child_locals_genex), 0, 0, 1, 1},
   {&__pyx_n_s_MCTS_search, __pyx_k_MCTS_search, sizeof(__pyx_k_MCTS_search), 0, 0, 1, 1},
   {&__pyx_n_s_MCTS_select, __pyx_k_MCTS_select, sizeof(__pyx_k_MCTS_select), 0, 0, 1, 1},
   {&__pyx_n_s_MCTS_simulate, __pyx_k_MCTS_simulate, sizeof(__pyx_k_MCTS_simulate), 0, 0, 1, 1},
   {&__pyx_n_s_Node, __pyx_k_Node, sizeof(__pyx_k_Node), 0, 0, 1, 1},
   {&__pyx_n_s_Node___init, __pyx_k_Node___init, sizeof(__pyx_k_Node___init), 0, 0, 1, 1},
   {&__pyx_kp_s_Non_terminal_state_has_no_legal, __pyx_k_Non_terminal_state_has_no_legal, sizeof(__pyx_k_Non_terminal_state_has_no_legal), 0, 0, 1, 0},
+  {&__pyx_n_s_NotImplementedError, __pyx_k_NotImplementedError, sizeof(__pyx_k_NotImplementedError), 0, 0, 1, 1},
   {&__pyx_kp_s_One_or_more_of_max_time_max_iter, __pyx_k_One_or_more_of_max_time_max_iter, sizeof(__pyx_k_One_or_more_of_max_time_max_iter), 0, 0, 1, 0},
   {&__pyx_kp_s_Represents_a_game_state_node_in, __pyx_k_Represents_a_game_state_node_in, sizeof(__pyx_k_Represents_a_game_state_node_in), 0, 0, 1, 0},
+  {&__pyx_n_s_StopIteration, __pyx_k_StopIteration, sizeof(__pyx_k_StopIteration), 0, 0, 1, 1},
   {&__pyx_kp_s_Tried_to_expand_a_fully_expanded, __pyx_k_Tried_to_expand_a_fully_expanded, sizeof(__pyx_k_Tried_to_expand_a_fully_expanded), 0, 0, 1, 0},
+  {&__pyx_n_s_Union, __pyx_k_Union, sizeof(__pyx_k_Union), 0, 0, 1, 1},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
   {&__pyx_n_s_backpropagate, __pyx_k_backpropagate, sizeof(__pyx_k_backpropagate), 0, 0, 1, 1},
   {&__pyx_n_s_best, __pyx_k_best, sizeof(__pyx_k_best), 0, 0, 1, 1},
   {&__pyx_n_s_child, __pyx_k_child, sizeof(__pyx_k_child), 0, 0, 1, 1},
   {&__pyx_n_s_children, __pyx_k_children, sizeof(__pyx_k_children), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_close, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
   {&__pyx_n_s_collections, __pyx_k_collections, sizeof(__pyx_k_collections), 0, 0, 1, 1},
   {&__pyx_n_s_cur_team, __pyx_k_cur_team, sizeof(__pyx_k_cur_team), 0, 0, 1, 1},
   {&__pyx_n_s_defaultdict, __pyx_k_defaultdict, sizeof(__pyx_k_defaultdict), 0, 0, 1, 1},
   {&__pyx_n_u_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 1, 0, 1},
   {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
   {&__pyx_n_s_end_time, __pyx_k_end_time, sizeof(__pyx_k_end_time), 0, 0, 1, 1},
+  {&__pyx_n_s_eq, __pyx_k_eq, sizeof(__pyx_k_eq), 0, 0, 1, 1},
   {&__pyx_n_s_expand, __pyx_k_expand, sizeof(__pyx_k_expand), 0, 0, 1, 1},
   {&__pyx_n_s_exploration_bias, __pyx_k_exploration_bias, sizeof(__pyx_k_exploration_bias), 0, 0, 1, 1},
   {&__pyx_n_u_float, __pyx_k_float, sizeof(__pyx_k_float), 0, 1, 0, 1},
-  {&__pyx_n_s_gamestate, __pyx_k_gamestate, sizeof(__pyx_k_gamestate), 0, 0, 1, 1},
   {&__pyx_n_s_genexpr, __pyx_k_genexpr, sizeof(__pyx_k_genexpr), 0, 0, 1, 1},
   {&__pyx_n_s_get_best_child, __pyx_k_get_best_child, sizeof(__pyx_k_get_best_child), 0, 0, 1, 1},
   {&__pyx_n_s_get_current_team, __pyx_k_get_current_team, sizeof(__pyx_k_get_current_team), 0, 0, 1, 1},
   {&__pyx_n_s_get_legal_moves, __pyx_k_get_legal_moves, sizeof(__pyx_k_get_legal_moves), 0, 0, 1, 1},
   {&__pyx_n_s_get_random_move, __pyx_k_get_random_move, sizeof(__pyx_k_get_random_move), 0, 0, 1, 1},
   {&__pyx_n_s_get_reward, __pyx_k_get_reward, sizeof(__pyx_k_get_reward), 0, 0, 1, 1},
+  {&__pyx_n_s_has_move, __pyx_k_has_move, sizeof(__pyx_k_has_move), 0, 0, 1, 1},
+  {&__pyx_n_s_hash, __pyx_k_hash, sizeof(__pyx_k_hash), 0, 0, 1, 1},
   {&__pyx_n_s_heuristic, __pyx_k_heuristic, sizeof(__pyx_k_heuristic), 0, 0, 1, 1},
   {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_kp_s_inf, __pyx_k_inf, sizeof(__pyx_k_inf), 0, 0, 1, 0},
   {&__pyx_n_s_init, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
   {&__pyx_n_u_int, __pyx_k_int, sizeof(__pyx_k_int), 0, 1, 0, 1},
   {&__pyx_n_s_is_fully_expanded, __pyx_k_is_fully_expanded, sizeof(__pyx_k_is_fully_expanded), 0, 0, 1, 1},
@@ -5243,18 +6225,20 @@
   {&__pyx_n_s_module, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
   {&__pyx_n_s_move, __pyx_k_move, sizeof(__pyx_k_move), 0, 0, 1, 1},
   {&__pyx_n_s_multimcts_mcts, __pyx_k_multimcts_mcts, sizeof(__pyx_k_multimcts_mcts), 0, 0, 1, 1},
   {&__pyx_kp_s_multimcts_mcts_pyx, __pyx_k_multimcts_mcts_pyx, sizeof(__pyx_k_multimcts_mcts_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_node, __pyx_k_node, sizeof(__pyx_k_node), 0, 0, 1, 1},
   {&__pyx_n_s_num_visits, __pyx_k_num_visits, sizeof(__pyx_k_num_visits), 0, 0, 1, 1},
+  {&__pyx_n_s_other, __pyx_k_other, sizeof(__pyx_k_other), 0, 0, 1, 1},
   {&__pyx_n_s_parent, __pyx_k_parent, sizeof(__pyx_k_parent), 0, 0, 1, 1},
   {&__pyx_n_s_pop, __pyx_k_pop, sizeof(__pyx_k_pop), 0, 0, 1, 1},
   {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
   {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
+  {&__pyx_n_s_randomize, __pyx_k_randomize, sizeof(__pyx_k_randomize), 0, 0, 1, 1},
   {&__pyx_n_s_remaining_moves, __pyx_k_remaining_moves, sizeof(__pyx_k_remaining_moves), 0, 0, 1, 1},
   {&__pyx_n_s_return, __pyx_k_return, sizeof(__pyx_k_return), 0, 0, 1, 1},
   {&__pyx_n_s_reward, __pyx_k_reward, sizeof(__pyx_k_reward), 0, 0, 1, 1},
   {&__pyx_n_s_score, __pyx_k_score, sizeof(__pyx_k_score), 0, 0, 1, 1},
   {&__pyx_n_s_search, __pyx_k_search, sizeof(__pyx_k_search), 0, 0, 1, 1},
   {&__pyx_n_s_select, __pyx_k_select, sizeof(__pyx_k_select), 0, 0, 1, 1},
   {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
@@ -5271,158 +6255,348 @@
   {&__pyx_n_s_typing, __pyx_k_typing, sizeof(__pyx_k_typing), 0, 0, 1, 1},
   {&__pyx_n_s_v, __pyx_k_v, sizeof(__pyx_k_v), 0, 0, 1, 1},
   {&__pyx_n_s_values, __pyx_k_values, sizeof(__pyx_k_values), 0, 0, 1, 1},
   {&__pyx_n_s_visits, __pyx_k_visits, sizeof(__pyx_k_visits), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_staticmethod = __Pyx_GetBuiltinName(__pyx_n_s_staticmethod); if (!__pyx_builtin_staticmethod) __PYX_ERR(0, 104, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 54, __pyx_L1_error)
-  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 118, __pyx_L1_error)
-  __pyx_builtin_sum = __Pyx_GetBuiltinName(__pyx_n_s_sum); if (!__pyx_builtin_sum) __PYX_ERR(0, 177, __pyx_L1_error)
+  __pyx_builtin_staticmethod = __Pyx_GetBuiltinName(__pyx_n_s_staticmethod); if (!__pyx_builtin_staticmethod) __PYX_ERR(0, 151, __pyx_L1_error)
+  __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 11, __pyx_L1_error)
+  __pyx_builtin_StopIteration = __Pyx_GetBuiltinName(__pyx_n_s_StopIteration); if (!__pyx_builtin_StopIteration) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 165, __pyx_L1_error)
+  __pyx_builtin_sum = __Pyx_GetBuiltinName(__pyx_n_s_sum); if (!__pyx_builtin_sum) __PYX_ERR(0, 224, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
+  /* "multimcts/mcts.pyx":11
+ *     def get_current_team(self) -> Union[int,str]:
+ *         """The identifier of the current player's team."""
+ *         raise NotImplementedError("GameState must implement get_current_team.")             # <<<<<<<<<<<<<<
+ * 
+ *     def get_legal_moves(self, randomize:bool=False) -> Iterator[Hashable]:
+ */
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_GameState_must_implement_get_cur); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 11, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple_);
+  __Pyx_GIVEREF(__pyx_tuple_);
+
+  /* "multimcts/mcts.pyx":17
+ *         The randomize param instructs the method to yield moves in a random order.
+ *         """
+ *         raise NotImplementedError("GameState must implement get_legal_moves.")             # <<<<<<<<<<<<<<
+ * 
+ *     def get_random_move(self) -> Hashable:
+ */
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_GameState_must_implement_get_leg); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__2);
+  __Pyx_GIVEREF(__pyx_tuple__2);
+
+  /* "multimcts/mcts.pyx":36
+ *         The current state object (self) should not be modified. Rather, modify a copy of it.
+ *         """
+ *         raise NotImplementedError("GameState must implement make_move.")             # <<<<<<<<<<<<<<
+ * 
+ *     def is_terminal(self) -> bool:
+ */
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_GameState_must_implement_make_mo); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
+
+  /* "multimcts/mcts.pyx":40
+ *     def is_terminal(self) -> bool:
+ *         """Checks if the game is over."""
+ *         raise NotImplementedError("GameState must implement is_terminal.")             # <<<<<<<<<<<<<<
+ * 
+ *     def get_reward(self) -> Union[float, Dict[Union[int,str], float]]:
+ */
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_GameState_must_implement_is_term); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__4);
+  __Pyx_GIVEREF(__pyx_tuple__4);
+
+  /* "multimcts/mcts.pyx":48
+ *         Note: This method is only evaluated on terminal states.
+ *         """
+ *         raise NotImplementedError("GameState must implement get_reward.")             # <<<<<<<<<<<<<<
+ * 
+ *     def __hash__(self) -> int:
+ */
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_GameState_must_implement_get_rew); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
+
+  /* "multimcts/mcts.pyx":51
+ * 
+ *     def __hash__(self) -> int:
+ *         raise NotImplementedError("GameState must implement __hash__")             # <<<<<<<<<<<<<<
+ * 
+ *     def __eq__(self, other:'GameState') -> bool:
+ */
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_GameState_must_implement___hash); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
+
   /* "multimcts/mcts.pyx":54
+ * 
+ *     def __eq__(self, other:'GameState') -> bool:
+ *         raise NotImplementedError("GameStates must implement __eq__")             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_GameStates_must_implement___eq); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
+
+  /* "multimcts/mcts.pyx":101
  *         """
  *         if max_iterations is None and max_time is None:
  *             raise ValueError("One or more of max_time/max_iterations is required.")             # <<<<<<<<<<<<<<
  * 
  *         self.exploration_bias = exploration_bias
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_One_or_more_of_max_time_max_iter); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 54, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple_);
-  __Pyx_GIVEREF(__pyx_tuple_);
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_One_or_more_of_max_time_max_iter); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "multimcts/mcts.pyx":119
+  /* "multimcts/mcts.pyx":166
  *             return child
  *         except IndexError:
  *             raise Exception("Tried to expand a fully-expanded or terminal node.")             # <<<<<<<<<<<<<<
  * 
  *     def simulate(self, node:Node) -> dict:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_Tried_to_expand_a_fully_expanded); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 119, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_Tried_to_expand_a_fully_expanded); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "multimcts/mcts.pyx":137
+  /* "multimcts/mcts.pyx":184
  *                         move = state.get_random_move()
  *                 except IndexError:#.forgot why this is an IndexError...
  *                     raise Exception("Non-terminal state has no legal moves.")             # <<<<<<<<<<<<<<
  * 
  *                 terminal_team = state.get_current_team()
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_Non_terminal_state_has_no_legal); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 137, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_Non_terminal_state_has_no_legal); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__10);
+  __Pyx_GIVEREF(__pyx_tuple__10);
+
+  /* "multimcts/mcts.pyx":9
+ * 
+ * class GameState():
+ *     def get_current_team(self) -> Union[int,str]:             # <<<<<<<<<<<<<<
+ *         """The identifier of the current player's team."""
+ *         raise NotImplementedError("GameState must implement get_current_team.")
+ */
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_current_team, 9, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 9, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":25
+  /* "multimcts/mcts.pyx":13
+ *         raise NotImplementedError("GameState must implement get_current_team.")
+ * 
+ *     def get_legal_moves(self, randomize:bool=False) -> Iterator[Hashable]:             # <<<<<<<<<<<<<<
+ *         """An iterator of all legal moves in this state.
+ *         The randomize param instructs the method to yield moves in a random order.
+ */
+  __pyx_tuple__13 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_randomize); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_legal_moves, 13, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(1, ((PyObject *)Py_False)); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
+
+  /* "multimcts/mcts.pyx":19
+ *         raise NotImplementedError("GameState must implement get_legal_moves.")
+ * 
+ *     def get_random_move(self) -> Hashable:             # <<<<<<<<<<<<<<
+ *         """Returns a random legal move from this state."""
+ *         return next(self.get_legal_moves(True))
+ */
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__16);
+  __Pyx_GIVEREF(__pyx_tuple__16);
+  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_random_move, 19, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 19, __pyx_L1_error)
+
+  /* "multimcts/mcts.pyx":23
+ *         return next(self.get_legal_moves(True))
+ * 
+ *     def has_move(self) -> bool:             # <<<<<<<<<<<<<<
+ *         """Returns whether there are any legal moves in this state."""
+ *         try:
+ */
+  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__18);
+  __Pyx_GIVEREF(__pyx_tuple__18);
+  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_has_move, 23, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 23, __pyx_L1_error)
+
+  /* "multimcts/mcts.pyx":31
+ *             return False
+ * 
+ *     def make_move(self, move:Hashable) -> 'GameState':             # <<<<<<<<<<<<<<
+ *         """Returns a new GameState, which is the result of applying the given move to this state.
+ *         This usually involves updating the board and advancing the player counter.
+ */
+  __pyx_tuple__20 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_move); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__20);
+  __Pyx_GIVEREF(__pyx_tuple__20);
+  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_make_move, 31, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 31, __pyx_L1_error)
+
+  /* "multimcts/mcts.pyx":38
+ *         raise NotImplementedError("GameState must implement make_move.")
+ * 
+ *     def is_terminal(self) -> bool:             # <<<<<<<<<<<<<<
+ *         """Checks if the game is over."""
+ *         raise NotImplementedError("GameState must implement is_terminal.")
+ */
+  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
+  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_is_terminal, 38, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 38, __pyx_L1_error)
+
+  /* "multimcts/mcts.pyx":42
+ *         raise NotImplementedError("GameState must implement is_terminal.")
+ * 
+ *     def get_reward(self) -> Union[float, Dict[Union[int,str], float]]:             # <<<<<<<<<<<<<<
+ *         """Returns the reward earned by the team that played the game-ending move.
+ *         Typically 1 for win, -1 for loss, 0 for draw.
+ */
+  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
+  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_reward, 42, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 42, __pyx_L1_error)
+
+  /* "multimcts/mcts.pyx":50
+ *         raise NotImplementedError("GameState must implement get_reward.")
+ * 
+ *     def __hash__(self) -> int:             # <<<<<<<<<<<<<<
+ *         raise NotImplementedError("GameState must implement __hash__")
+ * 
+ */
+  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__26);
+  __Pyx_GIVEREF(__pyx_tuple__26);
+  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_hash, 50, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 50, __pyx_L1_error)
+
+  /* "multimcts/mcts.pyx":53
+ *         raise NotImplementedError("GameState must implement __hash__")
+ * 
+ *     def __eq__(self, other:'GameState') -> bool:             # <<<<<<<<<<<<<<
+ *         raise NotImplementedError("GameStates must implement __eq__")
+ * 
+ */
+  __pyx_tuple__28 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_other); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__28);
+  __Pyx_GIVEREF(__pyx_tuple__28);
+  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_eq, 53, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 53, __pyx_L1_error)
+
+  /* "multimcts/mcts.pyx":72
  *         remaining_moves (list): A list of moves that have not yet been tried.
  *     """
  *     def __init__(self, state:GameState, parent:'Node'=None):             # <<<<<<<<<<<<<<
  *         self.state = state
  *         self.parent = parent
  */
-  __pyx_tuple__4 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_parent); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 25, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_init, 25, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 25, __pyx_L1_error)
-  __pyx_tuple__6 = PyTuple_Pack(1, ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 25, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
+  __pyx_tuple__30 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_parent); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__30);
+  __Pyx_GIVEREF(__pyx_tuple__30);
+  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_init, 72, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_tuple__32 = PyTuple_Pack(1, ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__32);
+  __Pyx_GIVEREF(__pyx_tuple__32);
 
-  /* "multimcts/mcts.pyx":40
+  /* "multimcts/mcts.pyx":87
  * 
  * class MCTS():
  *     def __init__(self, *, exploration_bias:float=1.414, heuristic=None, max_time:float=None, max_iterations:int=None):             # <<<<<<<<<<<<<<
  *         """Initializes an MCTS agent.
  * 
  */
-  __pyx_tuple__7 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_exploration_bias, __pyx_n_s_heuristic, __pyx_n_s_max_time, __pyx_n_s_max_iterations); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 40, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
-  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(1, 4, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_init, 40, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_tuple__33 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_exploration_bias, __pyx_n_s_heuristic, __pyx_n_s_max_time, __pyx_n_s_max_iterations); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__33);
+  __Pyx_GIVEREF(__pyx_tuple__33);
+  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(1, 4, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_init, 87, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 87, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":62
+  /* "multimcts/mcts.pyx":109
  *         self.max_iterations = max_iterations
  * 
  *     def search(self, state:GameState) -> GameState:             # <<<<<<<<<<<<<<
  *         """Searches for this state's best move until some limit has been reached.
  * 
  */
-  __pyx_tuple__9 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_node, __pyx_n_s_end_time, __pyx_n_s_i, __pyx_n_s_child, __pyx_n_s_reward); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 62, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
-  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(2, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_search, 62, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_tuple__35 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_node, __pyx_n_s_end_time, __pyx_n_s_i, __pyx_n_s_child, __pyx_n_s_reward); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__35);
+  __Pyx_GIVEREF(__pyx_tuple__35);
+  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(2, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_search, 109, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 109, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":91
+  /* "multimcts/mcts.pyx":138
  *         return self.get_best_child(node).state
  * 
  *     def select(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 1: Selection
  *         Traverse the tree for the node we most want to simulate.
  */
-  __pyx_tuple__11 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_node); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 91, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
-  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_select, 91, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __pyx_tuple__37 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_node); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(0, 138, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__37);
+  __Pyx_GIVEREF(__pyx_tuple__37);
+  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_select, 138, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(0, 138, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":105
+  /* "multimcts/mcts.pyx":152
  * 
  *     @staticmethod
  *     def expand(node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 2: Expansion
  *         Add a new child to this node.
  */
-  __pyx_tuple__13 = PyTuple_Pack(3, __pyx_n_s_node, __pyx_n_s_move, __pyx_n_s_child); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 105, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__13);
-  __Pyx_GIVEREF(__pyx_tuple__13);
-  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_expand, 105, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __pyx_tuple__39 = PyTuple_Pack(3, __pyx_n_s_node, __pyx_n_s_move, __pyx_n_s_child); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__39);
+  __Pyx_GIVEREF(__pyx_tuple__39);
+  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_expand, 152, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(0, 152, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":121
+  /* "multimcts/mcts.pyx":168
  *             raise Exception("Tried to expand a fully-expanded or terminal node.")
  * 
  *     def simulate(self, node:Node) -> dict:             # <<<<<<<<<<<<<<
  *         """Step 3: Simulation (aka playout, rollout)
  *         Play out a random game, from this node to termination, and return the final reward.
  */
-  __pyx_tuple__15 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_node, __pyx_n_s_state, __pyx_n_s_terminal_team, __pyx_n_s_move, __pyx_n_s_reward); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 121, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__15);
-  __Pyx_GIVEREF(__pyx_tuple__15);
-  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(2, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_simulate, 121, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 121, __pyx_L1_error)
+  __pyx_tuple__41 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_node, __pyx_n_s_state, __pyx_n_s_terminal_team, __pyx_n_s_move, __pyx_n_s_reward); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__41);
+  __Pyx_GIVEREF(__pyx_tuple__41);
+  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(2, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_simulate, 168, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 168, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":149
+  /* "multimcts/mcts.pyx":196
  * 
  *     @staticmethod
  *     def backpropagate(node:Node, reward:dict):             # <<<<<<<<<<<<<<
  *         """Step 4: Backpropagation
  *         Update all ancestors with the reward from this terminal node.
  */
-  __pyx_tuple__17 = PyTuple_Pack(5, __pyx_n_s_node, __pyx_n_s_reward, __pyx_n_s_key, __pyx_n_s_k, __pyx_n_s_v); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__17);
-  __Pyx_GIVEREF(__pyx_tuple__17);
-  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(2, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_backpropagate, 149, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_tuple__43 = PyTuple_Pack(5, __pyx_n_s_node, __pyx_n_s_reward, __pyx_n_s_key, __pyx_n_s_k, __pyx_n_s_v); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__43);
+  __Pyx_GIVEREF(__pyx_tuple__43);
+  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(2, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_backpropagate, 196, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 196, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":164
+  /* "multimcts/mcts.pyx":211
  *             node = node.parent
  * 
  *     def get_best_child(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         cur_team = node.state.get_current_team()
  *         cdef float ln_parent_visits = log(node.num_visits)
  */
-  __pyx_tuple__19 = PyTuple_Pack(13, __pyx_n_s_self, __pyx_n_s_node, __pyx_n_s_cur_team, __pyx_n_s_ln_parent_visits, __pyx_n_s_reward, __pyx_n_s_score, __pyx_n_s_visits, __pyx_n_s_exploration_bias, __pyx_n_s_max_score, __pyx_n_s_best, __pyx_n_s_child, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 164, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__19);
-  __Pyx_GIVEREF(__pyx_tuple__19);
-  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(2, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_best_child, 164, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 164, __pyx_L1_error)
+  __pyx_tuple__45 = PyTuple_Pack(13, __pyx_n_s_self, __pyx_n_s_node, __pyx_n_s_cur_team, __pyx_n_s_ln_parent_visits, __pyx_n_s_reward, __pyx_n_s_score, __pyx_n_s_visits, __pyx_n_s_exploration_bias, __pyx_n_s_max_score, __pyx_n_s_best, __pyx_n_s_child, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(0, 211, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__45);
+  __Pyx_GIVEREF(__pyx_tuple__45);
+  __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(2, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__45, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_best_child, 211, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(0, 211, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -5473,23 +6647,23 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_9multimcts_4mcts___pyx_scope_struct__get_best_child) < 0) __PYX_ERR(0, 164, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_9multimcts_4mcts___pyx_scope_struct__get_best_child) < 0) __PYX_ERR(0, 211, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_9multimcts_4mcts___pyx_scope_struct__get_best_child.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_9multimcts_4mcts___pyx_scope_struct__get_best_child.tp_dictoffset && __pyx_type_9multimcts_4mcts___pyx_scope_struct__get_best_child.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_9multimcts_4mcts___pyx_scope_struct__get_best_child.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_9multimcts_4mcts___pyx_scope_struct__get_best_child = &__pyx_type_9multimcts_4mcts___pyx_scope_struct__get_best_child;
-  if (PyType_Ready(&__pyx_type_9multimcts_4mcts___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 177, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_9multimcts_4mcts___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 224, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_9multimcts_4mcts___pyx_scope_struct_1_genexpr.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_9multimcts_4mcts___pyx_scope_struct_1_genexpr.tp_dictoffset && __pyx_type_9multimcts_4mcts___pyx_scope_struct_1_genexpr.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_9multimcts_4mcts___pyx_scope_struct_1_genexpr.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_9multimcts_4mcts___pyx_scope_struct_1_genexpr = &__pyx_type_9multimcts_4mcts___pyx_scope_struct_1_genexpr;
@@ -5618,14 +6792,17 @@
 #endif
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
@@ -5726,25 +6903,25 @@
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
   /* "multimcts/mcts.pyx":1
  * import time             # <<<<<<<<<<<<<<
  * from collections import defaultdict
- * from typing import Dict, Hashable
+ * from typing import Union, Iterator, Dict, Hashable
  */
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_time, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_time, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "multimcts/mcts.pyx":2
  * import time
  * from collections import defaultdict             # <<<<<<<<<<<<<<
- * from typing import Dict, Hashable
+ * from typing import Union, Iterator, Dict, Hashable
  * 
  */
   __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_defaultdict);
   __Pyx_GIVEREF(__pyx_n_s_defaultdict);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_defaultdict);
@@ -5756,336 +6933,585 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_defaultdict, __pyx_t_1) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "multimcts/mcts.pyx":3
  * import time
  * from collections import defaultdict
- * from typing import Dict, Hashable             # <<<<<<<<<<<<<<
+ * from typing import Union, Iterator, Dict, Hashable             # <<<<<<<<<<<<<<
  * 
  * from libc.math cimport log, sqrt
  */
-  __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_INCREF(__pyx_n_s_Union);
+  __Pyx_GIVEREF(__pyx_n_s_Union);
+  PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_Union);
+  __Pyx_INCREF(__pyx_n_s_Iterator);
+  __Pyx_GIVEREF(__pyx_n_s_Iterator);
+  PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_s_Iterator);
   __Pyx_INCREF(__pyx_n_s_Dict);
   __Pyx_GIVEREF(__pyx_n_s_Dict);
-  PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_Dict);
+  PyList_SET_ITEM(__pyx_t_2, 2, __pyx_n_s_Dict);
   __Pyx_INCREF(__pyx_n_s_Hashable);
   __Pyx_GIVEREF(__pyx_n_s_Hashable);
-  PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_s_Hashable);
+  PyList_SET_ITEM(__pyx_t_2, 3, __pyx_n_s_Hashable);
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_typing, __pyx_t_2, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Union); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Union, __pyx_t_2) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Iterator); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Iterator, __pyx_t_2) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Dict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Dict, __pyx_t_2) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Hashable); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Hashable, __pyx_t_2) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":7
- * from libc.math cimport log, sqrt
- * 
- * from gamestate import GameState             # <<<<<<<<<<<<<<
+  /* "multimcts/mcts.pyx":8
  * 
  * 
+ * class GameState():             # <<<<<<<<<<<<<<
+ *     def get_current_team(self) -> Union[int,str]:
+ *         """The identifier of the current player's team."""
  */
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_GameState, __pyx_n_s_GameState, (PyObject *) NULL, __pyx_n_s_multimcts_mcts, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_INCREF(__pyx_n_s_GameState);
-  __Pyx_GIVEREF(__pyx_n_s_GameState);
-  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_GameState);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_gamestate, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
+
+  /* "multimcts/mcts.pyx":9
+ * 
+ * class GameState():
+ *     def get_current_team(self) -> Union[int,str]:             # <<<<<<<<<<<<<<
+ *         """The identifier of the current player's team."""
+ *         raise NotImplementedError("GameState must implement get_current_team.")
+ */
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_GameState); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_GameState, __pyx_t_1) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Union); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_INCREF(((PyObject *)(&PyInt_Type)));
+  __Pyx_GIVEREF(((PyObject *)(&PyInt_Type)));
+  PyTuple_SET_ITEM(__pyx_t_4, 0, ((PyObject *)(&PyInt_Type)));
+  __Pyx_INCREF(((PyObject *)(&PyString_Type)));
+  __Pyx_GIVEREF(((PyObject *)(&PyString_Type)));
+  PyTuple_SET_ITEM(__pyx_t_4, 1, ((PyObject *)(&PyString_Type)));
+  __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_t_5) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_1get_current_team, 0, __pyx_n_s_GameState_get_current_team, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_2);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_current_team, __pyx_t_5) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+  /* "multimcts/mcts.pyx":13
+ *         raise NotImplementedError("GameState must implement get_current_team.")
+ * 
+ *     def get_legal_moves(self, randomize:bool=False) -> Iterator[Hashable]:             # <<<<<<<<<<<<<<
+ *         """An iterator of all legal moves in this state.
+ *         The randomize param instructs the method to yield moves in a random order.
+ */
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_randomize, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Iterator); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Hashable); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_t_3) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_3get_legal_moves, 0, __pyx_n_s_GameState_get_legal_moves, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__15);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_5);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_legal_moves, __pyx_t_3) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+  /* "multimcts/mcts.pyx":19
+ *         raise NotImplementedError("GameState must implement get_legal_moves.")
+ * 
+ *     def get_random_move(self) -> Hashable:             # <<<<<<<<<<<<<<
+ *         """Returns a random legal move from this state."""
+ *         return next(self.get_legal_moves(True))
+ */
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Hashable); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_t_5) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_5get_random_move, 0, __pyx_n_s_GameState_get_random_move, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_random_move, __pyx_t_5) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "multimcts/mcts.pyx":10
+  /* "multimcts/mcts.pyx":23
+ *         return next(self.get_legal_moves(True))
+ * 
+ *     def has_move(self) -> bool:             # <<<<<<<<<<<<<<
+ *         """Returns whether there are any legal moves in this state."""
+ *         try:
+ */
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_7has_move, 0, __pyx_n_s_GameState_has_move, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_5);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_has_move, __pyx_t_3) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+  /* "multimcts/mcts.pyx":31
+ *             return False
+ * 
+ *     def make_move(self, move:Hashable) -> 'GameState':             # <<<<<<<<<<<<<<
+ *         """Returns a new GameState, which is the result of applying the given move to this state.
+ *         This usually involves updating the board and advancing the player counter.
+ */
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Hashable); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_move, __pyx_t_5) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_GameState) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_9make_move, 0, __pyx_n_s_GameState_make_move, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_make_move, __pyx_t_5) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+  /* "multimcts/mcts.pyx":38
+ *         raise NotImplementedError("GameState must implement make_move.")
+ * 
+ *     def is_terminal(self) -> bool:             # <<<<<<<<<<<<<<
+ *         """Checks if the game is over."""
+ *         raise NotImplementedError("GameState must implement is_terminal.")
+ */
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_11is_terminal, 0, __pyx_n_s_GameState_is_terminal, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_5);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_is_terminal, __pyx_t_3) < 0) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+  /* "multimcts/mcts.pyx":42
+ *         raise NotImplementedError("GameState must implement is_terminal.")
+ * 
+ *     def get_reward(self) -> Union[float, Dict[Union[int,str], float]]:             # <<<<<<<<<<<<<<
+ *         """Returns the reward earned by the team that played the game-ending move.
+ *         Typically 1 for win, -1 for loss, 0 for draw.
+ */
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Union); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Dict); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Union); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_INCREF(((PyObject *)(&PyInt_Type)));
+  __Pyx_GIVEREF(((PyObject *)(&PyInt_Type)));
+  PyTuple_SET_ITEM(__pyx_t_6, 0, ((PyObject *)(&PyInt_Type)));
+  __Pyx_INCREF(((PyObject *)(&PyString_Type)));
+  __Pyx_GIVEREF(((PyObject *)(&PyString_Type)));
+  PyTuple_SET_ITEM(__pyx_t_6, 1, ((PyObject *)(&PyString_Type)));
+  __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_GIVEREF(__pyx_t_7);
+  PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_7);
+  __Pyx_INCREF(((PyObject *)(&PyFloat_Type)));
+  __Pyx_GIVEREF(((PyObject *)(&PyFloat_Type)));
+  PyTuple_SET_ITEM(__pyx_t_6, 1, ((PyObject *)(&PyFloat_Type)));
+  __pyx_t_7 = 0;
+  __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_INCREF(((PyObject *)(&PyFloat_Type)));
+  __Pyx_GIVEREF(((PyObject *)(&PyFloat_Type)));
+  PyTuple_SET_ITEM(__pyx_t_6, 0, ((PyObject *)(&PyFloat_Type)));
+  __Pyx_GIVEREF(__pyx_t_7);
+  PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_7);
+  __pyx_t_7 = 0;
+  __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_t_7) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_13get_reward, 0, __pyx_n_s_GameState_get_reward, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_3);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_reward, __pyx_t_7) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+
+  /* "multimcts/mcts.pyx":50
+ *         raise NotImplementedError("GameState must implement get_reward.")
+ * 
+ *     def __hash__(self) -> int:             # <<<<<<<<<<<<<<
+ *         raise NotImplementedError("GameState must implement __hash__")
+ * 
+ */
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_return, __pyx_n_u_int) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_15__hash__, 0, __pyx_n_s_GameState___hash, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_7);
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_hash, __pyx_t_3) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+  /* "multimcts/mcts.pyx":53
+ *         raise NotImplementedError("GameState must implement __hash__")
+ * 
+ *     def __eq__(self, other:'GameState') -> bool:             # <<<<<<<<<<<<<<
+ *         raise NotImplementedError("GameStates must implement __eq__")
+ * 
+ */
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_other, __pyx_n_s_GameState) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_17__eq__, 0, __pyx_n_s_GameState___eq, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_3);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_eq, __pyx_t_7) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+
+  /* "multimcts/mcts.pyx":8
+ * 
+ * 
+ * class GameState():             # <<<<<<<<<<<<<<
+ *     def get_current_team(self) -> Union[int,str]:
+ *         """The identifier of the current player's team."""
+ */
+  __pyx_t_7 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_GameState, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 8, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_GameState, __pyx_t_7) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "multimcts/mcts.pyx":57
  * 
  * 
  * class Node():             # <<<<<<<<<<<<<<
  *     """Represents a game state node in the MCTS search tree.
  * 
  */
-  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_Node, __pyx_n_s_Node, (PyObject *) NULL, __pyx_n_s_multimcts_mcts, __pyx_kp_s_Represents_a_game_state_node_in); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_Node, __pyx_n_s_Node, (PyObject *) NULL, __pyx_n_s_multimcts_mcts, __pyx_kp_s_Represents_a_game_state_node_in); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
 
-  /* "multimcts/mcts.pyx":25
+  /* "multimcts/mcts.pyx":72
  *         remaining_moves (list): A list of moves that have not yet been tried.
  *     """
  *     def __init__(self, state:GameState, parent:'Node'=None):             # <<<<<<<<<<<<<<
  *         self.state = state
  *         self.parent = parent
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_GameState); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_GameState); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_state, __pyx_t_3) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_state, __pyx_t_3) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_parent, __pyx_n_s_Node) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4Node_1__init__, 0, __pyx_n_s_Node___init, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_parent, __pyx_n_s_Node) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4Node_1__init__, 0, __pyx_n_s_Node___init, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__6);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_1);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_init, __pyx_t_3) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__32);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_7);
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_3) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "multimcts/mcts.pyx":10
+  /* "multimcts/mcts.pyx":57
  * 
  * 
  * class Node():             # <<<<<<<<<<<<<<
  *     """Represents a game state node in the MCTS search tree.
  * 
  */
-  __pyx_t_3 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_Node, __pyx_empty_tuple, __pyx_t_2, NULL, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_Node, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Node, __pyx_t_3) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Node, __pyx_t_3) < 0) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":39
+  /* "multimcts/mcts.pyx":86
  * 
  * 
  * class MCTS():             # <<<<<<<<<<<<<<
  *     def __init__(self, *, exploration_bias:float=1.414, heuristic=None, max_time:float=None, max_iterations:int=None):
  *         """Initializes an MCTS agent.
  */
-  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_MCTS, __pyx_n_s_MCTS, (PyObject *) NULL, __pyx_n_s_multimcts_mcts, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 39, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_MCTS, __pyx_n_s_MCTS, (PyObject *) NULL, __pyx_n_s_multimcts_mcts, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
 
-  /* "multimcts/mcts.pyx":40
+  /* "multimcts/mcts.pyx":87
  * 
  * class MCTS():
  *     def __init__(self, *, exploration_bias:float=1.414, heuristic=None, max_time:float=None, max_iterations:int=None):             # <<<<<<<<<<<<<<
  *         """Initializes an MCTS agent.
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = PyFloat_FromDouble(((double)1.414)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 40, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_exploration_bias, __pyx_t_1) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_heuristic, ((PyObject *)Py_None)) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_max_time, ((PyObject *)Py_None)) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_max_iterations, ((PyObject *)Py_None)) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 40, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_exploration_bias, __pyx_n_u_float) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_max_time, __pyx_n_u_float) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_max_iterations, __pyx_n_u_int) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_1__init__, 0, __pyx_n_s_MCTS___init, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 40, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_4, __pyx_t_3);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_1);
+  __pyx_t_7 = PyFloat_FromDouble(((double)1.414)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_exploration_bias, __pyx_t_7) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_heuristic, ((PyObject *)Py_None)) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_max_time, ((PyObject *)Py_None)) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_max_iterations, ((PyObject *)Py_None)) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_exploration_bias, __pyx_n_u_float) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_max_time, __pyx_n_u_float) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_max_iterations, __pyx_n_u_int) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_1__init__, 0, __pyx_n_s_MCTS___init, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_6, __pyx_t_3);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_6, __pyx_t_7);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_6) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "multimcts/mcts.pyx":62
+  /* "multimcts/mcts.pyx":109
  *         self.max_iterations = max_iterations
  * 
  *     def search(self, state:GameState) -> GameState:             # <<<<<<<<<<<<<<
  *         """Searches for this state's best move until some limit has been reached.
  * 
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 62, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_GameState); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_state, __pyx_t_1) < 0) __PYX_ERR(0, 62, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_GameState); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_t_1) < 0) __PYX_ERR(0, 62, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_3search, 0, __pyx_n_s_MCTS_search, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_1, __pyx_t_4);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_search, __pyx_t_1) < 0) __PYX_ERR(0, 62, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_GameState); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_state, __pyx_t_7) < 0) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_GameState); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_return, __pyx_t_7) < 0) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_3search, 0, __pyx_n_s_MCTS_search, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__36)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_6);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_search, __pyx_t_7) < 0) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "multimcts/mcts.pyx":91
+  /* "multimcts/mcts.pyx":138
  *         return self.get_best_child(node).state
  * 
  *     def select(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 1: Selection
  *         Traverse the tree for the node we most want to simulate.
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Node); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 91, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_node, __pyx_t_4) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Node); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 91, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_return, __pyx_t_4) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_5select, 0, __pyx_n_s_MCTS_select, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 91, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_1);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_select, __pyx_t_4) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 138, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Node); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 138, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_node, __pyx_t_6) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Node); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 138, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_return, __pyx_t_6) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_5select, 0, __pyx_n_s_MCTS_select, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__38)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 138, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_6, __pyx_t_7);
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_select, __pyx_t_6) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "multimcts/mcts.pyx":105
+  /* "multimcts/mcts.pyx":152
  * 
  *     @staticmethod
  *     def expand(node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 2: Expansion
  *         Add a new child to this node.
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 105, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Node); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_node, __pyx_t_1) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Node); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_t_1) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_7expand, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_MCTS_expand, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_1, __pyx_t_4);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Node); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_node, __pyx_t_7) < 0) __PYX_ERR(0, 152, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Node); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_return, __pyx_t_7) < 0) __PYX_ERR(0, 152, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_7expand, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_MCTS_expand, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__40)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_6);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "multimcts/mcts.pyx":104
+  /* "multimcts/mcts.pyx":151
  *         return node
  * 
  *     @staticmethod             # <<<<<<<<<<<<<<
  *     def expand(node:Node) -> Node:
  *         """Step 2: Expansion
  */
-  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 104, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_expand, __pyx_t_4) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 151, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_expand, __pyx_t_6) < 0) __PYX_ERR(0, 152, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "multimcts/mcts.pyx":121
+  /* "multimcts/mcts.pyx":168
  *             raise Exception("Tried to expand a fully-expanded or terminal node.")
  * 
  *     def simulate(self, node:Node) -> dict:             # <<<<<<<<<<<<<<
  *         """Step 3: Simulation (aka playout, rollout)
  *         Play out a random game, from this node to termination, and return the final reward.
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 121, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Node); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 121, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_node, __pyx_t_1) < 0) __PYX_ERR(0, 121, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_u_dict) < 0) __PYX_ERR(0, 121, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_9simulate, 0, __pyx_n_s_MCTS_simulate, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 121, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_1, __pyx_t_4);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_simulate, __pyx_t_1) < 0) __PYX_ERR(0, 121, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Node); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_node, __pyx_t_7) < 0) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_return, __pyx_n_u_dict) < 0) __PYX_ERR(0, 168, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_9simulate, 0, __pyx_n_s_MCTS_simulate, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__42)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_6);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_simulate, __pyx_t_7) < 0) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "multimcts/mcts.pyx":149
+  /* "multimcts/mcts.pyx":196
  * 
  *     @staticmethod
  *     def backpropagate(node:Node, reward:dict):             # <<<<<<<<<<<<<<
  *         """Step 4: Backpropagation
  *         Update all ancestors with the reward from this terminal node.
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Node); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_node, __pyx_t_4) < 0) __PYX_ERR(0, 149, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_reward, __pyx_n_u_dict) < 0) __PYX_ERR(0, 149, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_11backpropagate, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_MCTS_backpropagate, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_1);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Node); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_node, __pyx_t_6) < 0) __PYX_ERR(0, 196, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_reward, __pyx_n_u_dict) < 0) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_11backpropagate, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_MCTS_backpropagate, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_6, __pyx_t_7);
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "multimcts/mcts.pyx":148
+  /* "multimcts/mcts.pyx":195
  *         return reward
  * 
  *     @staticmethod             # <<<<<<<<<<<<<<
  *     def backpropagate(node:Node, reward:dict):
  *         """Step 4: Backpropagation
  */
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 148, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_backpropagate, __pyx_t_1) < 0) __PYX_ERR(0, 149, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 195, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_backpropagate, __pyx_t_7) < 0) __PYX_ERR(0, 196, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "multimcts/mcts.pyx":164
+  /* "multimcts/mcts.pyx":211
  *             node = node.parent
  * 
  *     def get_best_child(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         cur_team = node.state.get_current_team()
  *         cdef float ln_parent_visits = log(node.num_visits)
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Node); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 164, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_node, __pyx_t_4) < 0) __PYX_ERR(0, 164, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Node); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 164, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_return, __pyx_t_4) < 0) __PYX_ERR(0, 164, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_13get_best_child, 0, __pyx_n_s_MCTS_get_best_child, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 164, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_1);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_get_best_child, __pyx_t_4) < 0) __PYX_ERR(0, 164, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 211, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Node); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 211, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_node, __pyx_t_6) < 0) __PYX_ERR(0, 211, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Node); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 211, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_return, __pyx_t_6) < 0) __PYX_ERR(0, 211, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_13get_best_child, 0, __pyx_n_s_MCTS_get_best_child, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__46)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 211, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_6, __pyx_t_7);
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_best_child, __pyx_t_6) < 0) __PYX_ERR(0, 211, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "multimcts/mcts.pyx":39
+  /* "multimcts/mcts.pyx":86
  * 
  * 
  * class MCTS():             # <<<<<<<<<<<<<<
  *     def __init__(self, *, exploration_bias:float=1.414, heuristic=None, max_time:float=None, max_iterations:int=None):
  *         """Initializes an MCTS agent.
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_MCTS, __pyx_empty_tuple, __pyx_t_2, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 39, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_MCTS, __pyx_t_4) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_6 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_MCTS, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_MCTS, __pyx_t_6) < 0) __PYX_ERR(0, 86, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "multimcts/mcts.pyx":1
  * import time             # <<<<<<<<<<<<<<
  * from collections import defaultdict
- * from typing import Dict, Hashable
+ * from typing import Union, Iterator, Dict, Hashable
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
   if (__pyx_m) {
     if (__pyx_d) {
       __Pyx_AddTraceback("init multimcts.mcts", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
     PyErr_SetString(PyExc_ImportError, "init multimcts.mcts");
@@ -6143,39 +7569,216 @@
 #else
             "name '%.200s' is not defined", PyString_AS_STRING(name));
 #endif
     }
     return result;
 }
 
-/* RaiseArgTupleInvalid */
-static void __Pyx_RaiseArgtupleInvalid(
-    const char* func_name,
-    int exact,
-    Py_ssize_t num_min,
-    Py_ssize_t num_max,
-    Py_ssize_t num_found)
-{
-    Py_ssize_t num_expected;
-    const char *more_or_less;
-    if (num_found < num_min) {
-        num_expected = num_min;
-        more_or_less = "at least";
+/* PyObjectCall */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
+    PyObject *result;
+    ternaryfunc call = Py_TYPE(func)->tp_call;
+    if (unlikely(!call))
+        return PyObject_Call(func, arg, kw);
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
+        return NULL;
+    result = (*call)(func, arg, kw);
+    Py_LeaveRecursiveCall();
+    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
+        PyErr_SetString(
+            PyExc_SystemError,
+            "NULL result without error in PyObject_Call");
+    }
+    return result;
+}
+#endif
+
+/* PyErrFetchRestore */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    tmp_type = tstate->curexc_type;
+    tmp_value = tstate->curexc_value;
+    tmp_tb = tstate->curexc_traceback;
+    tstate->curexc_type = type;
+    tstate->curexc_value = value;
+    tstate->curexc_traceback = tb;
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+}
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+    *type = tstate->curexc_type;
+    *value = tstate->curexc_value;
+    *tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+}
+#endif
+
+/* RaiseException */
+#if PY_MAJOR_VERSION < 3
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
+                        CYTHON_UNUSED PyObject *cause) {
+    __Pyx_PyThreadState_declare
+    Py_XINCREF(type);
+    if (!value || value == Py_None)
+        value = NULL;
+    else
+        Py_INCREF(value);
+    if (!tb || tb == Py_None)
+        tb = NULL;
+    else {
+        Py_INCREF(tb);
+        if (!PyTraceBack_Check(tb)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: arg 3 must be a traceback or None");
+            goto raise_error;
+        }
+    }
+    if (PyType_Check(type)) {
+#if CYTHON_COMPILING_IN_PYPY
+        if (!value) {
+            Py_INCREF(Py_None);
+            value = Py_None;
+        }
+#endif
+        PyErr_NormalizeException(&type, &value, &tb);
     } else {
-        num_expected = num_max;
-        more_or_less = "at most";
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto raise_error;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(type);
+        Py_INCREF(type);
+        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: exception class must be a subclass of BaseException");
+            goto raise_error;
+        }
     }
-    if (exact) {
-        more_or_less = "exactly";
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrRestore(type, value, tb);
+    return;
+raise_error:
+    Py_XDECREF(value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+    return;
+}
+#else
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
+    PyObject* owned_instance = NULL;
+    if (tb == Py_None) {
+        tb = 0;
+    } else if (tb && !PyTraceBack_Check(tb)) {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: arg 3 must be a traceback or None");
+        goto bad;
     }
-    PyErr_Format(PyExc_TypeError,
-                 "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
-                 func_name, more_or_less, num_expected,
-                 (num_expected == 1) ? "" : "s", num_found);
+    if (value == Py_None)
+        value = 0;
+    if (PyExceptionInstance_Check(type)) {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto bad;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(value);
+    } else if (PyExceptionClass_Check(type)) {
+        PyObject *instance_class = NULL;
+        if (value && PyExceptionInstance_Check(value)) {
+            instance_class = (PyObject*) Py_TYPE(value);
+            if (instance_class != type) {
+                int is_subclass = PyObject_IsSubclass(instance_class, type);
+                if (!is_subclass) {
+                    instance_class = NULL;
+                } else if (unlikely(is_subclass == -1)) {
+                    goto bad;
+                } else {
+                    type = instance_class;
+                }
+            }
+        }
+        if (!instance_class) {
+            PyObject *args;
+            if (!value)
+                args = PyTuple_New(0);
+            else if (PyTuple_Check(value)) {
+                Py_INCREF(value);
+                args = value;
+            } else
+                args = PyTuple_Pack(1, value);
+            if (!args)
+                goto bad;
+            owned_instance = PyObject_Call(type, args, NULL);
+            Py_DECREF(args);
+            if (!owned_instance)
+                goto bad;
+            value = owned_instance;
+            if (!PyExceptionInstance_Check(value)) {
+                PyErr_Format(PyExc_TypeError,
+                             "calling %R should have returned an instance of "
+                             "BaseException, not %R",
+                             type, Py_TYPE(value));
+                goto bad;
+            }
+        }
+    } else {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: exception class must be a subclass of BaseException");
+        goto bad;
+    }
+    if (cause) {
+        PyObject *fixed_cause;
+        if (cause == Py_None) {
+            fixed_cause = NULL;
+        } else if (PyExceptionClass_Check(cause)) {
+            fixed_cause = PyObject_CallObject(cause, NULL);
+            if (fixed_cause == NULL)
+                goto bad;
+        } else if (PyExceptionInstance_Check(cause)) {
+            fixed_cause = cause;
+            Py_INCREF(fixed_cause);
+        } else {
+            PyErr_SetString(PyExc_TypeError,
+                            "exception causes must derive from "
+                            "BaseException");
+            goto bad;
+        }
+        PyException_SetCause(value, fixed_cause);
+    }
+    PyErr_SetObject(type, value);
+    if (tb) {
+#if CYTHON_FAST_THREAD_STATE
+        PyThreadState *tstate = __Pyx_PyThreadState_Current;
+        PyObject* tmp_tb = tstate->curexc_traceback;
+        if (tb != tmp_tb) {
+            Py_INCREF(tb);
+            tstate->curexc_traceback = tb;
+            Py_XDECREF(tmp_tb);
+        }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
+#endif
+    }
+bad:
+    Py_XDECREF(owned_instance);
+    return;
 }
+#endif
 
 /* RaiseDoubleKeywords */
 static void __Pyx_RaiseDoubleKeywordsError(
     const char* func_name,
     PyObject* kw_name)
 {
     PyErr_Format(PyExc_TypeError,
@@ -6285,87 +7888,93 @@
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
 bad:
     return -1;
 }
 
-/* PyObjectSetAttrStr */
-#if CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value) {
-    PyTypeObject* tp = Py_TYPE(obj);
-    if (likely(tp->tp_setattro))
-        return tp->tp_setattro(obj, attr_name, value);
-#if PY_MAJOR_VERSION < 3
-    if (likely(tp->tp_setattr))
-        return tp->tp_setattr(obj, PyString_AS_STRING(attr_name), value);
-#endif
-    return PyObject_SetAttr(obj, attr_name, value);
+/* RaiseArgTupleInvalid */
+static void __Pyx_RaiseArgtupleInvalid(
+    const char* func_name,
+    int exact,
+    Py_ssize_t num_min,
+    Py_ssize_t num_max,
+    Py_ssize_t num_found)
+{
+    Py_ssize_t num_expected;
+    const char *more_or_less;
+    if (num_found < num_min) {
+        num_expected = num_min;
+        more_or_less = "at least";
+    } else {
+        num_expected = num_max;
+        more_or_less = "at most";
+    }
+    if (exact) {
+        more_or_less = "exactly";
+    }
+    PyErr_Format(PyExc_TypeError,
+                 "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                 func_name, more_or_less, num_expected,
+                 (num_expected == 1) ? "" : "s", num_found);
 }
-#endif
 
-/* PyDictVersioning */
-#if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
-    PyObject *dict = Py_TYPE(obj)->tp_dict;
-    return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
-}
-static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj) {
-    PyObject **dictptr = NULL;
-    Py_ssize_t offset = Py_TYPE(obj)->tp_dictoffset;
-    if (offset) {
-#if CYTHON_COMPILING_IN_CPYTHON
-        dictptr = (likely(offset > 0)) ? (PyObject **) ((char *)obj + offset) : _PyObject_GetDictPtr(obj);
-#else
-        dictptr = _PyObject_GetDictPtr(obj);
-#endif
+/* IterNext */
+static PyObject *__Pyx_PyIter_Next2Default(PyObject* defval) {
+    PyObject* exc_type;
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    exc_type = __Pyx_PyErr_Occurred();
+    if (unlikely(exc_type)) {
+        if (!defval || unlikely(!__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration)))
+            return NULL;
+        __Pyx_PyErr_Clear();
+        Py_INCREF(defval);
+        return defval;
+    }
+    if (defval) {
+        Py_INCREF(defval);
+        return defval;
     }
-    return (dictptr && *dictptr) ? __PYX_GET_DICT_VERSION(*dictptr) : 0;
+    __Pyx_PyErr_SetNone(PyExc_StopIteration);
+    return NULL;
 }
-static CYTHON_INLINE int __Pyx_object_dict_version_matches(PyObject* obj, PY_UINT64_T tp_dict_version, PY_UINT64_T obj_dict_version) {
-    PyObject *dict = Py_TYPE(obj)->tp_dict;
-    if (unlikely(!dict) || unlikely(tp_dict_version != __PYX_GET_DICT_VERSION(dict)))
-        return 0;
-    return obj_dict_version == __Pyx_get_object_dict_version(obj);
+static void __Pyx_PyIter_Next_ErrorNoIterator(PyObject *iterator) {
+    PyErr_Format(PyExc_TypeError,
+        "%.200s object is not an iterator", Py_TYPE(iterator)->tp_name);
 }
-#endif
-
-/* GetModuleGlobalName */
-#if CYTHON_USE_DICT_VERSIONS
-static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value)
+static CYTHON_INLINE PyObject *__Pyx_PyIter_Next2(PyObject* iterator, PyObject* defval) {
+    PyObject* next;
+    iternextfunc iternext = Py_TYPE(iterator)->tp_iternext;
+    if (likely(iternext)) {
+#if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
+        next = iternext(iterator);
+        if (likely(next))
+            return next;
+        #if PY_VERSION_HEX >= 0x02070000 && CYTHON_COMPILING_IN_CPYTHON
+        if (unlikely(iternext == &_PyObject_NextNotImplemented))
+            return NULL;
+        #endif
 #else
-static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name)
+        next = PyIter_Next(iterator);
+        if (likely(next))
+            return next;
 #endif
-{
-    PyObject *result;
-#if !CYTHON_AVOID_BORROWED_REFS
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1
-    result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
-    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
-    if (likely(result)) {
-        return __Pyx_NewRef(result);
-    } else if (unlikely(PyErr_Occurred())) {
+    } else if (CYTHON_USE_TYPE_SLOTS || unlikely(!PyIter_Check(iterator))) {
+        __Pyx_PyIter_Next_ErrorNoIterator(iterator);
         return NULL;
     }
-#else
-    result = PyDict_GetItem(__pyx_d, name);
-    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
-    if (likely(result)) {
-        return __Pyx_NewRef(result);
-    }
-#endif
-#else
-    result = PyObject_GetItem(__pyx_d, name);
-    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
-    if (likely(result)) {
-        return __Pyx_NewRef(result);
+#if !CYTHON_USE_TYPE_SLOTS
+    else {
+        next = PyIter_Next(iterator);
+        if (likely(next))
+            return next;
     }
-    PyErr_Clear();
 #endif
-    return __Pyx_GetBuiltinName(name);
+    return __Pyx_PyIter_Next2Default(defval);
 }
 
 /* PyCFunctionFastCall */
 #if CYTHON_FAST_PYCCALL
 static CYTHON_INLINE PyObject * __Pyx_PyCFunction_FastCall(PyObject *func_obj, PyObject **args, Py_ssize_t nargs) {
     PyCFunctionObject *func = (PyCFunctionObject*)func_obj;
     PyCFunction meth = PyCFunction_GET_FUNCTION(func);
@@ -6502,34 +8111,14 @@
 done:
     Py_LeaveRecursiveCall();
     return result;
 }
 #endif
 #endif
 
-/* PyObjectCall */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
-    PyObject *result;
-    ternaryfunc call = Py_TYPE(func)->tp_call;
-    if (unlikely(!call))
-        return PyObject_Call(func, arg, kw);
-    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
-        return NULL;
-    result = (*call)(func, arg, kw);
-    Py_LeaveRecursiveCall();
-    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
-        PyErr_SetString(
-            PyExc_SystemError,
-            "NULL result without error in PyObject_Call");
-    }
-    return result;
-}
-#endif
-
 /* PyObjectCall2Args */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
     PyObject *args, *result = NULL;
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(function)) {
         PyObject *args[2] = {arg1, arg2};
         return __Pyx_PyFunction_FastCall(function, args, 2);
@@ -6633,196 +8222,243 @@
             return __Pyx_PyObject_CallMethO(func, NULL);
         }
     }
     return __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL);
 }
 #endif
 
-/* PyErrFetchRestore */
+/* GetTopmostException */
+#if CYTHON_USE_EXC_INFO_STACK
+static _PyErr_StackItem *
+__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
+{
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
+           exc_info->previous_item != NULL)
+    {
+        exc_info = exc_info->previous_item;
+    }
+    return exc_info;
+}
+#endif
+
+/* SaveResetException */
 #if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+    #if CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    *type = exc_info->exc_type;
+    *value = exc_info->exc_value;
+    *tb = exc_info->exc_traceback;
+    #else
+    *type = tstate->exc_type;
+    *value = tstate->exc_value;
+    *tb = tstate->exc_traceback;
+    #endif
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+}
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
     PyObject *tmp_type, *tmp_value, *tmp_tb;
-    tmp_type = tstate->curexc_type;
-    tmp_value = tstate->curexc_value;
-    tmp_tb = tstate->curexc_traceback;
-    tstate->curexc_type = type;
-    tstate->curexc_value = value;
-    tstate->curexc_traceback = tb;
+    #if CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    tmp_type = exc_info->exc_type;
+    tmp_value = exc_info->exc_value;
+    tmp_tb = exc_info->exc_traceback;
+    exc_info->exc_type = type;
+    exc_info->exc_value = value;
+    exc_info->exc_traceback = tb;
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = type;
+    tstate->exc_value = value;
+    tstate->exc_traceback = tb;
+    #endif
     Py_XDECREF(tmp_type);
     Py_XDECREF(tmp_value);
     Py_XDECREF(tmp_tb);
 }
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    *type = tstate->curexc_type;
-    *value = tstate->curexc_value;
-    *tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-}
 #endif
 
-/* RaiseException */
-#if PY_MAJOR_VERSION < 3
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
-                        CYTHON_UNUSED PyObject *cause) {
-    __Pyx_PyThreadState_declare
-    Py_XINCREF(type);
-    if (!value || value == Py_None)
-        value = NULL;
-    else
-        Py_INCREF(value);
-    if (!tb || tb == Py_None)
-        tb = NULL;
-    else {
-        Py_INCREF(tb);
-        if (!PyTraceBack_Check(tb)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: arg 3 must be a traceback or None");
-            goto raise_error;
-        }
+/* PyErrExceptionMatches */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
+    Py_ssize_t i, n;
+    n = PyTuple_GET_SIZE(tuple);
+#if PY_MAJOR_VERSION >= 3
+    for (i=0; i<n; i++) {
+        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
     }
-    if (PyType_Check(type)) {
-#if CYTHON_COMPILING_IN_PYPY
-        if (!value) {
-            Py_INCREF(Py_None);
-            value = Py_None;
-        }
 #endif
-        PyErr_NormalizeException(&type, &value, &tb);
-    } else {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto raise_error;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(type);
-        Py_INCREF(type);
-        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: exception class must be a subclass of BaseException");
-            goto raise_error;
-        }
+    for (i=0; i<n; i++) {
+        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
     }
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrRestore(type, value, tb);
-    return;
-raise_error:
-    Py_XDECREF(value);
-    Py_XDECREF(type);
-    Py_XDECREF(tb);
-    return;
+    return 0;
 }
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
+    PyObject *exc_type = tstate->curexc_type;
+    if (exc_type == err) return 1;
+    if (unlikely(!exc_type)) return 0;
+    if (unlikely(PyTuple_Check(err)))
+        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
+    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+}
+#endif
+
+/* GetException */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
 #else
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
-    PyObject* owned_instance = NULL;
-    if (tb == Py_None) {
-        tb = 0;
-    } else if (tb && !PyTraceBack_Check(tb)) {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: arg 3 must be a traceback or None");
-        goto bad;
-    }
-    if (value == Py_None)
-        value = 0;
-    if (PyExceptionInstance_Check(type)) {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto bad;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(value);
-    } else if (PyExceptionClass_Check(type)) {
-        PyObject *instance_class = NULL;
-        if (value && PyExceptionInstance_Check(value)) {
-            instance_class = (PyObject*) Py_TYPE(value);
-            if (instance_class != type) {
-                int is_subclass = PyObject_IsSubclass(instance_class, type);
-                if (!is_subclass) {
-                    instance_class = NULL;
-                } else if (unlikely(is_subclass == -1)) {
-                    goto bad;
-                } else {
-                    type = instance_class;
-                }
-            }
-        }
-        if (!instance_class) {
-            PyObject *args;
-            if (!value)
-                args = PyTuple_New(0);
-            else if (PyTuple_Check(value)) {
-                Py_INCREF(value);
-                args = value;
-            } else
-                args = PyTuple_Pack(1, value);
-            if (!args)
-                goto bad;
-            owned_instance = PyObject_Call(type, args, NULL);
-            Py_DECREF(args);
-            if (!owned_instance)
-                goto bad;
-            value = owned_instance;
-            if (!PyExceptionInstance_Check(value)) {
-                PyErr_Format(PyExc_TypeError,
-                             "calling %R should have returned an instance of "
-                             "BaseException, not %R",
-                             type, Py_TYPE(value));
-                goto bad;
-            }
-        }
-    } else {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: exception class must be a subclass of BaseException");
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
+#endif
+{
+    PyObject *local_type, *local_value, *local_tb;
+#if CYTHON_FAST_THREAD_STATE
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    local_type = tstate->curexc_type;
+    local_value = tstate->curexc_value;
+    local_tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+#else
+    PyErr_Fetch(&local_type, &local_value, &local_tb);
+#endif
+    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
+#if CYTHON_FAST_THREAD_STATE
+    if (unlikely(tstate->curexc_type))
+#else
+    if (unlikely(PyErr_Occurred()))
+#endif
         goto bad;
-    }
-    if (cause) {
-        PyObject *fixed_cause;
-        if (cause == Py_None) {
-            fixed_cause = NULL;
-        } else if (PyExceptionClass_Check(cause)) {
-            fixed_cause = PyObject_CallObject(cause, NULL);
-            if (fixed_cause == NULL)
-                goto bad;
-        } else if (PyExceptionInstance_Check(cause)) {
-            fixed_cause = cause;
-            Py_INCREF(fixed_cause);
-        } else {
-            PyErr_SetString(PyExc_TypeError,
-                            "exception causes must derive from "
-                            "BaseException");
+    #if PY_MAJOR_VERSION >= 3
+    if (local_tb) {
+        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
             goto bad;
-        }
-        PyException_SetCause(value, fixed_cause);
     }
-    PyErr_SetObject(type, value);
-    if (tb) {
+    #endif
+    Py_XINCREF(local_tb);
+    Py_XINCREF(local_type);
+    Py_XINCREF(local_value);
+    *type = local_type;
+    *value = local_value;
+    *tb = local_tb;
 #if CYTHON_FAST_THREAD_STATE
-        PyThreadState *tstate = __Pyx_PyThreadState_Current;
-        PyObject* tmp_tb = tstate->curexc_traceback;
-        if (tb != tmp_tb) {
-            Py_INCREF(tb);
-            tstate->curexc_traceback = tb;
-            Py_XDECREF(tmp_tb);
-        }
+    #if CYTHON_USE_EXC_INFO_STACK
+    {
+        _PyErr_StackItem *exc_info = tstate->exc_info;
+        tmp_type = exc_info->exc_type;
+        tmp_value = exc_info->exc_value;
+        tmp_tb = exc_info->exc_traceback;
+        exc_info->exc_type = local_type;
+        exc_info->exc_value = local_value;
+        exc_info->exc_traceback = local_tb;
+    }
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = local_type;
+    tstate->exc_value = local_value;
+    tstate->exc_traceback = local_tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
 #else
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
+    PyErr_SetExcInfo(local_type, local_value, local_tb);
 #endif
-    }
+    return 0;
 bad:
-    Py_XDECREF(owned_instance);
-    return;
+    *type = 0;
+    *value = 0;
+    *tb = 0;
+    Py_XDECREF(local_type);
+    Py_XDECREF(local_value);
+    Py_XDECREF(local_tb);
+    return -1;
 }
+
+/* PyObjectSetAttrStr */
+#if CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value) {
+    PyTypeObject* tp = Py_TYPE(obj);
+    if (likely(tp->tp_setattro))
+        return tp->tp_setattro(obj, attr_name, value);
+#if PY_MAJOR_VERSION < 3
+    if (likely(tp->tp_setattr))
+        return tp->tp_setattr(obj, PyString_AS_STRING(attr_name), value);
+#endif
+    return PyObject_SetAttr(obj, attr_name, value);
+}
+#endif
+
+/* PyDictVersioning */
+#if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
+    PyObject *dict = Py_TYPE(obj)->tp_dict;
+    return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
+}
+static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj) {
+    PyObject **dictptr = NULL;
+    Py_ssize_t offset = Py_TYPE(obj)->tp_dictoffset;
+    if (offset) {
+#if CYTHON_COMPILING_IN_CPYTHON
+        dictptr = (likely(offset > 0)) ? (PyObject **) ((char *)obj + offset) : _PyObject_GetDictPtr(obj);
+#else
+        dictptr = _PyObject_GetDictPtr(obj);
+#endif
+    }
+    return (dictptr && *dictptr) ? __PYX_GET_DICT_VERSION(*dictptr) : 0;
+}
+static CYTHON_INLINE int __Pyx_object_dict_version_matches(PyObject* obj, PY_UINT64_T tp_dict_version, PY_UINT64_T obj_dict_version) {
+    PyObject *dict = Py_TYPE(obj)->tp_dict;
+    if (unlikely(!dict) || unlikely(tp_dict_version != __PYX_GET_DICT_VERSION(dict)))
+        return 0;
+    return obj_dict_version == __Pyx_get_object_dict_version(obj);
+}
+#endif
+
+/* GetModuleGlobalName */
+#if CYTHON_USE_DICT_VERSIONS
+static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value)
+#else
+static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name)
+#endif
+{
+    PyObject *result;
+#if !CYTHON_AVOID_BORROWED_REFS
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1
+    result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
+    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
+    if (likely(result)) {
+        return __Pyx_NewRef(result);
+    } else if (unlikely(PyErr_Occurred())) {
+        return NULL;
+    }
+#else
+    result = PyDict_GetItem(__pyx_d, name);
+    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
+    if (likely(result)) {
+        return __Pyx_NewRef(result);
+    }
+#endif
+#else
+    result = PyObject_GetItem(__pyx_d, name);
+    __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
+    if (likely(result)) {
+        return __Pyx_NewRef(result);
+    }
+    PyErr_Clear();
 #endif
+    return __Pyx_GetBuiltinName(name);
+}
 
 /* None */
 static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname) {
     PyErr_Format(PyExc_UnboundLocalError, "local variable '%s' referenced before assignment", varname);
 }
 
 /* PyIntBinop */
@@ -7113,169 +8749,14 @@
         __Pyx_SET_SIZE(L, Py_SIZE(L) - 1);
         return PyList_GET_ITEM(L, PyList_GET_SIZE(L));
     }
     return __Pyx_CallUnboundCMethod0(&__pyx_umethod_PyList_Type_pop, L);
 }
 #endif
 
-/* GetTopmostException */
-#if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem *
-__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
-{
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
-           exc_info->previous_item != NULL)
-    {
-        exc_info = exc_info->previous_item;
-    }
-    return exc_info;
-}
-#endif
-
-/* SaveResetException */
-#if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
-    *type = exc_info->exc_type;
-    *value = exc_info->exc_value;
-    *tb = exc_info->exc_traceback;
-    #else
-    *type = tstate->exc_type;
-    *value = tstate->exc_value;
-    *tb = tstate->exc_traceback;
-    #endif
-    Py_XINCREF(*type);
-    Py_XINCREF(*value);
-    Py_XINCREF(*tb);
-}
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    tmp_type = exc_info->exc_type;
-    tmp_value = exc_info->exc_value;
-    tmp_tb = exc_info->exc_traceback;
-    exc_info->exc_type = type;
-    exc_info->exc_value = value;
-    exc_info->exc_traceback = tb;
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = type;
-    tstate->exc_value = value;
-    tstate->exc_traceback = tb;
-    #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-}
-#endif
-
-/* PyErrExceptionMatches */
-#if CYTHON_FAST_THREAD_STATE
-static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
-    Py_ssize_t i, n;
-    n = PyTuple_GET_SIZE(tuple);
-#if PY_MAJOR_VERSION >= 3
-    for (i=0; i<n; i++) {
-        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
-    }
-#endif
-    for (i=0; i<n; i++) {
-        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
-    }
-    return 0;
-}
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
-    PyObject *exc_type = tstate->curexc_type;
-    if (exc_type == err) return 1;
-    if (unlikely(!exc_type)) return 0;
-    if (unlikely(PyTuple_Check(err)))
-        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
-    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
-}
-#endif
-
-/* GetException */
-#if CYTHON_FAST_THREAD_STATE
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
-#else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
-#endif
-{
-    PyObject *local_type, *local_value, *local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    local_type = tstate->curexc_type;
-    local_value = tstate->curexc_value;
-    local_tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-#else
-    PyErr_Fetch(&local_type, &local_value, &local_tb);
-#endif
-    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
-#if CYTHON_FAST_THREAD_STATE
-    if (unlikely(tstate->curexc_type))
-#else
-    if (unlikely(PyErr_Occurred()))
-#endif
-        goto bad;
-    #if PY_MAJOR_VERSION >= 3
-    if (local_tb) {
-        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
-            goto bad;
-    }
-    #endif
-    Py_XINCREF(local_tb);
-    Py_XINCREF(local_type);
-    Py_XINCREF(local_value);
-    *type = local_type;
-    *value = local_value;
-    *tb = local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    #if CYTHON_USE_EXC_INFO_STACK
-    {
-        _PyErr_StackItem *exc_info = tstate->exc_info;
-        tmp_type = exc_info->exc_type;
-        tmp_value = exc_info->exc_value;
-        tmp_tb = exc_info->exc_traceback;
-        exc_info->exc_type = local_type;
-        exc_info->exc_value = local_value;
-        exc_info->exc_traceback = local_tb;
-    }
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = local_type;
-    tstate->exc_value = local_value;
-    tstate->exc_traceback = local_tb;
-    #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-#else
-    PyErr_SetExcInfo(local_type, local_value, local_tb);
-#endif
-    return 0;
-bad:
-    *type = 0;
-    *value = 0;
-    *tb = 0;
-    Py_XDECREF(local_type);
-    Py_XDECREF(local_value);
-    Py_XDECREF(local_tb);
-    return -1;
-}
-
 /* ArgTypeTest */
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
 {
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
         return 0;
     }
```

