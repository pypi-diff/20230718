# Comparing `tmp/pyspecter-0.1.0.tar.gz` & `tmp/pyspecter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspecter-0.1.0.tar", last modified: Sun Jan 22 12:57:34 2023, max compression
+gzip compressed data, was "pyspecter-0.1.1.tar", last modified: Tue Jul 18 17:11:00 2023, max compression
```

## Comparing `pyspecter-0.1.0.tar` & `pyspecter-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 12:57:34.076293 pyspecter-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-22 12:57:24.000000 pyspecter-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-01-22 12:57:34.076293 pyspecter-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-01-22 12:57:24.000000 pyspecter-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-01-22 12:57:24.000000 pyspecter-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 12:57:34.076293 pyspecter-0.1.0/pyspecter/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-01-22 12:57:24.000000 pyspecter-0.1.0/pyspecter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-01-22 12:57:24.000000 pyspecter-0.1.0/pyspecter/pyspecter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 12:57:34.076293 pyspecter-0.1.0/pyspecter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-01-22 12:57:34.000000 pyspecter-0.1.0/pyspecter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-01-22 12:57:34.000000 pyspecter-0.1.0/pyspecter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-22 12:57:34.000000 pyspecter-0.1.0/pyspecter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-22 12:57:34.000000 pyspecter-0.1.0/pyspecter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-22 12:57:34.076293 pyspecter-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-01-22 12:57:24.000000 pyspecter-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:11:00.277242 pyspecter-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-18 17:10:48.000000 pyspecter-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-07-18 17:11:00.277242 pyspecter-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-07-18 17:10:48.000000 pyspecter-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-18 17:10:48.000000 pyspecter-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:11:00.277242 pyspecter-0.1.1/pyspecter/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-18 17:10:48.000000 pyspecter-0.1.1/pyspecter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-07-18 17:10:48.000000 pyspecter-0.1.1/pyspecter/pyspecter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:11:00.277242 pyspecter-0.1.1/pyspecter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-07-18 17:11:00.000000 pyspecter-0.1.1/pyspecter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-18 17:11:00.000000 pyspecter-0.1.1/pyspecter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 17:11:00.000000 pyspecter-0.1.1/pyspecter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 17:11:00.000000 pyspecter-0.1.1/pyspecter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 17:11:00.277242 pyspecter-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-18 17:10:48.000000 pyspecter-0.1.1/setup.py
```

### Comparing `pyspecter-0.1.0/LICENSE` & `pyspecter-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspecter-0.1.0/PKG-INFO` & `pyspecter-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspecter
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library to query nested data in Python
 Home-page: https://github.com/yellowbean/pyspecter
 Author: Xiaoyu Zhang
 Author-email: always.zhang@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -80,14 +80,26 @@
     assert query(m, ["C", (S.FILTER, lambda k, v: k.endswith("2"))]) == [[3, 4]]
 
 Navigate to map which its key or value satisify a custom function 
 
     assert query(m, ["A", (S.MKEY_IF, lambda x:x.endswith("1"))]) == [[10, 20]]
     assert query(m, ["A", (S.MVAL_IF, lambda x:x==[10,20])]) == [[10, 20]]
     
+#### Branching paths
+
+Branching by multiple paths
+
+    mpath = {"A":{"B":1,
+                  "C":[2,3,4,5]}}
+    assert query(mpath,["A",
+                        (S.MULTI_PATH,["B"]
+                                     ,["C", S.LAST])]) == [1,5]
+
+
+
 #### Conditional Navigation
 
 Navigate to a specifie path
 
     assert query(m, ["D", (S.NTH_PATH, 2)]) == [3]
 
 Navigate to a position if and only if the path exists
```

### Comparing `pyspecter-0.1.0/README.md` & `pyspecter-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,26 @@
     assert query(m, ["C", (S.FILTER, lambda k, v: k.endswith("2"))]) == [[3, 4]]
 
 Navigate to map which its key or value satisify a custom function 
 
     assert query(m, ["A", (S.MKEY_IF, lambda x:x.endswith("1"))]) == [[10, 20]]
     assert query(m, ["A", (S.MVAL_IF, lambda x:x==[10,20])]) == [[10, 20]]
     
+#### Branching paths
+
+Branching by multiple paths
+
+    mpath = {"A":{"B":1,
+                  "C":[2,3,4,5]}}
+    assert query(mpath,["A",
+                        (S.MULTI_PATH,["B"]
+                                     ,["C", S.LAST])]) == [1,5]
+
+
+
 #### Conditional Navigation
 
 Navigate to a specifie path
 
     assert query(m, ["D", (S.NTH_PATH, 2)]) == [3]
 
 Navigate to a position if and only if the path exists
```

### Comparing `pyspecter-0.1.0/pyspecter/pyspecter.py` & `pyspecter-0.1.1/pyspecter/pyspecter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
 from functools import reduce  # forward compatibility for Python 3
 import operator
-import re
+import re,json,os
 
 
 def getFromDict(dataDict, mapList):
     return reduce(operator.getitem, mapList, dataDict)
 
 def lookupMap(m,ks):
     if not isinstance(m, dict) and len(ks) > 0:
@@ -46,23 +46,24 @@
     IF_PATH=23
     REGEX=24
     MAYBE=25
 
 class H(Enum):
     REDUCE=0 #
     MAP=1 #
