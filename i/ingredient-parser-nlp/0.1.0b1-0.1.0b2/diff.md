# Comparing `tmp/ingredient_parser_nlp-0.1.0b1.tar.gz` & `tmp/ingredient_parser_nlp-0.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ingredient_parser_nlp-0.1.0b1.tar", last modified: Sat Apr  8 17:11:32 2023, max compression
+gzip compressed data, was "ingredient_parser_nlp-0.1.0b2.tar", last modified: Tue Jul 18 18:06:36 2023, max compression
```

## Comparing `ingredient_parser_nlp-0.1.0b1.tar` & `ingredient_parser_nlp-0.1.0b2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-08 17:11:32.128593 ingredient_parser_nlp-0.1.0b1/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1068 2023-01-22 15:40:13.000000 ingredient_parser_nlp-0.1.0b1/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)       60 2022-09-02 18:55:35.000000 ingredient_parser_nlp-0.1.0b1/MANIFEST.in
--rw-rw-r--   0 tom       (1000) tom       (1000)     4262 2023-04-08 17:11:32.128593 ingredient_parser_nlp-0.1.0b1/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     2221 2023-04-08 16:25:47.000000 ingredient_parser_nlp-0.1.0b1/README.md
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-08 17:11:32.128593 ingredient_parser_nlp-0.1.0b1/ingredient_parser/
--rw-rw-r--   0 tom       (1000) tom       (1000)      304 2023-04-08 17:11:12.000000 ingredient_parser_nlp-0.1.0b1/ingredient_parser/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4991 2023-04-05 19:05:30.000000 ingredient_parser_nlp-0.1.0b1/ingredient_parser/_constants.py
--rw-rw-r--   0 tom       (1000) tom       (1000)  1492372 2023-04-08 16:21:50.000000 ingredient_parser_nlp-0.1.0b1/ingredient_parser/model.crfsuite
--rw-rw-r--   0 tom       (1000) tom       (1000)     5872 2023-04-07 16:23:13.000000 ingredient_parser_nlp-0.1.0b1/ingredient_parser/parsers.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    19932 2023-04-08 16:43:36.000000 ingredient_parser_nlp-0.1.0b1/ingredient_parser/preprocess.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5860 2023-04-05 19:05:30.000000 ingredient_parser_nlp-0.1.0b1/ingredient_parser/regex_parser.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5871 2023-04-01 07:57:16.000000 ingredient_parser_nlp-0.1.0b1/ingredient_parser/utils.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-08 17:11:32.128593 ingredient_parser_nlp-0.1.0b1/ingredient_parser_nlp.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)     4262 2023-04-08 17:11:32.000000 ingredient_parser_nlp-0.1.0b1/ingredient_parser_nlp.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)      551 2023-04-08 17:11:32.000000 ingredient_parser_nlp-0.1.0b1/ingredient_parser_nlp.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-04-08 17:11:32.000000 ingredient_parser_nlp-0.1.0b1/ingredient_parser_nlp.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       39 2023-04-08 17:11:32.000000 ingredient_parser_nlp-0.1.0b1/ingredient_parser_nlp.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       18 2023-04-08 17:11:32.000000 ingredient_parser_nlp-0.1.0b1/ingredient_parser_nlp.egg-info/top_level.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)     1942 2023-04-01 08:24:23.000000 ingredient_parser_nlp-0.1.0b1/pyproject.toml
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-08 17:11:32.128593 ingredient_parser_nlp-0.1.0b1/setup.cfg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-08 17:11:32.128593 ingredient_parser_nlp-0.1.0b1/tests/
--rw-rw-r--   0 tom       (1000) tom       (1000)     6076 2023-04-07 16:02:38.000000 ingredient_parser_nlp-0.1.0b1/tests/test_parser.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    20667 2023-04-08 16:43:10.000000 ingredient_parser_nlp-0.1.0b1/tests/test_preprocess.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6720 2023-03-31 15:12:24.000000 ingredient_parser_nlp-0.1.0b1/tests/test_utils.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-07-18 18:06:36.322743 ingredient_parser_nlp-0.1.0b2/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1068 2023-01-22 15:40:13.000000 ingredient_parser_nlp-0.1.0b2/LICENSE
+-rw-rw-r--   0 tom       (1000) tom       (1000)       60 2022-09-02 18:55:35.000000 ingredient_parser_nlp-0.1.0b2/MANIFEST.in
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4163 2023-07-18 18:06:36.322743 ingredient_parser_nlp-0.1.0b2/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2122 2023-06-30 14:35:35.000000 ingredient_parser_nlp-0.1.0b2/README.md
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-07-18 18:06:36.318743 ingredient_parser_nlp-0.1.0b2/ingredient_parser/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      304 2023-07-18 18:05:24.000000 ingredient_parser_nlp-0.1.0b2/ingredient_parser/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5528 2023-04-10 17:44:44.000000 ingredient_parser_nlp-0.1.0b2/ingredient_parser/_constants.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)  3070488 2023-07-18 17:57:43.000000 ingredient_parser_nlp-0.1.0b2/ingredient_parser/model.crfsuite
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5835 2023-06-30 12:54:11.000000 ingredient_parser_nlp-0.1.0b2/ingredient_parser/parsers.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    21016 2023-07-18 17:56:03.000000 ingredient_parser_nlp-0.1.0b2/ingredient_parser/preprocess.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5860 2023-04-08 17:12:49.000000 ingredient_parser_nlp-0.1.0b2/ingredient_parser/regex_parser.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5847 2023-06-30 12:54:47.000000 ingredient_parser_nlp-0.1.0b2/ingredient_parser/utils.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-07-18 18:06:36.322743 ingredient_parser_nlp-0.1.0b2/ingredient_parser_nlp.egg-info/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4163 2023-07-18 18:06:36.000000 ingredient_parser_nlp-0.1.0b2/ingredient_parser_nlp.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)      551 2023-07-18 18:06:36.000000 ingredient_parser_nlp-0.1.0b2/ingredient_parser_nlp.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-07-18 18:06:36.000000 ingredient_parser_nlp-0.1.0b2/ingredient_parser_nlp.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       39 2023-07-18 18:06:36.000000 ingredient_parser_nlp-0.1.0b2/ingredient_parser_nlp.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       18 2023-07-18 18:06:36.000000 ingredient_parser_nlp-0.1.0b2/ingredient_parser_nlp.egg-info/top_level.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1696 2023-04-10 11:22:58.000000 ingredient_parser_nlp-0.1.0b2/pyproject.toml
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-07-18 18:06:36.322743 ingredient_parser_nlp-0.1.0b2/setup.cfg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-07-18 18:06:36.322743 ingredient_parser_nlp-0.1.0b2/tests/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6076 2023-04-10 11:39:37.000000 ingredient_parser_nlp-0.1.0b2/tests/test_parser.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    20667 2023-04-08 17:12:49.000000 ingredient_parser_nlp-0.1.0b2/tests/test_preprocess.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6720 2023-03-31 15:12:24.000000 ingredient_parser_nlp-0.1.0b2/tests/test_utils.py
```

### Comparing `ingredient_parser_nlp-0.1.0b1/LICENSE` & `ingredient_parser_nlp-0.1.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `ingredient_parser_nlp-0.1.0b1/PKG-INFO` & `ingredient_parser_nlp-0.1.0b2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ingredient_parser_nlp
-Version: 0.1.0b1
+Version: 0.1.0b2
 Summary: A Python package to parse structured information from recipe ingredient sentences
 Author-email: Tom Strange <tpstrange@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tom Strange
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -52,29 +52,29 @@
 >>> from ingredient_parser import parse_ingredient
 
 >>> parse_ingredient("3 pounds pork shoulder, cut into 2-inch chunks")
 {'sentence': '3 pounds pork shoulder, cut into 2-inch chunks',
  'quantity': '3',
  'unit': 'pound',
  'name': 'pork shoulder',
- 'comment': ', cut into 2-inch chunks',
+ 'comment': 'cut into 2-inch chunks',
  'other': ''}
 
 # Output confidence for each label
 >>> parse_ingredient("3 pounds pork shoulder, cut into 2-inch chunks", confidence=True)
 {'sentence': '3 pounds pork shoulder, cut into 2-inch chunks',
  'quantity': '3',
  'unit': 'pound',
  'name': 'pork shoulder',
- 'comment': ', cut into 2-inch chunks',
+ 'comment': 'cut into 2-inch chunks',
  'other': '',
- 'confidence': {'quantity': 0.9986,
-  'unit': 0.9967,
-  'name': 0.9535,
-  'comment': 0.9967,
+ 'confidence': {'quantity': 0.9988,
+  'unit': 0.9969,
+  'name': 0.9698,
+  'comment': 0.9992,
   'other': 0}}
 ```
 
 The returned dictionary has the format
 
 ```python
 {
@@ -106,16 +106,12 @@
 ## Development
 
 The development dependencies are in the ```requirements-dev.txt``` file.
 
 Note that development includes training the model.
 
 * ```Black``` is used for code formatting.
-* ```isort``` is used for import sorting.
-
-* ```flake8``` is used for linting. Note the line length standard (E501) is ignored.
-
+* ```ruff``` is used for linting. 
 * ```pyright``` is used for type static analysis.
-
 * ```pytest``` is used for tests, with ```coverage``` being used for test coverage.
 
 The documentation dependencies are in the ```requirement-doc.txt``` file.
```

