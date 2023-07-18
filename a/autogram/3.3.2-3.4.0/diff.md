# Comparing `tmp/autogram-3.3.2.tar.gz` & `tmp/autogram-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogram-3.3.2.tar", last modified: Sat Apr  1 08:25:45 2023, max compression
+gzip compressed data, was "autogram-3.4.0.tar", last modified: Tue Jul 18 17:29:31 2023, max compression
```

## Comparing `autogram-3.3.2.tar` & `autogram-3.4.0.tar`

### file list

```diff
@@ -1,34 +1,21 @@
-drwxrwxr-x   0 sp3rtah   (1000) sp3rtah   (1000)        0 2023-04-01 08:25:45.737945 autogram-3.3.2/
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)     1064 2022-09-18 05:17:08.000000 autogram-3.3.2/LICENSE
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)     7482 2023-04-01 08:25:45.737945 autogram-3.3.2/PKG-INFO
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)     5757 2023-03-18 08:59:11.000000 autogram-3.3.2/README.md
-drwxrwxr-x   0 sp3rtah   (1000) sp3rtah   (1000)        0 2023-04-01 08:25:45.721946 autogram-3.3.2/autogram/
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)      424 2023-01-15 21:37:29.000000 autogram-3.3.2/autogram/__init__.py
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)     1495 2023-04-01 08:19:55.000000 autogram-3.3.2/autogram/config.py
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)    25335 2023-04-01 08:22:58.000000 autogram-3.3.2/autogram/main.py
-drwxrwxr-x   0 sp3rtah   (1000) sp3rtah   (1000)        0 2023-04-01 08:25:45.737945 autogram-3.3.2/autogram/updates/
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)     1328 2023-02-26 17:07:22.000000 autogram-3.3.2/autogram/updates/__init__.py
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)     1464 2023-01-19 13:26:28.000000 autogram-3.3.2/autogram/updates/callback_query.py
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)      374 2023-01-15 19:26:46.000000 autogram-3.3.2/autogram/updates/channel_post.py
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)      369 2023-01-15 19:26:46.000000 autogram-3.3.2/autogram/updates/chatJoin_request.py
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)      353 2023-01-15 19:26:46.000000 autogram-3.3.2/autogram/updates/chat_member.py
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)      378 2023-01-15 19:26:46.000000 autogram-3.3.2/autogram/updates/chosenInline_result.py
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)      375 2023-01-15 19:26:46.000000 autogram-3.3.2/autogram/updates/editedChannel_post.py
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)      362 2023-01-15 19:26:46.000000 autogram-3.3.2/autogram/updates/edited_message.py
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)      356 2023-01-18 09:56:23.000000 autogram-3.3.2/autogram/updates/inline_query.py
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)     4716 2023-02-26 17:07:22.000000 autogram-3.3.2/autogram/updates/message.py
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)      360 2023-01-15 19:26:46.000000 autogram-3.3.2/autogram/updates/myChat_member.py
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)      397 2023-01-15 19:26:46.000000 autogram-3.3.2/autogram/updates/notices.py
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)      333 2023-01-15 19:26:46.000000 autogram-3.3.2/autogram/updates/poll.py
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)      352 2023-02-26 17:07:22.000000 autogram-3.3.2/autogram/updates/poll_answer.py
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)      372 2023-01-15 19:26:46.000000 autogram-3.3.2/autogram/updates/precheckout_query.py
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)      362 2023-01-15 19:26:46.000000 autogram-3.3.2/autogram/updates/shipping_query.py
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)     1054 2023-02-26 07:40:30.000000 autogram-3.3.2/autogram/webhook.py
-drwxrwxr-x   0 sp3rtah   (1000) sp3rtah   (1000)        0 2023-04-01 08:25:45.725946 autogram-3.3.2/autogram.egg-info/
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)     7482 2023-04-01 08:25:45.000000 autogram-3.3.2/autogram.egg-info/PKG-INFO
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)      801 2023-04-01 08:25:45.000000 autogram-3.3.2/autogram.egg-info/SOURCES.txt
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)        1 2023-04-01 08:25:45.000000 autogram-3.3.2/autogram.egg-info/dependency_links.txt
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)       81 2023-04-01 08:25:45.000000 autogram-3.3.2/autogram.egg-info/requires.txt
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)        9 2023-04-01 08:25:45.000000 autogram-3.3.2/autogram.egg-info/top_level.txt
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)      773 2023-04-01 08:24:59.000000 autogram-3.3.2/pyproject.toml
--rw-rw-r--   0 sp3rtah   (1000) sp3rtah   (1000)       38 2023-04-01 08:25:45.737945 autogram-3.3.2/setup.cfg
+drwxrwxr-x   0 druid     (1001) druid     (1001)        0 2023-07-18 17:29:31.327509 autogram-3.4.0/
+-rw-rw-r--   0 druid     (1001) druid     (1001)     1064 2022-09-18 05:17:08.000000 autogram-3.4.0/LICENSE
+-rw-rw-r--   0 druid     (1001) druid     (1001)     4997 2023-07-18 17:29:31.327509 autogram-3.4.0/PKG-INFO
+-rw-rw-r--   0 druid     (1001) druid     (1001)     3265 2023-07-18 17:18:48.000000 autogram-3.4.0/README.md
+drwxrwxr-x   0 druid     (1001) druid     (1001)        0 2023-07-18 17:29:31.323509 autogram-3.4.0/autogram/
+-rw-rw-r--   0 druid     (1001) druid     (1001)      418 2023-07-18 17:18:48.000000 autogram-3.4.0/autogram/__init__.py
+-rw-rw-r--   0 druid     (1001) druid     (1001)     1913 2023-07-18 17:18:48.000000 autogram-3.4.0/autogram/app.py
+-rw-rw-r--   0 druid     (1001) druid     (1001)    11667 2023-07-18 17:18:48.000000 autogram-3.4.0/autogram/base.py
+-rw-rw-r--   0 druid     (1001) druid     (1001)     1514 2023-07-17 12:23:57.000000 autogram-3.4.0/autogram/config.py
+drwxrwxr-x   0 druid     (1001) druid     (1001)        0 2023-07-18 17:29:31.327509 autogram-3.4.0/autogram/updates/
+-rw-rw-r--   0 druid     (1001) druid     (1001)        0 2023-07-16 15:30:04.000000 autogram-3.4.0/autogram/updates/__init__.py
+-rw-rw-r--   0 druid     (1001) druid     (1001)        0 2023-07-16 15:30:04.000000 autogram-3.4.0/autogram/updates/base.py
+-rw-rw-r--   0 druid     (1001) druid     (1001)      940 2023-07-16 04:32:44.000000 autogram-3.4.0/autogram/webserver.py
+drwxrwxr-x   0 druid     (1001) druid     (1001)        0 2023-07-18 17:29:31.323509 autogram-3.4.0/autogram.egg-info/
+-rw-rw-r--   0 druid     (1001) druid     (1001)     4997 2023-07-18 17:29:31.000000 autogram-3.4.0/autogram.egg-info/PKG-INFO
+-rw-rw-r--   0 druid     (1001) druid     (1001)      340 2023-07-18 17:29:31.000000 autogram-3.4.0/autogram.egg-info/SOURCES.txt
+-rw-rw-r--   0 druid     (1001) druid     (1001)        1 2023-07-18 17:29:31.000000 autogram-3.4.0/autogram.egg-info/dependency_links.txt
+-rw-rw-r--   0 druid     (1001) druid     (1001)       85 2023-07-18 17:29:31.000000 autogram-3.4.0/autogram.egg-info/requires.txt
+-rw-rw-r--   0 druid     (1001) druid     (1001)        9 2023-07-18 17:29:31.000000 autogram-3.4.0/autogram.egg-info/top_level.txt
+-rw-rw-r--   0 druid     (1001) druid     (1001)      784 2023-07-18 17:18:48.000000 autogram-3.4.0/pyproject.toml
+-rw-rw-r--   0 druid     (1001) druid     (1001)       38 2023-07-18 17:29:31.327509 autogram-3.4.0/setup.cfg
```

### Comparing `autogram-3.3.2/LICENSE` & `autogram-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autogram-3.3.2/autogram/config.py` & `autogram-3.4.0/autogram/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 import os
 import sys
 import json
 from loguru import logger
 from typing import Callable, Dict
 
 default_config = {
-    'tcp-port': 4004,
-    'tcp-ip': 'ngrok',
-    'tcp-timeout': 10,
-    'max-workers': 32,
-    'echo-responses': False,
-    'media-quality': 'high',
-    'telegram-token': None,
+  'lport': 4004,
+  'media-quality': 'low',
+  'telegram-token': None
 }
 
