# Comparing `tmp/multimcts-0.1.4.tar.gz` & `tmp/multimcts-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multimcts-0.1.4.tar", last modified: Mon Jul 17 23:05:38 2023, max compression
+gzip compressed data, was "multimcts-0.1.5.tar", last modified: Tue Jul 18 19:17:42 2023, max compression
```

## Comparing `multimcts-0.1.4.tar` & `multimcts-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-17 23:05:38.927591 multimcts-0.1.4/
--rw-r--r--   0 taylorvance   (501) staff       (20)       24 2023-07-17 19:47:43.000000 multimcts-0.1.4/MANIFEST.in
--rw-r--r--   0 taylorvance   (501) staff       (20)      228 2023-07-17 23:05:38.927327 multimcts-0.1.4/PKG-INFO
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-17 23:05:38.926192 multimcts-0.1.4/multimcts/
--rw-r--r--   0 taylorvance   (501) staff       (20)       34 2023-07-17 20:09:40.000000 multimcts-0.1.4/multimcts/__init__.py
--rw-r--r--   0 taylorvance   (501) staff       (20)   508596 2023-07-17 23:05:38.000000 multimcts-0.1.4/multimcts/mcts.c
--rw-r--r--   0 taylorvance   (501) staff       (20)     9301 2023-07-17 20:09:14.000000 multimcts-0.1.4/multimcts/mcts.pyx
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-17 23:05:38.927055 multimcts-0.1.4/multimcts.egg-info/
--rw-r--r--   0 taylorvance   (501) staff       (20)      228 2023-07-17 23:05:38.000000 multimcts-0.1.4/multimcts.egg-info/PKG-INFO
--rw-r--r--   0 taylorvance   (501) staff       (20)      257 2023-07-17 23:05:38.000000 multimcts-0.1.4/multimcts.egg-info/SOURCES.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-17 23:05:38.000000 multimcts-0.1.4/multimcts.egg-info/dependency_links.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-17 23:05:38.000000 multimcts-0.1.4/multimcts.egg-info/not-zip-safe
--rw-r--r--   0 taylorvance   (501) staff       (20)       10 2023-07-17 23:05:38.000000 multimcts-0.1.4/multimcts.egg-info/top_level.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)      100 2023-07-17 18:23:36.000000 multimcts-0.1.4/pyproject.toml
--rw-r--r--   0 taylorvance   (501) staff       (20)       38 2023-07-17 23:05:38.927703 multimcts-0.1.4/setup.cfg
--rw-r--r--   0 taylorvance   (501) staff       (20)      424 2023-07-17 23:05:11.000000 multimcts-0.1.4/setup.py
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-18 19:17:42.326682 multimcts-0.1.5/
+-rw-r--r--   0 taylorvance   (501) staff       (20)       24 2023-07-17 19:47:43.000000 multimcts-0.1.5/MANIFEST.in
+-rw-r--r--   0 taylorvance   (501) staff       (20)     1941 2023-07-18 19:17:42.326467 multimcts-0.1.5/PKG-INFO
+-rw-r--r--   0 taylorvance   (501) staff       (20)     1680 2023-07-18 19:13:45.000000 multimcts-0.1.5/README.md
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-18 19:17:42.324906 multimcts-0.1.5/multimcts/
+-rw-r--r--   0 taylorvance   (501) staff       (20)       34 2023-07-17 20:09:40.000000 multimcts-0.1.5/multimcts/__init__.py
+-rw-r--r--   0 taylorvance   (501) staff       (20)     2206 2023-07-17 13:17:49.000000 multimcts-0.1.5/multimcts/gamestate.pyx
+-rw-r--r--   0 taylorvance   (501) staff       (20)   507235 2023-07-18 19:15:18.000000 multimcts-0.1.5/multimcts/mcts.c
+-rw-r--r--   0 taylorvance   (501) staff       (20)     9383 2023-07-18 18:29:54.000000 multimcts-0.1.5/multimcts/mcts.pyx
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-18 19:17:42.326192 multimcts-0.1.5/multimcts.egg-info/
+-rw-r--r--   0 taylorvance   (501) staff       (20)     1941 2023-07-18 19:17:42.000000 multimcts-0.1.5/multimcts.egg-info/PKG-INFO
+-rw-r--r--   0 taylorvance   (501) staff       (20)      257 2023-07-17 23:05:38.000000 multimcts-0.1.5/multimcts.egg-info/SOURCES 2.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)      324 2023-07-18 19:17:42.000000 multimcts-0.1.5/multimcts.egg-info/SOURCES.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-18 19:17:42.000000 multimcts-0.1.5/multimcts.egg-info/dependency_links.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-17 19:12:04.000000 multimcts-0.1.5/multimcts.egg-info/not-zip-safe
+-rw-r--r--   0 taylorvance   (501) staff       (20)       10 2023-07-18 19:17:42.000000 multimcts-0.1.5/multimcts.egg-info/top_level.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)      100 2023-07-17 18:23:36.000000 multimcts-0.1.5/pyproject.toml
+-rw-r--r--   0 taylorvance   (501) staff       (20)       38 2023-07-18 19:17:42.326740 multimcts-0.1.5/setup.cfg
+-rw-r--r--   0 taylorvance   (501) staff       (20)      522 2023-07-18 19:17:36.000000 multimcts-0.1.5/setup.py
```

### Comparing `multimcts-0.1.4/multimcts/mcts.c` & `multimcts-0.1.5/multimcts/mcts.c`

 * *Files 1% similar despite different names*

```diff
@@ -973,28 +973,28 @@
   "multimcts/mcts.pyx",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child;
 struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct_1_genexpr;
 
-/* "multimcts/mcts.pyx":211
+/* "multimcts/mcts.pyx":213
  *             node = node.parent
  * 
  *     def get_best_child(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         cur_team = node.state.get_current_team()
- *         cdef float ln_parent_visits = log(node.num_visits)
+ * 
  */
 struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child {
   PyObject_HEAD
   PyObject *__pyx_v_child;
 };
 
 
-/* "multimcts/mcts.pyx":224
+/* "multimcts/mcts.pyx":227
  *         for child in node.children.values():
  *             # Relative reward is this child's reward minus its siblings' rewards.
  *             reward = (2 * child.total_reward[cur_team]) - sum(x for x in child.total_reward.values())             # <<<<<<<<<<<<<<
  *             visits = child.num_visits
  * 
  */
 struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct_1_genexpr {
@@ -1283,25 +1283,14 @@
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
-/* None.proto */
-static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname);
-
-/* PyIntBinop.proto */
-#if !CYTHON_COMPILING_IN_PYPY
-static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
-#else
-#define __Pyx_PyInt_AddObjC(op1, op2, intval, inplace, zerodivision_check)\
-    (inplace ? PyNumber_InPlaceAdd(op1, op2) : PyNumber_Add(op1, op2))
-#endif
-
 /* PyObjectGetMethod.proto */
 static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
 
 /* PyObjectCallMethod0.proto */
 static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name);
 
 /* pop.proto */
@@ -1340,14 +1329,17 @@
                ((cfunc)->flag == METH_VARARGS ?  (*((cfunc)->func))(self, __pyx_empty_tuple) :\
                __Pyx__CallUnboundCMethod0(cfunc, self)))))) :\
         __Pyx__CallUnboundCMethod0(cfunc, self))
 #else
 #define __Pyx_CallUnboundCMethod0(cfunc, self)  __Pyx__CallUnboundCMethod0(cfunc, self)
 #endif
 
+/* None.proto */
+static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname);
+
 /* ArgTypeTest.proto */
 #define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
     ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
 /* py_dict_items.proto */
@@ -1364,14 +1356,22 @@
 
 /* UnpackItemEndCheck.proto */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected);
 
 /* PyIntCompare.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_NeObjC(PyObject *op1, PyObject *op2, long intval, long inplace);
 
+/* PyIntBinop.proto */
+#if !CYTHON_COMPILING_IN_PYPY
+static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
+#else
+#define __Pyx_PyInt_AddObjC(op1, op2, intval, inplace, zerodivision_check)\
+    (inplace ? PyNumber_InPlaceAdd(op1, op2) : PyNumber_Add(op1, op2))
+#endif
+
 /* RaiseNoneIterError.proto */
 static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void);
 
 /* UnpackTupleError.proto */
 static void __Pyx_UnpackTupleError(PyObject *, Py_ssize_t index);
 
 /* UnpackTuple2.proto */
@@ -1716,15 +1716,14 @@
 static const char __pyx_k_eq[] = "__eq__";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_inf[] = "-inf";
 static const char __pyx_k_int[] = "int";
 static const char __pyx_k_key[] = "key";
 static const char __pyx_k_pop[] = "pop";
 static const char __pyx_k_sum[] = "sum";
-static const char __pyx_k_Dict[] = "Dict";
 static const char __pyx_k_MCTS[] = "MCTS";
 static const char __pyx_k_Node[] = "Node";
 static const char __pyx_k_args[] = "args";
 static const char __pyx_k_best[] = "best";
 static const char __pyx_k_dict[] = "dict";
 static const char __pyx_k_hash[] = "__hash__";
 static const char __pyx_k_init[] = "__init__";
@@ -1823,15 +1822,14 @@
 static const char __pyx_k_GameState_must_implement_get_leg[] = "GameState must implement get_legal_moves.";
 static const char __pyx_k_GameState_must_implement_get_rew[] = "GameState must implement get_reward.";
 static const char __pyx_k_GameState_must_implement_is_term[] = "GameState must implement is_terminal.";
 static const char __pyx_k_GameState_must_implement_make_mo[] = "GameState must implement make_move.";
 static const char __pyx_k_MCTS_get_best_child_locals_genex[] = "MCTS.get_best_child.<locals>.genexpr";
 static const char __pyx_k_One_or_more_of_max_time_max_iter[] = "One or more of max_time/max_iterations is required.";
 static const char __pyx_k_Tried_to_expand_a_fully_expanded[] = "Tried to expand a fully-expanded or terminal node.";
-static PyObject *__pyx_n_s_Dict;
 static PyObject *__pyx_n_s_GameState;
 static PyObject *__pyx_n_s_GameState___eq;
 static PyObject *__pyx_n_s_GameState___hash;
 static PyObject *__pyx_n_s_GameState_get_current_team;
 static PyObject *__pyx_n_s_GameState_get_legal_moves;
 static PyObject *__pyx_n_s_GameState_get_random_move;
 static PyObject *__pyx_n_s_GameState_get_reward;
@@ -2620,15 +2618,15 @@
   __Pyx_RefNannySetupContext("is_terminal", 0);
 
   /* "multimcts/mcts.pyx":40
  *     def is_terminal(self) -> bool:
  *         """Checks if the game is over."""
  *         raise NotImplementedError("GameState must implement is_terminal.")             # <<<<<<<<<<<<<<
  * 
- *     def get_reward(self) -> Union[float, Dict[Union[int,str], float]]:
+ *     def get_reward(self) -> Union[float, dict[Union[int,str], float]]:
  */
   __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(0, 40, __pyx_L1_error)
 
@@ -2649,15 +2647,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "multimcts/mcts.pyx":42
  *         raise NotImplementedError("GameState must implement is_terminal.")
  * 
- *     def get_reward(self) -> Union[float, Dict[Union[int,str], float]]:             # <<<<<<<<<<<<<<
+ *     def get_reward(self) -> Union[float, dict[Union[int,str], float]]:             # <<<<<<<<<<<<<<
  *         """Returns the reward earned by the team that played the game-ending move.
  *         Typically 1 for win, -1 for loss, 0 for draw.
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_9multimcts_4mcts_9GameState_13get_reward(PyObject *__pyx_self, PyObject *__pyx_v_self); /*proto*/
 static char __pyx_doc_9multimcts_4mcts_9GameState_12get_reward[] = "Returns the reward earned by the team that played the game-ending move.\n        Typically 1 for win, -1 for loss, 0 for draw.\n        Alternatively, returns a dict of format {team:reward} or {team1:reward1, team2:reward2, ...}\n        Note: This method is only evaluated on terminal states.\n        ";
@@ -2694,15 +2692,15 @@
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(0, 48, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":42
  *         raise NotImplementedError("GameState must implement is_terminal.")
  * 
- *     def get_reward(self) -> Union[float, Dict[Union[int,str], float]]:             # <<<<<<<<<<<<<<
+ *     def get_reward(self) -> Union[float, dict[Union[int,str], float]]:             # <<<<<<<<<<<<<<
  *         """Returns the reward earned by the team that played the game-ending move.
  *         Typically 1 for win, -1 for loss, 0 for draw.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -2999,41 +2997,41 @@
   if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_state, __pyx_v_state) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":74
  *     def __init__(self, state:GameState, parent:'Node'=None):
  *         self.state = state
  *         self.parent = parent             # <<<<<<<<<<<<<<
  * 
- *         self.children:Dict[Hashable,'Node'] = {}
+ *         self.children:dict[Hashable,'Node'] = {}
  */
   if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_parent, __pyx_v_parent) < 0) __PYX_ERR(0, 74, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":76
  *         self.parent = parent
  * 
- *         self.children:Dict[Hashable,'Node'] = {}             # <<<<<<<<<<<<<<
+ *         self.children:dict[Hashable,'Node'] = {}             # <<<<<<<<<<<<<<
  *         self.num_visits = 0
  *         self.total_reward = defaultdict(float)
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_children, __pyx_t_1) < 0) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "multimcts/mcts.pyx":77
  * 
