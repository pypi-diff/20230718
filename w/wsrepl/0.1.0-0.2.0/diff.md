# Comparing `tmp/wsrepl-0.1.0.tar.gz` & `tmp/wsrepl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsrepl-0.1.0.tar", max compression
+gzip compressed data, was "wsrepl-0.2.0.tar", max compression
```

## Comparing `wsrepl-0.1.0.tar` & `wsrepl-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     5075 2023-06-12 14:27:41.314510 wsrepl-0.1.0/README.md
--rw-r--r--   0        0        0      585 2023-06-12 14:38:36.812621 wsrepl-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    10849 2023-06-12 13:59:53.045674 wsrepl-0.1.0/wsrepl/MessageHandler.py
--rw-r--r--   0        0        0      656 2023-06-08 13:01:11.368990 wsrepl-0.1.0/wsrepl/Ping0x1Thread.py
--rw-r--r--   0        0        0     2227 2023-06-08 12:41:39.436481 wsrepl-0.1.0/wsrepl/PingThread.py
--rw-r--r--   0        0        0     5307 2023-06-09 14:47:28.453637 wsrepl-0.1.0/wsrepl/Plugin.py
--rw-r--r--   0        0        0     6543 2023-06-08 13:08:08.895931 wsrepl-0.1.0/wsrepl/WSMessage.py
--rw-r--r--   0        0        0     5235 2023-06-07 21:31:52.548762 wsrepl-0.1.0/wsrepl/WebsocketConnection.py
--rw-r--r--   0        0        0      129 2023-06-08 13:33:01.480927 wsrepl-0.1.0/wsrepl/__init__.py
--rw-r--r--   0        0        0       34 2023-06-05 19:25:17.357359 wsrepl-0.1.0/wsrepl/__main__.py
--rw-r--r--   0        0        0     2456 2023-06-08 17:37:29.115404 wsrepl-0.1.0/wsrepl/app.css
--rw-r--r--   0        0        0     3875 2023-06-08 12:59:18.242328 wsrepl-0.1.0/wsrepl/app.py
--rw-r--r--   0        0        0     3776 2023-06-08 12:58:26.181417 wsrepl-0.1.0/wsrepl/cli.py
--rw-r--r--   0        0        0       25 2023-06-05 20:45:33.239158 wsrepl-0.1.0/wsrepl/constants.py
--rw-r--r--   0        0        0      945 2023-06-07 20:46:30.910701 wsrepl-0.1.0/wsrepl/log.py
--rw-r--r--   0        0        0     3428 2023-06-06 17:28:40.183946 wsrepl-0.1.0/wsrepl/utils.py
--rw-r--r--   0        0        0      566 2023-06-07 17:41:28.737261 wsrepl-0.1.0/wsrepl/widgets/CopyButton.py
--rw-r--r--   0        0        0      276 2023-06-05 21:54:34.842144 wsrepl-0.1.0/wsrepl/widgets/DirectionSign.py
--rw-r--r--   0        0        0      732 2023-06-08 12:12:44.695845 wsrepl-0.1.0/wsrepl/widgets/FormattedMessage.py
--rw-r--r--   0        0        0     2905 2023-06-08 12:07:26.915606 wsrepl-0.1.0/wsrepl/widgets/History.py
--rw-r--r--   0        0        0      314 2023-06-05 22:06:10.533999 wsrepl-0.1.0/wsrepl/widgets/HistoryIndex.py
--rw-r--r--   0        0        0     1460 2023-06-07 19:58:39.098093 wsrepl-0.1.0/wsrepl/widgets/HistoryRow.py
--rw-r--r--   0        0        0      418 2023-06-07 19:23:41.535567 wsrepl-0.1.0/wsrepl/widgets/Parent.py
--rw-r--r--   0        0        0      253 2023-06-08 13:32:52.732064 wsrepl-0.1.0/wsrepl/widgets/__init__.py
--rw-r--r--   0        0        0     5774 1970-01-01 00:00:00.000000 wsrepl-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6501 2023-07-18 15:55:56.236895 wsrepl-0.2.0/README.md
+-rw-r--r--   0        0        0      564 2023-07-18 16:41:53.346955 wsrepl-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    11502 2023-07-13 12:38:52.744359 wsrepl-0.2.0/wsrepl/MessageHandler.py
+-rw-r--r--   0        0        0      656 2023-06-08 13:01:11.368990 wsrepl-0.2.0/wsrepl/Ping0x1Thread.py
+-rw-r--r--   0        0        0     2227 2023-06-08 12:41:39.436481 wsrepl-0.2.0/wsrepl/PingThread.py
+-rw-r--r--   0        0        0     5137 2023-07-13 16:58:49.764288 wsrepl-0.2.0/wsrepl/Plugin.py
+-rw-r--r--   0        0        0     6543 2023-06-08 13:08:08.895931 wsrepl-0.2.0/wsrepl/WSMessage.py
+-rw-r--r--   0        0        0     5235 2023-06-07 21:31:52.548762 wsrepl-0.2.0/wsrepl/WebsocketConnection.py
+-rw-r--r--   0        0        0      129 2023-06-08 13:33:01.480927 wsrepl-0.2.0/wsrepl/__init__.py
+-rw-r--r--   0        0        0       34 2023-06-05 19:25:17.357359 wsrepl-0.2.0/wsrepl/__main__.py
+-rw-r--r--   0        0        0     2456 2023-06-08 17:37:29.115404 wsrepl-0.2.0/wsrepl/app.css
+-rw-r--r--   0        0        0     3948 2023-07-13 12:25:28.971827 wsrepl-0.2.0/wsrepl/app.py
+-rw-r--r--   0        0        0     5362 2023-07-13 12:50:14.547123 wsrepl-0.2.0/wsrepl/cli.py
+-rw-r--r--   0        0        0       25 2023-06-05 20:45:33.239158 wsrepl-0.2.0/wsrepl/constants.py
+-rw-r--r--   0        0        0      945 2023-06-07 20:46:30.910701 wsrepl-0.2.0/wsrepl/log.py
+-rw-r--r--   0        0        0     3434 2023-07-13 12:28:08.460208 wsrepl-0.2.0/wsrepl/utils.py
+-rw-r--r--   0        0        0      566 2023-06-07 17:41:28.737261 wsrepl-0.2.0/wsrepl/widgets/CopyButton.py
+-rw-r--r--   0        0        0      276 2023-06-05 21:54:34.842144 wsrepl-0.2.0/wsrepl/widgets/DirectionSign.py
+-rw-r--r--   0        0        0      732 2023-06-08 12:12:44.695845 wsrepl-0.2.0/wsrepl/widgets/FormattedMessage.py
+-rw-r--r--   0        0        0     2905 2023-06-08 12:07:26.915606 wsrepl-0.2.0/wsrepl/widgets/History.py
+-rw-r--r--   0        0        0      314 2023-06-05 22:06:10.533999 wsrepl-0.2.0/wsrepl/widgets/HistoryIndex.py
+-rw-r--r--   0        0        0     1460 2023-06-07 19:58:39.098093 wsrepl-0.2.0/wsrepl/widgets/HistoryRow.py
+-rw-r--r--   0        0        0      418 2023-06-07 19:23:41.535567 wsrepl-0.2.0/wsrepl/widgets/Parent.py
+-rw-r--r--   0        0        0      253 2023-06-08 13:32:52.732064 wsrepl-0.2.0/wsrepl/widgets/__init__.py
+-rw-r--r--   0        0        0     7158 1970-01-01 00:00:00.000000 wsrepl-0.2.0/PKG-INFO
```

### Comparing `wsrepl-0.1.0/README.md` & `wsrepl-0.2.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -2,61 +2,84 @@
 
 `wsrepl` is an interactive websocket REPL designed specifically for penetration testing. It provides an interface for observing incoming websocket messages and sending new ones, with an easy-to-use framework for automating this communication.
 
 ![Screenshot](docs/screenshot.png)
 
 ## Features
 
