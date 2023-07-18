# Comparing `tmp/ojtool-0.1.1.tar.gz` & `tmp/ojtool-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ojtool-0.1.1.tar", last modified: Tue Apr 11 07:20:01 2023, max compression
+gzip compressed data, was "ojtool-0.1.2.tar", last modified: Tue Jul 18 08:57:39 2023, max compression
```

## Comparing `ojtool-0.1.1.tar` & `ojtool-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 jihongwang   (501) staff       (20)        0 2023-04-11 07:20:01.418419 ojtool-0.1.1/
--rw-r--r--   0 jihongwang   (501) staff       (20)     1073 2023-04-10 02:07:11.000000 ojtool-0.1.1/LICENSE
--rw-r--r--   0 jihongwang   (501) staff       (20)      573 2023-04-11 07:20:01.418279 ojtool-0.1.1/PKG-INFO
--rw-r--r--   0 jihongwang   (501) staff       (20)       59 2023-04-10 02:07:11.000000 ojtool-0.1.1/README.md
--rw-r--r--   0 jihongwang   (501) staff       (20)       84 2023-04-10 02:07:11.000000 ojtool-0.1.1/pyproject.toml
--rw-r--r--   0 jihongwang   (501) staff       (20)       38 2023-04-11 07:20:01.418456 ojtool-0.1.1/setup.cfg
--rw-r--r--   0 jihongwang   (501) staff       (20)      812 2023-04-11 07:19:27.000000 ojtool-0.1.1/setup.py
-drwxr-xr-x   0 jihongwang   (501) staff       (20)        0 2023-04-11 07:20:01.411584 ojtool-0.1.1/src/
-drwxr-xr-x   0 jihongwang   (501) staff       (20)        0 2023-04-11 07:20:01.417138 ojtool-0.1.1/src/ojtool/
--rw-r--r--   0 jihongwang   (501) staff       (20)       41 2023-04-10 02:07:11.000000 ojtool-0.1.1/src/ojtool/__init__.py
--rw-r--r--   0 jihongwang   (501) staff       (20)     5060 2023-04-11 07:19:10.000000 ojtool-0.1.1/src/ojtool/ojtool.py
--rw-r--r--   0 jihongwang   (501) staff       (20)      425 2023-04-11 07:19:04.000000 ojtool-0.1.1/src/ojtool/utils.py
-drwxr-xr-x   0 jihongwang   (501) staff       (20)        0 2023-04-11 07:20:01.418065 ojtool-0.1.1/src/ojtool.egg-info/
--rw-r--r--   0 jihongwang   (501) staff       (20)      573 2023-04-11 07:20:01.000000 ojtool-0.1.1/src/ojtool.egg-info/PKG-INFO
--rw-r--r--   0 jihongwang   (501) staff       (20)      241 2023-04-11 07:20:01.000000 ojtool-0.1.1/src/ojtool.egg-info/SOURCES.txt
--rw-r--r--   0 jihongwang   (501) staff       (20)        1 2023-04-11 07:20:01.000000 ojtool-0.1.1/src/ojtool.egg-info/dependency_links.txt
--rw-r--r--   0 jihongwang   (501) staff       (20)        7 2023-04-11 07:20:01.000000 ojtool-0.1.1/src/ojtool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 08:57:39.114693 ojtool-0.1.2/
+-rw-rw-rw-   0        0        0     1091 2023-07-18 07:01:33.000000 ojtool-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      591 2023-07-18 08:57:39.113692 ojtool-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       61 2023-07-18 07:01:33.000000 ojtool-0.1.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-18 07:01:33.000000 ojtool-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 08:57:39.114693 ojtool-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      837 2023-07-18 08:54:47.000000 ojtool-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:57:39.091693 ojtool-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 08:57:39.109693 ojtool-0.1.2/src/ojtool/
+-rw-rw-rw-   0        0        0       42 2023-07-18 07:01:33.000000 ojtool-0.1.2/src/ojtool/__init__.py
+-rw-rw-rw-   0        0        0 13112562 2023-07-18 08:44:35.000000 ojtool-0.1.2/src/ojtool/data.py
+-rw-rw-rw-   0        0        0     5291 2023-07-18 07:19:55.000000 ojtool-0.1.2/src/ojtool/ojtool.py
+-rw-rw-rw-   0        0        0     1062 2023-07-18 08:54:19.000000 ojtool-0.1.2/src/ojtool/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:57:39.112693 ojtool-0.1.2/src/ojtool.egg-info/
+-rw-rw-rw-   0        0        0      591 2023-07-18 08:57:39.000000 ojtool-0.1.2/src/ojtool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-07-18 08:57:39.000000 ojtool-0.1.2/src/ojtool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 08:57:39.000000 ojtool-0.1.2/src/ojtool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-18 08:57:39.000000 ojtool-0.1.2/src/ojtool.egg-info/top_level.txt
```

### Comparing `ojtool-0.1.1/LICENSE` & `ojtool-0.1.2/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright (c) 2018 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `ojtool-0.1.1/PKG-INFO` & `ojtool-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1
-Name: ojtool
-Version: 0.1.1
-Summary: Online Judge Test Data Generator.
-Home-page: https://github.com/ElementCraft/python-ojtool
-Author: elecraft
-Author-email: elecraft@outlook.com
-Project-URL: Bug Tracker, https://github.com/ElementCraft/python-ojtool/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-## ojtool
-
-Online Judge Test Data Generator made by Python.
+Metadata-Version: 2.1
+Name: ojtool
+Version: 0.1.2
+Summary: Online Judge Test Data Generator.
+Home-page: https://github.com/ElementCraft/python-ojtool
+Author: elecraft
+Author-email: elecraft@outlook.com
+Project-URL: Bug Tracker, https://github.com/ElementCraft/python-ojtool/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## ojtool
+
+Online Judge Test Data Generator made by Python.
```