- *         self.children:Dict[Hashable,'Node'] = {}
+ *         self.children:dict[Hashable,'Node'] = {}
  *         self.num_visits = 0             # <<<<<<<<<<<<<<
  *         self.total_reward = defaultdict(float)
  * 
  */
   if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_num_visits, __pyx_int_0) < 0) __PYX_ERR(0, 77, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":78
- *         self.children:Dict[Hashable,'Node'] = {}
+ *         self.children:dict[Hashable,'Node'] = {}
  *         self.num_visits = 0
  *         self.total_reward = defaultdict(float)             # <<<<<<<<<<<<<<
  * 
  *         self.is_terminal = self.state.is_terminal()
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_defaultdict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
@@ -3263,48 +3261,48 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
   /* "multimcts/mcts.pyx":100
  *             max_iterations (int): The maximum number of iterations that the search method should execute.
  *         """
- *         if max_iterations is None and max_time is None:             # <<<<<<<<<<<<<<
+ *         if max_time is None and max_iterations is None:             # <<<<<<<<<<<<<<
  *             raise ValueError("One or more of max_time/max_iterations is required.")
  * 
  */
-  __pyx_t_2 = (__pyx_v_max_iterations == Py_None);
+  __pyx_t_2 = (__pyx_v_max_time == Py_None);
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
   } else {
     __pyx_t_1 = __pyx_t_3;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_3 = (__pyx_v_max_time == Py_None);
+  __pyx_t_3 = (__pyx_v_max_iterations == Py_None);
   __pyx_t_2 = (__pyx_t_3 != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
     /* "multimcts/mcts.pyx":101
  *         """
- *         if max_iterations is None and max_time is None:
+ *         if max_time is None and max_iterations is None:
  *             raise ValueError("One or more of max_time/max_iterations is required.")             # <<<<<<<<<<<<<<
  * 
  *         self.exploration_bias = exploration_bias
  */
     __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 101, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __PYX_ERR(0, 101, __pyx_L1_error)
 
     /* "multimcts/mcts.pyx":100
  *             max_iterations (int): The maximum number of iterations that the search method should execute.
  *         """
- *         if max_iterations is None and max_time is None:             # <<<<<<<<<<<<<<
+ *         if max_time is None and max_iterations is None:             # <<<<<<<<<<<<<<
  *             raise ValueError("One or more of max_time/max_iterations is required.")
  * 
  */
   }
 
   /* "multimcts/mcts.pyx":103
  *             raise ValueError("One or more of max_time/max_iterations is required.")
@@ -3438,39 +3436,40 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_2search(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_state) {
   PyObject *__pyx_v_node = NULL;
-  PyObject *__pyx_v_end_time = NULL;
-  PyObject *__pyx_v_i = NULL;
+  float __pyx_v_end_time;
+  int __pyx_v_i;
   PyObject *__pyx_v_child = NULL;
   PyObject *__pyx_v_reward = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_t_5;
-  int __pyx_t_6;
-  PyObject *__pyx_t_7 = NULL;
-  int __pyx_t_8;
+  float __pyx_t_6;
+  int __pyx_t_7;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("search", 0);
 
   /* "multimcts/mcts.pyx":117
  *             GameState: A new game state which is the result of applying the best move to the given state.
  *         """
  *         node = Node(state)             # <<<<<<<<<<<<<<
  * 
- *         if self.max_time is not None:
+ *         cdef float end_time
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Node); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 117, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -3484,390 +3483,381 @@
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 117, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_node = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":119
- *         node = Node(state)
- * 
+  /* "multimcts/mcts.pyx":121
+ *         cdef float end_time
+ *         cdef int i
  *         if self.max_time is not None:             # <<<<<<<<<<<<<<
- *             end_time = time.time() + self.max_time
+ *             end_time = time() + self.max_time
  *         if self.max_iterations is not None:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_4 = (__pyx_t_1 != Py_None);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_5 = (__pyx_t_4 != 0);
   if (__pyx_t_5) {
 
-    /* "multimcts/mcts.pyx":120
- * 
+    /* "multimcts/mcts.pyx":122
+ *         cdef int i
  *         if self.max_time is not None:
- *             end_time = time.time() + self.max_time             # <<<<<<<<<<<<<<
+ *             end_time = time() + self.max_time             # <<<<<<<<<<<<<<
  *         if self.max_iterations is not None:
- *             i = 0
+ *             i = self.max_iterations
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 122, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 120, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-      __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
-      if (likely(__pyx_t_2)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-        __Pyx_INCREF(__pyx_t_2);
+    __pyx_t_3 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+      if (likely(__pyx_t_3)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+        __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_3, function);
+        __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
-    __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 120, __pyx_L1_error)
+    __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 122, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 120, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = PyNumber_Add(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 122, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_3 = PyNumber_Add(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 122, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_6 = __pyx_PyFloat_AsFloat(__pyx_t_3); if (unlikely((__pyx_t_6 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 122, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_v_end_time = __pyx_t_2;
-    __pyx_t_2 = 0;
+    __pyx_v_end_time = __pyx_t_6;
 
-    /* "multimcts/mcts.pyx":119
- *         node = Node(state)
- * 
+    /* "multimcts/mcts.pyx":121
+ *         cdef float end_time
+ *         cdef int i
  *         if self.max_time is not None:             # <<<<<<<<<<<<<<
- *             end_time = time.time() + self.max_time
+ *             end_time = time() + self.max_time
  *         if self.max_iterations is not None:
  */
   }
 
-  /* "multimcts/mcts.pyx":121
+  /* "multimcts/mcts.pyx":123
  *         if self.max_time is not None:
- *             end_time = time.time() + self.max_time
+ *             end_time = time() + self.max_time
  *         if self.max_iterations is not None:             # <<<<<<<<<<<<<<
- *             i = 0
+ *             i = self.max_iterations
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_iterations); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 121, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = (__pyx_t_2 != Py_None);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_iterations); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_5 = (__pyx_t_3 != Py_None);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_4 = (__pyx_t_5 != 0);
   if (__pyx_t_4) {
 
-    /* "multimcts/mcts.pyx":122
- *             end_time = time.time() + self.max_time
+    /* "multimcts/mcts.pyx":124
+ *             end_time = time() + self.max_time
  *         if self.max_iterations is not None:
- *             i = 0             # <<<<<<<<<<<<<<
+ *             i = self.max_iterations             # <<<<<<<<<<<<<<
  * 
  *         while True:
  */
-    __Pyx_INCREF(__pyx_int_0);
-    __pyx_v_i = __pyx_int_0;
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_iterations); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 124, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 124, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_v_i = __pyx_t_7;
 
-    /* "multimcts/mcts.pyx":121
+    /* "multimcts/mcts.pyx":123
  *         if self.max_time is not None:
- *             end_time = time.time() + self.max_time
+ *             end_time = time() + self.max_time
  *         if self.max_iterations is not None:             # <<<<<<<<<<<<<<
- *             i = 0
+ *             i = self.max_iterations
  * 
  */
   }
 
-  /* "multimcts/mcts.pyx":124
- *             i = 0
+  /* "multimcts/mcts.pyx":126
+ *             i = self.max_iterations
  * 
  *         while True:             # <<<<<<<<<<<<<<
  *             child = self.select(node)
  *             reward = self.simulate(child)
  */
   while (1) {
 
-    /* "multimcts/mcts.pyx":125
+    /* "multimcts/mcts.pyx":127
  * 
  *         while True:
  *             child = self.select(node)             # <<<<<<<<<<<<<<
  *             reward = self.simulate(child)
  *             self.backpropagate(child, reward)
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_select); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 125, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_select); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 127, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_1 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_1)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_1);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_3, function);
+        __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
-    __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_1, __pyx_v_node) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_node);
+    __pyx_t_3 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_1, __pyx_v_node) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_node);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 125, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_child, __pyx_t_2);
-    __pyx_t_2 = 0;
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 127, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_child, __pyx_t_3);
+    __pyx_t_3 = 0;
 
-    /* "multimcts/mcts.pyx":126
+    /* "multimcts/mcts.pyx":128
  *         while True:
  *             child = self.select(node)
  *             reward = self.simulate(child)             # <<<<<<<<<<<<<<
  *             self.backpropagate(child, reward)
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_simulate); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 126, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_simulate); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 128, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_1 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_1)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_1);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_3, function);
+        __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
-    __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_1, __pyx_v_child) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_child);
+    __pyx_t_3 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_1, __pyx_v_child) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_child);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 126, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_reward, __pyx_t_2);
-    __pyx_t_2 = 0;
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 128, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_reward, __pyx_t_3);
+    __pyx_t_3 = 0;
 
-    /* "multimcts/mcts.pyx":127
+    /* "multimcts/mcts.pyx":129
  *             child = self.select(node)
  *             reward = self.simulate(child)
  *             self.backpropagate(child, reward)             # <<<<<<<<<<<<<<
  * 
- *             if self.max_time is not None and time.time() >= end_time:
+ *             if self.max_time is not None and time() >= end_time:
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_backpropagate); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 127, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_backpropagate); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 129, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_1 = NULL;
-    __pyx_t_6 = 0;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
+    __pyx_t_7 = 0;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_1)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_1);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_3, function);
-        __pyx_t_6 = 1;
+        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __pyx_t_7 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(__pyx_t_3)) {
+    if (PyFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_1, __pyx_v_child, __pyx_v_reward};
-      __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 127, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_GOTREF(__pyx_t_3);
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
+    if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_1, __pyx_v_child, __pyx_v_reward};
-      __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 127, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_GOTREF(__pyx_t_3);
     } else
     #endif
     {
-      __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 127, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
+      __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 129, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
       if (__pyx_t_1) {
-        __Pyx_GIVEREF(__pyx_t_1); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_1); __pyx_t_1 = NULL;
+        __Pyx_GIVEREF(__pyx_t_1); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_1); __pyx_t_1 = NULL;
       }
       __Pyx_INCREF(__pyx_v_child);
       __Pyx_GIVEREF(__pyx_v_child);
-      PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_v_child);
+      PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_v_child);
       __Pyx_INCREF(__pyx_v_reward);
       __Pyx_GIVEREF(__pyx_v_reward);
-      PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_v_reward);
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 127, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_v_reward);
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "multimcts/mcts.pyx":129
+    /* "multimcts/mcts.pyx":131
  *             self.backpropagate(child, reward)
  * 
- *             if self.max_time is not None and time.time() >= end_time:             # <<<<<<<<<<<<<<
+ *             if self.max_time is not None and time() >= end_time:             # <<<<<<<<<<<<<<
  *                 break
  *             if self.max_iterations is not None:
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 129, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_5 = (__pyx_t_2 != Py_None);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_8 = (__pyx_t_5 != 0);
-    if (__pyx_t_8) {
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_5 = (__pyx_t_3 != Py_None);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_9 = (__pyx_t_5 != 0);
+    if (__pyx_t_9) {
     } else {
-      __pyx_t_4 = __pyx_t_8;
+      __pyx_t_4 = __pyx_t_9;
       goto __pyx_L8_bool_binop_done;
     }
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_time); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 129, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
-      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_7);
-      if (likely(__pyx_t_3)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
-        __Pyx_INCREF(__pyx_t_3);
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_8 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+      __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_2);
+      if (likely(__pyx_t_8)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+        __Pyx_INCREF(__pyx_t_8);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_7, function);
+        __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
-    __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_7);
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 129, __pyx_L1_error)
+    __pyx_t_3 = (__pyx_t_8) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_8) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
+    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_2 = PyFloat_FromDouble(__pyx_v_end_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_v_end_time)) { __Pyx_RaiseUnboundLocalError("end_time"); __PYX_ERR(0, 129, __pyx_L1_error) }
-    __pyx_t_7 = PyObject_RichCompare(__pyx_t_2, __pyx_v_end_time, Py_GE); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 129, __pyx_L1_error)
+    __pyx_t_8 = PyObject_RichCompare(__pyx_t_3, __pyx_t_2, Py_GE); __Pyx_XGOTREF(__pyx_t_8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 129, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_4 = __pyx_t_8;
+    __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __pyx_t_4 = __pyx_t_9;
     __pyx_L8_bool_binop_done:;
     if (__pyx_t_4) {
 
-      /* "multimcts/mcts.pyx":130
+      /* "multimcts/mcts.pyx":132
  * 
- *             if self.max_time is not None and time.time() >= end_time:
+ *             if self.max_time is not None and time() >= end_time:
  *                 break             # <<<<<<<<<<<<<<
  *             if self.max_iterations is not None:
- *                 i += 1
+ *                 i -= 1
  */
       goto __pyx_L6_break;
 
-      /* "multimcts/mcts.pyx":129
+      /* "multimcts/mcts.pyx":131
  *             self.backpropagate(child, reward)
  * 
- *             if self.max_time is not None and time.time() >= end_time:             # <<<<<<<<<<<<<<
+ *             if self.max_time is not None and time() >= end_time:             # <<<<<<<<<<<<<<
  *                 break
  *             if self.max_iterations is not None:
  */
     }
 
-    /* "multimcts/mcts.pyx":131
- *             if self.max_time is not None and time.time() >= end_time:
+    /* "multimcts/mcts.pyx":133
+ *             if self.max_time is not None and time() >= end_time:
  *                 break
  *             if self.max_iterations is not None:             # <<<<<<<<<<<<<<
- *                 i += 1
- *                 if i >= self.max_iterations:
+ *                 i -= 1
+ *                 if i <= 0:
  */
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_iterations); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 131, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_4 = (__pyx_t_7 != Py_None);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_8 = (__pyx_t_4 != 0);
-    if (__pyx_t_8) {
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_iterations); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 133, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_4 = (__pyx_t_8 != Py_None);
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __pyx_t_9 = (__pyx_t_4 != 0);
+    if (__pyx_t_9) {
 
-      /* "multimcts/mcts.pyx":132
+      /* "multimcts/mcts.pyx":134
  *                 break
  *             if self.max_iterations is not None:
- *                 i += 1             # <<<<<<<<<<<<<<
- *                 if i >= self.max_iterations:
+ *                 i -= 1             # <<<<<<<<<<<<<<
+ *                 if i <= 0:
  *                     break
  */
-      if (unlikely(!__pyx_v_i)) { __Pyx_RaiseUnboundLocalError("i"); __PYX_ERR(0, 132, __pyx_L1_error) }
-      __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_v_i, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 132, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_7);
-      __pyx_t_7 = 0;
+      __pyx_v_i = (__pyx_v_i - 1);
 
-      /* "multimcts/mcts.pyx":133
+      /* "multimcts/mcts.pyx":135
  *             if self.max_iterations is not None:
- *                 i += 1
- *                 if i >= self.max_iterations:             # <<<<<<<<<<<<<<
+ *                 i -= 1
+ *                 if i <= 0:             # <<<<<<<<<<<<<<
  *                     break
  * 
  */
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_iterations); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 133, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_2 = PyObject_RichCompare(__pyx_v_i, __pyx_t_7, Py_GE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 133, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 133, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (__pyx_t_8) {
+      __pyx_t_9 = ((__pyx_v_i <= 0) != 0);
+      if (__pyx_t_9) {
 
-        /* "multimcts/mcts.pyx":134
- *                 i += 1
- *                 if i >= self.max_iterations:
+        /* "multimcts/mcts.pyx":136
+ *                 i -= 1
+ *                 if i <= 0:
  *                     break             # <<<<<<<<<<<<<<
  * 
  *         return self.get_best_child(node).state
  */
         goto __pyx_L6_break;
 
-        /* "multimcts/mcts.pyx":133
+        /* "multimcts/mcts.pyx":135
  *             if self.max_iterations is not None:
- *                 i += 1
- *                 if i >= self.max_iterations:             # <<<<<<<<<<<<<<
+ *                 i -= 1
+ *                 if i <= 0:             # <<<<<<<<<<<<<<
  *                     break
  * 
  */
       }
 
-      /* "multimcts/mcts.pyx":131
- *             if self.max_time is not None and time.time() >= end_time:
+      /* "multimcts/mcts.pyx":133
+ *             if self.max_time is not None and time() >= end_time:
  *                 break
  *             if self.max_iterations is not None:             # <<<<<<<<<<<<<<
- *                 i += 1
- *                 if i >= self.max_iterations:
+ *                 i -= 1
+ *                 if i <= 0:
  */
     }
   }
   __pyx_L6_break:;
 
-  /* "multimcts/mcts.pyx":136
+  /* "multimcts/mcts.pyx":138
  *                     break
  * 
  *         return self.get_best_child(node).state             # <<<<<<<<<<<<<<
  * 
  *     def select(self, node:Node) -> Node:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_get_best_child); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 136, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_get_best_child); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 138, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_7);
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_7, function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_3, __pyx_v_node) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_v_node);
+  __pyx_t_8 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_node) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_node);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_state); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 136, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
+  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 138, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_r = __pyx_t_7;
-  __pyx_t_7 = 0;
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_state); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 138, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_r = __pyx_t_2;
+  __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* "multimcts/mcts.pyx":109
  *         self.max_iterations = max_iterations
  * 
  *     def search(self, state:GameState) -> GameState:             # <<<<<<<<<<<<<<
  *         """Searches for this state's best move until some limit has been reached.
@@ -3875,29 +3865,27 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
   __Pyx_AddTraceback("multimcts.mcts.MCTS.search", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_node);
-  __Pyx_XDECREF(__pyx_v_end_time);
-  __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XDECREF(__pyx_v_child);
   __Pyx_XDECREF(__pyx_v_reward);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":138
+/* "multimcts/mcts.pyx":140
  *         return self.get_best_child(node).state
  * 
  *     def select(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 1: Selection
  *         Traverse the tree for the node we most want to simulate.
  */
 
