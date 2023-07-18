# Comparing `tmp/animegifs-0.7.0.tar.gz` & `tmp/animegifs-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animegifs-0.7.0.tar", last modified: Wed Jun 14 16:36:10 2023, max compression
+gzip compressed data, was "animegifs-0.7.1.tar", last modified: Tue Jul 18 17:27:53 2023, max compression
```

## Comparing `animegifs-0.7.0.tar` & `animegifs-0.7.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 16:36:10.506571 animegifs-0.7.0/
--rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-0.7.0/LICENSE
--rw-rw-rw-   0        0        0     4084 2023-06-14 16:36:10.505571 animegifs-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     3289 2023-06-14 16:25:37.000000 animegifs-0.7.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 16:36:10.486569 animegifs-0.7.0/animegifs/
--rw-rw-rw-   0        0        0        0 2023-05-09 23:54:36.000000 animegifs-0.7.0/animegifs/__init__.py
--rw-rw-rw-   0        0        0     3739 2023-06-14 16:29:46.000000 animegifs-0.7.0/animegifs/animegifs.py
-drwxrwxrwx   0        0        0        0 2023-06-14 16:36:10.503573 animegifs-0.7.0/animegifs/distutils/
--rw-rw-rw-   0        0        0        0 2023-05-09 23:54:59.000000 animegifs-0.7.0/animegifs/distutils/__init__.py
--rw-rw-rw-   0        0        0     2331 2023-06-08 15:47:16.000000 animegifs-0.7.0/animegifs/distutils/errors.py
--rw-rw-rw-   0        0        0     1157 2023-06-14 16:22:51.000000 animegifs-0.7.0/animegifs/distutils/gifs.py
-drwxrwxrwx   0        0        0        0 2023-06-14 16:36:10.495570 animegifs-0.7.0/animegifs.egg-info/
--rw-rw-rw-   0        0        0     4084 2023-06-14 16:36:10.000000 animegifs-0.7.0/animegifs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-06-14 16:36:10.000000 animegifs-0.7.0/animegifs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 16:36:10.000000 animegifs-0.7.0/animegifs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-14 16:36:10.000000 animegifs-0.7.0/animegifs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-14 16:36:10.000000 animegifs-0.7.0/animegifs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 16:36:10.506571 animegifs-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1282 2023-06-14 16:30:12.000000 animegifs-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:27:53.175184 animegifs-0.7.1/
+-rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-0.7.1/LICENSE
+-rw-rw-rw-   0        0        0     4949 2023-07-18 17:27:53.174184 animegifs-0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4132 2023-07-18 17:24:40.000000 animegifs-0.7.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 17:27:53.152657 animegifs-0.7.1/animegifs/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:54:36.000000 animegifs-0.7.1/animegifs/__init__.py
+-rw-rw-rw-   0        0        0     3736 2023-07-18 17:09:32.000000 animegifs-0.7.1/animegifs/animegifs.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:27:53.172186 animegifs-0.7.1/animegifs/distutils/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:54:59.000000 animegifs-0.7.1/animegifs/distutils/__init__.py
+-rw-rw-rw-   0        0        0     2823 2023-07-18 17:09:32.000000 animegifs-0.7.1/animegifs/distutils/errors.py
+-rw-rw-rw-   0        0        0     1157 2023-06-14 16:22:51.000000 animegifs-0.7.1/animegifs/distutils/gifs.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:27:53.162758 animegifs-0.7.1/animegifs.egg-info/
+-rw-rw-rw-   0        0        0     4949 2023-07-18 17:27:52.000000 animegifs-0.7.1/animegifs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-07-18 17:27:52.000000 animegifs-0.7.1/animegifs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 17:27:52.000000 animegifs-0.7.1/animegifs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-07-18 17:27:52.000000 animegifs-0.7.1/animegifs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-18 17:27:52.000000 animegifs-0.7.1/animegifs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 17:27:53.175184 animegifs-0.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1283 2023-07-18 17:25:55.000000 animegifs-0.7.1/setup.py
```

### Comparing `animegifs-0.7.0/LICENSE` & `animegifs-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `animegifs-0.7.0/PKG-INFO` & `animegifs-0.7.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: animegifs
-Version: 0.7.0
+Version: 0.7.1
 Summary: Get random anime gifs by category.
 Home-page: https://github.com/MarcoSa-2000/animegifs
 Author: Marco-Sa2000
 Author-email: grest0grest@gmail.com
 License: MIT
-Keywords: anime,gif,python,anime-gif,discord
+Keywords: anime,gif,python,anime-gifs,discord
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
@@ -29,14 +29,15 @@
     <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/animegifs?logo=Python&logoColor=%23FFFF00&style=for-the-badge">
     <img alt="GitHub watchers" src="https://img.shields.io/github/watchers/MarcoSa-2000/animegifs?style=social">
 </p>
 
 Get random anime gifs by category. Use Python (intended (for now) for Discord).
 
 WIP - updated in time to time. Versions below v0.5.3 aren't expected to work flawlessly or at all. Version below v0.6 will not have the gifs library updated anymore.
+For troubleshoots, known errors and categories list, check below.
 
 `pip install animegifs`
 
 # HOW TO USE
 ```py
 #v0.5.3>
 from animegifs import animegifs
