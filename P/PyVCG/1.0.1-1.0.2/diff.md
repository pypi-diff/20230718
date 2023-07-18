# Comparing `tmp/PyVCG-1.0.1.tar.gz` & `tmp/PyVCG-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyVCG-1.0.1.tar", last modified: Fri Jul 14 07:41:35 2023, max compression
+gzip compressed data, was "PyVCG-1.0.2.tar", last modified: Tue Jul 18 13:07:10 2023, max compression
```

## Comparing `PyVCG-1.0.1.tar` & `PyVCG-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-14 07:41:35.467819 PyVCG-1.0.1/
--rw-r--r--   0 florian   (1000) florian   (1000)    35149 2023-06-30 05:59:33.000000 PyVCG-1.0.1/LICENSE
--rw-r--r--   0 florian   (1000) florian   (1000)     3299 2023-07-14 07:41:35.467819 PyVCG-1.0.1/PKG-INFO
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-14 07:41:35.467819 PyVCG-1.0.1/PyVCG.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     3299 2023-07-14 07:41:35.000000 PyVCG-1.0.1/PyVCG.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      399 2023-07-14 07:41:35.000000 PyVCG-1.0.1/PyVCG.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-07-14 07:41:35.000000 PyVCG-1.0.1/PyVCG.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       12 2023-07-14 07:41:35.000000 PyVCG-1.0.1/PyVCG.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        6 2023-07-14 07:41:35.000000 PyVCG-1.0.1/PyVCG.egg-info/top_level.txt
--rw-r--r--   0 florian   (1000) florian   (1000)     2301 2023-07-11 11:06:20.000000 PyVCG-1.0.1/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-14 07:41:35.467819 PyVCG-1.0.1/pyvcg/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-30 18:37:56.000000 PyVCG-1.0.1/pyvcg/__init__.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-14 07:41:35.467819 PyVCG-1.0.1/pyvcg/driver/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-07-09 17:34:46.000000 PyVCG-1.0.1/pyvcg/driver/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)    20285 2023-07-11 11:06:20.000000 PyVCG-1.0.1/pyvcg/driver/cvc5_api.py
--rw-r--r--   0 florian   (1000) florian   (1000)    13462 2023-07-11 11:06:20.000000 PyVCG-1.0.1/pyvcg/driver/file_smtlib.py
--rw-r--r--   0 florian   (1000) florian   (1000)     6402 2023-07-09 17:38:38.000000 PyVCG-1.0.1/pyvcg/graph.py
--rw-r--r--   0 florian   (1000) florian   (1000)    41586 2023-07-14 07:41:10.000000 PyVCG-1.0.1/pyvcg/smt.py
--rw-r--r--   0 florian   (1000) florian   (1000)     3160 2023-07-04 10:59:04.000000 PyVCG-1.0.1/pyvcg/vcg.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1953 2023-07-14 07:41:32.000000 PyVCG-1.0.1/pyvcg/version.py
--rw-r--r--   0 florian   (1000) florian   (1000)       91 2023-07-14 07:41:35.467819 PyVCG-1.0.1/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2092 2023-07-14 07:41:10.000000 PyVCG-1.0.1/setup.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-14 07:41:35.467819 PyVCG-1.0.1/tests/
--rw-r--r--   0 florian   (1000) florian   (1000)     1851 2023-06-30 09:23:58.000000 PyVCG-1.0.1/tests/testGraphSimple.py
--rw-r--r--   0 florian   (1000) florian   (1000)     3603 2023-07-09 17:37:20.000000 PyVCG-1.0.1/tests/testSimpleVCG.py
--rw-r--r--   0 florian   (1000) florian   (1000)    36399 2023-07-14 07:41:10.000000 PyVCG-1.0.1/tests/testSmt.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-18 13:07:10.210017 PyVCG-1.0.2/
+-rw-r--r--   0 florian   (1000) florian   (1000)    35149 2023-06-30 05:59:33.000000 PyVCG-1.0.2/LICENSE
+-rw-r--r--   0 florian   (1000) florian   (1000)     3299 2023-07-18 13:07:10.210017 PyVCG-1.0.2/PKG-INFO
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-18 13:07:10.206017 PyVCG-1.0.2/PyVCG.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     3299 2023-07-18 13:07:10.000000 PyVCG-1.0.2/PyVCG.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      420 2023-07-18 13:07:10.000000 PyVCG-1.0.2/PyVCG.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-07-18 13:07:10.000000 PyVCG-1.0.2/PyVCG.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       12 2023-07-18 13:07:10.000000 PyVCG-1.0.2/PyVCG.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        6 2023-07-18 13:07:10.000000 PyVCG-1.0.2/PyVCG.egg-info/top_level.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)     2301 2023-07-11 11:06:20.000000 PyVCG-1.0.2/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-18 13:07:10.206017 PyVCG-1.0.2/pyvcg/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-30 18:37:56.000000 PyVCG-1.0.2/pyvcg/__init__.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-18 13:07:10.210017 PyVCG-1.0.2/pyvcg/driver/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-07-09 17:34:46.000000 PyVCG-1.0.2/pyvcg/driver/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    20285 2023-07-11 11:06:20.000000 PyVCG-1.0.2/pyvcg/driver/cvc5_api.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    13890 2023-07-18 13:04:12.000000 PyVCG-1.0.2/pyvcg/driver/file_smtlib.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     6402 2023-07-09 17:38:38.000000 PyVCG-1.0.2/pyvcg/graph.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    41586 2023-07-14 07:41:10.000000 PyVCG-1.0.2/pyvcg/smt.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     3160 2023-07-04 10:59:04.000000 PyVCG-1.0.2/pyvcg/vcg.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     1953 2023-07-18 13:07:07.000000 PyVCG-1.0.2/pyvcg/version.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       91 2023-07-18 13:07:10.210017 PyVCG-1.0.2/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2092 2023-07-14 07:41:10.000000 PyVCG-1.0.2/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-18 13:07:10.210017 PyVCG-1.0.2/tests/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1851 2023-06-30 09:23:58.000000 PyVCG-1.0.2/tests/testGraphSimple.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     3603 2023-07-09 17:37:20.000000 PyVCG-1.0.2/tests/testSimpleVCG.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    36399 2023-07-14 07:41:10.000000 PyVCG-1.0.2/tests/testSmt.py
+-rw-r--r--   0 florian   (1000) florian   (1000)      316 2023-07-18 13:04:12.000000 PyVCG-1.0.2/tests/testStrings.py
```

### Comparing `PyVCG-1.0.1/LICENSE` & `PyVCG-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyVCG-1.0.1/PKG-INFO` & `PyVCG-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyVCG
-Version: 1.0.1
+Version: 1.0.2
 Summary: Verification Condition Generator
 Home-page: https://github.com/florianschanda/PyVCG
 Author: Florian Schanda
 Author-email: florian@schanda.org.uk
 License: GNU General Public License v3
 Project-URL: Bug Tracker, https://github.com/florianschanda/PyVCG/issues
 Project-URL: Documentation, https://github.com/pages/florianschanda/PyVCG/