@@ -3933,32 +3921,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("select", 1, 2, 2, 1); __PYX_ERR(0, 138, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("select", 1, 2, 2, 1); __PYX_ERR(0, 140, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "select") < 0)) __PYX_ERR(0, 138, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "select") < 0)) __PYX_ERR(0, 140, __pyx_L3_error)
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
-  __Pyx_RaiseArgtupleInvalid("select", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 138, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("select", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 140, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.MCTS.select", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_4select(__pyx_self, __pyx_v_self, __pyx_v_node);
 
@@ -3977,124 +3965,124 @@
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("select", 0);
   __Pyx_INCREF(__pyx_v_node);
 
-  /* "multimcts/mcts.pyx":143
+  /* "multimcts/mcts.pyx":145
  *         Looks for an unexplored child of this node's best child's best child's...best child.
  *         """
  *         while not node.is_terminal:             # <<<<<<<<<<<<<<
  *             if not node.is_fully_expanded:
  *                 return self.expand(node)
  */
   while (1) {
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 145, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 143, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 145, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_3 = ((!__pyx_t_2) != 0);
     if (!__pyx_t_3) break;
 
-    /* "multimcts/mcts.pyx":144
+    /* "multimcts/mcts.pyx":146
  *         """
  *         while not node.is_terminal:
  *             if not node.is_fully_expanded:             # <<<<<<<<<<<<<<
  *                 return self.expand(node)
  *             else:
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_is_fully_expanded); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_is_fully_expanded); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 146, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 144, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 146, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_2 = ((!__pyx_t_3) != 0);
     if (__pyx_t_2) {
 
-      /* "multimcts/mcts.pyx":145
+      /* "multimcts/mcts.pyx":147
  *         while not node.is_terminal:
  *             if not node.is_fully_expanded:
  *                 return self.expand(node)             # <<<<<<<<<<<<<<
  *             else:
  *                 node = self.get_best_child(node)
  */
       __Pyx_XDECREF(__pyx_r);
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_expand); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 145, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_expand); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 147, __pyx_L1_error)
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
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 145, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 147, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_r = __pyx_t_1;
       __pyx_t_1 = 0;
       goto __pyx_L0;
 
-      /* "multimcts/mcts.pyx":144
+      /* "multimcts/mcts.pyx":146
  *         """
  *         while not node.is_terminal:
  *             if not node.is_fully_expanded:             # <<<<<<<<<<<<<<
  *                 return self.expand(node)
  *             else:
  */
     }
 
-    /* "multimcts/mcts.pyx":147
+    /* "multimcts/mcts.pyx":149
  *                 return self.expand(node)
  *             else:
  *                 node = self.get_best_child(node)             # <<<<<<<<<<<<<<
  * 
  *         return node
  */
     /*else*/ {
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_get_best_child); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 147, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_get_best_child); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 149, __pyx_L1_error)
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
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 147, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF_SET(__pyx_v_node, __pyx_t_1);
       __pyx_t_1 = 0;
     }
   }
 
-  /* "multimcts/mcts.pyx":149
+  /* "multimcts/mcts.pyx":151
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
 
-  /* "multimcts/mcts.pyx":138
+  /* "multimcts/mcts.pyx":140
  *         return self.get_best_child(node).state
  * 
  *     def select(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 1: Selection
  *         Traverse the tree for the node we most want to simulate.
  */
 
@@ -4108,15 +4096,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_node);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":152
+/* "multimcts/mcts.pyx":154
  * 
  *     @staticmethod
  *     def expand(node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 2: Expansion
  *         Add a new child to this node.
  */
 
@@ -4152,15 +4140,15 @@
   Py_ssize_t __pyx_t_10;
   int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("expand", 0);
 
-  /* "multimcts/mcts.pyx":156
+  /* "multimcts/mcts.pyx":158
  *         Add a new child to this node.
  *         """
  *         try:             # <<<<<<<<<<<<<<
  *             move = node.remaining_moves.pop()
  *             child = Node(node.state.make_move(move), node)
  */
   {
@@ -4168,56 +4156,56 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "multimcts/mcts.pyx":157
+      /* "multimcts/mcts.pyx":159
  *         """
  *         try:
  *             move = node.remaining_moves.pop()             # <<<<<<<<<<<<<<
  *             child = Node(node.state.make_move(move), node)
  *             node.children[move] = child
  */
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_remaining_moves); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 157, __pyx_L3_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_remaining_moves); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 159, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = __Pyx_PyObject_Pop(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 157, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyObject_Pop(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 159, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_v_move = __pyx_t_5;
       __pyx_t_5 = 0;
 
-      /* "multimcts/mcts.pyx":158
+      /* "multimcts/mcts.pyx":160
  *         try:
  *             move = node.remaining_moves.pop()
  *             child = Node(node.state.make_move(move), node)             # <<<<<<<<<<<<<<
  *             node.children[move] = child
  * 
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Node); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 158, __pyx_L3_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Node); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 160, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_state); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 158, __pyx_L3_error)
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_state); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 160, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_make_move); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 158, __pyx_L3_error)
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_make_move); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 160, __pyx_L3_error)
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
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 158, __pyx_L3_error)
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 160, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __pyx_t_8 = NULL;
       __pyx_t_9 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_8)) {
@@ -4227,152 +4215,152 @@
           __Pyx_DECREF_SET(__pyx_t_4, function);
           __pyx_t_9 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_4)) {
         PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_6, __pyx_v_node};
-        __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 158, __pyx_L3_error)
+        __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 160, __pyx_L3_error)
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
         PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_6, __pyx_v_node};
-        __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 158, __pyx_L3_error)
+        __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 160, __pyx_L3_error)
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       } else
       #endif
       {
-        __pyx_t_7 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 158, __pyx_L3_error)
+        __pyx_t_7 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 160, __pyx_L3_error)
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
-        __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 158, __pyx_L3_error)
+        __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 160, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       }
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_v_child = __pyx_t_5;
       __pyx_t_5 = 0;
 
-      /* "multimcts/mcts.pyx":159
+      /* "multimcts/mcts.pyx":161
  *             move = node.remaining_moves.pop()
  *             child = Node(node.state.make_move(move), node)
  *             node.children[move] = child             # <<<<<<<<<<<<<<
  * 
  *             if len(node.remaining_moves) == 0:
  */
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_children); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 159, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_children); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 161, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
-      if (unlikely(PyObject_SetItem(__pyx_t_5, __pyx_v_move, __pyx_v_child) < 0)) __PYX_ERR(0, 159, __pyx_L3_error)
+      if (unlikely(PyObject_SetItem(__pyx_t_5, __pyx_v_move, __pyx_v_child) < 0)) __PYX_ERR(0, 161, __pyx_L3_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-      /* "multimcts/mcts.pyx":161
+      /* "multimcts/mcts.pyx":163
  *             node.children[move] = child
  * 
  *             if len(node.remaining_moves) == 0:             # <<<<<<<<<<<<<<
  *                 node.is_fully_expanded = True
  * 
  */
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_remaining_moves); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 161, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_remaining_moves); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 163, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_10 = PyObject_Length(__pyx_t_5); if (unlikely(__pyx_t_10 == ((Py_ssize_t)-1))) __PYX_ERR(0, 161, __pyx_L3_error)
+      __pyx_t_10 = PyObject_Length(__pyx_t_5); if (unlikely(__pyx_t_10 == ((Py_ssize_t)-1))) __PYX_ERR(0, 163, __pyx_L3_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_11 = ((__pyx_t_10 == 0) != 0);
       if (__pyx_t_11) {
 
-        /* "multimcts/mcts.pyx":162
+        /* "multimcts/mcts.pyx":164
  * 
  *             if len(node.remaining_moves) == 0:
  *                 node.is_fully_expanded = True             # <<<<<<<<<<<<<<
  * 
  *             return child
  */
-        if (__Pyx_PyObject_SetAttrStr(__pyx_v_node, __pyx_n_s_is_fully_expanded, Py_True) < 0) __PYX_ERR(0, 162, __pyx_L3_error)
+        if (__Pyx_PyObject_SetAttrStr(__pyx_v_node, __pyx_n_s_is_fully_expanded, Py_True) < 0) __PYX_ERR(0, 164, __pyx_L3_error)
 
-        /* "multimcts/mcts.pyx":161
+        /* "multimcts/mcts.pyx":163
  *             node.children[move] = child
  * 
  *             if len(node.remaining_moves) == 0:             # <<<<<<<<<<<<<<
  *                 node.is_fully_expanded = True
  * 
  */
       }
 
-      /* "multimcts/mcts.pyx":164
+      /* "multimcts/mcts.pyx":166
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
 
-      /* "multimcts/mcts.pyx":156
+      /* "multimcts/mcts.pyx":158
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
 
-    /* "multimcts/mcts.pyx":165
+    /* "multimcts/mcts.pyx":167
  * 
  *             return child
  *         except IndexError:             # <<<<<<<<<<<<<<
  *             raise Exception("Tried to expand a fully-expanded or terminal node.")
  * 
  */
     __pyx_t_9 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_IndexError);
     if (__pyx_t_9) {
       __Pyx_AddTraceback("multimcts.mcts.MCTS.expand", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_4, &__pyx_t_7) < 0) __PYX_ERR(0, 165, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_4, &__pyx_t_7) < 0) __PYX_ERR(0, 167, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "multimcts/mcts.pyx":166
+      /* "multimcts/mcts.pyx":168
  *             return child
  *         except IndexError:
  *             raise Exception("Tried to expand a fully-expanded or terminal node.")             # <<<<<<<<<<<<<<
  * 
  *     def simulate(self, node:Node) -> dict:
  */
-      __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 166, __pyx_L5_except_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 168, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __PYX_ERR(0, 166, __pyx_L5_except_error)
+      __PYX_ERR(0, 168, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "multimcts/mcts.pyx":156
+    /* "multimcts/mcts.pyx":158
  *         Add a new child to this node.
  *         """
  *         try:             # <<<<<<<<<<<<<<
  *             move = node.remaining_moves.pop()
  *             child = Node(node.state.make_move(move), node)
  */
     __Pyx_XGIVEREF(__pyx_t_1);
@@ -4384,15 +4372,15 @@
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L0;
   }
 
-  /* "multimcts/mcts.pyx":152
+  /* "multimcts/mcts.pyx":154
  * 
  *     @staticmethod
  *     def expand(node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 2: Expansion
  *         Add a new child to this node.
  */
 
@@ -4409,15 +4397,15 @@
   __Pyx_XDECREF(__pyx_v_move);
   __Pyx_XDECREF(__pyx_v_child);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":168
+/* "multimcts/mcts.pyx":170
  *             raise Exception("Tried to expand a fully-expanded or terminal node.")
  * 
  *     def simulate(self, node:Node) -> dict:             # <<<<<<<<<<<<<<
  *         """Step 3: Simulation (aka playout, rollout)
  *         Play out a random game, from this node to termination, and return the final reward.
  */
 
@@ -4453,32 +4441,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("simulate", 1, 2, 2, 1); __PYX_ERR(0, 168, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("simulate", 1, 2, 2, 1); __PYX_ERR(0, 170, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "simulate") < 0)) __PYX_ERR(0, 168, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "simulate") < 0)) __PYX_ERR(0, 170, __pyx_L3_error)
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
-  __Pyx_RaiseArgtupleInvalid("simulate", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 168, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("simulate", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 170, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.MCTS.simulate", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_8simulate(__pyx_self, __pyx_v_self, __pyx_v_node);
 
@@ -4505,114 +4493,114 @@
   int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("simulate", 0);
 
-  /* "multimcts/mcts.pyx":172
+  /* "multimcts/mcts.pyx":174
  *         Play out a random game, from this node to termination, and return the final reward.
  *         """
  *         state = node.state             # <<<<<<<<<<<<<<
  * 
  *         if node.is_terminal:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_state); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_state); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 174, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_state = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":174
+  /* "multimcts/mcts.pyx":176
  *         state = node.state
  * 
  *         if node.is_terminal:             # <<<<<<<<<<<<<<
  *             terminal_team = node.parent.state.get_current_team()
  *         else:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 174, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 176, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 174, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 176, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
-    /* "multimcts/mcts.pyx":175
+    /* "multimcts/mcts.pyx":177
  * 
  *         if node.is_terminal:
  *             terminal_team = node.parent.state.get_current_team()             # <<<<<<<<<<<<<<
  *         else:
  *             while not state.is_terminal():
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_parent); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 175, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_parent); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 177, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_state); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 175, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_state); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 177, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 175, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 177, __pyx_L1_error)
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
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 175, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_terminal_team = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "multimcts/mcts.pyx":174
+    /* "multimcts/mcts.pyx":176
  *         state = node.state
  * 
  *         if node.is_terminal:             # <<<<<<<<<<<<<<
  *             terminal_team = node.parent.state.get_current_team()
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "multimcts/mcts.pyx":177
+  /* "multimcts/mcts.pyx":179
  *             terminal_team = node.parent.state.get_current_team()
  *         else:
  *             while not state.is_terminal():             # <<<<<<<<<<<<<<
  *                 try:
  *                     if self.heuristic is not None:
  */
   /*else*/ {
     while (1) {
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 177, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_is_terminal); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 179, __pyx_L1_error)
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
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 177, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 179, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_5 = ((!__pyx_t_2) != 0);
       if (!__pyx_t_5) break;
 
-      /* "multimcts/mcts.pyx":178
+      /* "multimcts/mcts.pyx":180
  *         else:
  *             while not state.is_terminal():
  *                 try:             # <<<<<<<<<<<<<<
  *                     if self.heuristic is not None:
  *                         move = self.heuristic(state)
  */
       {
@@ -4620,96 +4608,96 @@
         __Pyx_PyThreadState_assign
         __Pyx_ExceptionSave(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8);
         __Pyx_XGOTREF(__pyx_t_6);
         __Pyx_XGOTREF(__pyx_t_7);
         __Pyx_XGOTREF(__pyx_t_8);
         /*try:*/ {
 
-          /* "multimcts/mcts.pyx":179
+          /* "multimcts/mcts.pyx":181
  *             while not state.is_terminal():
  *                 try:
  *                     if self.heuristic is not None:             # <<<<<<<<<<<<<<
  *                         move = self.heuristic(state)
  *                     else:
  */
-          __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_heuristic); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L6_error)
+          __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_heuristic); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L6_error)
           __Pyx_GOTREF(__pyx_t_1);
           __pyx_t_5 = (__pyx_t_1 != Py_None);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __pyx_t_2 = (__pyx_t_5 != 0);
           if (__pyx_t_2) {
 
-            /* "multimcts/mcts.pyx":180
+            /* "multimcts/mcts.pyx":182
  *                 try:
  *                     if self.heuristic is not None:
  *                         move = self.heuristic(state)             # <<<<<<<<<<<<<<
  *                     else:
  *                         move = state.get_random_move()
  */
-            __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_heuristic); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 180, __pyx_L6_error)
+            __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_heuristic); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 182, __pyx_L6_error)
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
-            if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 180, __pyx_L6_error)
+            if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 182, __pyx_L6_error)
             __Pyx_GOTREF(__pyx_t_1);
             __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
             __Pyx_XDECREF_SET(__pyx_v_move, __pyx_t_1);
             __pyx_t_1 = 0;
 
-            /* "multimcts/mcts.pyx":179
+            /* "multimcts/mcts.pyx":181
  *             while not state.is_terminal():
  *                 try:
  *                     if self.heuristic is not None:             # <<<<<<<<<<<<<<
  *                         move = self.heuristic(state)
  *                     else:
  */
             goto __pyx_L14;
           }
 
-          /* "multimcts/mcts.pyx":182
+          /* "multimcts/mcts.pyx":184
  *                         move = self.heuristic(state)
  *                     else:
  *                         move = state.get_random_move()             # <<<<<<<<<<<<<<
  *                 except IndexError:#.forgot why this is an IndexError...
  *                     raise Exception("Non-terminal state has no legal moves.")
  */
           /*else*/ {
-            __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_random_move); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 182, __pyx_L6_error)
+            __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_random_move); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 184, __pyx_L6_error)
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
-            if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 182, __pyx_L6_error)
+            if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L6_error)
             __Pyx_GOTREF(__pyx_t_1);
             __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
             __Pyx_XDECREF_SET(__pyx_v_move, __pyx_t_1);
             __pyx_t_1 = 0;
           }
           __pyx_L14:;
 
