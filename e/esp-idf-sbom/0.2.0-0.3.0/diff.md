# Comparing `tmp/esp-idf-sbom-0.2.0.tar.gz` & `tmp/esp-idf-sbom-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/esp-idf-sbom/esp-idf-sbom/dist/.tmp-jka_u2tl/esp-idf-sbom-0.2.0.tar", last modified: Tue Jun 27 12:01:07 2023, max compression
+gzip compressed data, was "/home/runner/work/esp-idf-sbom/esp-idf-sbom/dist/.tmp-vuqrkyty/esp-idf-sbom-0.3.0.tar", last modified: Tue Jul 18 10:12:11 2023, max compression
```

## Comparing `esp-idf-sbom-0.2.0.tar` & `esp-idf-sbom-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:01:07.000000 esp-idf-sbom-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-06-27 12:00:50.000000 esp-idf-sbom-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-06-27 12:01:07.000000 esp-idf-sbom-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-06-27 12:00:50.000000 esp-idf-sbom-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:01:07.000000 esp-idf-sbom-0.2.0/esp-idf-sbom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:00:50.000000 esp-idf-sbom-0.2.0/esp-idf-sbom/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:01:07.000000 esp-idf-sbom-0.2.0/esp_idf_sbom/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-27 12:00:50.000000 esp-idf-sbom-0.2.0/esp_idf_sbom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-27 12:00:50.000000 esp-idf-sbom-0.2.0/esp_idf_sbom/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:01:07.000000 esp-idf-sbom-0.2.0/esp_idf_sbom/libsbom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:00:50.000000 esp-idf-sbom-0.2.0/esp_idf_sbom/libsbom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-06-27 12:00:50.000000 esp-idf-sbom-0.2.0/esp_idf_sbom/libsbom/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-27 12:00:50.000000 esp-idf-sbom-0.2.0/esp_idf_sbom/libsbom/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-27 12:00:50.000000 esp-idf-sbom-0.2.0/esp_idf_sbom/libsbom/nvd.py
--rw-r--r--   0 runner    (1001) docker     (123)    39587 2023-06-27 12:00:50.000000 esp-idf-sbom-0.2.0/esp_idf_sbom/libsbom/spdx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-27 12:00:50.000000 esp-idf-sbom-0.2.0/esp_idf_sbom/libsbom/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10078 2023-06-27 12:00:50.000000 esp-idf-sbom-0.2.0/esp_idf_sbom/sbom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:01:07.000000 esp-idf-sbom-0.2.0/esp_idf_sbom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-06-27 12:01:07.000000 esp-idf-sbom-0.2.0/esp_idf_sbom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-27 12:01:07.000000 esp-idf-sbom-0.2.0/esp_idf_sbom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 12:01:07.000000 esp-idf-sbom-0.2.0/esp_idf_sbom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-27 12:01:07.000000 esp-idf-sbom-0.2.0/esp_idf_sbom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-27 12:01:07.000000 esp-idf-sbom-0.2.0/esp_idf_sbom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-27 12:01:07.000000 esp-idf-sbom-0.2.0/esp_idf_sbom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 12:01:07.000000 esp-idf-sbom-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-27 12:00:50.000000 esp-idf-sbom-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:12:11.000000 esp-idf-sbom-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-07-18 10:11:53.000000 esp-idf-sbom-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12668 2023-07-18 10:12:11.000000 esp-idf-sbom-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-07-18 10:11:53.000000 esp-idf-sbom-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:12:11.000000 esp-idf-sbom-0.3.0/esp-idf-sbom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 10:11:53.000000 esp-idf-sbom-0.3.0/esp-idf-sbom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:12:11.000000 esp-idf-sbom-0.3.0/esp_idf_sbom/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-18 10:11:53.000000 esp-idf-sbom-0.3.0/esp_idf_sbom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-18 10:11:53.000000 esp-idf-sbom-0.3.0/esp_idf_sbom/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:12:11.000000 esp-idf-sbom-0.3.0/esp_idf_sbom/libsbom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 10:11:53.000000 esp-idf-sbom-0.3.0/esp_idf_sbom/libsbom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-07-18 10:11:53.000000 esp-idf-sbom-0.3.0/esp_idf_sbom/libsbom/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-07-18 10:11:53.000000 esp-idf-sbom-0.3.0/esp_idf_sbom/libsbom/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-18 10:11:53.000000 esp-idf-sbom-0.3.0/esp_idf_sbom/libsbom/nvd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48388 2023-07-18 10:11:53.000000 esp-idf-sbom-0.3.0/esp_idf_sbom/libsbom/spdx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-18 10:11:53.000000 esp-idf-sbom-0.3.0/esp_idf_sbom/libsbom/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10528 2023-07-18 10:11:53.000000 esp-idf-sbom-0.3.0/esp_idf_sbom/sbom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:12:11.000000 esp-idf-sbom-0.3.0/esp_idf_sbom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12668 2023-07-18 10:12:11.000000 esp-idf-sbom-0.3.0/esp_idf_sbom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-18 10:12:11.000000 esp-idf-sbom-0.3.0/esp_idf_sbom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 10:12:11.000000 esp-idf-sbom-0.3.0/esp_idf_sbom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-18 10:12:11.000000 esp-idf-sbom-0.3.0/esp_idf_sbom.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-18 10:12:11.000000 esp-idf-sbom-0.3.0/esp_idf_sbom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-18 10:12:11.000000 esp-idf-sbom-0.3.0/esp_idf_sbom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 10:12:11.000000 esp-idf-sbom-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-18 10:11:53.000000 esp-idf-sbom-0.3.0/setup.py
```

### Comparing `esp-idf-sbom-0.2.0/LICENSE` & `esp-idf-sbom-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esp-idf-sbom-0.2.0/PKG-INFO` & `esp-idf-sbom-0.3.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,49 @@
-Metadata-Version: 2.1
-Name: esp-idf-sbom
-Version: 0.2.0
-Summary: SPDX SBOM generator for ESP-IDF projects
-Home-page: https://github.com/espressif/esp-idf-sbom
-Author: Espressif Systems
-Author-email: 
-Keywords: espressif,embedded,spdx,sbom
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Environment :: Console
-Classifier: Topic :: Software Development :: Embedded Systems
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ESP-IDF SBOM Tool (**esp-idf-sbom**)
 
 > :warning: **This is experimental implementation, which is subject to change without prior
 > notice and no backward compatibility is guaranteed.**
 
 The esp-idf-sbom tool creates [Software bill of materials][1] (SBOM)
 files in the [Software Package Data Exchange][2] (SPDX) format for applications
 generated by the [Espressif IoT Development Framework][3] (ESP-IDF).
 It also allows to check generated SBOM files for know vulnerabilities against
 the [National Vulnerability Database][4] (NVD) based on the
 [Common Platform Enumeration][5] (CPE) provided in the SBOM.
 