-    ORDER=2 # 
+    ORDER=2 #
     MAX=3 #
     MIN=4 #
     SUM=5 #
+    COUNT=6
 
 
-def query(d,p,debug=False):
+def query(d, p, debug=False):
     if debug:
-        print("matching",d,p)
+        print(f"matching path={p} with data: {d}")
     match p:
         case []:
             return d
         case [S.MKEYS,*_r] if isinstance(d,dict):
             return query(list(d.keys()),_r)
         case [S.ALL,*_r] :
             if isinstance(d,list) or isinstance(d,range):
@@ -125,15 +126,15 @@
         case [S.VAL, *_r]:
             sub_result = query(d,_r)
             return [ [d, _] for _ in sub_result ]
         case [(S.NONE_VAL, v), *_r]:
             if d is None:
                 return v
             return query(d, _r)
-        case [(S.SRANGE, s,e), *_r]:
+        case [(S.SRANGE, s, e), *_r]:
             return query(d[s:e], _r)
         case [(S.MUST,*k), *_r]:
             x = lookupMap(d, k)
             return query(x, _r)
         case [(S.IF_PATH, cond, t), *_r]:
             if lookupMap(d, cond):
                 return query(d, t + _r)
@@ -141,19 +142,17 @@
                 return None
         case [(S.IF_PATH, cond,t,f), *_r]:
             if lookupMap(d, cond):
                 return query(d, t + _r)
             else:
                 return query(d, f + _r)
         case [(S.REGEX, reg), *_r] if isinstance(d,dict):
-            pass_keys = [ query(d[k], _r) for k in d.keys() if re.match(reg,k) ]
-            return pass_keys
+            return [ query(d[k], _r) for k in d.keys() if re.match(reg,k) ]
         case [(S.REGEX, reg), *_r] if isinstance(d,list):
-            pass_keys = [ query(d[i], _r) for i,k in enumerate(d) if re.match(reg,k) ]
-            return pass_keys
+            return [ query(d[i], _r) for i,k in enumerate(d) if re.match(reg,k) ]
         case [(S.MAYBE, *m), *_r]:
             if len(m)>0 :
                 new_m = m[1:]
                 if m[0] in d:
                     return query(d[m[0]], [(S.MAYBE, *new_m)]+_r)
                 else:
                     return query(d, [(S.MAYBE, *new_m)]+_r)
@@ -187,16 +186,32 @@
         case [(H.MIN,f), *_r] if isinstance(d,list):
             return query(min([ f(_) for _ in d]) , _r) 
         case [H.ORDER, *_r] if isinstance(d,list):
             return query(sorted(d) , _r)
         case [(H.ORDER, f), *_r] if isinstance(d,list):
             _m_list = [f(_) for _ in d]
             return query(sorted(_m_list), _r) 
+        case [H.COUNT, *_r]:
+            return query(len(d), _r) 
         case [_h, *_r] if isinstance(d,dict):
             try:
                 return query(d[_h], _r)
             except KeyError as ke:
                 print(f"{_h} is not in {d}")
             except TypeError as te:
                 print(f"Error->{te}")
                 print(f"navigate to {_h} on {d}, rest path:{_r}")
 
+def queryFile(f, p, debug=False):
+    with open(f,'r') as _f:
+        i = json.load(_f)
+        return query(i, p, debug=debug)
+
+def queryFolder(fp,p,m:str=None):
+    fs = os.listdir(fp)
+    if m is not None:
+        fs = [ _ for _ in fs if re.match(m,_)]
+    fsp = [ (_,os.path.join(fp,_)) for _ in fs]
+    return {fn:queryFile(fp, p) for fn,fp in fsp}
+
+    
+
```

### Comparing `pyspecter-0.1.0/pyspecter.egg-info/PKG-INFO` & `pyspecter-0.1.1/pyspecter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspecter
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library to query nested data in Python
 Home-page: https://github.com/yellowbean/pyspecter
 Author: Xiaoyu Zhang
 Author-email: always.zhang@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -80,14 +80,26 @@
     assert query(m, ["C", (S.FILTER, lambda k, v: k.endswith("2"))]) == [[3, 4]]
 
 Navigate to map which its key or value satisify a custom function 
 
     assert query(m, ["A", (S.MKEY_IF, lambda x:x.endswith("1"))]) == [[10, 20]]
     assert query(m, ["A", (S.MVAL_IF, lambda x:x==[10,20])]) == [[10, 20]]
     
+#### Branching paths
+
+Branching by multiple paths
+
+    mpath = {"A":{"B":1,
+                  "C":[2,3,4,5]}}
+    assert query(mpath,["A",
+                        (S.MULTI_PATH,["B"]
+                                     ,["C", S.LAST])]) == [1,5]
+
+
+
 #### Conditional Navigation
 
 Navigate to a specifie path
 
     assert query(m, ["D", (S.NTH_PATH, 2)]) == [3]
 
 Navigate to a position if and only if the path exists
```

### Comparing `pyspecter-0.1.0/setup.py` & `pyspecter-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyspecter",                     # This is the name of the package
-    version="0.1.0",                        # The initial release version
+    version="0.1.1",                        # The initial release version
     author="Xiaoyu Zhang",                     # Full name of the author
     author_email="always.zhang@gmail.com",
     description="A library to query nested data in Python",
     url="https://github.com/yellowbean/pyspecter",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
```

