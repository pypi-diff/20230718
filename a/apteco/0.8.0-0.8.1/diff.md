# Comparing `tmp/apteco-0.8.0.tar.gz` & `tmp/apteco-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apteco-0.8.0.tar", last modified: Tue May 25 13:39:23 2021, max compression
+gzip compressed data, was "apteco-0.8.1.tar", max compression
```

## Comparing `apteco-0.8.0.tar` & `apteco-0.8.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0    18219 2021-05-25 13:39:22.876665 apteco-0.8.0/docs/source/readme.rst
--rw-r--r--   0        0        0    11556 2019-06-24 15:29:29.422000 apteco-0.8.0/LICENSE
--rw-r--r--   0        0        0     1397 2021-05-25 13:34:08.140444 apteco-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      216 2021-05-25 13:34:08.140444 apteco-0.8.0/src/apteco/__init__.py
--rw-r--r--   0        0        0      338 2021-05-17 16:09:18.069547 apteco-0.8.0/src/apteco/common.py
--rw-r--r--   0        0        0    11858 2021-05-14 12:26:02.310463 apteco-0.8.0/src/apteco/cube.py
--rw-r--r--   0        0        0     9914 2021-02-28 00:48:24.467001 apteco-0.8.0/src/apteco/data/apteco_logo.py
--rw-r--r--   0        0        0     4348 2021-02-28 00:48:52.174023 apteco-0.8.0/src/apteco/datagrid.py
--rw-r--r--   0        0        0     1472 2020-11-01 22:22:57.610696 apteco-0.8.0/src/apteco/exceptions.py
--rw-r--r--   0        0        0    45925 2021-05-04 13:15:29.027874 apteco-0.8.0/src/apteco/query.py
--rw-r--r--   0        0        0    25159 2021-02-28 12:22:42.978091 apteco-0.8.0/src/apteco/session.py
--rw-r--r--   0        0        0     3321 2021-05-17 15:05:20.804033 apteco-0.8.0/src/apteco/statistics.py
--rw-r--r--   0        0        0     8561 2021-01-21 13:54:27.988640 apteco-0.8.0/src/apteco/tables.py
--rw-r--r--   0        0        0    18444 2021-05-14 12:26:02.322996 apteco-0.8.0/src/apteco/variables.py
--rw-r--r--   0        0        0    19098 2021-05-25 13:39:23.566615 apteco-0.8.0/setup.py
--rw-r--r--   0        0        0    18751 2021-05-25 13:39:23.568609 apteco-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    18219 2023-07-18 09:47:39.975657 apteco-0.8.1/docs/source/readme.rst
+-rw-r--r--   0        0        0    11556 2019-06-24 15:29:29.422000 apteco-0.8.1/LICENSE
+-rw-r--r--   0        0        0     1505 2023-07-18 09:46:43.433214 apteco-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      216 2023-07-18 09:46:43.437214 apteco-0.8.1/src/apteco/__init__.py
+-rw-r--r--   0        0        0      338 2021-05-17 16:09:18.069547 apteco-0.8.1/src/apteco/common.py
+-rw-r--r--   0        0        0    11858 2021-05-14 12:26:02.310463 apteco-0.8.1/src/apteco/cube.py
+-rw-r--r--   0        0        0     9914 2021-02-28 00:48:24.467001 apteco-0.8.1/src/apteco/data/apteco_logo.py
+-rw-r--r--   0        0        0     4348 2021-02-28 00:48:52.174023 apteco-0.8.1/src/apteco/datagrid.py
+-rw-r--r--   0        0        0     1472 2020-11-01 22:22:57.610696 apteco-0.8.1/src/apteco/exceptions.py
+-rw-r--r--   0        0        0    46099 2022-01-26 17:41:09.465700 apteco-0.8.1/src/apteco/query.py
+-rw-r--r--   0        0        0    25159 2023-06-30 13:02:13.179172 apteco-0.8.1/src/apteco/session.py
+-rw-r--r--   0        0        0     3321 2021-05-17 15:05:20.804033 apteco-0.8.1/src/apteco/statistics.py
+-rw-r--r--   0        0        0     8561 2021-01-21 13:54:27.988640 apteco-0.8.1/src/apteco/tables.py
+-rw-r--r--   0        0        0    18444 2021-05-14 12:26:02.322996 apteco-0.8.1/src/apteco/variables.py
+-rw-r--r--   0        0        0    18853 1970-01-01 00:00:00.000000 apteco-0.8.1/PKG-INFO
```

### Comparing `apteco-0.8.0/docs/source/readme.rst` & `apteco-0.8.1/docs/source/readme.rst`

 * *Files identical despite different names*

### Comparing `apteco-0.8.0/LICENSE` & `apteco-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `apteco-0.8.0/pyproject.toml` & `apteco-0.8.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apteco"
-version = "0.8.0"
+version = "0.8.1"
 description = "A Python package for interacting with Apteco Marketing Suite resources via the Apteco API."
 authors = ["Apteco Ltd <support@apteco.com>"]
 license = "Apache-2.0"
 readme = "docs/source/readme.rst"
 homepage = "https://help.apteco.com/python/index.html"
 repository = "https://github.com/Apteco/py-apteco"
 keywords = ["Apteco", "FastStats", "Orbit", "API", "Marketing"]
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.6.1"  # pandas 1.0 requires >=3.6.1, see: https://github.com/pandas-dev/pandas/pull/29212#issuecomment-551370118
-apteco-api = "^0.2.1"
+apteco-api = "^0.3.1"
 pysimplegui = "^4.0"
 pandas = "^1.0"
 numpy = "^1.18"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.0"
 isort = "^4.3"
@@ -33,10 +33,15 @@
 sphinx = "^2.1"
 sphinx_rtd_theme = "^0.4.3"
 pytest-cov = "^2.8"
 pytest-cases = "^2.0.4"
 twine = "^3.2.0"
 bump2version = "^1.0.1"
 
+[[tool.poetry.source]]
+name = "test-pypi"
+url = "https://test.pypi.org/simple/"
+priority = "explicit"
+
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `apteco-0.8.0/src/apteco/cube.py` & `apteco-0.8.1/src/apteco/cube.py`

 * *Files identical despite different names*

### Comparing `apteco-0.8.0/src/apteco/data/apteco_logo.py` & `apteco-0.8.1/src/apteco/data/apteco_logo.py`

 * *Files identical despite different names*

### Comparing `apteco-0.8.0/src/apteco/datagrid.py` & `apteco-0.8.1/src/apteco/datagrid.py`

 * *Files identical despite different names*

### Comparing `apteco-0.8.0/src/apteco/exceptions.py` & `apteco-0.8.1/src/apteco/exceptions.py`

 * *Files identical despite different names*

### Comparing `apteco-0.8.0/src/apteco/query.py` & `apteco-0.8.1/src/apteco/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections.abc import Sequence
 from datetime import date, datetime
 from decimal import Decimal
 from fractions import Fraction
 from numbers import Integral, Number, Rational, Real
 from typing import Iterable, List, Optional
 
 import apteco_api as aa
