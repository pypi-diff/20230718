# Comparing `tmp/ghfetch-pip-1.2.5.tar.gz` & `tmp/ghfetch-pip-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghfetch-pip-1.2.5.tar", last modified: Thu Jul 13 20:57:29 2023, max compression
+gzip compressed data, was "ghfetch-pip-1.3.2.tar", last modified: Tue Jul 18 20:11:00 2023, max compression
```

## Comparing `ghfetch-pip-1.2.5.tar` & `ghfetch-pip-1.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bloodbendet  (1000) bloodbendet  (1000)        0 2023-07-13 20:57:29.626147 ghfetch-pip-1.2.5/
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)     1071 2023-07-08 19:18:11.000000 ghfetch-pip-1.2.5/LICENSE
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      234 2023-07-13 20:57:29.626147 ghfetch-pip-1.2.5/PKG-INFO
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)     1242 2023-07-13 20:55:47.000000 ghfetch-pip-1.2.5/README.md
-drwxr-xr-x   0 bloodbendet  (1000) bloodbendet  (1000)        0 2023-07-13 20:57:29.626147 ghfetch-pip-1.2.5/ghfetch/
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)        0 2023-07-13 20:55:47.000000 ghfetch-pip-1.2.5/ghfetch/__init__.py
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)    10585 2023-07-13 20:55:59.000000 ghfetch-pip-1.2.5/ghfetch/main.py
-drwxr-xr-x   0 bloodbendet  (1000) bloodbendet  (1000)        0 2023-07-13 20:57:29.626147 ghfetch-pip-1.2.5/ghfetch_pip.egg-info/
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      234 2023-07-13 20:57:29.000000 ghfetch-pip-1.2.5/ghfetch_pip.egg-info/PKG-INFO
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      284 2023-07-13 20:57:29.000000 ghfetch-pip-1.2.5/ghfetch_pip.egg-info/SOURCES.txt
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)        1 2023-07-13 20:57:29.000000 ghfetch-pip-1.2.5/ghfetch_pip.egg-info/dependency_links.txt
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)       46 2023-07-13 20:57:29.000000 ghfetch-pip-1.2.5/ghfetch_pip.egg-info/entry_points.txt
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)       20 2023-07-13 20:57:29.000000 ghfetch-pip-1.2.5/ghfetch_pip.egg-info/requires.txt
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)        8 2023-07-13 20:57:29.000000 ghfetch-pip-1.2.5/ghfetch_pip.egg-info/top_level.txt
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      219 2023-07-13 20:57:29.626147 ghfetch-pip-1.2.5/setup.cfg
--rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      483 2023-07-13 20:55:59.000000 ghfetch-pip-1.2.5/setup.py
+drwxr-xr-x   0 bloodbendet  (1000) bloodbendet  (1000)        0 2023-07-18 20:11:00.944329 ghfetch-pip-1.3.2/
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)     1071 2023-07-13 21:40:21.000000 ghfetch-pip-1.3.2/LICENSE
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      234 2023-07-18 20:11:00.944329 ghfetch-pip-1.3.2/PKG-INFO
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)     1425 2023-07-13 23:14:01.000000 ghfetch-pip-1.3.2/README.md
+drwxr-xr-x   0 bloodbendet  (1000) bloodbendet  (1000)        0 2023-07-18 20:11:00.944329 ghfetch-pip-1.3.2/ghfetch/
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)        0 2023-07-13 21:40:21.000000 ghfetch-pip-1.3.2/ghfetch/__init__.py
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)    11567 2023-07-18 19:20:55.000000 ghfetch-pip-1.3.2/ghfetch/main.py
+drwxr-xr-x   0 bloodbendet  (1000) bloodbendet  (1000)        0 2023-07-18 20:11:00.944329 ghfetch-pip-1.3.2/ghfetch_pip.egg-info/
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      234 2023-07-18 20:11:00.000000 ghfetch-pip-1.3.2/ghfetch_pip.egg-info/PKG-INFO
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      284 2023-07-18 20:11:00.000000 ghfetch-pip-1.3.2/ghfetch_pip.egg-info/SOURCES.txt
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)        1 2023-07-18 20:11:00.000000 ghfetch-pip-1.3.2/ghfetch_pip.egg-info/dependency_links.txt
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)       46 2023-07-18 20:11:00.000000 ghfetch-pip-1.3.2/ghfetch_pip.egg-info/entry_points.txt
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)       20 2023-07-18 20:11:00.000000 ghfetch-pip-1.3.2/ghfetch_pip.egg-info/requires.txt
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)        8 2023-07-18 20:11:00.000000 ghfetch-pip-1.3.2/ghfetch_pip.egg-info/top_level.txt
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      219 2023-07-18 20:11:00.944329 ghfetch-pip-1.3.2/setup.cfg
+-rw-r--r--   0 bloodbendet  (1000) bloodbendet  (1000)      483 2023-07-18 19:24:44.000000 ghfetch-pip-1.3.2/setup.py
```

### Comparing `ghfetch-pip-1.2.5/LICENSE` & `ghfetch-pip-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ghfetch-pip-1.2.5/README.md` & `ghfetch-pip-1.3.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,19 +3,25 @@
 
 ghfetch is a CLI information tool written in `Python >=3.11` that displays info about any user/org/repo you pass as argument.
 
 Upon execution, the script displays on the terminal relevant information, like the profile picture, public repos, stars, followers, etc.
 
 ## Installation
 
