# Comparing `tmp/cudagrad-0.0.19.tar.gz` & `tmp/cudagrad-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cudagrad-0.0.19.tar", last modified: Tue Jul 18 06:14:24 2023, max compression
+gzip compressed data, was "cudagrad-0.0.2.tar", last modified: Sat Jul 15 20:18:47 2023, max compression
```

## Comparing `cudagrad-0.0.19.tar` & `cudagrad-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-18 06:14:24.013570 cudagrad-0.0.19/
--rw-r--r--   0 ryan       (501) staff       (20)       25 2023-07-18 02:40:23.000000 cudagrad-0.0.19/MANIFEST.in
--rw-r--r--   0 ryan       (501) staff       (20)     3615 2023-07-18 06:14:24.013451 cudagrad-0.0.19/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)     3113 2023-07-18 03:03:04.000000 cudagrad-0.0.19/README.md
--rw-r--r--   0 ryan       (501) staff       (20)      724 2023-07-18 06:13:54.000000 cudagrad-0.0.19/pyproject.toml
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-18 06:14:24.013611 cudagrad-0.0.19/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)     1592 2023-07-18 02:40:23.000000 cudagrad-0.0.19/setup.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-18 06:14:24.011984 cudagrad-0.0.19/src/
--rw-r--r--   0 ryan       (501) staff       (20)     3414 2023-07-18 06:13:07.000000 cudagrad-0.0.19/src/bindings.cpp
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-18 06:14:24.013027 cudagrad-0.0.19/src/cudagrad.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)     3615 2023-07-18 06:14:23.000000 cudagrad-0.0.19/src/cudagrad.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      307 2023-07-18 06:14:23.000000 cudagrad-0.0.19/src/cudagrad.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-18 06:14:23.000000 cudagrad-0.0.19/src/cudagrad.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-18 02:46:33.000000 cudagrad-0.0.19/src/cudagrad.egg-info/not-zip-safe
--rw-r--r--   0 ryan       (501) staff       (20)       25 2023-07-18 06:14:23.000000 cudagrad-0.0.19/src/cudagrad.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)        9 2023-07-18 06:14:23.000000 cudagrad-0.0.19/src/cudagrad.egg-info/top_level.txt
--rw-r--r--   0 ryan       (501) staff       (20)    23608 2023-07-18 06:10:12.000000 cudagrad-0.0.19/src/cudagrad.hpp
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-18 06:14:24.013154 cudagrad-0.0.19/tests/
--rw-r--r--   0 ryan       (501) staff       (20)     1046 2023-07-18 02:40:23.000000 cudagrad-0.0.19/tests/test.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-15 20:18:47.828782 cudagrad-0.0.2/
+-rw-r--r--   0 ryan       (501) staff       (20)     3481 2023-07-15 20:18:47.828668 cudagrad-0.0.2/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)     2980 2023-07-15 19:49:48.000000 cudagrad-0.0.2/README.md
+-rw-r--r--   0 ryan       (501) staff       (20)      732 2023-07-15 20:15:50.000000 cudagrad-0.0.2/pyproject.toml
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-15 20:18:47.828816 cudagrad-0.0.2/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)     1285 2023-07-15 20:18:01.000000 cudagrad-0.0.2/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-15 20:18:47.827340 cudagrad-0.0.2/src/
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-15 20:18:47.828213 cudagrad-0.0.2/src/cudagrad.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)     3481 2023-07-15 20:18:47.000000 cudagrad-0.0.2/src/cudagrad.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      274 2023-07-15 20:18:47.000000 cudagrad-0.0.2/src/cudagrad.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-15 20:18:47.000000 cudagrad-0.0.2/src/cudagrad.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-15 20:18:22.000000 cudagrad-0.0.2/src/cudagrad.egg-info/not-zip-safe
+-rw-r--r--   0 ryan       (501) staff       (20)       25 2023-07-15 20:18:47.000000 cudagrad-0.0.2/src/cudagrad.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        9 2023-07-15 20:18:47.000000 cudagrad-0.0.2/src/cudagrad.egg-info/top_level.txt
+-rw-r--r--   0 ryan       (501) staff       (20)      858 2023-07-15 18:31:47.000000 cudagrad-0.0.2/src/main.cpp
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-15 20:18:47.828315 cudagrad-0.0.2/tests/
+-rw-r--r--   0 ryan       (501) staff       (20)      108 2023-07-15 20:14:26.000000 cudagrad-0.0.2/tests/test.py
```

### Comparing `cudagrad-0.0.19/PKG-INFO` & `cudagrad-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,65 @@
 Metadata-Version: 2.1
 Name: cudagrad
