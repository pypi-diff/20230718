# Comparing `tmp/Janex-0.0.7.tar.gz` & `tmp/Janex-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Janex-0.0.7.tar", last modified: Mon Jul 17 14:59:03 2023, max compression
+gzip compressed data, was "Janex-0.0.8.tar", last modified: Tue Jul 18 02:04:42 2023, max compression
```

## Comparing `Janex-0.0.7.tar` & `Janex-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:59:03.490299 Janex-0.0.7/
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:59:03.487177 Janex-0.0.7/Janex/
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:59:03.489998 Janex-0.0.7/Janex/JanexSub/
--rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:07:05.000000 Janex-0.0.7/Janex/JanexSub/JanexSub.py
--rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:20:34.000000 Janex-0.0.7/Janex/JanexSub/__init__.py
--rw-r--r--   0 cipher     (501) staff       (20)       20 2023-07-17 14:57:49.000000 Janex-0.0.7/Janex/__init__.py
--rw-r--r--   0 cipher     (501) staff       (20)      260 2023-07-07 20:07:57.000000 Janex-0.0.7/Janex/chat.py
--rw-r--r--   0 cipher     (501) staff       (20)     5046 2023-07-17 14:57:41.000000 Janex-0.0.7/Janex/main.py
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:59:03.489695 Janex-0.0.7/Janex.egg-info/
--rw-r--r--   0 cipher     (501) staff       (20)     3398 2023-07-17 14:59:03.000000 Janex-0.0.7/Janex.egg-info/PKG-INFO
--rw-r--r--   0 cipher     (501) staff       (20)      279 2023-07-17 14:59:03.000000 Janex-0.0.7/Janex.egg-info/SOURCES.txt
--rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-17 14:59:03.000000 Janex-0.0.7/Janex.egg-info/dependency_links.txt
--rw-r--r--   0 cipher     (501) staff       (20)       12 2023-07-17 14:59:03.000000 Janex-0.0.7/Janex.egg-info/requires.txt
--rw-r--r--   0 cipher     (501) staff       (20)        6 2023-07-17 14:59:03.000000 Janex-0.0.7/Janex.egg-info/top_level.txt
--rw-r--r--   0 cipher     (501) staff       (20)     2950 2023-07-07 12:33:15.000000 Janex-0.0.7/LICENSE
--rw-r--r--   0 cipher     (501) staff       (20)     3398 2023-07-17 14:59:03.490169 Janex-0.0.7/PKG-INFO
--rw-r--r--   0 cipher     (501) staff       (20)     3029 2023-07-17 10:56:37.000000 Janex-0.0.7/README.md
--rw-r--r--   0 cipher     (501) staff       (20)     1283 2023-07-17 14:58:26.000000 Janex-0.0.7/Setup.py
--rw-r--r--   0 cipher     (501) staff       (20)       38 2023-07-17 14:59:03.490339 Janex-0.0.7/setup.cfg
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-07-18 02:04:42.720974 Janex-0.0.8/
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-07-18 02:04:42.720974 Janex-0.0.8/Janex/
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-07-18 02:04:42.720974 Janex-0.0.8/Janex/JanexSub/
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-07-09 22:55:43.000000 Janex-0.0.8/Janex/JanexSub/JanexSub.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-07-09 22:55:43.000000 Janex-0.0.8/Janex/JanexSub/__init__.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-07-17 23:57:36.000000 Janex-0.0.8/Janex/__init__.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      260 2023-07-09 22:55:43.000000 Janex-0.0.8/Janex/chat.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     5408 2023-07-18 01:59:26.000000 Janex-0.0.8/Janex/main.py
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-07-18 02:04:42.720974 Janex-0.0.8/Janex.egg-info/
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     3427 2023-07-18 02:04:42.000000 Janex-0.0.8/Janex.egg-info/PKG-INFO
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      270 2023-07-18 02:04:42.000000 Janex-0.0.8/Janex.egg-info/SOURCES.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        1 2023-07-18 02:04:42.000000 Janex-0.0.8/Janex.egg-info/dependency_links.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       12 2023-07-18 02:04:42.000000 Janex-0.0.8/Janex.egg-info/requires.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        6 2023-07-18 02:04:42.000000 Janex-0.0.8/Janex.egg-info/top_level.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     2950 2023-06-30 13:17:04.000000 Janex-0.0.8/LICENSE
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     3427 2023-07-18 02:04:42.720974 Janex-0.0.8/PKG-INFO
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     3022 2023-07-18 00:12:10.000000 Janex-0.0.8/README.md
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1319 2023-07-18 02:02:14.000000 Janex-0.0.8/Setup.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       38 2023-07-18 02:04:42.720974 Janex-0.0.8/setup.cfg
```

### Comparing `Janex-0.0.7/Janex/main.py` & `Janex-0.0.8/Janex/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -73,20 +73,23 @@
         else:
             raise ValueError("No matching intent class found.")
 
     def response_compare(self, input_string, intent_class):
         input_string_lower = input_string.lower()
         highest_similarity = 0
         similarity_percentage = 0
+        distance = 0
         most_similar_response = None
 
         responses = intent_class["responses"] if intent_class else []
 
         for response in responses:
             similarity = 0
+            Count = 0
+            InputCount = 0
             response_lower = response.lower()
             word_list = self.tokenize(response_lower)
             new_list = []
             new_bag = []
 
             for word in word_list:
                 word = self.stem(word)