-<!-- ### Package manager
+### Package manager
+
 **Arch Linux:**
 ```sh
 yay -S ghfetch
-``` -->
+```
+
+**PIP:**
+```sh
+pip install ghfetch-pip
+```
 
 ### Manual installation
 ```sh
 git clone https://github.com/ghfetch/ghfetch.git
 cd ghfetch
 pip3 install -i requirements.txt
 ```
@@ -59,19 +65,23 @@
 
 ### Code 💻
 
 - [ ] Private API key for access to private repositories
 
 ### Package upload 📦
 
-- [ ] Yay
+- [X] Yay
 - [ ] Apt
-- [ ] Pip
+- [X] Pip
 - [ ] Snap
 - [ ] DNF/Yum
 - [ ] Brew
 - [ ] Windows
 - [ ] Zypper
 - [ ] DPKG
 
 ### Wishlist 🥺
-- [ ] Pacman
+- [ ] Pacman
+
+
+## People 👨‍💻
+This project was developed with ❤️ by [Nullgaro](https://github.com/nullgaro) and [Icutum](https://github.com/icutum).
```

### Comparing `ghfetch-pip-1.2.5/ghfetch/main.py` & `ghfetch-pip-1.3.2/ghfetch/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,60 @@
 #!/bin/python
-
-import sys
-import requests
-from math import floor
+from json import load
+from sys import argv
+from requests import get
+from math import floor, ceil
 from pathlib import Path
 
 # requirements
-import asyncio
-import aiohttp
-from rich import print
+from asyncio import run
+from aiohttp import request
+from rich.console import Console
 from PIL import Image
 
 HOME_PATH = Path().home()
-THIS_PATH = Path(__file__).parent.resolve()
+THIS_PATH = Path(__file__).resolve().parent.resolve()
+UNICODE_BLOCK_CHAR = '\u2588'
+LANGUAGES_BLOCK_CHAR = '\u2580'
 
 def startup():
     tmp_folder = Path(f'{HOME_PATH}/.ghfetch/tmp')
 
     Path(tmp_folder).mkdir(parents=True, exist_ok=True)
 
 async def api_call(is_repo, name):
     BASE_URL = 'https://api.github.com/'
     ENDPOINT_URL = 'repos/' if is_repo else 'users/'
 
     URL = f'{BASE_URL}{ENDPOINT_URL}{name}'
 