### Comparing `ingredient_parser_nlp-0.1.0b1/README.md` & `ingredient_parser_nlp-0.1.0b2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -22,29 +22,29 @@
 >>> from ingredient_parser import parse_ingredient
 
 >>> parse_ingredient("3 pounds pork shoulder, cut into 2-inch chunks")
 {'sentence': '3 pounds pork shoulder, cut into 2-inch chunks',
  'quantity': '3',
  'unit': 'pound',
  'name': 'pork shoulder',
- 'comment': ', cut into 2-inch chunks',
+ 'comment': 'cut into 2-inch chunks',
  'other': ''}
 
 # Output confidence for each label
 >>> parse_ingredient("3 pounds pork shoulder, cut into 2-inch chunks", confidence=True)
 {'sentence': '3 pounds pork shoulder, cut into 2-inch chunks',
  'quantity': '3',
  'unit': 'pound',
  'name': 'pork shoulder',
- 'comment': ', cut into 2-inch chunks',
+ 'comment': 'cut into 2-inch chunks',
  'other': '',
- 'confidence': {'quantity': 0.9986,
-  'unit': 0.9967,
-  'name': 0.9535,
-  'comment': 0.9967,
+ 'confidence': {'quantity': 0.9988,
+  'unit': 0.9969,
+  'name': 0.9698,
+  'comment': 0.9992,
   'other': 0}}
 ```
 
 The returned dictionary has the format
 
 ```python
 {
@@ -76,16 +76,12 @@
 ## Development
 
 The development dependencies are in the ```requirements-dev.txt``` file.
 
 Note that development includes training the model.
 
 * ```Black``` is used for code formatting.
-* ```isort``` is used for import sorting.
-
-* ```flake8``` is used for linting. Note the line length standard (E501) is ignored.
-
+* ```ruff``` is used for linting. 
 * ```pyright``` is used for type static analysis.
-
 * ```pytest``` is used for tests, with ```coverage``` being used for test coverage.
 
 The documentation dependencies are in the ```requirement-doc.txt``` file.
```

### Comparing `ingredient_parser_nlp-0.1.0b1/ingredient_parser/_constants.py` & `ingredient_parser_nlp-0.1.0b2/ingredient_parser/_constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -85,14 +85,33 @@
 }
 # Generate capitalized version of each entry in the UNITS dictionary
 _capitalized_units = {}
 for plural, singular in UNITS.items():
     _capitalized_units[plural.capitalize()] = singular.capitalize()
 UNITS = UNITS | _capitalized_units
 
+
+# Units that can be part of the name
+# e.g. 1 teaspoon ground cloves, or 5 bay leaves
+AMBIGUOUS_UNITS = [
+    "cloves",
+    "leaves",
+    "slabs",
+    "wedges",
+]
+# Extend list automatically to include singular and capitalized forms
+_ambiguous_units_alt_forms = []
+for amb_unit in AMBIGUOUS_UNITS:
+    _ambiguous_units_alt_forms.append(amb_unit.capitalize())
+    _ambiguous_units_alt_forms.append(UNITS[amb_unit])
+    _ambiguous_units_alt_forms.append(UNITS[amb_unit.capitalize()])
+
+AMBIGUOUS_UNITS.extend(_ambiguous_units_alt_forms)
+
+
 # Strings and their numeric representation
 STRING_NUMBERS = {
     "half": "0.5",
     "one": "1",
     "two": "2",
     "three": "3",
     "four": "4",
```

### Comparing `ingredient_parser_nlp-0.1.0b1/ingredient_parser/parsers.py` & `ingredient_parser_nlp-0.1.0b2/ingredient_parser/parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python3
 
 import argparse
 import importlib.resources as pkg_resources
 import json
-from typing import Dict, List, Union
 
 import pycrfsuite
 from typing_extensions import NotRequired, TypedDict
 
 from .preprocess import PreProcessor
 from .utils import average, find_idx, fix_punctuation, join_adjacent, pluralise_units
 
@@ -21,15 +20,15 @@
 
     sentence: str
     quantity: str
     unit: str
     name: str
     comment: str
     other: str
-    confidence: NotRequired[Dict[str, float]]
+    confidence: NotRequired[dict[str, float]]
 
 
 # Create TAGGER object
 TAGGER = pycrfsuite.Tagger()
 with pkg_resources.path(__package__, "model.crfsuite") as p:
     TAGGER.open(str(p))
 
@@ -44,15 +43,15 @@
         {
             "sentence": str,
             "quantity": str,
             "unit": str,
             "name": str,
             "comment": str,
             "other": str,
-            "confidence": Dict[str, float] <- Optional
+            "confidence": dict[str, float] <- Optional
         }
 
     Parameters
     ----------
     sentence : str
         Ingredient sentence to parse
     confidence : bool, optional
@@ -122,34 +121,34 @@
             "other": average(labels, scores, "OTHER"),
         }
 
     return parsed
 
 
 def parse_multiple_ingredients(
-    sentences: List[str], confidence: bool = False
-) -> List[ParsedIngredient]:
+    sentences: list[str], confidence: bool = False
+) -> list[ParsedIngredient]:
     """Parse multiple ingredient sentences in one go.
 
     This function accepts a list of sentences, with element of the list representing
     one ingredient sentence.
     A list of dictionaries is returned, with optional confidence values.
     This function is a simple for-loop that iterates through each element of the
     input list.
 
     Parameters
     ----------
-    sentences : List[str]
+    sentences : list[str]
         List of sentences to parse
     confidence : bool, optional
         Return confidence scores for labels
 
     Returns
     -------
-    List[ParsedIngredient]
+    list[ParsedIngredient]
         List of dictionaries of structured data parsed from input sentences
 
     Examples
     ------
     >>> parse_multiple_ingredients(sentences)
     >>> sentences = [
         "3 tablespoons fresh lime juice, plus lime wedges for serving",
```

### Comparing `ingredient_parser_nlp-0.1.0b1/ingredient_parser/preprocess.py` & `ingredient_parser_nlp-0.1.0b2/ingredient_parser/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python3
 
 import re
 from fractions import Fraction
 from html import unescape
-from typing import Any, Dict, List, Union
+from typing import Any
 
 from nltk.stem.porter import PorterStemmer
 from nltk.tag import pos_tag
 from nltk.tokenize import RegexpTokenizer
 
-from ._constants import STOP_WORDS, STRING_NUMBERS_REGEXES, UNITS
+from ._constants import AMBIGUOUS_UNITS, STOP_WORDS, STRING_NUMBERS_REGEXES, UNITS
 
 # Regex pattern for fraction parts.
 # Matches 0+ numbers followed by 0+ white space characters followed by a number then
 # a forward slash then another number
 FRACTION_PARTS_PATTERN = re.compile(r"(\d*\s*\d/\d+)")
 
 # Regex pattern for checking if token starts with a capital letter
@@ -152,22 +152,22 @@
 
     Attributes
     ----------
     defer_pos_tagging : bool
         Defer part of speech tagging until feature generation
     input : str
         Input ingredient sentence.
-    pos_tags : List[str]
+    pos_tags : list[str]
         Part of speech tag for each token in the tokenized sentence.
     sentence : str
         Input ingredient sentence, cleaned to standardised form.
-    singularised_indices : List[int]
+    singularised_indices : list[int]
         Indices of tokens in tokenised sentence that have been converted from plural
         to singular
-    tokenized_sentence : List[str]
+    tokenized_sentence : list[str]
         Tokenised ingredient sentence.
     """
 
     def __init__(self, input_sentence: str, defer_pos_tagging=False):
         """Initialisation
 
         Parameters
@@ -185,15 +185,15 @@
         (
             self.tokenized_sentence,
             self.singularised_indices,
         ) = self._singlarise_units(_tokenised_sentence)
 
         self.defer_pos_tagging: bool = defer_pos_tagging
         if not defer_pos_tagging:
-            self.pos_tags: List[str] = self._tag_partofspeech(self.tokenized_sentence)
+            self.pos_tags: list[str] = self._tag_partofspeech(self.tokenized_sentence)
         else:
             self.pos_tags = []
 
     def __repr__(self) -> str:
         """__repr__ method
 
         Returns