+## Required ESP-IDF versions
+
+All release branches of currently supported ESP-IDF versions allow to
+generate the SBOM file.
+
+| ESP-IDF version | branch with SBOM support  | commits
+|-----------------|---------------------------|----------------------------------------------------------------------------------------------------------------------------------|
+| 4.3             | release/v4.3              | [befb32b45bc9314b48c29624f9a2c2ef30e34260](https://github.com/espressif/esp-idf/commit/befb32b45bc9314b48c29624f9a2c2ef30e34260) |
+|                 |                           | [f1eef50947ab5770ae4d904c07615e7acab06002](https://github.com/espressif/esp-idf/commit/f1eef50947ab5770ae4d904c07615e7acab06002) |
+| 4.4             | release/v4.4              | [ee505a996045c3657711c3d70c58af8dd48b1426](https://github.com/espressif/esp-idf/commit/ee505a996045c3657711c3d70c58af8dd48b1426) |
+|                 |                           | [53f271ce108d6fa99cf92d59fe9b9dcc4b8fb45b](https://github.com/espressif/esp-idf/commit/53f271ce108d6fa99cf92d59fe9b9dcc4b8fb45b) |
+| 5.0             | release/v5.0              | [30735b33efabd6cf038bcb258b674cf828ad5ecf](https://github.com/espressif/esp-idf/commit/30735b33efabd6cf038bcb258b674cf828ad5ecf) |
+|                 |                           | [9156bbb55c920d6704329975311c331b931ed6bc](https://github.com/espressif/esp-idf/commit/9156bbb55c920d6704329975311c331b931ed6bc) |
+| 5.1             | release/v5.1              | [0f781c718c8548cd2b0e41a30e1814f1c6ed93a2](https://github.com/espressif/esp-idf/commit/0f781c718c8548cd2b0e41a30e1814f1c6ed93a2) |
+|                 |                           | [03162bb276d4155760e8aa839020f0587f5ef599](https://github.com/espressif/esp-idf/commit/03162bb276d4155760e8aa839020f0587f5ef599) |
+| latest          | master                    |                                                                                                                                  |
+
+Older versions, e.g. `v5.0.2`, do not have the required code merged and the following error
+message will be printed.
+
+    E: Project description file "build/project_description.json" does not support SBOM generation. Please see the list of IDF versions required by esp-idf-sbom.
+
+If you see this error message and want to try `esp-idf-sbom`, you can
+
+1. switch to the release branch for version you are using. For example `release/v5.0` if you are using `v5.0.2`.
+2. use future ESP-IDF versions to experiment with esp-idf-sbom.
+3. use `git-cherry-pick` and apply commits for your release from the table above. For example for `v5.0.2` use
+
+    $ git cherry-pick 30735b33efabd6cf038bcb258b674cf828ad5ecf 9156bbb55c920d6704329975311c331b931ed6bc
+
 
 ## SPDX SBOM layout
 
 The SBOM file is created based on application sources, build artefacts, information
 provided by the ESP-IDF build system and SBOM manifest files. The resulting SBOM
 file contains SPDX packages for the final **project** application, used **toolchain**,
 **components** used during build and git **submodules**. Packages are linked
@@ -76,14 +80,17 @@
     Package originator. If the package comes from another person or organization
     that has been identified as a supplier. For example if a component is based
     on 3rd party code with some modifications, the originator is the 3rd party code
     author, but the supplier is the person or organization distributing the final
     component. For more detailed information please see the SPDX specification.
     As for supplier, *Person:* or *Organization:* prefix should be used for
     originator value.
+* **license**:
+    License expression explicitly declared by the author.
+
 
 Example of the `sbom.yml` manifest file for the ESP-IDF blink example.
 
 ```
 version: 0.1.0
 description: Blink application example
 url: https://blink.org/blink-0.1.0.tar.gz # non-existing package download URL example
@@ -97,32 +104,44 @@
 ```
 version: 0.1.0
 description: Main component for blink application
 repository: https://github.com/espressif/esp-idf.git@dc016f59877d13e6e7d4fc193aa5aa764547f16d#examples/get-started/blink
 supplier: 'Organization: Espressif Systems (Shanghai) CO LTD'
 ```
 
-Information from the `sbom.yml` file are mapped to the following SPDX tags.
+Information from the `sbom.yml` manifest file are mapped to the following SPDX tags.
 
 | manifest     | SPDX                         |
 |--------------|------------------------------|
 | version      | PackageVersion               |
 | description  | PackageSummary               |
 | repository   | ExternalRef OTHER repository |
 | url          | PackageDownloadLocation      |
 | cpe          | ExternalRef cpe23Type        |
 | supplier     | PackageSupplier              |
 | originator   | PackageOriginator            |
+| license      | PackageLicenseDeclared       |
 
 Even though the `sbom.yml` file is the primary source of information, the esp-idf-sbom tool
-is also looking at other places if it's not present. The version, description and url
-information from the `idf_component.yml` manifest file is used for components managed by
-the component manager. Component version may be guessed based on git-describe and Espressif
+is also looking at other places if it's not present. The version, description, maintainers and
+url information from the `idf_component.yml` manifest file is used for components managed by
+the component manager.
+
+Information from the `idf_component.yml` manifest file are mapped to the following SPDX tags.
+
+| manifest     | SPDX                         |
+|--------------|------------------------------|
+| version      | PackageVersion               |
+| description  | PackageSummary               |
+| maintainers  | PackageSupplier              |
+| url          | PackageDownloadLocation      |
+
+Component version may be guessed based on git-describe and Espressif
 as a default supplier may be guessed based on git repository or package URL. The guessing
-may be dissabled by using the '--no-guess' option. For submodules, the .gitmodules file is
+may be disabled by using the '--no-guess' option. For submodules, the .gitmodules file is
 also checked for additional submodule information.
 
 
 ## Installation
 
 Currently esp-idf-sbom is not integrated into ESP-IDF and needs to by installed
 separately from Python Package Index (PyPI) with
@@ -155,26 +174,43 @@
 Vulnerabilities are checked based on the [Common Platform Enumeration][5] (CPE) information
 included in the SBOM file for SPDX packages. While checking for vulnerabilities, only packages
 with direct or indirect relationship to the **project** package are examined. For example if mbedtls
 component is compiled, due to component dependecies, but it's actually not linked into the
 final binary, it will be by default presented in the SBOM file, but it will not be reachable
 from the root **project** package and hence it will not be checked for vulnerabilities.
 The reason for this is to avoid possible false possitives, because such packages
-have no direct impact on the resulting application. This can be changed with the `--all`
+have no direct impact on the resulting application. This can be changed with the `--check-all-packages`
 option. If used, all packages in the SBOM file will be checked for possible vulnerabilities
 regardless their relationships to the application binary.
 
 SBOM file generated by the esp-idf-sbom tool can be checked for known vulnerabilities
 with
 
     esp-idf-sbom check [SBOM file]
 
 If *SBOM file* is not provided, the stardard input stream is used.
 
 
+## Licenses and Copyrights
+
+All **component** and **submodule** files are scanned for the `SPDX-License-Identifier`,
+`SPDX-FileCopyrightText` and `SPDX-FileContributor` SPDX file tags. Information from
+these tags is used in the generated SBOM file to specify licenses and copyrights for
+SPDX packages which represent **project**, **component** or **submodule**. The project's
+final license expression is a logical AND of all licenses concluded from **components**
+and **submodules** used in the final project binary.
+
+The license can be also explicitly declared by the author in the `sbom.yml` file with the `license`
+variable. This information is used as a value for the `PackageLicenseDeclared` SPDX tag for
+given **project**, **component** or **submodule**.
+
+The `--no-file-tags` option disables scanning for SPDX file tags. When used the license and
+copyright information from files will not be presented in the generated SBOM file.
+
+
 ## Usage example
 
 This is an example of basic usage for the blink project, which is part of the ESP-IDF. The
 two `sbom.yml` files for project and main component showed above were added. It's expected
 that ESP-IDF is installed and set.
 
 ```
```

### Comparing `esp-idf-sbom-0.2.0/esp_idf_sbom/libsbom/git.py` & `esp-idf-sbom-0.3.0/esp_idf_sbom/libsbom/git.py`

 * *Files identical despite different names*

### Comparing `esp-idf-sbom-0.2.0/esp_idf_sbom/libsbom/log.py` & `esp-idf-sbom-0.3.0/esp_idf_sbom/libsbom/log.py`

 * *Files identical despite different names*

### Comparing `esp-idf-sbom-0.2.0/esp_idf_sbom/libsbom/nvd.py` & `esp-idf-sbom-0.3.0/esp_idf_sbom/libsbom/nvd.py`

 * *Files identical despite different names*

### Comparing `esp-idf-sbom-0.2.0/esp_idf_sbom/libsbom/spdx.py` & `esp-idf-sbom-0.3.0/esp_idf_sbom/libsbom/spdx.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,24 +10,130 @@
 import hashlib
 import json
 import os
 import re
 import sys
 import uuid
 from argparse import Namespace
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Set
 
 import schema
 import yaml
+from license_expression import ExpressionError, get_spdx_licensing
 
 from esp_idf_sbom import __version__
 from esp_idf_sbom.libsbom import git, log, utils
 
 
-class SPDXObject(object):
+class SPDXTags:
+    """Base class representing SPDX tags found in files."""
+    # SPDX file tags
+    SPDX_LICENSE_RE = re.compile(r'SPDX-License-Identifier: *(.*)')
+    SPDX_COPYRIGHT_RE = re.compile(r'SPDX-FileCopyrightText: *(.*)')
+    SPDX_CONTRIBUTOR_RE = re.compile(r'SPDX-FileContributor: *(.*)')
+    # SPDX license parser/validator
+    licensing = get_spdx_licensing()
+
+    def __init__(self) -> None:
+        self.licenses: Set[str] = set()
+        self.licenses_expressions: Set[str] = set()
+        self.copyrights: Set[str] = set()
+        self.contributors: Set[str] = set()
+
+    def get_license_concluded(self) -> str:
+        # SPDX-specification-2-2 Appendix IV: SPDX License Expressions
+        # Composite License Expressions
+        #   4) Order of Precedence and Parentheses
+        #   +, WITH, AND, OR  (OR has lowest precedence)
+        # Use parentheses around each found license expression to make
+        # sure the concluded license is correct.
+        # Use parentheses around each found license expression to make
+        # sure the concluded license is correct.
+
+        exprs = [f'({expr})' for expr in self.licenses_expressions]
+        expr = ' AND '.join(exprs)
+        parsed = self.licensing.parse(expr)
+        return str(parsed.simplify())
+
+    def __ior__(self, other):
+        # Tags unification.
+        self.licenses_expressions |= other.licenses_expressions
+        self.licenses |= other.licenses
+        self.copyrights |= other.copyrights
+        self.contributors |= other.contributors
+        return self
+
+
+class SPDXFileTags(SPDXTags):
+    """SPDX file tags found in single file."""
+    def __init__(self, file: str) -> None:
+        super().__init__()
+        self.path = file
+
+        with open(file) as f:
+            # check only first 10 lines
+            for i in range(1, 10):
+                try:
+                    line = f.readline()
+                except UnicodeDecodeError:
+                    # ignore decode errors, the file may be some binary file
+                    continue
+                match = self.SPDX_COPYRIGHT_RE.search(line)
+                if match:
+                    self.copyrights.add(match.group(1))
+                    continue
+                match = self.SPDX_CONTRIBUTOR_RE.search(line)
+                if match:
+                    self.contributors.add(match.group(1))
+                    continue
+                match = self.SPDX_LICENSE_RE.search(line)
+                if match:
+                    expr = match.group(1)
+                    try:
+                        parsed = self.licensing.parse(expr, validate=True)
+                    except ExpressionError as e:
+                        log.err.warn(f'License expression "{expr}" found in "{self.path}" is not valid: {e}')
+                        parsed = self.licensing.parse(expr)
+                    self.licenses_expressions.add(expr)
+                    for lic in parsed.objects:
+                        self.licenses.add(lic)
+
+
+class SPDXFilesTags(SPDXTags):
+    """Unified SPDX file tags for list of files."""
+    def __init__(self, files: List[str]) -> None:
+        super().__init__()
+        self.files = files
+        for file in files:
+            self |= SPDXFileTags(file)
+
+
+class SPDXFileObjsTags(SPDXTags):
+    """Unified SPDX file tags collected from already created SPDXFile objects."""
+    def __init__(self, files: List['SPDXFile']) -> None:
+        super().__init__()
+        self.files = files
+        for file in files:
+            self |= file.tags
+
+
+class SPDXDirTags(SPDXTags):
+    """Unified SPDX file tags found in the whole directory, except file in exclude_dirs."""
+    def __init__(self, path: str, exclude_dirs: Optional[List[str]]=None) -> None:
+        super().__init__()
+        self.path = path
+
+        for root, dirs, files in os.walk(path):
+            if exclude_dirs and root in exclude_dirs:
+                continue
+            for fn in files:
+                self |= SPDXFileTags(utils.pjoin(root, fn))
+
+
+class SPDXObject:
     """Base class for all SPDX objects, which contains some common methods and helpers.
     It stores the tag/value SPDX data in a simple dictionary, where tag is a key
     and value is stored in a list of values for given tag.
     self[tag]  = [value, ...] # assign new list of value(s) to tag
     self[tag] += [value, ...] # add value(s) to existing tag
     """
     # SPDXID tag value has an requirement that it should contain
@@ -35,25 +141,27 @@
     # to create valid SPDXID value.
     SPDXID_RE = re.compile(r'[^0-9a-zA-Z\.\-\+]')
     SPDX_TAGS = ['SPDXVersion', 'DataLicense', 'SPDXID', 'DocumentName', 'DocumentNamespace',
                  'Creator', 'Created', 'CreatorComment', 'Relationship', 'PackageName', 'PackageSummary',
                  'PackageVersion', 'PackageSupplier', 'PackageOriginator', 'PackageDownloadLocation', 'FilesAnalyzed',
                  'PackageVerificationCode', 'PackageLicenseInfoFromFiles', 'PackageLicenseConcluded',
                  'PackageLicenseDeclared', 'PackageCopyrightText', 'PackageComment', 'FileName',
-                 'LicenseInfoInFile', 'FileCopyrightText', 'FileChecksum', 'ExternalRef', 'LicenseConcluded']
+                 'LicenseInfoInFile', 'FileCopyrightText', 'FileChecksum', 'ExternalRef', 'LicenseConcluded',
+                 'FileContributor']
     # Used to automatically identify Espressif as supplier if package URL or
     # git repository matches.
     ESPRESSIF_RE = re.compile(r'^(\w+://)?(\w+@)?(gitlab\.espressif\.|github.com[:/]espressif/).*')
     # Supplier tag value for Espressif.
     ESPRESSIF_SUPPLIER = 'Organization: Espressif Systems (Shanghai) CO LTD'
 
     def __init__(self, args: Namespace, proj_desc: Dict[str, Any]) -> None:
         self.args = args
         self.proj_desc = proj_desc
         self.spdx: Dict[str, List[str]] = {}
+        self.tags = SPDXTags()
 
     def dump(self, colors=False) -> str:
         """Return SPDX tag/value string representing the SPDX object."""
         out = log.LogString(colors=colors)
         out += ''
         for tag, value in self.spdx.items():
             for v in value:
@@ -84,16 +192,18 @@
     def get_verification_code(self, sha1s: list) -> str:
         """Calculate package verification code from file SHA1 values"""
         sha1s_joined = ''.join(sorted(sha1s))
         return hashlib.sha1(sha1s_joined.encode()).hexdigest()
 
     def hash_file(self, fn: str, alg: str='sha1') -> str:
         """Hash file with requested algorithm"""
+        h = hashlib.new(alg)
         with open(fn, 'rb') as f:
-            return hashlib.file_digest(f, alg).hexdigest()  # type: ignore
+            h.update(f.read())
+            return h.hexdigest()
 
     def get_files(self, path: str, prefix: str, exclude_dirs: Optional[List[str]]=None) -> List['SPDXFile']:
         """Return list of SPDXFile objects for files found in path.
 
         :param path: path to recursively traverse
         :param prefix: prefix to use in SPDXID for files to avoid possible SPDXID collisions
         :param exclude_dirs: list sub-dirs to skip
@@ -176,43 +286,51 @@
         if (self.is_espressif_url(url) or
                 self.is_espressif_url(repo) or
                 self.is_espressif_path(path)):
             return self.ESPRESSIF_SUPPLIER
         else:
             return ''
 
+    def check_person_organization(self, s: str) -> bool:
+        if s.startswith('Person: ') or s.startswith('Organization: '):
+            return True
+        raise schema.SchemaError((f'Value "{s}" must have "Person: " or "Organization: " prefix.'))
+
+    def check_url(self, url: str) -> bool:
+        if utils.is_remote_url(url):
+            return True
+        raise schema.SchemaError((f'Value {url} must have "git", "http" or "https" scheme and domain.'))
+
+    def check_cpe(self, cpe: str) -> bool:
+        # Note: WFN, well-formed CPE name, attributes rules are stricter
+        if re.match(r'^cpe:2\.3:[aho](?::\S+){10}', cpe):
+            return True
+        raise schema.SchemaError((f'Value "{cpe}" does not seem to be well-formed CPE name (WFN)'))
+
+    def check_license(self, lic: str) -> bool:
+        try:
+            self.tags.licensing.parse(lic, validate=True)
+        except ExpressionError as e:
+            raise schema.SchemaError((f'License expression "{lic}" is not valid: {e}'))
+        return True
+
     def get_manifest(self, directory: str) -> Dict[str,str]:
         """Return manifest information found in given directory."""
         def validate_sbom_manifest(manifest: Dict[str,str]) -> None:
-            def check_person_organization(s: str) -> bool:
-                if s.startswith('Person: ') or s.startswith('Organization: '):
-                    return True
-                raise schema.SchemaError((f'Value "{s}" must have "Person: " or "Organization: " prefix.'))
-
-            def check_url(url: str) -> bool:
-                if utils.is_remote_url(url):
-                    return True
-                raise schema.SchemaError((f'Value {url} must have "git", "http" or "https" scheme and domain.'))
-
-            def check_cpe(cpe: str):
-                # Note: WFN, well-formed CPE name, attributes rules are stricter
-                if re.match(r'^cpe:2\.3:[aho](?::\S+){10}', cpe):
-                    return True
-                raise schema.SchemaError((f'Value "{cpe}" does not seem to be well-formed CPE name (WFN)'))
-
             try:
                 sbom_schema = schema.Schema(
                     {
                         schema.Optional('version'): str,
-                        schema.Optional('repository'): schema.And(str, check_url),
-                        schema.Optional('url'): schema.And(str, check_url),
-                        schema.Optional('cpe'): schema.And(str, check_cpe),
-                        schema.Optional('supplier'): schema.And(str, check_person_organization),
-                        schema.Optional('originator'): schema.And(str, check_person_organization),
+                        schema.Optional('repository'): schema.And(str, self.check_url),
+                        schema.Optional('url'): schema.And(str, self.check_url),
+                        schema.Optional('cpe'): schema.And(str, self.check_cpe),
+                        schema.Optional('supplier'): schema.And(str, self.check_person_organization),
+                        schema.Optional('originator'): schema.And(str, self.check_person_organization),
                         schema.Optional('description'): str,
+                        schema.Optional('license'): schema.And(str, self.check_license),
                     })
 
                 sbom_schema.validate(manifest)
             except schema.SchemaError as e:
                 log.err.die(f'The sbom.yml manifest file in "{directory}" is not valid: {e}')
 
         def load(fn: str) -> Dict[str,str]:
@@ -239,14 +357,15 @@
             'version': '',
             'repository': '',
             'url': '',
             'cpe': '',
             'supplier': '',
             'originator': '',
             'description': '',
+            'license': '',
         }
 
         sbom_yml = load('sbom.yml')
         validate_sbom_manifest(sbom_yml)
         update(manifest, sbom_yml)
         idf_component_yml = load('idf_component.yml')
         update(manifest, idf_component_yml)
@@ -315,15 +434,15 @@
             with open(proj_desc_path, 'r') as f:
                 proj_desc = json.load(f)
         except (OSError, ValueError) as e:
             log.err.die(f'cannot read project description file: {e}')
 
         if 'version' not in proj_desc:
             log.err.die((f'Project description file "{proj_desc_path}" does not support SBOM generation. '
-                         f'Please see the list of IDF versions supported by esp-idf-sbom.'))
+                         f'Please see the list of IDF versions required by esp-idf-sbom.'))
 
         return proj_desc  # type: ignore
 
     def dump(self, colors=False) -> str:
         out = log.LogString(colors=colors)
         header = ' '.join('\"' + arg + '\"' if ' ' in arg else arg for arg in sys.argv)
         out.set_color(out.BLUE)
@@ -379,57 +498,65 @@
         self.toolchain = SPDXToolchain(self.args, self.proj_desc)
         self.file = None
 
         if self.include_files():
             fn = utils.pjoin(self.proj_desc['build_dir'], self.proj_desc['app_bin'])
             self.file = SPDXFile(self.args, self.proj_desc, fn, self.proj_desc['build_dir'], self.name)
 
+        self._add_spdx_file_tags()
+
         self['PackageName'] = [self.name]
         if self.manifest['description']:
             self['PackageSummary'] = [f'<text>{self.manifest["description"]}</text>']
         self['SPDXID'] = ['SPDXRef-PROJECT-' + self.sanitize_spdxid(self.name)]
         self['PackageVersion'] = [self.version]
         self['PackageSupplier'] = [self.manifest['supplier'] or 'NOASSERTION']
         self['PackageDownloadLocation'] = [self.manifest['url'] or 'NOASSERTION']
         if self.file:
             self['FilesAnalyzed'] = ['true']
             self['PackageVerificationCode'] = [self.get_verification_code([self.file.sha1])]
-            self['PackageLicenseInfoFromFiles'] = ['NOASSERTION']
+            self['PackageLicenseInfoFromFiles'] = list(self.tags.licenses)
         else:
             self['FilesAnalyzed'] = ['false']
-        self['PackageLicenseConcluded'] = ['NOASSERTION']
-        self['PackageLicenseDeclared'] = ['NOASSERTION']
-        self['PackageCopyrightText'] = ['NOASSERTION']
+        if self.tags.licenses_expressions:
+            self['PackageLicenseConcluded'] = [self.tags.get_license_concluded()]
+        else:
+            self['PackageLicenseConcluded'] = ['NOASSERTION']
+        self['PackageLicenseDeclared'] = [self.manifest['license'] or 'NOASSERTION']
+        if self.tags.copyrights:
+            self['PackageCopyrightText'] = ['<text>{}</text>'.format('\n'.join(self.tags.copyrights))]
+        else:
+            self['PackageCopyrightText'] = ['NOASSERTION']
 
         self._add_relationships()
 
     def _get_manifest(self) -> Dict[str, str]:
         # Get manifest information and try to fill in missing pieces.
         manifest = self.get_manifest(self.proj_desc['project_path'])
         if not manifest['version']:
             manifest['version'] = self.proj_desc['project_version']
 
         return manifest
 
     def _remove_components(self, remove: List[str],
-                           components: Dict[str, 'SPDXComponent']) -> Dict[str, 'SPDXComponent']:
+                           components: Dict[str, Dict]) -> Dict[str, Dict]:
         # Helper to remove components and dependencies on them from component list.
-        def remove_from_reqs(req_type: str, info: SPDXComponent):
+        def remove_from_reqs(req_type: str, info: Dict):
             info[req_type] = list(set(info[req_type]) - set(remove))
 
         for comp in remove:
             del components[comp]
 
         for name, info in components.items():
             for req_type in ['reqs', 'priv_reqs', 'managed_reqs', 'managed_priv_reqs']:
                 remove_from_reqs(req_type, info)
 
         return components
 
-    def _remove_config_only(self, components: Dict[str, 'SPDXComponent']) -> Dict[str, 'SPDXComponent']:
+    def _remove_config_only(self, components: Dict[str, Dict]) -> Dict[str, Dict]:
         # Remove configuration only components.
         if not self.args.rem_config:
             return components
 
         remove = []
         for name, info in components.items():
             if info['type'] == 'CONFIG_ONLY':
@@ -458,35 +585,48 @@
             lib = line.split('(',1)[0]
             if not os.path.isabs(lib):
                 lib = utils.pjoin(self.proj_desc['build_dir'], lib)
             libs.add(lib)
 
         return list(libs)
 
-    def _remove_not_linked(self, components: Dict[str, 'SPDXComponent']) -> Dict[str, 'SPDXComponent']:
+    def _remove_not_linked(self, components: Dict[str, Dict]) -> Dict[str, Dict]:
         # Remove components not linked into the final binary.
         if not self.args.rem_unused:
             return components
 
         remove = []
         for name, info in components.items():
             if info['type'] == 'CONFIG_ONLY':
                 continue
             if not info['file'] in self.linked_libs:
                 remove.append(name)
 
         return self._remove_components(remove, components)
 
-    def _filter_components(self, components: Dict[str, 'SPDXComponent']) -> Dict[str, 'SPDXComponent']:
+    def _filter_components(self, components: Dict[str, Dict]) -> Dict[str, Dict]:
         # Wrapper for all filtering functions.
         components = self._remove_config_only(components)
         components = self._remove_not_linked(components)
 
         return components
 
+    def _component_used(self, info: Dict) -> bool:
+        """Helper to check if component was used as part of the project.
+        Configuration only components and components not linked into the final binary
+        are considered as not used, unless explicitly requested."""
+        # Configuration only component.
+        if not self.args.add_config_deps and info['type'] == 'CONFIG_ONLY':
+            return False
+        # Components not linked into final binary.
+        if not self.args.add_unused_deps and info['type'] == 'LIBRARY' and info['file'] not in self.linked_libs:
+            return False
+
+        return True
+
     def _get_components(self) -> Dict[str, 'SPDXComponent']:
         """Get information about components from project_description.json.
         Components are filtered based on preferences and their dependencies linked
         via SPDX Relationship tag."""
         build_components = self.proj_desc['build_component_info']
         build_components = self._filter_components(build_components)
         components: Dict[str, SPDXComponent] = {}
@@ -494,29 +634,35 @@
         for name, info in build_components.items():
             components[name] = SPDXComponent(self.args, self.proj_desc, name, info)
 
         for name, info in build_components.items():
             reqs = set(info['reqs'] + info['priv_reqs'] + info['managed_reqs'] + info['managed_priv_reqs'])
             log.err.debug(f'component {name} requires: {reqs}')
             for req in reqs:
-                # Don't add dependencies on configuration only components for components
-                # with library, unless explicitly requested.
-                if (not self.args.add_config_deps and
-                        build_components[req]['type'] == 'CONFIG_ONLY'):
-                    continue
-                # Don't add dependencies on components not linked into final binary, unless
-                # explicitly requested.
-                if (not self.args.add_unused_deps and
-                        build_components[req]['type'] == 'LIBRARY' and
-                        build_components[req]['file'] not in self.linked_libs):
+                if not self._component_used(build_components[req]):
                     continue
                 components[name]['Relationship'] += [f'{components[name]["SPDXID"][0]} DEPENDS_ON {components[req]["SPDXID"][0]}']
 
         return components
 
+    def _add_spdx_file_tags(self) -> None:
+        # Collect tags from components and submodules which have
+        # relationship with Project package.
+        def walk_submodules(submodules):
+            for submodule in submodules:
+                yield submodule
+                yield from walk_submodules(submodule.submodules)
+
+        for component in self.components.values():
+            if not self._component_used(component.info):
+                continue
+            self.tags |= component.tags
+            for submodule in walk_submodules(component.submodules):
+                self.tags |= submodule.tags
+
     def _add_relationships(self) -> None:
         if self.manifest['repository']:
             self['ExternalRef'] += [f'OTHER repository {self.manifest["repository"]}']
 
         if self.manifest['cpe']:
             self['ExternalRef'] += [f'SECURITY cpe23Type {self.manifest["cpe"]}']
         else:
@@ -537,24 +683,15 @@
         for name, info in build_components.items():
             tmp = info['reqs'] + info['priv_reqs'] + info['managed_reqs'] + info['managed_priv_reqs']
             reqs |= set(tmp)
 
         for name, info in build_components.items():
             if name in reqs:
                 continue
-            # Don't add Project dependency on configuration components unless
-            # explicitly requested.
-            if (not self.args.add_config_deps and
-                    build_components[name]['type'] == 'CONFIG_ONLY'):
-                continue
-            # Don't add Project dependency on not linked components unless
-            # explicitly requested.
-            if (not self.args.add_unused_deps and
-                    build_components[name]['type'] == 'LIBRARY' and
-                    build_components[name]['file'] not in self.linked_libs):
+            if not self._component_used(build_components[name]):
                 continue
             self['Relationship'] += [f'{self["SPDXID"][0]} DEPENDS_ON {self.components[name]["SPDXID"][0]}']
 
     def dump(self, colors=False) -> str:
         out = log.LogString(colors=colors)
         out += super().dump(colors)
 
@@ -581,33 +718,44 @@
         super().__init__(args, proj_desc)
 
         self.info = self._get_toolchain_info()
         self.name = self.info['name']
         self.version = self.info['version']
         self.files = None
 
+        path = utils.pjoin(self.info['path'], self.info['version'])
         if self.include_files(url=self.info['url'], ver=self.info['version']):
-            path = utils.pjoin(self.info['path'], self.info['version'])
             self.files = self.get_files(path, self.name)
+        if args.file_tags:
+            self.tags = SPDXDirTags(path)
 
         self['PackageName'] = [self.name]
         self['PackageSummary'] = [f'<text>{self.info["description"]}</text>']
         self['SPDXID'] = ['SPDXRef-TOOLCHAIN-' + self.sanitize_spdxid(self.name)]
         self['PackageVersion'] = [self.version]
         self['PackageSupplier'] = [self.ESPRESSIF_SUPPLIER]
         self['PackageDownloadLocation'] = [self.info['url']]
         if self.files:
             self['FilesAnalyzed'] = ['true']
             self['PackageVerificationCode'] = [self.get_verification_code([f.sha1 for f in self.files])]
-            self['PackageLicenseInfoFromFiles'] = ['NOASSERTION']
+            if self.tags.licenses:
+                self['PackageLicenseInfoFromFiles'] = list(self.tags.licenses)
+            else:
+                self['PackageLicenseInfoFromFiles'] = ['NOASSERTION']
         else:
             self['FilesAnalyzed'] = ['false']
-        self['PackageLicenseConcluded'] = ['NOASSERTION']
+        if self.tags.licenses_expressions:
+            self['PackageLicenseConcluded'] = [self.tags.get_license_concluded()]
+        else:
+            self['PackageLicenseConcluded'] = ['NOASSERTION']
         self['PackageLicenseDeclared'] = ['NOASSERTION']
-        self['PackageCopyrightText'] = ['NOASSERTION']
+        if self.tags.copyrights:
+            self['PackageCopyrightText'] = ['<text>{}</text>'.format('\n'.join(self.tags.copyrights))]
+        else:
+            self['PackageCopyrightText'] = ['NOASSERTION']
 
     def _get_current_platform(self) -> str:
         # Get current platform directly from idf_tools.py.
         idf_tools = utils.pjoin(self.proj_desc['idf_path'], 'tools')
         sys.path.append(idf_tools)
         from idf_tools import CURRENT_PLATFORM
         return str(CURRENT_PLATFORM)
@@ -678,45 +826,58 @@
     def __init__(self, args: Namespace, proj_desc: Dict[str, Any], name: str, info: dict):
         super().__init__(args, proj_desc)
         self.name = name
         self.dir = info['dir']
         self.info = info
         self.manifest = self._get_manifest()
         self.submodules = self.get_submodules(self.dir, self.name)
-        self.files = None
+        self.files = []
 
-        # exclude submodules path if any
+        # exclude submodule paths if any
         exclude_dirs = [submod.dir for submod in self.submodules]
+
         if self.include_files(repo=self.manifest['repository'],
                               url=self.manifest['url'],
-                              ver=self.manifest['version'],
-                              ):
+                              ver=self.manifest['version']):
             self.files = self.get_files(self.dir, self.name, exclude_dirs)
 
+        if args.file_tags:
+            if self.files:
+                self.tags = SPDXFileObjsTags(self.files)
+            else:
+                self.tags = SPDXDirTags(self.dir, exclude_dirs)
+
         self['PackageName'] = [f'component-{self.name}']
         if self.manifest['description']:
             self['PackageSummary'] = [f'<text>{self.manifest["description"]}</text>']
         self['SPDXID'] = ['SPDXRef-COMPONENT-' + self.sanitize_spdxid(self.name)]
         if self.manifest['version']:
             self['PackageVersion'] = [self.manifest['version']]
         self['PackageSupplier'] = [self.manifest['supplier'] or 'NOASSERTION']
         if self.manifest['originator']:
             self['PackageOriginator'] = [self.manifest['originator']]
         self['PackageDownloadLocation'] = [self.manifest['url'] or 'NOASSERTION']
         if self.files:
             self['FilesAnalyzed'] = ['true']
             self['PackageVerificationCode'] = [self.get_verification_code([f.sha1 for f in self.files])]
-            self['PackageLicenseInfoFromFiles'] = ['NOASSERTION']
+            if self.tags.licenses:
+                self['PackageLicenseInfoFromFiles'] = list(self.tags.licenses)
+            else:
+                self['PackageLicenseInfoFromFiles'] = ['NOASSERTION']
         else:
             self['FilesAnalyzed'] = ['false']
-        self['PackageLicenseConcluded'] = ['NOASSERTION']
-        self['PackageLicenseDeclared'] = ['NOASSERTION']
-        self['PackageCopyrightText'] = ['NOASSERTION']
-        if self.info['type'] == 'CONFIG_ONLY':
-            self['PackageComment'] = ['<text>Configuration only component.</text>']
+        if self.tags.licenses_expressions:
+            self['PackageLicenseConcluded'] = [self.tags.get_license_concluded()]
+        else:
+            self['PackageLicenseConcluded'] = ['NOASSERTION']
+        self['PackageLicenseDeclared'] = [self.manifest['license'] or 'NOASSERTION']
+        if self.tags.copyrights:
+            self['PackageCopyrightText'] = ['<text>{}</text>'.format('\n'.join(self.tags.copyrights))]
+        else:
+            self['PackageCopyrightText'] = ['NOASSERTION']
 
         self._add_relationships()
 
     def _get_manifest(self) -> Dict[str, str]:
         # Get manifest information and try to fill in missing pieces.
         manifest = self.get_manifest(self.dir)
         if not manifest['version']:
@@ -767,50 +928,91 @@
     def __init__(self, args: Namespace, proj_desc: Dict[str, Any], parent_name: str, info: dict):
         super().__init__(args, proj_desc)
         self.name = info['rel_path']
         self.info = info
         self.dir = info['path']
         self.manifest = self._get_manifest()
         self.submodules = self.get_submodules(self.dir, f'{parent_name}-{self.name}')
-        self.files = None
+        self.files = []
 
+        # exclude submodule paths if any
         exclude_dirs = [submod.dir for submod in self.submodules]
+
         if self.include_files(repo=self.manifest['repository'],
                               url=self.manifest['url'],
-                              ver=self.manifest['version'],
-                              ):
+                              ver=self.manifest['version']):
             self.files = self.get_files(self.dir, f'{parent_name}-{self.name}', exclude_dirs)
 
+        if args.file_tags:
+            if self.files:
+                self.tags = SPDXFileObjsTags(self.files)
+            else:
+                self.tags = SPDXDirTags(self.dir, exclude_dirs)
+
         self['PackageName'] = [f'submodule-./{self.name}']
         if self.manifest['description']:
             self['PackageSummary'] = [f'<text>{self.manifest["description"]}</text>']
         self['SPDXID'] = ['SPDXRef-SUBMODULE-' + self.sanitize_spdxid(f'{parent_name}-{self.name}')]
         if self.manifest['version']:
             self['PackageVersion'] = [self.manifest['version']]
         self['PackageSupplier'] = [self.manifest['supplier'] or 'NOASSERTION']
         if self.manifest['originator']:
             self['PackageOriginator'] = [self.manifest['originator']]
         self['PackageDownloadLocation'] = [self.manifest['url'] or 'NOASSERTION']
         if self.files:
             self['FilesAnalyzed'] = ['true']
             self['PackageVerificationCode'] = [self.get_verification_code([f.sha1 for f in self.files])]
-            self['PackageLicenseInfoFromFiles'] = ['NOASSERTION']
+            if self.tags.licenses:
+                self['PackageLicenseInfoFromFiles'] = list(self.tags.licenses)
+            else:
+                self['PackageLicenseInfoFromFiles'] = ['NOASSERTION']
         else:
             self['FilesAnalyzed'] = ['false']
-        self['PackageLicenseConcluded'] = ['NOASSERTION']
-        self['PackageLicenseDeclared'] = ['NOASSERTION']
-        self['PackageCopyrightText'] = ['NOASSERTION']
+        if self.tags.licenses_expressions:
+            self['PackageLicenseConcluded'] = [self.tags.get_license_concluded()]
+        else:
+            self['PackageLicenseConcluded'] = ['NOASSERTION']
+        self['PackageLicenseDeclared'] = [self.manifest['license'] or 'NOASSERTION']
+        if self.tags.copyrights:
+            self['PackageCopyrightText'] = ['<text>{}</text>'.format('\n'.join(self.tags.copyrights))]
+        else:
+            self['PackageCopyrightText'] = ['NOASSERTION']
 
         self._add_relationships()
 
     def _get_manifest(self) -> Dict[str, str]:
         # Get manifest information and try to fill in missing pieces from .gitmodules
         # if available.
+        def get_submodule_config() -> Dict[str,str]:
+            # Return validated submodule git configuration.
+            def validate_submodule_config(config: Dict[str,str]) -> None:
+                try:
+                    submodule_schema = schema.Schema(
+                        {
+                            schema.Optional('sbom-version'): str,
+                            schema.Optional('sbom-repository'): schema.And(str, self.check_url),
+                            schema.Optional('sbom-url'): schema.And(str, self.check_url),
+                            schema.Optional('sbom-cpe'): schema.And(str, self.check_cpe),
+                            schema.Optional('sbom-supplier'): schema.And(str, self.check_person_organization),
+                            schema.Optional('sbom-originator'): schema.And(str, self.check_person_organization),
+                            schema.Optional('sbom-description'): str,
+                            schema.Optional('sbom-license'): schema.And(str, self.check_license),
+                        }, ignore_extra_keys=True)
+
+                    submodule_schema.validate(config)
+                except schema.SchemaError as e:
+                    fn = utils.pjoin(self.info['git_wdir'], '.gitmodules')
+                    log.err.die(f'The submodule "{self.info["sm_path"]}" sbom information in "{fn}" is not valid: {e}')
+
+            module_cfg = git.get_submodule_config(self.info['git_wdir'], self.info['name'])
+            validate_submodule_config(module_cfg)
+            return module_cfg
+
         manifest = self.get_manifest(self.dir)
-        module_cfg = git.get_submodule_config(self.info['git_wdir'], self.info['name'])
+        module_cfg = get_submodule_config()
         if not manifest['version']:
             if 'sbom-version' in module_cfg:
                 manifest['version'] = module_cfg['sbom-version']
             else:
                 manifest['version'] = self.guess_version(self.dir)
 
         if not manifest['cpe']:
@@ -821,14 +1023,17 @@
 
         if not manifest['url']:
             manifest['url'] = module_cfg.get('sbom-url', '')
 
         if not manifest['description']:
             manifest['description'] = module_cfg.get('sbom-description', '')
 
+        if not manifest['license']:
+            manifest['license'] = module_cfg.get('sbom-license', '')
+
         if not manifest['repository']:
             if 'sbom-repository' in module_cfg:
                 manifest['repository'] = module_cfg['sbom-repository']
             else:
                 manifest['repository'] = git.get_remote_location(self.dir)
 
         if not manifest['supplier']:
@@ -872,26 +1077,45 @@
         return str(out)
 
 
 class SPDXFile(SPDXObject):
     """SPDX File Information."""
     def __init__(self, args: Namespace, proj_desc: Dict[str, Any], fn: str, basedir: str, prefix: str):
         super().__init__(args, proj_desc)
+        self.path = fn
         self.sha1 = self.hash_file(fn, 'sha1')
         self.sha256 = self.hash_file(fn, 'sha256')
         relpath = utils.prelpath(fn, basedir)
 
+        if args.file_tags:
+            self.tags = SPDXFileTags(self.path)
+
         self['FileName'] = ['./' + relpath]
         self['SPDXID'] = ['SPDXRef-FILE-' + self.sanitize_spdxid(f'{prefix}-{relpath}')]
-        self['LicenseConcluded'] = ['NOASSERTION']
-        self['LicenseInfoInFile'] = ['NOASSERTION']
-        self['FileCopyrightText'] = ['NOASSERTION']
         self['FileChecksum'] += [f'SHA1: {self.sha1}']
         self['FileChecksum'] += [f'SHA256: {self.sha256}']
 
+        if self.tags.licenses:
+            self['LicenseInfoInFile'] = list(self.tags.licenses)
+        else:
+            self['LicenseInfoInFile'] = ['NOASSERTION']
+
+        if self.tags.licenses_expressions:
+            self['LicenseConcluded'] = [self.tags.get_license_concluded()]
+        else:
+            self['LicenseConcluded'] = ['NOASSERTION']
+
+        if self.tags.copyrights:
+            self['FileCopyrightText'] = ['<text>' + '\n'.join(self.tags.copyrights) + '</text>']
+        else:
+            self['FileCopyrightText'] = ['NOASSERTION']
+
+        if self.tags.contributors:
+            self['FileContributor'] = list(self.tags.contributors)
+
     def dump(self, colors=False) -> str:
         return super().dump(colors)
 
 
 def parse_packages(buf: str) -> Dict[str, Dict[str, List[str]]]:
     """Very dummy SPDX file parser. Returns dictionary, where key is
     package SPDXID and value is dictionary with SPDX tag/values."""
@@ -904,15 +1128,16 @@
 
         if not line or line[0] == '#':
             continue
 
         try:
             tag, val = line.split(':', maxsplit=1)
         except ValueError:
-            log.err.die(f'invalid spdx tag/value line: "{line}"')
+            # can be multiline text inside <text>...</text>
+            continue
 
         tag = tag.strip()
         val = val.strip()
 
         if tag == 'PackageName':
             in_package = True
             idx += 1
```

### Comparing `esp-idf-sbom-0.2.0/esp_idf_sbom/libsbom/utils.py` & `esp-idf-sbom-0.3.0/esp_idf_sbom/libsbom/utils.py`

 * *Files identical despite different names*

### Comparing `esp-idf-sbom-0.2.0/esp_idf_sbom/sbom.py` & `esp-idf-sbom-0.3.0/esp_idf_sbom/sbom.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,14 +155,20 @@
                                      'to identify versions. With this option PackageSupplier and '
                                      'PackageVersion will be omitted, unless explicitly stated in '
                                      'sbom.yml, idf_component.yml or .gitmodules.'))
     create_parser.add_argument('-p', '--print',
                                action='store_true',
                                default=bool(os.environ.get('SBOM_CREATE_PRINT')),
                                help=('Print generated SBOM file to stdout even if "--output-file" is used.'))
+    create_parser.add_argument('--no-file-tags',
+                               dest='file_tags',
+                               action='store_false',
+                               default=not bool(os.environ.get('SBOM_CREATE_NO_FILE_TAGS')),
+                               help=('Do not scan files for SPDX file tags. This includes SPDX-License-Identifier, '
+                                     'SPDX-FileCopyrightText and SPDX-FileContributor'))
 
     check_parser = subparsers.add_parser('check',
                                          help=('Check components/submodules in the ESP-IDF SBOM file '
                                                'for possible vulnerabilities reported in the '
                                                'National Vulnerability Database.'))
     check_parser.set_defaults(func=cmd_check)
     check_parser.add_argument('input_file',
```

### Comparing `esp-idf-sbom-0.2.0/esp_idf_sbom.egg-info/PKG-INFO` & `esp-idf-sbom-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-idf-sbom
-Version: 0.2.0
+Version: 0.3.0
 Summary: SPDX SBOM generator for ESP-IDF projects
 Home-page: https://github.com/espressif/esp-idf-sbom
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,spdx,sbom
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -32,14 +32,44 @@
 The esp-idf-sbom tool creates [Software bill of materials][1] (SBOM)
 files in the [Software Package Data Exchange][2] (SPDX) format for applications
 generated by the [Espressif IoT Development Framework][3] (ESP-IDF).
 It also allows to check generated SBOM files for know vulnerabilities against
 the [National Vulnerability Database][4] (NVD) based on the
 [Common Platform Enumeration][5] (CPE) provided in the SBOM.
 
+## Required ESP-IDF versions
+
+All release branches of currently supported ESP-IDF versions allow to
+generate the SBOM file.
+
+| ESP-IDF version | branch with SBOM support  | commits
+|-----------------|---------------------------|----------------------------------------------------------------------------------------------------------------------------------|
+| 4.3             | release/v4.3              | [befb32b45bc9314b48c29624f9a2c2ef30e34260](https://github.com/espressif/esp-idf/commit/befb32b45bc9314b48c29624f9a2c2ef30e34260) |
+|                 |                           | [f1eef50947ab5770ae4d904c07615e7acab06002](https://github.com/espressif/esp-idf/commit/f1eef50947ab5770ae4d904c07615e7acab06002) |
+| 4.4             | release/v4.4              | [ee505a996045c3657711c3d70c58af8dd48b1426](https://github.com/espressif/esp-idf/commit/ee505a996045c3657711c3d70c58af8dd48b1426) |
+|                 |                           | [53f271ce108d6fa99cf92d59fe9b9dcc4b8fb45b](https://github.com/espressif/esp-idf/commit/53f271ce108d6fa99cf92d59fe9b9dcc4b8fb45b) |
+| 5.0             | release/v5.0              | [30735b33efabd6cf038bcb258b674cf828ad5ecf](https://github.com/espressif/esp-idf/commit/30735b33efabd6cf038bcb258b674cf828ad5ecf) |
+|                 |                           | [9156bbb55c920d6704329975311c331b931ed6bc](https://github.com/espressif/esp-idf/commit/9156bbb55c920d6704329975311c331b931ed6bc) |
+| 5.1             | release/v5.1              | [0f781c718c8548cd2b0e41a30e1814f1c6ed93a2](https://github.com/espressif/esp-idf/commit/0f781c718c8548cd2b0e41a30e1814f1c6ed93a2) |
+|                 |                           | [03162bb276d4155760e8aa839020f0587f5ef599](https://github.com/espressif/esp-idf/commit/03162bb276d4155760e8aa839020f0587f5ef599) |
+| latest          | master                    |                                                                                                                                  |
+
+Older versions, e.g. `v5.0.2`, do not have the required code merged and the following error
+message will be printed.
+
+    E: Project description file "build/project_description.json" does not support SBOM generation. Please see the list of IDF versions required by esp-idf-sbom.
+
+If you see this error message and want to try `esp-idf-sbom`, you can
+
+1. switch to the release branch for version you are using. For example `release/v5.0` if you are using `v5.0.2`.
+2. use future ESP-IDF versions to experiment with esp-idf-sbom.
+3. use `git-cherry-pick` and apply commits for your release from the table above. For example for `v5.0.2` use
+
+    $ git cherry-pick 30735b33efabd6cf038bcb258b674cf828ad5ecf 9156bbb55c920d6704329975311c331b931ed6bc
+
 
 ## SPDX SBOM layout
 
 The SBOM file is created based on application sources, build artefacts, information
 provided by the ESP-IDF build system and SBOM manifest files. The resulting SBOM
 file contains SPDX packages for the final **project** application, used **toolchain**,
 **components** used during build and git **submodules**. Packages are linked
@@ -76,14 +106,17 @@
     Package originator. If the package comes from another person or organization
     that has been identified as a supplier. For example if a component is based
     on 3rd party code with some modifications, the originator is the 3rd party code
     author, but the supplier is the person or organization distributing the final
     component. For more detailed information please see the SPDX specification.
     As for supplier, *Person:* or *Organization:* prefix should be used for
     originator value.
+* **license**:
+    License expression explicitly declared by the author.
+
 
 Example of the `sbom.yml` manifest file for the ESP-IDF blink example.
 
 ```
 version: 0.1.0
 description: Blink application example
 url: https://blink.org/blink-0.1.0.tar.gz # non-existing package download URL example
@@ -97,32 +130,44 @@
 ```
 version: 0.1.0
 description: Main component for blink application
 repository: https://github.com/espressif/esp-idf.git@dc016f59877d13e6e7d4fc193aa5aa764547f16d#examples/get-started/blink
 supplier: 'Organization: Espressif Systems (Shanghai) CO LTD'
 ```
 
-Information from the `sbom.yml` file are mapped to the following SPDX tags.
+Information from the `sbom.yml` manifest file are mapped to the following SPDX tags.
 
 | manifest     | SPDX                         |
 |--------------|------------------------------|
 | version      | PackageVersion               |
 | description  | PackageSummary               |
 | repository   | ExternalRef OTHER repository |
 | url          | PackageDownloadLocation      |
 | cpe          | ExternalRef cpe23Type        |
 | supplier     | PackageSupplier              |
 | originator   | PackageOriginator            |
+| license      | PackageLicenseDeclared       |
 
 Even though the `sbom.yml` file is the primary source of information, the esp-idf-sbom tool
-is also looking at other places if it's not present. The version, description and url
-information from the `idf_component.yml` manifest file is used for components managed by
-the component manager. Component version may be guessed based on git-describe and Espressif
+is also looking at other places if it's not present. The version, description, maintainers and
+url information from the `idf_component.yml` manifest file is used for components managed by
+the component manager.
+
+Information from the `idf_component.yml` manifest file are mapped to the following SPDX tags.
+
+| manifest     | SPDX                         |
+|--------------|------------------------------|
+| version      | PackageVersion               |
+| description  | PackageSummary               |
+| maintainers  | PackageSupplier              |
+| url          | PackageDownloadLocation      |
+
+Component version may be guessed based on git-describe and Espressif
 as a default supplier may be guessed based on git repository or package URL. The guessing
-may be dissabled by using the '--no-guess' option. For submodules, the .gitmodules file is
+may be disabled by using the '--no-guess' option. For submodules, the .gitmodules file is
 also checked for additional submodule information.
 
 
 ## Installation
 
 Currently esp-idf-sbom is not integrated into ESP-IDF and needs to by installed
 separately from Python Package Index (PyPI) with
@@ -155,26 +200,43 @@
 Vulnerabilities are checked based on the [Common Platform Enumeration][5] (CPE) information
 included in the SBOM file for SPDX packages. While checking for vulnerabilities, only packages
 with direct or indirect relationship to the **project** package are examined. For example if mbedtls
 component is compiled, due to component dependecies, but it's actually not linked into the
 final binary, it will be by default presented in the SBOM file, but it will not be reachable
 from the root **project** package and hence it will not be checked for vulnerabilities.
 The reason for this is to avoid possible false possitives, because such packages
-have no direct impact on the resulting application. This can be changed with the `--all`
+have no direct impact on the resulting application. This can be changed with the `--check-all-packages`
 option. If used, all packages in the SBOM file will be checked for possible vulnerabilities
 regardless their relationships to the application binary.
 
 SBOM file generated by the esp-idf-sbom tool can be checked for known vulnerabilities
 with
 
     esp-idf-sbom check [SBOM file]
 
 If *SBOM file* is not provided, the stardard input stream is used.
 
 
+## Licenses and Copyrights
+
+All **component** and **submodule** files are scanned for the `SPDX-License-Identifier`,
+`SPDX-FileCopyrightText` and `SPDX-FileContributor` SPDX file tags. Information from
+these tags is used in the generated SBOM file to specify licenses and copyrights for
+SPDX packages which represent **project**, **component** or **submodule**. The project's
+final license expression is a logical AND of all licenses concluded from **components**
+and **submodules** used in the final project binary.
+
+The license can be also explicitly declared by the author in the `sbom.yml` file with the `license`
+variable. This information is used as a value for the `PackageLicenseDeclared` SPDX tag for
+given **project**, **component** or **submodule**.
+
+The `--no-file-tags` option disables scanning for SPDX file tags. When used the license and
+copyright information from files will not be presented in the generated SBOM file.
+
+
 ## Usage example
 
 This is an example of basic usage for the blink project, which is part of the ESP-IDF. The
 two `sbom.yml` files for project and main component showed above were added. It's expected
 that ESP-IDF is installed and set.
 
 ```
```

### Comparing `esp-idf-sbom-0.2.0/esp_idf_sbom.egg-info/SOURCES.txt` & `esp-idf-sbom-0.3.0/esp_idf_sbom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `esp-idf-sbom-0.2.0/setup.py` & `esp-idf-sbom-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     url='https://github.com/espressif/esp-idf-sbom',
     packages=find_packages(),
     python_requires='>=3.7',
     keywords=['espressif', 'embedded', 'spdx', 'sbom'],
     install_requires=[
         'PyYAML',
         'schema',
+        'license-expression',
     ],
     classifiers=[
         'Development Status :: 1 - Planning',
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'Environment :: Console',
         'Topic :: Software Development :: Embedded Systems',
```