@@ -99,49 +102,62 @@
 
             word_list = new_list
             word_list_2 = new_bag
             overall_word_list = word_list + word_list_2
 
             for word in word_list_2:
                 if word in word_list:
-                    similarity += 1
+            # Check if the word begins with a capital letter
+                    if word.istitle():
+                        similarity += 2  # Add 2 to the similarity for words with capital letters
+                    else:
+                        similarity += 1
+
+            response_words = self.tokenize(response)
+            input_words = self.tokenize(input_string)
+
+            for word in response_words:
+                Count += 0.01
+
+            for word in input_words:
+                InputCount += 0.01
+
+            distance = Count + InputCount / 2
+
+#            print(distance)
+
+            similarity = similarity - distance
+
+        # Calculate the similarity percentage and the distance
+            similarity_percentage = similarity / len(overall_word_list)  # Calculate average similarity
 
             if similarity > highest_similarity:
-                similarity_percentage = similarity / (len(overall_word_list) + len(word_list_2))
                 highest_similarity = similarity
                 most_similar_response = response
 
         print(f"Similarity: {similarity_percentage:.2%}")
-
-        # Convert most_similar_response back into the original string
-        for response in responses:
-            low_response_list = []
-            low_response = response.lower()
-            low_response_list = self.stem_sentence(low_response)
-
-            for low_response_word in low_response_list:
-                if low_response_word == most_similar_response:
-                    most_similar_response = response
+        print(f"Distance: {distance}")
 
         return most_similar_response
 
     def stem(self, input_word):
         suffixes = ["ing", "ly", "ed", "es", "'s", "er", "est", "y", "ily", "able", "ful", "ness", "less", "ment", "ive", "ize", "ous"]
         for suffix in suffixes:
             if input_word.endswith(suffix):
                 input_word = input_word[:-len(suffix)]
                 break
         return input_word
 
     def stem_sentence(self, input_string):
         word_list = input_string.split(" ")
         stemmed_words = []
+
         for input_word in word_list:
             word = self.stem(input_word)
-            stemmed_words.append(word)
+            stemmed_word.append(word)
 
         return stemmed_words
 
     def stem_list(self, input_list):
         stemmed_words = []
         for word in input_list:
             stemmed_word = self.stem(word)
```

### Comparing `Janex-0.0.7/Janex.egg-info/PKG-INFO` & `Janex-0.0.8/Janex.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: Janex
-Version: 0.0.7
+Version: 0.0.8
 Home-page: https://github.com/Cipher58
-Download-URL: https://github.com/Cipher58/Janex/
+Download-URL: https://github.com/Cipher58/Janex/archive/refs/tags/v0.0.2-beta.tar.gz
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -65,15 +65,15 @@
 <h5>Intent classifying:</h5>
 
 To compare the input with the patterns from your intents.json storage file, you have to declare the intents file path.
 
 ```
 intents_file_path = "intents.json"
 
-intent_class = matcher.pattern_compare(input_string, intents_file_path)
+intent_class, similarity = matcher.pattern_compare(input_string)
 
 print(intent_class)
 ```
 
 <h5>Response similarity:</h5>
 
 Sometimes a list of responses in a class can become varied in terms of context, and so in order to get the best possible response, we can use the 'responsecompare' function to compare the input string with your list of responses.
```

### Comparing `Janex-0.0.7/LICENSE` & `Janex-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `Janex-0.0.7/PKG-INFO` & `Janex-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: Janex
-Version: 0.0.7
+Version: 0.0.8
 Home-page: https://github.com/Cipher58
-Download-URL: https://github.com/Cipher58/Janex/
+Download-URL: https://github.com/Cipher58/Janex/archive/refs/tags/v0.0.2-beta.tar.gz
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -65,15 +65,15 @@
 <h5>Intent classifying:</h5>
 
 To compare the input with the patterns from your intents.json storage file, you have to declare the intents file path.
 
 ```
 intents_file_path = "intents.json"
 
-intent_class = matcher.pattern_compare(input_string, intents_file_path)
+intent_class, similarity = matcher.pattern_compare(input_string)
 
 print(intent_class)
 ```
 
 <h5>Response similarity:</h5>
 
 Sometimes a list of responses in a class can become varied in terms of context, and so in order to get the best possible response, we can use the 'responsecompare' function to compare the input string with your list of responses.
```

### Comparing `Janex-0.0.7/README.md` & `Janex-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 <h5>Intent classifying:</h5>
 
 To compare the input with the patterns from your intents.json storage file, you have to declare the intents file path.
 
 ```
 intents_file_path = "intents.json"
 
-intent_class = matcher.pattern_compare(input_string, intents_file_path)
+intent_class, similarity = matcher.pattern_compare(input_string)
 
 print(intent_class)
 ```
 
 <h5>Response similarity:</h5>
 
 Sometimes a list of responses in a class can become varied in terms of context, and so in order to get the best possible response, we can use the 'responsecompare' function to compare the input string with your list of responses.
```

### Comparing `Janex-0.0.7/Setup.py` & `Janex-0.0.8/Setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,20 +4,20 @@
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="Janex",
 
     # version of the module
-    version="0.0.7",
+    version="0.0.8",
 
     # Name of Author
     author="Cipher58",
 
-    download_url = 'https://github.com/Cipher58/Janex/',
+    download_url = 'https://github.com/Cipher58/Janex/archive/refs/tags/v0.0.2-beta.tar.gz',
 
     # your Email address
     author_email="cipher58public@gmail.com",
 
     # #Small Description about module
     # description="adding number",
```