-    async with aiohttp.request('GET', URL) as res:
+    async with request('GET', URL) as res:
         http_status = res.status
 
         if http_status != 200:
             return http_status
 
         content = await res.json()
         return content
 
+def api_rate_exceeded(code):
+    if not isinstance(code, int):
+        return False
+
+    if code == 401:
+        print("You don't have access to this")
+    if code == 403:
+        print("This works through the Github API and looks like you've reached the hourly limit.\nTake advantage of this and go to make yourself a cup of coffee \u2615")
+    if code == 404:
+        print("The passed parameter it's not an existing User / Company / repo")
+
+    return True
+
 async def create_languages_stat(url):
-    async with aiohttp.request('GET', url) as res:
+    async with request('GET', url) as res:
         http_status = res.status
 
         if http_status != 200:
             return http_status
 
         languages = await res.json()
 
@@ -56,26 +71,26 @@
         'owner': info['owner']['login'],
         'stars': info['stargazers_count'],
         'watchers': info['watchers_count'],
         'forks': info['forks_count'],
         'archived': info['archived'],
         **({'license': info['license']['name']} if info['license'] is not None else {'license': None}),
         **({'forked_parent': info['parent']['html_url']} if info['fork'] else {}),
-        'languages': asyncio.run(create_languages_stat(info['languages_url'])),
+        'languages': run(create_languages_stat(info['languages_url'])),
     }
 
 def fetch_user(info):
     return {'company': info['company'],}
 
 def fetch_main(name):
     is_repo = '/' in name
 
-    info = asyncio.run(api_call(is_repo, name))
+    info = run(api_call(is_repo, name))
 