@@ -234,14 +235,101 @@
         return [normalize_datetime_value(input_value, error_msg)]
     elif isinstance(input_value, Iterable) and not isinstance(input_value, str):
         return [normalize_datetime_value(v, error_msg) for v in input_value]
     else:
         raise ValueError(error_msg)
 
 
+def validate_n_frac_input(n, frac, allow_range=False):
+    if sum((i is not None) for i in (n, frac)) != 1:
+        raise ValueError("Must specify either n or frac")
+    total = None
+    percent = None
+    fraction = None
+
+    if n is not None:
+        kind, total = validate_numerical_input(n, Integral, int, "n", "an integer greater than 0", 0, None, allow_range, "an integer or a tuple of two integers (to indicate a range)")
+    else:
+        try:
+            kind, fraction = validate_numerical_input(frac, Rational, rational_to_fraction, "frac", "a rational number between 0 and 1", 0, 1, allow_range, "a ration number or a tuple of two rational numbers (to indicate a range)")
+        except ValueError:  # if we fail, maybe it's still Real
+            kind, percent = validate_numerical_input(frac, Real, float, "frac", "a number between 0 and 1", 0, 1, allow_range, "a number or a tuple of two numbers (to indicate a range)")
+            if kind == "range":
+                percent = (percent[0] * 100, percent[1] * 100)
+            else:
+                percent *= 100
+    return total, percent, fraction
+
+
+def validate_total_percent_input(total, percent):
+    if total is not None:
+        if percent is not None:
+            raise ValueError("Must specify either total or percent, but not both")
+        single_or_range, total = validate_numerical_input(total, Integral, int, "total", "an integer", 0, None, True, "an integer or a tuple of two integers (to indicate a range)")
+        kind = (single_or_range, "total")
+    elif percent is not None:
+        single_or_range, percent = validate_numerical_input(percent, Real, float, "percent", "a percentage", 0, 100, True, "a number or a tuple of two numbers (to indicate a range)")
+        kind = (single_or_range, "percent")
+    else:
+        raise ValueError("Must specify one of total or percent")
+    return kind, total, percent
+
+
+def rational_to_fraction(frac):
+    return Fraction(frac.numerator, frac.denominator)
+
+
+def validate_numerical_input(value, abstract_class, concrete_class, metavar, valid_text, lower_bound=None, upper_bound=None, allow_range=False, valid_range_text=None):
+    if allow_range and isinstance(value, Sequence) and not isinstance(value, str):
+        final_valid_text = valid_range_text
+        kind = "range"
+        validate_input = validate_range_input
+    elif isinstance(value, Number):
+        final_valid_text = valid_text
+        kind = "single"
+        validate_input = validate_single_input
+    else:
+        raise ValueError(f"{metavar} must be {valid_range_text if allow_range else valid_text}")
+    try:
+        return kind, validate_input(value, abstract_class, concrete_class, metavar, valid_text, lower_bound, upper_bound)
+    except TypeError:
+        raise ValueError(f"{metavar} must be {final_valid_text}") from None
+
+
+def validate_range_input(value, abstract_class, concrete_class, metavar, valid_text, lower_bound=None, upper_bound=None):
+    if not (isinstance(value, tuple) and len(value) == 2):
+        raise TypeError(f"{metavar} must be {valid_text}")
+    start, end = value
+
+    try:
+        start = validate_single_input(start, abstract_class, concrete_class, "start of range", valid_text, lower_bound, upper_bound)
+        end = validate_single_input(end, abstract_class, concrete_class, "end of range", valid_text, lower_bound, upper_bound)
+    except (TypeError, ValueError) as exc:
+        raise ValueError(f"Invalid range given for {metavar} - {exc.args[0]}")
+    if not start < end:
+        raise ValueError(f"Invalid range given for {metavar} - start of range must be less than end")
+
+    return start, end
+
+
+def validate_single_input(value, abstract_class, concrete_class, metavar, valid_text, lower_bound=None, upper_bound=None):
+    if not isinstance(value, abstract_class):
+        raise TypeError(f"{metavar} must be {valid_text}")
+    value = concrete_class(value)
+
+    if upper_bound is None and lower_bound is not None and not lower_bound < value:
+        raise ValueError(f"{metavar} must be greater than {lower_bound}")
+    if lower_bound is None and upper_bound is not None and not value < upper_bound:
+        raise ValueError(f"{metavar} must be less than {upper_bound}")
+    if lower_bound is not None and upper_bound is not None and not lower_bound < value < upper_bound:
+        raise ValueError(f"{metavar} must be between {lower_bound} and {upper_bound}")
+
+    return value
+
+
 class Clause:
     @property
     def table_name(self):
         return self.table.name
 
     def count(self):
         query_final = aa.Query(selection=self._to_model_selection())
@@ -349,39 +437,22 @@
             table=table if table is not None else self.table,
             session=self.session,
         )
 
     def sample(
         self, n=None, frac=None, sample_type="Random", skip_first=0, *, label=None
     ):
-        if sum((i is not None) for i in (n, frac)) != 1:
-            raise ValueError("Must specify either n or frac")
-        total = None
-        percent = None
-        fraction = None
-        if n is not None:
-            if not isinstance(n, Integral) or n < 1:
-                raise ValueError("n must be an integer greater than 0")
-            total = int(n)
-        else:
-            if not isinstance(frac, Real):
-                raise ValueError("frac must be either a float or a fraction")
-            if not 0 < float(frac) < 1:
-                raise ValueError("frac must be between 0 and 1")
-            if isinstance(frac, Rational):
-                fraction = Fraction(frac.numerator, frac.denominator)
-            else:
-                percent = float(frac) * 100
+        total, percent, fraction = validate_n_frac_input(n, frac)
 
         if sample_type.title() not in ("First", "Stratified", "Random"):
             raise ValueError(f"'{sample_type}' is not a valid sample type")
         sample_type = sample_type.title()
 
         if not isinstance(skip_first, Integral) or int(skip_first) < 0:
-            raise ValueError("`skip_first` must be a non-negative integer")
+            raise ValueError("skip_first must be a non-negative integer")
         skip_first = int(skip_first)
 
         return LimitClause(
             clause=self,
             total=total,
             percent=percent,
             fraction=fraction,
@@ -394,58 +465,59 @@
     def limit(
         self, n=None, frac=None, by=None, ascending=None, per=None, *, label=None
     ):
         if ascending is not None:
             if not isinstance(ascending, bool):
                 raise ValueError("ascending must be True or False")
             if by is None:
-                raise ValueError("Must specify by with ascending")
+                raise ValueError("Must specify `by` with ascending")
         else:
             ascending = False
-        # if by is not None and not isinstance(by, Variable):
-        #     raise ValueError("by must be a variable")
+        if by is not None and not hasattr(by, "is_selectable"):  # only vars have attr
+            raise ValueError("`by` must be an ordered variable")
+
         if per is not None:
             # nper
+            if n is None:
+                raise ValueError("Must specify `n` with `per`")
+            else:
+                __, total = validate_numerical_input(
+                    n, Integral, int, "n", "an integer greater than 0", 0
+                )
             try:
                 return per._as_nper_clause(
-                    clause=self, n=n, by=by, ascending=ascending, label=label
+                    clause=self, n=total, by=by, ascending=ascending, label=label
                 )
             except AttributeError:
                 raise ValueError("`per` must be a table or a variable") from None
-        if by is None:
-            # call.sample()
-            return self.sample(n=n, frac=frac, label=label)
-        # topn
-        if n is not None:
-            return TopNClause(
-                clause=self,
-                total=n,
-                percent=None,
-                by=by,
-                ascending=ascending,
-                label=label,
-                session=self.session,
-            )
-        if frac is not None:
-            if isinstance(frac, tuple):
-                percent = tuple(i * 100 for i in frac)
-            elif isinstance(frac, Real):
-                percent = frac * 100
-            else:
-                raise ValueError()
+
+        total, percent, fraction = validate_n_frac_input(n, frac, allow_range=True)
+
+        if by is not None:
+            # topn
             return TopNClause(
                 clause=self,
-                total=None,
-                percent=percent,
+                total=total,
+                percent=fraction * 100 if fraction else percent,
                 by=by,
                 ascending=ascending,
                 label=label,
                 session=self.session,
             )
-        raise ValueError()
+        # limit
+        return LimitClause(
+            clause=self,
+            total=total,
+            percent=percent,
+            fraction=fraction,
+            sample_type="Random",
+            skip_first=0,
+            label=label,
+            session=self.session,
+        )
 
 
 class SelectorClauseMixin:
     @staticmethod
     def _verify_values(values: Iterable[str], variable_name: str, session: "Session"):
         systems_controller = APIController(aa.FastStatsSystemsApi, session)
 
@@ -1053,101 +1125,28 @@
                 else None,
             ),
             table_name=self.table_name,
             name=self.label,
         )
 
 
-def ensure_single_or_range(
-    input_value,
-    type_,
-    convert,
-    number_text,
-    param_text,
-    lower_bound=None,
-    upper_bound=None,
-):
-
-    if isinstance(input_value, Iterable) and not isinstance(input_value, str):
-        if not (isinstance(input_value, tuple) and len(input_value) == 2):
-            raise ValueError(
-                f"Invalid range given for `{param_text}`"
-                f" - must be a tuple of two values."
-            )
-        try:
-            start, end = input_value
-            start = ensure_single(
-                start,
-                type_,
-                convert,
-                number_text,
-                f"start of range",
-                lower_bound,
-                upper_bound,
-            )
-            end = ensure_single(
-                end,
-                type_,
-                convert,
-                number_text,
-                f"end of range",
-                lower_bound,
-                upper_bound,
-            )
-        except ValueError as exc:
-            exc_msg = f"Invalid range given for `{param_text}` - {exc.args[0]}"
-            raise ValueError(exc_msg)
-        if not start < end:
-            raise ValueError(
-                f"Invalid range given for `{param_text}`"
-                f" - start of range must be less than the end."
-            )
-        return "range", (start, end)
-
-    return (
-        "single",
-        ensure_single(
-            input_value,
-            type_,
-            convert,
-            number_text,
-            f"`{param_text}`",
-            lower_bound,
-            upper_bound,
-        ),
-    )
-
-
-def ensure_single(
-    value, type_, convert, number_text, param_text, lower_bound=None, upper_bound=None
-):
-    if not isinstance(value, type_):
-        raise ValueError(f"{param_text} must be {number_text}")
-    value = convert(value)
-    if lower_bound is not None and not lower_bound < value:
-        raise ValueError(f"{param_text} must be greater than {lower_bound}")
-    if upper_bound is not None and not value < upper_bound:
-        raise ValueError(f"{param_text} must be less than {upper_bound}")
-    return value
-
-
 class TopNClause(BaseLimitClause):
     def __init__(
         self,
         clause,
         total=None,
         percent=None,
         by=None,
         ascending=False,
         *,
         label=None,
         session=None,
     ):
