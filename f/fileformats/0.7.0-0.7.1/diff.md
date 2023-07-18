# Comparing `tmp/fileformats-0.7.0.tar.gz` & `tmp/fileformats-0.7.1.tar.gz`

## Comparing `fileformats-0.7.0.tar` & `fileformats-0.7.1.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/archive/__init__.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/audio/__init__.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/_version.py
--rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/converter.py
--rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/datatype.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/exceptions.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/field.py
--rw-r--r--   0        0        0    42563 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/fileset.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/mark.py
--rw-r--r--   0        0        0    24544 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/mixin.py
--rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/utils.py
--rw-r--r--   0        0        0     8172 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/tests/test_classifiers.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/tests/test_converter.py
--rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/tests/test_detection.py
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/tests/test_general.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/tests/test_mime.py
--rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/tests/test_mixin.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/tests/test_subpackages.py
--rw-r--r--   0        0        0    11427 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/tests/test_utils.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/document/__init__.py
--rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/field/__init__.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/field/tests/test_fields.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/field/tests/test_fields_mime.py
--rw-r--r--   0        0        0     8335 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/generic/__init__.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/image/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/image/base.py
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/image/raster.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/image/vector.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/image/tests/test_image_raster.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/misc/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/misc/medical.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/numeric/__init__.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/serialization/__init__.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/testing/__init__.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/testing/basic.py
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/testing/classifiers.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/testing/headers.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/text/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/video/__init__.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.7.0/.gitignore
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.7.0/AUTHORS
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.7.0/LICENSE
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 fileformats-0.7.0/README.rst
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 fileformats-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    22316 2020-02-02 00:00:00.000000 fileformats-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/archive/__init__.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/audio/__init__.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/core/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/core/_version.py
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/core/converter.py
+-rw-r--r--   0        0        0    10609 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/core/datatype.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/core/exceptions.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/core/field.py
+-rw-r--r--   0        0        0    44247 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/core/fileset.py
+-rw-r--r--   0        0        0     6126 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/core/mark.py
+-rw-r--r--   0        0        0    24544 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/core/mixin.py
+-rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/core/utils.py
+-rw-r--r--   0        0        0     8172 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/core/tests/test_classifiers.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/core/tests/test_converter.py
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/core/tests/test_detection.py
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/core/tests/test_general.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/core/tests/test_mime.py
+-rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/core/tests/test_mixin.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/core/tests/test_subpackages.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/core/tests/test_test_extras.py
+-rw-r--r--   0        0        0    11427 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/core/tests/test_utils.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/document/__init__.py
+-rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/field/__init__.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/field/tests/test_fields.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/field/tests/test_fields_mime.py
+-rw-r--r--   0        0        0     7965 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/generic/__init__.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/image/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/image/base.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/image/raster.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/image/vector.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/image/tests/test_image_raster.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/misc/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/misc/medical.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/numeric/__init__.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/serialization/__init__.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/testing/__init__.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/testing/basic.py
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/testing/classifiers.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/testing/headers.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/text/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 fileformats-0.7.1/fileformats/video/__init__.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.7.1/.gitignore
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.7.1/AUTHORS
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.7.1/LICENSE
+-rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 fileformats-0.7.1/README.rst
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 fileformats-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0    22348 2020-02-02 00:00:00.000000 fileformats-0.7.1/PKG-INFO
```

### Comparing `fileformats-0.7.0/fileformats/archive/__init__.py` & `fileformats-0.7.1/fileformats/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.0/fileformats/audio/__init__.py` & `fileformats-0.7.1/fileformats/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.0/fileformats/core/converter.py` & `fileformats-0.7.1/fileformats/core/converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.0/fileformats/core/datatype.py` & `fileformats-0.7.1/fileformats/core/datatype.py`

 * *Files 4% similar despite different names*

```diff
@@ -269,10 +269,13 @@
                 for f in FileSet.all_formats
                 if getattr(f, "generically_qualifies", False)
             }
         return cls._generically_qualifies_by_name
 
     _generically_qualifies_by_name = None  # Register all generically classified types
 
+    REQUIRED_ANNOTATION = "__fileformats_required__"
+    CHECK_ANNOTATION = "__fileformats_check__"
+
 
 from .fileset import FileSet  # noqa
 from .field import Field  # noqa
