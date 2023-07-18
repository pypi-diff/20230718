# Comparing `tmp/dockerfile-parse-1.2.0.tar.gz` & `tmp/dockerfile-parse-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dockerfile-parse-1.2.0.tar", last modified: Wed Jun  9 13:18:15 2021, max compression
+gzip compressed data, was "dockerfile-parse-2.0.0.tar", last modified: Tue Dec 13 18:32:43 2022, max compression
```

## Comparing `dockerfile-parse-1.2.0.tar` & `dockerfile-parse-2.0.0.tar`

### file list

```diff
@@ -1,25 +1,22 @@
-drwxr-xr-x   0 rcerven   (1000) rcerven   (1000)        0 2021-06-09 13:18:15.964176 dockerfile-parse-1.2.0/
--rw-r--r--   0 rcerven   (1000) rcerven   (1000)     1488 2017-01-30 17:32:10.000000 dockerfile-parse-1.2.0/LICENSE
--rw-r--r--   0 rcerven   (1000) rcerven   (1000)      148 2017-02-03 13:19:31.000000 dockerfile-parse-1.2.0/MANIFEST.in
--rw-r--r--   0 rcerven   (1000) rcerven   (1000)     3791 2021-06-09 13:18:15.964176 dockerfile-parse-1.2.0/PKG-INFO
--rw-r--r--   0 rcerven   (1000) rcerven   (1000)     2198 2021-06-09 13:15:33.000000 dockerfile-parse-1.2.0/README.md
-drwxr-xr-x   0 rcerven   (1000) rcerven   (1000)        0 2021-06-09 13:18:15.962175 dockerfile-parse-1.2.0/dockerfile_parse/
--rw-r--r--   0 rcerven   (1000) rcerven   (1000)      359 2021-06-09 13:15:36.000000 dockerfile-parse-1.2.0/dockerfile_parse/__init__.py
--rw-r--r--   0 rcerven   (1000) rcerven   (1000)      403 2020-05-12 09:06:05.000000 dockerfile-parse-1.2.0/dockerfile_parse/constants.py
--rw-r--r--   0 rcerven   (1000) rcerven   (1000)    33451 2021-06-09 13:15:33.000000 dockerfile-parse-1.2.0/dockerfile_parse/parser.py
--rw-r--r--   0 rcerven   (1000) rcerven   (1000)    10747 2021-06-09 13:15:33.000000 dockerfile-parse-1.2.0/dockerfile_parse/util.py
-drwxr-xr-x   0 rcerven   (1000) rcerven   (1000)        0 2021-06-09 13:18:15.963175 dockerfile-parse-1.2.0/dockerfile_parse.egg-info/
--rw-r--r--   0 rcerven   (1000) rcerven   (1000)     3791 2021-06-09 13:18:15.000000 dockerfile-parse-1.2.0/dockerfile_parse.egg-info/PKG-INFO
--rw-r--r--   0 rcerven   (1000) rcerven   (1000)      466 2021-06-09 13:18:15.000000 dockerfile-parse-1.2.0/dockerfile_parse.egg-info/SOURCES.txt
--rw-r--r--   0 rcerven   (1000) rcerven   (1000)        1 2021-06-09 13:18:15.000000 dockerfile-parse-1.2.0/dockerfile_parse.egg-info/dependency_links.txt
--rw-r--r--   0 rcerven   (1000) rcerven   (1000)        4 2021-06-09 13:18:15.000000 dockerfile-parse-1.2.0/dockerfile_parse.egg-info/requires.txt
--rw-r--r--   0 rcerven   (1000) rcerven   (1000)       17 2021-06-09 13:18:15.000000 dockerfile-parse-1.2.0/dockerfile_parse.egg-info/top_level.txt
--rw-r--r--   0 rcerven   (1000) rcerven   (1000)        0 2017-02-03 13:19:31.000000 dockerfile-parse-1.2.0/requirements-py3.txt
--rw-r--r--   0 rcerven   (1000) rcerven   (1000)        4 2018-08-22 13:11:35.000000 dockerfile-parse-1.2.0/requirements.txt
--rw-r--r--   0 rcerven   (1000) rcerven   (1000)       38 2021-06-09 13:18:15.964176 dockerfile-parse-1.2.0/setup.cfg
--rwxr-xr-x   0 rcerven   (1000) rcerven   (1000)     2306 2021-06-09 13:15:36.000000 dockerfile-parse-1.2.0/setup.py
-drwxr-xr-x   0 rcerven   (1000) rcerven   (1000)        0 2021-06-09 13:18:15.964176 dockerfile-parse-1.2.0/tests/
--rw-r--r--   0 rcerven   (1000) rcerven   (1000)      178 2017-01-30 17:32:10.000000 dockerfile-parse-1.2.0/tests/__init__.py
--rw-r--r--   0 rcerven   (1000) rcerven   (1000)     1223 2020-06-26 14:42:56.000000 dockerfile-parse-1.2.0/tests/fixtures.py
--rw-r--r--   0 rcerven   (1000) rcerven   (1000)       44 2021-06-09 13:15:33.000000 dockerfile-parse-1.2.0/tests/requirements.txt
--rw-r--r--   0 rcerven   (1000) rcerven   (1000)    57284 2021-06-09 13:15:33.000000 dockerfile-parse-1.2.0/tests/test_parser.py
+drwxrwxr-x   0 mkosiarc  (1000) mkosiarc  (1000)        0 2022-12-13 18:32:43.042649 dockerfile-parse-2.0.0/
+-rw-rw-r--   0 mkosiarc  (1000) mkosiarc  (1000)     1488 2022-12-13 18:20:34.000000 dockerfile-parse-2.0.0/LICENSE
+-rw-rw-r--   0 mkosiarc  (1000) mkosiarc  (1000)      148 2022-12-13 18:20:34.000000 dockerfile-parse-2.0.0/MANIFEST.in
+-rw-rw-r--   0 mkosiarc  (1000) mkosiarc  (1000)     3333 2022-12-13 18:32:43.041649 dockerfile-parse-2.0.0/PKG-INFO
+-rw-rw-r--   0 mkosiarc  (1000) mkosiarc  (1000)     2198 2022-12-13 18:20:34.000000 dockerfile-parse-2.0.0/README.md
+drwxrwxr-x   0 mkosiarc  (1000) mkosiarc  (1000)        0 2022-12-13 18:32:43.041649 dockerfile-parse-2.0.0/dockerfile_parse/
+-rw-rw-r--   0 mkosiarc  (1000) mkosiarc  (1000)      464 2022-12-13 18:23:05.000000 dockerfile-parse-2.0.0/dockerfile_parse/__init__.py
+-rw-rw-r--   0 mkosiarc  (1000) mkosiarc  (1000)      269 2022-12-13 18:20:34.000000 dockerfile-parse-2.0.0/dockerfile_parse/constants.py
+-rw-rw-r--   0 mkosiarc  (1000) mkosiarc  (1000)    33320 2022-12-13 18:20:34.000000 dockerfile-parse-2.0.0/dockerfile_parse/parser.py
+-rw-rw-r--   0 mkosiarc  (1000) mkosiarc  (1000)    10562 2022-12-13 18:20:34.000000 dockerfile-parse-2.0.0/dockerfile_parse/util.py
+drwxrwxr-x   0 mkosiarc  (1000) mkosiarc  (1000)        0 2022-12-13 18:32:43.041649 dockerfile-parse-2.0.0/dockerfile_parse.egg-info/
+-rw-rw-r--   0 mkosiarc  (1000) mkosiarc  (1000)     3333 2022-12-13 18:32:43.000000 dockerfile-parse-2.0.0/dockerfile_parse.egg-info/PKG-INFO
+-rw-rw-r--   0 mkosiarc  (1000) mkosiarc  (1000)      389 2022-12-13 18:32:43.000000 dockerfile-parse-2.0.0/dockerfile_parse.egg-info/SOURCES.txt
+-rw-rw-r--   0 mkosiarc  (1000) mkosiarc  (1000)        1 2022-12-13 18:32:43.000000 dockerfile-parse-2.0.0/dockerfile_parse.egg-info/dependency_links.txt
+-rw-rw-r--   0 mkosiarc  (1000) mkosiarc  (1000)       17 2022-12-13 18:32:43.000000 dockerfile-parse-2.0.0/dockerfile_parse.egg-info/top_level.txt
+-rw-rw-r--   0 mkosiarc  (1000) mkosiarc  (1000)       38 2022-12-13 18:32:43.042649 dockerfile-parse-2.0.0/setup.cfg
+-rwxrwxr-x   0 mkosiarc  (1000) mkosiarc  (1000)     2096 2022-12-13 18:23:05.000000 dockerfile-parse-2.0.0/setup.py
+drwxrwxr-x   0 mkosiarc  (1000) mkosiarc  (1000)        0 2022-12-13 18:32:43.041649 dockerfile-parse-2.0.0/tests/
+-rw-rw-r--   0 mkosiarc  (1000) mkosiarc  (1000)      178 2022-12-13 18:20:34.000000 dockerfile-parse-2.0.0/tests/__init__.py
+-rw-rw-r--   0 mkosiarc  (1000) mkosiarc  (1000)     1165 2022-12-13 18:20:34.000000 dockerfile-parse-2.0.0/tests/fixtures.py
+-rw-rw-r--   0 mkosiarc  (1000) mkosiarc  (1000)       44 2022-12-13 18:20:34.000000 dockerfile-parse-2.0.0/tests/requirements.txt
+-rw-rw-r--   0 mkosiarc  (1000) mkosiarc  (1000)    57411 2022-12-13 18:20:34.000000 dockerfile-parse-2.0.0/tests/test_parser.py
```

### Comparing `dockerfile-parse-1.2.0/LICENSE` & `dockerfile-parse-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dockerfile-parse-1.2.0/README.md` & `dockerfile-parse-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dockerfile-parse-1.2.0/dockerfile_parse/parser.py` & `dockerfile-parse-2.0.0/dockerfile_parse/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,20 @@
 Copyright (c) 2015, 2018, 2019 Red Hat, Inc
 All rights reserved.
 
 This software may be modified and distributed under the terms
 of the BSD license. See the LICENSE file for details.
 """
 
-from __future__ import print_function, unicode_literals, absolute_import
-
 import json
 import logging
 import os
 import re
 from contextlib import contextmanager
-from six import string_types
-from six.moves import shlex_quote as quote
+from shlex import quote
 
 from .constants import DOCKERFILE_FILENAME, COMMENT_INSTRUCTION
 from .util import (b2u, extract_key_values, get_key_val_dictionary,
                    u2b, Context, WordSplitter)
 
 
 logger = logging.getLogger(__name__)
@@ -161,34 +158,34 @@
         :return: list containing lines (unicode) from Dockerfile
         """
         if self.cache_content and self.cached_content:
             return self.cached_content.splitlines(True)
 
         try:
             with self._open_dockerfile('rb') as dockerfile:
-                lines = [b2u(l) for l in dockerfile.readlines()]
+                lines = [b2u(line) for line in dockerfile.readlines()]
                 if self.cache_content:
                     self.cached_content = ''.join(lines)
                 return lines
         except (IOError, OSError) as ex:
             logger.error("Couldn't retrieve lines from dockerfile: %r", ex)
             raise
 
     @lines.setter
     def lines(self, lines):
         """
         Fill Dockerfile content with specified lines
         :param lines: list of lines to be written to Dockerfile
         """
         if self.cache_content:
-            self.cached_content = ''.join([b2u(l) for l in lines])
+            self.cached_content = ''.join(b2u(line) for line in lines)
 
         try:
             with self._open_dockerfile('wb') as dockerfile:
-                dockerfile.writelines([u2b(l) for l in lines])
+                dockerfile.writelines(u2b(line) for line in lines)
         except (IOError, OSError) as ex:
             logger.error("Couldn't write lines to dockerfile: %r", ex)
             raise
 
     @property
     def content(self):
         """
@@ -270,15 +267,15 @@
         directive_possible = True
         # escape directive regex
         escape_directive_re = re.compile(r'^\s*#\s*escape\s*=\s*(\\|`)\s*$', re.I)
         # syntax directive regex
         syntax_directive_re = re.compile(r'^\s*#\s*syntax\s*=\s*(.*)\s*$', re.I)
 
         in_continuation = False
-        current_instruction = None
+        current_instruction = {}
 
         for line in self.lines:
             lineno += 1
 
             if directive_possible:
                 # once support for python versions before 3.8 is dropped use walrus operator
                 if escape_directive_re.match(line):
@@ -312,24 +309,22 @@
                         instruction=m.groups()[0].upper(),
                         value=_rstrip_eol(m.groups()[1], line_continuation_char)
                     )
                 else:
                     current_instruction['content'] += line
                     current_instruction['endline'] = lineno
 
-                    # pylint: disable=unsupported-assignment-operation
                     if current_instruction['value']:
                         current_instruction['value'] += _rstrip_eol(line, line_continuation_char)
                     else:
                         current_instruction['value'] = _rstrip_eol(line.lstrip(),
                                                                    line_continuation_char)
-                    # pylint: enable=unsupported-assignment-operation
 
                 in_continuation = contre.match(line)
-                if not in_continuation and current_instruction is not None:
+                if not in_continuation and current_instruction:
                     instructions.append(current_instruction)
 
         return instructions
 
     @property
     def json(self):
         """
