# Comparing `tmp/linkedin-messaging-0.5.6.tar.gz` & `tmp/linkedin_messaging-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkedin-messaging-0.5.6.tar", last modified: Tue Jun  6 04:34:28 2023, max compression
+gzip compressed data, was "linkedin_messaging-0.5.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `linkedin-messaging-0.5.6.tar` & `linkedin_messaging-0.5.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      386 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/.editorconfig
--rw-r--r--   0        0        0      782 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/.envrc
--rw-r--r--   0        0        0      205 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/.github/dependabot.yml
--rw-r--r--   0        0        0     2288 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/.github/workflows/python.yaml
--rw-r--r--   0        0        0     2287 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/.gitignore
--rw-r--r--   0        0        0     1133 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      240 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/.vim/coc-settings.json
--rw-r--r--   0        0        0     3742 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/CHANGELOG.md
--rw-r--r--   0        0        0    11358 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/LICENSE
--rw-r--r--   0        0        0      888 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/README.md
--rwxr-xr-x   0        0        0     1878 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/cicd/custom_style_check.py
--rw-r--r--   0        0        0     3832 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/dev-requirements.txt
--rw-r--r--   0        0        0     1284 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/examples/get-conversation.py
--rw-r--r--   0        0        0     1818 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/examples/listen-for-events.py
--rw-r--r--   0        0        0      870 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/examples/manual-login.py
--rw-r--r--   0        0        0      955 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/examples/mark-conversation-as-read.py
--rw-r--r--   0        0        0      823 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/examples/pickle-example.py
--rw-r--r--   0        0        0     1332 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/examples/redact-message.py
--rw-r--r--   0        0        0     1478 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/examples/send-message.py
--rw-r--r--   0        0        0     1730 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/examples/send-reaction.py
--rw-r--r--   0        0        0      542 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/examples/simple-2fa.py
--rw-r--r--   0        0        0      447 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/linkedin_messaging/__init__.py
--rw-r--r--   0        0        0    17222 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/linkedin_messaging/api_objects.py
--rw-r--r--   0        0        0       48 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/linkedin_messaging/exceptions.py
--rw-r--r--   0        0        0    20911 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/linkedin_messaging/linkedin.py
--rw-r--r--   0        0        0        0 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/linkedin_messaging/py.typed
--rw-r--r--   0        0        0     1803 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     1060 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/requirements.txt
--rw-r--r--   0        0        0      224 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/setup.cfg
--rw-r--r--   0        0        0      228 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/shell.nix
--rw-r--r--   0        0        0      321 2023-06-06 04:34:13.981949 linkedin-messaging-0.5.6/tests/test_urn.py
--rw-r--r--   0        0        0     2643 1970-01-01 00:00:00.000000 linkedin-messaging-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0      386 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/.editorconfig
+-rw-r--r--   0        0        0      782 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/.envrc
+-rw-r--r--   0        0        0      205 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/.github/dependabot.yml
+-rw-r--r--   0        0        0     2288 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/.github/workflows/python.yaml
+-rw-r--r--   0        0        0     2287 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/.gitignore
+-rw-r--r--   0        0        0     1133 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      240 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/.vim/coc-settings.json
+-rw-r--r--   0        0        0     3795 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/CHANGELOG.md
+-rw-r--r--   0        0        0    11358 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/LICENSE
+-rw-r--r--   0        0        0      888 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/README.md
+-rwxr-xr-x   0        0        0     1878 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/cicd/custom_style_check.py
+-rw-r--r--   0        0        0     3732 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/dev-requirements.txt
+-rw-r--r--   0        0        0     1284 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/examples/get-conversation.py
+-rw-r--r--   0        0        0     1818 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/examples/listen-for-events.py
+-rw-r--r--   0        0        0      870 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/examples/manual-login.py
+-rw-r--r--   0        0        0      955 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/examples/mark-conversation-as-read.py
+-rw-r--r--   0        0        0      823 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/examples/pickle-example.py
+-rw-r--r--   0        0        0     1332 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/examples/redact-message.py
+-rw-r--r--   0        0        0     1478 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/examples/send-message.py
+-rw-r--r--   0        0        0     1730 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/examples/send-reaction.py
+-rw-r--r--   0        0        0      542 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/examples/simple-2fa.py
+-rw-r--r--   0        0        0      447 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/linkedin_messaging/__init__.py
+-rw-r--r--   0        0        0    17268 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/linkedin_messaging/api_objects.py
+-rw-r--r--   0        0        0       48 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/linkedin_messaging/exceptions.py
+-rw-r--r--   0        0        0    20911 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/linkedin_messaging/linkedin.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/linkedin_messaging/py.typed
+-rw-r--r--   0        0        0     1803 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0      955 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/requirements.txt
+-rw-r--r--   0        0        0      224 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/setup.cfg
+-rw-r--r--   0        0        0      228 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/shell.nix
+-rw-r--r--   0        0        0      321 2023-07-18 06:10:39.438747 linkedin_messaging-0.5.7/tests/test_urn.py
+-rw-r--r--   0        0        0     2643 1970-01-01 00:00:00.000000 linkedin_messaging-0.5.7/PKG-INFO
```

### Comparing `linkedin-messaging-0.5.6/.envrc` & `linkedin_messaging-0.5.7/.envrc`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.6/.github/workflows/python.yaml` & `linkedin_messaging-0.5.7/.github/workflows/python.yaml`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.6/.gitignore` & `linkedin_messaging-0.5.7/.gitignore`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.6/.pre-commit-config.yaml` & `linkedin_messaging-0.5.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.6/CHANGELOG.md` & `linkedin_messaging-0.5.7/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# v0.5.7
+
+* Added objects to support message edits.
+
 # v0.5.6
 
 * Added objects to support voice messages.
 * Updated versions of many dependencies and all of the pre-commit hooks.
 
 # v0.5.5
```

