# Comparing `tmp/dynamicprompts-0.7.0.tar.gz` & `tmp/dynamicprompts-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamicprompts-0.7.0.tar", max compression
+gzip compressed data, was "dynamicprompts-0.7.1.tar", max compression
```

## Comparing `dynamicprompts-0.7.0.tar` & `dynamicprompts-0.7.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1086 2023-01-28 19:37:33.719780 dynamicprompts-0.7.0/LICENSE
--rw-r--r--   0        0        0    18469 2023-02-11 10:16:53.519946 dynamicprompts-0.7.0/README.md
--rw-r--r--   0        0        0     1967 2023-02-11 10:16:53.523946 dynamicprompts-0.7.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-02-11 10:16:53.523946 dynamicprompts-0.7.0/src/dynamicprompts/__init__.py
--rw-r--r--   0        0        0      477 2023-02-11 10:15:56.188261 dynamicprompts-0.7.0/src/dynamicprompts/commands/__init__.py
--rw-r--r--   0        0        0       87 2023-02-11 10:15:56.192261 dynamicprompts-0.7.0/src/dynamicprompts/commands/base.py
--rw-r--r--   0        0        0      394 2023-02-11 10:15:56.192261 dynamicprompts-0.7.0/src/dynamicprompts/commands/literal_command.py
--rw-r--r--   0        0        0     1003 2023-02-11 10:15:56.192261 dynamicprompts-0.7.0/src/dynamicprompts/commands/sequence_command.py
--rw-r--r--   0        0        0     2029 2023-02-11 10:15:56.192261 dynamicprompts-0.7.0/src/dynamicprompts/commands/variant_command.py
--rw-r--r--   0        0        0      342 2023-02-11 10:15:56.192261 dynamicprompts-0.7.0/src/dynamicprompts/commands/wildcard_command.py
--rw-r--r--   0        0        0      227 2023-02-11 10:15:56.192261 dynamicprompts-0.7.0/src/dynamicprompts/constants.py
--rw-r--r--   0        0        0      757 2023-01-28 19:37:33.723780 dynamicprompts-0.7.0/src/dynamicprompts/generators/__init__.py
--rw-r--r--   0        0        0     1984 2023-01-28 21:14:07.862450 dynamicprompts-0.7.0/src/dynamicprompts/generators/attentiongenerator.py
--rw-r--r--   0        0        0      687 2023-01-28 21:14:07.862450 dynamicprompts-0.7.0/src/dynamicprompts/generators/batched_combinatorial.py
--rw-r--r--   0        0        0     1194 2023-02-11 10:16:53.523946 dynamicprompts-0.7.0/src/dynamicprompts/generators/combinatorial.py
--rw-r--r--   0        0        0      290 2023-01-28 21:14:07.862450 dynamicprompts-0.7.0/src/dynamicprompts/generators/dummygenerator.py
--rw-r--r--   0        0        0     1377 2023-01-28 21:14:07.862450 dynamicprompts-0.7.0/src/dynamicprompts/generators/feelinglucky.py
--rw-r--r--   0        0        0     1581 2023-02-06 08:34:25.567125 dynamicprompts-0.7.0/src/dynamicprompts/generators/jinjagenerator.py
--rw-r--r--   0        0        0     5867 2023-01-28 21:14:07.862450 dynamicprompts-0.7.0/src/dynamicprompts/generators/magicprompt.py
--rw-r--r--   0        0        0      237 2023-01-28 19:37:33.723780 dynamicprompts-0.7.0/src/dynamicprompts/generators/promptgenerator.py
--rw-r--r--   0        0        0     1516 2023-02-11 10:16:53.523946 dynamicprompts-0.7.0/src/dynamicprompts/generators/randomprompt.py
--rw-r--r--   0        0        0     2529 2023-02-05 22:33:22.967646 dynamicprompts-0.7.0/src/dynamicprompts/jinja_extensions.py
--rw-r--r--   0        0        0        0 2022-12-29 19:50:53.188526 dynamicprompts-0.7.0/src/dynamicprompts/parser/__init__.py
--rw-r--r--   0        0        0      489 2023-01-30 15:30:05.726170 dynamicprompts-0.7.0/src/dynamicprompts/parser/action_builder.py
--rw-r--r--   0        0        0      177 2023-02-11 10:16:53.523946 dynamicprompts-0.7.0/src/dynamicprompts/parser/config.py
--rw-r--r--   0        0        0     7987 2023-02-11 10:16:53.523946 dynamicprompts-0.7.0/src/dynamicprompts/parser/parse.py
--rw-r--r--   0        0        0        0 2023-01-30 17:58:40.103470 dynamicprompts-0.7.0/src/dynamicprompts/py.typed
--rw-r--r--   0        0        0      256 2023-02-11 10:15:56.192261 dynamicprompts-0.7.0/src/dynamicprompts/samplers/__init__.py
--rw-r--r--   0        0        0     2023 2023-02-11 10:16:53.523946 dynamicprompts-0.7.0/src/dynamicprompts/samplers/base.py
--rw-r--r--   0        0        0     3069 2023-02-11 10:15:56.196261 dynamicprompts-0.7.0/src/dynamicprompts/samplers/combinatorial.py
--rw-r--r--   0        0        0     3151 2023-02-11 10:16:53.523946 dynamicprompts-0.7.0/src/dynamicprompts/samplers/random.py
--rw-r--r--   0        0        0      231 2023-02-11 10:15:56.196261 dynamicprompts-0.7.0/src/dynamicprompts/utils.py
--rw-r--r--   0        0        0      947 2023-02-11 10:15:56.196261 dynamicprompts-0.7.0/src/dynamicprompts/wildcardfile.py
--rw-r--r--   0        0        0     4344 2023-02-11 10:15:56.196261 dynamicprompts-0.7.0/src/dynamicprompts/wildcardmanager.py
--rw-r--r--   0        0        0    20084 1970-01-01 00:00:00.000000 dynamicprompts-0.7.0/setup.py
--rw-r--r--   0        0        0    19940 1970-01-01 00:00:00.000000 dynamicprompts-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-02-13 12:28:30.581769 dynamicprompts-0.7.1/LICENSE
+-rw-r--r--   0        0        0    18469 2023-02-12 19:42:25.061127 dynamicprompts-0.7.1/README.md
+-rw-r--r--   0        0        0     1967 2023-02-13 12:25:57.642609 dynamicprompts-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-02-13 12:25:19.802818 dynamicprompts-0.7.1/src/dynamicprompts/__init__.py
+-rw-r--r--   0        0        0      477 2023-02-12 22:29:30.261355 dynamicprompts-0.7.1/src/dynamicprompts/commands/__init__.py
+-rw-r--r--   0        0        0       87 2023-02-12 22:29:30.261355 dynamicprompts-0.7.1/src/dynamicprompts/commands/base.py
+-rw-r--r--   0        0        0      394 2023-02-12 22:29:30.261355 dynamicprompts-0.7.1/src/dynamicprompts/commands/literal_command.py
+-rw-r--r--   0        0        0     1003 2023-02-12 22:29:30.261355 dynamicprompts-0.7.1/src/dynamicprompts/commands/sequence_command.py
+-rw-r--r--   0        0        0     2029 2023-02-12 22:29:30.261355 dynamicprompts-0.7.1/src/dynamicprompts/commands/variant_command.py
+-rw-r--r--   0        0        0      342 2023-02-12 22:29:30.261355 dynamicprompts-0.7.1/src/dynamicprompts/commands/wildcard_command.py
+-rw-r--r--   0        0        0      227 2023-02-12 22:28:16.565694 dynamicprompts-0.7.1/src/dynamicprompts/constants.py
+-rw-r--r--   0        0        0      757 2023-01-28 19:37:33.723780 dynamicprompts-0.7.1/src/dynamicprompts/generators/__init__.py
+-rw-r--r--   0        0        0     1984 2023-01-28 21:14:07.862450 dynamicprompts-0.7.1/src/dynamicprompts/generators/attentiongenerator.py
+-rw-r--r--   0        0        0      687 2023-01-28 21:14:07.862450 dynamicprompts-0.7.1/src/dynamicprompts/generators/batched_combinatorial.py
+-rw-r--r--   0        0        0     1262 2023-02-13 12:28:13.821861 dynamicprompts-0.7.1/src/dynamicprompts/generators/combinatorial.py
+-rw-r--r--   0        0        0      290 2023-01-28 21:14:07.862450 dynamicprompts-0.7.1/src/dynamicprompts/generators/dummygenerator.py
+-rw-r--r--   0        0        0     1377 2023-01-28 21:14:07.862450 dynamicprompts-0.7.1/src/dynamicprompts/generators/feelinglucky.py
+-rw-r--r--   0        0        0     1581 2023-02-06 08:34:25.567125 dynamicprompts-0.7.1/src/dynamicprompts/generators/jinjagenerator.py
+-rw-r--r--   0        0        0     5867 2023-01-28 21:14:07.862450 dynamicprompts-0.7.1/src/dynamicprompts/generators/magicprompt.py
+-rw-r--r--   0        0        0      237 2023-01-28 19:37:33.723780 dynamicprompts-0.7.1/src/dynamicprompts/generators/promptgenerator.py
+-rw-r--r--   0        0        0     1516 2023-02-12 22:29:30.261355 dynamicprompts-0.7.1/src/dynamicprompts/generators/randomprompt.py
+-rw-r--r--   0        0        0     2529 2023-02-05 22:33:22.967646 dynamicprompts-0.7.1/src/dynamicprompts/jinja_extensions.py
+-rw-r--r--   0        0        0        0 2022-12-29 19:50:53.188526 dynamicprompts-0.7.1/src/dynamicprompts/parser/__init__.py
+-rw-r--r--   0        0        0      489 2023-01-30 15:30:05.726170 dynamicprompts-0.7.1/src/dynamicprompts/parser/action_builder.py
+-rw-r--r--   0        0        0      177 2023-02-12 19:42:25.065127 dynamicprompts-0.7.1/src/dynamicprompts/parser/config.py
+-rw-r--r--   0        0        0     7987 2023-02-12 22:29:30.261355 dynamicprompts-0.7.1/src/dynamicprompts/parser/parse.py
+-rw-r--r--   0        0        0        0 2023-01-30 17:58:40.103470 dynamicprompts-0.7.1/src/dynamicprompts/py.typed
+-rw-r--r--   0        0        0      256 2023-02-12 22:29:30.261355 dynamicprompts-0.7.1/src/dynamicprompts/samplers/__init__.py
+-rw-r--r--   0        0        0     2023 2023-02-12 22:29:30.261355 dynamicprompts-0.7.1/src/dynamicprompts/samplers/base.py
+-rw-r--r--   0        0        0     3069 2023-02-12 22:29:30.261355 dynamicprompts-0.7.1/src/dynamicprompts/samplers/combinatorial.py
+-rw-r--r--   0        0        0     3151 2023-02-12 22:29:30.261355 dynamicprompts-0.7.1/src/dynamicprompts/samplers/random.py
+-rw-r--r--   0        0        0      231 2023-02-12 22:29:30.261355 dynamicprompts-0.7.1/src/dynamicprompts/utils.py
+-rw-r--r--   0        0        0      947 2023-02-12 19:42:25.065127 dynamicprompts-0.7.1/src/dynamicprompts/wildcardfile.py
+-rw-r--r--   0        0        0     4344 2023-02-12 19:42:25.065127 dynamicprompts-0.7.1/src/dynamicprompts/wildcardmanager.py
+-rw-r--r--   0        0        0    20084 1970-01-01 00:00:00.000000 dynamicprompts-0.7.1/setup.py
+-rw-r--r--   0        0        0    19940 1970-01-01 00:00:00.000000 dynamicprompts-0.7.1/PKG-INFO
```

### Comparing `dynamicprompts-0.7.0/LICENSE` & `dynamicprompts-0.7.1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2023 Adi Eyal and others
+Copyright (c) 2023 Adi Eyal and Aarni Koskela
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `dynamicprompts-0.7.0/README.md` & `dynamicprompts-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `dynamicprompts-0.7.0/pyproject.toml` & `dynamicprompts-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dynamicprompts"
-version = "0.7.0"
+version = "0.7.1"
 description = "Dynamic prompts templating library for Stable Diffusion"
 homepage = "https://github.com/adieyal/dynamicprompts"
 authors = ["Adi Eyal <adi@clearforest.io>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["stable diffusion", "prompt engineering", "automatic1111", "text2img"]
 classifiers = [
```

### Comparing `dynamicprompts-0.7.0/src/dynamicprompts/commands/sequence_command.py` & `dynamicprompts-0.7.1/src/dynamicprompts/commands/sequence_command.py`

 * *Files identical despite different names*

### Comparing `dynamicprompts-0.7.0/src/dynamicprompts/commands/variant_command.py` & `dynamicprompts-0.7.1/src/dynamicprompts/commands/variant_command.py`

 * *Files identical despite different names*

### Comparing `dynamicprompts-0.7.0/src/dynamicprompts/generators/__init__.py` & `dynamicprompts-0.7.1/src/dynamicprompts/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `dynamicprompts-0.7.0/src/dynamicprompts/generators/attentiongenerator.py` & `dynamicprompts-0.7.1/src/dynamicprompts/generators/attentiongenerator.py`

 * *Files identical despite different names*

### Comparing `dynamicprompts-0.7.0/src/dynamicprompts/generators/batched_combinatorial.py` & `dynamicprompts-0.7.1/src/dynamicprompts/generators/batched_combinatorial.py`

 * *Files identical despite different names*

### Comparing `dynamicprompts-0.7.0/src/dynamicprompts/generators/combinatorial.py` & `dynamicprompts-0.7.1/src/dynamicprompts/generators/combinatorial.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from __future__ import annotations
 
 import logging
 from typing import Iterable
 
 from dynamicprompts import constants
 from dynamicprompts.generators.promptgenerator import PromptGenerator
-from dynamicprompts.parser.parse import default_parser_config
+from dynamicprompts.parser.config import ParserConfig, default_parser_config
 from dynamicprompts.samplers.combinatorial import CombinatorialSampler
 from dynamicprompts.wildcardmanager import WildcardManager
 
 logger = logging.getLogger(__name__)
 
 
 class CombinatorialPromptGenerator(PromptGenerator):
     def __init__(
         self,
         wildcard_manager: WildcardManager,
         ignore_whitespace: bool = False,
+        parser_config: ParserConfig = default_parser_config,
     ) -> None:
         self._wildcard_manager = wildcard_manager
         self._sampler = CombinatorialSampler(
             wildcard_manager=wildcard_manager,
             ignore_whitespace=ignore_whitespace,
-            parser_config=default_parser_config,
+            parser_config=parser_config,
         )
 
     def generate(  # type: ignore[override]
         self,
         template: str | None,
         max_prompts: int | None = constants.MAX_IMAGES,
     ) -> Iterable[str]:
```

### Comparing `dynamicprompts-0.7.0/src/dynamicprompts/generators/feelinglucky.py` & `dynamicprompts-0.7.1/src/dynamicprompts/generators/feelinglucky.py`

 * *Files identical despite different names*

### Comparing `dynamicprompts-0.7.0/src/dynamicprompts/generators/jinjagenerator.py` & `dynamicprompts-0.7.1/src/dynamicprompts/generators/jinjagenerator.py`

 * *Files identical despite different names*

### Comparing `dynamicprompts-0.7.0/src/dynamicprompts/generators/magicprompt.py` & `dynamicprompts-0.7.1/src/dynamicprompts/generators/magicprompt.py`

 * *Files identical despite different names*

### Comparing `dynamicprompts-0.7.0/src/dynamicprompts/generators/randomprompt.py` & `dynamicprompts-0.7.1/src/dynamicprompts/generators/randomprompt.py`

 * *Files identical despite different names*

### Comparing `dynamicprompts-0.7.0/src/dynamicprompts/jinja_extensions.py` & `dynamicprompts-0.7.1/src/dynamicprompts/jinja_extensions.py`

 * *Files identical despite different names*

### Comparing `dynamicprompts-0.7.0/src/dynamicprompts/parser/parse.py` & `dynamicprompts-0.7.1/src/dynamicprompts/parser/parse.py`

 * *Files identical despite different names*

### Comparing `dynamicprompts-0.7.0/src/dynamicprompts/samplers/base.py` & `dynamicprompts-0.7.1/src/dynamicprompts/samplers/base.py`

 * *Files identical despite different names*

### Comparing `dynamicprompts-0.7.0/src/dynamicprompts/samplers/combinatorial.py` & `dynamicprompts-0.7.1/src/dynamicprompts/samplers/combinatorial.py`

 * *Files identical despite different names*

### Comparing `dynamicprompts-0.7.0/src/dynamicprompts/samplers/random.py` & `dynamicprompts-0.7.1/src/dynamicprompts/samplers/random.py`

 * *Files identical despite different names*

### Comparing `dynamicprompts-0.7.0/src/dynamicprompts/wildcardfile.py` & `dynamicprompts-0.7.1/src/dynamicprompts/wildcardfile.py`

 * *Files identical despite different names*

### Comparing `dynamicprompts-0.7.0/src/dynamicprompts/wildcardmanager.py` & `dynamicprompts-0.7.1/src/dynamicprompts/wildcardmanager.py`

 * *Files identical despite different names*

### Comparing `dynamicprompts-0.7.0/setup.py` & `dynamicprompts-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 extras_require = \
 {':extra == "magicprompt"': ['transformers[torch]>=4.19.2'],
  'attentiongrabber': ['spacy>=3.4.4,<4.0.0']}
 
 setup_kwargs = {
     'name': 'dynamicprompts',
-    'version': '0.7.0',
+    'version': '0.7.1',
     'description': 'Dynamic prompts templating library for Stable Diffusion',
     'long_description': '# Dynamic Prompts\nA library that provides tools and a templating language for designing prompts for text-to-image generators such as Stable Diffusion. This is useful if you would like to generate a number of new prompts using a template.\n\nThe following template\n\n\tA {house|apartment|lodge|cottage} in {summer|winter|autumn|spring} by {2$$artist1|artist2|artist3}\n\nwill produce any of the following prompts:\n\n> A **house** in **summer** by **artist1**, **artist2**<br>\n> A **lodge** in **autumn** by **artist3**, **artist1**<br>\n> A **cottage** in **winter** by **artist2**, **artist3**<br>\n> ...<br>\n\nYou can use these templates like these to search for interesting combinations of artists and styles.\n\nYou can also pick a random string from a file. Assuming you have the file seasons.txt in WILDCARD_DIR (see below), then:\n\n    __seasons__ is coming\n\nMight generate the following:\n\n> Winter is coming<br>\n> Spring is coming<br>\n> ...<br>\n\nYou can also use the same wildcard twice\n\n    I love __seasons__ better than __seasons__\n\n> I love Winter better than Summer<br>\n> I love Spring better than Spring<br>\n\nMore complete documentation can be found [below](#syntax).\n\n## Dynamic Prompts in the wild.\nDynamic Prompts has been used in:\n1. [SD Dynamic Prompts](https://github.com/adieyal/sd-dynamic-prompts/edit/main/README.md) Auto1111 extension\n2. Deforum 0.7 [colab](https://colab.research.google.com/drive/1qtYHUwFl9ocLyzDRL1_MlpQluV32ndoT?usp=sharing)\n\n## Installation\n\n`pip install dynamicprompts`\n\nAdditional functionality (see below) can be installed with this command:\n\n`pip install "dynamicprompts[magicprompt, attentiongrabber]"`\n\n## Quick Start\n\nUse the RandomPromptGenerator to create 5 random prompts using a given template:\n\n```python\nfrom pathlib import Path\nfrom dynamicprompts.wildcardmanager import WildcardManager\nfrom dynamicprompts.generators import RandomPromptGenerator\n\nWILDCARD_DIR = Path("/path/to/wildcards/directory")\nwm = WildcardManager(WILDCARD_DIR)\n\ngenerator = RandomPromptGenerator(wm)\nnum_prompts = 5\ngenerator.generate("I love {red|green|blue} roses", num_prompts)\n\n>> [\'I love blue roses\', \'I love red roses\', \'I love green roses\', \'I love red roses\', \'I love red roses\']\n```\n\nAssuming you have a file called colours.txt in /path/to/wildcards/directory with one colour per line, e.g.\n\n```\nred\ngreen\nblue\npurple\nyellow\n```\n\nthen\n\n```python\ngenerator.generate("I love __colours__ roses", num_prompts)\n>> [\'I love pink roses\', \'I love violet roses\', \'I love white roses\', \'I love violet roses\', \'I love blue roses\']\n```\n\nSee more examples below.\n\n## Combinatorial Generation\nInstead of generating random prompts from a template, combinatorial generation produced every possible prompt from the given string. For example:\n\n`I {love|hate} {New York|Chicago} in {June|July|August}`\n\nwill produce:\n> I love New York in June<br>\n> I love New York in July<br>\n> I love New York in August<br>\n> I love Chicago in June<br>\n> I love Chicago in July<br>\n> I love Chicago in August<br>\n> I hate New York in June<br>\n> I hate New York in July<br>\n> I hate New York in August<br>\n> I hate Chicago in June<br>\n> I hate Chicago in July<br>\n> I hate Chicago in August<br>\n\nIf a `__wildcard__` is provided, then a new prompt will be produced for every value in the wildcard file. For example:\n\n`My favourite season is __seasons__`\n\nwill produce:\n> My favourite season is Summer<br>\n> My favourite season is August<br>\n> My favourite season is Winter<br>\n> My favourite season is Sprint<br>\n\n### Usage\n```python\nfrom pathlib import Path\nfrom dynamicprompts.wildcardmanager import WildcardManager\nfrom dynamicprompts.generators import CombinatorialPromptGenerator\n\nWILDCARD_DIR = Path("/path/to/wildcards/directory")\nwm = WildcardManager(WILDCARD_DIR)\n\ngenerator = CombinatorialPromptGenerator(wm)\n\nnum_prompts = 5\ngenerator.generate("I love {red|green|blue} roses", num_prompts)\n\n>> [\'I love red roses\', \'I love green roses\', \'I love blue roses\']\n```\n\nNotice that only 3 prompts were generated, even though we requested 5. Since there are only three options, i.e. red, green, and blue, only 3 unique prompts can be created. `num_prompts` in this case acts as an upper bound. Combinatorial generation can very quickly produce many more prompts than you intended. `num_prompts` is a safeguard to ensure that you don\'t accidentally produced thousands or tens of thousands of prompts.\n\nConsider this template:\n\n`My favourite colours are __colours__, __colours__, and __colours__`\n\nIf colours.txt contains 10 different colours, a combinatorial enumeration of that template will create `10 * 10 * 10 = 1000` different prompts. e.g.\n\n> My favourite colours are red, green, and blue<br>\n> My favourite colours are red, green, and yellow<br>\n> My favourite colours are red, green, and purple<br>\n> My favourite colours are red, blue, and yellow<br>\n> My favourite colours are red, blue, and purple<br>\n> ...<br>\n\n\n## Magic Prompt\nUsing [Gustavosta](https://huggingface.co/Gustavosta/MagicPrompt-Stable-Diffusion)\'s MagicPrompt model, automatically generate new prompts from the input. Trained on 80,000 prompts from [Lexica.art](lexica.art), it can help give you interesting new prompts on a given subject. Here are some automatically generated variations for "dogs playing football":\n\n> dogs playing football, in the streets of a japanese town at night, with people watching in wonder, in the style of studio ghibli and makoto shinkai, highly detailed digital art, trending on artstation<br>\n> dogs playing football, in the background is a nuclear explosion. photorealism. hq. hyper. realistic. 4 k. award winning.<br>\n> dogs playing football, in the background is a nuclear explosion. photorealistic. realism. 4 k wideshot. cinematic. unreal engine. artgerm. marc simonetti. jc leyendecker<br>\n\nThis is compatible with the wildcard syntax described above.\n\nThe first time you use it, the model is downloaded. It is approximately 500mb and so will take some time depending on how fast your connection is. It will also take a few seconds on first activation as the model is loaded into memory. Note, if you\'re low in VRAM, you might get a Cuda error. My GPU uses less than 8GB by YMMV.\n\nMagic Prompt is not available by default, you need to install it as follows:\n\n`pip install "dynamicprompts[magicprompt]"`\n\nThere a few alternatives to Gusacosta\'s model available. You can try:\n\n\n`magic_generator = MagicPromptGenerator(generator, "AUTOMATIC/promptgen-lexart")`\n`magic_generator = MagicPromptGenerator(generator, "AUTOMATIC/promptgen-majinai-safe")`\n`magic_generator = MagicPromptGenerator(generator, "AUTOMATIC/promptgen-majinai-unsafe")`\n\nNote that each model requires a download of large model files.\n\n### Usage\n```python\nfrom pathlib import Path\nfrom dynamicprompts.wildcardmanager import WildcardManager\nfrom dynamicprompts.generators import RandomPromptGenerator\nfrom dynamicprompts.generators.magicprompt import MagicPromptGenerator\n\nWILDCARD_DIR = Path("/path/to/wildcards/directory")\nwm = WildcardManager(WILDCARD_DIR)\n\ngenerator = RandomPromptGenerator(wm)\nmagic_generator = MagicPromptGenerator(generator, device=0) # device = 0 for CUDA or -1 for CPU\n\nnum_prompts = 5\ngenerator.generate("I love {red|green|blue} roses", num_prompts)\n\n>> [\'I love red roses trending on artstation #vividart #pixiv\', \'I love red roses trending on artstation artwork\', \'I love blue roses breakfast club, cute, intricate, highly detailed, digital painting, artstation, concept art, smooth, sharp focus, illustration, unreal engine 5, 8 k, art by artgerm and greg rutkowski and alphonse mucha\', \'I love green roses I love green flowers, smile, Tristan Eaton, victo ngai, artgerm, RHADS, ross draws\', \'I love red roses smile, Tristan Eaton, victo ngai, artgerm, RHADS, ross draws\']\n\n```\n\n## I\'m feeling lucky\nUse the [lexica.art](https://lexica.art) API to create random prompts. Useful if you\'re looking for inspiration, or are simply too lazy to think of your own prompts. When this option is selected, the template is used as a search string. For example, prompt "Mech warrior" might return:\n\n> A large robot stone statue in the middle of a forest by Greg Rutkowski, Sung Choi, Mitchell Mohrhauser, Maciej Kuciara, Johnson Ting, Maxim Verehin, Peter Konig, final fantasy , 8k photorealistic, cinematic lighting, HD, high details, atmospheric,\n\n> a beautiful portrait painting of a ( ( ( cyberpunk ) ) ) armor by simon stalenhag and pascal blanche and alphonse mucha and nekro. in style of digital art. colorful comic, film noirs, symmetry, brush stroke, vibrating colors, hyper detailed. octane render. trending on artstation\n\n> symmetry!! portrait of a robot astronaut, floral! horizon zero dawn machine, intricate, elegant, highly detailed, digital painting, artstation, concept art, smooth, sharp focus, illustration, art by artgerm and greg rutkowski and alphonse mucha, 8 k\n\n<img src="images/feeling-lucky.png">\n\n### Usage\n\n```python\nfrom pathlib import Path\nfrom dynamicprompts.wildcardmanager import WildcardManager\nfrom dynamicprompts.generators import RandomPromptGenerator\nfrom dynamicprompts.generators.feelinglucky import FeelingLuckyGenerator\n\ngenerator = RandomPromptGenerator(wm)\nlucky_generator = FeelingLuckyGenerator(generator)\n\nnum_prompts = 5\nlucky_generator.generate("I love {red|green|blue} roses", num_prompts)\n\n>> [\'“ guns and roses ” \', \'🌹🥀🏜. 🌌🌠⭐. 💯. \', \'tattoo design, stencil, beautiful japanese girls face, roses and ivy surrounding by artgerm, artgerm, cat girl, anime \', \'rose made of glass dramatic lighting\', \'a wireframe render of a red rose\']\n\n```\n\n## Attention Generator\nIf you are using [Automatic1111](https://github.com/AUTOMATIC1111/stable-diffusion-webui/) or a similar frontend to Stable Diffusion that uses attention syntax, e.g. `(some text:1.4)`, AttentionGenerator will randomly add attention to various phrases in your prompt. This injects a small amount of randomness into your prompt.\n\n### Usage\n\n```python\nfrom pathlib import Path\nfrom dynamicprompts.wildcardmanager import WildcardManager\nfrom dynamicprompts.generators import RandomPromptGenerator\nfrom dynamicprompts.generators.attentiongenerator import AttentionGenerator\n\nWILDCARD_DIR = Path("/path/to/wildcards/directory")\nwm = WildcardManager(WILDCARD_DIR)\n\ngenerator = RandomPromptGenerator(wm)\nattention_generator = AttentionGenerator(generator)\n\nnum_prompts = 1\nprompt = "a portrait an anthropomorphic panda mage casting a spell, wearing mage robes, landscape in background, cute, dnd character art portrait, by jason felix and peter mohrbacher, cinematic lighting"\nattention_generator.generate(prompt, num_prompts)\n\n>> [\'a portrait an anthropomorphic panda mage casting a spell, wearing (mage robes:0.77), landscape in background, cute, dnd character art portrait, by jason felix and peter mohrbacher, cinematic lighting\']\n\n```\n\n<img src="images/emphasis.png">\n\nNote, AttentionGenerator is not installed by default as it needs additional libraries to run. Use this command to install it:\n\n`pip install "dynamicprompts[attentiongrabber]"`\n\nOne your first use it, a model will automatically be downloaded.\n\n# Template syntax\n\nThe templating language understands 3 different core constructs:\n* Literals - this is plain text, e.g. `A red rose`\n* [wildcards](https://github.com/adieyal/sd-dynamic-prompts/blob/main/docs/SYNTAX.md#wildcard-files) - a wildcard represent a variable that is populated from a file, e.g. `A __colours__ rose` - a prompt will be generated by randomly choosing a value from a file called colours.txt in the [wildcards directory](https://github.com/adieyal/sd-dynamic-prompts#wildcard_dir)\n* [variants or combinations](https://github.com/adieyal/sd-dynamic-prompts/blob/main/docs/SYNTAX.md#combinations) - `A {red|pink|white} rose` - Dynamic Prompts will chose one of the colours at random when generating the prompt. They are called combinations because syntax is available to choose more than one value at once, `A {2$$red|pink|white} rose` will generate one of: A red,pink rose, A red,white rose, A pink,red rose, .... etc.\n\n## Combinations\n\t{2$$opt1|opt2|opt3}\n\nThis will randomly combine two of the options for every batch, separated with a comma.  In this case, "opt1, opt2" or "opt2, opt3", or "opt1, opt3" or the same pairs in the reverse order.\n\n\t{1-3$$opt1|opt2|opt3}\n\nThis will use a random number of options between 1 and 3 for each batch.\n\nIf the number of combinations chosen is greater than the number of options listed then options may be repeated in the output.\nIf the number of combinations chosen is less than or equal to the number of options listed then the same options will not be chosen more than once.\n\n\t{4$$and$$opt1|opt2|opt3|opt4|opt5}\n\nThis will choose 4 options and join them together with \'and\' instead of the default comma. When there are multiple $$ tokens then the first item is the number of options to choose and the second option is the joiner to use.\n\n\t{-$$opt1|opt2|opt3}\n\nAn omitted minimum is assumed to be 0 and an omitted maximum is assumed to be the number of options.\n\n\t{opt1|opt2|opt3}\n\nIf you omit the `$$` prefix, one item will be selected. (Equivalent to `1$$`)\n\nOptions are chosen randomly with replacement. This means that `{2$$opt1|opt2}` can return any of the following:\n\n> opt1, opt1<br>\n> opt1, opt2<br>\n> opt2, opt1<br>\n> opt2, opt2<br>\n\nThis is useful in conjunction with wildcards (see below).\n\n\nOptions can be assigned relative weights using a `::` prefix operator.\n\n\tphoto of a {3::blue|red} ball\n\nThis will generate 3 photos of a blue ball per every 1 photo of a red ball.\n\n<img src="images/weighting-colours.png">\n\n\tphoto of a {blue|0.25::red} ball\n\nDecimals also work as expected: this will generate 4 photos of a blue ball per every 1 photo of a red ball.\n\n\tphoto portrait of a {59::white|21::latino|14::black|8::asian} {man|woman}\n\nThis would generate photo portraits of men and women of different races, proportional to the 2020 U.S. census.\n<img src="images/weighting-us-population.png">\n\nIf you omit the `::` prefix, it will have a default weight of 1.0. (Equivalent to `1::prompt`)\n\n## Wildcard files\nWildcards are text files (ending in .txt). Each line contains a term, artist name, or modifier. The wildcard file can then be embedded in your prompt by removing the .txt extension and surrounding it with double underscores. e.g:\n\n\tMy favourite colour is __colours__\n\nEmpty lines and lines starting with `#` are ignored. This can be used to add comments or disable sections of the file.\n\nMixing Combinations and Wildcards can be useful. For example,\n\n\ta photo of a {2-4$$and$$__adjective__} house\n\nwill choose between 2 and 4 options from adjective.txt, join them together with "and", for results such as "a photo of a cozy and ancient and delicate house"\n\n\n## Nesting\n\nMany constructed can nest sub-prompts. This means that you can create more advanced templates. Here are some examples:\n\n### Combinations\nYou can nest inside combinations.\n\n    {__seasons__|__timeofday__}\n\n\nThis will then either choose a season from seasons.txt or a time of day from timeofday.txt.\n\nCombinations can also be nested inside other combinations, e.g.\n\n    {{a|b|c}|d}\n\nYou can even nest complete prompts in combinations:\n\n\t{A {small|large} __monster__|A {scary|friendly} ghost}\n\nThis produce one of:\n\n> A small dragon (assuming dragon is contained in the monster.txt file)<br>\n> A large dragon<br>\n> A scary ghost<br>\n> A friendly ghost<br>\n\nIf you find that your prompts are becoming too complicated to read, consider using [whitespace](#whitespace)\n\n### Wildcard files\nWildcard files are processed recursively. If a wildcard file contains a row with dynamic syntax, then that will be resolved as well. For example if seasons.txt contains the following rows:\n\n\tSummer\n\tWinter\n\t{Autumn|Fall}\n\tSpring\n\nif the 3rd row is chosen, then either Autumn or Fall will be selected. You could go pretty wild e.g.\n\n\tSummer\n\t__winter_in_different_languages__\n\t{Autumn|Fall}\n\tSpring\n\n## Comments\nPython and c-style comments are supported:\n\n    Test string\n    # This  a comment until the end of the line\n    // this is also a comment until the end of the line\n    {A|/* this is an inline comment */B}\n\n## Whitespace\nIn most cases, whitespace is ignored which allows you to create more expressive and readable prompts, e.g.\n\n\twisdom {\n    \twoman, __colours__ eyes, braided hair\n    \t|man using a __war/weapons/swords/european__, red turban\n    \t|dwarf wielding a warhammer, __colours__ beard\n\t},\n\tknows the meaning of life, warrior, hyper-realistic, peaceful, dark fantasy, unreal engine, 8k\n\n## Syntax customisation\nTo address potential syntax clashes with other tools it is possible to change various tokens. Instead of `{red|green|blue}` you can configure the library to use the `<` `>` pair instead, e.g. `<red|green|blue>`.\n\n```python\n\nfrom pathlib import Path\nfrom dynamicprompts.wildcardmanager import WildcardManager\nfrom dynamicprompts.generators import RandomPromptGenerator\nfrom dynamicprompts.parser.config import ParserConfig\n\nWILDCARD_DIR = Path("/path/to/wildcards/directory")\nwm = WildcardManager(WILDCARD_DIR)\nparser_config = ParserConfig(variant_start="<", variant_end=">")\n\ngenerator = RandomPromptGenerator(wm, parser_config=parser_config)\n\n```\n\nCurrently only variant braces can be customised, but other tokens may be implemented in future.\n\n## Prompt development\nThe flexibility provided in the templating language makes it easy to start developing more sophisticated prompts, e.g,here is a prompt for an engagement ring.\n\n    Elegant solitaire engagement ring.\n    {classic|petite|thin|cigar|tapered|twisted}     # Band design\n    {silver|{white|rose|yellow}gold|platinum}       # Band metal\n    {round|faceted|honeycomb}                       # Band texture\n    band with a\n    {round|brilliant|oval|heart-shaped}             # Stone cut\n    __items/materials/gems__                        # Gem type.\n\nBelow are some example prompts generated from this pattern:\n> Elegant solitaire engagement ring. tapered rose gold round band with a brilliant anthophyllite<br>\n> Elegant solitaire engagement ring. thin yellow gold faceted band with a brilliant grandidierite<br>\n> Elegant solitaire engagement ring. cigar platinum faceted band with a brilliant tusionite<br>\n> Elegant solitaire engagement ring. thin yellow gold honeycomb band with a oval bowenite<br>\n> Elegant solitaire engagement ring. classic silver round band with a heart-shaped musgravite<br>\n',
     'author': 'Adi Eyal',
     'author_email': 'adi@clearforest.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/adieyal/dynamicprompts',
```

### Comparing `dynamicprompts-0.7.0/PKG-INFO` & `dynamicprompts-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamicprompts
-Version: 0.7.0
+Version: 0.7.1
 Summary: Dynamic prompts templating library for Stable Diffusion
 Home-page: https://github.com/adieyal/dynamicprompts
 License: MIT
 Keywords: stable diffusion,prompt engineering,automatic1111,text2img
 Author: Adi Eyal
 Author-email: adi@clearforest.io
 Requires-Python: >=3.7,<4.0
```