-          /* "multimcts/mcts.pyx":178
+          /* "multimcts/mcts.pyx":180
  *         else:
  *             while not state.is_terminal():
  *                 try:             # <<<<<<<<<<<<<<
  *                     if self.heuristic is not None:
  *                         move = self.heuristic(state)
  */
         }
@@ -4718,192 +4706,192 @@
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
         goto __pyx_L13_try_end;
         __pyx_L6_error:;
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-        /* "multimcts/mcts.pyx":183
+        /* "multimcts/mcts.pyx":185
  *                     else:
  *                         move = state.get_random_move()
  *                 except IndexError:#.forgot why this is an IndexError...             # <<<<<<<<<<<<<<
  *                     raise Exception("Non-terminal state has no legal moves.")
  * 
  */
         __pyx_t_9 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_IndexError);
         if (__pyx_t_9) {
           __Pyx_AddTraceback("multimcts.mcts.MCTS.simulate", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_3, &__pyx_t_4) < 0) __PYX_ERR(0, 183, __pyx_L8_except_error)
+          if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_3, &__pyx_t_4) < 0) __PYX_ERR(0, 185, __pyx_L8_except_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_GOTREF(__pyx_t_4);
 
-          /* "multimcts/mcts.pyx":184
+          /* "multimcts/mcts.pyx":186
  *                         move = state.get_random_move()
  *                 except IndexError:#.forgot why this is an IndexError...
  *                     raise Exception("Non-terminal state has no legal moves.")             # <<<<<<<<<<<<<<
  * 
  *                 terminal_team = state.get_current_team()
  */
-          __pyx_t_10 = __Pyx_PyObject_Call(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 184, __pyx_L8_except_error)
+          __pyx_t_10 = __Pyx_PyObject_Call(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 186, __pyx_L8_except_error)
           __Pyx_GOTREF(__pyx_t_10);
           __Pyx_Raise(__pyx_t_10, 0, 0, 0);
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-          __PYX_ERR(0, 184, __pyx_L8_except_error)
+          __PYX_ERR(0, 186, __pyx_L8_except_error)
         }
         goto __pyx_L8_except_error;
         __pyx_L8_except_error:;
 
-        /* "multimcts/mcts.pyx":178
+        /* "multimcts/mcts.pyx":180
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
 
-      /* "multimcts/mcts.pyx":186
+      /* "multimcts/mcts.pyx":188
  *                     raise Exception("Non-terminal state has no legal moves.")
  * 
  *                 terminal_team = state.get_current_team()             # <<<<<<<<<<<<<<
  *                 state = state.make_move(move)
  * 
  */
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 186, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 188, __pyx_L1_error)
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
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 186, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 188, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF_SET(__pyx_v_terminal_team, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "multimcts/mcts.pyx":187
+      /* "multimcts/mcts.pyx":189
  * 
  *                 terminal_team = state.get_current_team()
  *                 state = state.make_move(move)             # <<<<<<<<<<<<<<
  * 
  *         reward = state.get_reward()
  */
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_make_move); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 187, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_make_move); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 189, __pyx_L1_error)
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
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 187, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 189, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF_SET(__pyx_v_state, __pyx_t_4);
       __pyx_t_4 = 0;
     }
   }
   __pyx_L3:;
 
-  /* "multimcts/mcts.pyx":189
+  /* "multimcts/mcts.pyx":191
  *                 state = state.make_move(move)
  * 
  *         reward = state.get_reward()             # <<<<<<<<<<<<<<
  *         if not isinstance(reward, dict):
  *             reward = {terminal_team: reward}
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_reward); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 189, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_state, __pyx_n_s_get_reward); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 191, __pyx_L1_error)
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
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 189, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_reward = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "multimcts/mcts.pyx":190
+  /* "multimcts/mcts.pyx":192
  * 
  *         reward = state.get_reward()
  *         if not isinstance(reward, dict):             # <<<<<<<<<<<<<<
  *             reward = {terminal_team: reward}
  * 
  */
   __pyx_t_2 = PyDict_Check(__pyx_v_reward); 
   __pyx_t_5 = ((!(__pyx_t_2 != 0)) != 0);
   if (__pyx_t_5) {
 
-    /* "multimcts/mcts.pyx":191
+    /* "multimcts/mcts.pyx":193
  *         reward = state.get_reward()
  *         if not isinstance(reward, dict):
  *             reward = {terminal_team: reward}             # <<<<<<<<<<<<<<
  * 
  *         return reward
  */
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 191, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (unlikely(!__pyx_v_terminal_team)) { __Pyx_RaiseUnboundLocalError("terminal_team"); __PYX_ERR(0, 191, __pyx_L1_error) }
-    if (PyDict_SetItem(__pyx_t_4, __pyx_v_terminal_team, __pyx_v_reward) < 0) __PYX_ERR(0, 191, __pyx_L1_error)
+    if (unlikely(!__pyx_v_terminal_team)) { __Pyx_RaiseUnboundLocalError("terminal_team"); __PYX_ERR(0, 193, __pyx_L1_error) }
+    if (PyDict_SetItem(__pyx_t_4, __pyx_v_terminal_team, __pyx_v_reward) < 0) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_DECREF_SET(__pyx_v_reward, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "multimcts/mcts.pyx":190
+    /* "multimcts/mcts.pyx":192
  * 
  *         reward = state.get_reward()
  *         if not isinstance(reward, dict):             # <<<<<<<<<<<<<<
  *             reward = {terminal_team: reward}
  * 
  */
   }
 
-  /* "multimcts/mcts.pyx":193
+  /* "multimcts/mcts.pyx":195
  *             reward = {terminal_team: reward}
  * 
  *         return reward             # <<<<<<<<<<<<<<
  * 
  *     @staticmethod
  */
   __Pyx_XDECREF(__pyx_r);
-  if (!(likely(PyDict_CheckExact(__pyx_v_reward))||((__pyx_v_reward) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_v_reward)->tp_name), 0))) __PYX_ERR(0, 193, __pyx_L1_error)
+  if (!(likely(PyDict_CheckExact(__pyx_v_reward))||((__pyx_v_reward) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "dict", Py_TYPE(__pyx_v_reward)->tp_name), 0))) __PYX_ERR(0, 195, __pyx_L1_error)
   __Pyx_INCREF(__pyx_v_reward);
   __pyx_r = ((PyObject*)__pyx_v_reward);
   goto __pyx_L0;
 
-  /* "multimcts/mcts.pyx":168
+  /* "multimcts/mcts.pyx":170
  *             raise Exception("Tried to expand a fully-expanded or terminal node.")
  * 
  *     def simulate(self, node:Node) -> dict:             # <<<<<<<<<<<<<<
  *         """Step 3: Simulation (aka playout, rollout)
  *         Play out a random game, from this node to termination, and return the final reward.
  */
 
@@ -4921,15 +4909,15 @@
   __Pyx_XDECREF(__pyx_v_move);
   __Pyx_XDECREF(__pyx_v_reward);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":196
+/* "multimcts/mcts.pyx":198
  * 
  *     @staticmethod
  *     def backpropagate(node:Node, reward:dict):             # <<<<<<<<<<<<<<
  *         """Step 4: Backpropagation
  *         Update all ancestors with the reward from this terminal node.
  */
 
@@ -4965,38 +4953,38 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_reward)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("backpropagate", 1, 2, 2, 1); __PYX_ERR(0, 196, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("backpropagate", 1, 2, 2, 1); __PYX_ERR(0, 198, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "backpropagate") < 0)) __PYX_ERR(0, 196, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "backpropagate") < 0)) __PYX_ERR(0, 198, __pyx_L3_error)
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
-  __Pyx_RaiseArgtupleInvalid("backpropagate", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 196, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("backpropagate", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 198, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("multimcts.mcts.MCTS.backpropagate", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_reward), (&PyDict_Type), 1, "reward", 1))) __PYX_ERR(0, 196, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_reward), (&PyDict_Type), 1, "reward", 1))) __PYX_ERR(0, 198, __pyx_L1_error)
   __pyx_r = __pyx_pf_9multimcts_4mcts_4MCTS_10backpropagate(__pyx_self, __pyx_v_node, __pyx_v_reward);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -5027,126 +5015,126 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("backpropagate", 0);
   __Pyx_INCREF(__pyx_v_node);
   __Pyx_INCREF(__pyx_v_reward);
 
-  /* "multimcts/mcts.pyx":201
+  /* "multimcts/mcts.pyx":203
  *         """
  *         # Remove 0-values for efficiency
  *         reward = {k:v for k,v in reward.items() if v!=0}             # <<<<<<<<<<<<<<
  * 
  *         while node is not None:
  */
   { /* enter inner scope */
-    __pyx_t_1 = PyDict_New(); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L5_error)
+    __pyx_t_1 = PyDict_New(); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 203, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (unlikely(__pyx_v_reward == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-      __PYX_ERR(0, 201, __pyx_L5_error)
+      __PYX_ERR(0, 203, __pyx_L5_error)
     }
-    __pyx_t_2 = __Pyx_PyDict_Items(__pyx_v_reward); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L5_error)
+    __pyx_t_2 = __Pyx_PyDict_Items(__pyx_v_reward); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 203, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_2);
     if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
       __pyx_t_3 = __pyx_t_2; __Pyx_INCREF(__pyx_t_3); __pyx_t_4 = 0;
       __pyx_t_5 = NULL;
     } else {
-      __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 201, __pyx_L5_error)
+      __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 203, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_5 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 201, __pyx_L5_error)
+      __pyx_t_5 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 203, __pyx_L5_error)
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     for (;;) {
       if (likely(!__pyx_t_5)) {
         if (likely(PyList_CheckExact(__pyx_t_3))) {
           if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 201, __pyx_L5_error)
+          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 203, __pyx_L5_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L5_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 203, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         } else {
           if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 201, __pyx_L5_error)
+          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 203, __pyx_L5_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L5_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 203, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         }
       } else {
         __pyx_t_2 = __pyx_t_5(__pyx_t_3);
         if (unlikely(!__pyx_t_2)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 201, __pyx_L5_error)
+            else __PYX_ERR(0, 203, __pyx_L5_error)
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
-          __PYX_ERR(0, 201, __pyx_L5_error)
+          __PYX_ERR(0, 203, __pyx_L5_error)
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
-        __pyx_t_6 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L5_error)
+        __pyx_t_6 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 203, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_7 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L5_error)
+        __pyx_t_7 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 203, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_7);
         #endif
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       } else {
         Py_ssize_t index = -1;
-        __pyx_t_8 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 201, __pyx_L5_error)
+        __pyx_t_8 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 203, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_t_9 = Py_TYPE(__pyx_t_8)->tp_iternext;
         index = 0; __pyx_t_6 = __pyx_t_9(__pyx_t_8); if (unlikely(!__pyx_t_6)) goto __pyx_L8_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_6);
         index = 1; __pyx_t_7 = __pyx_t_9(__pyx_t_8); if (unlikely(!__pyx_t_7)) goto __pyx_L8_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_7);
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_8), 2) < 0) __PYX_ERR(0, 201, __pyx_L5_error)
+        if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_8), 2) < 0) __PYX_ERR(0, 203, __pyx_L5_error)
         __pyx_t_9 = NULL;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         goto __pyx_L9_unpacking_done;
         __pyx_L8_unpacking_failed:;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __pyx_t_9 = NULL;
         if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 201, __pyx_L5_error)
+        __PYX_ERR(0, 203, __pyx_L5_error)
         __pyx_L9_unpacking_done:;
       }
       __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_k, __pyx_t_6);
       __pyx_t_6 = 0;
       __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_v, __pyx_t_7);
       __pyx_t_7 = 0;
-      __pyx_t_2 = __Pyx_PyInt_NeObjC(__pyx_7genexpr__pyx_v_v, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L5_error)
+      __pyx_t_2 = __Pyx_PyInt_NeObjC(__pyx_7genexpr__pyx_v_v, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 203, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 201, __pyx_L5_error)
+      __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 203, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (__pyx_t_10) {
-        if (unlikely(PyDict_SetItem(__pyx_t_1, (PyObject*)__pyx_7genexpr__pyx_v_k, (PyObject*)__pyx_7genexpr__pyx_v_v))) __PYX_ERR(0, 201, __pyx_L5_error)
+        if (unlikely(PyDict_SetItem(__pyx_t_1, (PyObject*)__pyx_7genexpr__pyx_v_k, (PyObject*)__pyx_7genexpr__pyx_v_v))) __PYX_ERR(0, 203, __pyx_L5_error)
       }
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_k); __pyx_7genexpr__pyx_v_k = 0;
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_v); __pyx_7genexpr__pyx_v_v = 0;
     goto __pyx_L11_exit_scope;
     __pyx_L5_error:;
@@ -5154,102 +5142,102 @@
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_v); __pyx_7genexpr__pyx_v_v = 0;
     goto __pyx_L1_error;
     __pyx_L11_exit_scope:;
   } /* exit inner scope */
   __Pyx_DECREF_SET(__pyx_v_reward, ((PyObject*)__pyx_t_1));
   __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":203
+  /* "multimcts/mcts.pyx":205
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
 
-    /* "multimcts/mcts.pyx":204
+    /* "multimcts/mcts.pyx":206
  * 
  *         while node is not None:
  *             node.num_visits += 1             # <<<<<<<<<<<<<<
  * 
  *             for key in reward:
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_num_visits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 204, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_num_visits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 206, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_t_1, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 204, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_t_1, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 206, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_node, __pyx_n_s_num_visits, __pyx_t_3) < 0) __PYX_ERR(0, 204, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_v_node, __pyx_n_s_num_visits, __pyx_t_3) < 0) __PYX_ERR(0, 206, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "multimcts/mcts.pyx":206
+    /* "multimcts/mcts.pyx":208
  *             node.num_visits += 1
  * 
  *             for key in reward:             # <<<<<<<<<<<<<<
  *                 node.total_reward[key] += reward[key]
  * 
  */
     __pyx_t_4 = 0;