@@ -236,14 +236,15 @@
         # Note that the order matters
         funcs = [
             self._replace_string_numbers,
             self._replace_html_fractions,
             self._replace_unicode_fractions,
             self._replace_fake_fractions,
             self._split_quantity_and_units,
+            self._remove_unit_trailing_period,
             self._replace_string_range,
         ]
 
         for func in funcs:
             sentence = func(sentence)
 
         return sentence.strip()
@@ -376,14 +377,34 @@
         Returns
         -------
         str
             Ingredient sentence with spaces inserted between quantity and units
         """
         return QUANTITY_UNITS_PATTERN.sub(r"\1 \2", sentence)
 
+    def _remove_unit_trailing_period(self, sentence: str) -> str:
+        """Remove trailling periods from units e.g. tsp. -> tsp
+
+        Parameters
+        ----------
+        sentence : str
+            Ingredient sentence
+
+        Returns
+        -------
+        str
+            Ingredient sentence with trailing periods from units removed
+        """
+        units = ["tsp.", "tsps.", "tbsp.", "tbsps.", "lb.", "lbs.", "oz."]
+        for unit in units:
+            unit_no_period = unit.replace(".", "")
+            sentence = sentence.replace(unit, unit_no_period)
+
+        return sentence
+
     def _replace_string_range(self, sentence: str) -> str:
         """Replace range in the form "<num> to <num" with
         standardised range "<num>-<num>".
 
         For example
         -----------
         1 to 2 -> 1-2
