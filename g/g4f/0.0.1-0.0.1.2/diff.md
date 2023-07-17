# Comparing `tmp/g4f-0.0.1.tar.gz` & `tmp/g4f-0.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g4f-0.0.1.tar", last modified: Mon Jul 17 00:10:14 2023, max compression
+gzip compressed data, was "g4f-0.0.1.2.tar", last modified: Mon Jul 17 23:14:52 2023, max compression
```

## Comparing `g4f-0.0.1.tar` & `g4f-0.0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-07-17 00:10:14.309190 g4f-0.0.1/
--rw-r--r--   0 tek        (501) staff       (20)    35149 2023-04-16 23:05:26.000000 g4f-0.0.1/LICENSE
--rw-r--r--   0 tek        (501) staff       (20)    18050 2023-07-17 00:10:14.308871 g4f-0.0.1/PKG-INFO
--rw-r--r--   0 tek        (501) staff       (20)    17304 2023-07-16 18:26:15.000000 g4f-0.0.1/README.md
-drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-07-17 00:10:14.306551 g4f-0.0.1/g4f/
-drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-07-17 00:10:14.308328 g4f-0.0.1/g4f/Provider/
--rw-r--r--   0 tek        (501) staff       (20)      501 2023-07-16 19:31:22.000000 g4f-0.0.1/g4f/Provider/Provider.py
--rw-r--r--   0 tek        (501) staff       (20)      353 2023-07-16 18:49:10.000000 g4f-0.0.1/g4f/Provider/__init__.py
--rw-r--r--   0 tek        (501) staff       (20)     1691 2023-07-16 19:31:26.000000 g4f-0.0.1/g4f/__init__.py
--rw-r--r--   0 tek        (501) staff       (20)     7561 2023-07-16 18:58:49.000000 g4f-0.0.1/g4f/models.py
--rw-r--r--   0 tek        (501) staff       (20)      110 2023-07-16 17:53:33.000000 g4f-0.0.1/g4f/typing.py
--rw-r--r--   0 tek        (501) staff       (20)     1700 2023-07-16 17:53:33.000000 g4f-0.0.1/g4f/utils.py
-drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-07-17 00:10:14.307815 g4f-0.0.1/g4f.egg-info/
--rw-r--r--   0 tek        (501) staff       (20)    18050 2023-07-17 00:10:14.000000 g4f-0.0.1/g4f.egg-info/PKG-INFO
--rw-r--r--   0 tek        (501) staff       (20)      267 2023-07-17 00:10:14.000000 g4f-0.0.1/g4f.egg-info/SOURCES.txt
--rw-r--r--   0 tek        (501) staff       (20)        1 2023-07-17 00:10:14.000000 g4f-0.0.1/g4f.egg-info/dependency_links.txt
--rw-r--r--   0 tek        (501) staff       (20)       91 2023-07-17 00:10:14.000000 g4f-0.0.1/g4f.egg-info/requires.txt
--rw-r--r--   0 tek        (501) staff       (20)        4 2023-07-17 00:10:14.000000 g4f-0.0.1/g4f.egg-info/top_level.txt
--rw-r--r--   0 tek        (501) staff       (20)       38 2023-07-17 00:10:14.309277 g4f-0.0.1/setup.cfg
--rw-r--r--   0 tek        (501) staff       (20)     1316 2023-07-17 00:09:44.000000 g4f-0.0.1/setup.py
+drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-07-17 23:14:52.556352 g4f-0.0.1.2/
+-rw-r--r--   0 tek        (501) staff       (20)    35149 2023-04-16 23:05:26.000000 g4f-0.0.1.2/LICENSE
+-rw-r--r--   0 tek        (501) staff       (20)    19162 2023-07-17 23:14:52.556091 g4f-0.0.1.2/PKG-INFO
+-rw-r--r--   0 tek        (501) staff       (20)    18414 2023-07-17 00:16:47.000000 g4f-0.0.1.2/README.md
+drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-07-17 23:14:52.553658 g4f-0.0.1.2/g4f/
+drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-07-17 23:14:52.555562 g4f-0.0.1.2/g4f/Provider/
+-rw-r--r--   0 tek        (501) staff       (20)      501 2023-07-16 19:31:22.000000 g4f-0.0.1.2/g4f/Provider/Provider.py
+-rw-r--r--   0 tek        (501) staff       (20)      353 2023-07-16 18:49:10.000000 g4f-0.0.1.2/g4f/Provider/__init__.py
+-rw-r--r--   0 tek        (501) staff       (20)     1691 2023-07-16 19:31:26.000000 g4f-0.0.1.2/g4f/__init__.py
+-rw-r--r--   0 tek        (501) staff       (20)     7561 2023-07-16 18:58:49.000000 g4f-0.0.1.2/g4f/models.py
+-rw-r--r--   0 tek        (501) staff       (20)      110 2023-07-16 17:53:33.000000 g4f-0.0.1.2/g4f/typing.py
+-rw-r--r--   0 tek        (501) staff       (20)     1700 2023-07-16 17:53:33.000000 g4f-0.0.1.2/g4f/utils.py
+drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-07-17 23:14:52.554899 g4f-0.0.1.2/g4f.egg-info/
+-rw-r--r--   0 tek        (501) staff       (20)    19162 2023-07-17 23:14:52.000000 g4f-0.0.1.2/g4f.egg-info/PKG-INFO
+-rw-r--r--   0 tek        (501) staff       (20)      267 2023-07-17 23:14:52.000000 g4f-0.0.1.2/g4f.egg-info/SOURCES.txt
+-rw-r--r--   0 tek        (501) staff       (20)        1 2023-07-17 23:14:52.000000 g4f-0.0.1.2/g4f.egg-info/dependency_links.txt
+-rw-r--r--   0 tek        (501) staff       (20)       93 2023-07-17 23:14:52.000000 g4f-0.0.1.2/g4f.egg-info/requires.txt
+-rw-r--r--   0 tek        (501) staff       (20)        4 2023-07-17 23:14:52.000000 g4f-0.0.1.2/g4f.egg-info/top_level.txt
+-rw-r--r--   0 tek        (501) staff       (20)       38 2023-07-17 23:14:52.556500 g4f-0.0.1.2/setup.cfg
+-rw-r--r--   0 tek        (501) staff       (20)     1318 2023-07-17 23:09:23.000000 g4f-0.0.1.2/setup.py
```

### Comparing `g4f-0.0.1/LICENSE` & `g4f-0.0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `g4f-0.0.1/PKG-INFO` & `g4f-0.0.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.0.1
+Version: 0.0.1.2
 Summary: The official gpt4free repository | various collection of powerful language models
 Author: Tekky
 Author-email: <support@g4f.ai>
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,20 @@
 ![image](https://github.com/onlpx/gpt4free-v2/assets/98614666/7886223b-c1d1-4260-82aa-da5741f303bb)
 
 By using this repository or any code related to it, you agree to the [legal notice](./LEGAL_NOTICE.md). The author is not responsible for any copies, forks, or reuploads made by other users. This is the author's only account and repository. To prevent impersonation or irresponsible actions, you may comply with the GNU GPL license this Repository uses.
 
 This (quite censored) New Version of gpt4free, was just released, it may contain bugs, open an issue or contribute a PR when encountering one, some features were disabled.
 Docker is for now not available but I would be happy if someone contributes a PR. The g4f GUI will be uploaded soon enough.
 
+### New
+- pypi package:
+```
+pip install g4f
+```
+
 ## Table of Contents:
 
 - [Getting Started](#getting-started)
     + [Prerequisites](#prerequisites)
     + [Setting up the project](#setting-up-the-project)
 - [Usage](#usage)
   * [The `g4f` Package](#the-g4f-package)
@@ -42,14 +48,21 @@
 
 ## Getting Started
 
 #### Prerequisites:
 1. [Download and install Python](https://www.python.org/downloads/) (Version 3.x is recommended).
 
 #### Setting up the project:
+##### Install using pypi
+```
+pip install g4f
+```
+
+##### or
+
 1. Clone the GitHub repository: 
 ```
 git clone https://github.com/xtekky/gpt4free.git
 ```
 2. Navigate to the project directory:
 ```
 cd gpt4free