-    __pyx_t_1 = __Pyx_dict_iterator(__pyx_v_reward, 1, ((PyObject *)NULL), (&__pyx_t_12), (&__pyx_t_13)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 206, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_dict_iterator(__pyx_v_reward, 1, ((PyObject *)NULL), (&__pyx_t_12), (&__pyx_t_13)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 208, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF(__pyx_t_3);
     __pyx_t_3 = __pyx_t_1;
     __pyx_t_1 = 0;
     while (1) {
       __pyx_t_14 = __Pyx_dict_iter_next(__pyx_t_3, __pyx_t_12, &__pyx_t_4, &__pyx_t_1, NULL, NULL, __pyx_t_13);
       if (unlikely(__pyx_t_14 == 0)) break;
-      if (unlikely(__pyx_t_14 == -1)) __PYX_ERR(0, 206, __pyx_L1_error)
+      if (unlikely(__pyx_t_14 == -1)) __PYX_ERR(0, 208, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "multimcts/mcts.pyx":207
+      /* "multimcts/mcts.pyx":209
  * 
  *             for key in reward:
  *                 node.total_reward[key] += reward[key]             # <<<<<<<<<<<<<<
  * 
  *             node = node.parent
  */
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_total_reward); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_total_reward); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 209, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_v_key);
       __pyx_t_2 = __pyx_v_key;
-      __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 207, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 209, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_6 = __Pyx_PyDict_GetItem(__pyx_v_reward, __pyx_v_key); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 207, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyDict_GetItem(__pyx_v_reward, __pyx_v_key); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 209, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_8 = PyNumber_InPlaceAdd(__pyx_t_7, __pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 207, __pyx_L1_error)
+      __pyx_t_8 = PyNumber_InPlaceAdd(__pyx_t_7, __pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 209, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_t_2, __pyx_t_8) < 0)) __PYX_ERR(0, 207, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_t_2, __pyx_t_8) < 0)) __PYX_ERR(0, 209, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "multimcts/mcts.pyx":209
+    /* "multimcts/mcts.pyx":211
  *                 node.total_reward[key] += reward[key]
  * 
  *             node = node.parent             # <<<<<<<<<<<<<<
  * 
  *     def get_best_child(self, node:Node) -> Node:
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_parent); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 209, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_parent); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 211, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF_SET(__pyx_v_node, __pyx_t_3);
     __pyx_t_3 = 0;
   }
 
-  /* "multimcts/mcts.pyx":196
+  /* "multimcts/mcts.pyx":198
  * 
  *     @staticmethod
  *     def backpropagate(node:Node, reward:dict):             # <<<<<<<<<<<<<<
  *         """Step 4: Backpropagation
  *         Update all ancestors with the reward from this terminal node.
  */
 
@@ -5272,20 +5260,20 @@
   __Pyx_XDECREF(__pyx_v_node);
   __Pyx_XDECREF(__pyx_v_reward);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":211
+/* "multimcts/mcts.pyx":213
  *             node = node.parent
  * 
  *     def get_best_child(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         cur_team = node.state.get_current_team()
- *         cdef float ln_parent_visits = log(node.num_visits)
+ * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_13get_best_child(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_9multimcts_4mcts_4MCTS_13get_best_child = {"get_best_child", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9multimcts_4mcts_4MCTS_13get_best_child, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_9multimcts_4mcts_4MCTS_13get_best_child(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
@@ -5315,46 +5303,46 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("get_best_child", 1, 2, 2, 1); __PYX_ERR(0, 211, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_best_child", 1, 2, 2, 1); __PYX_ERR(0, 213, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_best_child") < 0)) __PYX_ERR(0, 211, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_best_child") < 0)) __PYX_ERR(0, 213, __pyx_L3_error)
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
-  __Pyx_RaiseArgtupleInvalid("get_best_child", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 211, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_best_child", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 213, __pyx_L3_error)
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
 
-/* "multimcts/mcts.pyx":224
+/* "multimcts/mcts.pyx":227
  *         for child in node.children.values():
  *             # Relative reward is this child's reward minus its siblings' rewards.
  *             reward = (2 * child.total_reward[cur_team]) - sum(x for x in child.total_reward.values())             # <<<<<<<<<<<<<<
  *             visits = child.num_visits
  * 
  */
 
@@ -5366,23 +5354,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct_1_genexpr *)__pyx_tp_new_9multimcts_4mcts___pyx_scope_struct_1_genexpr(__pyx_ptype_9multimcts_4mcts___pyx_scope_struct_1_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct_1_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 224, __pyx_L1_error)
+    __PYX_ERR(0, 227, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child *) __pyx_self;
   __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_outer_scope));
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_outer_scope);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_9multimcts_4mcts_4MCTS_14get_best_child_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_MCTS_get_best_child_locals_genex, __pyx_n_s_multimcts_mcts); if (unlikely(!gen)) __PYX_ERR(0, 224, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_9multimcts_4mcts_4MCTS_14get_best_child_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_MCTS_get_best_child_locals_genex, __pyx_n_s_multimcts_mcts); if (unlikely(!gen)) __PYX_ERR(0, 227, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -5412,71 +5400,71 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L6_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 224, __pyx_L1_error)
-  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_child)) { __Pyx_RaiseClosureNameError("child"); __PYX_ERR(0, 224, __pyx_L1_error) }
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_child, __pyx_n_s_total_reward); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 224, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 227, __pyx_L1_error)
+  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_child)) { __Pyx_RaiseClosureNameError("child"); __PYX_ERR(0, 227, __pyx_L1_error) }
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_child, __pyx_n_s_total_reward); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 227, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_values); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 224, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_values); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 227, __pyx_L1_error)
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
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
     __pyx_t_3 = __pyx_t_1; __Pyx_INCREF(__pyx_t_3); __pyx_t_4 = 0;
     __pyx_t_5 = NULL;
   } else {
-    __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 224, __pyx_L1_error)
+    __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 227, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 224, __pyx_L1_error)
+    __pyx_t_5 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 227, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     if (likely(!__pyx_t_5)) {
       if (likely(PyList_CheckExact(__pyx_t_3))) {
         if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_3)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_1); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 224, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_1); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 227, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
         if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_1); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 224, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_1); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 227, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
       __pyx_t_1 = __pyx_t_5(__pyx_t_3);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 224, __pyx_L1_error)
+          else __PYX_ERR(0, 227, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_x);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_x, __pyx_t_1);
@@ -5496,15 +5484,15 @@
     return __pyx_r;
     __pyx_L6_resume_from_yield:;
     __pyx_t_3 = __pyx_cur_scope->__pyx_t_0;
     __pyx_cur_scope->__pyx_t_0 = 0;
     __Pyx_XGOTREF(__pyx_t_3);
     __pyx_t_4 = __pyx_cur_scope->__pyx_t_1;
     __pyx_t_5 = __pyx_cur_scope->__pyx_t_2;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 224, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 227, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
   /* function exit code */
   PyErr_SetNone(PyExc_StopIteration);
   goto __pyx_L0;
@@ -5520,328 +5508,328 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "multimcts/mcts.pyx":211
+/* "multimcts/mcts.pyx":213
  *             node = node.parent
  * 
  *     def get_best_child(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         cur_team = node.state.get_current_team()
- *         cdef float ln_parent_visits = log(node.num_visits)
+ * 
  */
 
 static PyObject *__pyx_pf_9multimcts_4mcts_4MCTS_12get_best_child(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_node) {
   struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child *__pyx_cur_scope;
   PyObject *__pyx_v_cur_team = NULL;
-  float __pyx_v_ln_parent_visits;
+  int __pyx_v_visits;
   float __pyx_v_reward;
   float __pyx_v_score;
-  int __pyx_v_visits;
   float __pyx_v_exploration_bias;
+  float __pyx_v_ln_parent_visits;
   float __pyx_v_max_score;
   PyObject *__pyx_v_best = NULL;
   PyObject *__pyx_gb_9multimcts_4mcts_4MCTS_14get_best_child_2generator = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
-  double __pyx_t_4;
-  float __pyx_t_5;
+  float __pyx_t_4;
+  double __pyx_t_5;
   Py_ssize_t __pyx_t_6;
   PyObject *(*__pyx_t_7)(PyObject *);
   PyObject *__pyx_t_8 = NULL;
   int __pyx_t_9;
   int __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_best_child", 0);
   __pyx_cur_scope = (struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child *)__pyx_tp_new_9multimcts_4mcts___pyx_scope_struct__get_best_child(__pyx_ptype_9multimcts_4mcts___pyx_scope_struct__get_best_child, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_9multimcts_4mcts___pyx_scope_struct__get_best_child *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 211, __pyx_L1_error)
+    __PYX_ERR(0, 213, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
 
-  /* "multimcts/mcts.pyx":212
+  /* "multimcts/mcts.pyx":214
  * 
  *     def get_best_child(self, node:Node) -> Node:
  *         cur_team = node.state.get_current_team()             # <<<<<<<<<<<<<<
- *         cdef float ln_parent_visits = log(node.num_visits)
  * 
+ *         # Initialize UCB variables.
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_state); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 212, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_state); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 214, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 212, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get_current_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 214, __pyx_L1_error)
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
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 212, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 214, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_cur_team = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":213
- *     def get_best_child(self, node:Node) -> Node:
- *         cur_team = node.state.get_current_team()
- *         cdef float ln_parent_visits = log(node.num_visits)             # <<<<<<<<<<<<<<
- * 
+  /* "multimcts/mcts.pyx":219
+ *         cdef int visits
  *         cdef float reward, score
+ *         cdef float exploration_bias = self.exploration_bias             # <<<<<<<<<<<<<<
+ *         cdef float ln_parent_visits = log(node.num_visits)
+ * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_num_visits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 213, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_exploration_bias); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 213, __pyx_L1_error)
+  __pyx_t_4 = __pyx_PyFloat_AsFloat(__pyx_t_1); if (unlikely((__pyx_t_4 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 219, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v_ln_parent_visits = log(__pyx_t_4);
+  __pyx_v_exploration_bias = __pyx_t_4;
 
-  /* "multimcts/mcts.pyx":217
+  /* "multimcts/mcts.pyx":220
  *         cdef float reward, score
- *         cdef int visits
- *         cdef float exploration_bias = self.exploration_bias             # <<<<<<<<<<<<<<
+ *         cdef float exploration_bias = self.exploration_bias
+ *         cdef float ln_parent_visits = log(node.num_visits)             # <<<<<<<<<<<<<<
  * 
  *         cdef float max_score = float('-inf')
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_exploration_bias); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 217, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_num_visits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __pyx_PyFloat_AsFloat(__pyx_t_1); if (unlikely((__pyx_t_5 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 217, __pyx_L1_error)
+  __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 220, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v_exploration_bias = __pyx_t_5;
+  __pyx_v_ln_parent_visits = log(__pyx_t_5);
 
-  /* "multimcts/mcts.pyx":219
- *         cdef float exploration_bias = self.exploration_bias
+  /* "multimcts/mcts.pyx":222
+ *         cdef float ln_parent_visits = log(node.num_visits)
  * 
  *         cdef float max_score = float('-inf')             # <<<<<<<<<<<<<<
- *         best = None
+ *         best:Node = None
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_AsDouble(__pyx_kp_s_inf); if (unlikely(__pyx_t_4 == ((double)((double)-1)) && PyErr_Occurred())) __PYX_ERR(0, 219, __pyx_L1_error)
-  __pyx_v_max_score = __pyx_t_4;
+  __pyx_t_5 = __Pyx_PyObject_AsDouble(__pyx_kp_s_inf); if (unlikely(__pyx_t_5 == ((double)((double)-1)) && PyErr_Occurred())) __PYX_ERR(0, 222, __pyx_L1_error)
+  __pyx_v_max_score = __pyx_t_5;
 
-  /* "multimcts/mcts.pyx":220
+  /* "multimcts/mcts.pyx":223
  * 
  *         cdef float max_score = float('-inf')
- *         best = None             # <<<<<<<<<<<<<<
+ *         best:Node = None             # <<<<<<<<<<<<<<
  * 
  *         for child in node.children.values():
  */
   __Pyx_INCREF(Py_None);
   __pyx_v_best = Py_None;
 
-  /* "multimcts/mcts.pyx":222
- *         best = None
+  /* "multimcts/mcts.pyx":225
+ *         best:Node = None
  * 
  *         for child in node.children.values():             # <<<<<<<<<<<<<<
  *             # Relative reward is this child's reward minus its siblings' rewards.
  *             reward = (2 * child.total_reward[cur_team]) - sum(x for x in child.total_reward.values())
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_children); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 222, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_node, __pyx_n_s_children); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 225, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_values); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 222, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_values); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 225, __pyx_L1_error)
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
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 225, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
     __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2); __pyx_t_6 = 0;
     __pyx_t_7 = NULL;
   } else {
-    __pyx_t_6 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __pyx_t_6 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 225, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_7 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __pyx_t_7 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 225, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     if (likely(!__pyx_t_7)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_1); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 222, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_1); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 225, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 225, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
         if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_1); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 222, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_1); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 225, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 225, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
       __pyx_t_1 = __pyx_t_7(__pyx_t_2);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 222, __pyx_L1_error)
+          else __PYX_ERR(0, 225, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_child);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_child, __pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "multimcts/mcts.pyx":224
+    /* "multimcts/mcts.pyx":227
  *         for child in node.children.values():
  *             # Relative reward is this child's reward minus its siblings' rewards.
  *             reward = (2 * child.total_reward[cur_team]) - sum(x for x in child.total_reward.values())             # <<<<<<<<<<<<<<
  *             visits = child.num_visits
  * 
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_child, __pyx_n_s_total_reward); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_child, __pyx_n_s_total_reward); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_cur_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 224, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_cur_team); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 227, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_Multiply(__pyx_int_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Multiply(__pyx_int_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __pyx_pf_9multimcts_4mcts_4MCTS_14get_best_child_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 224, __pyx_L1_error)
+    __pyx_t_3 = __pyx_pf_9multimcts_4mcts_4MCTS_14get_best_child_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 227, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_8 = __Pyx_PyObject_CallOneArg(__pyx_builtin_sum, __pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 224, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_CallOneArg(__pyx_builtin_sum, __pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 227, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyNumber_Subtract(__pyx_t_1, __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 224, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Subtract(__pyx_t_1, __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 227, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_5 = __pyx_PyFloat_AsFloat(__pyx_t_3); if (unlikely((__pyx_t_5 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 224, __pyx_L1_error)
+    __pyx_t_4 = __pyx_PyFloat_AsFloat(__pyx_t_3); if (unlikely((__pyx_t_4 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 227, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_v_reward = __pyx_t_5;
+    __pyx_v_reward = __pyx_t_4;
 
-    /* "multimcts/mcts.pyx":225
+    /* "multimcts/mcts.pyx":228
  *             # Relative reward is this child's reward minus its siblings' rewards.
  *             reward = (2 * child.total_reward[cur_team]) - sum(x for x in child.total_reward.values())
  *             visits = child.num_visits             # <<<<<<<<<<<<<<
  * 
  *             """UCB := (x / n) + C * sqrt(ln(N) / n)
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_child, __pyx_n_s_num_visits); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 225, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_child, __pyx_n_s_num_visits); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 228, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_9 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_9 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 225, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_9 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 228, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_visits = __pyx_t_9;
 
-    /* "multimcts/mcts.pyx":233
+    /* "multimcts/mcts.pyx":236
  *             C=exploration bias
  *             """
  *             score = (reward / visits) + exploration_bias * sqrt(ln_parent_visits / visits)             # <<<<<<<<<<<<<<
  * 
  *             if score > max_score:
  */
     if (unlikely(__pyx_v_visits == 0)) {
       PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 233, __pyx_L1_error)
+      __PYX_ERR(0, 236, __pyx_L1_error)
     }
     if (unlikely(__pyx_v_visits == 0)) {
       PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 233, __pyx_L1_error)
+      __PYX_ERR(0, 236, __pyx_L1_error)
     }
     __pyx_v_score = ((__pyx_v_reward / __pyx_v_visits) + (__pyx_v_exploration_bias * sqrt((__pyx_v_ln_parent_visits / __pyx_v_visits))));
 
-    /* "multimcts/mcts.pyx":235
+    /* "multimcts/mcts.pyx":238
  *             score = (reward / visits) + exploration_bias * sqrt(ln_parent_visits / visits)
  * 
  *             if score > max_score:             # <<<<<<<<<<<<<<
  *                 max_score = score
  *                 best = child
  */
     __pyx_t_10 = ((__pyx_v_score > __pyx_v_max_score) != 0);
     if (__pyx_t_10) {
 
-      /* "multimcts/mcts.pyx":236
+      /* "multimcts/mcts.pyx":239
  * 
  *             if score > max_score:
  *                 max_score = score             # <<<<<<<<<<<<<<
  *                 best = child
  * 
  */
       __pyx_v_max_score = __pyx_v_score;
 
-      /* "multimcts/mcts.pyx":237
+      /* "multimcts/mcts.pyx":240
  *             if score > max_score:
  *                 max_score = score
  *                 best = child             # <<<<<<<<<<<<<<
  * 
  *         return best
  */
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_child);
       __Pyx_DECREF_SET(__pyx_v_best, __pyx_cur_scope->__pyx_v_child);
 
-      /* "multimcts/mcts.pyx":235
+      /* "multimcts/mcts.pyx":238
  *             score = (reward / visits) + exploration_bias * sqrt(ln_parent_visits / visits)
  * 
  *             if score > max_score:             # <<<<<<<<<<<<<<
  *                 max_score = score
  *                 best = child
  */
     }
 