-        self.kind, self.total, self.percent = self._check_numerical_inputs(
-            percent, total
+        self.kind, self.total, self.percent = validate_total_percent_input(
+            total, percent
         )
 
         if by is None or not hasattr(by, "name"):
             raise ValueError("`by` must be an ordered variable")
         self.by = by
 
         if not isinstance(ascending, bool):
@@ -1156,51 +1155,14 @@
 
         self.clause = clause
         self.table = clause.table
 
         self.label = label
         self.session = session
 
-    @staticmethod
-    def _check_numerical_inputs(percent, total):
-        if total is not None:
-            if percent is not None:
-                raise ValueError(
-                    "Must specify either `total` or `percent`, but not both"
-                )
-            try:
-                single_or_range, total = ensure_single_or_range(
-                    total, Integral, int, "an integer", "total", lower_bound=0
-                )
-                kind = (single_or_range, "total")
-                return kind, total, None
-            except ValueError:
-                raise ValueError(
-                    "`total` must be an integer or a tuple of two integers (to indicate a range)"
-                ) from None
-        elif percent is not None:
-            try:
-                single_or_range, percent = ensure_single_or_range(
-                    percent,
-                    Real,
-                    float,
-                    "a percentage",
-                    "percent",
-                    lower_bound=0,
-                    upper_bound=100,
-                )
-                kind = (single_or_range, "percent")
-                return kind, None, percent
-            except ValueError:
-                raise ValueError(
-                    "`percent` must be a number or a tuple of two numbers (to indicate a range)"
-                )
-        else:
-            raise ValueError("Must specify one of `total` or `percent`")
-
     def _to_model_selection(self):
         if self.kind[0] == "single":
             if self.kind[1] == "total":
                 value = self.total
                 percent = "NaN"
             elif self.kind[1] == "percent":
                 value = 0
```

### Comparing `apteco-0.8.0/src/apteco/session.py` & `apteco-0.8.1/src/apteco/session.py`

 * *Files identical despite different names*

### Comparing `apteco-0.8.0/src/apteco/statistics.py` & `apteco-0.8.1/src/apteco/statistics.py`

 * *Files identical despite different names*

### Comparing `apteco-0.8.0/src/apteco/tables.py` & `apteco-0.8.1/src/apteco/tables.py`

 * *Files identical despite different names*

### Comparing `apteco-0.8.0/src/apteco/variables.py` & `apteco-0.8.1/src/apteco/variables.py`

 * *Files identical despite different names*

### Comparing `apteco-0.8.0/setup.py` & `apteco-0.8.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,514 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: apteco
+Version: 0.8.1
+Summary: A Python package for interacting with Apteco Marketing Suite resources via the Apteco API.
+Home-page: https://help.apteco.com/python/index.html
+License: Apache-2.0
+Keywords: Apteco,FastStats,Orbit,API,Marketing
+Author: Apteco Ltd
+Author-email: support@apteco.com
+Requires-Python: >=3.6.1,<4.0.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Requires-Dist: apteco-api (>=0.3.1,<0.4.0)
+Requires-Dist: numpy (>=1.18,<2.0)
+Requires-Dist: pandas (>=1.0,<2.0)
+Requires-Dist: pysimplegui (>=4.0,<5.0)
+Project-URL: Repository, https://github.com/Apteco/py-apteco
+Description-Content-Type: text/x-rst
 
-package_dir = \
-{'': 'src'}
+**************
+  Quickstart
+**************
 
-packages = \
-['apteco', 'apteco.data']
+Requirements
+============
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['apteco-api>=0.2.1,<0.3.0',
- 'numpy>=1.18,<2.0',
- 'pandas>=1.0,<2.0',
- 'pysimplegui>=4.0,<5.0']
-
-setup_kwargs = {
-    'name': 'apteco',
-    'version': '0.8.0',
-    'description': 'A Python package for interacting with Apteco Marketing Suite resources via the Apteco API.',
-    'long_description': '**************\n  Quickstart\n**************\n\nRequirements\n============\n\n* Python 3.6+\n* Access to an installation of the Apteco API\n\nThe Apteco API (which also goes under the name **Orbit API**)\nis part of the Apteco Orbit™ installation.\nIf you have access to Apteco Orbit™, you also have access to the Apteco API!\nIf you\'re not sure about this, contact whoever administers your Apteco software,\nor get in touch with Apteco support (support@apteco.com).\n\nInstallation\n============\n\nYou can install the package the usual way from PyPI using ``pip``:\n\n.. code-block:: console\n\n   python -m pip install apteco\n\nLogging in\n==========\n\nYour login credentials are the same username and password\nyou would use to log in to Apteco Orbit™:\n\n.. code-block:: python\n\n    >>> from apteco import login\n    >>> my_session = login("https://my-site.com/OrbitAPI", "my_data_view", "my_system", "jdoe")\n\nYou will be asked to enter your password in the terminal, which won\'t be echoed.\nIf Python is unable to ask for your password in this way,\nit will provide a pop-up box instead.\nThis might appear in the background,\nso check your taskbar for a new window if nothing seems to be happening.\n\nIf you don\'t want to enter your password every time,\nthere\'s also a ``login_with_password`` function which takes your password\nas a fifth argument:\n\n.. code-block:: python\n\n    >>> from apteco import login_with_password\n    >>> my_session = login_with_password(\n    ...     "https://my-site.com/OrbitAPI",\n    ...     "my_data_view",\n    ...     "my_system",\n    ...     "jdoe",\n    ...     "password",  # password is in plain sight in the code!\n    ... )\n\nTables\n======\n\nTables are accessed through the ``tables`` attribute on the ``Session`` object.\nYou can retrieve a table using its name:\n\n.. code-block:: python\n\n    >>> bookings = my_session.tables["Bookings"]\n\n``Table`` objects have properties for various metadata:\n\n.. code-block:: python\n\n    >>> print(\n    ...     f"There are {bookings.total_records:,}"\n    ...     f" {bookings.plural.lower()}"\n    ...     f" in the system."\n    ... )\n    There are 2,130,081 bookings in the system.\n\nVariables\n=========\n\nVariables are accessed through the ``variables`` attribute\non the ``Session`` object.\nYou can retrieve a variable using its name or description:\n\n.. code-block:: python\n\n    >>> occupation = my_session.variables["peOccu"]  # name\n    >>> cost = my_session.variables["Cost"]  # description\n\nEach table also has a ``variables`` attribute\nfor accessing the variables on that table:\n\n.. code-block:: python\n\n    >>> occupation = people.variables["peOccu"]\n    >>> cost = bookings.variables["Cost"]\n\nFor convenience you can access variables by indexing into the ``Table`` itself:\n\n.. code-block:: python\n\n    >>> occupation = people["peOccu"]\n    >>> cost = bookings["Cost"]\n\n``Variable`` objects have attributes with various metadata:\n\n.. code-block:: python\n\n    >>> occupation.type\n    <VariableType.SELECTOR: \'Selector\'>\n    >>> cost.description\n    \'Cost\'\n\nCreating selections\n===================\n\nYou can use the Python operators with ``Variable`` objects to build selections\nbased on criteria and return a count:\n\n.. code-block:: python\n\n    >>> sweden = bookings["Destination"] == "29"\n    >>> sweden.count()\n    25207\n\nYou can specify multiple values using any *iterable*:\n\n.. code-block:: python\n\n    >>> people = my_session.tables["People"]\n    >>> high_earners = people["Income"] == (f"{i:02}" for i in range(7, 12))\n    >>> high_earners.count()\n    7114\n\nYou can use other operators as well; for example, to exclude values:\n\n.. code-block:: python\n\n    >>> households = my_session.tables["Households"]\n    >>> uk_only = households["Region"] != "14"  # 14 is Channel Islands\n    >>> uk_only.count()\n    741572\n\nOr to allow a range of values:\n\n.. code-block:: python\n\n    >>> low_profit = bookings["Profit"] <= 25\n    >>> low_profit.count()\n    211328\n\n.. code-block:: python\n\n    >>> second_half_of_alphabet = people["Surname"] >= "N"\n    >>> second_half_of_alphabet.count()\n    410954\n\nDate and DateTime variables use the built-in ``datetime`` module:\n\n.. code-block:: python\n\n    >>> from datetime import date, datetime\n    >>> bookings_before_2019 = bookings["Booking Date"] <= date(2018, 12, 31)\n    >>> bookings_before_2019.count()\n    972439\n\nYou can take advantage of functionality available in other Python packages:\n\n.. code-block:: python\n\n    >>> from dateutil.relativedelta import relativedelta\n    >>> under_30 = people["DOB"] >= date.today() - relativedelta(years=30)\n    >>> under_30.count()\n    207737\n\nCombining selections\n====================\n\nYou can use the ``&`` ``|`` operators to combine selection criteria:\n\n.. code-block:: python\n\n    >>> sweden = bookings["Destination"] == "29"\n    >>> cost_at_least_2k = bookings["Cost"] >= 2000\n    >>> expensive_sweden = sweden & cost_at_least_2k\n    >>> expensive_sweden.count()\n    632\n    >>> student = people["Occupation"] == "4"\n    >>> under_21 = people["DOB"] >= date.today() - relativedelta(years=21)\n    >>> eligible_for_discount = student | under_21\n    >>> eligible_for_discount.count()\n    188364\n\nThe ``~`` operator negates a selection:\n\n.. code-block:: python\n\n    >>> pay_full_price = ~eligible_for_discount\n    >>> pay_full_price.count()\n    968189\n\nYou can join clauses from different tables and it will automatically handle\nthe required table changes:\n\n.. code-block:: python\n\n    >>> high_affordability = high_earners | cost_at_least_2k  # will resolve to people\n    >>> high_affordability.count()\n    56096\n    >>> high_affordability.table_name\n    \'People\'\n\nThe left-most clause determines the resolve table:\n\n.. code-block:: python\n\n    >>> female = people["Gender"] == "F"\n    >>> usa = bookings["Destination"] == "38"\n    >>> female.table_name\n    \'People\'\n    >>> usa.table_name\n    \'Bookings\'\n    >>> (female & usa).table_name\n    \'People\'\n    >>> (usa & female).table_name\n    \'Bookings\'\n\nYou can manually set the resolve table using the ``*`` operator:\n\n.. code-block:: python\n\n    >>> bookings_by_under_21s = bookings * under_21\n    >>> bookings_by_under_21s.count()\n    135100\n    >>> bookings_by_under_21s.table_name\n    \'Bookings\'\n\nCompound clauses follow Python operator precedence:\n\n.. code-block:: python\n\n    >>> student_or_young_female = student | female & under_21\n    >>> student_or_young_female.count()\n    166708\n    >>> student_or_female_must_be_young = (student | female) & under_21\n    >>> student_or_female_must_be_young.count()\n    49225\n\nBe especially careful where compound clauses involve table changes:\n\n.. code-block:: python\n\n    >>> women_to_sweden = female & sweden\n    >>> women_to_sweden.count()  # selection on People table\n    8674\n    >>> audience_1 = bookings * (female & sweden)\n    >>> audience_1.count()  # bookings by women who\'ve been to sweden\n    23553\n    >>> audience_2 = (bookings * female) & sweden\n    >>> audience_2.count()  # bookings made by a woman, with destination of sweden\n    8687\n\nCreating data grids\n===================\n\nYou can create a data grid from a table:\n\n.. code-block:: python\n\n    >>> urn = bookings["Booking URN"]\n    >>> dest = bookings["Destination"]\n    >>> occupation = people["Occupation"]\n    >>> town = households["Town"]\n    >>> datagrid = bookings.datagrid([urn, dest, cost, occupation, town])\n\nConvert it to a Pandas DataFrame:\n\n.. code-block:: python\n\n    >>> datagrid.to_df()\n        Booking URN    Destination     Cost       Occupation        Town\n    0      10001265         France  1392.35  Sales Executive    Aberdeen\n    1      10001266         France   780.34  Sales Executive    Aberdeen\n    2      10011532        Germany   181.68    Manual Worker      Alford\n    3      10011533        Germany   300.67    Manual Worker      Alford\n    4      10015830   Unclassified   228.70  Sales Executive     Macduff\n    ..          ...            ...      ...              ...         ...\n    995    10996176  United States   241.24     Professional  Glenrothes\n    996    10996177         Greece   343.23          Manager  Glenrothes\n    997    10996178  United States   636.22          Manager  Glenrothes\n    998    10996179  United States   356.21          Manager  Glenrothes\n    999    10996180  United States   438.20          Manager  Glenrothes\n\n    [1000 rows x 5 columns]\n\nYou can use a base selection to filter the records:\n\n.. code-block:: python\n\n    >>> sweden = dest == "29"\n    >>> sweden_datagrid = sweden.datagrid([urn, dest, cost, occupation, town])\n    >>> sweden_datagrid.to_df()\n        Booking URN Destination     Cost       Occupation           Town\n    0      10172319      Sweden  1201.81  Sales Executive         Bolton\n    1      10384970      Sweden   344.30          Manager     Chelmsford\n    2      10421011      Sweden   322.89  Sales Executive        Croydon\n    3      10425298      Sweden   880.02          Student  South Croydon\n    4      10479109      Sweden   172.91    Retail Worker       Nantwich\n    ..          ...         ...      ...              ...            ...\n    995    11471824      Sweden   118.76  Sales Executive    King\'s Lynn\n    996    11576762      Sweden   652.38    Public Sector        Redhill\n    997    11576764      Sweden   183.36    Public Sector        Redhill\n    998    11682962      Sweden  1166.38          Manager         London\n    999    11754655      Sweden   192.45  Sales Executive          Ascot\n\n    [1000 rows x 5 columns]\n\nYou can filter using a selection from a different table:\n\n.. code-block:: python\n\n    >>> manchester = households["Region"] == "13"\n    >>> manc_datagrid = manchester.datagrid(\n    ...     [urn, dest, cost, occupation, town], table=bookings\n    ... )\n    >>> manc_datagrid.to_df()\n        Booking URN    Destination     Cost       Occupation         Town\n    0      10172319         Sweden  1201.81  Sales Executive       Bolton\n    1      10172320  United States  1616.80  Sales Executive       Bolton\n    2      10173729         France   581.71          Student       Bolton\n    3      10173730         France  2224.70          Student       Bolton\n    4      10177047         France   686.53  Sales Executive       Bolton\n    ..          ...            ...      ...              ...          ...\n    995    11739340      Australia   316.60     Professional  Stalybridge\n    996    11739342   Unclassified   316.58  Sales Executive  Stalybridge\n    997    12087034         Greece  1305.66    Public Sector   Altrincham\n    998    12087035  United States   585.65    Public Sector   Altrincham\n    999    12087036      Australia   496.64    Public Sector   Altrincham\n\n    [1000 rows x 5 columns]\n\nCreating cubes\n==============\n\nYou can create a cube from a table:\n\n.. code-block:: python\n\n    >>> occupation = people["Occupation"]\n    >>> income = people["Income"]\n    >>> gender = people["Gender"]\n    >>> cube = people.cube([occupation, income, gender])\n\nConvert it to a Pandas DataFrame:\n\n.. code-block:: python\n\n    >>> df = cube.to_df()\n    >>> df.head(10)\n                                   People\n    Occupation    Income  Gender\n    Manual Worker <£10k   Female    15624\n                          Male       5321\n                          Unknown       5\n                  £10-20k Female    43051\n                          Male       5992\n                          Unknown      25\n                  £20-30k Female     1498\n                          Male        649\n                          Unknown      14\n                  £30-40k Female      675\n\nYou can pivot the dimensions to make it easier to read:\n\n.. code-block:: python\n\n    >>> df.unstack(level=0)\n                       People          ...\n    Occupation       Director Manager  ... Student Unemployed\n    Income   Gender                    ...\n    <£10k    Female      1279    4649  ...   28002      21385\n             Male         832    2926  ...   14296       8386\n             Unknown        4      16  ...      10        155\n    £10-20k  Female      4116   16665  ...   39462      17230\n             Male        2139    9123  ...   17917       4532\n             Unknown        9      47  ...      25        368\n    £100k+   Female         2       1  ...       2          0\n             Male           1       0  ...       3          0\n             Unknown        1       0  ...       1          0\n    £20-30k  Female      1267    6238  ...    6669       5747\n             Male        1050    5315  ...    5274       1345\n             Unknown        5      45  ...      22        236\n    £30-40k  Female      1591    6621  ...    5690       3117\n             Male        1940    9713  ...    6345       1049\n             Unknown       46     140  ...      63        519\n    £40-50k  Female       265     965  ...     587        262\n             Male         518    1800  ...     943        115\n             Unknown       22      58  ...      29        110\n    £50-60k  Female       336     806  ...     425        277\n             Male         607    1677  ...     692         69\n             Unknown       47      88  ...      64         89\n    £60-70k  Female        40     112  ...      54         58\n             Male          96     220  ...      95          8\n             Unknown       11      16  ...      17         17\n    £70-80k  Female        44      96  ...      42         27\n             Male         102     179  ...      63          5\n             Unknown       12      22  ...      15          5\n    £80-90k  Female        11      11  ...       3          0\n             Male          14      13  ...      16          0\n             Unknown        4       3  ...       5          0\n    £90-100k Female         1       0  ...       1          1\n             Male          11       7  ...       4          0\n             Unknown        3       6  ...       9          0\n\n    [33 rows x 10 columns]\n\nYou can use a base selection to filter the records:\n\n.. code-block:: python\n\n    >>> occupation = people["Occupation"]\n    >>> region = households["Region"]\n    >>> student = occupation == "4"\n    >>> student_cube = student.cube([occupation, dest, region])\n    >>> student_df = student_cube.to_df()\n    >>> student_df.head()\n                                                                     People\n    Occupation    Destination Region\n    Manual Worker Australia   North                                       0\n                              North West (Excluding Gtr Manchester)       0\n                              South East (Outside M25 )                   0\n                              South West                                  0\n                              East Midlands                               0\n\nSelecting only cells where ``Occupation`` is *Student*,\nand pivoting ``Destination`` dimension:\n\n.. code-block:: python\n\n    >>> student_df.loc["Student"].unstack(level=0)\n                                             People          ...\n    Destination                           Australia Denmark  ... Sweden United States\n    Region                                                   ...\n    Channel Islands                              46       1  ...     10            81\n    East Anglia                                 989       0  ...    109           905\n    East Midlands                              1956       0  ...    174          1762\n    Greater Manchester                         1197       1  ...    147          1089\n    North                                       959       2  ...    115           869\n    North West (Excluding Gtr Manchester)      1594       2  ...    177          1429\n    Northern Ireland                            467       0  ...     42           492\n    Scotland                                   2061       1  ...    224          1964\n    South East (Inside M25 )                   3935       0  ...    390          3580\n    South East (Outside M25 )                  6255       1  ...    608          5587\n    South West                                 2310       0  ...    182          2037\n    Wales                                       974       0  ...    122           860\n    West Midlands                              2643       0  ...    288          2362\n    Yorkshire and Humber                       2295       0  ...    249          2089\n\n    [14 rows x 19 columns]\n\nYou can use a selection from a different table to filter the records in the cube:\n\n.. code-block:: python\n\n    >>> manchester = region == "13"\n    >>> manc_cube = manchester.cube([occupation, dest, region], table=bookings)\n    >>> manc_cube.to_df()\n                                                                      Bookings\n    Occupation    Destination  Region\n    Manual Worker Australia    North                                         0\n                               North West (Excluding Gtr Manchester)         0\n                               South East (Outside M25 )                     0\n                               South West                                    0\n                               East Midlands                                 0\n                                                                        ...\n    Retired       South Africa Scotland                                      0\n                               Wales                                         0\n                               Northern Ireland                              0\n                               Greater Manchester                            0\n                               Channel Islands                               0\n\n    [2660 rows x 1 columns]\n\nYou can find the complete documentation\nincluding a more thorough `tutorial <https://help.apteco.com/python/tutorial.html>`_\non the `Apteco website <https://help.apteco.com/python/index.html>`_.',
-    'author': 'Apteco Ltd',
-    'author_email': 'support@apteco.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://help.apteco.com/python/index.html',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6.1,<4.0.0',
-}
+* Python 3.6+
+* Access to an installation of the Apteco API
 
+The Apteco API (which also goes under the name **Orbit API**)
+is part of the Apteco Orbit™ installation.
+If you have access to Apteco Orbit™, you also have access to the Apteco API!
+If you're not sure about this, contact whoever administers your Apteco software,
+or get in touch with Apteco support (support@apteco.com).
 
-setup(**setup_kwargs)
+Installation
+============
+
+You can install the package the usual way from PyPI using ``pip``:
+
+.. code-block:: console
+
+   python -m pip install apteco
+
+Logging in
+==========
+
+Your login credentials are the same username and password
+you would use to log in to Apteco Orbit™:
+
+.. code-block:: python
+
+    >>> from apteco import login
+    >>> my_session = login("https://my-site.com/OrbitAPI", "my_data_view", "my_system", "jdoe")
+
+You will be asked to enter your password in the terminal, which won't be echoed.
+If Python is unable to ask for your password in this way,
+it will provide a pop-up box instead.
+This might appear in the background,
+so check your taskbar for a new window if nothing seems to be happening.
+
+If you don't want to enter your password every time,
+there's also a ``login_with_password`` function which takes your password
+as a fifth argument:
+
+.. code-block:: python
+
+    >>> from apteco import login_with_password
+    >>> my_session = login_with_password(
+    ...     "https://my-site.com/OrbitAPI",
+    ...     "my_data_view",
+    ...     "my_system",
+    ...     "jdoe",
+    ...     "password",  # password is in plain sight in the code!
+    ... )
+
+Tables
+======
+
+Tables are accessed through the ``tables`` attribute on the ``Session`` object.
+You can retrieve a table using its name:
+
+.. code-block:: python
+
+    >>> bookings = my_session.tables["Bookings"]
+
+``Table`` objects have properties for various metadata:
+
+.. code-block:: python
+
+    >>> print(
+    ...     f"There are {bookings.total_records:,}"
+    ...     f" {bookings.plural.lower()}"
+    ...     f" in the system."
+    ... )
+    There are 2,130,081 bookings in the system.
+
+Variables
+=========
+
+Variables are accessed through the ``variables`` attribute
+on the ``Session`` object.
+You can retrieve a variable using its name or description:
+
+.. code-block:: python
+
+    >>> occupation = my_session.variables["peOccu"]  # name
+    >>> cost = my_session.variables["Cost"]  # description
+
+Each table also has a ``variables`` attribute
+for accessing the variables on that table:
+
+.. code-block:: python
+
+    >>> occupation = people.variables["peOccu"]
+    >>> cost = bookings.variables["Cost"]
+
+For convenience you can access variables by indexing into the ``Table`` itself:
+
+.. code-block:: python
+
+    >>> occupation = people["peOccu"]
+    >>> cost = bookings["Cost"]
+
+``Variable`` objects have attributes with various metadata:
+
+.. code-block:: python
+
+    >>> occupation.type
+    <VariableType.SELECTOR: 'Selector'>
+    >>> cost.description
+    'Cost'
+
+Creating selections
+===================
+
+You can use the Python operators with ``Variable`` objects to build selections
+based on criteria and return a count:
+
+.. code-block:: python
+
+    >>> sweden = bookings["Destination"] == "29"
+    >>> sweden.count()
+    25207
+
+You can specify multiple values using any *iterable*:
+
+.. code-block:: python
+
+    >>> people = my_session.tables["People"]
+    >>> high_earners = people["Income"] == (f"{i:02}" for i in range(7, 12))
+    >>> high_earners.count()
+    7114
+
+You can use other operators as well; for example, to exclude values:
+
+.. code-block:: python
+
+    >>> households = my_session.tables["Households"]
+    >>> uk_only = households["Region"] != "14"  # 14 is Channel Islands
+    >>> uk_only.count()
+    741572
+
+Or to allow a range of values:
+
+.. code-block:: python
+
+    >>> low_profit = bookings["Profit"] <= 25
+    >>> low_profit.count()
+    211328
+
+.. code-block:: python
+
+    >>> second_half_of_alphabet = people["Surname"] >= "N"
+    >>> second_half_of_alphabet.count()
+    410954
+
+Date and DateTime variables use the built-in ``datetime`` module:
+
+.. code-block:: python
+
+    >>> from datetime import date, datetime
+    >>> bookings_before_2019 = bookings["Booking Date"] <= date(2018, 12, 31)
+    >>> bookings_before_2019.count()
+    972439
+
+You can take advantage of functionality available in other Python packages:
+
+.. code-block:: python
+
+    >>> from dateutil.relativedelta import relativedelta
+    >>> under_30 = people["DOB"] >= date.today() - relativedelta(years=30)
+    >>> under_30.count()
+    207737
+
+Combining selections
+====================
+
+You can use the ``&`` ``|`` operators to combine selection criteria:
+
+.. code-block:: python
+
+    >>> sweden = bookings["Destination"] == "29"
+    >>> cost_at_least_2k = bookings["Cost"] >= 2000
+    >>> expensive_sweden = sweden & cost_at_least_2k
+    >>> expensive_sweden.count()
+    632
+    >>> student = people["Occupation"] == "4"
+    >>> under_21 = people["DOB"] >= date.today() - relativedelta(years=21)
+    >>> eligible_for_discount = student | under_21
+    >>> eligible_for_discount.count()
+    188364
+
+The ``~`` operator negates a selection:
+
+.. code-block:: python
+
+    >>> pay_full_price = ~eligible_for_discount
+    >>> pay_full_price.count()
+    968189
+
+You can join clauses from different tables and it will automatically handle
+the required table changes:
+
+.. code-block:: python
+
+    >>> high_affordability = high_earners | cost_at_least_2k  # will resolve to people
+    >>> high_affordability.count()
+    56096
+    >>> high_affordability.table_name
+    'People'
+
+The left-most clause determines the resolve table:
+
+.. code-block:: python
+
+    >>> female = people["Gender"] == "F"
+    >>> usa = bookings["Destination"] == "38"
+    >>> female.table_name
+    'People'
+    >>> usa.table_name
+    'Bookings'
+    >>> (female & usa).table_name
+    'People'
+    >>> (usa & female).table_name
+    'Bookings'
+
+You can manually set the resolve table using the ``*`` operator:
+
+.. code-block:: python
+
+    >>> bookings_by_under_21s = bookings * under_21
+    >>> bookings_by_under_21s.count()
+    135100
+    >>> bookings_by_under_21s.table_name
+    'Bookings'
+
+Compound clauses follow Python operator precedence:
+
+.. code-block:: python
+
+    >>> student_or_young_female = student | female & under_21
+    >>> student_or_young_female.count()
+    166708
+    >>> student_or_female_must_be_young = (student | female) & under_21
+    >>> student_or_female_must_be_young.count()
+    49225
+
+Be especially careful where compound clauses involve table changes:
+
+.. code-block:: python
+
+    >>> women_to_sweden = female & sweden
+    >>> women_to_sweden.count()  # selection on People table
+    8674
+    >>> audience_1 = bookings * (female & sweden)
+    >>> audience_1.count()  # bookings by women who've been to sweden
+    23553
+    >>> audience_2 = (bookings * female) & sweden
+    >>> audience_2.count()  # bookings made by a woman, with destination of sweden
+    8687
+
+Creating data grids
+===================
+
+You can create a data grid from a table:
+
+.. code-block:: python
+
+    >>> urn = bookings["Booking URN"]
+    >>> dest = bookings["Destination"]
+    >>> occupation = people["Occupation"]
+    >>> town = households["Town"]
+    >>> datagrid = bookings.datagrid([urn, dest, cost, occupation, town])
+
+Convert it to a Pandas DataFrame:
+
+.. code-block:: python
+
+    >>> datagrid.to_df()
+        Booking URN    Destination     Cost       Occupation        Town
+    0      10001265         France  1392.35  Sales Executive    Aberdeen
+    1      10001266         France   780.34  Sales Executive    Aberdeen
+    2      10011532        Germany   181.68    Manual Worker      Alford
+    3      10011533        Germany   300.67    Manual Worker      Alford
+    4      10015830   Unclassified   228.70  Sales Executive     Macduff
+    ..          ...            ...      ...              ...         ...
+    995    10996176  United States   241.24     Professional  Glenrothes
+    996    10996177         Greece   343.23          Manager  Glenrothes
+    997    10996178  United States   636.22          Manager  Glenrothes
+    998    10996179  United States   356.21          Manager  Glenrothes
+    999    10996180  United States   438.20          Manager  Glenrothes
+
+    [1000 rows x 5 columns]
+
+You can use a base selection to filter the records:
+
+.. code-block:: python
+
+    >>> sweden = dest == "29"
+    >>> sweden_datagrid = sweden.datagrid([urn, dest, cost, occupation, town])
+    >>> sweden_datagrid.to_df()
+        Booking URN Destination     Cost       Occupation           Town
+    0      10172319      Sweden  1201.81  Sales Executive         Bolton
+    1      10384970      Sweden   344.30          Manager     Chelmsford
+    2      10421011      Sweden   322.89  Sales Executive        Croydon
+    3      10425298      Sweden   880.02          Student  South Croydon
+    4      10479109      Sweden   172.91    Retail Worker       Nantwich
+    ..          ...         ...      ...              ...            ...
+    995    11471824      Sweden   118.76  Sales Executive    King's Lynn
+    996    11576762      Sweden   652.38    Public Sector        Redhill
+    997    11576764      Sweden   183.36    Public Sector        Redhill
+    998    11682962      Sweden  1166.38          Manager         London
+    999    11754655      Sweden   192.45  Sales Executive          Ascot
+
+    [1000 rows x 5 columns]
+
+You can filter using a selection from a different table:
+
+.. code-block:: python
+
+    >>> manchester = households["Region"] == "13"
+    >>> manc_datagrid = manchester.datagrid(
+    ...     [urn, dest, cost, occupation, town], table=bookings
+    ... )
+    >>> manc_datagrid.to_df()
+        Booking URN    Destination     Cost       Occupation         Town
+    0      10172319         Sweden  1201.81  Sales Executive       Bolton
+    1      10172320  United States  1616.80  Sales Executive       Bolton
+    2      10173729         France   581.71          Student       Bolton
+    3      10173730         France  2224.70          Student       Bolton
+    4      10177047         France   686.53  Sales Executive       Bolton
+    ..          ...            ...      ...              ...          ...
+    995    11739340      Australia   316.60     Professional  Stalybridge
+    996    11739342   Unclassified   316.58  Sales Executive  Stalybridge
+    997    12087034         Greece  1305.66    Public Sector   Altrincham
+    998    12087035  United States   585.65    Public Sector   Altrincham
+    999    12087036      Australia   496.64    Public Sector   Altrincham
+
+    [1000 rows x 5 columns]
+
+Creating cubes
+==============
+
+You can create a cube from a table:
+
+.. code-block:: python
+
+    >>> occupation = people["Occupation"]
+    >>> income = people["Income"]
+    >>> gender = people["Gender"]
+    >>> cube = people.cube([occupation, income, gender])
+
+Convert it to a Pandas DataFrame:
+
+.. code-block:: python
+
+    >>> df = cube.to_df()
+    >>> df.head(10)
+                                   People
+    Occupation    Income  Gender
+    Manual Worker <£10k   Female    15624
+                          Male       5321
+                          Unknown       5
+                  £10-20k Female    43051
+                          Male       5992
+                          Unknown      25
+                  £20-30k Female     1498
+                          Male        649
+                          Unknown      14
+                  £30-40k Female      675
+
+You can pivot the dimensions to make it easier to read:
+
+.. code-block:: python
+
+    >>> df.unstack(level=0)
+                       People          ...
+    Occupation       Director Manager  ... Student Unemployed
+    Income   Gender                    ...
+    <£10k    Female      1279    4649  ...   28002      21385
+             Male         832    2926  ...   14296       8386
+             Unknown        4      16  ...      10        155
+    £10-20k  Female      4116   16665  ...   39462      17230
+             Male        2139    9123  ...   17917       4532
+             Unknown        9      47  ...      25        368
+    £100k+   Female         2       1  ...       2          0
+             Male           1       0  ...       3          0
+             Unknown        1       0  ...       1          0
+    £20-30k  Female      1267    6238  ...    6669       5747
+             Male        1050    5315  ...    5274       1345
+             Unknown        5      45  ...      22        236
+    £30-40k  Female      1591    6621  ...    5690       3117
+             Male        1940    9713  ...    6345       1049
+             Unknown       46     140  ...      63        519
+    £40-50k  Female       265     965  ...     587        262
+             Male         518    1800  ...     943        115
+             Unknown       22      58  ...      29        110
+    £50-60k  Female       336     806  ...     425        277
+             Male         607    1677  ...     692         69
+             Unknown       47      88  ...      64         89
+    £60-70k  Female        40     112  ...      54         58
+             Male          96     220  ...      95          8
+             Unknown       11      16  ...      17         17
+    £70-80k  Female        44      96  ...      42         27
+             Male         102     179  ...      63          5
+             Unknown       12      22  ...      15          5
+    £80-90k  Female        11      11  ...       3          0
+             Male          14      13  ...      16          0
+             Unknown        4       3  ...       5          0
+    £90-100k Female         1       0  ...       1          1
+             Male          11       7  ...       4          0
+             Unknown        3       6  ...       9          0
+
+    [33 rows x 10 columns]
+
+You can use a base selection to filter the records:
+
+.. code-block:: python
+
+    >>> occupation = people["Occupation"]
+    >>> region = households["Region"]
+    >>> student = occupation == "4"
+    >>> student_cube = student.cube([occupation, dest, region])
+    >>> student_df = student_cube.to_df()
+    >>> student_df.head()
+                                                                     People
+    Occupation    Destination Region
+    Manual Worker Australia   North                                       0
+                              North West (Excluding Gtr Manchester)       0
+                              South East (Outside M25 )                   0
+                              South West                                  0
+                              East Midlands                               0
+
+Selecting only cells where ``Occupation`` is *Student*,
+and pivoting ``Destination`` dimension:
+
+.. code-block:: python
+
+    >>> student_df.loc["Student"].unstack(level=0)
+                                             People          ...
+    Destination                           Australia Denmark  ... Sweden United States
+    Region                                                   ...
+    Channel Islands                              46       1  ...     10            81
+    East Anglia                                 989       0  ...    109           905
+    East Midlands                              1956       0  ...    174          1762
+    Greater Manchester                         1197       1  ...    147          1089
+    North                                       959       2  ...    115           869
+    North West (Excluding Gtr Manchester)      1594       2  ...    177          1429
+    Northern Ireland                            467       0  ...     42           492
+    Scotland                                   2061       1  ...    224          1964
+    South East (Inside M25 )                   3935       0  ...    390          3580
+    South East (Outside M25 )                  6255       1  ...    608          5587
+    South West                                 2310       0  ...    182          2037
+    Wales                                       974       0  ...    122           860
+    West Midlands                              2643       0  ...    288          2362
+    Yorkshire and Humber                       2295       0  ...    249          2089
+
+    [14 rows x 19 columns]
+
+You can use a selection from a different table to filter the records in the cube:
+
+.. code-block:: python
+
+    >>> manchester = region == "13"
+    >>> manc_cube = manchester.cube([occupation, dest, region], table=bookings)
+    >>> manc_cube.to_df()
+                                                                      Bookings
+    Occupation    Destination  Region
+    Manual Worker Australia    North                                         0
+                               North West (Excluding Gtr Manchester)         0
+                               South East (Outside M25 )                     0
+                               South West                                    0
+                               East Midlands                                 0
+                                                                        ...
+    Retired       South Africa Scotland                                      0
+                               Wales                                         0
+                               Northern Ireland                              0
+                               Greater Manchester                            0
+                               Channel Islands                               0
+
+    [2660 rows x 1 columns]
+
+You can find the complete documentation
+including a more thorough `tutorial <https://help.apteco.com/python/tutorial.html>`_
+on the `Apteco website <https://help.apteco.com/python/index.html>`_.
```