### Comparing `linkedin-messaging-0.5.6/LICENSE` & `linkedin_messaging-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.6/README.md` & `linkedin_messaging-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.6/cicd/custom_style_check.py` & `linkedin_messaging-0.5.7/cicd/custom_style_check.py`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.6/dev-requirements.txt` & `linkedin_messaging-0.5.7/dev-requirements.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,110 +1,105 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --extra=dev --output-file=dev-requirements.txt --resolver=backtracking pyproject.toml
+#    pip-compile --extra=dev --output-file=dev-requirements.txt pyproject.toml
 #
 aiohttp==3.8.4
-    # via linkedin_messaging (pyproject.toml)
+    # via linkedin-messaging (pyproject.toml)
 aiosignal==1.3.1
     # via aiohttp
 async-timeout==4.0.2
     # via aiohttp
-attrs==22.2.0
+attrs==23.1.0
     # via
     #   aiohttp
     #   flake8-annotations
     #   flake8-bugbear
-    #   pytest
 beautifulsoup4==4.12.2
-    # via linkedin_messaging (pyproject.toml)
-black==23.3.0
-    # via linkedin_messaging (pyproject.toml)
+    # via linkedin-messaging (pyproject.toml)
+black==23.7.0
+    # via linkedin-messaging (pyproject.toml)
 build==0.10.0
     # via pip-tools
 certifi==2023.5.7
     # via requests
 cfgv==3.3.1
     # via pre-commit
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via
     #   aiohttp
     #   requests
-click==8.1.3
+click==8.1.5
     # via
     #   black
     #   pip-tools
-coverage[toml]==7.2.5
+coverage[toml]==7.2.7
     # via pytest-cov
-dataclasses-json==0.5.7
-    # via linkedin_messaging (pyproject.toml)
-distlib==0.3.6
+dataclasses-json==0.5.12
+    # via linkedin-messaging (pyproject.toml)
+distlib==0.3.7
     # via virtualenv
-docutils==0.19
+docutils==0.20.1
     # via flit
-exceptiongroup==1.1.1
+exceptiongroup==1.1.2
     # via pytest
-filelock==3.9.0
+filelock==3.12.2
     # via virtualenv
 flake8==6.0.0
     # via
     #   flake8-annotations
     #   flake8-bugbear
     #   flake8-comprehensions
     #   flake8-isort
     #   flake8-pep3101
     #   flake8-print
-    #   linkedin_messaging (pyproject.toml)
-flake8-annotations==3.0.0
-    # via linkedin_messaging (pyproject.toml)
-flake8-bugbear==23.3.12
-    # via linkedin_messaging (pyproject.toml)
-flake8-comprehensions==3.12.0
-    # via linkedin_messaging (pyproject.toml)
+    #   linkedin-messaging (pyproject.toml)
+flake8-annotations==3.0.1
+    # via linkedin-messaging (pyproject.toml)
+flake8-bugbear==23.7.10
+    # via linkedin-messaging (pyproject.toml)
+flake8-comprehensions==3.14.0
+    # via linkedin-messaging (pyproject.toml)
 flake8-isort==6.0.0