-    /* "multimcts/mcts.pyx":222
- *         best = None
+    /* "multimcts/mcts.pyx":225
+ *         best:Node = None
  * 
  *         for child in node.children.values():             # <<<<<<<<<<<<<<
  *             # Relative reward is this child's reward minus its siblings' rewards.
  *             reward = (2 * child.total_reward[cur_team]) - sum(x for x in child.total_reward.values())
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "multimcts/mcts.pyx":239
+  /* "multimcts/mcts.pyx":242
  *                 best = child
  * 
  *         return best             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_best);
   __pyx_r = __pyx_v_best;
   goto __pyx_L0;
 
-  /* "multimcts/mcts.pyx":211
+  /* "multimcts/mcts.pyx":213
  *             node = node.parent
  * 
  *     def get_best_child(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         cur_team = node.state.get_current_team()
- *         cdef float ln_parent_visits = log(node.num_visits)
+ * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
@@ -6135,15 +6123,14 @@
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  {&__pyx_n_s_Dict, __pyx_k_Dict, sizeof(__pyx_k_Dict), 0, 0, 1, 1},
   {&__pyx_n_s_GameState, __pyx_k_GameState, sizeof(__pyx_k_GameState), 0, 0, 1, 1},
   {&__pyx_n_s_GameState___eq, __pyx_k_GameState___eq, sizeof(__pyx_k_GameState___eq), 0, 0, 1, 1},
   {&__pyx_n_s_GameState___hash, __pyx_k_GameState___hash, sizeof(__pyx_k_GameState___hash), 0, 0, 1, 1},
   {&__pyx_n_s_GameState_get_current_team, __pyx_k_GameState_get_current_team, sizeof(__pyx_k_GameState_get_current_team), 0, 0, 1, 1},
   {&__pyx_n_s_GameState_get_legal_moves, __pyx_k_GameState_get_legal_moves, sizeof(__pyx_k_GameState_get_legal_moves), 0, 0, 1, 1},
   {&__pyx_n_s_GameState_get_random_move, __pyx_k_GameState_get_random_move, sizeof(__pyx_k_GameState_get_random_move), 0, 0, 1, 1},
   {&__pyx_n_s_GameState_get_reward, __pyx_k_GameState_get_reward, sizeof(__pyx_k_GameState_get_reward), 0, 0, 1, 1},
@@ -6255,20 +6242,20 @@
   {&__pyx_n_s_typing, __pyx_k_typing, sizeof(__pyx_k_typing), 0, 0, 1, 1},
   {&__pyx_n_s_v, __pyx_k_v, sizeof(__pyx_k_v), 0, 0, 1, 1},
   {&__pyx_n_s_values, __pyx_k_values, sizeof(__pyx_k_values), 0, 0, 1, 1},
   {&__pyx_n_s_visits, __pyx_k_visits, sizeof(__pyx_k_visits), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_staticmethod = __Pyx_GetBuiltinName(__pyx_n_s_staticmethod); if (!__pyx_builtin_staticmethod) __PYX_ERR(0, 151, __pyx_L1_error)
+  __pyx_builtin_staticmethod = __Pyx_GetBuiltinName(__pyx_n_s_staticmethod); if (!__pyx_builtin_staticmethod) __PYX_ERR(0, 153, __pyx_L1_error)
   __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 11, __pyx_L1_error)
   __pyx_builtin_StopIteration = __Pyx_GetBuiltinName(__pyx_n_s_StopIteration); if (!__pyx_builtin_StopIteration) __PYX_ERR(0, 28, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 101, __pyx_L1_error)
-  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 165, __pyx_L1_error)
-  __pyx_builtin_sum = __Pyx_GetBuiltinName(__pyx_n_s_sum); if (!__pyx_builtin_sum) __PYX_ERR(0, 224, __pyx_L1_error)
+  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 167, __pyx_L1_error)
+  __pyx_builtin_sum = __Pyx_GetBuiltinName(__pyx_n_s_sum); if (!__pyx_builtin_sum) __PYX_ERR(0, 227, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -6308,15 +6295,15 @@
   __Pyx_GIVEREF(__pyx_tuple__3);
 
   /* "multimcts/mcts.pyx":40
  *     def is_terminal(self) -> bool:
  *         """Checks if the game is over."""
  *         raise NotImplementedError("GameState must implement is_terminal.")             # <<<<<<<<<<<<<<
  * 
- *     def get_reward(self) -> Union[float, Dict[Union[int,str], float]]:
+ *     def get_reward(self) -> Union[float, dict[Union[int,str], float]]:
  */
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_GameState_must_implement_is_term); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
   /* "multimcts/mcts.pyx":48
  *         Note: This method is only evaluated on terminal states.
@@ -6349,42 +6336,42 @@
  */
   __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_GameStates_must_implement___eq); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
   /* "multimcts/mcts.pyx":101
  *         """
- *         if max_iterations is None and max_time is None:
+ *         if max_time is None and max_iterations is None:
  *             raise ValueError("One or more of max_time/max_iterations is required.")             # <<<<<<<<<<<<<<
  * 
  *         self.exploration_bias = exploration_bias
  */
   __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_One_or_more_of_max_time_max_iter); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "multimcts/mcts.pyx":166
+  /* "multimcts/mcts.pyx":168
  *             return child
  *         except IndexError:
  *             raise Exception("Tried to expand a fully-expanded or terminal node.")             # <<<<<<<<<<<<<<
  * 
  *     def simulate(self, node:Node) -> dict:
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_Tried_to_expand_a_fully_expanded); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_Tried_to_expand_a_fully_expanded); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 168, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "multimcts/mcts.pyx":184
+  /* "multimcts/mcts.pyx":186
  *                         move = state.get_random_move()
  *                 except IndexError:#.forgot why this is an IndexError...
  *                     raise Exception("Non-terminal state has no legal moves.")             # <<<<<<<<<<<<<<
  * 
  *                 terminal_team = state.get_current_team()
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_Non_terminal_state_has_no_legal); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_Non_terminal_state_has_no_legal); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 186, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
   /* "multimcts/mcts.pyx":9
  * 
  * class GameState():
  *     def get_current_team(self) -> Union[int,str]:             # <<<<<<<<<<<<<<
@@ -6458,15 +6445,15 @@
   __Pyx_GOTREF(__pyx_tuple__22);
   __Pyx_GIVEREF(__pyx_tuple__22);
   __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_is_terminal, 38, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 38, __pyx_L1_error)
 
   /* "multimcts/mcts.pyx":42
  *         raise NotImplementedError("GameState must implement is_terminal.")
  * 
- *     def get_reward(self) -> Union[float, Dict[Union[int,str], float]]:             # <<<<<<<<<<<<<<
+ *     def get_reward(self) -> Union[float, dict[Union[int,str], float]]:             # <<<<<<<<<<<<<<
  *         """Returns the reward earned by the team that played the game-ending move.
  *         Typically 1 for win, -1 for loss, 0 for draw.
  */
   __pyx_tuple__24 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__24);
   __Pyx_GIVEREF(__pyx_tuple__24);
   __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_reward, 42, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 42, __pyx_L1_error)
@@ -6530,73 +6517,73 @@
  * 
  */
   __pyx_tuple__35 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_node, __pyx_n_s_end_time, __pyx_n_s_i, __pyx_n_s_child, __pyx_n_s_reward); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__35);
   __Pyx_GIVEREF(__pyx_tuple__35);
   __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(2, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_search, 109, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 109, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":138
+  /* "multimcts/mcts.pyx":140
  *         return self.get_best_child(node).state
  * 
  *     def select(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 1: Selection
  *         Traverse the tree for the node we most want to simulate.
  */
-  __pyx_tuple__37 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_node); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(0, 138, __pyx_L1_error)
+  __pyx_tuple__37 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_node); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(0, 140, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__37);
   __Pyx_GIVEREF(__pyx_tuple__37);
-  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_select, 138, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(0, 138, __pyx_L1_error)
+  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_select, 140, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(0, 140, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":152
+  /* "multimcts/mcts.pyx":154
  * 
  *     @staticmethod
  *     def expand(node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 2: Expansion
  *         Add a new child to this node.
  */
-  __pyx_tuple__39 = PyTuple_Pack(3, __pyx_n_s_node, __pyx_n_s_move, __pyx_n_s_child); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_tuple__39 = PyTuple_Pack(3, __pyx_n_s_node, __pyx_n_s_move, __pyx_n_s_child); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(0, 154, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__39);
   __Pyx_GIVEREF(__pyx_tuple__39);
-  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_expand, 152, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_expand, 154, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(0, 154, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":168
+  /* "multimcts/mcts.pyx":170
  *             raise Exception("Tried to expand a fully-expanded or terminal node.")
  * 
  *     def simulate(self, node:Node) -> dict:             # <<<<<<<<<<<<<<
  *         """Step 3: Simulation (aka playout, rollout)
  *         Play out a random game, from this node to termination, and return the final reward.
  */
-  __pyx_tuple__41 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_node, __pyx_n_s_state, __pyx_n_s_terminal_team, __pyx_n_s_move, __pyx_n_s_reward); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __pyx_tuple__41 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_node, __pyx_n_s_state, __pyx_n_s_terminal_team, __pyx_n_s_move, __pyx_n_s_reward); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(0, 170, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__41);
   __Pyx_GIVEREF(__pyx_tuple__41);
-  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(2, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_simulate, 168, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(2, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_simulate, 170, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 170, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":196
+  /* "multimcts/mcts.pyx":198
  * 
  *     @staticmethod
  *     def backpropagate(node:Node, reward:dict):             # <<<<<<<<<<<<<<
  *         """Step 4: Backpropagation
  *         Update all ancestors with the reward from this terminal node.
  */
-  __pyx_tuple__43 = PyTuple_Pack(5, __pyx_n_s_node, __pyx_n_s_reward, __pyx_n_s_key, __pyx_n_s_k, __pyx_n_s_v); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_tuple__43 = PyTuple_Pack(5, __pyx_n_s_node, __pyx_n_s_reward, __pyx_n_s_key, __pyx_n_s_k, __pyx_n_s_v); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 198, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__43);
   __Pyx_GIVEREF(__pyx_tuple__43);
-  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(2, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_backpropagate, 196, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(2, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_backpropagate, 198, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 198, __pyx_L1_error)
 
-  /* "multimcts/mcts.pyx":211
+  /* "multimcts/mcts.pyx":213
  *             node = node.parent
  * 
  *     def get_best_child(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         cur_team = node.state.get_current_team()
- *         cdef float ln_parent_visits = log(node.num_visits)
+ * 
  */
-  __pyx_tuple__45 = PyTuple_Pack(13, __pyx_n_s_self, __pyx_n_s_node, __pyx_n_s_cur_team, __pyx_n_s_ln_parent_visits, __pyx_n_s_reward, __pyx_n_s_score, __pyx_n_s_visits, __pyx_n_s_exploration_bias, __pyx_n_s_max_score, __pyx_n_s_best, __pyx_n_s_child, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(0, 211, __pyx_L1_error)
+  __pyx_tuple__45 = PyTuple_Pack(13, __pyx_n_s_self, __pyx_n_s_node, __pyx_n_s_cur_team, __pyx_n_s_visits, __pyx_n_s_reward, __pyx_n_s_score, __pyx_n_s_exploration_bias, __pyx_n_s_ln_parent_visits, __pyx_n_s_max_score, __pyx_n_s_best, __pyx_n_s_child, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(0, 213, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__45);
   __Pyx_GIVEREF(__pyx_tuple__45);
-  __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(2, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__45, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_best_child, 211, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(0, 211, __pyx_L1_error)
+  __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(2, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__45, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_multimcts_mcts_pyx, __pyx_n_s_get_best_child, 213, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(0, 213, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -6647,23 +6634,23 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_9multimcts_4mcts___pyx_scope_struct__get_best_child) < 0) __PYX_ERR(0, 211, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_9multimcts_4mcts___pyx_scope_struct__get_best_child) < 0) __PYX_ERR(0, 213, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_9multimcts_4mcts___pyx_scope_struct__get_best_child.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_9multimcts_4mcts___pyx_scope_struct__get_best_child.tp_dictoffset && __pyx_type_9multimcts_4mcts___pyx_scope_struct__get_best_child.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_9multimcts_4mcts___pyx_scope_struct__get_best_child.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_9multimcts_4mcts___pyx_scope_struct__get_best_child = &__pyx_type_9multimcts_4mcts___pyx_scope_struct__get_best_child;
-  if (PyType_Ready(&__pyx_type_9multimcts_4mcts___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 224, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_9multimcts_4mcts___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 227, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_9multimcts_4mcts___pyx_scope_struct_1_genexpr.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_9multimcts_4mcts___pyx_scope_struct_1_genexpr.tp_dictoffset && __pyx_type_9multimcts_4mcts___pyx_scope_struct_1_genexpr.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_9multimcts_4mcts___pyx_scope_struct_1_genexpr.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_9multimcts_4mcts___pyx_scope_struct_1_genexpr = &__pyx_type_9multimcts_4mcts___pyx_scope_struct_1_genexpr;
@@ -6794,15 +6781,14 @@
 {
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
@@ -6901,153 +6887,155 @@
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
   /* "multimcts/mcts.pyx":1
- * import time             # <<<<<<<<<<<<<<
+ * from time import time             # <<<<<<<<<<<<<<
  * from collections import defaultdict
- * from typing import Union, Iterator, Dict, Hashable
+ * from typing import Union, Iterator, Hashable
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_time, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_INCREF(__pyx_n_s_time);
+  __Pyx_GIVEREF(__pyx_n_s_time);
+  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_time);
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_time, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_time, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "multimcts/mcts.pyx":2
- * import time
+ * from time import time
  * from collections import defaultdict             # <<<<<<<<<<<<<<
- * from typing import Union, Iterator, Dict, Hashable
+ * from typing import Union, Iterator, Hashable
  * 
  */
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_defaultdict);
   __Pyx_GIVEREF(__pyx_n_s_defaultdict);
-  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_defaultdict);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_collections, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_defaultdict); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
+  PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_defaultdict);
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_collections, __pyx_t_2, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_defaultdict, __pyx_t_1) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_defaultdict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_defaultdict, __pyx_t_2) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "multimcts/mcts.pyx":3
- * import time
+ * from time import time
  * from collections import defaultdict
- * from typing import Union, Iterator, Dict, Hashable             # <<<<<<<<<<<<<<
+ * from typing import Union, Iterator, Hashable             # <<<<<<<<<<<<<<
  * 
  * from libc.math cimport log, sqrt
  */
-  __pyx_t_2 = PyList_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = PyList_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_Union);
   __Pyx_GIVEREF(__pyx_n_s_Union);
-  PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_Union);
+  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_Union);
   __Pyx_INCREF(__pyx_n_s_Iterator);
   __Pyx_GIVEREF(__pyx_n_s_Iterator);
-  PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_s_Iterator);
-  __Pyx_INCREF(__pyx_n_s_Dict);
-  __Pyx_GIVEREF(__pyx_n_s_Dict);
-  PyList_SET_ITEM(__pyx_t_2, 2, __pyx_n_s_Dict);
+  PyList_SET_ITEM(__pyx_t_1, 1, __pyx_n_s_Iterator);
   __Pyx_INCREF(__pyx_n_s_Hashable);
   __Pyx_GIVEREF(__pyx_n_s_Hashable);
-  PyList_SET_ITEM(__pyx_t_2, 3, __pyx_n_s_Hashable);
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_typing, __pyx_t_2, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Union); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Union, __pyx_t_2) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Iterator); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Iterator, __pyx_t_2) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Dict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
+  PyList_SET_ITEM(__pyx_t_1, 2, __pyx_n_s_Hashable);
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_typing, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Dict, __pyx_t_2) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Hashable); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Hashable, __pyx_t_2) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Union); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Union, __pyx_t_1) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Iterator); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Iterator, __pyx_t_1) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Hashable); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Hashable, __pyx_t_1) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "multimcts/mcts.pyx":8
  * 
  * 
  * class GameState():             # <<<<<<<<<<<<<<
  *     def get_current_team(self) -> Union[int,str]:
  *         """The identifier of the current player's team."""
  */