```

### Comparing `PyVCG-1.0.1/PyVCG.egg-info/PKG-INFO` & `PyVCG-1.0.2/PyVCG.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyVCG
-Version: 1.0.1
+Version: 1.0.2
 Summary: Verification Condition Generator
 Home-page: https://github.com/florianschanda/PyVCG
 Author: Florian Schanda
 Author-email: florian@schanda.org.uk
 License: GNU General Public License v3
 Project-URL: Bug Tracker, https://github.com/florianschanda/PyVCG/issues
 Project-URL: Documentation, https://github.com/pages/florianschanda/PyVCG/
```

### Comparing `PyVCG-1.0.1/README.md` & `PyVCG-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `PyVCG-1.0.1/pyvcg/driver/cvc5_api.py` & `PyVCG-1.0.2/pyvcg/driver/cvc5_api.py`

 * *Files identical despite different names*

### Comparing `PyVCG-1.0.1/pyvcg/driver/file_smtlib.py` & `PyVCG-1.0.2/pyvcg/driver/file_smtlib.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,23 +31,36 @@
     def __init__(self):
         self.lines  = []
         self.values = []
 
     def emit_comment(self, comment):
         assert isinstance(comment, str) or comment is None
         if comment is not None:
-            self.lines.append(";; %s" % comment)
+            self.lines.append(";; %s" % comment.replace("\n", " "))
 