@@ -54,14 +55,29 @@
 
 gif = gifs.get_gif(category) #gifs.get_gif('hug') and return the url of the gif.
 mal = gifs.get_mal(gif) #get url of the gif's anime myanimelist page.
 title = gifs.get_animetitle(gif) #get the title of the gif's anime.
 malid = gifs.get_malId(gif) #get the ID of the gif's anime myanimelist page.
 ```
 
+```py
+#v0.6>
+from animegifs import animegifs
+
+gifs = animegifs.Animegifs()
+
+user_input = input() #let user send any input and search if that input matches a category.
+#if user_input == "nom":  #nom as category doesn't exist, but is similar to bite (as example)
+#   user_input = "bite"
+try:
+    gif = gifs.get_gif(user_input) #return the url of the gif if category exists.
+except animegifs.errors.CategoryError:
+    print("not a valid gif category.")
+```
+
 ## Category list:
 
 **A**
 * Attack
 
 **B**
 * Bite, Bloodsuck, Blush, Bonk, Brofist
@@ -118,18 +134,23 @@
 
 * Random, Steal-magic
 
 # Live API
 
 You can test out the API (and lib functionality) on my bot's website here: https://enkidu-app.github.io/animegifs
 
+# Submit a GIF
+
+If you also want to contribute to the gifs collection, you can submit a gif at: https://forms.gle/wxWmRuy5VCdDCZWp8
+
 # Troubleshooting and other
 
+The first call (only!) in the session is expected to have a slower reaction time (5-15s) because of the authentication process.
 If you encounter an error, please raise an issue on the issue page: https://github.com/MarcoSa-2000/animegifs/issues. 
-Alternatively, you can join my Discord server to request new categories, functions, provide feedback, or report any errors. 
+Alternatively, you can join my Discord server (https://discord.com/invite/TKZJ4GJj2z) to request new categories, functions, provide feedback, or report any errors. 
 I do also have a multi-function Discord bot. Feel free to check out the web dashboard here: https://enkidu-app.github.io.
 
 # Copyright
 
 This repository doesn't include any copyrighted material. 
 If you happen to come across any copyrighted content within this repository (but hosted elsewhere) that you own or represent, email me at **grest0grest@gmail.com**. 
 Please provide specific details about the copyrighted material and where it can be found.
```

#### html2text {}