@@ -398,56 +419,58 @@
         Returns
         -------
         str
             Ingredient sentence with string ranges replaced with standardised range
         """
         return STRING_RANGE_PATTERN.sub(r"\1-\4", sentence)
 
-    def _singlarise_units(self, tokenised_sentence: List[str]) -> List[int]:
+    def _singlarise_units(
+        self, tokenised_sentence: list[str]
+    ) -> tuple[list[str], list[int]]:
         """Singularise units in tokenised sentence and return list of singularised
         indices e.g. cups -> cup, tablespoons -> tablespoon
 
         Parameters
         ----------
-        tokenised_sentence : List[str]
+        tokenised_sentence : list[str]
             Tokenised sentence
 
         Returns
         -------
-        List[str]
+        list[str]
             Tokenised sentence with units singularised
-        List[int]
+        list[int]
             List of indices of tokenised sentence that have been singularised
         """
         singularised_indices = []
         for idx, token in enumerate(tokenised_sentence):
             singular = UNITS.get(token, None)
             if singular is not None:
                 tokenised_sentence[idx] = singular
                 singularised_indices.append(idx)
 
         return (tokenised_sentence, singularised_indices)
 
-    def _tag_partofspeech(self, tokens: List[str]) -> List[str]:
+    def _tag_partofspeech(self, tokens: list[str]) -> list[str]:
         """Tag tokens with part of speech using universal tagset
 
         This function manually fixes tags that are incorrect in the context of
         ----------------------------------------------------------------------
         1. Change tags of numeric ranges to CD
         2. Change tag of "ground" from NN to VBD e.g. ground almonds
 
 
         Parameters
         ----------