```

### Comparing `fileformats-0.7.0/fileformats/core/field.py` & `fileformats-0.7.1/fileformats/core/field.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.0/fileformats/core/fileset.py` & `fileformats-0.7.1/fileformats/core/fileset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 from __future__ import annotations
 import os
 from copy import copy
 import struct
 from enum import Enum, IntEnum
 from warnings import warn
+import tempfile
 from collections import Counter
-import traceback
 import typing as ty
-import importlib
 import shutil
 from operator import itemgetter
 import itertools
 import functools
 from pathlib import Path
 import hashlib
 import logging
 import attrs
 from .utils import (
     classproperty,
     fspaths_converter,
     to_mime_format_name,
     STANDARD_NAMESPACES,
     describe_task,
+    import_extras_module,
 )
 from .converter import SubtypeVar
 from .exceptions import (
     FileFormatsError,
     FormatMismatchError,
     FormatConversionError,
 )
 from .datatype import DataType
+from . import mark
+
+try:
+    from typing import Self
+except ImportError:
+    from typing_extensions import Self
 
-# Tools imported from Arcana, will remove again once file-formats and "cells"
-# have been split
-REQUIRED_ANNOTATION = "__fileformats_required__"
-CHECK_ANNOTATION = "__fileformats_check__"
 
 FILE_CHUNK_LEN_DEFAULT = 8192
 
 
 logger = logging.getLogger("fileformats")
 
 
@@ -55,21 +57,14 @@
     fspaths : set[Path]
         a set of file-system paths pointing to all the resources in the file-set
     checks : bool
         whether to run in-depth "checks" to verify the file format
     """
 
     fspaths: ty.FrozenSet[Path] = attrs.field(default=None, converter=fspaths_converter)
-    _metadata: ty.Dict[str, ty.Any] = attrs.field(
-        default=None,
-        init=False,
-        repr=False,
-        eq=False,
-        hash=False,
-    )
 
     # Explicitly set the Internet Assigned Numbers Authority (https://iana_mime.org) MIME
     # type to None for any base classes that should not correspond to a MIME or MIME-like
     # type.
     iana_mime = None
     ext = ""
 
@@ -118,17 +113,19 @@
                     f"\n\nFiles in the present parent directory '{str(parent)}' are:\n"
                 )
                 msg += "\n".join(str(p) for p in parent.iterdir())
             raise FileNotFoundError(msg)
 
     @property
     def metadata(self):
-        if self._metadata is None and hasattr(self, "load_metadata"):
-            self._metadata = self.load_metadata()
-        return self._metadata
+        return self.load_metadata()
+
+    @mark.extra
+    def load_metadata(self):
+        raise NotImplementedError
 
     @property
     def parent(self) -> Path:
         "A common parent directory for all the top-level paths in the file-set"
         return Path(os.path.commonpath(p.parent for p in self.fspaths))
 
     @property
@@ -172,15 +169,15 @@
         fileset_props = dir(FileSet)
         for attr_name in dir(cls):
             if attr_name in fileset_props:
                 continue
             klass_attr = getattr(cls, attr_name)
             if isinstance(klass_attr, property):
                 try:
-                    klass_attr.fget.__annotations__[REQUIRED_ANNOTATION]
+                    klass_attr.fget.__annotations__[cls.REQUIRED_ANNOTATION]
                 except KeyError:
                     pass
                 else:
                     yield attr_name
 
     def required_paths(self) -> ty.Set[Path]:
         """Returns all fspaths that are required for the format"""
@@ -235,15 +232,15 @@
         # Loop through all attributes and find methods marked by CHECK_ANNOTATION
         fileset_props = dir(FileSet)
         for attr_name in dir(cls):
             if attr_name in fileset_props:
                 continue
             klass_attr = getattr(cls, attr_name)
             try:
-                klass_attr.__annotations__[CHECK_ANNOTATION]
+                klass_attr.__annotations__[cls.CHECK_ANNOTATION]
             except (AttributeError, KeyError):
                 pass
             else:
                 yield attr_name
 
     def select_by_ext(
         self, fileformat: ty.Optional[type] = None, allow_none: bool = False
@@ -374,22 +371,20 @@
             ambiguous (i.e. more than one) converters found between source and dest format
         """
         if source_format.issubtype(cls):
             return None
         converters = (
             cls.get_converters_dict()
         )  # triggers loading of standard converters for target format
-        # Ensure standard converters from source format are loaded
-        source_format.import_standard_converters()
         try:
             unclassified = source_format.unclassified
         except AttributeError:
-            pass
+            import_extras_module(source_format)
         else:
-            unclassified.import_standard_converters()
+            import_extras_module(unclassified)
         try:
             converter_tuple = converters[source_format]
         except KeyError:
             # If no direct mapping check for mapping from source super types and wildcard
             # matches
             available_converters = cls.get_converter_tuples(source_format)
             if len(available_converters) > 1:
@@ -397,18 +392,26 @@
                     describe_task(a[0]) for a in available_converters
                 )
                 raise FormatConversionError(
                     f"Ambiguous converters found between '{cls.mime_like}' and "
                     f"'{source_format.mime_like}':\n{available_str}"
                 ) from None
             elif not available_converters:
-                raise FormatConversionError(
+                msg = (
                     f"Could not find converter between '{source_format.mime_like}' and "
                     f"'{cls.mime_like}' formats"
-                ) from None
+                )
+                extras_imported, sub_pkg = import_extras_module(cls)
+                if not extras_imported:
+                    msg += (
+                        f'. Was not able to import "extras" module, fileformats.extras.{sub_pkg}, '
+                        f"you may want to try installing the 'fileformats-{sub_pkg}-extras' package "
+                        f"from PyPI (e.g. pip install fileformats-{sub_pkg}-extras)"
+                    )
+                raise FormatConversionError(msg) from None
             converter_tuple = available_converters[0]
             # Store mapping for future reference
             converters[source_format] = converter_tuple
         converter, conv_kwargs = converter_tuple
         if kwargs:
             # Merge kwargs provided to get_conveter with stored kwargs
             conv_kwargs = copy(conv_kwargs)
@@ -417,45 +420,24 @@
 
     @classmethod
     def get_converters_dict(cls, klass=None):
         # Only access converters to the specific class, not superclasses (which may not
         # be able to convert to the specific type)
         if klass is None:
             klass = cls
+        # import related extras module for the target class
+        import_extras_module(klass)
         try:
             converters_dict = klass.__dict__["converters"]
         except KeyError:
             converters_dict = {}
             klass.converters = converters_dict
-            klass.import_standard_converters()
         return converters_dict
 
     @classmethod
-    def import_standard_converters(cls):
-        """Attempts to import standard converters for the format class, which are
-        located at `fileformats.<namespace>.converters`
-        """
-        standard_converters_module = f"fileformats.{cls.namespace}.converters"
-        try:
-            importlib.import_module(standard_converters_module)
-        except ImportError as e:
-            if str(e) != f"No module named '{standard_converters_module}'":
-                if cls.namespace in STANDARD_NAMESPACES:
-                    pkg = "fileformats"
-                else:
-                    pkg = f"fileformats-{cls.namespace}"
-                warn(
-                    f"Could not import standard converters for '{cls.namespace}' namespace, "
-                    f"please install '{pkg}' with the 'extended' install option to "
-                    f"use converters for {cls.namespace}, i.e.\n\n"
-                    f"    $ python3 -m pip install '{pkg}[extended]':\n\n"
-                    f"Import error was:\n{traceback.format_exc()}"
-                )
-
-    @classmethod
     def get_converter_tuples(
         cls, source_format: type
     ) -> ty.List[ty.Tuple[ty.Callable, ty.Dict[str, ty.Any]]]:
         """Search the registered converters to find any matches and return list of
         task and associated key-word args to perform the conversion between source and
         target formats
 
@@ -741,22 +723,87 @@
         """
         cls = type(self)
         yield f"{cls.__module__}.{cls.__name__}:".encode()
         for key, chunk_iter in self.byte_chunks():
             yield (",'" + key + "'=").encode()
             yield from chunk_iter
 