```diff
@@ -1,42 +1,52 @@
-Metadata-Version: 2.1 Name: animegifs Version: 0.7.0 Summary: Get random anime
+Metadata-Version: 2.1 Name: animegifs Version: 0.7.1 Summary: Get random anime
 gifs by category. Home-page: https://github.com/MarcoSa-2000/animegifs Author:
 Marco-Sa2000 Author-email: grest0grest@gmail.com License: MIT Keywords:
-anime,gif,python,anime-gif,discord Classifier: Programming Language :: Python
+anime,gif,python,anime-gifs,discord Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: Microsoft :: Windows Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE # animegifs.py
   [PyPi_Downloads] [Discord_Server] [GitHub_release_(latest_by_date)] [PyPI -
                        Python Version] [GitHub watchers]
 Get random anime gifs by category. Use Python (intended (for now) for Discord).
 WIP - updated in time to time. Versions below v0.5.3 aren't expected to work
 flawlessly or at all. Version below v0.6 will not have the gifs library updated
-anymore. `pip install animegifs` # HOW TO USE ```py #v0.5.3> from animegifs
-import animegifs gifs = animegifs.Animegifs() gif = gifs.get_gif(category)
-#return the url of the gif. ``` ```py #v0.6> from animegifs import animegifs
-gifs = animegifs.Animegifs() gif = gifs.get_gif(category) #gifs.get_gif('hug')
-and return the url of the gif. mal = gifs.get_mal(gif) #get url of the gif's
-anime myanimelist page. title = gifs.get_animetitle(gif) #get the title of the
-gif's anime. malid = gifs.get_malId(gif) #get the ID of the gif's anime
-myanimelist page. ``` ## Category list: **A** * Attack **B** * Bite, Bloodsuck,
-Blush, Bonk, Brofist **C** * Cry, Cuddle **D** * Dance, Disgust **E** *
-Exploding **F** * Facedesk, Facepalm, Flick, Flirt **H** * Handhold, Happy,
-Harass, Highfive, Hug **I** * Icecream, Insult **K** * Kill, Kiss **L** * Lick,
-Love **M** * Marry **N** * Nod, Nosebleed, Nuzzle **P** * Pat, Peck, Poke,
-Popcorn, Pout, Punch, Punish **R** * Run **S** * Sad, Scared, ,Shoot, Shrug,
-Sip, Slap, Smirk, Sorry, Spank, Stare **T** * Tease, Threat, Tickle, Tired
-**W** * Wave **Y** * Yawn **Special Category List** * Random, Steal-magic #
-Live API You can test out the API (and lib functionality) on my bot's website
-here: https://enkidu-app.github.io/animegifs # Troubleshooting and other If you
-encounter an error, please raise an issue on the issue page: https://
-github.com/MarcoSa-2000/animegifs/issues. Alternatively, you can join my
-Discord server to request new categories, functions, provide feedback, or
-report any errors. I do also have a multi-function Discord bot. Feel free to
-check out the web dashboard here: https://enkidu-app.github.io. # Copyright
-This repository doesn't include any copyrighted material. If you happen to come
-across any copyrighted content within this repository (but hosted elsewhere)
-that you own or represent, email me at **grest0grest@gmail.com**. Please
-provide specific details about the copyrighted material and where it can be
-found. Once I confirm your claim, I'll take immediate action to remove the
-identified material.
+anymore. For troubleshoots, known errors and categories list, check below. `pip
+install animegifs` # HOW TO USE ```py #v0.5.3> from animegifs import animegifs
+gifs = animegifs.Animegifs() gif = gifs.get_gif(category) #return the url of
+the gif. ``` ```py #v0.6> from animegifs import animegifs gifs =
+animegifs.Animegifs() gif = gifs.get_gif(category) #gifs.get_gif('hug') and
+return the url of the gif. mal = gifs.get_mal(gif) #get url of the gif's anime
+myanimelist page. title = gifs.get_animetitle(gif) #get the title of the gif's
+anime. malid = gifs.get_malId(gif) #get the ID of the gif's anime myanimelist
+page. ``` ```py #v0.6> from animegifs import animegifs gifs =
+animegifs.Animegifs() user_input = input() #let user send any input and search
+if that input matches a category. #if user_input == "nom": #nom as category
+doesn't exist, but is similar to bite (as example) # user_input = "bite" try:
+gif = gifs.get_gif(user_input) #return the url of the gif if category exists.
+except animegifs.errors.CategoryError: print("not a valid gif category.") ```
+## Category list: **A** * Attack **B** * Bite, Bloodsuck, Blush, Bonk, Brofist
+**C** * Cry, Cuddle **D** * Dance, Disgust **E** * Exploding **F** * Facedesk,
+Facepalm, Flick, Flirt **H** * Handhold, Happy, Harass, Highfive, Hug **I** *
+Icecream, Insult **K** * Kill, Kiss **L** * Lick, Love **M** * Marry **N** *
+Nod, Nosebleed, Nuzzle **P** * Pat, Peck, Poke, Popcorn, Pout, Punch, Punish
+**R** * Run **S** * Sad, Scared, ,Shoot, Shrug, Sip, Slap, Smirk, Sorry, Spank,
+Stare **T** * Tease, Threat, Tickle, Tired **W** * Wave **Y** * Yawn **Special
+Category List** * Random, Steal-magic # Live API You can test out the API (and
+lib functionality) on my bot's website here: https://enkidu-app.github.io/
+animegifs # Submit a GIF If you also want to contribute to the gifs collection,
+you can submit a gif at: https://forms.gle/wxWmRuy5VCdDCZWp8 # Troubleshooting
+and other The first call (only!) in the session is expected to have a slower
+reaction time (5-15s) because of the authentication process. If you encounter
+an error, please raise an issue on the issue page: https://github.com/MarcoSa-
+2000/animegifs/issues. Alternatively, you can join my Discord server (https://
+discord.com/invite/TKZJ4GJj2z) to request new categories, functions, provide
+feedback, or report any errors. I do also have a multi-function Discord bot.
+Feel free to check out the web dashboard here: https://enkidu-app.github.io. #
+Copyright This repository doesn't include any copyrighted material. If you
+happen to come across any copyrighted content within this repository (but
+hosted elsewhere) that you own or represent, email me at
+**grest0grest@gmail.com**. Please provide specific details about the
+copyrighted material and where it can be found. Once I confirm your claim, I'll
+take immediate action to remove the identified material.
```