@@ -798,15 +793,15 @@
             assert anchor in self.structure, "Current structure does not match: {0}".format(anchor)
             if replace:
                 df_lines[anchor['startline']:anchor['endline'] + 1] = []
             if after:
                 anchor = anchor['endline']
             else:
                 anchor = anchor['startline']
-        elif isinstance(anchor, string_types):  # line contents
+        elif isinstance(anchor, str):  # line contents
             matches = [index for index, text in enumerate(df_lines) if text == anchor]
             if not matches:
                 raise RuntimeError("Cannot find line in the build file:\n" + anchor)
             anchor = matches[-1]
             if replace:
                 del df_lines[anchor]
         else:
@@ -867,18 +862,20 @@
 
 
 def image_from(from_value):
     """
     :param from_value: string like "image:tag" or "image:tag AS name"
     :return: tuple of the image and stage name, e.g. ("image:tag", None)
     """
-    regex = re.compile(r"""(?xi)     # readable, case-insensitive regex
-        \s*                          # ignore leading whitespace
-        (?P<image> \S+ )             # image and optional tag
-        (?:                          # optional "AS name" clause for stage
+    regex = re.compile(r"""(?xi)        # readable, case-insensitive regex
+        \s*                             # ignore leading whitespace
+        (?P<platform> --platform=\S+)?  # optional platform parameter
+        \s*                             # more whitespaces
+        (?P<image> \S+ )                # image and optional tag
+        (?:                             # optional "AS name" clause for stage
             \s+ AS \s+
             (?P<name> \S+ )
         )?
         """)
     match = re.match(regex, from_value)
     return match.group('image', 'name') if match else (None, None)
```

### Comparing `dockerfile-parse-1.2.0/dockerfile_parse/util.py` & `dockerfile-parse-2.0.0/dockerfile_parse/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,33 +3,27 @@
 Copyright (c) 2015 Red Hat, Inc
 All rights reserved.
 
 This software may be modified and distributed under the terms
 of the BSD license. See the LICENSE file for details.
 """
 
-from __future__ import print_function, unicode_literals, absolute_import
-
 from io import StringIO
-from six import text_type
-
-from .constants import PY2
 
 
 def b2u(string):
     """ bytes to unicode """
-    if (isinstance(string, bytes)
-            or (PY2 and isinstance(string, str))):
+    if isinstance(string, bytes):
         return string.decode('utf-8')
     return string
 
 
 def u2b(string):
     """ unicode to bytes"""
-    if isinstance(string, text_type):
+    if isinstance(string, str):
         return string.encode('utf-8')
     return string
 
 
 class WordSplitter(object):
     """
     Split string into words, substituting environment variables if provided
```

### Comparing `dockerfile-parse-1.2.0/setup.py` & `dockerfile-parse-2.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 All rights reserved.
 
 This software may be modified and distributed under the terms
 of the BSD license. See the LICENSE file for details.
 """
 
 import re
-import sys
 import io
 
 from os import path
 from setuptools import setup, find_packages
 
 
 def _get_requirements(path):
@@ -20,51 +19,45 @@
         with open(path) as f:
             packages = f.read().splitlines()
     except (IOError, OSError) as ex:
         raise RuntimeError("Can't open file with requirements: %s", repr(ex))
     return [p.strip() for p in packages if not re.match(r"^\s*#", p)]
 
 
-def _install_requirements():
-    requirements = _get_requirements('requirements.txt')
-    if sys.version_info[0] >= 3:
-        requirements += _get_requirements('requirements-py3.txt')
-    return requirements
-
-
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with io.open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='dockerfile-parse',
-    version='1.2.0',
+    version='2.0.0',
     description='Python library for Dockerfile manipulation',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Jiri Popelka',
     author_email='jpopelka@redhat.com',
     url='https://github.com/containerbuildsystem/dockerfile-parse',
     license="BSD",
     packages=find_packages(exclude=["tests"]),
-    install_requires=_install_requirements(),
+    python_requires='>=3.6',
+    install_requires=[],
     tests_require=_get_requirements('tests/requirements.txt'),
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Other Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Topic :: Software Development :: Libraries :: Python Modules'
     ],
 )