-Version: 0.0.19
+Version: 0.0.2
 Summary: A small autograd engine
 Home-page: https://github.com/yrom1/cudagrad
 Author: Ryan Moore
 Author-email: Ryan Moore <moorethreads@hey.com>
 Project-URL: Homepage, https://github.com/yrom1/cudagrad
 Project-URL: Bug Tracker, https://github.com/yrom1/cudagrad/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 
-# cudagrad
+# cudagrad ⚡️
 
-A small autograd engine
-
-![](parallel_1_20.png)
+A small autograd engine, inspired by PyTorch and micrograd
 
 ## Example
 
 ```cpp
-// c++ -std=c++11 -I./src examples/example.cpp && ./a.out
 #include "cudagrad.hpp"
 int main() {
   auto a = cg::tensor({2, 2}, {2.0, 3.0, 4.0, 5.0});
   auto b = cg::tensor({2, 2}, {6.0, 7.0, 8.0, 9.0});
   auto c = cg::tensor({2, 2}, {10.0, 10.0, 10.0, 10.0});
   auto d = cg::tensor({2, 2}, {11.0, 11.0, 11.0, 11.0});
   auto e = (cg::matmul(a, b) + c) * d;
   auto f = e.get()->sum();
   f.get()->backward();
 
-  using namespace std;
-  for (auto& x : f.get()->data_) {cout<<x<<" ";} // 2794
-  for (auto& x : f.get()->size_) {cout<<x<<" ";} // 1
-  for (auto& x : a.get()->grad_) {cout<<x<<" ";} // 143 187 143 187
-  for (auto& x : b.get()->grad_) {cout<<x<<" ";} // 66 66 88 88
+  // (std::vector<float> &) { 2794.00f }
+  f.get()->data_;
+  // (std::vector<float> &) { 143.000f, 187.000f, 143.000f, 187.000f }
+  a.get()->grad_;
+  // (std::vector<float> &) { 66.0000f, 66.0000f, 88.0000f, 88.0000f }
+  b.get()->grad_;
 }
 ```
 