### Comparing `animegifs-0.7.0/README.md` & `animegifs-0.7.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/animegifs?logo=Python&logoColor=%23FFFF00&style=for-the-badge">
     <img alt="GitHub watchers" src="https://img.shields.io/github/watchers/MarcoSa-2000/animegifs?style=social">
 </p>
 
 Get random anime gifs by category. Use Python (intended (for now) for Discord).
 
 WIP - updated in time to time. Versions below v0.5.3 aren't expected to work flawlessly or at all. Version below v0.6 will not have the gifs library updated anymore.
+For troubleshoots, known errors and categories list, check below.
 
 `pip install animegifs`
 
 # HOW TO USE
 ```py
 #v0.5.3>
 from animegifs import animegifs
@@ -34,14 +35,29 @@
 
 gif = gifs.get_gif(category) #gifs.get_gif('hug') and return the url of the gif.
 mal = gifs.get_mal(gif) #get url of the gif's anime myanimelist page.
 title = gifs.get_animetitle(gif) #get the title of the gif's anime.
 malid = gifs.get_malId(gif) #get the ID of the gif's anime myanimelist page.
 ```
 
+```py
+#v0.6>
+from animegifs import animegifs
+
+gifs = animegifs.Animegifs()
+
+user_input = input() #let user send any input and search if that input matches a category.
+#if user_input == "nom":  #nom as category doesn't exist, but is similar to bite (as example)
+#   user_input = "bite"
+try:
+    gif = gifs.get_gif(user_input) #return the url of the gif if category exists.
+except animegifs.errors.CategoryError:
+    print("not a valid gif category.")
+```
+
 ## Category list:
 
 **A**
 * Attack
 
 **B**
 * Bite, Bloodsuck, Blush, Bonk, Brofist
@@ -98,18 +114,23 @@
 
 * Random, Steal-magic
 
 # Live API
 
 You can test out the API (and lib functionality) on my bot's website here: https://enkidu-app.github.io/animegifs
 
+# Submit a GIF
+
+If you also want to contribute to the gifs collection, you can submit a gif at: https://forms.gle/wxWmRuy5VCdDCZWp8
+
 # Troubleshooting and other
 
+The first call (only!) in the session is expected to have a slower reaction time (5-15s) because of the authentication process.
 If you encounter an error, please raise an issue on the issue page: https://github.com/MarcoSa-2000/animegifs/issues. 