-    # via linkedin_messaging (pyproject.toml)
+    # via linkedin-messaging (pyproject.toml)
 flake8-pep3101==2.0.0
-    # via linkedin_messaging (pyproject.toml)
+    # via linkedin-messaging (pyproject.toml)
 flake8-print==5.0.0
-    # via linkedin_messaging (pyproject.toml)
-flit==3.8.0
-    # via linkedin_messaging (pyproject.toml)
-flit-core==3.8.0
+    # via linkedin-messaging (pyproject.toml)
+flit==3.9.0
+    # via linkedin-messaging (pyproject.toml)
+flit-core==3.9.0
     # via flit
-frozenlist==1.3.3
+frozenlist==1.4.0
     # via
     #   aiohttp
     #   aiosignal
 identify==2.5.24
     # via pre-commit
 idna==3.4
     # via
     #   requests
     #   yarl
 iniconfig==2.0.0
     # via pytest
 isort==5.12.0
     # via
     #   flake8-isort
-    #   linkedin_messaging (pyproject.toml)
+    #   linkedin-messaging (pyproject.toml)
 marshmallow==3.19.0
-    # via
-    #   dataclasses-json
-    #   marshmallow-enum
-marshmallow-enum==1.5.1
     # via dataclasses-json
 mccabe==0.7.0
     # via flake8
 multidict==6.0.4
     # via
     #   aiohttp
     #   yarl
-mypy==1.3.0
-    # via linkedin_messaging (pyproject.toml)
+mypy==1.4.1
+    # via linkedin-messaging (pyproject.toml)
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
     #   typing-inspect
 nodeenv==1.8.0
     # via pre-commit
@@ -112,70 +107,71 @@
     # via
     #   black
     #   build
     #   marshmallow
     #   pytest
 pathspec==0.11.1
     # via black
-pip-tools==6.13.0
-    # via linkedin_messaging (pyproject.toml)
-platformdirs==3.1.1
+pip-tools==7.0.0
+    # via linkedin-messaging (pyproject.toml)
+platformdirs==3.9.1
     # via
     #   black
     #   virtualenv
-pluggy==1.0.0
+pluggy==1.2.0
     # via pytest
-pre-commit==3.3.2
-    # via linkedin_messaging (pyproject.toml)
+pre-commit==3.3.3
+    # via linkedin-messaging (pyproject.toml)
 pycodestyle==2.10.0
     # via
     #   flake8
     #   flake8-print
 pyflakes==3.0.1
     # via flake8
 pyproject-hooks==1.0.0
     # via build
-pytest==7.2.2
+pytest==7.4.0
     # via
-    #   linkedin_messaging (pyproject.toml)
+    #   linkedin-messaging (pyproject.toml)
     #   pytest-cov
-pytest-cov==4.0.0
-    # via linkedin_messaging (pyproject.toml)
-pyyaml==6.0
+pytest-cov==4.1.0
+    # via linkedin-messaging (pyproject.toml)
+pyyaml==6.0.1
     # via pre-commit
-requests==2.28.2
+requests==2.31.0
     # via flit
-soupsieve==2.4
+soupsieve==2.4.1
     # via beautifulsoup4
-termcolor==2.2.0
-    # via linkedin_messaging (pyproject.toml)
+termcolor==2.3.0
+    # via linkedin-messaging (pyproject.toml)
 tomli==2.0.1
     # via
     #   black
     #   build
     #   coverage
     #   mypy
+    #   pip-tools
     #   pyproject-hooks
     #   pytest
 tomli-w==1.0.0
     # via flit
 types-termcolor==1.1.6.2
-    # via linkedin_messaging (pyproject.toml)
-typing-extensions==4.5.0
+    # via linkedin-messaging (pyproject.toml)
+typing-extensions==4.7.1
     # via
     #   black
     #   mypy
     #   typing-inspect
 typing-inspect==0.9.0
     # via dataclasses-json
-urllib3==1.26.15
+urllib3==2.0.3
     # via requests
-virtualenv==20.21.0
+virtualenv==20.24.0
     # via pre-commit
 wheel==0.40.0
     # via pip-tools