-Available on [PyPI](https://pypi.org/project/cudagrad/), use `pip install cudagrad` to get the Python bindings
-
 ```py
-# pip install cudagrad; py ./examples/example.py
-import cudagrad as cg
-
-a = cg.tensor([2, 2], [2.0, 3.0, 4.0, 5.0])
-b = cg.tensor([2, 2], [6.0, 7.0, 8.0, 9.0])
-c = cg.tensor([2, 2], [10.0, 10.0, 10.0, 10.0])
-d = cg.tensor([2, 2], [11.0, 11.0, 11.0, 11.0])
-e = ((a @ b) + c) * d
-f = e.sum()
-f.backward()
-
-print(f.data) # [2794.0]
-print(f.size) # [1]
-print(a.grad) # [143.0, 187.0, 143.0, 187.0]
-print(b.grad) # [66.0, 66.0, 88.0, 88.0]
+>>> import torch
+>>> a = torch.tensor(((2.0, 3.0), (4.0, 5.0)), requires_grad=True)
+>>> b = torch.tensor(((6.0, 7.0), (8.0, 9.0)), requires_grad=True)
+>>> c = torch.tensor(((10.0, 10.0), (10.0, 10.0)), requires_grad=True)
+>>> d = torch.tensor(((11.0, 11.0), (11.0, 11.0)), requires_grad=True)
+>>> e = (a.matmul(b) + c) * d
+>>> f = e.sum()
+>>> f.backward()
+>>> f
+tensor(2794., grad_fn=<SumBackward0>)
+>>> a.grad
+tensor([[143., 187.],
+        [143., 187.]])
+>>> b.grad
+tensor([[66., 66.],
+        [88., 88.]])
 ```
 
 ## Design
 
 ~~The plan is to be similar to PyTorch's internals, particularily the [Variable/Tensor Merge Proposal](https://github.com/pytorch/pytorch/issues/13638) design.~~ The design is a mix of PyTorch and micrograd, with micrograd like members and PyTorch like backward classes with an `apply()` interface.
 
 For simplicity, many features PyTorch has cudagrad does not, like broadcasting and views. All operations are defined only on `std::shared_ptr<Tensor>`, for now at least.
@@ -80,12 +77,11 @@
 ## Running tests
 
 Taking inspiration from [micrograd's tests](https://github.com/karpathy/micrograd/blob/master/test/test_engine.py), we will use [PyTorch's C++ frontend](https://pytorch.org/cppdocs/frontend.html) for high level sanity checks using GoogleTest.
 
 To run the tests use:
 
 ```sh
-chmod +x manage.sh
-./manage.sh test
+sh test.sh
 ```
 
 Running the tests requires: `cmake`, `make`, `torch` installed (on the version of Python accessed by the `python` command), `git`, and a C++ compiler. Note that these requirements are only for when you need to run the tests, otherwise except the C++ compiler they are not needed.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cudagrad-0.0.19/README.md` & `cudagrad-0.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,50 @@
-# cudagrad
+# cudagrad ⚡️
 
-A small autograd engine
-
-![](parallel_1_20.png)
+A small autograd engine, inspired by PyTorch and micrograd
 
 ## Example
 
 ```cpp
-// c++ -std=c++11 -I./src examples/example.cpp && ./a.out
 #include "cudagrad.hpp"
 int main() {
   auto a = cg::tensor({2, 2}, {2.0, 3.0, 4.0, 5.0});
   auto b = cg::tensor({2, 2}, {6.0, 7.0, 8.0, 9.0});
   auto c = cg::tensor({2, 2}, {10.0, 10.0, 10.0, 10.0});
   auto d = cg::tensor({2, 2}, {11.0, 11.0, 11.0, 11.0});
   auto e = (cg::matmul(a, b) + c) * d;
   auto f = e.get()->sum();
   f.get()->backward();
 
-  using namespace std;
-  for (auto& x : f.get()->data_) {cout<<x<<" ";} // 2794
-  for (auto& x : f.get()->size_) {cout<<x<<" ";} // 1
-  for (auto& x : a.get()->grad_) {cout<<x<<" ";} // 143 187 143 187
-  for (auto& x : b.get()->grad_) {cout<<x<<" ";} // 66 66 88 88
+  // (std::vector<float> &) { 2794.00f }
+  f.get()->data_;
+  // (std::vector<float> &) { 143.000f, 187.000f, 143.000f, 187.000f }
+  a.get()->grad_;
+  // (std::vector<float> &) { 66.0000f, 66.0000f, 88.0000f, 88.0000f }
+  b.get()->grad_;
 }
 ```
 
-Available on [PyPI](https://pypi.org/project/cudagrad/), use `pip install cudagrad` to get the Python bindings
-
 ```py
-# pip install cudagrad; py ./examples/example.py
-import cudagrad as cg
-
-a = cg.tensor([2, 2], [2.0, 3.0, 4.0, 5.0])
-b = cg.tensor([2, 2], [6.0, 7.0, 8.0, 9.0])
-c = cg.tensor([2, 2], [10.0, 10.0, 10.0, 10.0])
-d = cg.tensor([2, 2], [11.0, 11.0, 11.0, 11.0])
-e = ((a @ b) + c) * d
-f = e.sum()
-f.backward()
-
-print(f.data) # [2794.0]
-print(f.size) # [1]
-print(a.grad) # [143.0, 187.0, 143.0, 187.0]
-print(b.grad) # [66.0, 66.0, 88.0, 88.0]
+>>> import torch
+>>> a = torch.tensor(((2.0, 3.0), (4.0, 5.0)), requires_grad=True)
+>>> b = torch.tensor(((6.0, 7.0), (8.0, 9.0)), requires_grad=True)
+>>> c = torch.tensor(((10.0, 10.0), (10.0, 10.0)), requires_grad=True)
+>>> d = torch.tensor(((11.0, 11.0), (11.0, 11.0)), requires_grad=True)
+>>> e = (a.matmul(b) + c) * d
+>>> f = e.sum()
+>>> f.backward()
+>>> f
+tensor(2794., grad_fn=<SumBackward0>)
+>>> a.grad
+tensor([[143., 187.],
+        [143., 187.]])
+>>> b.grad
+tensor([[66., 66.],
+        [88., 88.]])
 ```
 
 ## Design
 
 ~~The plan is to be similar to PyTorch's internals, particularily the [Variable/Tensor Merge Proposal](https://github.com/pytorch/pytorch/issues/13638) design.~~ The design is a mix of PyTorch and micrograd, with micrograd like members and PyTorch like backward classes with an `apply()` interface.
 
 For simplicity, many features PyTorch has cudagrad does not, like broadcasting and views. All operations are defined only on `std::shared_ptr<Tensor>`, for now at least.
@@ -65,12 +62,11 @@
 ## Running tests
 
 Taking inspiration from [micrograd's tests](https://github.com/karpathy/micrograd/blob/master/test/test_engine.py), we will use [PyTorch's C++ frontend](https://pytorch.org/cppdocs/frontend.html) for high level sanity checks using GoogleTest.
 
 To run the tests use:
 
 ```sh
-chmod +x manage.sh
-./manage.sh test
+sh test.sh
 ```
 
 Running the tests requires: `cmake`, `make`, `torch` installed (on the version of Python accessed by the `python` command), `git`, and a C++ compiler. Note that these requirements are only for when you need to run the tests, otherwise except the C++ compiler they are not needed.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cudagrad-0.0.19/setup.py` & `cudagrad-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,25 @@
 # Available at setup time due to pyproject.toml
-
-import toml
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import setup
 
-
-def get_version_from_toml():
-    data = toml.load('pyproject.toml')
-    version = data.get('project', {}).get('version', None)
-    if version is None:
-        raise RuntimeError("Can't get version in TOML!")
-    else:
-        return version
-
-__version__ = get_version_from_toml()
+__version__ = "0.0.2"
 
 # The main interface is through Pybind11Extension.
 # * You can add cxx_std=11/14/17, and then build_ext can be removed.
 # * You can set include_pybind11=false to add the include directory yourself,
 #   say from a submodule.
 #
 # Note:
 #   Sort input source files if you glob sources to ensure bit-for-bit
 #   reproducible builds (https://github.com/pybind/cudagrad/pull/53)
 
 ext_modules = [
     Pybind11Extension("cudagrad",
-        ["src/bindings.cpp"],
+        ["src/main.cpp"],
         # Example: passing in the version to the compiled code
         define_macros = [('VERSION_INFO', __version__)],
         ),
 ]
 
 setup(
     name="cudagrad",
@@ -43,9 +32,8 @@
     ext_modules=ext_modules,
     extras_require={"test": "pytest"},
     # Currently, build_ext only provides an optional "highest supported C++
     # level" feature, but in the future it may provide more features.
     cmdclass={"build_ext": build_ext},
     zip_safe=False,
     python_requires=">=3.7",
-    include_package_data=True,
 )
```

### Comparing `cudagrad-0.0.19/src/cudagrad.egg-info/PKG-INFO` & `cudagrad-0.0.2/src/cudagrad.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,65 @@
 Metadata-Version: 2.1
 Name: cudagrad
-Version: 0.0.19
+Version: 0.0.2
 Summary: A small autograd engine
 Home-page: https://github.com/yrom1/cudagrad
 Author: Ryan Moore
 Author-email: Ryan Moore <moorethreads@hey.com>
 Project-URL: Homepage, https://github.com/yrom1/cudagrad
 Project-URL: Bug Tracker, https://github.com/yrom1/cudagrad/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 
-# cudagrad
+# cudagrad ⚡️
 
-A small autograd engine
-
-![](parallel_1_20.png)
+A small autograd engine, inspired by PyTorch and micrograd
 
 ## Example
 
 ```cpp
-// c++ -std=c++11 -I./src examples/example.cpp && ./a.out
 #include "cudagrad.hpp"
 int main() {
   auto a = cg::tensor({2, 2}, {2.0, 3.0, 4.0, 5.0});
   auto b = cg::tensor({2, 2}, {6.0, 7.0, 8.0, 9.0});
   auto c = cg::tensor({2, 2}, {10.0, 10.0, 10.0, 10.0});
   auto d = cg::tensor({2, 2}, {11.0, 11.0, 11.0, 11.0});
   auto e = (cg::matmul(a, b) + c) * d;
   auto f = e.get()->sum();
   f.get()->backward();
 
-  using namespace std;
-  for (auto& x : f.get()->data_) {cout<<x<<" ";} // 2794
-  for (auto& x : f.get()->size_) {cout<<x<<" ";} // 1
-  for (auto& x : a.get()->grad_) {cout<<x<<" ";} // 143 187 143 187
-  for (auto& x : b.get()->grad_) {cout<<x<<" ";} // 66 66 88 88
+  // (std::vector<float> &) { 2794.00f }
+  f.get()->data_;
+  // (std::vector<float> &) { 143.000f, 187.000f, 143.000f, 187.000f }
+  a.get()->grad_;
+  // (std::vector<float> &) { 66.0000f, 66.0000f, 88.0000f, 88.0000f }
+  b.get()->grad_;
 }
 ```
 
-Available on [PyPI](https://pypi.org/project/cudagrad/), use `pip install cudagrad` to get the Python bindings
-
 ```py
-# pip install cudagrad; py ./examples/example.py
-import cudagrad as cg
-
-a = cg.tensor([2, 2], [2.0, 3.0, 4.0, 5.0])
-b = cg.tensor([2, 2], [6.0, 7.0, 8.0, 9.0])
-c = cg.tensor([2, 2], [10.0, 10.0, 10.0, 10.0])
-d = cg.tensor([2, 2], [11.0, 11.0, 11.0, 11.0])
-e = ((a @ b) + c) * d
-f = e.sum()
-f.backward()
-
-print(f.data) # [2794.0]
-print(f.size) # [1]
-print(a.grad) # [143.0, 187.0, 143.0, 187.0]
-print(b.grad) # [66.0, 66.0, 88.0, 88.0]
+>>> import torch
+>>> a = torch.tensor(((2.0, 3.0), (4.0, 5.0)), requires_grad=True)
+>>> b = torch.tensor(((6.0, 7.0), (8.0, 9.0)), requires_grad=True)
+>>> c = torch.tensor(((10.0, 10.0), (10.0, 10.0)), requires_grad=True)
+>>> d = torch.tensor(((11.0, 11.0), (11.0, 11.0)), requires_grad=True)
+>>> e = (a.matmul(b) + c) * d
+>>> f = e.sum()
+>>> f.backward()
+>>> f
+tensor(2794., grad_fn=<SumBackward0>)
+>>> a.grad
+tensor([[143., 187.],
+        [143., 187.]])
+>>> b.grad
+tensor([[66., 66.],
+        [88., 88.]])
 ```
 
 ## Design
 
 ~~The plan is to be similar to PyTorch's internals, particularily the [Variable/Tensor Merge Proposal](https://github.com/pytorch/pytorch/issues/13638) design.~~ The design is a mix of PyTorch and micrograd, with micrograd like members and PyTorch like backward classes with an `apply()` interface.
 
 For simplicity, many features PyTorch has cudagrad does not, like broadcasting and views. All operations are defined only on `std::shared_ptr<Tensor>`, for now at least.
@@ -80,12 +77,11 @@
 ## Running tests
 
 Taking inspiration from [micrograd's tests](https://github.com/karpathy/micrograd/blob/master/test/test_engine.py), we will use [PyTorch's C++ frontend](https://pytorch.org/cppdocs/frontend.html) for high level sanity checks using GoogleTest.
 
 To run the tests use:
 
 ```sh
-chmod +x manage.sh
-./manage.sh test
+sh test.sh
 ```
 
 Running the tests requires: `cmake`, `make`, `torch` installed (on the version of Python accessed by the `python` command), `git`, and a C++ compiler. Note that these requirements are only for when you need to run the tests, otherwise except the C++ compiler they are not needed.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

