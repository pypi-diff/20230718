# Comparing `tmp/gpteasy-1.1.2.tar.gz` & `tmp/gpteasy-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpteasy-1.1.2.tar", last modified: Sat Jun 17 22:40:07 2023, max compression
+gzip compressed data, was "gpteasy-1.1.7.tar", last modified: Tue Jul 18 14:41:53 2023, max compression
```

## Comparing `gpteasy-1.1.2.tar` & `gpteasy-1.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 22:40:07.855403 gpteasy-1.1.2/
--rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 gpteasy-1.1.2/LICENSE
--rw-r--r--   0 hp         (501) staff       (20)     5188 2023-06-17 22:40:07.855023 gpteasy-1.1.2/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)     3335 2023-06-17 22:40:00.000000 gpteasy-1.1.2/README.md
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 22:40:07.851307 gpteasy-1.1.2/gpteasy/
--rw-r--r--   0 hp         (501) staff       (20)      118 2023-06-16 09:28:57.000000 gpteasy-1.1.2/gpteasy/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     4907 2023-06-17 22:38:27.000000 gpteasy-1.1.2/gpteasy/commands.py
--rw-r--r--   0 hp         (501) staff       (20)      572 2023-06-16 09:08:00.000000 gpteasy-1.1.2/gpteasy/display.py
--rw-r--r--   0 hp         (501) staff       (20)    13176 2023-06-17 22:16:40.000000 gpteasy-1.1.2/gpteasy/gpt.py
--rw-r--r--   0 hp         (501) staff       (20)     1193 2023-06-17 13:35:36.000000 gpteasy-1.1.2/gpteasy/repl.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 22:40:07.854556 gpteasy-1.1.2/gpteasy.egg-info/
--rw-r--r--   0 hp         (501) staff       (20)     5188 2023-06-17 22:40:07.000000 gpteasy-1.1.2/gpteasy.egg-info/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)      276 2023-06-17 22:40:07.000000 gpteasy-1.1.2/gpteasy.egg-info/SOURCES.txt
--rw-r--r--   0 hp         (501) staff       (20)        1 2023-06-17 22:40:07.000000 gpteasy-1.1.2/gpteasy.egg-info/dependency_links.txt
--rw-r--r--   0 hp         (501) staff       (20)      105 2023-06-17 22:40:07.000000 gpteasy-1.1.2/gpteasy.egg-info/requires.txt
--rw-r--r--   0 hp         (501) staff       (20)        8 2023-06-17 22:40:07.000000 gpteasy-1.1.2/gpteasy.egg-info/top_level.txt
--rw-r--r--   0 hp         (501) staff       (20)     1146 2023-06-17 22:40:00.000000 gpteasy-1.1.2/pyproject.toml
--rw-r--r--   0 hp         (501) staff       (20)       38 2023-06-17 22:40:07.855534 gpteasy-1.1.2/setup.cfg
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-07-18 14:41:53.148301 gpteasy-1.1.7/
+-rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 gpteasy-1.1.7/LICENSE
+-rw-r--r--   0 hp         (501) staff       (20)     5188 2023-07-18 14:41:53.148033 gpteasy-1.1.7/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)     3335 2023-07-18 14:41:46.000000 gpteasy-1.1.7/README.md
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-07-18 14:41:53.145582 gpteasy-1.1.7/gpteasy/
+-rw-r--r--   0 hp         (501) staff       (20)      118 2023-06-16 09:28:57.000000 gpteasy-1.1.7/gpteasy/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     5420 2023-07-07 12:58:10.000000 gpteasy-1.1.7/gpteasy/commands.py
+-rw-r--r--   0 hp         (501) staff       (20)      572 2023-06-16 09:08:00.000000 gpteasy-1.1.7/gpteasy/display.py
+-rw-r--r--   0 hp         (501) staff       (20)    14647 2023-07-18 14:35:51.000000 gpteasy-1.1.7/gpteasy/gpt.py
+-rw-r--r--   0 hp         (501) staff       (20)     1193 2023-06-17 13:35:36.000000 gpteasy-1.1.7/gpteasy/repl.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-07-18 14:41:53.147644 gpteasy-1.1.7/gpteasy.egg-info/
+-rw-r--r--   0 hp         (501) staff       (20)     5188 2023-07-18 14:41:53.000000 gpteasy-1.1.7/gpteasy.egg-info/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)      276 2023-07-18 14:41:53.000000 gpteasy-1.1.7/gpteasy.egg-info/SOURCES.txt
+-rw-r--r--   0 hp         (501) staff       (20)        1 2023-07-18 14:41:53.000000 gpteasy-1.1.7/gpteasy.egg-info/dependency_links.txt
+-rw-r--r--   0 hp         (501) staff       (20)      105 2023-07-18 14:41:53.000000 gpteasy-1.1.7/gpteasy.egg-info/requires.txt
+-rw-r--r--   0 hp         (501) staff       (20)        8 2023-07-18 14:41:53.000000 gpteasy-1.1.7/gpteasy.egg-info/top_level.txt
+-rw-r--r--   0 hp         (501) staff       (20)     1146 2023-07-18 14:41:46.000000 gpteasy-1.1.7/pyproject.toml
+-rw-r--r--   0 hp         (501) staff       (20)       38 2023-07-18 14:41:53.148374 gpteasy-1.1.7/setup.cfg
```

### Comparing `gpteasy-1.1.2/LICENSE` & `gpteasy-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gpteasy-1.1.2/PKG-INFO` & `gpteasy-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpteasy
-Version: 1.1.2
+Version: 1.1.7
 Summary: Makes working with OpenAi's GPT API super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -38,15 +38,15 @@
 License-File: LICENSE
 
 # GPT Easy
 
 Package to make working with the OpenAI GPT API in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 1.1.2