-yarl==1.8.2
+yarl==1.9.2
     # via aiohttp
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `linkedin-messaging-0.5.6/examples/get-conversation.py` & `linkedin_messaging-0.5.7/examples/get-conversation.py`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.6/examples/listen-for-events.py` & `linkedin_messaging-0.5.7/examples/listen-for-events.py`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.6/examples/manual-login.py` & `linkedin_messaging-0.5.7/examples/manual-login.py`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.6/examples/mark-conversation-as-read.py` & `linkedin_messaging-0.5.7/examples/mark-conversation-as-read.py`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.6/examples/pickle-example.py` & `linkedin_messaging-0.5.7/examples/pickle-example.py`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.6/examples/redact-message.py` & `linkedin_messaging-0.5.7/examples/redact-message.py`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.6/examples/send-message.py` & `linkedin_messaging-0.5.7/examples/send-message.py`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.6/examples/send-reaction.py` & `linkedin_messaging-0.5.7/examples/send-reaction.py`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.6/examples/simple-2fa.py` & `linkedin_messaging-0.5.7/examples/simple-2fa.py`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.6/linkedin_messaging/api_objects.py` & `linkedin_messaging-0.5.7/linkedin_messaging/api_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,14 +401,15 @@
 @dataclass
 class MessageEvent:
     body: str = ""
     feed_update: Optional[FeedUpdate] = None
     message_body_render_format: str = ""
     subject: Optional[str] = None
     recalled_at: Optional[datetime] = None
+    last_edited_at: Optional[datetime] = None
     attributed_body: Optional[AttributedBody] = None
     attachments: list[MessageAttachment] = field(default_factory=list)
     media_attachments: list[MediaAttachment] = field(default_factory=list)
     custom_content: Optional[MessageCustomContent] = None
 
 
 @dataclass_json(letter_case=LetterCase.CAMEL, undefined=Undefined.EXCLUDE)
```

### Comparing `linkedin-messaging-0.5.6/linkedin_messaging/linkedin.py` & `linkedin_messaging-0.5.7/linkedin_messaging/linkedin.py`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.6/pyproject.toml` & `linkedin_messaging-0.5.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `linkedin-messaging-0.5.6/requirements.txt` & `linkedin_messaging-0.5.7/requirements.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,44 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements.txt --resolver=backtracking pyproject.toml
+#    pip-compile --output-file=requirements.txt pyproject.toml
 #
 aiohttp==3.8.4
-    # via linkedin_messaging (pyproject.toml)
+    # via linkedin-messaging (pyproject.toml)
 aiosignal==1.3.1
     # via aiohttp
 async-timeout==4.0.2
     # via aiohttp
-attrs==22.2.0
+attrs==23.1.0
     # via aiohttp
 beautifulsoup4==4.12.2
-    # via linkedin_messaging (pyproject.toml)
-charset-normalizer==3.1.0
+    # via linkedin-messaging (pyproject.toml)
+charset-normalizer==3.2.0
     # via aiohttp
-dataclasses-json==0.5.7
-    # via linkedin_messaging (pyproject.toml)
-frozenlist==1.3.3
+dataclasses-json==0.5.12
+    # via linkedin-messaging (pyproject.toml)
+frozenlist==1.4.0
     # via
     #   aiohttp
     #   aiosignal
 idna==3.4
     # via yarl
 marshmallow==3.19.0
-    # via
-    #   dataclasses-json
-    #   marshmallow-enum
-marshmallow-enum==1.5.1
     # via dataclasses-json
 multidict==6.0.4
     # via
     #   aiohttp
     #   yarl
 mypy-extensions==1.0.0
     # via typing-inspect
 packaging==23.1
     # via marshmallow
-soupsieve==2.4
+soupsieve==2.4.1
     # via beautifulsoup4
-typing-extensions==4.5.0
+typing-extensions==4.7.1
     # via typing-inspect
 typing-inspect==0.9.0
     # via dataclasses-json
-yarl==1.8.2
+yarl==1.9.2
     # via aiohttp
```

### Comparing `linkedin-messaging-0.5.6/PKG-INFO` & `linkedin_messaging-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkedin-messaging
-Version: 0.5.6
+Version: 0.5.7
 Summary: An unofficial API for interacting with LinkedIn Messaging
 Keywords: LinkedIn,messaging
 Author-email: Sumner Evans <sumner@beeper.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO
```