-        tokens : List[str]
+        tokens : list[str]
             Tokenized ingredient sentence
 
         Returns
         -------
-        List[str]
+        list[str]
             List of part of speech tags
         """
         tags = []
         # If we don't make each token lower case, that POS tag maybe different in
         # ways that are unhelpful. For example, if a sentence starts with a unit.
         for token, tag in pos_tag([t.lower() for t in tokens]):
             if RANGE_PATTERN.match(token):
@@ -576,34 +599,50 @@
         Returns
         -------
         bool
             True if token is a stop word, else False.
         """
         return token in STOP_WORDS
 
-    def _token_features(self, index: int) -> Dict[str, Union[str, bool]]:
+    def _is_ambiguous_unit(self, token: str) -> bool:
+        """Return True if token is in AMBIGUOUS_UNITS list
+
+        Parameters
+        ----------
+        token : str
+            Token to check
+
+        Returns
+        -------
+        bool
+            True if token is in AMBIGUOUS_UNITS, else False
+        """
+        return token in AMBIGUOUS_UNITS
+
+    def _token_features(self, index: int) -> dict[str, str | bool]:
         """Return the features for each token in the sentence
 
         Parameters
         ----------
         index : int
             Index of token to get features for.
 
         Returns
         -------
-        Dict[str, Any]
+        dict[str, Any]
             Dictionary of features for token at index
         """
         token = self.tokenized_sentence[index]
         features = {
             "stem": STEMMER.stem(token),
             "pos": self.pos_tags[index],
             "is_capitalised": self._is_capitalised(token),
             "is_numeric": self._is_numeric(token),
             "is_unit": self._is_unit(token),
+            "is_ambiguous": self._is_ambiguous_unit(token),
             "is_in_parens": self._is_inside_parentheses(index),
             "is_stop_word": self._is_stop_word(token),
             "is_after_comma": self._follows_comma(index),
             "is_after_plus": self._follows_plus(index),
         }
 
         if index > 0:
@@ -620,20 +659,20 @@
 
         if index < len(self.tokenized_sentence) - 2:
             features["next_pos2"] = self.pos_tags[index + 2]
             features["next_word2"] = STEMMER.stem(self.tokenized_sentence[index + 2])
 
         return features
 
-    def sentence_features(self) -> List[Dict[str, Any]]:
+    def sentence_features(self) -> list[dict[str, Any]]:
         """Return features for all tokens in sentence
 
         Returns
         -------
-        List[Dict[str, Any]]
+        list[dict[str, Any]]
             List of features for each token in sentence
         """
         if self.defer_pos_tagging:
             # If part of speech tagging was deferred, do it now
             self.pos_tags = self._tag_partofspeech(self.tokenized_sentence)
 
         features = []
```

### Comparing `ingredient_parser_nlp-0.1.0b1/ingredient_parser/regex_parser.py` & `ingredient_parser_nlp-0.1.0b2/ingredient_parser/regex_parser.py`

 * *Files identical despite different names*

### Comparing `ingredient_parser_nlp-0.1.0b1/ingredient_parser/utils.py` & `ingredient_parser_nlp-0.1.0b2/ingredient_parser/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #!/usr/bin/env python3
 
 import re
 from itertools import groupby
 from operator import itemgetter
-from typing import Generator, Iterator, List, Union
+from typing import Generator, Iterator
 
 from ._constants import UNITS
 
 