```

### Comparing `dockerfile-parse-1.2.0/tests/fixtures.py` & `dockerfile-parse-2.0.0/tests/fixtures.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 Copyright (c) 2015 Red Hat, Inc
 All rights reserved.
 
 This software may be modified and distributed under the terms
 of the BSD license. See the LICENSE file for details.
 """
 
-from __future__ import unicode_literals, absolute_import
+import io
 
 import pytest
-import six
+
 
 from dockerfile_parse import DockerfileParser
 
 
 @pytest.fixture(
     params=[(use_fileobj, cache_content)
             for use_fileobj in [True, False]
@@ -25,15 +25,15 @@
     :param tmpdir: already existing fixture defined in pytest
     :param request: parameter, cache_content arg to DockerfileParser
     :return: DockerfileParser instance
     """
 
     use_fileobj, cache_content = request.param
     if use_fileobj:
-        fileobj = six.BytesIO()
+        fileobj = io.BytesIO()
         return DockerfileParser(fileobj=fileobj, cache_content=cache_content)
     else:
         tmpdir_path = str(tmpdir.realpath())
         return DockerfileParser(path=tmpdir_path, cache_content=cache_content)
 
 
 @pytest.fixture(params=['LABEL', 'ENV', 'ARG'])
```

### Comparing `dockerfile-parse-1.2.0/tests/test_parser.py` & `dockerfile-parse-2.0.0/tests/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,20 @@
 Copyright (c) 2015, 2019 Red Hat, Inc
 All rights reserved.
 
 This software may be modified and distributed under the terms
 of the BSD license. See the LICENSE file for details.
 """
 
-from __future__ import unicode_literals, absolute_import
-
 import inspect
+import io
 import json
 import os
 import pytest
 import re
-import six
 import sys
 from textwrap import dedent
 
 from dockerfile_parse import DockerfileParser
 from dockerfile_parse.parser import image_from
 from dockerfile_parse.constants import COMMENT_INSTRUCTION
 from dockerfile_parse.util import b2u, u2b, Context
@@ -49,20 +47,20 @@
         setup_py = os.path.join(project_dir, "setup.py")
         spec_version = read_version(specfile, r"\nVersion:\s*(.+?)\s*\n")
         setup_py_version = read_version(setup_py, r"version=['\"](.+)['\"]")
         assert spec_version == module_version
         assert setup_py_version == module_version
 
     def test_util_b2u(self):
-        assert isinstance(b2u(u'string'), six.text_type)
-        assert isinstance(b2u(b'byte'), six.text_type)
+        assert isinstance(b2u('string'), str)
+        assert isinstance(b2u(b'byte'), str)
 
     def test_util_u2b(self):
-        assert isinstance(u2b(u'string'), six.binary_type)
-        assert isinstance(u2b(b'byte'), six.binary_type)
+        assert isinstance(u2b('string'), bytes)
+        assert isinstance(u2b(b'byte'), bytes)
 
     def test_util_context_exceptions(self):
         context = Context()
         with pytest.raises(ValueError):
             context.get_values('FOO')
         with pytest.raises(ValueError):
             context.get_line_value('FOO')
@@ -75,29 +73,29 @@
             LABEL label={0}""".format(NON_ASCII))
         df_lines = ["FROM fedora\n", "LABEL label={0}".format(NON_ASCII)]
 
         dfparser.content = ""
         dfparser.content = df_content
         assert dfparser.content == df_content
         assert dfparser.lines == df_lines