-@logger.catch
 def load_config(config_file : str, config_path : str):
-    """Load configuration file from config_path dir"""
-    if not os.path.exists(config_path):
-        os.mkdir(config_path)
-    #
-    config_file = os.path.join(config_path, config_file)
-    if not os.path.exists(config_file):
-        with open(config_file, 'w') as conf:
-            json.dump(default_config, conf, indent=3)
-        print(f"Please edit [{config_file}]")
-        sys.exit(1)
-    config = {'config-file': config_file}
-    with open(config_file, 'r') as conf:
-        config |= json.load(conf)
-    return config
+  """Load configuration file from config_path dir"""
+  if not os.path.exists(config_path):
+    os.mkdir(config_path)
+  #
+  configuration = os.path.join(config_path, config_file)
+  if not os.path.exists(configuration):
+    with open(configuration, 'w') as conf:
+      json.dump(default_config, conf, indent=3)
+    logger.critical(f"Please edit [{configuration}]")
+    sys.exit(0)
+  config = {'config-file': configuration}
+  with open(configuration, 'r') as conf:
+    config |= json.load(conf)
+  return config
 
-@logger.catch
 def save_config(config :Dict):
-    """config-file must be in the dictionary"""
-    if config.get('config-file'):
-        conffile = config.pop('config-file')
-        with open(conffile, 'w') as conf:
-            json.dump(config, conf, indent=3)
-            conf.flush()
-        return True
-    return False
-
-@logger.catch
-def onStart(conf = 'autogram.json', confpath = '.'):
-    """Call custom function with config as parameter"""
-    def wrapper(func: Callable):
-        return func(load_config(conf, confpath))
-    return wrapper
+  """config-file must be in the dictionary"""
+  try:
+    conffile = config.pop('config-file')
+    with open(conffile, 'w') as conf:
+      json.dump(config, conf, indent=2)
+      conf.flush()
+  except:
+    conffile = conffile or None
+    if conffile:
+      return config | {'config-file': conffile}
+    else:
+      logger.critical('Failed saving config file!')
+
+def Start(config_file :str|None =None, config_path :str|None =None):
+  """Call custom function with config as parameter"""
+  config_path = config_path or os.getcwd()
+  config_file = config_file or 'autogram.json'
+  #
+  def wrapper(func: Callable):
+    return func(load_config(config_file, config_path))
+  return wrapper
 #
 