-def find_idx(labels: List[str], key: str) -> List[int]:
+def find_idx(labels: list[str], key: str) -> list[int]:
     """Find indices of elements in list matching key.
 
     Return the indices of every element in the input list whose value is equal to the
     given key.
     If there is an element with the COMMA label before an element with label key,
     include this in the list of matched indices
 
     Parameters
     ----------
-    labels : List[str]
+    labels : list[str]
         List to search for key in
     key : str
         Key to find in list
 
     Returns
     -------
-    List[int]
+    list[int]
         List of indices of elements with label key
         Includes elements with label COMMA if the element is previous to a key label
 
     Examples
     -------
     >>> find_idx(["QTY", "UNIT", "NAME", "NAME", "COMMENT", "COMMENT"], "NAME")
     [2, 3]
@@ -45,68 +45,68 @@
                 matches.append(idx - 1)
             matches.append(idx)
 
         prev_el = el
     return matches
 
 
-def group_consecutive_idx(idx: List[int]) -> Generator[Iterator[int], None, None]:
+def group_consecutive_idx(idx: list[int]) -> Generator[Iterator[int], None, None]:
     """Yield groups of consecutive indices
 
     Given a list of integers, yield groups of integers where the value of each in a
     group is adjacent to the previous element's value.
 
     Parameters
     ----------
-    idx : List[int]
+    idx : list[int]
         List of indices
 
     Yields
     ------
-    List[List[int]]
+    list[list[int]]
         List of lists, where each sub-list contains consecutive indices
 
     Examples
     -------
     >>> groups = group_consecutive_idx([0, 1, 2, 4, 5, 6, 8, 9])
     >>> [list(g) for g in groups]
     [[0, 1, 2], [4, 5, 6], [8, 9]]
     """
     for k, g in groupby(enumerate(idx), key=lambda x: x[0] - x[1]):
         yield map(itemgetter(1), g)
 
 
-def join_adjacent(tokens: List[str], idx: List[int]) -> Union[str, List[str]]:
+def join_adjacent(tokens: list[str], idx: list[int]) -> str | list[str]:
     """Join tokens with adjacent indices in idx list into strings.
 
     Given a list of tokens and list of indices for token with a particular value,
     join all the token with adjacent indices in the idx list into space seperated
     strings.
 
     If idx is an empty list, return an empty string.
 
     If there is only one group of adjacent values in idx, return a string.
 
     If there are multiple groups of adjacent values in idx, return a list of strings.
 
     Parameters
     ----------
-    tokens : List[str]
+    tokens : list[str]
         List of ingredient sentence tokens
-    idx : List[int]
+    idx : list[int]
         Indices of tokens to group and join
 
     Returns
     -------
-    Union(str, List[str])
+    str | list[str]
         List of strings, with adjacent tokens joined
         If the list only contains one element, return as a string
 
     Examples
-    -------
+    --------
     >>> join_adjacent(["a", "b", "c", "d", "e", "f"], [0, 1, 3, 4, 5])
     ['a b', 'd e f']
     """
     grouped = []
     for group in group_consecutive_idx(idx):
         joined = " ".join([tokens[idx] for idx in group])
         grouped.append(joined)
@@ -115,26 +115,26 @@
         return ""
     elif len(grouped) == 1:
         return grouped[0]
     else:
         return grouped
 
 
-def average(labels: List[str], scores: List[float], key: str) -> float:
+def average(labels: list[str], scores: list[float], key: str) -> float:
     """Average the scores for labels matching key
 
     Given a particular label (key), find the indices of the labels that have that key.
     Then use those indices to take the average of the associated score in the scores
     input.
 
     Parameters
     ----------
-    labels : List[str]
+    labels : list[str]
         List of labels to search key for
-    scores : List[float]
+    scores : list[float]
         Confidence score for each label
     key : str
         Key to calculate confidence for
 
     Returns
     -------
     float