-- Interactively send and receive websocket messages.
-- Customize headers, ping/pong messages, and other parameters.
-- Handle SSL verification and reconnections.
-- Plug-in support for automating complex interaction scenarios.
-- Full logging and message history.
+- Interactively send and receive websocket messages
+- Customize headers, ping/pong messages, and other parameters
+- Handle SSL verification and reconnections
+- Plug-in support for automating complex interaction scenarios
+- Full logging and message history
+- Supports curl command line arguments for easy onboarding from Developer Tools or Burp Suite (use 'Copy as Curl' menu and replace `curl` with `wsrepl`)
 
 ## Installation
 
 You can download and install wsrepl using pip:
 
 ```
 pip install wsrepl
 ```
 
+Alternatively, you can clone this repository and install it from source:
+
+```
+git clone https://github.com/doyensec/wsrepl
+cd wsrepl
+pip install .
+```
+
 ## Usage
 
 The basic command for starting wsrepl is as follows:
 
 ```
 wsrepl -u URL
 ```
 
 Replace URL with your target websocket URL, e.g. `wss://echo.websocket.org`. For more options and settings, you can use the -h or --help option:
 
 ```
-usage: wsrepl [-h] -u URL [-s] [-A USER_AGENT] [-O ORIGIN] [-H HEADER]
+usage: wsrepl [-h] [-u URL] [-i] [-s] [-k] [-X REQUEST] [-H HEADER]
+              [-b COOKIE] [--compressed] [-S] [-A USER_AGENT] [-O ORIGIN]
               [-F HEADERS_FILE] [--no-native-ping]
               [--ping-interval PING_INTERVAL] [--hide-ping-pong]
               [--ping-0x1-interval PING_0X1_INTERVAL]
               [--ping-0x1-payload PING_0X1_PAYLOAD]
               [--pong-0x1-payload PONG_0X1_PAYLOAD] [--hide-0x1-ping-pong]
-              [-t TTL] [-p HTTP_PROXY] [-k] [-r RECONNECT_INTERVAL]
-              [-i INITIAL_MESSAGES] [-P PLUGIN] [-v VERBOSE]
+              [-t TTL] [-p HTTP_PROXY] [-r RECONNECT_INTERVAL]
+              [-I INITIAL_MESSAGES] [-P PLUGIN] [-v VERBOSE]
+              [url_positional]
 
 Websocket Client
 
+positional arguments:
+  url_positional        Websocket URL (e.g. wss://echo.websocket.org)
+
 options:
   -h, --help            show this help message and exit
   -u URL, --url URL     Websocket URL (e.g. wss://echo.websocket.org)
-  -s, --small           Smaller UI
+  -i, --include         No effect, just for curl compatibility
+  -s, --silent          No effect, just for curl compatibility
+  -k, --insecure        Disable SSL verification
+  -X REQUEST, --request REQUEST
+                        No effect, just for curl compatibility
+  -H HEADER, --header HEADER
+                        Additional header (e.g. "X-Header: value"), can be
+                        used multiple times
+  -b COOKIE, --cookie COOKIE
+                        Cookie header (e.g. "name=value"), can be used
+                        multiple times
+  --compressed          No effect, just for curl compatibility
+  -S, --small           Smaller UI
   -A USER_AGENT, --user-agent USER_AGENT
                         User-Agent header
   -O ORIGIN, --origin ORIGIN
                         Origin header
-  -H HEADER, --header HEADER
-                        Additional header (e.g. "X-Header: value"), can be
-                        used multiple times
   -F HEADERS_FILE, --headers-file HEADERS_FILE
                         Additional headers file (e.g. "headers.txt")
   --no-native-ping      Disable native ping/pong messages
   --ping-interval PING_INTERVAL
                         Ping interval (seconds)
   --hide-ping-pong      Hide ping/pong messages
   --ping-0x1-interval PING_0X1_INTERVAL
@@ -65,18 +88,17 @@
                         Fake ping (0x1 opcode) payload
   --pong-0x1-payload PONG_0X1_PAYLOAD
                         Fake pong (0x1 opcode) payload
   --hide-0x1-ping-pong  Hide fake ping/pong messages
   -t TTL, --ttl TTL     Heartbeet interval (seconds)
   -p HTTP_PROXY, --http-proxy HTTP_PROXY
                         HTTP Proxy Address (e.g. 127.0.0.1:8080)
-  -k, --insecure        Disable SSL verification
   -r RECONNECT_INTERVAL, --reconnect-interval RECONNECT_INTERVAL
                         Reconnect interval (seconds, default: 2)
-  -i INITIAL_MESSAGES, --initial-messages INITIAL_MESSAGES
+  -I INITIAL_MESSAGES, --initial-messages INITIAL_MESSAGES
                         Send the messages from this file on connect
   -P PLUGIN, --plugin PLUGIN
                         Plugin file to load
   -v VERBOSE, --verbose VERBOSE
                         Verbosity level, 1-4 default: 3 (errors, warnings,
                         info), 4 adds debug
 ```