+    @classmethod
+    def mock(cls, *fspaths: ty.Tuple[ty.Union[Path, str]]) -> Self:
+        """Return an instance of a mocked sub-class of the file format to be used in
+        test routines like doctests.
+
+        Parameters
+        ----------
+        *fspaths: tuple[Path]
+            the paths to be provided to the mocked class, by default will be ["mock/<class-name-lower>"]
+
+        Returns
+        -------
+        FileSet
+            a file-set that will pass type-checking as an instance of the given
+            fileset class but which doesn't actually point to any FS objects.
+        """
+        mock_cls = type(cls.__name__ + "Mock", (MockMixin, cls), {})
+        if not fspaths:
+            fspaths = []
+            fspath = f"/mock/{cls.__name__.lower()}"
+            try:
+                fspath += cls.ext
+            except AttributeError:
+                pass
+            fspaths.append(fspath)
+        return mock_cls(fspaths=fspaths)
+
+    @classmethod
+    def arbitrary(cls, dest_dir: ty.Optional[Path] = None) -> Self:
+        """Return an arbitrary instance of the file-set type for classes where the
+        `test_data` extra has been implemented
+
+        Parameters
+        ----------
+        dest_dir : Path, optional
+            the path in which to create the test data
+
+        Returns
+        -------
+        FileSet
+            an instance of the given file-set class
+        """
+        if not dest_dir:
+            dest_dir = Path(tempfile.mkdtemp())
+        # Need to use mock to get an instance in order to use the singledispatch-based
+        # mark.extra decorator
+        mock = cls.mock()
+        return cls(mock.generate_test_data(dest_dir))
+
+    @mark.extra
+    def generate_test_data(self, dest_dir: Path) -> ty.Iterable[Path]:
+        """Generate test data at the fspaths of the file-set
+
+        Parameters
+        ----------
+        dest_dir : Path
+            the directory to generate the test data within
+
+        Returns
+        -------
+        fspaths : ty.Iterable
+            the generated fspaths
+        """
+        raise NotImplementedError
+
     class ExtensionDecomposition(IntEnum):
         """What to consider the file extension to be for paths without an explicitly
         defined extension
 
         Options
         -------
         none
-            assume it doesn't have a file extension
+            assume it doesn't have a file extension, i.e. all parts are included in the stem
         single
             assume that anything after the last '.' is the extension, e.g. the extension
             of "file.nii.gz" would be ".gz"
         multiple
             assume that anything after the first '.' is the extension, e.g. the extension
             of "file.nii.gz" would be "nii.gz"
         """
@@ -1114,7 +1161,23 @@
         """For b/w compatibility (temporary message)"""
         warn("'FileSet.copy_to()' has been deprecated, please use copy() instead")
         return self.copy(*args, **kwargs)
 
     _all_formats = None
     _formats_by_iana_mime = None
     _formats_by_name = None
+
+
+@attrs.define(slots=False)
+class MockMixin:
+    """Strips out validation methods of a class, allowing it to be mocked in a way that
+    still satisfies type-checking"""
+
+    # Mirror fspaths here so we can unset its validator
+    fspaths: ty.FrozenSet[Path] = attrs.field(default=None, converter=fspaths_converter)
+
+    def __attrs_post_init__(self):
+        pass
+
+    @fspaths.validator
+    def validate_fspaths(self, _, fspaths):
+        pass
```

### Comparing `fileformats-0.7.0/fileformats/core/mixin.py` & `fileformats-0.7.1/fileformats/core/mixin.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.0/fileformats/core/utils.py` & `fileformats-0.7.1/fileformats/core/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 import importlib
 from pathlib import Path
 import inspect
 import typing as ty
 import re