```

### Comparing `ingredient_parser_nlp-0.1.0b1/ingredient_parser_nlp.egg-info/PKG-INFO` & `ingredient_parser_nlp-0.1.0b2/ingredient_parser_nlp.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ingredient-parser-nlp
-Version: 0.1.0b1
+Version: 0.1.0b2
 Summary: A Python package to parse structured information from recipe ingredient sentences
 Author-email: Tom Strange <tpstrange@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tom Strange
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -52,29 +52,29 @@
 >>> from ingredient_parser import parse_ingredient
 
 >>> parse_ingredient("3 pounds pork shoulder, cut into 2-inch chunks")
 {'sentence': '3 pounds pork shoulder, cut into 2-inch chunks',
  'quantity': '3',
  'unit': 'pound',
  'name': 'pork shoulder',
- 'comment': ', cut into 2-inch chunks',
+ 'comment': 'cut into 2-inch chunks',
  'other': ''}
 
 # Output confidence for each label
 >>> parse_ingredient("3 pounds pork shoulder, cut into 2-inch chunks", confidence=True)
 {'sentence': '3 pounds pork shoulder, cut into 2-inch chunks',
  'quantity': '3',
  'unit': 'pound',
  'name': 'pork shoulder',
- 'comment': ', cut into 2-inch chunks',
+ 'comment': 'cut into 2-inch chunks',
  'other': '',
- 'confidence': {'quantity': 0.9986,
-  'unit': 0.9967,
-  'name': 0.9535,
-  'comment': 0.9967,
+ 'confidence': {'quantity': 0.9988,
+  'unit': 0.9969,
+  'name': 0.9698,
+  'comment': 0.9992,
   'other': 0}}
 ```
 
 The returned dictionary has the format
 
 ```python
 {
@@ -106,16 +106,12 @@
 ## Development
 
 The development dependencies are in the ```requirements-dev.txt``` file.
 
 Note that development includes training the model.
 
 * ```Black``` is used for code formatting.
-* ```isort``` is used for import sorting.
-
-* ```flake8``` is used for linting. Note the line length standard (E501) is ignored.
-
+* ```ruff``` is used for linting. 
 * ```pyright``` is used for type static analysis.
-
 * ```pytest``` is used for tests, with ```coverage``` being used for test coverage.
 
 The documentation dependencies are in the ```requirement-doc.txt``` file.
```

### Comparing `ingredient_parser_nlp-0.1.0b1/ingredient_parser_nlp.egg-info/SOURCES.txt` & `ingredient_parser_nlp-0.1.0b2/ingredient_parser_nlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ingredient_parser_nlp-0.1.0b1/pyproject.toml` & `ingredient_parser_nlp-0.1.0b2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -52,32 +52,19 @@
 ]
 
 [tool.black]
 target-version = ["py39"]
 include = "\\.py$"
 extend-exclude = "\\.ipynb$"
 
-[tool.isort]
-profile = "black"
-src_paths = ["ingredient_parser", "train", "tests"]
-
-
-[tool.pyright]
-include = ["ingredient_parser"]
-exclude = ["**/__pycache__"]
-
-[tool.flake8]
-max-line-length = 88
-filename = "*.py"
-extend-ignore = [
-    # import ordering set by isort
-    "E402",
-    # line breaks set by black
-    "W503",
-    # spaces around colons set by black
-    "E203",
-]
+[tool.ruff]
+select = ["E", "F", "I"]
 exclude = [
     "**/__pycache__",
     ".git",
     "venv"
-]
+]
+line-length = 88
+
+[tool.pyright]
+include = ["ingredient_parser"]
+exclude = ["**/__pycache__"]
```

### Comparing `ingredient_parser_nlp-0.1.0b1/tests/test_parser.py` & `ingredient_parser_nlp-0.1.0b2/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `ingredient_parser_nlp-0.1.0b1/tests/test_preprocess.py` & `ingredient_parser_nlp-0.1.0b2/tests/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `ingredient_parser_nlp-0.1.0b1/tests/test_utils.py` & `ingredient_parser_nlp-0.1.0b2/tests/test_utils.py`

 * *Files identical despite different names*

