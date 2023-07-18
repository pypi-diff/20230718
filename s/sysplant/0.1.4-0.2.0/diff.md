# Comparing `tmp/sysplant-0.1.4.tar.gz` & `tmp/sysplant-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysplant-0.1.4.tar", max compression
+gzip compressed data, was "sysplant-0.2.0.tar", max compression
```

## Comparing `sysplant-0.1.4.tar` & `sysplant-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     1075 2023-07-17 14:43:14.455687 sysplant-0.1.4/LICENSE
--rw-r--r--   0        0        0     9545 2023-07-17 14:43:14.455687 sysplant-0.1.4/README.md
--rw-r--r--   0        0        0      864 2023-07-17 14:43:14.459687 sysplant-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-17 14:43:14.459687 sysplant-0.1.4/sysplant/__init__.py
--rw-r--r--   0        0        0        0 2023-07-17 14:43:14.459687 sysplant-0.1.4/sysplant/abstracts/__init__.py
--rw-r--r--   0        0        0     3492 2023-07-17 14:43:14.459687 sysplant-0.1.4/sysplant/abstracts/abstractFactory.py
--rw-r--r--   0        0        0     1998 2023-07-17 14:43:14.459687 sysplant-0.1.4/sysplant/abstracts/abstractGenerator.py
--rw-r--r--   0        0        0     3820 2023-07-17 14:43:14.459687 sysplant-0.1.4/sysplant/constants/__init__.py
--rw-r--r--   0        0        0     1981 2023-07-17 14:43:14.459687 sysplant-0.1.4/sysplant/constants/sysplantConstants.py
--rw-r--r--   0        0        0        0 2023-07-17 14:43:14.459687 sysplant-0.1.4/sysplant/data/__init__.py
--rw-r--r--   0        0        0    44046 2023-07-17 14:43:14.459687 sysplant-0.1.4/sysplant/data/definitions.json
--rw-r--r--   0        0        0   332144 2023-07-17 14:43:14.459687 sysplant-0.1.4/sysplant/data/prototypes.json
--rw-r--r--   0        0        0   431123 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/data/windef.nim
--rw-r--r--   0        0        0        0 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/managers/__init__.py
--rw-r--r--   0        0        0    12333 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/managers/nimGenerator.py
--rw-r--r--   0        0        0    12756 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/managers/templateManager.py
--rw-r--r--   0        0        0     6210 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/sysplant.py
--rw-r--r--   0        0        0        0 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/__init__.py
--rw-r--r--   0        0        0     3018 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/base.nim
--rw-r--r--   0        0        0        0 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/iterators/__init__.py
--rw-r--r--   0        0        0     3359 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/iterators/canterlot.nim
--rw-r--r--   0        0        0     2698 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/iterators/freshy.nim
--rw-r--r--   0        0        0     4461 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/iterators/halo.nim
--rw-r--r--   0        0        0     3414 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/iterators/hell.nim
--rw-r--r--   0        0        0     2561 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/iterators/syswhispers.nim
--rw-r--r--   0        0        0     4527 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/iterators/tartarus.nim
--rw-r--r--   0        0        0        0 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/resolvers/__init__.py
--rw-r--r--   0        0        0       99 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/resolvers/basic.nim
--rw-r--r--   0        0        0      229 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/resolvers/random.nim
--rw-r--r--   0        0        0        0 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/stubs/__init__.py
--rw-r--r--   0        0        0      509 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/stubs/direct_x64.nim
--rw-r--r--   0        0        0      568 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/templates/stubs/indirect_x64.nim
--rw-r--r--   0        0        0        0 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/utils/__init__.py
--rw-r--r--   0        0        0     3474 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/utils/loggerSingleton.py
--rw-r--r--   0        0        0      261 2023-07-17 14:43:14.463687 sysplant-0.1.4/sysplant/utils/singleton.py
--rw-r--r--   0        0        0    10082 1970-01-01 00:00:00.000000 sysplant-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35077 2023-07-18 08:07:39.991296 sysplant-0.2.0/LICENSE
+-rw-r--r--   0        0        0     9423 2023-07-18 08:07:39.991296 sysplant-0.2.0/README.md
+-rw-r--r--   0        0        0      886 2023-07-18 08:07:39.995296 sysplant-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-18 08:07:39.995296 sysplant-0.2.0/sysplant/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 08:07:39.995296 sysplant-0.2.0/sysplant/abstracts/__init__.py
+-rw-r--r--   0        0        0     3492 2023-07-18 08:07:39.995296 sysplant-0.2.0/sysplant/abstracts/abstractFactory.py
+-rw-r--r--   0        0        0     1998 2023-07-18 08:07:39.995296 sysplant-0.2.0/sysplant/abstracts/abstractGenerator.py
+-rw-r--r--   0        0        0     3820 2023-07-18 08:07:39.995296 sysplant-0.2.0/sysplant/constants/__init__.py
+-rw-r--r--   0        0        0     1981 2023-07-18 08:07:39.995296 sysplant-0.2.0/sysplant/constants/sysplantConstants.py
+-rw-r--r--   0        0        0        0 2023-07-18 08:07:39.995296 sysplant-0.2.0/sysplant/data/__init__.py
+-rw-r--r--   0        0        0    44046 2023-07-18 08:07:39.995296 sysplant-0.2.0/sysplant/data/definitions.json
+-rw-r--r--   0        0        0   332144 2023-07-18 08:07:39.995296 sysplant-0.2.0/sysplant/data/prototypes.json
+-rw-r--r--   0        0        0   431123 2023-07-18 08:07:39.999296 sysplant-0.2.0/sysplant/data/windef.nim
+-rw-r--r--   0        0        0        0 2023-07-18 08:07:39.999296 sysplant-0.2.0/sysplant/managers/__init__.py
+-rw-r--r--   0        0        0    12333 2023-07-18 08:07:39.999296 sysplant-0.2.0/sysplant/managers/nimGenerator.py
+-rw-r--r--   0        0        0    12756 2023-07-18 08:07:39.999296 sysplant-0.2.0/sysplant/managers/templateManager.py
+-rw-r--r--   0        0        0     6210 2023-07-18 08:07:39.999296 sysplant-0.2.0/sysplant/sysplant.py
+-rw-r--r--   0        0        0        0 2023-07-18 08:07:39.999296 sysplant-0.2.0/sysplant/templates/__init__.py
+-rw-r--r--   0        0        0     3018 2023-07-18 08:07:39.999296 sysplant-0.2.0/sysplant/templates/base.nim
+-rw-r--r--   0        0        0        0 2023-07-18 08:07:39.999296 sysplant-0.2.0/sysplant/templates/iterators/__init__.py
+-rw-r--r--   0        0        0     3359 2023-07-18 08:07:39.999296 sysplant-0.2.0/sysplant/templates/iterators/canterlot.nim
+-rw-r--r--   0        0        0     2698 2023-07-18 08:07:39.999296 sysplant-0.2.0/sysplant/templates/iterators/freshy.nim
+-rw-r--r--   0        0        0     4461 2023-07-18 08:07:39.999296 sysplant-0.2.0/sysplant/templates/iterators/halo.nim
+-rw-r--r--   0        0        0     3414 2023-07-18 08:07:39.999296 sysplant-0.2.0/sysplant/templates/iterators/hell.nim
+-rw-r--r--   0        0        0     2561 2023-07-18 08:07:39.999296 sysplant-0.2.0/sysplant/templates/iterators/syswhispers.nim
+-rw-r--r--   0        0        0     2873 2023-07-18 08:07:39.999296 sysplant-0.2.0/sysplant/templates/iterators/syswhispers3.nim
+-rw-r--r--   0        0        0     4527 2023-07-18 08:07:39.999296 sysplant-0.2.0/sysplant/templates/iterators/tartarus.nim
+-rw-r--r--   0        0        0        0 2023-07-18 08:07:39.999296 sysplant-0.2.0/sysplant/templates/resolvers/__init__.py
+-rw-r--r--   0        0        0       99 2023-07-18 08:07:39.999296 sysplant-0.2.0/sysplant/templates/resolvers/basic.nim
+-rw-r--r--   0        0        0      229 2023-07-18 08:07:39.999296 sysplant-0.2.0/sysplant/templates/resolvers/random.nim
+-rw-r--r--   0        0        0        0 2023-07-18 08:07:39.999296 sysplant-0.2.0/sysplant/templates/stubs/__init__.py
+-rw-r--r--   0        0        0      509 2023-07-18 08:07:39.999296 sysplant-0.2.0/sysplant/templates/stubs/direct_x64.nim
+-rw-r--r--   0        0        0      568 2023-07-18 08:07:39.999296 sysplant-0.2.0/sysplant/templates/stubs/indirect_x64.nim
+-rw-r--r--   0        0        0        0 2023-07-18 08:07:39.999296 sysplant-0.2.0/sysplant/utils/__init__.py
+-rw-r--r--   0        0        0     3474 2023-07-18 08:07:39.999296 sysplant-0.2.0/sysplant/utils/loggerSingleton.py
+-rw-r--r--   0        0        0      261 2023-07-18 08:07:39.999296 sysplant-0.2.0/sysplant/utils/singleton.py
+-rw-r--r--   0        0        0     9960 1970-01-01 00:00:00.000000 sysplant-0.2.0/PKG-INFO
```

### Comparing `sysplant-0.1.4/README.md` & `sysplant-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,24 +12,27 @@
 </p>
 
 [![PyPI version](https://img.shields.io/pypi/v/sysplant.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/sysplant/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/sysplant.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/sysplant/)
 [![Build Status](https://github.com/x42en/sysplant/actions/workflows/build.yml/badge.svg)](https://github.com/x42en/sysplant)
 [![Project Licence](https://img.shields.io/github/license/x42en/sysplant.svg)](https://github.com/x42en/sysplant/blob/main/LICENSE)
 [![PyPI downloads](https://img.shields.io/pypi/dm/sysplant.svg)](https://pypistats.org/packages/sysplant)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/ec4504a242554c748120299cd7a1ea6d)](https://app.codacy.com/gh/x42en/sysplant/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![Code Coverage](https://codecov.io/gh/x42en/sysplant/branch/main/graph/badge.svg)](https://codecov.io/gh/x42en/sysplant)
 [![Code style: Black](https://img.shields.io/badge/code%20style-Black-000000.svg)](https://github.com/psf/black)
 
 
 SysPlant is a small implementation in NIM of the currently known syscall hooking methods. It currently supports following gates:
   - [Hell's Gate](https://github.com/am0nsec/HellsGate) : Lookup syscall by first opcodes
   - [Halos's Gate](https://blog.sektor7.net/#!res/2021/halosgate.md) : Lookup syscall by first opcodes and search nearby if first instruction is a JMP
   - [Tartarus' Gate](https://github.com/trickster0/TartarusGate) : Lookup syscall by first opcodes and search nearby if first or third instruction is a JMP
   - [FreshyCalls](https://github.com/crummie5/FreshyCalls) : Lookup syscall by name (start with Nt and not Ntdll), sort addresses to retrieve syscall number
   - [SysWhispers2](https://github.com/jthuraisamy/SysWhispers2) : Lookup syscall by name (start with Zw), sort addresses to retrieve syscall number
-  - **Canterlot's Gate ! :unicorn: :rainbow:** *(from an initial idea of [MDSEC article](https://www.mdsec.co.uk/2022/04/resolving-system-service-numbers-using-the-exception-directory/)) but who was missing a pony name* : Lookup syscall using Runtime Exception Table (sorted by syscall number) and detect padding to syscall instruction for random jumps.
+  - [SysWhispers3](https://github.com/klezVirus/SysWhispers3) : SysWhispers2 style but introduce direct/indirect/random jump with static offset
+  - **Canterlot's Gate ! :unicorn: :rainbow:** *(from an initial idea of [MDSEC article](https://www.mdsec.co.uk/2022/04/resolving-system-service-numbers-using-the-exception-directory/)) but who was missing a pony name* : Lookup syscall using Runtime Exception Table (sorted by syscall number) and detect offset to syscall instruction for random jumps.
   - **Custom** Allows you to choose a generation method, a syscall resolver (basic / random) and a syscall stub (direct / indirect). **Careful: some combinations means nothing so it won't work (eg: freshy iterator + random resolver + indirect stub => as Freshy return back the syscall stub entry address, your syscall number will be rewrite by a random one)**  
 
 *Note: You can also generate your own combinations using the proper options... But be careful some options might not work or even make sense*
 
 > :warning: **DISCLAIMER**
 > Please only use this tool on systems you have permission to access.
 > Usage is restricted to Pentesting or Education only.
@@ -102,18 +105,18 @@
   -h, --help  show this help message and exit
 ```
 
 #### Generate action
 In order to use the generate action you could check the associated help `./main.py generate -h`
 ```bash
 $ ./main.py generate -h
-usage: main.py generate [-h] [-x86 | -wow | -x64] [-p {all,donut,common} | -f FUNCTIONS] [-x] -o OUTPUT {hell,halo,tartarus,freshy,syswhispers,canterlot,custom} ...
+usage: main.py generate [-h] [-x86 | -wow | -x64] [-p {all,donut,common} | -f FUNCTIONS] [-x] -o OUTPUT {hell,halo,tartarus,freshy,syswhispers,syswhispers3,canterlot,custom} ...
 
 positional arguments:
-  {hell,halo,tartarus,freshy,syswhispers,canterlot,custom}
+  {hell,halo,tartarus,freshy,syswhispers,syswhispers3,canterlot,custom}
 
 optional arguments:
   -h, --help            show this help message and exit
   -x, --scramble        Randomize internal function names to evade static analysis
   -o OUTPUT, --output OUTPUT
                         Output path for NIM generated file
 
@@ -125,29 +128,14 @@
 Syscall options:
   -p {all,donut,common}, --preset {all,donut,common}
                         Preset functions to generate (Default: common)
   -f FUNCTIONS, --functions FUNCTIONS
                         Comma-separated functions
 ```
 
-If you choose the `custom` generation method, some precise options apply:
-```bash
-$ ./main.py generate custom -h
-usage: main.py generate custom [-h] [-i {hell,halo,tartarus,freshy,syswhispers,canterlot}] [-r {basic,random}] [-s {direct,indirect}]
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -i {hell,halo,tartarus,freshy,syswhispers,canterlot}, --iterator {hell,halo,tartarus,freshy,syswhispers,canterlot}
-                        Select syscall iterator (Default: canterlot)
-  -r {basic,random}, --resolver {basic,random}
-                        Select syscall resolver (Default: basic)
-  -s {direct,indirect}, --stub {direct,indirect}
-                        Select syscall stub (Default: indirect)
-```
-
 ## Usage
 Here are some usage examples that will generate common NtFunctions only. This tool is not restricted to them, please **[READ THE DOC](https://x42en.github.io/sysplant/)**
 
 #### Hell's Gate generation
 ```bash
 $ ./main.py generate -o syscall.nim hell
 ```
@@ -168,14 +156,19 @@
 ```
 
 #### Syswhispers2 like generation
 ```bash
 $ ./main.py generate -o syscall.nim syswhispers
 ```
 
+#### Syswhispers3 like generation
+```bash
+$ ./main.py generate -o syscall.nim syswhispers3
+```
+
 #### Canterlot's Gate generation
 ```bash
 $ ./main.py generate -o syscall.nim canterlot
 ```
 
 #### Custom generation
 ```bash
@@ -207,8 +200,8 @@
   - [ ] Add x86 support
   - [ ] Add WoW64 support
   - [ ] Setup C templates
   - [ ] Setup Go templates
   - [ ] Setup Rust? templates
 
 ## License
-This project is licensed under the [MIT License](https://www.tldrlegal.com/license/mit-license), for individuals only. If you want to integrate this work in your commercial project please contact me through `0x42en[at]gmail.com`
+This project is licensed under the [GPLv3 License](https://www.gnu.org/licenses/quick-guide-gplv3.en.html), for individuals only. If you want to integrate this work in your commercial project please contact me through `0x42en[at]gmail.com`
```

### Comparing `sysplant-0.1.4/pyproject.toml` & `sysplant-0.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "sysplant"
-version = "0.1.4"
+version = "0.2.0"
 description = "SysPlant - Your syscall factory"
 authors = ["Ben Mz <x42en@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 mkdocs-awesome-pages-plugin = "^2.9.1"
 lazydocs = "^0.4.8"
 poetry-bumpversion = "^0.3.1"
+pytest-cov = "^4.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [[tool.poetry_bumpversion.replacements]]
```

### Comparing `sysplant-0.1.4/sysplant/abstracts/abstractFactory.py` & `sysplant-0.2.0/sysplant/abstracts/abstractFactory.py`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.4/sysplant/abstracts/abstractGenerator.py` & `sysplant-0.2.0/sysplant/abstracts/abstractGenerator.py`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.4/sysplant/constants/__init__.py` & `sysplant-0.2.0/sysplant/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.4/sysplant/constants/sysplantConstants.py` & `sysplant-0.2.0/sysplant/constants/sysplantConstants.py`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.4/sysplant/data/definitions.json` & `sysplant-0.2.0/sysplant/data/definitions.json`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.4/sysplant/data/prototypes.json` & `sysplant-0.2.0/sysplant/data/prototypes.json`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.4/sysplant/data/windef.nim` & `sysplant-0.2.0/sysplant/data/windef.nim`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.4/sysplant/managers/nimGenerator.py` & `sysplant-0.2.0/sysplant/managers/nimGenerator.py`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.4/sysplant/managers/templateManager.py` & `sysplant-0.2.0/sysplant/managers/templateManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         Returns:
             str: Return the file content (text mode)
         """
         if name is None:
             raise ValueError("Template name can not be null")
 
         # Check only extension dot is set
-        if not name.replace(".", "", 1).replace(f"_{self.__arch}", "", 1).isalpha():
+        if not name.replace(".", "", 1).replace(f"_{self.__arch}", "", 1).isalnum():
             raise ValueError("Invalid template name")
 
         # Adapt module based on what to load
         raw = pkg_resources.open_text(pkg_module, name)
         return raw.read()
 
     def __load_prototypes(self) -> None:
```

### Comparing `sysplant-0.1.4/sysplant/sysplant.py` & `sysplant-0.2.0/sysplant/sysplant.py`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.4/sysplant/templates/base.nim` & `sysplant-0.2.0/sysplant/templates/base.nim`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.4/sysplant/templates/iterators/canterlot.nim` & `sysplant-0.2.0/sysplant/templates/iterators/canterlot.nim`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.4/sysplant/templates/iterators/freshy.nim` & `sysplant-0.2.0/sysplant/templates/iterators/freshy.nim`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.4/sysplant/templates/iterators/halo.nim` & `sysplant-0.2.0/sysplant/templates/iterators/halo.nim`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.4/sysplant/templates/iterators/hell.nim` & `sysplant-0.2.0/sysplant/templates/iterators/hell.nim`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.4/sysplant/templates/iterators/syswhispers.nim` & `sysplant-0.2.0/sysplant/templates/iterators/syswhispers.nim`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.4/sysplant/templates/iterators/tartarus.nim` & `sysplant-0.2.0/sysplant/templates/iterators/tartarus.nim`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.4/sysplant/templates/stubs/indirect_x64.nim` & `sysplant-0.2.0/sysplant/templates/stubs/indirect_x64.nim`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.4/sysplant/utils/loggerSingleton.py` & `sysplant-0.2.0/sysplant/utils/loggerSingleton.py`

 * *Files identical despite different names*

### Comparing `sysplant-0.1.4/PKG-INFO` & `sysplant-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysplant
-Version: 0.1.4
+Version: 0.2.0
 Summary: SysPlant - Your syscall factory
 License: MIT
 Author: Ben Mz
 Author-email: x42en@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -28,24 +28,27 @@
 </p>
 
 [![PyPI version](https://img.shields.io/pypi/v/sysplant.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/sysplant/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/sysplant.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/sysplant/)
 [![Build Status](https://github.com/x42en/sysplant/actions/workflows/build.yml/badge.svg)](https://github.com/x42en/sysplant)
 [![Project Licence](https://img.shields.io/github/license/x42en/sysplant.svg)](https://github.com/x42en/sysplant/blob/main/LICENSE)
 [![PyPI downloads](https://img.shields.io/pypi/dm/sysplant.svg)](https://pypistats.org/packages/sysplant)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/ec4504a242554c748120299cd7a1ea6d)](https://app.codacy.com/gh/x42en/sysplant/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![Code Coverage](https://codecov.io/gh/x42en/sysplant/branch/main/graph/badge.svg)](https://codecov.io/gh/x42en/sysplant)
 [![Code style: Black](https://img.shields.io/badge/code%20style-Black-000000.svg)](https://github.com/psf/black)
 
 
 SysPlant is a small implementation in NIM of the currently known syscall hooking methods. It currently supports following gates:
   - [Hell's Gate](https://github.com/am0nsec/HellsGate) : Lookup syscall by first opcodes
   - [Halos's Gate](https://blog.sektor7.net/#!res/2021/halosgate.md) : Lookup syscall by first opcodes and search nearby if first instruction is a JMP
   - [Tartarus' Gate](https://github.com/trickster0/TartarusGate) : Lookup syscall by first opcodes and search nearby if first or third instruction is a JMP
   - [FreshyCalls](https://github.com/crummie5/FreshyCalls) : Lookup syscall by name (start with Nt and not Ntdll), sort addresses to retrieve syscall number
   - [SysWhispers2](https://github.com/jthuraisamy/SysWhispers2) : Lookup syscall by name (start with Zw), sort addresses to retrieve syscall number
-  - **Canterlot's Gate ! :unicorn: :rainbow:** *(from an initial idea of [MDSEC article](https://www.mdsec.co.uk/2022/04/resolving-system-service-numbers-using-the-exception-directory/)) but who was missing a pony name* : Lookup syscall using Runtime Exception Table (sorted by syscall number) and detect padding to syscall instruction for random jumps.
+  - [SysWhispers3](https://github.com/klezVirus/SysWhispers3) : SysWhispers2 style but introduce direct/indirect/random jump with static offset
+  - **Canterlot's Gate ! :unicorn: :rainbow:** *(from an initial idea of [MDSEC article](https://www.mdsec.co.uk/2022/04/resolving-system-service-numbers-using-the-exception-directory/)) but who was missing a pony name* : Lookup syscall using Runtime Exception Table (sorted by syscall number) and detect offset to syscall instruction for random jumps.
   - **Custom** Allows you to choose a generation method, a syscall resolver (basic / random) and a syscall stub (direct / indirect). **Careful: some combinations means nothing so it won't work (eg: freshy iterator + random resolver + indirect stub => as Freshy return back the syscall stub entry address, your syscall number will be rewrite by a random one)**  
 
 *Note: You can also generate your own combinations using the proper options... But be careful some options might not work or even make sense*
 
 > :warning: **DISCLAIMER**
 > Please only use this tool on systems you have permission to access.
 > Usage is restricted to Pentesting or Education only.
@@ -118,18 +121,18 @@
   -h, --help  show this help message and exit
 ```
 
 #### Generate action
 In order to use the generate action you could check the associated help `./main.py generate -h`
 ```bash
 $ ./main.py generate -h
-usage: main.py generate [-h] [-x86 | -wow | -x64] [-p {all,donut,common} | -f FUNCTIONS] [-x] -o OUTPUT {hell,halo,tartarus,freshy,syswhispers,canterlot,custom} ...
+usage: main.py generate [-h] [-x86 | -wow | -x64] [-p {all,donut,common} | -f FUNCTIONS] [-x] -o OUTPUT {hell,halo,tartarus,freshy,syswhispers,syswhispers3,canterlot,custom} ...
 
 positional arguments:
-  {hell,halo,tartarus,freshy,syswhispers,canterlot,custom}
+  {hell,halo,tartarus,freshy,syswhispers,syswhispers3,canterlot,custom}
 
 optional arguments:
   -h, --help            show this help message and exit
   -x, --scramble        Randomize internal function names to evade static analysis
   -o OUTPUT, --output OUTPUT
                         Output path for NIM generated file
 
@@ -141,29 +144,14 @@
 Syscall options:
   -p {all,donut,common}, --preset {all,donut,common}
                         Preset functions to generate (Default: common)
   -f FUNCTIONS, --functions FUNCTIONS
                         Comma-separated functions
 ```
 
-If you choose the `custom` generation method, some precise options apply:
-```bash
-$ ./main.py generate custom -h
-usage: main.py generate custom [-h] [-i {hell,halo,tartarus,freshy,syswhispers,canterlot}] [-r {basic,random}] [-s {direct,indirect}]
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -i {hell,halo,tartarus,freshy,syswhispers,canterlot}, --iterator {hell,halo,tartarus,freshy,syswhispers,canterlot}
-                        Select syscall iterator (Default: canterlot)
-  -r {basic,random}, --resolver {basic,random}
-                        Select syscall resolver (Default: basic)
-  -s {direct,indirect}, --stub {direct,indirect}
-                        Select syscall stub (Default: indirect)
-```
-
 ## Usage
 Here are some usage examples that will generate common NtFunctions only. This tool is not restricted to them, please **[READ THE DOC](https://x42en.github.io/sysplant/)**
 
 #### Hell's Gate generation
 ```bash
 $ ./main.py generate -o syscall.nim hell
 ```
@@ -184,14 +172,19 @@
 ```
 
 #### Syswhispers2 like generation
 ```bash
 $ ./main.py generate -o syscall.nim syswhispers
 ```
 
+#### Syswhispers3 like generation
+```bash
+$ ./main.py generate -o syscall.nim syswhispers3
+```
+
 #### Canterlot's Gate generation
 ```bash
 $ ./main.py generate -o syscall.nim canterlot
 ```
 
 #### Custom generation
 ```bash
@@ -223,9 +216,9 @@
   - [ ] Add x86 support
   - [ ] Add WoW64 support
   - [ ] Setup C templates
   - [ ] Setup Go templates
   - [ ] Setup Rust? templates
 
 ## License
-This project is licensed under the [MIT License](https://www.tldrlegal.com/license/mit-license), for individuals only. If you want to integrate this work in your commercial project please contact me through `0x42en[at]gmail.com`
+This project is licensed under the [GPLv3 License](https://www.gnu.org/licenses/quick-guide-gplv3.en.html), for individuals only. If you want to integrate this work in your commercial project please contact me through `0x42en[at]gmail.com`
```