-        assert [isinstance(line, six.text_type) for line in dfparser.lines]
+        assert [isinstance(line, str) for line in dfparser.lines]
 
         dfparser.content = ""
         dfparser.lines = df_lines
         assert dfparser.content == df_content
         assert dfparser.lines == df_lines
-        assert [isinstance(line, six.text_type) for line in dfparser.lines]
+        assert [isinstance(line, str) for line in dfparser.lines]
 
         dockerfile = os.path.join(str(tmpdir), 'Dockerfile')
         with open(dockerfile, 'wb') as fp:
             fp.write(df_content.encode('utf-8'))
         dfparser = DockerfileParser(dockerfile)
         assert dfparser.content == df_content
         assert dfparser.lines == df_lines
-        assert [isinstance(line, six.text_type) for line in dfparser.lines]
+        assert [isinstance(line, str) for line in dfparser.lines]
 
     def test_dockerfileparser_exceptions(self, tmpdir):
         df_content = dedent("""\
             FROM fedora
             LABEL label={0}""".format(NON_ASCII))
         df_lines = ["FROM fedora\n", "LABEL label={0}".format(NON_ASCII)]
 
@@ -308,14 +306,19 @@
         assert dfparser.labels == {'eggs': 'bacon❤'}
 
     def test_get_baseimg_from_df(self, dfparser):
         dfparser.lines = ["From fedora:latest\n",
                           "LABEL a b\n"]
         assert dfparser.baseimage == 'fedora:latest'
 