-Alternatively, you can join my Discord server to request new categories, functions, provide feedback, or report any errors. 
+Alternatively, you can join my Discord server (https://discord.com/invite/TKZJ4GJj2z) to request new categories, functions, provide feedback, or report any errors. 
 I do also have a multi-function Discord bot. Feel free to check out the web dashboard here: https://enkidu-app.github.io.
 
 # Copyright
 
 This repository doesn't include any copyrighted material. 
 If you happen to come across any copyrighted content within this repository (but hosted elsewhere) that you own or represent, email me at **grest0grest@gmail.com**. 
 Please provide specific details about the copyrighted material and where it can be found.
```

#### html2text {}

```diff
@@ -1,34 +1,44 @@
 # animegifs.py
   [PyPi_Downloads] [Discord_Server] [GitHub_release_(latest_by_date)] [PyPI -
                        Python Version] [GitHub watchers]
 Get random anime gifs by category. Use Python (intended (for now) for Discord).
 WIP - updated in time to time. Versions below v0.5.3 aren't expected to work
 flawlessly or at all. Version below v0.6 will not have the gifs library updated
-anymore. `pip install animegifs` # HOW TO USE ```py #v0.5.3> from animegifs
-import animegifs gifs = animegifs.Animegifs() gif = gifs.get_gif(category)
-#return the url of the gif. ``` ```py #v0.6> from animegifs import animegifs
-gifs = animegifs.Animegifs() gif = gifs.get_gif(category) #gifs.get_gif('hug')
-and return the url of the gif. mal = gifs.get_mal(gif) #get url of the gif's
-anime myanimelist page. title = gifs.get_animetitle(gif) #get the title of the
-gif's anime. malid = gifs.get_malId(gif) #get the ID of the gif's anime
-myanimelist page. ``` ## Category list: **A** * Attack **B** * Bite, Bloodsuck,
-Blush, Bonk, Brofist **C** * Cry, Cuddle **D** * Dance, Disgust **E** *
-Exploding **F** * Facedesk, Facepalm, Flick, Flirt **H** * Handhold, Happy,
-Harass, Highfive, Hug **I** * Icecream, Insult **K** * Kill, Kiss **L** * Lick,
-Love **M** * Marry **N** * Nod, Nosebleed, Nuzzle **P** * Pat, Peck, Poke,
-Popcorn, Pout, Punch, Punish **R** * Run **S** * Sad, Scared, ,Shoot, Shrug,
-Sip, Slap, Smirk, Sorry, Spank, Stare **T** * Tease, Threat, Tickle, Tired
-**W** * Wave **Y** * Yawn **Special Category List** * Random, Steal-magic #
-Live API You can test out the API (and lib functionality) on my bot's website
-here: https://enkidu-app.github.io/animegifs # Troubleshooting and other If you
-encounter an error, please raise an issue on the issue page: https://
-github.com/MarcoSa-2000/animegifs/issues. Alternatively, you can join my
-Discord server to request new categories, functions, provide feedback, or
-report any errors. I do also have a multi-function Discord bot. Feel free to
-check out the web dashboard here: https://enkidu-app.github.io. # Copyright
-This repository doesn't include any copyrighted material. If you happen to come
-across any copyrighted content within this repository (but hosted elsewhere)
-that you own or represent, email me at **grest0grest@gmail.com**. Please
-provide specific details about the copyrighted material and where it can be
-found. Once I confirm your claim, I'll take immediate action to remove the
-identified material.
+anymore. For troubleshoots, known errors and categories list, check below. `pip
+install animegifs` # HOW TO USE ```py #v0.5.3> from animegifs import animegifs
+gifs = animegifs.Animegifs() gif = gifs.get_gif(category) #return the url of
+the gif. ``` ```py #v0.6> from animegifs import animegifs gifs =
+animegifs.Animegifs() gif = gifs.get_gif(category) #gifs.get_gif('hug') and
+return the url of the gif. mal = gifs.get_mal(gif) #get url of the gif's anime
+myanimelist page. title = gifs.get_animetitle(gif) #get the title of the gif's
+anime. malid = gifs.get_malId(gif) #get the ID of the gif's anime myanimelist
+page. ``` ```py #v0.6> from animegifs import animegifs gifs =
+animegifs.Animegifs() user_input = input() #let user send any input and search
+if that input matches a category. #if user_input == "nom": #nom as category
+doesn't exist, but is similar to bite (as example) # user_input = "bite" try:
+gif = gifs.get_gif(user_input) #return the url of the gif if category exists.
+except animegifs.errors.CategoryError: print("not a valid gif category.") ```
+## Category list: **A** * Attack **B** * Bite, Bloodsuck, Blush, Bonk, Brofist
+**C** * Cry, Cuddle **D** * Dance, Disgust **E** * Exploding **F** * Facedesk,
+Facepalm, Flick, Flirt **H** * Handhold, Happy, Harass, Highfive, Hug **I** *
+Icecream, Insult **K** * Kill, Kiss **L** * Lick, Love **M** * Marry **N** *
+Nod, Nosebleed, Nuzzle **P** * Pat, Peck, Poke, Popcorn, Pout, Punch, Punish
+**R** * Run **S** * Sad, Scared, ,Shoot, Shrug, Sip, Slap, Smirk, Sorry, Spank,
+Stare **T** * Tease, Threat, Tickle, Tired **W** * Wave **Y** * Yawn **Special
+Category List** * Random, Steal-magic # Live API You can test out the API (and
+lib functionality) on my bot's website here: https://enkidu-app.github.io/
+animegifs # Submit a GIF If you also want to contribute to the gifs collection,
+you can submit a gif at: https://forms.gle/wxWmRuy5VCdDCZWp8 # Troubleshooting
+and other The first call (only!) in the session is expected to have a slower
+reaction time (5-15s) because of the authentication process. If you encounter
+an error, please raise an issue on the issue page: https://github.com/MarcoSa-
+2000/animegifs/issues. Alternatively, you can join my Discord server (https://
+discord.com/invite/TKZJ4GJj2z) to request new categories, functions, provide
+feedback, or report any errors. I do also have a multi-function Discord bot.
+Feel free to check out the web dashboard here: https://enkidu-app.github.io. #
+Copyright This repository doesn't include any copyrighted material. If you
+happen to come across any copyrighted content within this repository (but
+hosted elsewhere) that you own or represent, email me at
+**grest0grest@gmail.com**. Please provide specific details about the
+copyrighted material and where it can be found. Once I confirm your claim, I'll
+take immediate action to remove the identified material.
```

### Comparing `animegifs-0.7.0/animegifs/animegifs.py` & `animegifs-0.7.1/animegifs/animegifs.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,11 +98,11 @@
         for key, gif_url in gifs.access().items():
             for gif_name in gif_url:
                 if gif_name[0] == gif:
                     result = gif_name[1]
                     try:
                         title = Anime(int(result)).title
                     except ValueError as exc:
-                        raise errors.MethodNotUpdated(gif) from exc
+                        raise errors.AnimeNotFound(gif) from exc
                     return title
             else:
                 continue
```

### Comparing `animegifs-0.7.0/animegifs/distutils/errors.py` & `animegifs-0.7.1/animegifs/distutils/errors.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,14 +39,26 @@
     """
 
     def __init__(self, gif, error="Method not yet available for this gif."):
         self.gif = gif
         self.error = error
         super().__init__(self.error)
 
+class AnimeNotFound(Exception):
+    """
+    Raised if the anime's id is either invalid or has been removed or relocated.
+    Check firstly if myanimelist.net is working correctly, if confirmed,
+    please raise an issue in https://github.com/MarcoSa-2000/animegifs/issues.
+    """
+
+    def __init__(self, gif, error="Anime's ID is either invalid, removed or MyAnimeList is currently down."):
+        self.gif = gif
+        self.error = error
+        super().__init__(self.error)
+
 class AuthTimeout(Exception):
     """
     Authentication request timed out. Probably status error 504 on server side.
     Check your connection too.
     """
 
     def __init__(self, exc, error="Authentication request timed out."):
```

### Comparing `animegifs-0.7.0/animegifs/distutils/gifs.py` & `animegifs-0.7.1/animegifs/distutils/gifs.py`

 * *Files identical despite different names*

### Comparing `animegifs-0.7.0/animegifs.egg-info/PKG-INFO` & `animegifs-0.7.1/animegifs.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: animegifs
-Version: 0.7.0
+Version: 0.7.1
 Summary: Get random anime gifs by category.
 Home-page: https://github.com/MarcoSa-2000/animegifs
 Author: Marco-Sa2000
 Author-email: grest0grest@gmail.com
 License: MIT
-Keywords: anime,gif,python,anime-gif,discord
+Keywords: anime,gif,python,anime-gifs,discord
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
@@ -29,14 +29,15 @@
     <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/animegifs?logo=Python&logoColor=%23FFFF00&style=for-the-badge">
     <img alt="GitHub watchers" src="https://img.shields.io/github/watchers/MarcoSa-2000/animegifs?style=social">
 </p>
 
 Get random anime gifs by category. Use Python (intended (for now) for Discord).
 
 WIP - updated in time to time. Versions below v0.5.3 aren't expected to work flawlessly or at all. Version below v0.6 will not have the gifs library updated anymore.
+For troubleshoots, known errors and categories list, check below.
 
 `pip install animegifs`
 
 # HOW TO USE
 ```py
 #v0.5.3>
 from animegifs import animegifs
@@ -54,14 +55,29 @@
 
 gif = gifs.get_gif(category) #gifs.get_gif('hug') and return the url of the gif.
 mal = gifs.get_mal(gif) #get url of the gif's anime myanimelist page.
 title = gifs.get_animetitle(gif) #get the title of the gif's anime.
 malid = gifs.get_malId(gif) #get the ID of the gif's anime myanimelist page.
 ```
 
+```py
+#v0.6>
+from animegifs import animegifs
+
+gifs = animegifs.Animegifs()
+
+user_input = input() #let user send any input and search if that input matches a category.
+#if user_input == "nom":  #nom as category doesn't exist, but is similar to bite (as example)
+#   user_input = "bite"
+try:
+    gif = gifs.get_gif(user_input) #return the url of the gif if category exists.
+except animegifs.errors.CategoryError:
+    print("not a valid gif category.")
+```
+
 ## Category list:
 
 **A**
 * Attack
 
 **B**
 * Bite, Bloodsuck, Blush, Bonk, Brofist
@@ -118,18 +134,23 @@
 
 * Random, Steal-magic
 
 # Live API
 
 You can test out the API (and lib functionality) on my bot's website here: https://enkidu-app.github.io/animegifs
 
+# Submit a GIF
+
+If you also want to contribute to the gifs collection, you can submit a gif at: https://forms.gle/wxWmRuy5VCdDCZWp8
+
 # Troubleshooting and other
 
+The first call (only!) in the session is expected to have a slower reaction time (5-15s) because of the authentication process.
 If you encounter an error, please raise an issue on the issue page: https://github.com/MarcoSa-2000/animegifs/issues. 
-Alternatively, you can join my Discord server to request new categories, functions, provide feedback, or report any errors. 
+Alternatively, you can join my Discord server (https://discord.com/invite/TKZJ4GJj2z) to request new categories, functions, provide feedback, or report any errors. 
 I do also have a multi-function Discord bot. Feel free to check out the web dashboard here: https://enkidu-app.github.io.
 
 # Copyright
 
 This repository doesn't include any copyrighted material. 
 If you happen to come across any copyrighted content within this repository (but hosted elsewhere) that you own or represent, email me at **grest0grest@gmail.com**. 
 Please provide specific details about the copyrighted material and where it can be found.
```

#### html2text {}

```diff
@@ -1,42 +1,52 @@
-Metadata-Version: 2.1 Name: animegifs Version: 0.7.0 Summary: Get random anime
+Metadata-Version: 2.1 Name: animegifs Version: 0.7.1 Summary: Get random anime
 gifs by category. Home-page: https://github.com/MarcoSa-2000/animegifs Author:
 Marco-Sa2000 Author-email: grest0grest@gmail.com License: MIT Keywords:
-anime,gif,python,anime-gif,discord Classifier: Programming Language :: Python
+anime,gif,python,anime-gifs,discord Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: Microsoft :: Windows Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE # animegifs.py
   [PyPi_Downloads] [Discord_Server] [GitHub_release_(latest_by_date)] [PyPI -
                        Python Version] [GitHub watchers]
 Get random anime gifs by category. Use Python (intended (for now) for Discord).
 WIP - updated in time to time. Versions below v0.5.3 aren't expected to work
 flawlessly or at all. Version below v0.6 will not have the gifs library updated
-anymore. `pip install animegifs` # HOW TO USE ```py #v0.5.3> from animegifs
-import animegifs gifs = animegifs.Animegifs() gif = gifs.get_gif(category)
-#return the url of the gif. ``` ```py #v0.6> from animegifs import animegifs
-gifs = animegifs.Animegifs() gif = gifs.get_gif(category) #gifs.get_gif('hug')
-and return the url of the gif. mal = gifs.get_mal(gif) #get url of the gif's
-anime myanimelist page. title = gifs.get_animetitle(gif) #get the title of the
-gif's anime. malid = gifs.get_malId(gif) #get the ID of the gif's anime
-myanimelist page. ``` ## Category list: **A** * Attack **B** * Bite, Bloodsuck,
-Blush, Bonk, Brofist **C** * Cry, Cuddle **D** * Dance, Disgust **E** *
-Exploding **F** * Facedesk, Facepalm, Flick, Flirt **H** * Handhold, Happy,
-Harass, Highfive, Hug **I** * Icecream, Insult **K** * Kill, Kiss **L** * Lick,
-Love **M** * Marry **N** * Nod, Nosebleed, Nuzzle **P** * Pat, Peck, Poke,
-Popcorn, Pout, Punch, Punish **R** * Run **S** * Sad, Scared, ,Shoot, Shrug,
-Sip, Slap, Smirk, Sorry, Spank, Stare **T** * Tease, Threat, Tickle, Tired
-**W** * Wave **Y** * Yawn **Special Category List** * Random, Steal-magic #
-Live API You can test out the API (and lib functionality) on my bot's website
-here: https://enkidu-app.github.io/animegifs # Troubleshooting and other If you
-encounter an error, please raise an issue on the issue page: https://
-github.com/MarcoSa-2000/animegifs/issues. Alternatively, you can join my
-Discord server to request new categories, functions, provide feedback, or
-report any errors. I do also have a multi-function Discord bot. Feel free to
-check out the web dashboard here: https://enkidu-app.github.io. # Copyright
-This repository doesn't include any copyrighted material. If you happen to come
-across any copyrighted content within this repository (but hosted elsewhere)
-that you own or represent, email me at **grest0grest@gmail.com**. Please
-provide specific details about the copyrighted material and where it can be
-found. Once I confirm your claim, I'll take immediate action to remove the
-identified material.
+anymore. For troubleshoots, known errors and categories list, check below. `pip
+install animegifs` # HOW TO USE ```py #v0.5.3> from animegifs import animegifs
+gifs = animegifs.Animegifs() gif = gifs.get_gif(category) #return the url of
+the gif. ``` ```py #v0.6> from animegifs import animegifs gifs =
+animegifs.Animegifs() gif = gifs.get_gif(category) #gifs.get_gif('hug') and
+return the url of the gif. mal = gifs.get_mal(gif) #get url of the gif's anime
+myanimelist page. title = gifs.get_animetitle(gif) #get the title of the gif's
+anime. malid = gifs.get_malId(gif) #get the ID of the gif's anime myanimelist
+page. ``` ```py #v0.6> from animegifs import animegifs gifs =
+animegifs.Animegifs() user_input = input() #let user send any input and search
+if that input matches a category. #if user_input == "nom": #nom as category
+doesn't exist, but is similar to bite (as example) # user_input = "bite" try:
+gif = gifs.get_gif(user_input) #return the url of the gif if category exists.
+except animegifs.errors.CategoryError: print("not a valid gif category.") ```
+## Category list: **A** * Attack **B** * Bite, Bloodsuck, Blush, Bonk, Brofist
+**C** * Cry, Cuddle **D** * Dance, Disgust **E** * Exploding **F** * Facedesk,
+Facepalm, Flick, Flirt **H** * Handhold, Happy, Harass, Highfive, Hug **I** *
+Icecream, Insult **K** * Kill, Kiss **L** * Lick, Love **M** * Marry **N** *
+Nod, Nosebleed, Nuzzle **P** * Pat, Peck, Poke, Popcorn, Pout, Punch, Punish
+**R** * Run **S** * Sad, Scared, ,Shoot, Shrug, Sip, Slap, Smirk, Sorry, Spank,
+Stare **T** * Tease, Threat, Tickle, Tired **W** * Wave **Y** * Yawn **Special
+Category List** * Random, Steal-magic # Live API You can test out the API (and
+lib functionality) on my bot's website here: https://enkidu-app.github.io/
+animegifs # Submit a GIF If you also want to contribute to the gifs collection,
+you can submit a gif at: https://forms.gle/wxWmRuy5VCdDCZWp8 # Troubleshooting
+and other The first call (only!) in the session is expected to have a slower
+reaction time (5-15s) because of the authentication process. If you encounter
+an error, please raise an issue on the issue page: https://github.com/MarcoSa-
+2000/animegifs/issues. Alternatively, you can join my Discord server (https://
+discord.com/invite/TKZJ4GJj2z) to request new categories, functions, provide
+feedback, or report any errors. I do also have a multi-function Discord bot.
+Feel free to check out the web dashboard here: https://enkidu-app.github.io. #
+Copyright This repository doesn't include any copyrighted material. If you
+happen to come across any copyrighted content within this repository (but
+hosted elsewhere) that you own or represent, email me at
+**grest0grest@gmail.com**. Please provide specific details about the
+copyrighted material and where it can be found. Once I confirm your claim, I'll
+take immediate action to remove the identified material.
```

### Comparing `animegifs-0.7.0/setup.py` & `animegifs-0.7.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 LONG_DESCRIPTION = long_description
-VERSION = '0.7.0'
+VERSION = '0.7.1'
 
 setup(
     name='animegifs',
     package_dir={"anime_gifs": "animegifs"},
     packages=["animegifs", "animegifs.distutils"],
     version=VERSION,
     description='Get random anime gifs by category.',
@@ -31,9 +31,9 @@
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: Microsoft :: Windows"],
-    keywords=['anime', 'gif', 'python', 'anime-gif', 'discord'],
+    keywords=['anime', 'gif', 'python', 'anime-gifs', 'discord'],
 )
```