-__all__ = [ "onStart", "save_config", "load_config"]
-
+__all__ = [ "Start", "save_config", "load_config"]
```

### Comparing `autogram-3.3.2/autogram/webhook.py` & `autogram-3.4.0/autogram/webserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import socket
 from bottle import WSGIRefServer
 from wsgiref.simple_server import make_server
 from wsgiref.simple_server import WSGIRequestHandler, WSGIServer
 
-class MyServer(WSGIRefServer):
-    def run(self, app):
-        #
-        class FixedHandler(WSGIRequestHandler):
-            def address_string(self):
-                return self.client_address[0]
-            def log_request(*args, **kw):
-                if not self.quiet:
-                    return WSGIRequestHandler.log_request(*args, **kw)
-        #
-        handler_cls = self.options.get('handler_class', FixedHandler)
-        server_cls  = self.options.get('server_class', WSGIServer)
-        #
-        if ':' in self.host:
-            if getattr(server_cls, 'address_family') == socket.AF_INET:
-                class server_cls(server_cls):
-                    address_family = socket.AF_INET6
-        #
-        srv = make_server(self.host, self.port, app, server_cls, handler_cls)
-        self.srv = srv
-        srv.serve_forever()
-
-    def shutdown(self):
-        self.srv.shutdown()
+class WebServer(WSGIRefServer):
+  def run(self, app):
+    #
+    class FixedHandler(WSGIRequestHandler):
+      def address_string(self):
+        return self.client_address[0]
+      def log_request(*args, **kw):
+        if not self.quiet:
+          return WSGIRequestHandler.log_request(*args, **kw)
+    #
+    handler_cls = self.options.get('handler_class', FixedHandler)
+    server_cls  = self.options.get('server_class', WSGIServer)
+    #
+    if ':' in self.host:
+      if getattr(server_cls, 'address_family') == socket.AF_INET:
+        class server_cls(server_cls):
+          address_family = socket.AF_INET6
+    #
+    srv = make_server(self.host, self.port, app, server_cls, handler_cls)
+    self.srv = srv
+    srv.serve_forever()
 
+  def shutdown(self):
+    self.srv.shutdown()
```

### Comparing `autogram-3.3.2/pyproject.toml` & `autogram-3.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autogram"
-version = "3.3.2"
-description = "An extensible telegram API wrapper"
+version = "3.4.0"
+description = "An easily extensible telegram API wrapper"
 readme = "README.md"
 authors = [{ name = "sp3rtah", email = "ngaira14nelson@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["telegram", "API", "wrapper"]
 dependencies = [
-	"pexpect==4.8.0",
-	"loguru==0.6.0",
-	"bottle==0.12.23",
-	"requests==2.28.1",
+	"SQLAlchemy==2.0.19",
+	"loguru==0.7.0",
+	"bottle==0.12.25",
+	"requests==2.31.1",
 ]
 requires-python = ">=3.6"
 
 [project.optional-dependencies]
 dev = ["build", "twine"]
 
 [project.urls]
```