@@ -163,31 +176,37 @@
 
 ## Models
 
 ### gpt-3.5 / gpt-4
 
 | Website| Provider| gpt-3.5 | gpt-4 | Streaming | Status | Auth |
 | --- | --- | --- | --- | --- | --- | --- |
-| [bing.com](https://bing.com/chat) | `g4f.Provider.Bing` | ✔️ | ✔️ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [super.lockchat.app](http://super.lockchat.app) | `g4f.Provider.Lockchat` | ✔️ | ✔️ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [liaobots.com](https://liaobots.com) | `g4f.Provider.Liaobots` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ✔️ |
-| [ai.ls](https://ai.ls) | `g4f.Provider.Ails` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [you.com](https://you.com) | `g4f.Provider.You` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [chat9.yqcloud.top](https://chat9.yqcloud.top/) | `g4f.Provider.Yqcloud` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [theb.ai](https://theb.ai) | `g4f.Provider.Theb` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [play.vercel.ai](https://play.vercel.ai) | `g4f.Provider.Vercel` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [forefront.com](https://forefront.com) | `g4f.Provider.Forefront` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [deepai.org](https://deepai.org) | `g4f.Provider.DeepAi` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [chat.getgpt.world](https://chat.getgpt.world/) | `g4f.Provider.GetGpt` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |   
-| [chatgptlogin.ac](https://chatgptlogin.ac) | `g4f.Provider.ChatgptLogin` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [chat-gpt.org](https://chat-gpt.org/chat) | `g4f.Provider.Aichat` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [chat.acytoo.com](https://chat.acytoo.com) | `g4f.Provider.Acytoo` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [aitianhu.com](https://aitianhu.com) | `g4f.Provider.AItianhu` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [chat.dfehub.com](https://chat.dfehub.com) | `g4f.Provider.DFEHub` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [free.easychat.work](https://free.easychat.work) | `g4f.Provider.EasyChat` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [ai.ls](https://ai.ls) | `g4f.ProviderAils` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [you.com](https://you.com) | `g4f.ProviderYou` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [bing.com](https://bing.com/chat) | `g4f.ProviderBing` | ❌ | ✔️ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [chat9.yqcloud.top](https://chat9.yqcloud.top/) | `g4f.ProviderYqcloud` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [theb.ai](https://theb.ai) | `g4f.ProviderTheb` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [chat-gpt.org](https://chat-gpt.org/chat) | `g4f.ProviderAichat` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [bard.google.com](https://bard.google.com) | `g4f.ProviderBard` | ❌ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ✔️ |
+| [play.vercel.ai](https://play.vercel.ai) | `g4f.ProviderVercel` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [forefront.com](https://forefront.com) | `g4f.ProviderForefront` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [supertest.lockchat.app](http://supertest.lockchat.app) | `g4f.ProviderLockchat` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [liaobots.com](https://liaobots.com) | `g4f.ProviderLiaobots` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ✔️ |
+| [gpt-gm.h2o.ai](https://gpt-gm.h2o.ai) | `g4f.ProviderH2o` | ❌ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [chatgptlogin.ac](https://chatgptlogin.ac) | `g4f.ProviderChatgptLogin` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [deepai.org](https://deepai.org) | `g4f.ProviderDeepAi` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [chat.getgpt.world](https://chat.getgpt.world/) | `g4f.ProviderGetGpt` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [www.aitianhu.com](https://www.aitianhu.com/api/chat-process) | `g4f.ProviderAItianhu` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [free.easychat.work](https://free.easychat.work) | `g4f.ProviderEasyChat` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [chat.acytoo.com](https://chat.acytoo.com/api/completions) | `g4f.ProviderAcytoo` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [chat.dfehub.com](https://chat.dfehub.com/api/chat) | `g4f.ProviderDfeHub` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [aiservice.vercel.app](https://aiservice.vercel.app/api/chat/answer) | `g4f.ProviderAiService` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [b.ai-huan.xyz](https://b.ai-huan.xyz) | `g4f.ProviderBingHuan` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [wewordle.org](https://wewordle.org/gptapi/v1/android/turbo) | `g4f.ProviderWewordle` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [chatgpt.ai](https://chatgpt.ai/gpt-4/) | `g4f.ProviderChatgptAi` | ❌ | ✔️ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 
 
 ### Other Models
 
 | Model| Base Provider | Provider | Website |
 | ------- | ----------- | ---- |---- |
 | palm2 | Google | `g4f.Provider.Bard` | [bard.google.com](https://bard.google.com/) |
```

### Comparing `g4f-0.0.1/README.md` & `g4f-0.0.1.2/g4f.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,37 @@
+Metadata-Version: 2.1
+Name: g4f
+Version: 0.0.1.2
+Summary: The official gpt4free repository | various collection of powerful language models
+Author: Tekky
+Author-email: <support@g4f.ai>
+Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
 ![image](https://github.com/onlpx/gpt4free-v2/assets/98614666/7886223b-c1d1-4260-82aa-da5741f303bb)
 
 By using this repository or any code related to it, you agree to the [legal notice](./LEGAL_NOTICE.md). The author is not responsible for any copies, forks, or reuploads made by other users. This is the author's only account and repository. To prevent impersonation or irresponsible actions, you may comply with the GNU GPL license this Repository uses.
 
 This (quite censored) New Version of gpt4free, was just released, it may contain bugs, open an issue or contribute a PR when encountering one, some features were disabled.
 Docker is for now not available but I would be happy if someone contributes a PR. The g4f GUI will be uploaded soon enough.
 
+### New
+- pypi package:
+```
+pip install g4f
+```
+
 ## Table of Contents:
 
 - [Getting Started](#getting-started)
     + [Prerequisites](#prerequisites)
     + [Setting up the project](#setting-up-the-project)
 - [Usage](#usage)
   * [The `g4f` Package](#the-g4f-package)
@@ -25,14 +48,21 @@
 
 ## Getting Started
 
 #### Prerequisites:
 1. [Download and install Python](https://www.python.org/downloads/) (Version 3.x is recommended).
 
 #### Setting up the project:
+##### Install using pypi
+```
+pip install g4f
+```
+
+##### or
+
 1. Clone the GitHub repository: 
 ```
 git clone https://github.com/xtekky/gpt4free.git
 ```
 2. Navigate to the project directory:
 ```
 cd gpt4free
@@ -146,31 +176,37 @@
 
 ## Models
 
 ### gpt-3.5 / gpt-4
 
 | Website| Provider| gpt-3.5 | gpt-4 | Streaming | Status | Auth |
 | --- | --- | --- | --- | --- | --- | --- |
-| [bing.com](https://bing.com/chat) | `g4f.Provider.Bing` | ✔️ | ✔️ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [super.lockchat.app](http://super.lockchat.app) | `g4f.Provider.Lockchat` | ✔️ | ✔️ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [liaobots.com](https://liaobots.com) | `g4f.Provider.Liaobots` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ✔️ |
-| [ai.ls](https://ai.ls) | `g4f.Provider.Ails` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [you.com](https://you.com) | `g4f.Provider.You` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [chat9.yqcloud.top](https://chat9.yqcloud.top/) | `g4f.Provider.Yqcloud` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [theb.ai](https://theb.ai) | `g4f.Provider.Theb` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [play.vercel.ai](https://play.vercel.ai) | `g4f.Provider.Vercel` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [forefront.com](https://forefront.com) | `g4f.Provider.Forefront` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [deepai.org](https://deepai.org) | `g4f.Provider.DeepAi` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [chat.getgpt.world](https://chat.getgpt.world/) | `g4f.Provider.GetGpt` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |   
-| [chatgptlogin.ac](https://chatgptlogin.ac) | `g4f.Provider.ChatgptLogin` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [chat-gpt.org](https://chat-gpt.org/chat) | `g4f.Provider.Aichat` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [chat.acytoo.com](https://chat.acytoo.com) | `g4f.Provider.Acytoo` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [aitianhu.com](https://aitianhu.com) | `g4f.Provider.AItianhu` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [chat.dfehub.com](https://chat.dfehub.com) | `g4f.Provider.DFEHub` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [free.easychat.work](https://free.easychat.work) | `g4f.Provider.EasyChat` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [ai.ls](https://ai.ls) | `g4f.ProviderAils` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [you.com](https://you.com) | `g4f.ProviderYou` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [bing.com](https://bing.com/chat) | `g4f.ProviderBing` | ❌ | ✔️ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [chat9.yqcloud.top](https://chat9.yqcloud.top/) | `g4f.ProviderYqcloud` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [theb.ai](https://theb.ai) | `g4f.ProviderTheb` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [chat-gpt.org](https://chat-gpt.org/chat) | `g4f.ProviderAichat` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [bard.google.com](https://bard.google.com) | `g4f.ProviderBard` | ❌ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ✔️ |
+| [play.vercel.ai](https://play.vercel.ai) | `g4f.ProviderVercel` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [forefront.com](https://forefront.com) | `g4f.ProviderForefront` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [supertest.lockchat.app](http://supertest.lockchat.app) | `g4f.ProviderLockchat` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [liaobots.com](https://liaobots.com) | `g4f.ProviderLiaobots` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ✔️ |
+| [gpt-gm.h2o.ai](https://gpt-gm.h2o.ai) | `g4f.ProviderH2o` | ❌ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [chatgptlogin.ac](https://chatgptlogin.ac) | `g4f.ProviderChatgptLogin` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [deepai.org](https://deepai.org) | `g4f.ProviderDeepAi` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [chat.getgpt.world](https://chat.getgpt.world/) | `g4f.ProviderGetGpt` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [www.aitianhu.com](https://www.aitianhu.com/api/chat-process) | `g4f.ProviderAItianhu` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [free.easychat.work](https://free.easychat.work) | `g4f.ProviderEasyChat` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [chat.acytoo.com](https://chat.acytoo.com/api/completions) | `g4f.ProviderAcytoo` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [chat.dfehub.com](https://chat.dfehub.com/api/chat) | `g4f.ProviderDfeHub` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [aiservice.vercel.app](https://aiservice.vercel.app/api/chat/answer) | `g4f.ProviderAiService` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [b.ai-huan.xyz](https://b.ai-huan.xyz) | `g4f.ProviderBingHuan` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [wewordle.org](https://wewordle.org/gptapi/v1/android/turbo) | `g4f.ProviderWewordle` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [chatgpt.ai](https://chatgpt.ai/gpt-4/) | `g4f.ProviderChatgptAi` | ❌ | ✔️ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 
 
 ### Other Models
 
 | Model| Base Provider | Provider | Website |
 | ------- | ----------- | ---- |---- |
 | palm2 | Google | `g4f.Provider.Bard` | [bard.google.com](https://bard.google.com/) |
```

### Comparing `g4f-0.0.1/g4f/__init__.py` & `g4f-0.0.1.2/g4f/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.0.1/g4f/models.py` & `g4f-0.0.1.2/g4f/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.0.1/g4f/utils.py` & `g4f-0.0.1.2/g4f/utils.py`

 * *Files identical despite different names*

### Comparing `g4f-0.0.1/g4f.egg-info/PKG-INFO` & `g4f-0.0.1.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,20 @@
-Metadata-Version: 2.1
-Name: g4f
-Version: 0.0.1
-Summary: The official gpt4free repository | various collection of powerful language models
-Author: Tekky
-Author-email: <support@g4f.ai>
-Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
 ![image](https://github.com/onlpx/gpt4free-v2/assets/98614666/7886223b-c1d1-4260-82aa-da5741f303bb)
 
 By using this repository or any code related to it, you agree to the [legal notice](./LEGAL_NOTICE.md). The author is not responsible for any copies, forks, or reuploads made by other users. This is the author's only account and repository. To prevent impersonation or irresponsible actions, you may comply with the GNU GPL license this Repository uses.
 
 This (quite censored) New Version of gpt4free, was just released, it may contain bugs, open an issue or contribute a PR when encountering one, some features were disabled.
 Docker is for now not available but I would be happy if someone contributes a PR. The g4f GUI will be uploaded soon enough.
 
+### New
+- pypi package:
+```
+pip install g4f
+```
+
 ## Table of Contents:
 
 - [Getting Started](#getting-started)
     + [Prerequisites](#prerequisites)
     + [Setting up the project](#setting-up-the-project)
 - [Usage](#usage)
   * [The `g4f` Package](#the-g4f-package)
@@ -42,14 +31,21 @@
 
 ## Getting Started
 
 #### Prerequisites:
 1. [Download and install Python](https://www.python.org/downloads/) (Version 3.x is recommended).
 
 #### Setting up the project:
+##### Install using pypi
+```
+pip install g4f
+```
+
+##### or
+
 1. Clone the GitHub repository: 
 ```
 git clone https://github.com/xtekky/gpt4free.git
 ```
 2. Navigate to the project directory:
 ```
 cd gpt4free
@@ -163,31 +159,37 @@
 
 ## Models
 
 ### gpt-3.5 / gpt-4
 
 | Website| Provider| gpt-3.5 | gpt-4 | Streaming | Status | Auth |
 | --- | --- | --- | --- | --- | --- | --- |
-| [bing.com](https://bing.com/chat) | `g4f.Provider.Bing` | ✔️ | ✔️ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [super.lockchat.app](http://super.lockchat.app) | `g4f.Provider.Lockchat` | ✔️ | ✔️ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [liaobots.com](https://liaobots.com) | `g4f.Provider.Liaobots` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ✔️ |
-| [ai.ls](https://ai.ls) | `g4f.Provider.Ails` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [you.com](https://you.com) | `g4f.Provider.You` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [chat9.yqcloud.top](https://chat9.yqcloud.top/) | `g4f.Provider.Yqcloud` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [theb.ai](https://theb.ai) | `g4f.Provider.Theb` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [play.vercel.ai](https://play.vercel.ai) | `g4f.Provider.Vercel` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [forefront.com](https://forefront.com) | `g4f.Provider.Forefront` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [deepai.org](https://deepai.org) | `g4f.Provider.DeepAi` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [chat.getgpt.world](https://chat.getgpt.world/) | `g4f.Provider.GetGpt` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |   
-| [chatgptlogin.ac](https://chatgptlogin.ac) | `g4f.Provider.ChatgptLogin` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [chat-gpt.org](https://chat-gpt.org/chat) | `g4f.Provider.Aichat` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [chat.acytoo.com](https://chat.acytoo.com) | `g4f.Provider.Acytoo` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [aitianhu.com](https://aitianhu.com) | `g4f.Provider.AItianhu` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [chat.dfehub.com](https://chat.dfehub.com) | `g4f.Provider.DFEHub` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [free.easychat.work](https://free.easychat.work) | `g4f.Provider.EasyChat` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [ai.ls](https://ai.ls) | `g4f.ProviderAils` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [you.com](https://you.com) | `g4f.ProviderYou` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [bing.com](https://bing.com/chat) | `g4f.ProviderBing` | ❌ | ✔️ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [chat9.yqcloud.top](https://chat9.yqcloud.top/) | `g4f.ProviderYqcloud` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [theb.ai](https://theb.ai) | `g4f.ProviderTheb` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [chat-gpt.org](https://chat-gpt.org/chat) | `g4f.ProviderAichat` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [bard.google.com](https://bard.google.com) | `g4f.ProviderBard` | ❌ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ✔️ |
+| [play.vercel.ai](https://play.vercel.ai) | `g4f.ProviderVercel` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [forefront.com](https://forefront.com) | `g4f.ProviderForefront` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [supertest.lockchat.app](http://supertest.lockchat.app) | `g4f.ProviderLockchat` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [liaobots.com](https://liaobots.com) | `g4f.ProviderLiaobots` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ✔️ |
+| [gpt-gm.h2o.ai](https://gpt-gm.h2o.ai) | `g4f.ProviderH2o` | ❌ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [chatgptlogin.ac](https://chatgptlogin.ac) | `g4f.ProviderChatgptLogin` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [deepai.org](https://deepai.org) | `g4f.ProviderDeepAi` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [chat.getgpt.world](https://chat.getgpt.world/) | `g4f.ProviderGetGpt` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [www.aitianhu.com](https://www.aitianhu.com/api/chat-process) | `g4f.ProviderAItianhu` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [free.easychat.work](https://free.easychat.work) | `g4f.ProviderEasyChat` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [chat.acytoo.com](https://chat.acytoo.com/api/completions) | `g4f.ProviderAcytoo` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [chat.dfehub.com](https://chat.dfehub.com/api/chat) | `g4f.ProviderDfeHub` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [aiservice.vercel.app](https://aiservice.vercel.app/api/chat/answer) | `g4f.ProviderAiService` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [b.ai-huan.xyz](https://b.ai-huan.xyz) | `g4f.ProviderBingHuan` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [wewordle.org](https://wewordle.org/gptapi/v1/android/turbo) | `g4f.ProviderWewordle` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [chatgpt.ai](https://chatgpt.ai/gpt-4/) | `g4f.ProviderChatgptAi` | ❌ | ✔️ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 
 
 ### Other Models
 
 | Model| Base Provider | Provider | Website |
 | ------- | ----------- | ---- |---- |
 | palm2 | Google | `g4f.Provider.Bard` | [bard.google.com](https://bard.google.com/) |
```

### Comparing `g4f-0.0.1/setup.py` & `g4f-0.0.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
     
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
-VERSION = '0.0.1'
+VERSION = '0.0.1.2'
 DESCRIPTION = 'The official gpt4free repository | various collection of powerful language models'
 
 # Setting up
 setup(
     name="g4f",
     version=VERSION,
     author="Tekky",
```