+Current version: 1.1.7
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install gpteasy
 ~~~~
 2. Create an OpenAI acccount [here](https://platform.openai.com/))
```

### Comparing `gpteasy-1.1.2/README.md` & `gpteasy-1.1.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # GPT Easy
 
 Package to make working with the OpenAI GPT API in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 1.1.2
+Current version: 1.1.7
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install gpteasy
 ~~~~
 2. Create an OpenAI acccount [here](https://platform.openai.com/))
```

### Comparing `gpteasy-1.1.2/gpteasy/commands.py` & `gpteasy-1.1.7/gpteasy/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """ Handles special commands starting with : to set system parameters or model parameters """
-from .display import color_print, ERROR_COLOR, SYSTEM_COLOR
+from .display import color_print, ERROR_COLOR, SYSTEM_COLOR, ASSISTANT_COLOR
 from .gpt import GPT
 
 
 class CommandHandler:
     def __init__(self, gpt: GPT):
         self.gpt = gpt
 
         self.commands = {}
         self.add_command('quit', self.handle_quit, ":quit - Quit the program")
         self.add_command('load', self.handle_load, ":load name - loads the saved conversation with the specified name")
         self.add_command('save', self.handle_save, ":save name - saves the conversation under the specified name")
         self.add_command('debug', self.handle_debug, ":debug - set to True displays all prompts and model replies")
         self.add_command('input', self.handle_input, ":input filename - loads an input from the specified file")
         self.add_command('model', self.handle_gpt_attribute, ":model gpt-4 - Sets the AI model")
+        self.add_command('system', self.handle_system, ":system system_message - Sets the system message for the model.")
         self.add_command('max_tokens', self.handle_gpt_attribute,
                          ":max_tokens 800 - The maximum number of tokens to generate in the completion")
         self.add_command('temperature', self.handle_gpt_attribute, ":temperature 0.9 - What sampling temperature to " +
                                                                    "use, between 0 and 2")
         self.add_command('n', self.handle_gpt_attribute, ":n 1 - Specifies the number answers given")
         self.add_command('stop', self.handle_gpt_attribute, ':stop ["\\n", " Human:", " AI:"] - Up to 4 sequences ' +
                                                             'where the API will stop generating further tokens')
@@ -50,14 +51,23 @@
     def handle_save(self, filename=None):
         if not filename:
             filename = self.gpt.name
         self.gpt.save(filename)
         color_print(f"Saved to {(self.gpt.save_dir / filename).with_suffix('.txt')}\n", color=SYSTEM_COLOR)
         return True
 
+    def handle_system(self, system_message):
+        if not system_message:
+            color_print(f"Pass a system message\n", color=ERROR_COLOR)
+            return True
+        self.gpt.system_message = system_message
+        color_print(f"System message set to ", color=SYSTEM_COLOR)
+        color_print(f"{system_message}\n", color=ASSISTANT_COLOR)
+        return True
+
     def handle_reset(self):
         self.gpt.reset()
         color_print(f"Conversation reset\n", color=SYSTEM_COLOR)
         return True
 
     def handle_debug(self, debug: str=None):
         if debug is None:
```

### Comparing `gpteasy-1.1.2/gpteasy/display.py` & `gpteasy-1.1.7/gpteasy/display.py`

 * *Files identical despite different names*

### Comparing `gpteasy-1.1.2/gpteasy/gpt.py` & `gpteasy-1.1.7/gpteasy/gpt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ Handles the GPT API and the conversation state. """
 import json
 import os
 import re
+import sys
 from pathlib import Path
 
 import openai
 from tenacity import retry, wait_random_exponential, stop_after_attempt
 from dotenv import load_dotenv
 from openai.error import APIConnectionError, APIError, RateLimitError
 
@@ -160,59 +161,66 @@
         del self.functions[name]
 
     def get_functions(self):
         return [f.in_completion_format() for f in self.functions.values()] if self.functions else None
 
     def chat(self, prompt, add_to_messages=True):
 
-        @retry(wait=wait_random_exponential(min=1, max=40), stop=stop_after_attempt(3))
-        def chat_completion_request():
+        def chat_completion_request(function_call="auto"):
             if self.debug:
+                color_print(f"\nRunning completion with these messages", color=DEBUG_COLOR1)
                 for message in self.messages:
                     if hasattr(message, 'text'):
-                        color_print(f"{message.role}: {message.text}", color=DEBUG_COLOR1)
-            try:
+                        color_print(f"{message}", color=DEBUG_COLOR1)
                 if self.functions:
-                    completion = openai.ChatCompletion.create(
-                        model=self.model,
-                        messages=self.get_messages(),
-                        temperature=self.temperature,
-                        max_tokens=self.max_tokens,
-                        n=self.n,
-                        top_p=self.top_p,
-                        frequency_penalty=self.frequency_penalty,
-                        presence_penalty=self.presence_penalty,
-                        stop=self.stop,
-                        functions=self.get_functions(),
-                        function_call="auto" if self.functions else None  # auto is default, but we'll be explicit
-                    )
-                else:  # Version for models without the possibility to use functions
-                    completion = openai.ChatCompletion.create(
-                        model=self.model,
-                        messages=self.get_messages(),
-                        temperature=self.temperature,
-                        max_tokens=self.max_tokens,
-                        n=self.n,
-                        top_p=self.top_p,
-                        frequency_penalty=self.frequency_penalty,
-                        presence_penalty=self.presence_penalty,
-                        stop=self.stop
-                    )
-                if self.debug and hasattr(completion.choices[0], 'text'):
-                    color_print(f"{completion.choices[0].text}", color=DEBUG_COLOR2)
-                return completion
-            except APIConnectionError as e:
-                color_print("Connection error.", color=SYSTEM_COLOR)
-                return e
-            except APIError as e:
-                color_print("API error", color=SYSTEM_COLOR)
-                return e
-            except RateLimitError as e:
-                color_print(f"{self.model} is overloaded", color=SYSTEM_COLOR)
-                return e
+                    color_print(f"And these functions", color=DEBUG_COLOR1)
+                    for function in self.functions.values():
+                        color_print(f"{function.function_name}({function.parameters})", color=DEBUG_COLOR1)
+                print()
+
+            messages = self.get_messages()
+            for _ in range(3):
+                try:
+                    if self.functions:
+                        functions = self.get_functions()
+                        completion = openai.ChatCompletion.create(
+                            model=self.model,
+                            messages=messages,
+                            temperature=self.temperature,
+                            max_tokens=self.max_tokens,
+                            n=self.n,
+                            top_p=self.top_p,
+                            frequency_penalty=self.frequency_penalty,
+                            presence_penalty=self.presence_penalty,
+                            stop=self.stop,
+                            functions=functions,
+                            function_call=function_call
+                        )
+                    else:  # Version for models without the possibility to use functions
+                        completion = openai.ChatCompletion.create(
+                            model=self.model,
+                            messages=messages,
+                            temperature=self.temperature,
+                            max_tokens=self.max_tokens,
+                            n=self.n,
+                            top_p=self.top_p,
+                            frequency_penalty=self.frequency_penalty,
+                            presence_penalty=self.presence_penalty,
+                            stop=self.stop
+                        )
+                    if self.debug and hasattr(completion.choices[0], 'text'):
+                        color_print(f"{completion.choices[0].text}", color=DEBUG_COLOR2)
+                    return completion
+                except APIConnectionError as e:
+                    color_print("Connection error.", color=SYSTEM_COLOR)
+                except APIError as e:
+                    color_print("API error", color=SYSTEM_COLOR)
+                except RateLimitError as e:
+                    color_print(f"{self.model} is overloaded", color=SYSTEM_COLOR)
+            sys.exit('Too many errors. Aborting.')
 
         if self.messages and not self.name:
             self.name = re.sub(r'\W+', '', self.messages[0].text).replace(' ', '_')[:20]
         self.messages += [Message('user', prompt)]
 
         completion = chat_completion_request()
 
@@ -222,15 +230,18 @@
             function_to_call = self.functions[function_call["name"]]
             kwargs = json.loads(function_call["arguments"])
             function_response = function_to_call(**kwargs)
 
             self.messages += [Message('function', function_name=function_call["name"], function_content=function_response)]
 
             # get a new response from GPT where it can see the function response
-            completion = chat_completion_request()
+            completion = chat_completion_request(function_call="none")
+
+            # Special case: sometimes the model returns a sql query instead of the answer
+            # In this case explain this to the model and ask for the answer.
 
         message = Message('assistant', completion)
         if add_to_messages:
             self.messages += [message]
         return message
 
     def after_response(self, message):
@@ -298,18 +309,45 @@
             self.raw_completion = None
         else:
             self.raw_completion = text_or_completion
             self.text = text_or_completion['choices'][0]['message']['content'] if text_or_completion else ''
         self.function_name = function_name  # Name of the function called in case model called a function
         self.function_content = function_content  # Result of the function called in case model called a function
 
+    @classmethod
+    def from_dict(cls, dict):
+        message = cls()
+        for key, value in dict.items():
+            setattr(message, key, value)
+        return message
+
     def content(self):
         try:
             return json.loads(self.raw_completion['choices'][0]['message']['content'])
         except json.decoder.JSONDecodeError:
             return {'type': 'other', 'response': self.raw_completion['choices'][0]['message']['content']}
 
     def tokens(self):
         return self.raw_completion['usage']['total_tokens']
 
     def __bool__(self):
         return bool(self.raw_completion) or bool(self.text)
+
+    def __str__(self):
+        res = f'role: {self.role}'
+        if self.text:
+            res += f' text: {self.text}'
+        if self.raw_completion:
+            res += f' raw_completion: {self.raw_completion}'
+        if self.function_name:
+            res += f' function_name: {self.function_name}'
+        if self.function_content:
+            res += f' function_content: {self.function_content}'
+        return res
+
+    def to_dict(self):
+        dict = {}
+        for key, value in self.__dict__.items():
+            if value != None:
+                json.dumps(value)
+                dict[key] = value
+        return dict
```

### Comparing `gpteasy-1.1.2/gpteasy/repl.py` & `gpteasy-1.1.7/gpteasy/repl.py`

 * *Files identical despite different names*

### Comparing `gpteasy-1.1.2/gpteasy.egg-info/PKG-INFO` & `gpteasy-1.1.7/gpteasy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpteasy
-Version: 1.1.2
+Version: 1.1.7
 Summary: Makes working with OpenAi's GPT API super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -38,15 +38,15 @@
 License-File: LICENSE
 
 # GPT Easy
 
 Package to make working with the OpenAI GPT API in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 1.1.2
+Current version: 1.1.7
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install gpteasy
 ~~~~
 2. Create an OpenAI acccount [here](https://platform.openai.com/))
```

### Comparing `gpteasy-1.1.2/pyproject.toml` & `gpteasy-1.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gpteasy"
-version = "1.1.2"
+version = "1.1.7"
 description = "Makes working with OpenAi's GPT API super easy"
 readme = "README.md"
 authors = [{ name = "HP Harmsen", email = "hp@harmsen.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