+import urllib.request
+import urllib.error
 import os
 import logging
 import pkgutil
 from contextlib import contextmanager
 from fileformats.core.exceptions import (
     MissingExtendedDepenciesError,
     FileFormatsError,
@@ -238,7 +240,66 @@
     if inspect.isfunction(task):
         import cloudpickle
 
         task = cloudpickle.loads(task().inputs._func)
     src_file = inspect.getsourcefile(task)
     src_line = inspect.getsourcelines(task)[-1]
     return f"{task} (defined at line {src_line} of {src_file})"
+
+
+def check_package_exists_on_pypi(package_name: str) -> bool:
+    """Check if a package exists on PyPI
+
+    Parameters
+    ----------
+    package_name : str
+        the name of the package to check for
+
+    Returns
+    -------
+    bool
+        whether the package exists on PyPI or not
+    """
+    url = f"https://pypi.org/pypi/{package_name}/json"
+    try:
+        urllib.request.urlopen(url)
+    except urllib.error.HTTPError as e:
+        if e.code == 404:
+            return False
+        else:
+            raise
+    return True
+
+
+def import_extras_module(klass: type) -> ty.Tuple[bool, str]:
+    """Attempt to load extras module corresponding to the provided class's module
+
+    Parameters
+    ----------
+    klass : ty.Type
+        the class to load the extras module for
+
+    Returns
+    -------
+    imported : bool
+        whether the module was imported or not
+    sub_pkg : str
+        the name of the sub-package that was attempted to be loaded
+    """
+
+    pkg_parts = klass.__module__.split(".")
+    if pkg_parts[0] != "fileformats":
+        logger.debug(
+            "There is no 'extras' module for classes not within the 'fileformats' package, "
+            "not %s in %s",
+            klass.__name__,
+            klass.__module__,
+        )
+        return True, None
+    sub_pkg = pkg_parts[1]
+    try:
+        importlib.import_module("fileformats.extras." + sub_pkg)
+    except ImportError:
+        extras_imported = False
+    else:
+        extras_imported = True
+    return extras_imported, sub_pkg
```

### Comparing `fileformats-0.7.0/fileformats/core/tests/test_classifiers.py` & `fileformats-0.7.1/fileformats/core/tests/test_classifiers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.0/fileformats/core/tests/test_converter.py` & `fileformats-0.7.1/fileformats/core/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.0/fileformats/core/tests/test_detection.py` & `fileformats-0.7.1/fileformats/core/tests/test_detection.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.0/fileformats/core/tests/test_general.py` & `fileformats-0.7.1/fileformats/core/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.0/fileformats/core/tests/test_mime.py` & `fileformats-0.7.1/fileformats/core/tests/test_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.0/fileformats/core/tests/test_mixin.py` & `fileformats-0.7.1/fileformats/core/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.0/fileformats/core/tests/test_subpackages.py` & `fileformats-0.7.1/fileformats/core/tests/test_subpackages.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.0/fileformats/core/tests/test_utils.py` & `fileformats-0.7.1/fileformats/core/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.0/fileformats/document/__init__.py` & `fileformats-0.7.1/fileformats/document/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.0/fileformats/field/__init__.py` & `fileformats-0.7.1/fileformats/field/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.0/fileformats/field/tests/test_fields.py` & `fileformats-0.7.1/fileformats/field/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.0/fileformats/field/tests/test_fields_mime.py` & `fileformats-0.7.1/fileformats/field/tests/test_fields_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.0/fileformats/generic/__init__.py` & `fileformats-0.7.1/fileformats/generic/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import typing as ty
 from pathlib import Path
 import attrs
 from fileformats.core.fileset import FileSet
 from fileformats.core.exceptions import FormatMismatchError, FileFormatsError
 from fileformats.core import mark
 from fileformats.core.utils import classproperty
 from fileformats.core.mixin import WithClassifiers
@@ -40,29 +41,20 @@
     binary = False
     is_dir = False
 
     @mark.required
     @property
     def fspath(self):
         fspath = self.select_by_ext()
-        if not fspath.is_file():
-            if not fspath.exists():
-                msg = (
-                    f"Selected fspath for {type(self)}, '{str(fspath)}', does not exist"
-                )
-                if fspath.parent.exists():
-                    neighbours = [p.name for p in fspath.parent.iterdir()]
-                    msg += f". Found neighbouring files {neighbours}"
-                raise FileFormatsError(msg)
-            else:
-                msg = ", it is a directory" if fspath.is_dir() else ""
-                raise FormatMismatchError(
-                    f'Path that matches extension of "{type(self)}", {fspath}, is not a '
-                    "file in {repr(self)}" + msg
-                )
+        if fspath.is_dir():
+            # fspath is guaranteed to exist
+            raise FormatMismatchError(
+                f'Path that matches extension of {type(self)}, "{fspath}", '
+                f"is a directory not a file"
+            )
         return fspath
 
     @classmethod
     def copy_ext(
         cls,
         old_path: Path,
         new_path: Path,
@@ -147,15 +139,16 @@
     is_dir = True
 
     content_types = ()
 
     @mark.required
     @property
     def fspath(self):
-        dirs = [p for p in self.fspaths if p.is_dir()]
+        # fspaths are checked for existence with the exception of mock classes
+        dirs = [p for p in self.fspaths if not p.is_file()]
         if not dirs:
             raise FormatMismatchError(f"No directory paths provided {repr(self)}")
         if len(dirs) > 1:
             raise FormatMismatchError(
                 f"More than one directory path provided {dirs} to {repr(self)}"
             )
         fspath = dirs[0]
```

### Comparing `fileformats-0.7.0/fileformats/image/raster.py` & `fileformats-0.7.1/fileformats/image/raster.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from fileformats.core.mixin import WithMagicNumber
-from fileformats.core import mark, MissingExtendedDependency
+from fileformats.core import mark
 from fileformats.core.exceptions import FormatMismatchError
 from .base import Image
 
-try:
-    import imageio
-except ImportError:
-    imageio = MissingExtendedDependency("imageio", __name__)
-
 
 class RasterImage(Image):
     iana_mime = None
     binary = True
 
-    def load(self):
-        return imageio.imread(self.fspath)
+    @mark.extra
+    def read_data(self):
+        raise NotImplementedError
+
+    @mark.extra
+    def write_data(self, data_array):
+        raise NotImplementedError
 
     @classmethod
     def save_new(cls, fspath, data_array):
-        imageio.imwrite(fspath, data_array)
+        # We have to use a mock object as the data file hasn't been written yet
+        mock = cls.mock(fspath)
+        mock.write_data(data_array)
         return cls(fspath)
 
 
 class Bitmap(WithMagicNumber, RasterImage):
     ext = ".bmp"
     magic_number = b"BM"
     iana_mime = "image/bmp"
```

### Comparing `fileformats-0.7.0/fileformats/image/tests/test_image_raster.py` & `fileformats-0.7.1/fileformats/image/tests/test_image_raster.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 
 @pytest.fixture(scope="session")
 def png_path():
     return get_remote_file("images/chelsea.png")
 
 
-@pytest.mark.xfail(reason="No converter between PNG and tiff")
 def test_tiff_endianness(png_path):
     png = Png(png_path)
     Tiff.convert(png)
 
 
 def test_tiff_fail(png_path, work_dir):
     bad_tiff_path = work_dir / "bad_tiff.tiff"
```

### Comparing `fileformats-0.7.0/fileformats/serialization/__init__.py` & `fileformats-0.7.1/fileformats/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.0/fileformats/testing/classifiers.py` & `fileformats-0.7.1/fileformats/testing/classifiers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.0/fileformats/testing/headers.py` & `fileformats-0.7.1/fileformats/testing/headers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.0/fileformats/text/__init__.py` & `fileformats-0.7.1/fileformats/text/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.0/LICENSE` & `fileformats-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.0/README.rst` & `fileformats-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats-0.7.0/pyproject.toml` & `fileformats-0.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fileformats"
 description = "Classes for representing different file formats in Python classes for use in type hinting in data workflows"
 readme = "README.rst"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
     "attrs>=22.1.0",
+    "typing_extensions >=4.6.3; python_version < '3.11'"
 ]
 license = {file = "LICENSE"}
 authors = [
     {name = "Thomas G. Close", email = "tom.g.close@gmail.com"},
 ]
 maintainers = [
     {name = "Thomas G. Close", email = "tom.g.close@gmail.com"},
@@ -51,16 +52,15 @@
     "flake8-pyproject",
     "fileformats[test]",
 ]
 test = [
     "pytest >=6.2.5",
     "pytest-env>=0.6.2",
     "pytest-cov>=2.12.1",
-    "imageio",
-    "pydra >=0.22",
+    "fileformats-extras",
 ]
 docs = [
     "packaging",
     "docutils>=0.10",
     "mock>1.0",
     "sphinx >=2.1.2",
     "sphinx-argparse>=0.2.0",
```

### Comparing `fileformats-0.7.0/PKG-INFO` & `fileformats-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileformats
-Version: 0.7.0
+Version: 0.7.1
 Summary: Classes for representing different file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
         
@@ -108,16 +108,17 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: attrs>=22.1.0
+Requires-Dist: typing-extensions>=4.6.3; python_version < '3.11'
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: codespell; extra == 'dev'
 Requires-Dist: fileformats[test]; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
 Requires-Dist: flake8-pyproject; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
@@ -127,16 +128,15 @@
 Requires-Dist: mock>1.0; extra == 'docs'
 Requires-Dist: numpydoc>=0.6.0; extra == 'docs'
 Requires-Dist: packaging; extra == 'docs'
 Requires-Dist: sphinx-argparse>=0.2.0; extra == 'docs'
 Requires-Dist: sphinx-click>=3.1; extra == 'docs'
 Requires-Dist: sphinx>=2.1.2; extra == 'docs'
 Provides-Extra: test
-Requires-Dist: imageio; extra == 'test'
-Requires-Dist: pydra>=0.22; extra == 'test'
+Requires-Dist: fileformats-extras; extra == 'test'
 Requires-Dist: pytest-cov>=2.12.1; extra == 'test'
 Requires-Dist: pytest-env>=0.6.2; extra == 'test'
 Requires-Dist: pytest>=6.2.5; extra == 'test'
 Description-Content-Type: text/x-rst
 
 FileFormats
 ===========
```

