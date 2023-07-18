# Comparing `tmp/anicli-ru-4.2.3.tar.gz` & `tmp/anicli_ru-4.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anicli-ru-4.2.3.tar", last modified: Wed Jun 28 19:53:01 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `anicli-ru-4.2.3.tar` & `anicli_ru-4.2.4.tar`

### file list

```diff
@@ -1,35 +1,24 @@
-drwxr-xr-x   0 georgiy   (1000) georgiy   (1000)        0 2023-06-28 19:53:01.844024 anicli-ru-4.2.3/
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)    35148 2021-11-01 12:04:16.000000 anicli-ru-4.2.3/LICENSE
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)     4288 2023-06-28 19:53:01.845024 anicli-ru-4.2.3/PKG-INFO
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)     3992 2023-03-29 06:40:38.000000 anicli-ru-4.2.3/README.md
-drwxr-xr-x   0 georgiy   (1000) georgiy   (1000)        0 2023-06-28 19:53:01.831024 anicli-ru-4.2.3/anicli_ru/
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)       72 2023-03-29 06:40:38.000000 anicli-ru-4.2.3/anicli_ru/__init__.py
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)       93 2023-03-29 06:40:38.000000 anicli-ru-4.2.3/anicli_ru/__main__.py
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)       52 2023-06-28 19:48:21.000000 anicli-ru-4.2.3/anicli_ru/__version__.py
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)     1117 2023-03-29 06:40:38.000000 anicli-ru-4.2.3/anicli_ru/_http.py
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)     4051 2023-03-29 06:40:38.000000 anicli-ru-4.2.3/anicli_ru/aniboom.py
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)    10051 2023-06-28 19:46:31.000000 anicli-ru-4.2.3/anicli_ru/anicli.py
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)    12327 2023-06-28 14:41:08.000000 anicli-ru-4.2.3/anicli_ru/base.py
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)     2988 2023-03-30 19:09:16.000000 anicli-ru-4.2.3/anicli_ru/defaults.py
-drwxr-xr-x   0 georgiy   (1000) georgiy   (1000)        0 2023-06-28 19:53:01.840024 anicli-ru-4.2.3/anicli_ru/extractors/
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)        0 2023-03-29 06:40:33.000000 anicli-ru-4.2.3/anicli_ru/extractors/__init__.py
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)     2090 2023-03-29 06:40:38.000000 anicli-ru-4.2.3/anicli_ru/extractors/__template__.py
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)     4437 2023-03-29 06:40:38.000000 anicli-ru-4.2.3/anicli_ru/extractors/anilibria.py
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)     4638 2023-03-29 06:40:38.000000 anicli-ru-4.2.3/anicli_ru/extractors/animania.py
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)     5598 2023-06-28 14:41:00.000000 anicli-ru-4.2.3/anicli_ru/extractors/animego.py
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)     4518 2023-03-29 06:40:38.000000 anicli-ru-4.2.3/anicli_ru/extractors/animevost.py
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)     6970 2023-06-28 14:40:22.000000 anicli-ru-4.2.3/anicli_ru/kodik.py
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)     2089 2023-03-29 06:40:38.000000 anicli-ru-4.2.3/anicli_ru/loader.py
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)     6405 2023-03-29 06:40:38.000000 anicli-ru-4.2.3/anicli_ru/options.py
-drwxr-xr-x   0 georgiy   (1000) georgiy   (1000)        0 2023-06-28 19:53:01.843024 anicli-ru-4.2.3/anicli_ru/utils/
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)       47 2023-03-29 06:40:38.000000 anicli-ru-4.2.3/anicli_ru/utils/__init__.py
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)     2371 2023-03-29 06:40:38.000000 anicli-ru-4.2.3/anicli_ru/utils/random_agent.py
-drwxr-xr-x   0 georgiy   (1000) georgiy   (1000)        0 2023-06-28 19:53:01.833024 anicli-ru-4.2.3/anicli_ru.egg-info/
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)     4288 2023-06-28 19:53:01.000000 anicli-ru-4.2.3/anicli_ru.egg-info/PKG-INFO
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)      728 2023-06-28 19:53:01.000000 anicli-ru-4.2.3/anicli_ru.egg-info/SOURCES.txt
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)        1 2023-06-28 19:53:01.000000 anicli-ru-4.2.3/anicli_ru.egg-info/dependency_links.txt
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)       52 2023-06-28 19:53:01.000000 anicli-ru-4.2.3/anicli_ru.egg-info/entry_points.txt
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)        9 2023-06-28 19:53:01.000000 anicli-ru-4.2.3/anicli_ru.egg-info/requires.txt
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)       10 2023-06-28 19:53:01.000000 anicli-ru-4.2.3/anicli_ru.egg-info/top_level.txt
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)      428 2023-06-28 19:53:01.847024 anicli-ru-4.2.3/setup.cfg
--rw-r--r--   0 georgiy   (1000) georgiy   (1000)      687 2023-03-30 19:11:50.000000 anicli-ru-4.2.3/setup.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 anicli_ru-4.2.4/anicli_ru/__init__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 anicli_ru-4.2.4/anicli_ru/__main__.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 anicli_ru-4.2.4/anicli_ru/__version__.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 anicli_ru-4.2.4/anicli_ru/_http.py
+-rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 anicli_ru-4.2.4/anicli_ru/aniboom.py
+-rw-r--r--   0        0        0    10051 2020-02-02 00:00:00.000000 anicli_ru-4.2.4/anicli_ru/anicli.py
+-rw-r--r--   0        0        0    12327 2020-02-02 00:00:00.000000 anicli_ru-4.2.4/anicli_ru/base.py
+-rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 anicli_ru-4.2.4/anicli_ru/defaults.py
+-rw-r--r--   0        0        0     6970 2020-02-02 00:00:00.000000 anicli_ru-4.2.4/anicli_ru/kodik.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 anicli_ru-4.2.4/anicli_ru/loader.py
+-rw-r--r--   0        0        0     6405 2020-02-02 00:00:00.000000 anicli_ru-4.2.4/anicli_ru/options.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anicli_ru-4.2.4/anicli_ru/extractors/__init__.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 anicli_ru-4.2.4/anicli_ru/extractors/__template__.py
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 anicli_ru-4.2.4/anicli_ru/extractors/anilibria.py
+-rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 anicli_ru-4.2.4/anicli_ru/extractors/animania.py
+-rw-r--r--   0        0        0     5598 2020-02-02 00:00:00.000000 anicli_ru-4.2.4/anicli_ru/extractors/animego.py
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 anicli_ru-4.2.4/anicli_ru/extractors/animevost.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 anicli_ru-4.2.4/anicli_ru/utils/__init__.py
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 anicli_ru-4.2.4/anicli_ru/utils/random_agent.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 anicli_ru-4.2.4/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 anicli_ru-4.2.4/LICENSE
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 anicli_ru-4.2.4/README.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 anicli_ru-4.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 anicli_ru-4.2.4/PKG-INFO
```