-    if info in (401, 404, 429):
+    if info in (401, 403, 404):
         return info
 
     generic_info = {
         **({'image': info['avatar_url']} if not is_repo else {'image': info['owner']['avatar_url']}),
         **({'description': info['bio']} if not is_repo else {'description': info['description']}),
         **({'website': info['blog']} if not is_repo else {'website': info['homepage']}),
         **({'username': info['login']} if not is_repo else {}),
@@ -103,20 +118,19 @@
 
 def rgb_to_hex(r, g, b):
     return f'#{r:02x}{g:02x}{b:02x}'
 
 def image_to_unicode(url):
     IMAGE_WIDTH = 35
     COLORED_CHAR_LENGTH = 20 # Number of characters needed in raw to print a colored unicode character [#012345]█[/#012345]
-    UNICODE_BLOCK_CHAR = '\u2588'
 
     file_name = url.split('/')[-1].split('?')[0]
     user_img_location = Path(f'{HOME_PATH}/.ghfetch/tmp/{file_name}.png')
 
-    img_data = requests.get(url).content
+    img_data = get(url).content
 
     with open(user_img_location, 'wb') as file:
         file.write(img_data)
 
     with Image.open(user_img_location) as image:
         MULTIPLIER = 0.45 # Used to fix the image height because the characters are taller
 
@@ -145,26 +159,29 @@
 
         Path.unlink(user_img_location, missing_ok=True)
 
         return unicode_per_rows
 
 def print_output(fetched_info):
     COLOR_TITLE = '#068FFF'
-    COLOR_TEXT = '#EEEEEE'
+    COLOR_TEXT = '#EDEDED'
     COLOR_ARCHIVED = '#F48024'
 
-    def title(text):
-        return f'[{COLOR_TITLE}]{text}[/{COLOR_TITLE}]'
+    def title(text, color = COLOR_TITLE):
+        return f'[{color}]{text}[/{color}]'
 
     def text(text):
         return f'[{COLOR_TEXT}]{text}[/{COLOR_TEXT}]'
 
     def archived(text):
         return f'[{COLOR_ARCHIVED}]{text}[/{COLOR_ARCHIVED}]'
 
+    def language(color):
+        return f'[{color}]{LANGUAGES_BLOCK_CHAR}[/{color}]'
+
     n = 0 # Where n is the row where to start
 
     output = image_to_unicode(fetched_info['image'])
 
     if fetched_info['type'] == 'User':
         output[n]      += title(fetched_info["username"])
         output[n + 1]  += text('-' * (len(fetched_info['username'])))
@@ -209,40 +226,56 @@
         output[n + 4] += f'{title("Description")}: {text(fetched_info["description"][:50] + "..." if (fetched_info["description"] is not None) and (len(fetched_info["description"]) > 50) else fetched_info["description"])}'
         output[n + 5] += f'{title("License")}: {text(fetched_info["license"])}'
         output[n + 6] += f'{title("Stars")}: {text(fetched_info["stars"])}'
         output[n + 7] += f'{title("Watchers")}: {text(fetched_info["watchers"])}'
         output[n + 8] += f'{title("Forks")}: {text(fetched_info["forks"])}'
         output[n + 9] += f'{title("Joined at")}: {text(fetched_info["created_at"])}'
         output[n + 10] += f'{title("Github URL")}: {text(fetched_info["github_url"])}'
-        output[n + 11] += f'{title("Langs")}: ' if len(fetched_info['languages'].items()) > 0 else ''
 
-        if len(fetched_info["languages"].items()) > 2:
-            output[n + 12] += f'{", ".join([(f"{title(k)}: {text(v)}") for k, v in fetched_info["languages"].items()][:2])}, '
-            output[n + 13] += ', '.join([(f"{title(k)}: {text(v)}") for k, v in fetched_info["languages"].items()][2:])
-        else:
-            output[n + 12] += ', '.join([(f"{title(k)}: {text(v)}") for k, v in fetched_info["languages"].items()])
+        def get_lang_color(dict, lang):
+            return (
+                dict.get(lang)
+                    .get('color') or COLOR_TEXT
+            )
+
+        with open(Path(f'{THIS_PATH}/data/language-colors.json'), 'r') as languages:
+            languages = load(languages)
+
+            if len(fetched_info["languages"].items()) > 2:
+                output[n + 13] += ', '.join([(f"{title(k, get_lang_color(languages, k))}: {text(v)}") for k, v in fetched_info["languages"].items()][:2]) + ' '
+                output[n + 14] += ', '.join([(f"{title(k, get_lang_color(languages, k))}: {text(v)}") for k, v in fetched_info["languages"].items()][2:])
+            else:
+                output[n + 13] += ', '.join([(f"{title(k, get_lang_color(languages, k))}: {text(v)}") for k, v in fetched_info["languages"].items()])
+
+
+            LENTH_BAR_DIVIDER = 3
+
+            for lang, percentage in fetched_info['languages'].items():
+                percentage = float(percentage[:-1])
+                color = get_lang_color(languages, lang)
+
+
+                cols = ceil(percentage / LENTH_BAR_DIVIDER)
+                for _ in range(cols):
+                    output[n + 12] += f'{language(color)}'
 
     for line in output:
-        print(line)
+        Console().print(line, overflow='crop', soft_wrap=True)
 
 
 def main():
     startup()
 
-    if len(sys.argv) != 2:
+    if len(argv) != 2:
         return print('Only one argument must be provided')
 
-    name = sys.argv[1]
+    name = argv[1]
 
     # API call
     fetched_info = fetch_main(name)
-    if fetched_info == 401:
-        return print("You don't have access to this")
-    if fetched_info == 404:
-        return print("The passed parameter it's not an existing User / Company / repo")
-    if fetched_info == 429:
-        return print("This works through the Github API and looks like you've reached the hourly limit.\nTake advantage of this and go to make yourself a cup of coffee\u2615")
+    if api_rate_exceeded(fetched_info):
+        return
 
     print_output(fetched_info)
 
 if __name__ == '__main__':
     main()
```