-  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_GameState, __pyx_n_s_GameState, (PyObject *) NULL, __pyx_n_s_multimcts_mcts, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 8, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_GameState, __pyx_n_s_GameState, (PyObject *) NULL, __pyx_n_s_multimcts_mcts, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 8, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
 
   /* "multimcts/mcts.pyx":9
  * 
  * class GameState():
  *     def get_current_team(self) -> Union[int,str]:             # <<<<<<<<<<<<<<
  *         """The identifier of the current player's team."""
  *         raise NotImplementedError("GameState must implement get_current_team.")
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Union); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(((PyObject *)(&PyInt_Type)));
   __Pyx_GIVEREF(((PyObject *)(&PyInt_Type)));
   PyTuple_SET_ITEM(__pyx_t_4, 0, ((PyObject *)(&PyInt_Type)));
   __Pyx_INCREF(((PyObject *)(&PyString_Type)));
   __Pyx_GIVEREF(((PyObject *)(&PyString_Type)));
   PyTuple_SET_ITEM(__pyx_t_4, 1, ((PyObject *)(&PyString_Type)));
   __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_t_5) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_return, __pyx_t_5) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_1get_current_team, 0, __pyx_n_s_GameState_get_current_team, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_2);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_current_team, __pyx_t_5) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_1);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_get_current_team, __pyx_t_5) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "multimcts/mcts.pyx":13
  *         raise NotImplementedError("GameState must implement get_current_team.")
  * 
  *     def get_legal_moves(self, randomize:bool=False) -> Iterator[Hashable]:             # <<<<<<<<<<<<<<
  *         """An iterator of all legal moves in this state.
  *         The randomize param instructs the method to yield moves in a random order.
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_randomize, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Iterator); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Iterator); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Hashable); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_t_3) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_3get_legal_moves, 0, __pyx_n_s_GameState_get_legal_moves, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__15);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_legal_moves, __pyx_t_3) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_get_legal_moves, __pyx_t_3) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "multimcts/mcts.pyx":19
  *         raise NotImplementedError("GameState must implement get_legal_moves.")
  * 
  *     def get_random_move(self) -> Hashable:             # <<<<<<<<<<<<<<
  *         """Returns a random legal move from this state."""
@@ -7059,15 +7047,15 @@
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_t_5) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_5get_random_move, 0, __pyx_n_s_GameState_get_random_move, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_random_move, __pyx_t_5) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_get_random_move, __pyx_t_5) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "multimcts/mcts.pyx":23
  *         return next(self.get_legal_moves(True))
  * 
  *     def has_move(self) -> bool:             # <<<<<<<<<<<<<<
  *         """Returns whether there are any legal moves in this state."""
@@ -7076,15 +7064,15 @@
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
   __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_7has_move, 0, __pyx_n_s_GameState_has_move, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_has_move, __pyx_t_3) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_has_move, __pyx_t_3) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "multimcts/mcts.pyx":31
  *             return False
  * 
  *     def make_move(self, move:Hashable) -> 'GameState':             # <<<<<<<<<<<<<<
  *         """Returns a new GameState, which is the result of applying the given move to this state.
@@ -7097,15 +7085,15 @@
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_move, __pyx_t_5) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_GameState) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
   __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_9make_move, 0, __pyx_n_s_GameState_make_move, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_make_move, __pyx_t_5) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_make_move, __pyx_t_5) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "multimcts/mcts.pyx":38
  *         raise NotImplementedError("GameState must implement make_move.")
  * 
  *     def is_terminal(self) -> bool:             # <<<<<<<<<<<<<<
  *         """Checks if the game is over."""
@@ -7114,404 +7102,400 @@
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 38, __pyx_L1_error)
   __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_11is_terminal, 0, __pyx_n_s_GameState_is_terminal, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_is_terminal, __pyx_t_3) < 0) __PYX_ERR(0, 38, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_is_terminal, __pyx_t_3) < 0) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "multimcts/mcts.pyx":42
  *         raise NotImplementedError("GameState must implement is_terminal.")
  * 
- *     def get_reward(self) -> Union[float, Dict[Union[int,str], float]]:             # <<<<<<<<<<<<<<
+ *     def get_reward(self) -> Union[float, dict[Union[int,str], float]]:             # <<<<<<<<<<<<<<
  *         """Returns the reward earned by the team that played the game-ending move.
  *         Typically 1 for win, -1 for loss, 0 for draw.
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Union); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Dict); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Union); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Union); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 42, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 42, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(((PyObject *)(&PyInt_Type)));
   __Pyx_GIVEREF(((PyObject *)(&PyInt_Type)));
-  PyTuple_SET_ITEM(__pyx_t_6, 0, ((PyObject *)(&PyInt_Type)));
+  PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)(&PyInt_Type)));
   __Pyx_INCREF(((PyObject *)(&PyString_Type)));
   __Pyx_GIVEREF(((PyObject *)(&PyString_Type)));
-  PyTuple_SET_ITEM(__pyx_t_6, 1, ((PyObject *)(&PyString_Type)));
-  __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 42, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 42, __pyx_L1_error)
+  PyTuple_SET_ITEM(__pyx_t_1, 1, ((PyObject *)(&PyString_Type)));
+  __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GIVEREF(__pyx_t_7);
-  PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_7);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_6);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_6);
   __Pyx_INCREF(((PyObject *)(&PyFloat_Type)));
   __Pyx_GIVEREF(((PyObject *)(&PyFloat_Type)));
-  PyTuple_SET_ITEM(__pyx_t_6, 1, ((PyObject *)(&PyFloat_Type)));
-  __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 42, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 42, __pyx_L1_error)
+  PyTuple_SET_ITEM(__pyx_t_1, 1, ((PyObject *)(&PyFloat_Type)));
+  __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)(&PyDict_Type)), __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(((PyObject *)(&PyFloat_Type)));
   __Pyx_GIVEREF(((PyObject *)(&PyFloat_Type)));
-  PyTuple_SET_ITEM(__pyx_t_6, 0, ((PyObject *)(&PyFloat_Type)));
-  __Pyx_GIVEREF(__pyx_t_7);
-  PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_7);
-  __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 42, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)(&PyFloat_Type)));
+  __Pyx_GIVEREF(__pyx_t_6);
+  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_6);
+  __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_t_6) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_t_7) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_13get_reward, 0, __pyx_n_s_GameState_get_reward, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 42, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_3);
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_13get_reward, 0, __pyx_n_s_GameState_get_reward, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_6, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_reward, __pyx_t_7) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_get_reward, __pyx_t_6) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
   /* "multimcts/mcts.pyx":50
  *         raise NotImplementedError("GameState must implement get_reward.")
  * 
  *     def __hash__(self) -> int:             # <<<<<<<<<<<<<<
  *         raise NotImplementedError("GameState must implement __hash__")
  * 
  */
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 50, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_return, __pyx_n_u_int) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_return, __pyx_n_u_int) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
   __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_15__hash__, 0, __pyx_n_s_GameState___hash, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_7);
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_hash, __pyx_t_3) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_6);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_hash, __pyx_t_3) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "multimcts/mcts.pyx":53
  *         raise NotImplementedError("GameState must implement __hash__")
  * 
  *     def __eq__(self, other:'GameState') -> bool:             # <<<<<<<<<<<<<<
  *         raise NotImplementedError("GameStates must implement __eq__")
  * 
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_other, __pyx_n_s_GameState) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_17__eq__, 0, __pyx_n_s_GameState___eq, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 53, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_3);
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_9GameState_17__eq__, 0, __pyx_n_s_GameState___eq, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_6, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_eq, __pyx_t_7) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_eq, __pyx_t_6) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
   /* "multimcts/mcts.pyx":8
  * 
  * 
  * class GameState():             # <<<<<<<<<<<<<<
  *     def get_current_team(self) -> Union[int,str]:
  *         """The identifier of the current player's team."""
  */
-  __pyx_t_7 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_GameState, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 8, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_GameState, __pyx_t_7) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_6 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_GameState, __pyx_empty_tuple, __pyx_t_2, NULL, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 8, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_GameState, __pyx_t_6) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "multimcts/mcts.pyx":57
  * 
  * 
  * class Node():             # <<<<<<<<<<<<<<
  *     """Represents a game state node in the MCTS search tree.
  * 
  */
-  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_Node, __pyx_n_s_Node, (PyObject *) NULL, __pyx_n_s_multimcts_mcts, __pyx_kp_s_Represents_a_game_state_node_in); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_Node, __pyx_n_s_Node, (PyObject *) NULL, __pyx_n_s_multimcts_mcts, __pyx_kp_s_Represents_a_game_state_node_in); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
 
   /* "multimcts/mcts.pyx":72
  *         remaining_moves (list): A list of moves that have not yet been tried.
  *     """
  *     def __init__(self, state:GameState, parent:'Node'=None):             # <<<<<<<<<<<<<<
  *         self.state = state
  *         self.parent = parent
  */
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 72, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_GameState); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_state, __pyx_t_3) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_state, __pyx_t_3) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_parent, __pyx_n_s_Node) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_parent, __pyx_n_s_Node) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
   __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4Node_1__init__, 0, __pyx_n_s_Node___init, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__32);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_7);
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_3) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_6);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_init, __pyx_t_3) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "multimcts/mcts.pyx":57
  * 
  * 
  * class Node():             # <<<<<<<<<<<<<<
  *     """Represents a game state node in the MCTS search tree.
  * 
  */
-  __pyx_t_3 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_Node, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_Node, __pyx_empty_tuple, __pyx_t_2, NULL, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Node, __pyx_t_3) < 0) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "multimcts/mcts.pyx":86
  * 
  * 
  * class MCTS():             # <<<<<<<<<<<<<<
  *     def __init__(self, *, exploration_bias:float=1.414, heuristic=None, max_time:float=None, max_iterations:int=None):
  *         """Initializes an MCTS agent.
  */
-  __pyx_t_1 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_MCTS, __pyx_n_s_MCTS, (PyObject *) NULL, __pyx_n_s_multimcts_mcts, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_MCTS, __pyx_n_s_MCTS, (PyObject *) NULL, __pyx_n_s_multimcts_mcts, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
 
   /* "multimcts/mcts.pyx":87
  * 
  * class MCTS():
  *     def __init__(self, *, exploration_bias:float=1.414, heuristic=None, max_time:float=None, max_iterations:int=None):             # <<<<<<<<<<<<<<
  *         """Initializes an MCTS agent.
  * 
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = PyFloat_FromDouble(((double)1.414)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 87, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_exploration_bias, __pyx_t_7) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_6 = PyFloat_FromDouble(((double)1.414)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_exploration_bias, __pyx_t_6) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_heuristic, ((PyObject *)Py_None)) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_max_time, ((PyObject *)Py_None)) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_max_iterations, ((PyObject *)Py_None)) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 87, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_exploration_bias, __pyx_n_u_float) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_max_time, __pyx_n_u_float) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_max_iterations, __pyx_n_u_int) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_1__init__, 0, __pyx_n_s_MCTS___init, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_6, __pyx_t_3);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_6, __pyx_t_7);
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_exploration_bias, __pyx_n_u_float) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_max_time, __pyx_n_u_float) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_max_iterations, __pyx_n_u_int) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_1__init__, 0, __pyx_n_s_MCTS___init, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_1, __pyx_t_3);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_1, __pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_6) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_init, __pyx_t_1) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "multimcts/mcts.pyx":109
  *         self.max_iterations = max_iterations
  * 
  *     def search(self, state:GameState) -> GameState:             # <<<<<<<<<<<<<<
  *         """Searches for this state's best move until some limit has been reached.
  * 
  */
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_GameState); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_GameState); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 109, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_state, __pyx_t_7) < 0) __PYX_ERR(0, 109, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_GameState); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 109, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_return, __pyx_t_7) < 0) __PYX_ERR(0, 109, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_3search, 0, __pyx_n_s_MCTS_search, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__36)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 109, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_6);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_state, __pyx_t_6) < 0) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_GameState); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_return, __pyx_t_6) < 0) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_3search, 0, __pyx_n_s_MCTS_search, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__36)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_6, __pyx_t_1);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_search, __pyx_t_6) < 0) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_search, __pyx_t_7) < 0) __PYX_ERR(0, 109, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "multimcts/mcts.pyx":138
+  /* "multimcts/mcts.pyx":140
  *         return self.get_best_child(node).state
  * 
  *     def select(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 1: Selection
  *         Traverse the tree for the node we most want to simulate.
  */
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 138, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Node); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 138, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_node, __pyx_t_6) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Node); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 138, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_return, __pyx_t_6) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_5select, 0, __pyx_n_s_MCTS_select, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__38)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 138, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 140, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_6, __pyx_t_7);
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_select, __pyx_t_6) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Node); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 140, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_node, __pyx_t_1) < 0) __PYX_ERR(0, 140, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Node); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 140, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_return, __pyx_t_1) < 0) __PYX_ERR(0, 140, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_5select, 0, __pyx_n_s_MCTS_select, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__38)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 140, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_1, __pyx_t_6);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_select, __pyx_t_1) < 0) __PYX_ERR(0, 140, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":152
+  /* "multimcts/mcts.pyx":154
  * 
  *     @staticmethod
  *     def expand(node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         """Step 2: Expansion
  *         Add a new child to this node.
  */
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Node); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_node, __pyx_t_6) < 0) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Node); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 154, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Node); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 152, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_node, __pyx_t_7) < 0) __PYX_ERR(0, 152, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Node); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 152, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_return, __pyx_t_7) < 0) __PYX_ERR(0, 152, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_7expand, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_MCTS_expand, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__40)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 152, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_6);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_return, __pyx_t_6) < 0) __PYX_ERR(0, 154, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_7expand, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_MCTS_expand, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__40)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_6, __pyx_t_1);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":151
+  /* "multimcts/mcts.pyx":153
  *         return node
  * 
  *     @staticmethod             # <<<<<<<<<<<<<<
  *     def expand(node:Node) -> Node:
  *         """Step 2: Expansion
  */
-  __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 151, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_expand, __pyx_t_6) < 0) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 153, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_expand, __pyx_t_1) < 0) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "multimcts/mcts.pyx":168
+  /* "multimcts/mcts.pyx":170
  *             raise Exception("Tried to expand a fully-expanded or terminal node.")
  * 
  *     def simulate(self, node:Node) -> dict:             # <<<<<<<<<<<<<<
  *         """Step 3: Simulation (aka playout, rollout)
  *         Play out a random game, from this node to termination, and return the final reward.
  */
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 170, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Node); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 170, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Node); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_node, __pyx_t_7) < 0) __PYX_ERR(0, 168, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_return, __pyx_n_u_dict) < 0) __PYX_ERR(0, 168, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_9simulate, 0, __pyx_n_s_MCTS_simulate, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__42)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 168, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_6);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_node, __pyx_t_6) < 0) __PYX_ERR(0, 170, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_return, __pyx_n_u_dict) < 0) __PYX_ERR(0, 170, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_9simulate, 0, __pyx_n_s_MCTS_simulate, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__42)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 170, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_6, __pyx_t_1);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_simulate, __pyx_t_6) < 0) __PYX_ERR(0, 170, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_simulate, __pyx_t_7) < 0) __PYX_ERR(0, 168, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "multimcts/mcts.pyx":196
+  /* "multimcts/mcts.pyx":198
  * 
  *     @staticmethod
  *     def backpropagate(node:Node, reward:dict):             # <<<<<<<<<<<<<<
  *         """Step 4: Backpropagation
  *         Update all ancestors with the reward from this terminal node.
  */
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 196, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Node); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 198, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_node, __pyx_t_6) < 0) __PYX_ERR(0, 196, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Node); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 198, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_node, __pyx_t_1) < 0) __PYX_ERR(0, 198, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_reward, __pyx_n_u_dict) < 0) __PYX_ERR(0, 198, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_11backpropagate, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_MCTS_backpropagate, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 198, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_1, __pyx_t_6);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_reward, __pyx_n_u_dict) < 0) __PYX_ERR(0, 196, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_11backpropagate, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_MCTS_backpropagate, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 196, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_6, __pyx_t_7);
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "multimcts/mcts.pyx":195
+  /* "multimcts/mcts.pyx":197
  *         return reward
  * 
  *     @staticmethod             # <<<<<<<<<<<<<<
  *     def backpropagate(node:Node, reward:dict):
  *         """Step 4: Backpropagation
  */