+    def test_get_baseimg_from_df_with_platform(self, dfparser):
+        dfparser.lines = ["From --platform=linux/amd64 fedora:latest\n",
+                          "LABEL a b\n"]
+        assert dfparser.baseimage == 'fedora:latest'
+
     def test_get_baseimg_from_arg(self, dfparser):
         dfparser.lines = ["ARG BASE=fedora:latest\n",
                           "FROM $BASE\n",
                           "LABEL a b\n"]
         assert dfparser.baseimage == 'fedora:latest'
 
     def test_get_baseimg_from_build_arg(self, tmpdir):
@@ -902,18 +905,18 @@
         dfparser.lines = ["FROM fedora\n",
                           "{0} V=v\n".format(instruction),
                           "LABEL TEST={0}\n".format(label)]
         assert dfparser.labels['TEST'] == expected
 
     def test_path_and_fileobj_together(self):
         with pytest.raises(ValueError):
-            DockerfileParser(path='.', fileobj=six.StringIO())
+            DockerfileParser(path='.', fileobj=io.StringIO())
 
     def test_nonseekable_fileobj(self):
-        with pytest.raises(AttributeError):
+        with pytest.raises((AttributeError, io.UnsupportedOperation)):
             DockerfileParser(fileobj=sys.stdin)
 
     def test_context_structure_per_line(self, dfparser, instruction):
         dfparser.content = dedent("""\
             FROM fedora:25
 
             {0} multi.label❤1="value❤1" \\
```