### Comparing `anicli-ru-4.2.3/LICENSE` & `anicli_ru-4.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `anicli-ru-4.2.3/PKG-INFO` & `anicli_ru-4.2.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,62 @@
 Metadata-Version: 2.1
 Name: anicli-ru
-Version: 4.2.3
+Version: 4.2.4
 Summary: anime grabber video api and cli tool
-Home-page: https://github.com/vypivshiy/ani-cli-ru
+Project-URL: Homepage, https://github.com/vypivshiy/ani-cli-ru
 Author: Georgiy aka Vypivshiy
-Author-email: 
-License: GPL-3
+License-Expression: GPL-3.0
+License-File: LICENSE
 Requires-Python: >=3.8
+Requires-Dist: requests
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # anicli-ru
 [![CI](https://github.com/vypivshiy/ani-cli-ru/actions/workflows/ci.yml/badge.svg)](https://github.com/vypivshiy/ani-cli-ru/actions/workflows/ci.yml)
 ___
 Скрипт для поиска и просмотра аниме из терминала с русской озвучкой или субтитрами для linux систем, 
 написанный на python.
 
 Парсит видео со сторонних сайтов, **как youtube-dl**.
 ___
-# Supported video hostings:
+## Supported video hostings:
 * sibnet
 * aniboom
 * kodik
 ---
-# Dependencies:
-* python 3.7+
+## Dependencies:
+* python 3.8+
+* requests
 * mpv
-* ffmpeg (опционально, для скачивания видео через аргумент "**-d**")
 ___
-# Install:
-```
-# Если у вас установлен скрипт версией ниже 4.0.0, то перед обновлением удалите старый файл запуска командой:
-sudo rm /usr/local/bin/anicli-ru
 
-# установка 
-python3 -m pip install anicli-ru
+## Install:
+### pipx (рекомендуется)
+`pipx install anicli-ru`
 
-# или клонировать и установить вручную:
 
-git clone https://github.com/vypivshiy/ani-cli-ru && cd ani-cli-ru
-pip install .
+### pip
+```shell
+pip install anicli-ru
 ```
+
 ___
-# Usage:
+## Usage:
 `anicli-ru`
 ___
-# CLI Commands:
+## CLI Commands:
 ```
 q [q]uit - выход из программы
 e [e]xit - alias q
 b [b]ack to the previous step - возвратиться на предыдущий шаг
 h [h]elp - вывод списка доступных команд
 c [c]lear - очистить консоль
 o [o]ngoing - напечатать недавно вышедшие онгоинги
 ```
-# FAQ
+## FAQ
 **Q**: У меня скрипт ничего не находит
 
 **A**: Возможно сайт с которого хотите достать видео включили cloudflare или не работает. 
 Используйте сторонние источники через аргумент `-s {число}`. 
 
 Все доступные источники для парсинга можно получить через команду 
 `anicli-ru --print-sources`
@@ -75,32 +73,33 @@
 # ~/.bashrc
 export PATH="$HOME/.local/bin:$PATH"
 # ~/.zshrc
 export PATH="$HOME/.local/bin:$PATH"
 ```
 
 ---
-# Program Api usage
-Если вам нужен программный интерфейс для своих проектов, то можете импортировать любой доступный 
-парсер из директории anicli_ru.extractors.* или вывести все доступные и импортировать через метод __import\__
+## Program Api usage
+### В стадии разработки
+Самый актуальный api интерфейс парсеров находится в [anicli-api](https://github.com/vypivshiy/anicli-api/tree/dev) 
+репозитории, в этом поддержки кода не будет:
+
+```shell
+pip install anicli-api
+```
+
+### Устаревший способ
+Вы можете использовать напрямую этот пакет
+Все реализованые парсеры лежат в модуле `anicli_ru.extractors.*`
+
 ```python
-# quick example
 from anicli_ru.extractors.animania import *
 from anicli_ru.loader import all_extractors
 
 print(all_extractors())  # вывод всех доступных парсеров из директории extractors
 a = Anime()
 ongoings = a.ongoing()  # получить онгоинги
 results = a.search("experiments lain")  # поиск тайтла по названию
 episodes = results[0].episodes()  # получить эпизоды с первого найденного тайтла
 players = episodes[0].player()  # получить сырые ссылки на видеохостниги (не прямую ссылку на видео)
 print(players[0].get_video())  # получить прямую ссылку на видео с видеохостинга для плеера
 ```
----
-# Contributing
-
-[DEV GUIDE](DEV.md)
-# TODO
-* ~~dev guide~~
-* ~~CI/CD github actions: add autotest utils (without test parser), pylance, etc~~
-* ~~mypy fix typing~~
```

### Comparing `anicli-ru-4.2.3/README.md` & `anicli_ru-4.2.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,51 +2,49 @@
 [![CI](https://github.com/vypivshiy/ani-cli-ru/actions/workflows/ci.yml/badge.svg)](https://github.com/vypivshiy/ani-cli-ru/actions/workflows/ci.yml)
 ___
 Скрипт для поиска и просмотра аниме из терминала с русской озвучкой или субтитрами для linux систем, 
 написанный на python.
 
 Парсит видео со сторонних сайтов, **как youtube-dl**.
 ___
-# Supported video hostings:
+## Supported video hostings:
 * sibnet
 * aniboom
 * kodik
 ---
-# Dependencies:
-* python 3.7+
+## Dependencies:
+* python 3.8+
+* requests
 * mpv
-* ffmpeg (опционально, для скачивания видео через аргумент "**-d**")
 ___
-# Install:
-```
-# Если у вас установлен скрипт версией ниже 4.0.0, то перед обновлением удалите старый файл запуска командой:
-sudo rm /usr/local/bin/anicli-ru
 
-# установка 
-python3 -m pip install anicli-ru
+## Install:
+### pipx (рекомендуется)
+`pipx install anicli-ru`
 
-# или клонировать и установить вручную:
 
-git clone https://github.com/vypivshiy/ani-cli-ru && cd ani-cli-ru
-pip install .
+### pip
+```shell
+pip install anicli-ru
 ```
+
 ___
-# Usage:
+## Usage:
 `anicli-ru`
 ___
-# CLI Commands:
+## CLI Commands:
 ```
 q [q]uit - выход из программы
 e [e]xit - alias q
 b [b]ack to the previous step - возвратиться на предыдущий шаг
 h [h]elp - вывод списка доступных команд
 c [c]lear - очистить консоль
 o [o]ngoing - напечатать недавно вышедшие онгоинги
 ```
-# FAQ
+## FAQ
 **Q**: У меня скрипт ничего не находит
 
 **A**: Возможно сайт с которого хотите достать видео включили cloudflare или не работает. 
 Используйте сторонние источники через аргумент `-s {число}`. 
 
 Все доступные источники для парсинга можно получить через команду 
 `anicli-ru --print-sources`
@@ -63,32 +61,33 @@
 # ~/.bashrc
 export PATH="$HOME/.local/bin:$PATH"
 # ~/.zshrc
 export PATH="$HOME/.local/bin:$PATH"
 ```
 
 ---
-# Program Api usage
-Если вам нужен программный интерфейс для своих проектов, то можете импортировать любой доступный 
-парсер из директории anicli_ru.extractors.* или вывести все доступные и импортировать через метод __import\__
+## Program Api usage
+### В стадии разработки
+Самый актуальный api интерфейс парсеров находится в [anicli-api](https://github.com/vypivshiy/anicli-api/tree/dev) 
+репозитории, в этом поддержки кода не будет:
+
+```shell
+pip install anicli-api
+```
+
+### Устаревший способ
+Вы можете использовать напрямую этот пакет
+Все реализованые парсеры лежат в модуле `anicli_ru.extractors.*`
+
 ```python
-# quick example
 from anicli_ru.extractors.animania import *
 from anicli_ru.loader import all_extractors
 
 print(all_extractors())  # вывод всех доступных парсеров из директории extractors
 a = Anime()
 ongoings = a.ongoing()  # получить онгоинги
 results = a.search("experiments lain")  # поиск тайтла по названию
 episodes = results[0].episodes()  # получить эпизоды с первого найденного тайтла
 players = episodes[0].player()  # получить сырые ссылки на видеохостниги (не прямую ссылку на видео)
 print(players[0].get_video())  # получить прямую ссылку на видео с видеохостинга для плеера
 ```
----
-# Contributing
-
-[DEV GUIDE](DEV.md)
-# TODO
-* ~~dev guide~~
-* ~~CI/CD github actions: add autotest utils (without test parser), pylance, etc~~
-* ~~mypy fix typing~~
```

### Comparing `anicli-ru-4.2.3/anicli_ru/_http.py` & `anicli_ru-4.2.4/anicli_ru/_http.py`

 * *Files identical despite different names*

### Comparing `anicli-ru-4.2.3/anicli_ru/aniboom.py` & `anicli_ru-4.2.4/anicli_ru/aniboom.py`

 * *Files identical despite different names*

### Comparing `anicli-ru-4.2.3/anicli_ru/anicli.py` & `anicli_ru-4.2.4/anicli_ru/anicli.py`

 * *Files identical despite different names*

### Comparing `anicli-ru-4.2.3/anicli_ru/base.py` & `anicli_ru-4.2.4/anicli_ru/base.py`

 * *Files identical despite different names*

### Comparing `anicli-ru-4.2.3/anicli_ru/defaults.py` & `anicli_ru-4.2.4/anicli_ru/defaults.py`

 * *Files identical despite different names*

### Comparing `anicli-ru-4.2.3/anicli_ru/extractors/__template__.py` & `anicli_ru-4.2.4/anicli_ru/extractors/__template__.py`

 * *Files identical despite different names*

### Comparing `anicli-ru-4.2.3/anicli_ru/extractors/anilibria.py` & `anicli_ru-4.2.4/anicli_ru/extractors/anilibria.py`

 * *Files identical despite different names*

### Comparing `anicli-ru-4.2.3/anicli_ru/extractors/animania.py` & `anicli_ru-4.2.4/anicli_ru/extractors/animania.py`

 * *Files identical despite different names*

### Comparing `anicli-ru-4.2.3/anicli_ru/extractors/animego.py` & `anicli_ru-4.2.4/anicli_ru/extractors/animego.py`

 * *Files identical despite different names*

### Comparing `anicli-ru-4.2.3/anicli_ru/extractors/animevost.py` & `anicli_ru-4.2.4/anicli_ru/extractors/animevost.py`

 * *Files identical despite different names*

### Comparing `anicli-ru-4.2.3/anicli_ru/kodik.py` & `anicli_ru-4.2.4/anicli_ru/kodik.py`

 * *Files identical despite different names*

### Comparing `anicli-ru-4.2.3/anicli_ru/loader.py` & `anicli_ru-4.2.4/anicli_ru/loader.py`

 * *Files identical despite different names*

### Comparing `anicli-ru-4.2.3/anicli_ru/options.py` & `anicli_ru-4.2.4/anicli_ru/options.py`

 * *Files identical despite different names*

### Comparing `anicli-ru-4.2.3/anicli_ru/utils/random_agent.py` & `anicli_ru-4.2.4/anicli_ru/utils/random_agent.py`

 * *Files identical despite different names*