### Comparing `ojtool-0.1.1/setup.py` & `ojtool-0.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import setuptools
-
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="ojtool",
-    version="0.1.1",
-    author="elecraft",
-    author_email="elecraft@outlook.com",
-    description="Online Judge Test Data Generator.",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/ElementCraft/python-ojtool",
-    project_urls={
-        "Bug Tracker": "https://github.com/ElementCraft/python-ojtool/issues",
-    },
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    package_dir={"": "src"},
-    packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.6",
+import setuptools
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="ojtool",
+    version="0.1.2",
+    author="elecraft",
+    author_email="elecraft@outlook.com",
+    description="Online Judge Test Data Generator.",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/ElementCraft/python-ojtool",
+    project_urls={
+        "Bug Tracker": "https://github.com/ElementCraft/python-ojtool/issues",
+    },
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    package_dir={"": "src"},
+    packages=setuptools.find_packages(where="src"),
+    python_requires=">=3.6",
 )
```

### Comparing `ojtool-0.1.1/src/ojtool/ojtool.py` & `ojtool-0.1.2/src/ojtool/ojtool.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,152 +1,154 @@
-import os
-import platform
-import inspect
-import sys
-import zipfile
-import subprocess
-
-class IO:
-    """
-    @author noobug 
-    @desc IO类提供生成数据文件的所有功能
-    """
-
-    def __init__(self, data_count, prefix="", std="std", save_path="tmp/", suffix_in=".in", suffix_out=".out", debug=True):
-        """
-        @data_count 数据点个数，必填！
-        @prefix 生成文件的前缀名，默认空
-        @std 标程名称，windows下会自动带上.exe
-        @save_path 指定生成数据文件存放的路径，必须以/结尾，默认tmp文件夹
-        @suffix_in 指定输入文件的后缀名，默认.in
-        @suffix_out 指定输出文件的后缀名，默认.out
-        @debug 默认开启显示数据生成进度，设置为False关闭
-        """
-        assert data_count > 0
-        self.debug = debug
-        self.IN = []
-        self.OUT = []
-        self.FILES = []
-        self.suffix_in = suffix_in
-        self.suffix_out = suffix_out
-        # self.funclist = [None for _ in range(MAX_DATA_COUNT+5)]
-        self.prefix = prefix
-        self.data_count = data_count
-
-        # 处理保存路径
-        if os.path.isabs(save_path):
-            self.save_path = save_path
-        else:
-            sp = self.getRunningScriptPath()
-            self.save_path = os.path.join(sp, save_path)
-
-        # os.path.abspath(sys.argv[0])
-        if platform.system() == "Windows":
-            if std.endswith(".exe"):
-                self.std = std
-            else:
-                self.std = std + ".exe"
-        else:
-            self.std = std
-
-        # 处理std路径
-        if not os.path.isabs(self.std):
-            sp = self.getRunningScriptPath()
-            self.std = os.path.join(sp, self.std)
-
-    # 获取当前执行文件所在目录
-    def getRunningScriptPath(self):
-        p = os.path.abspath(sys.argv[0])
-        return os.path.split(p)[0]
-
-    def resetIO(self):
-        self.IN = []
-        self.OUT = []
-
-    def write(self, *params, **keys):
-        l = len(self.IN)
-        if l == 0:
-            self.IN.append([])
-        arr = self.IN[-1]
-        arr.extend(params)
-    
-    def writeln(self, *params):
-        l = len(self.IN)
-        if l == 0:
-            self.IN.append([])
-        arr = self.IN[-1]
-        arr.extend(params)
-        self.IN.append([])
-
-    def _writeDataIntoFile(self, fp, data):
-        t = type(data)
-        if t is str:
-            data = data.strip()
-            fp.write(str(data))
-            fp.write(" ")
-        elif t is list or t is tuple:
-            for d in data:
-                self._writeDataIntoFile(fp, d)
-        else:
-            fp.write(str(data))
-            fp.write(" ")
-
-    def _processData(self, func, id, isdefault):
-        self.resetIO()
-        if isdefault:
-            func(id)
-        else:
-            func(id)
-        if not os.path.exists(self.save_path):
-            os.mkdir(self.save_path)
-        fname = f"{self.prefix}{id}{self.suffix_in}"
-        finpath = os.path.join(self.save_path,fname)
-        with open(finpath, "w", encoding="UTF-8") as f:
-            for a in self.IN:
-                self._writeDataIntoFile(f, a)
-                f.write("\n")
-
-        foutname = f"{self.prefix}{id}{self.suffix_out}"
-        foutpath = os.path.join(self.save_path,foutname)
-
-        if platform.system() == "Windows":
-            ret = subprocess.run([self.std, "<", finpath, ">", foutpath], shell=True)
-            if ret.returncode != 0:
-                if self.debug: print(ret)
-        else:
-            os.system(f"\"{self.std}\" < \"{finpath}\" > \"{foutpath}\"")
-        self.FILES.append(finpath)
-        self.FILES.append(foutpath)
-        
-    def done(self, o, zip=False):
-        '''
-        开始根据配置生成数据，需传入一个对象实例。
-        '''
-        if self.debug: print(f"=========OJUtil生成数据==========")
-        for i in range(1, self.data_count+1):
-            if self.debug: print(f">>> 生成第 {i} 个数据点...", end="")
-            fname = f"data_{i}"
-            if hasattr(o, fname):
-                f = getattr(o, fname)
-                if inspect.ismethod(f):
-                    self._processData(f, i, False)
-            else:
-                if hasattr(o, "default"):
-                    f = getattr(o, "default")
-                    if inspect.ismethod(f):
-                        self._processData(f, i, True)
-            if self.debug: print(f"OK. <<<")
-        if self.debug: print(f"=========数据已生成完毕==========")
-
-        if zip:
-            zipname = self.prefix
-            if zipname == None or zipname == "": 
-                zipname = "data.zip"
-            else:
-                zipname += ".zip"
-            zippath = os.path.join(self.save_path, zipname)
-            zz = zipfile.ZipFile(zippath, "w")
-            for x in self.FILES:
-                if os.path.exists(x):
-                    zz.write(x, arcname=os.path.split(x)[1])
-            zz.close()
+import os
+import platform
+import inspect
+import sys
+import zipfile
+import subprocess
+
+class IO:
+    """
+    @author noobug 
+    @desc IO类提供生成数据文件的所有功能
+    """
+
+    def __init__(self, data_count, prefix="", std="std", save_path="tmp/", suffix_in=".in", suffix_out=".out", debug=True):
+        """
+        @data_count 数据点个数，必填！
+        @prefix 生成文件的前缀名，默认空
+        @std 标程名称，windows下会自动带上.exe
+        @save_path 指定生成数据文件存放的路径，必须以/结尾，默认tmp文件夹
+        @suffix_in 指定输入文件的后缀名，默认.in
+        @suffix_out 指定输出文件的后缀名，默认.out
+        @debug 默认开启显示数据生成进度，设置为False关闭
+        """
+        assert data_count > 0
+        self.debug = debug
+        self.IN = []
+        self.OUT = []
+        self.FILES = []
+        self.suffix_in = suffix_in
+        self.suffix_out = suffix_out
+        # self.funclist = [None for _ in range(MAX_DATA_COUNT+5)]
+        self.prefix = prefix
+        self.data_count = data_count
+
+        # 处理保存路径
+        if os.path.isabs(save_path):
+            self.save_path = save_path
+        else:
+            sp = self.getRunningScriptPath()
+            self.save_path = os.path.join(sp, save_path)
+
+        # os.path.abspath(sys.argv[0])
+        if platform.system() == "Windows":
+            if std.endswith(".exe"):
+                self.std = std
+            else:
+                self.std = std + ".exe"
+        else:
+            self.std = std
+
+        # 处理std路径
+        if not os.path.isabs(self.std):
+            sp = self.getRunningScriptPath()
+            self.std = os.path.join(sp, self.std)
+
+    # 获取当前执行文件所在目录
+    def getRunningScriptPath(self):
+        p = os.path.abspath(sys.argv[0])
+        return os.path.split(p)[0]
+
+    def resetIO(self):
+        self.IN = []
+        self.OUT = []
+
+    def write(self, *params, **keys):
+        l = len(self.IN)
+        if l == 0:
+            self.IN.append([])
+        arr = self.IN[-1]
+        arr.extend(params)
+    
+    def writeln(self, *params):
+        l = len(self.IN)
+        if l == 0:
+            self.IN.append([])
+        arr = self.IN[-1]
+        arr.extend(params)
+        self.IN.append([])
+
+    def _writeDataIntoFile(self, fp, data):
+        t = type(data)
+        if t is str:
+            data = data.strip()
+            fp.write(str(data))
+            fp.write(" ")
+        elif t is list or t is tuple:
+            for d in data:
+                self._writeDataIntoFile(fp, d)
+        else:
+            fp.write(str(data))
+            fp.write(" ")
+
+    def _processData(self, func, id, isdefault):
+        self.resetIO()
+        if isdefault:
+            func(id)
+        else:
+            func(id)
+        if not os.path.exists(self.save_path):
+            os.mkdir(self.save_path)
+        fname = f"{self.prefix}{id}{self.suffix_in}"
+        finpath = os.path.join(self.save_path,fname)
+        with open(finpath, "w", encoding="UTF-8") as f:
+            lim = len(self.IN)
+            for i,a in enumerate(self.IN):
+                self._writeDataIntoFile(f, a)
+                if i < lim-1:
+                    f.write("\n")
+
+        foutname = f"{self.prefix}{id}{self.suffix_out}"
+        foutpath = os.path.join(self.save_path,foutname)
+
+        if platform.system() == "Windows":
+            ret = subprocess.run([self.std, "<", finpath, ">", foutpath], shell=True)
+            if ret.returncode != 0:
+                if self.debug: print(ret)
+        else:
+            os.system(f"\"{self.std}\" < \"{finpath}\" > \"{foutpath}\"")
+        self.FILES.append(finpath)
+        self.FILES.append(foutpath)
+        
+    def done(self, o, zip=False):
+        '''
+        开始根据配置生成数据，需传入一个对象实例。
+        '''
+        if self.debug: print(f"=========OJUtil生成数据==========")
+        for i in range(1, self.data_count+1):
+            if self.debug: print(f">>> 生成第 {i} 个数据点...", end="")
+            fname = f"data_{i}"
+            if hasattr(o, fname):
+                f = getattr(o, fname)
+                if inspect.ismethod(f):
+                    self._processData(f, i, False)
+            else:
+                if hasattr(o, "default"):
+                    f = getattr(o, "default")
+                    if inspect.ismethod(f):
+                        self._processData(f, i, True)
+            if self.debug: print(f"OK. <<<")
+        if self.debug: print(f"=========数据已生成完毕==========")
+
+        if zip:
+            zipname = self.prefix
+            if zipname == None or zipname == "": 
+                zipname = "data.zip"
+            else:
+                zipname += ".zip"
+            zippath = os.path.join(self.save_path, zipname)
+            zz = zipfile.ZipFile(zippath, "w")
+            for x in self.FILES:
+                if os.path.exists(x):
+                    zz.write(x, arcname=os.path.split(x)[1])
+            zz.close()
             if self.debug: print(f"=========压缩完毕==========")
```

### Comparing `ojtool-0.1.1/src/ojtool.egg-info/PKG-INFO` & `ojtool-0.1.2/src/ojtool.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1
-Name: ojtool
-Version: 0.1.1
-Summary: Online Judge Test Data Generator.
-Home-page: https://github.com/ElementCraft/python-ojtool
-Author: elecraft
-Author-email: elecraft@outlook.com
-Project-URL: Bug Tracker, https://github.com/ElementCraft/python-ojtool/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-## ojtool
-
-Online Judge Test Data Generator made by Python.
+Metadata-Version: 2.1
+Name: ojtool
+Version: 0.1.2
+Summary: Online Judge Test Data Generator.
+Home-page: https://github.com/ElementCraft/python-ojtool
+Author: elecraft
+Author-email: elecraft@outlook.com
+Project-URL: Bug Tracker, https://github.com/ElementCraft/python-ojtool/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## ojtool
+
+Online Judge Test Data Generator made by Python.
```