@@ -104,15 +126,17 @@
     async def on_message_received(self, message: WSMessage):
         # This method is called when a message is received from the server.
         pass
 
     # ... Other hooks can be defined here.
 ```
 
-Refer to the source of [Plugin class](wsrepl/Plugin.py) for the full list of hooks you can use and what they do.
+Refer to the source of [Plugin class](wsrepl/Plugin.py) for the full list of hooks you can use and what they do:
+
+![Plugin Hooks](docs/hooks-mermaid.png)
 
 ### Example Plugin
 
 Here is an example of a plugin that sends a predefined authentication message to a server:
 
 ```python
 from wsrepl import Plugin
@@ -134,10 +158,19 @@
 
 ```
 wsrepl -u URL -P auth_plugin.py
 ```
 
 Replace URL with your target websocket URL and auth_plugin.py with the path to the Python file containing your plugin.
 
+[docs/](./docs/) directory contains a few more example plugins.
+
 ## Contributing
 
-Contributions to wsrepl are welcome!
+Contributions to wsrepl are welcome! Please, [create an issue](https://github.com/doyensec/wsrepl/issues) or submit a pull request if you have any ideas or suggestions. In particular, adding more plugin examples would be very helpful.
+
+## Credits
+
+This project has been sponsored by [Doyensec LLC](https://www.doyensec.com/).
+
+![Doyensec Research](https://raw.githubusercontent.com/doyensec/inql/master/docs/doyensec_logo.svg "Doyensec Logo")
+
```

### Comparing `wsrepl-0.1.0/pyproject.toml` & `wsrepl-0.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
 name = "wsrepl"
-version = "0.1.0"
+version = "0.2.0"
 description = "Websocket REPL for pentesters"
 authors = ["Andrew Konstantinov <105389353+execveat@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/doyensec/wsrepl"
 keywords = ["websocket", "pentesting"]
 
 [tool.poetry.dependencies]
 python = ">3.10,<4.0"
 websocket-client = "^1.5.2"
-Pygments = "^2.15.1"
 pyperclip = "^1.8.2"
-rich = "^13.3.3"
-textual = "^0.27.0"
+rich = "^13.4.2"
+textual = "^0.30.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 wsrepl = "wsrepl:cli"
```

### Comparing `wsrepl-0.1.0/wsrepl/MessageHandler.py` & `wsrepl-0.2.0/wsrepl/MessageHandler.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 class MessageHandler:
     def __init__(self,
                  app: textual.app.App,
                  url: str,
                  user_agent: str | None         = None,
                  origin: str | None             = None,
+                 cookies: list[str] | None      = None,
                  headers: list[str] | None      = None,
                  headers_file: str | None       = None,
                  ping_interval: int | float     = 24,
                  hide_ping_pong: bool           = False,
                  ping_0x1_interval: int | float = 24,
                  ping_0x1_payload: str | None   = None,
                  pong_0x1_payload: str | None   = None,
@@ -32,30 +33,30 @@
                  verify_tls: bool               = True,
                  initial_msgs_file: str | None  = None,
                  plugin_path: str | None        = None) -> None:
 
         self.app = app
         self.plugin = load_plugin(plugin_path)(message_handler=self)
         self.initial_messages: list[WSMessage] = self._load_initial_messages(initial_msgs_file)
-        headers: OrderedDict = self._process_headers(headers, headers_file, user_agent, origin)
+        processed_headers: OrderedDict = self._process_headers(headers, headers_file, user_agent, origin, cookies)
 
         self._ws = WebsocketConnection(
             # Stuff WebsocketConnection needs to call back to us
             async_handler=self,
             # WebSocketApp args
             url=url,
-            header=headers
+            header=processed_headers
         )
 
         # Args passed to websocket.WebSocketApp.run_forever()
         if isinstance(proxy, str):
             proxy = 'http://' + proxy if '://' not in proxy else proxy
 
         self._ws.connect_args = {
-            'suppress_origin': 'Origin' in headers,
+            'suppress_origin': 'Origin' in processed_headers,
             'sslopt': {'cert_reqs': ssl.CERT_NONE} if not verify_tls else {},
             'ping_interval': 0, # Disable websocket-client's autoping because it doesn't provide feedback
             'http_proxy_host': urlparse(proxy).hostname if proxy else None,
             'http_proxy_port': urlparse(proxy).port if proxy else None,
             'proxy_type': 'http' if proxy else None,
             'reconnect': reconnect_interval
         }
@@ -78,41 +79,54 @@
             self.ping_0x1_thread = None
 
         # Whether to show ping / pong messages in the history
         self.hide_ping_pong = hide_ping_pong
         self.hide_0x1_ping_pong = hide_0x1_ping_pong
 
     def _process_headers(self, headers: list[str] | None, headers_file: str | None,
-                         user_agent: str | None, origin: str | None) -> OrderedDict:
+                         user_agent: str | None, origin: str | None, cookies: list[str]) -> OrderedDict:
         """Process headers and return an OrderedDict of headers."""
         result = OrderedDict()
+        cookie_headers = []
 
         # Headers from command line take precedence
         if headers:
             for header in headers:
                 name, value = map(str.strip, header.split(":", 1))
-                result[name] = value
+                if name.lower().strip() == "cookie":
+                    cookie_headers.append(value.strip())
+                else:
+                    result[name] = value
 
         # Headers from file are next
         if headers_file:
             with open(headers_file, "r") as f:
                 for header in f.read().splitlines():
                     name, value = map(str.strip, header.split(":", 1))
-                    if name in result:
-                        continue
-                    result[name] = value
+                    if name.lower().strip() == "cookie":
+                        cookie_headers.append(value.strip())
+                    elif name not in result:
+                        result[name] = value
 
         # Add User-Agent if not already present
         if user_agent and "User-Agent" not in result:
             result["User-Agent"] = user_agent
 
         # Add Origin if not already present
         if origin and "Origin" not in result:
             result["Origin"] = origin
 
+        # Merge and add Cookies
+        if cookies:
+            cookie_value = "; ".join(cookies)
+            if cookie_headers:
+                result['Cookie'] = cookie_value + "; " + "; ".join(cookie_headers)
+            else:
+                result['Cookie'] = cookie_value
+
         return result
 
     def _load_initial_messages(self, initial_msgs_file: str | None) -> list[WSMessage]:
         messages = []
         if initial_msgs_file:
             with open(initial_msgs_file, "r") as f:
                 for msg in f.readlines():
```

### Comparing `wsrepl-0.1.0/wsrepl/Ping0x1Thread.py` & `wsrepl-0.2.0/wsrepl/Ping0x1Thread.py`

 * *Files identical despite different names*

### Comparing `wsrepl-0.1.0/wsrepl/PingThread.py` & `wsrepl-0.2.0/wsrepl/PingThread.py`

 * *Files identical despite different names*

### Comparing `wsrepl-0.1.0/wsrepl/Plugin.py` & `wsrepl-0.2.0/wsrepl/Plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,29 +47,25 @@
     async def after_connect(self) -> None:
         pass
 
     async def on_disconnect(self) -> None:
         """Called when the websocket connection is lost"""
         pass
 
-    async def on_reconnect(self, timeout: int) -> None:
-        """Called when the websocket connection is lost, but will be reconnected after a timeout"""
-        pass
-
     # Message frame
     async def on_message_received(self, message: WSMessage) -> None:
         """Called when a (text) message is received from the server. Can modify the message before it is pushed to the history.
 
         - message.msg contains the original message received from the server (should not be modified)
         - message.short contains a shortened version of the message that will be displayed in the history (can be overwritten)
         - message.long contains a long version of the message that will be displayed upon selection (can be overwritten)
 
         - message.is_hidden - if True, the message will not be displayed in the history
 
-        ! Do not use this hook to send respondes to the server. Use the after_message_received hook instead !
+        ! Do not use this hook to send responses to the server. Use the after_message_received hook instead !
         """
         pass
 
     async def after_message_received(self, message: WSMessage) -> None:
         """Called after a message is received from the server. Use this hook to send responses to the server."""
         pass
```

### Comparing `wsrepl-0.1.0/wsrepl/WSMessage.py` & `wsrepl-0.2.0/wsrepl/WSMessage.py`

 * *Files identical despite different names*

### Comparing `wsrepl-0.1.0/wsrepl/WebsocketConnection.py` & `wsrepl-0.2.0/wsrepl/WebsocketConnection.py`

 * *Files identical despite different names*

### Comparing `wsrepl-0.1.0/wsrepl/app.css` & `wsrepl-0.2.0/wsrepl/app.css`

 * *Files identical despite different names*

### Comparing `wsrepl-0.1.0/wsrepl/app.py` & `wsrepl-0.2.0/wsrepl/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,15 @@
                  # URL is the only required argument
                  url: str,
                  # UI settings
                  small: bool                    = False,
                  # Websocket settings
                  user_agent: str | None         = None,
                  origin: str | None             = None,
+                 cookies: list[str] | None      = None,
                  headers: list[str] | None      = None,
                  headers_file: str | None       = None,
                  ping_interval: int | float     = 24, # 0 -> disable auto ping
                  hide_ping_pong: bool           = False,
                  ping_0x1_interval: int | float = 24, # 0 -> disable fake ping
                  ping_0x1_payload: str | None   = None,
                  pong_0x1_payload: str | None   = None,
@@ -52,15 +53,15 @@
 
         # Verbosity for logging level
         self.verbosity = verbosity
 
         # Message handler, spawns a thread to handle the websocket connection
         self.message_handler = MessageHandler(
             app=self,
-            url=url, user_agent=user_agent, origin=origin, headers=headers, headers_file=headers_file,
+            url=url, user_agent=user_agent, origin=origin, cookies=cookies, headers=headers, headers_file=headers_file,
             ping_interval=ping_interval, hide_ping_pong=hide_ping_pong,
             ping_0x1_interval=ping_0x1_interval, ping_0x1_payload=ping_0x1_payload, pong_0x1_payload=pong_0x1_payload,
             hide_0x1_ping_pong=hide_0x1_ping_pong,
             reconnect_interval=reconnect_interval, proxy=proxy, verify_tls=verify_tls,
             initial_msgs_file=initial_msgs_file, plugin_path=plugin_path
         )
```

### Comparing `wsrepl-0.1.0/wsrepl/log.py` & `wsrepl-0.2.0/wsrepl/log.py`

 * *Files identical despite different names*

### Comparing `wsrepl-0.1.0/wsrepl/utils.py` & `wsrepl-0.2.0/wsrepl/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 def _get_plugin_name(plugin_path):
     # Extracts the module name from the plugin file path
     plugin_file = os.path.basename(plugin_path)
     plugin_name = os.path.splitext(plugin_file)[0]
     return plugin_name
 
 
-def load_plugin(plugin_path) -> Plugin:
+def load_plugin(plugin_path) -> type[Plugin]:
     """Loads a plugin from a file path or returns an empty plugin if no path is specified"""
     if not plugin_path:
         return Plugin
 
     plugin_name = _get_plugin_name(plugin_path)
     spec = importlib.util.spec_from_file_location(plugin_name, plugin_path)
     module = importlib.util.module_from_spec(spec)
```

### Comparing `wsrepl-0.1.0/wsrepl/widgets/CopyButton.py` & `wsrepl-0.2.0/wsrepl/widgets/CopyButton.py`

 * *Files identical despite different names*

### Comparing `wsrepl-0.1.0/wsrepl/widgets/FormattedMessage.py` & `wsrepl-0.2.0/wsrepl/widgets/FormattedMessage.py`

 * *Files identical despite different names*

### Comparing `wsrepl-0.1.0/wsrepl/widgets/History.py` & `wsrepl-0.2.0/wsrepl/widgets/History.py`

 * *Files identical despite different names*

### Comparing `wsrepl-0.1.0/wsrepl/widgets/HistoryRow.py` & `wsrepl-0.2.0/wsrepl/widgets/HistoryRow.py`

 * *Files identical despite different names*

### Comparing `wsrepl-0.1.0/PKG-INFO` & `wsrepl-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,82 +1,104 @@
 Metadata-Version: 2.1
 Name: wsrepl
-Version: 0.1.0
+Version: 0.2.0
 Summary: Websocket REPL for pentesters
 Home-page: https://github.com/doyensec/wsrepl
 License: MIT
 Keywords: websocket,pentesting
 Author: Andrew Konstantinov
 Author-email: 105389353+execveat@users.noreply.github.com
 Requires-Python: >3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Pygments (>=2.15.1,<3.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
-Requires-Dist: rich (>=13.3.3,<14.0.0)
-Requires-Dist: textual (>=0.27.0,<0.28.0)
+Requires-Dist: rich (>=13.4.2,<14.0.0)
+Requires-Dist: textual (>=0.30.0,<0.31.0)
 Requires-Dist: websocket-client (>=1.5.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 # `wsrepl` - Websocket REPL for pentesters
 
 `wsrepl` is an interactive websocket REPL designed specifically for penetration testing. It provides an interface for observing incoming websocket messages and sending new ones, with an easy-to-use framework for automating this communication.
 
 ![Screenshot](docs/screenshot.png)
 
 ## Features
 
-- Interactively send and receive websocket messages.
-- Customize headers, ping/pong messages, and other parameters.
-- Handle SSL verification and reconnections.
-- Plug-in support for automating complex interaction scenarios.
-- Full logging and message history.
+- Interactively send and receive websocket messages
+- Customize headers, ping/pong messages, and other parameters
+- Handle SSL verification and reconnections
+- Plug-in support for automating complex interaction scenarios
+- Full logging and message history
+- Supports curl command line arguments for easy onboarding from Developer Tools or Burp Suite (use 'Copy as Curl' menu and replace `curl` with `wsrepl`)
 
 ## Installation
 
 You can download and install wsrepl using pip:
 
 ```
 pip install wsrepl
 ```
 
+Alternatively, you can clone this repository and install it from source:
+
+```
+git clone https://github.com/doyensec/wsrepl
+cd wsrepl
+pip install .
+```
+
 ## Usage
 
 The basic command for starting wsrepl is as follows:
 
 ```
 wsrepl -u URL
 ```
 
 Replace URL with your target websocket URL, e.g. `wss://echo.websocket.org`. For more options and settings, you can use the -h or --help option:
 
 ```
-usage: wsrepl [-h] -u URL [-s] [-A USER_AGENT] [-O ORIGIN] [-H HEADER]
+usage: wsrepl [-h] [-u URL] [-i] [-s] [-k] [-X REQUEST] [-H HEADER]
+              [-b COOKIE] [--compressed] [-S] [-A USER_AGENT] [-O ORIGIN]
               [-F HEADERS_FILE] [--no-native-ping]
               [--ping-interval PING_INTERVAL] [--hide-ping-pong]
               [--ping-0x1-interval PING_0X1_INTERVAL]
               [--ping-0x1-payload PING_0X1_PAYLOAD]
               [--pong-0x1-payload PONG_0X1_PAYLOAD] [--hide-0x1-ping-pong]
-              [-t TTL] [-p HTTP_PROXY] [-k] [-r RECONNECT_INTERVAL]
-              [-i INITIAL_MESSAGES] [-P PLUGIN] [-v VERBOSE]
+              [-t TTL] [-p HTTP_PROXY] [-r RECONNECT_INTERVAL]
+              [-I INITIAL_MESSAGES] [-P PLUGIN] [-v VERBOSE]
+              [url_positional]
 
 Websocket Client
 
+positional arguments:
+  url_positional        Websocket URL (e.g. wss://echo.websocket.org)
+
 options:
   -h, --help            show this help message and exit
   -u URL, --url URL     Websocket URL (e.g. wss://echo.websocket.org)
-  -s, --small           Smaller UI
+  -i, --include         No effect, just for curl compatibility
+  -s, --silent          No effect, just for curl compatibility
+  -k, --insecure        Disable SSL verification
+  -X REQUEST, --request REQUEST
+                        No effect, just for curl compatibility
+  -H HEADER, --header HEADER
+                        Additional header (e.g. "X-Header: value"), can be
+                        used multiple times
+  -b COOKIE, --cookie COOKIE
+                        Cookie header (e.g. "name=value"), can be used
+                        multiple times
+  --compressed          No effect, just for curl compatibility
+  -S, --small           Smaller UI
   -A USER_AGENT, --user-agent USER_AGENT
                         User-Agent header
   -O ORIGIN, --origin ORIGIN
                         Origin header
-  -H HEADER, --header HEADER
-                        Additional header (e.g. "X-Header: value"), can be
-                        used multiple times
   -F HEADERS_FILE, --headers-file HEADERS_FILE
                         Additional headers file (e.g. "headers.txt")
   --no-native-ping      Disable native ping/pong messages
   --ping-interval PING_INTERVAL
                         Ping interval (seconds)
   --hide-ping-pong      Hide ping/pong messages
   --ping-0x1-interval PING_0X1_INTERVAL
@@ -85,18 +107,17 @@
                         Fake ping (0x1 opcode) payload
   --pong-0x1-payload PONG_0X1_PAYLOAD
                         Fake pong (0x1 opcode) payload
   --hide-0x1-ping-pong  Hide fake ping/pong messages
   -t TTL, --ttl TTL     Heartbeet interval (seconds)
   -p HTTP_PROXY, --http-proxy HTTP_PROXY
                         HTTP Proxy Address (e.g. 127.0.0.1:8080)
-  -k, --insecure        Disable SSL verification
   -r RECONNECT_INTERVAL, --reconnect-interval RECONNECT_INTERVAL
                         Reconnect interval (seconds, default: 2)
-  -i INITIAL_MESSAGES, --initial-messages INITIAL_MESSAGES
+  -I INITIAL_MESSAGES, --initial-messages INITIAL_MESSAGES
                         Send the messages from this file on connect
   -P PLUGIN, --plugin PLUGIN
                         Plugin file to load
   -v VERBOSE, --verbose VERBOSE
                         Verbosity level, 1-4 default: 3 (errors, warnings,
                         info), 4 adds debug
 ```
@@ -124,15 +145,17 @@
     async def on_message_received(self, message: WSMessage):
         # This method is called when a message is received from the server.
         pass
 
     # ... Other hooks can be defined here.
 ```
 
-Refer to the source of [Plugin class](wsrepl/Plugin.py) for the full list of hooks you can use and what they do.
+Refer to the source of [Plugin class](wsrepl/Plugin.py) for the full list of hooks you can use and what they do:
+
+![Plugin Hooks](docs/hooks-mermaid.png)
 
 ### Example Plugin
 
 Here is an example of a plugin that sends a predefined authentication message to a server:
 
 ```python
 from wsrepl import Plugin
@@ -154,11 +177,20 @@
 
 ```
 wsrepl -u URL -P auth_plugin.py
 ```
 
 Replace URL with your target websocket URL and auth_plugin.py with the path to the Python file containing your plugin.
 
+[docs/](./docs/) directory contains a few more example plugins.
+
 ## Contributing
 
-Contributions to wsrepl are welcome!
+Contributions to wsrepl are welcome! Please, [create an issue](https://github.com/doyensec/wsrepl/issues) or submit a pull request if you have any ideas or suggestions. In particular, adding more plugin examples would be very helpful.
+
+## Credits
+
+This project has been sponsored by [Doyensec LLC](https://www.doyensec.com/).
+
+![Doyensec Research](https://raw.githubusercontent.com/doyensec/inql/master/docs/doyensec_logo.svg "Doyensec Logo")
+
```