-    def emit_name(self, name):
+    @staticmethod
+    def escape_name(name):
         assert isinstance(name, str) and "|" not in name
         if re.match(r"^[a-zA-Z_][a-zA-Z0-9_]*$", name):
             return name
         else:
             return "|%s|" % name
 
+    @staticmethod
+    def escape_string_literal(string):
+        escaped = ""
+        for c in string:
+            if c == '"':
+                escaped += '""'
+            elif c.isprintable():
+                escaped += c
+            else:
+                escaped += r"\u{%x}" % ord(c)
+        return escaped
+
     def visit_script(self, node, logic, functions):
         assert isinstance(node, smt.Script)
         assert isinstance(logic, str)
         assert isinstance(functions, set)
         assert all(isinstance(function, str)
                    for function in functions)
 
@@ -108,25 +121,25 @@
                                                            tr_value))
 
     def visit_function_declaration(self, node, tr_sort, tr_body):
         assert isinstance(node, smt.Function_Declaration)
 
         self.emit_comment(node.comment)
 
-        tr_name   = self.emit_name(node.function.name)
+        tr_name   = self.escape_name(node.function.name)
 
         if tr_body is None:
             tr_params = " ".join(par.sort.walk(self)
                                  for par in node.function.parameters)
             self.lines.append("(declare-fun %s (%s) %s)" % (tr_name,
                                                             tr_params,
                                                             tr_sort))
 
         else:
-            tr_params = " ".join("(%s %s)" % (self.emit_name(par.name),
+            tr_params = " ".join("(%s %s)" % (self.escape_name(par.name),
                                               par.sort.walk(self))
                                  for par in node.function.parameters)
             self.lines.append("(define-fun %s (%s) %s" % (tr_name,
                                                           tr_params,
                                                           tr_sort))
             self.lines.append("  %s)" % tr_body)
 
@@ -135,49 +148,50 @@
         self.emit_comment(node.comment)
         self.lines.append("(assert %s)" % tr_expression)
 
     def visit_enumeration_declaration(self, node):
         assert isinstance(node, smt.Enumeration_Declaration)
         self.emit_comment(node.comment)
         self.lines.append("(declare-datatype %s (%s))" %
-                          (self.emit_name(node.sort.name),
+                          (self.escape_name(node.sort.name),
                            " ".join("(%s)" % literal
                                     for literal in node.sort.literals)))
 
     def visit_record_declaration(self, node):
         assert isinstance(node, smt.Record_Declaration)
         self.emit_comment(node.comment)
         self.lines.append("(declare-datatype %s ((%s" %
-                          (self.emit_name(node.sort.name),
-                           self.emit_name(node.sort.name + "__cons")))
+                          (self.escape_name(node.sort.name),
+                           self.escape_name(node.sort.name + "__cons")))
         for name, sort in node.sort.components.items():
-            self.lines.append("  (%s %s)" % (self.emit_name(name),
+            self.lines.append("  (%s %s)" % (self.escape_name(name),
                                              sort.walk(self)))
         self.lines[-1] += ")))"
 
     def visit_sort(self, node):
         assert isinstance(node, smt.Sort)
-        return self.emit_name(node.name)
+        return self.escape_name(node.name)
 
     def visit_parametric_sort(self, node, tr_parameters):
         assert isinstance(node, smt.Parametric_Sort)
         assert isinstance(tr_parameters, list)
-        return "(%s %s)" % (self.emit_name(node.name), " ".join(tr_parameters))
+        return "(%s %s)" % (self.escape_name(node.name),
+                            " ".join(tr_parameters))
 
     def visit_function(self, node):
         assert isinstance(node, smt.Function)
-        return self.emit_name(node.name)
+        return self.escape_name(node.name)
 
     def visit_enumeration(self, node):
         assert isinstance(node, smt.Enumeration)
-        return self.emit_name(node.name)
+        return self.escape_name(node.name)
 
     def visit_record(self, node):
         assert isinstance(node, smt.Record)
-        return self.emit_name(node.name)
+        return self.escape_name(node.name)
 
     def visit_boolean_literal(self, node, tr_sort):
         assert isinstance(node, smt.Boolean_Literal)
         return "true" if node.value else "false"
 
     def visit_integer_literal(self, node, tr_sort):
         assert isinstance(node, smt.Integer_Literal)
@@ -194,23 +208,23 @@
 
     def visit_enumeration_literal(self, node, tr_sort):
         assert isinstance(node, smt.Enumeration_Literal)
         return "(as %s %s)" % (node.value, tr_sort)
 
     def visit_string_literal(self, node, tr_sort):
         assert isinstance(node, smt.String_Literal)
-        return '"%s"' % node.value
+        return '"%s"' % self.escape_string_literal(node.value)
 
     def visit_constant(self, node, tr_sort):
         assert isinstance(node, smt.Constant)
-        return self.emit_name(node.name)
+        return self.escape_name(node.name)
 
     def visit_bound_variable(self, node, tr_sort):
         assert isinstance(node, smt.Bound_Variable)
-        return self.emit_name(node.name)
+        return self.escape_name(node.name)
 
     def visit_boolean_negation(self, node, tr_sort, tr_expression):
         assert isinstance(node, smt.Boolean_Negation)
         return "(not %s)" % tr_expression
 
     def visit_conjunction(self, node, tr_sort, tr_terms):
         assert isinstance(node, smt.Conjunction)
@@ -305,11 +319,11 @@
                                    tr_true,
                                    tr_false)
 
     def visit_quantifier(self, node, tr_variables, tr_body):
         assert isinstance(node, smt.Quantifier)
         return "(%s (%s)\n  %s)" % (
             node.kind,
-            " ".join("(%s %s)" % (self.emit_name(var.name),
+            " ".join("(%s %s)" % (self.escape_name(var.name),
                                   var.sort.walk(self))
                      for var in node.variables),
             tr_body)
```

### Comparing `PyVCG-1.0.1/pyvcg/graph.py` & `PyVCG-1.0.2/pyvcg/graph.py`

 * *Files identical despite different names*

### Comparing `PyVCG-1.0.1/pyvcg/smt.py` & `PyVCG-1.0.2/pyvcg/smt.py`

 * *Files identical despite different names*

### Comparing `PyVCG-1.0.1/pyvcg/vcg.py` & `PyVCG-1.0.2/pyvcg/vcg.py`

 * *Files identical despite different names*

### Comparing `PyVCG-1.0.1/pyvcg/version.py` & `PyVCG-1.0.2/pyvcg/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,14 @@
 ##  General Public License for more details.                                ##
 ##                                                                          ##
 ##  You should have received a copy of the GNU General Public License       ##
 ##  along with PyVCG. If not, see <http://www.gnu.org/licenses/>.           ##
 ##                                                                          ##
 ##############################################################################
 
-VERSION_TUPLE = (1, 0, 1)
+VERSION_TUPLE = (1, 0, 2)
 VERSION_SUFFIX = ""
 
 PYVCG_VERSION = ("%u.%u.%u" % VERSION_TUPLE) + \
     ("-%s" % VERSION_SUFFIX if VERSION_SUFFIX else "")
 
 FULL_NAME = "PyVCG %s" % PYVCG_VERSION
```

### Comparing `PyVCG-1.0.1/setup.py` & `PyVCG-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `PyVCG-1.0.1/tests/testGraphSimple.py` & `PyVCG-1.0.2/tests/testGraphSimple.py`

 * *Files identical despite different names*

### Comparing `PyVCG-1.0.1/tests/testSimpleVCG.py` & `PyVCG-1.0.2/tests/testSimpleVCG.py`

 * *Files identical despite different names*

### Comparing `PyVCG-1.0.1/tests/testSmt.py` & `PyVCG-1.0.2/tests/testSmt.py`

 * *Files identical despite different names*