-  __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 195, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_backpropagate, __pyx_t_6) < 0) __PYX_ERR(0, 198, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_backpropagate, __pyx_t_7) < 0) __PYX_ERR(0, 196, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "multimcts/mcts.pyx":211
+  /* "multimcts/mcts.pyx":213
  *             node = node.parent
  * 
  *     def get_best_child(self, node:Node) -> Node:             # <<<<<<<<<<<<<<
  *         cur_team = node.state.get_current_team()
- *         cdef float ln_parent_visits = log(node.num_visits)
+ * 
  */
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 211, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Node); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 211, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 213, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_node, __pyx_t_6) < 0) __PYX_ERR(0, 211, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Node); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 211, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_return, __pyx_t_6) < 0) __PYX_ERR(0, 211, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_13get_best_child, 0, __pyx_n_s_MCTS_get_best_child, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__46)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 211, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_6, __pyx_t_7);
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_best_child, __pyx_t_6) < 0) __PYX_ERR(0, 211, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Node); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 213, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_node, __pyx_t_1) < 0) __PYX_ERR(0, 213, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Node); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 213, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_return, __pyx_t_1) < 0) __PYX_ERR(0, 213, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9multimcts_4mcts_4MCTS_13get_best_child, 0, __pyx_n_s_MCTS_get_best_child, NULL, __pyx_n_s_multimcts_mcts, __pyx_d, ((PyObject *)__pyx_codeobj__46)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 213, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_1, __pyx_t_6);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_get_best_child, __pyx_t_1) < 0) __PYX_ERR(0, 213, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "multimcts/mcts.pyx":86
  * 
  * 
  * class MCTS():             # <<<<<<<<<<<<<<
  *     def __init__(self, *, exploration_bias:float=1.414, heuristic=None, max_time:float=None, max_iterations:int=None):
  *         """Initializes an MCTS agent.
  */
-  __pyx_t_6 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_MCTS, __pyx_empty_tuple, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 86, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_MCTS, __pyx_t_6) < 0) __PYX_ERR(0, 86, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_1 = __Pyx_Py3ClassCreate(((PyObject*)&__Pyx_DefaultClassType), __pyx_n_s_MCTS, __pyx_empty_tuple, __pyx_t_2, NULL, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_MCTS, __pyx_t_1) < 0) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "multimcts/mcts.pyx":1
- * import time             # <<<<<<<<<<<<<<
+ * from time import time             # <<<<<<<<<<<<<<
  * from collections import defaultdict
- * from typing import Union, Iterator, Dict, Hashable
+ * from typing import Union, Iterator, Hashable
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
   if (__pyx_m) {
     if (__pyx_d) {
       __Pyx_AddTraceback("init multimcts.mcts", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
     PyErr_SetString(PyExc_ImportError, "init multimcts.mcts");
@@ -8452,143 +8436,14 @@
         return __Pyx_NewRef(result);
     }
     PyErr_Clear();
 #endif
     return __Pyx_GetBuiltinName(name);
 }
 
-/* None */
-static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname) {
-    PyErr_Format(PyExc_UnboundLocalError, "local variable '%s' referenced before assignment", varname);
-}
-
-/* PyIntBinop */
-#if !CYTHON_COMPILING_IN_PYPY
-static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, CYTHON_UNUSED long intval, int inplace, int zerodivision_check) {
-    (void)inplace;
-    (void)zerodivision_check;
-    #if PY_MAJOR_VERSION < 3
-    if (likely(PyInt_CheckExact(op1))) {
-        const long b = intval;
-        long x;
-        long a = PyInt_AS_LONG(op1);
-            x = (long)((unsigned long)a + b);
-            if (likely((x^a) >= 0 || (x^b) >= 0))
-                return PyInt_FromLong(x);
-            return PyLong_Type.tp_as_number->nb_add(op1, op2);
-    }
-    #endif
-    #if CYTHON_USE_PYLONG_INTERNALS
-    if (likely(PyLong_CheckExact(op1))) {
-        const long b = intval;
-        long a, x;
-#ifdef HAVE_LONG_LONG
-        const PY_LONG_LONG llb = intval;
-        PY_LONG_LONG lla, llx;
-#endif
-        const digit* digits = ((PyLongObject*)op1)->ob_digit;
-        const Py_ssize_t size = Py_SIZE(op1);
-        if (likely(__Pyx_sst_abs(size) <= 1)) {
-            a = likely(size) ? digits[0] : 0;
-            if (size == -1) a = -a;
-        } else {
-            switch (size) {
-                case -2:
-                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                        a = -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-#ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
-                        lla = -(PY_LONG_LONG) (((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-#endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case 2:
-                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                        a = (long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-#ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
-                        lla = (PY_LONG_LONG) (((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-#endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case -3:
-                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                        a = -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-#ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
-                        lla = -(PY_LONG_LONG) (((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-#endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case 3:
-                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                        a = (long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-#ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
-                        lla = (PY_LONG_LONG) (((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-#endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case -4:
-                    if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                        a = -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-#ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
-                        lla = -(PY_LONG_LONG) (((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-#endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                case 4:
-                    if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                        a = (long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
-                        break;
-#ifdef HAVE_LONG_LONG
-                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
-                        lla = (PY_LONG_LONG) (((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
-                        goto long_long;
-#endif
-                    }
-                    CYTHON_FALLTHROUGH;
-                default: return PyLong_Type.tp_as_number->nb_add(op1, op2);
-            }
-        }
-                x = a + b;
-            return PyLong_FromLong(x);
-#ifdef HAVE_LONG_LONG
-        long_long:
-                llx = lla + llb;
-            return PyLong_FromLongLong(llx);
-#endif
-        
-        
-    }
-    #endif
-    if (PyFloat_CheckExact(op1)) {
-        const long b = intval;
-        double a = PyFloat_AS_DOUBLE(op1);
-            double result;
-            PyFPE_START_PROTECT("add", return NULL)
-            result = ((double)a) + (double)b;
-            PyFPE_END_PROTECT(result)
-            return PyFloat_FromDouble(result);
-    }
-    return (inplace ? PyNumber_InPlaceAdd : PyNumber_Add)(op1, op2);
-}
-#endif
-
 /* PyObjectGetMethod */
 static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
     PyObject *attr;
 #if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
     PyTypeObject *tp = Py_TYPE(obj);
     PyObject *descr;
     descrgetfunc f = NULL;
@@ -8749,14 +8604,19 @@
         __Pyx_SET_SIZE(L, Py_SIZE(L) - 1);
         return PyList_GET_ITEM(L, PyList_GET_SIZE(L));
     }
     return __Pyx_CallUnboundCMethod0(&__pyx_umethod_PyList_Type_pop, L);
 }
 #endif
 
+/* None */
+static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname) {
+    PyErr_Format(PyExc_UnboundLocalError, "local variable '%s' referenced before assignment", varname);
+}
+
 /* ArgTypeTest */
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
 {
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
         return 0;
     }
@@ -8903,14 +8763,138 @@
         double a = PyFloat_AS_DOUBLE(op1);
         if ((double)a != (double)b) Py_RETURN_TRUE; else Py_RETURN_FALSE;
     }
     return (
         PyObject_RichCompare(op1, op2, Py_NE));
 }
 
+/* PyIntBinop */
+#if !CYTHON_COMPILING_IN_PYPY
+static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, CYTHON_UNUSED long intval, int inplace, int zerodivision_check) {
+    (void)inplace;
+    (void)zerodivision_check;
+    #if PY_MAJOR_VERSION < 3
+    if (likely(PyInt_CheckExact(op1))) {
+        const long b = intval;
+        long x;
+        long a = PyInt_AS_LONG(op1);
+            x = (long)((unsigned long)a + b);
+            if (likely((x^a) >= 0 || (x^b) >= 0))
+                return PyInt_FromLong(x);
+            return PyLong_Type.tp_as_number->nb_add(op1, op2);
+    }
+    #endif
+    #if CYTHON_USE_PYLONG_INTERNALS
+    if (likely(PyLong_CheckExact(op1))) {
+        const long b = intval;
+        long a, x;
+#ifdef HAVE_LONG_LONG
+        const PY_LONG_LONG llb = intval;
+        PY_LONG_LONG lla, llx;
+#endif
+        const digit* digits = ((PyLongObject*)op1)->ob_digit;
+        const Py_ssize_t size = Py_SIZE(op1);
+        if (likely(__Pyx_sst_abs(size) <= 1)) {
+            a = likely(size) ? digits[0] : 0;
+            if (size == -1) a = -a;
+        } else {
+            switch (size) {
+                case -2:
+                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
+                        a = -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                        break;
+#ifdef HAVE_LONG_LONG
+                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
+                        lla = -(PY_LONG_LONG) (((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
+                        goto long_long;
+#endif
+                    }
+                    CYTHON_FALLTHROUGH;
+                case 2:
+                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
+                        a = (long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                        break;
+#ifdef HAVE_LONG_LONG
+                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
+                        lla = (PY_LONG_LONG) (((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
+                        goto long_long;
+#endif
+                    }
+                    CYTHON_FALLTHROUGH;
+                case -3:
+                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
+                        a = -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                        break;
+#ifdef HAVE_LONG_LONG
+                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
+                        lla = -(PY_LONG_LONG) (((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
+                        goto long_long;
+#endif
+                    }
+                    CYTHON_FALLTHROUGH;
+                case 3:
+                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
+                        a = (long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                        break;
+#ifdef HAVE_LONG_LONG
+                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
+                        lla = (PY_LONG_LONG) (((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
+                        goto long_long;
+#endif
+                    }
+                    CYTHON_FALLTHROUGH;
+                case -4:
+                    if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
+                        a = -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                        break;
+#ifdef HAVE_LONG_LONG
+                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
+                        lla = -(PY_LONG_LONG) (((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
+                        goto long_long;
+#endif
+                    }
+                    CYTHON_FALLTHROUGH;
+                case 4:
+                    if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
+                        a = (long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
+                        break;
+#ifdef HAVE_LONG_LONG
+                    } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
+                        lla = (PY_LONG_LONG) (((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
+                        goto long_long;
+#endif
+                    }
+                    CYTHON_FALLTHROUGH;
+                default: return PyLong_Type.tp_as_number->nb_add(op1, op2);
+            }
+        }
+                x = a + b;
+            return PyLong_FromLong(x);
+#ifdef HAVE_LONG_LONG
+        long_long:
+                llx = lla + llb;
+            return PyLong_FromLongLong(llx);
+#endif
+        
+        
+    }
+    #endif
+    if (PyFloat_CheckExact(op1)) {
+        const long b = intval;
+        double a = PyFloat_AS_DOUBLE(op1);
+            double result;
+            PyFPE_START_PROTECT("add", return NULL)
+            result = ((double)a) + (double)b;
+            PyFPE_END_PROTECT(result)
+            return PyFloat_FromDouble(result);
+    }
+    return (inplace ? PyNumber_InPlaceAdd : PyNumber_Add)(op1, op2);
+}
+#endif
+
 /* RaiseNoneIterError */
 static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
 }
 
 /* UnpackTupleError */
 static void __Pyx_UnpackTupleError(PyObject *t, Py_ssize_t index) {
```

### Comparing `multimcts-0.1.4/multimcts/mcts.pyx` & `multimcts-0.1.5/multimcts/mcts.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import time
+from time import time
 from collections import defaultdict
-from typing import Union, Iterator, Dict, Hashable
+from typing import Union, Iterator, Hashable
 
 from libc.math cimport log, sqrt
 
 
 class GameState():
     def get_current_team(self) -> Union[int,str]:
         """The identifier of the current player's team."""
@@ -35,15 +35,15 @@
         """
         raise NotImplementedError("GameState must implement make_move.")
 
     def is_terminal(self) -> bool:
         """Checks if the game is over."""
         raise NotImplementedError("GameState must implement is_terminal.")
 
-    def get_reward(self) -> Union[float, Dict[Union[int,str], float]]:
+    def get_reward(self) -> Union[float, dict[Union[int,str], float]]:
         """Returns the reward earned by the team that played the game-ending move.
         Typically 1 for win, -1 for loss, 0 for draw.
         Alternatively, returns a dict of format {team:reward} or {team1:reward1, team2:reward2, ...}
         Note: This method is only evaluated on terminal states.
         """
         raise NotImplementedError("GameState must implement get_reward.")
 
@@ -69,15 +69,15 @@
         is_fully_expanded (bool): Whether all children of the node have been visited.
         remaining_moves (list): A list of moves that have not yet been tried.
     """
     def __init__(self, state:GameState, parent:'Node'=None):
         self.state = state
         self.parent = parent
 
-        self.children:Dict[Hashable,'Node'] = {}
+        self.children:dict[Hashable,'Node'] = {}
         self.num_visits = 0
         self.total_reward = defaultdict(float)
 
         self.is_terminal = self.state.is_terminal()
         self.is_fully_expanded = self.is_terminal
 
         self.remaining_moves = [] if self.is_fully_expanded else list(self.state.get_legal_moves(True))
@@ -93,15 +93,15 @@
                 Default is 1.414, which is sqrt(2) and often used in practice.
             heuristic (function): A function that can be used to guide the simulation step.
                 The function should take a GameState object as an argument and return a legal move.
                 If no heuristic is provided, a random legal move is chosen.
             max_time (float): The maximum time, in seconds, that the search method should run.
             max_iterations (int): The maximum number of iterations that the search method should execute.
         """
-        if max_iterations is None and max_time is None:
+        if max_time is None and max_iterations is None:
             raise ValueError("One or more of max_time/max_iterations is required.")
 
         self.exploration_bias = exploration_bias
         self.heuristic = heuristic
 
         self.max_time = max_time
         self.max_iterations = max_iterations
@@ -112,29 +112,31 @@
         Args:
             state (GameState): The game state for which to find the best move.
         Returns:
             GameState: A new game state which is the result of applying the best move to the given state.
         """
         node = Node(state)
 
+        cdef float end_time
+        cdef int i
         if self.max_time is not None:
-            end_time = time.time() + self.max_time
+            end_time = time() + self.max_time
         if self.max_iterations is not None:
-            i = 0
+            i = self.max_iterations
 
         while True:
             child = self.select(node)
             reward = self.simulate(child)
             self.backpropagate(child, reward)
 
-            if self.max_time is not None and time.time() >= end_time:
+            if self.max_time is not None and time() >= end_time:
                 break
             if self.max_iterations is not None:
-                i += 1
-                if i >= self.max_iterations:
+                i -= 1
+                if i <= 0:
                     break
 
         return self.get_best_child(node).state
 
     def select(self, node:Node) -> Node:
         """Step 1: Selection
         Traverse the tree for the node we most want to simulate.
@@ -206,22 +208,23 @@
             for key in reward:
                 node.total_reward[key] += reward[key]
 
             node = node.parent
 
     def get_best_child(self, node:Node) -> Node:
         cur_team = node.state.get_current_team()
-        cdef float ln_parent_visits = log(node.num_visits)
 
-        cdef float reward, score
+        # Initialize UCB variables.
         cdef int visits
+        cdef float reward, score
         cdef float exploration_bias = self.exploration_bias
+        cdef float ln_parent_visits = log(node.num_visits)
 
         cdef float max_score = float('-inf')
-        best = None
+        best:Node = None
 
         for child in node.children.values():
             # Relative reward is this child's reward minus its siblings' rewards.
             reward = (2 * child.total_reward[cur_team]) - sum(x for x in child.total_reward.values())
             visits = child.num_visits
 
             """UCB := (x / n) + C * sqrt(ln(N) / n)
```

