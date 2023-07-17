# Comparing `tmp/oobabot_plugin-0.2.0.tar.gz` & `tmp/oobabot_plugin-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oobabot_plugin-0.2.0.tar", max compression
+gzip compressed data, was "oobabot_plugin-0.2.1.tar", max compression
```

## Comparing `oobabot_plugin-0.2.0.tar` & `oobabot_plugin-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1067 2023-05-24 23:25:59.529104 oobabot_plugin-0.2.0/LICENSE
--rw-r--r--   0        0        0     1951 2023-05-24 23:25:59.529239 oobabot_plugin-0.2.0/README.md
--rw-r--r--   0        0        0     1871 2023-07-07 10:24:51.238182 oobabot_plugin-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      264 2023-06-24 23:44:13.221133 oobabot_plugin-0.2.0/src/oobabot_plugin/__init__.py
--rw-r--r--   0        0        0     7536 2023-06-24 09:50:54.210004 oobabot_plugin-0.2.0/src/oobabot_plugin/bootstrap.py
--rw-r--r--   0        0        0     7784 2023-07-07 10:24:51.240296 oobabot_plugin-0.2.0/src/oobabot_plugin/button_enablers.py
--rw-r--r--   0        0        0     9560 2023-07-07 10:24:51.240670 oobabot_plugin-0.2.0/src/oobabot_plugin/button_handlers.py
--rw-r--r--   0        0        0     3039 2023-07-07 10:24:51.241673 oobabot_plugin-0.2.0/src/oobabot_plugin/controller.py
--rw-r--r--   0        0        0     9903 2023-05-25 05:24:15.485352 oobabot_plugin-0.2.0/src/oobabot_plugin/input_handlers.py
--rw-r--r--   0        0        0     3305 2023-05-25 06:56:54.200392 oobabot_plugin-0.2.0/src/oobabot_plugin/install.py
--rw-r--r--   0        0        0      806 2023-05-24 23:25:59.534874 oobabot_plugin-0.2.0/src/oobabot_plugin/instructions.md
--rw-r--r--   0        0        0    15924 2023-07-07 10:24:51.242055 oobabot_plugin-0.2.0/src/oobabot_plugin/layout.py
--rw-r--r--   0        0        0     4826 2023-07-07 10:26:33.202649 oobabot_plugin-0.2.0/src/oobabot_plugin/oobabot_log.css
--rw-r--r--   0        0        0      498 2023-06-26 15:36:57.565953 oobabot_plugin-0.2.0/src/oobabot_plugin/oobabot_log.js
--rw-r--r--   0        0        0     1144 2023-06-24 06:51:19.539687 oobabot_plugin-0.2.0/src/oobabot_plugin/script.py
--rw-r--r--   0        0        0      783 2023-06-22 12:29:04.858021 oobabot_plugin-0.2.0/src/oobabot_plugin/server.py
--rw-r--r--   0        0        0     4446 2023-07-07 10:24:51.243563 oobabot_plugin-0.2.0/src/oobabot_plugin/strings.py
--rw-r--r--   0        0        0      211 2023-07-07 10:24:51.243788 oobabot_plugin-0.2.0/src/oobabot_plugin/transcript.md
--rw-r--r--   0        0        0     5702 2023-07-07 10:24:51.244597 oobabot_plugin-0.2.0/src/oobabot_plugin/transcript_view.py
--rw-r--r--   0        0        0     8867 2023-07-05 22:59:41.850315 oobabot_plugin-0.2.0/src/oobabot_plugin/worker.py
--rw-r--r--   0        0        0     2743 1970-01-01 00:00:00.000000 oobabot_plugin-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-24 23:25:59.529104 oobabot_plugin-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1951 2023-05-24 23:25:59.529239 oobabot_plugin-0.2.1/README.md
+-rw-r--r--   0        0        0     1892 2023-07-17 23:13:28.166029 oobabot_plugin-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      264 2023-07-17 23:13:28.166406 oobabot_plugin-0.2.1/src/oobabot_plugin/__init__.py
+-rw-r--r--   0        0        0     7536 2023-06-24 09:50:54.210004 oobabot_plugin-0.2.1/src/oobabot_plugin/bootstrap.py
+-rw-r--r--   0        0        0     7976 2023-07-12 11:59:27.606739 oobabot_plugin-0.2.1/src/oobabot_plugin/button_enablers.py
+-rw-r--r--   0        0        0     9560 2023-07-07 10:24:51.240670 oobabot_plugin-0.2.1/src/oobabot_plugin/button_handlers.py
+-rw-r--r--   0        0        0     3385 2023-07-12 10:54:51.062187 oobabot_plugin-0.2.1/src/oobabot_plugin/controller.py
+-rw-r--r--   0        0        0     9903 2023-05-25 05:24:15.485352 oobabot_plugin-0.2.1/src/oobabot_plugin/input_handlers.py
+-rw-r--r--   0        0        0     3305 2023-05-25 06:56:54.200392 oobabot_plugin-0.2.1/src/oobabot_plugin/install.py
+-rw-r--r--   0        0        0      806 2023-05-24 23:25:59.534874 oobabot_plugin-0.2.1/src/oobabot_plugin/instructions.md
+-rw-r--r--   0        0        0    16325 2023-07-12 11:58:29.964662 oobabot_plugin-0.2.1/src/oobabot_plugin/layout.py
+-rw-r--r--   0        0        0     4100 2023-07-12 12:09:49.203841 oobabot_plugin-0.2.1/src/oobabot_plugin/oobabot_log.css
+-rw-r--r--   0        0        0      498 2023-06-26 15:36:57.565953 oobabot_plugin-0.2.1/src/oobabot_plugin/oobabot_log.js
+-rw-r--r--   0        0        0     1144 2023-06-24 06:51:19.539687 oobabot_plugin-0.2.1/src/oobabot_plugin/script.py
+-rw-r--r--   0        0        0      783 2023-06-22 12:29:04.858021 oobabot_plugin-0.2.1/src/oobabot_plugin/server.py
+-rw-r--r--   0        0        0     6740 2023-07-12 12:05:48.229050 oobabot_plugin-0.2.1/src/oobabot_plugin/strings.py
+-rw-r--r--   0        0        0      211 2023-07-07 10:24:51.243788 oobabot_plugin-0.2.1/src/oobabot_plugin/transcript.md
+-rw-r--r--   0        0        0     5702 2023-07-12 10:44:52.595621 oobabot_plugin-0.2.1/src/oobabot_plugin/transcript_view.py
+-rw-r--r--   0        0        0     9034 2023-07-12 10:44:41.273374 oobabot_plugin-0.2.1/src/oobabot_plugin/worker.py
+-rw-r--r--   0        0        0     2743 1970-01-01 00:00:00.000000 oobabot_plugin-0.2.1/PKG-INFO
```

### Comparing `oobabot_plugin-0.2.0/LICENSE` & `oobabot_plugin-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.2.0/README.md` & `oobabot_plugin-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.2.0/pyproject.toml` & `oobabot_plugin-0.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "oobabot-plugin"
-version = "0.2.0"
+version = "0.2.1"
 description = "A Discord bot plugin to oobabooga's text-generation-webui, based on oobabot."
 authors = ["Christopher Rude <chris@rudesoftware.net>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/chrisrude/oobabot-plugin"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
-oobabot = "^0.2.0"
+oobabot = "^0.2.1"
 # oobabot = { path = "../oobabot" }
 # we can't use the latest version of gradio, since a range of
 # text-generation-webui versions are incompatible with it.  But
 # we don't want to use a version older than 3.34.0, since those
 # have serious security issues.  So this version seems like the
 # only compromise, until at least text-generation-webui supports
 # a newer version of gradio.
@@ -41,16 +41,17 @@
 pycodestyle = ["-E203", "-W503", "-W504"]
 
 [tool.poetry.group.test.dependencies]
 black = "^23.3.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 pre-commit = "^3.2.0"
-pytest = "^7.1"
 pylint = "^2.17.4"
+pyright = "^1.1.316"
+pytest = "^7.1"
 
 [tool.isort]
 profile = "black"
 force_single_line = true
 force_sort_within_sections = true
 single_line_exclusions = ["typing", "typing_extensions"]
```

### Comparing `oobabot_plugin-0.2.0/src/oobabot_plugin/bootstrap.py` & `oobabot_plugin-0.2.1/src/oobabot_plugin/bootstrap.py`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.2.0/src/oobabot_plugin/button_enablers.py` & `oobabot_plugin-0.2.1/src/oobabot_plugin/button_enablers.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,15 @@
         )
 
         # enable or disable all other input controls based on the running state
         layout.running_state_textbox.change(
             self._handle_running_state_change,
             inputs=[layout.running_state_textbox],
             outputs=[
+                layout.status_html,
                 layout.start_button,
                 layout.stop_button,
                 layout.save_settings_button,
                 layout.discord_token_save_button,
                 layout.advanced_save_settings_button,
                 layout.advanced_yaml_editor,
                 *self._get_input_handlers().keys(),
@@ -137,22 +138,26 @@
             enable_stop = False
             enable_advanced = True
             enable_inputs_and_start = True
         else:
             raise ValueError(f"unknown running state: {running_state}")
 
         # order of outputs:
+        #   layout.status_markdown,
         #   layout.start_button,
         #   layout.stop_button,
         #   layout.save_settings_button,
         #   layout.discord_token_save_button
         #   layout.advanced_save_settings_button,
         #   layout.advanced_yaml_editor,
         #   *self._get_input_handlers().keys(),
         results = [
+            self.layout.status_html.update(
+                value=strings.status_heading(running_state),
+            ),
             self.layout.start_button.update(interactive=enable_inputs_and_start),
             self.layout.stop_button.update(interactive=enable_stop),
             self.layout.save_settings_button.update(
                 interactive=enable_inputs_and_start
             ),
             self.layout.discord_token_save_button.update(
                 interactive=enable_inputs_and_start
```

### Comparing `oobabot_plugin-0.2.0/src/oobabot_plugin/button_handlers.py` & `oobabot_plugin-0.2.1/src/oobabot_plugin/button_handlers.py`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.2.0/src/oobabot_plugin/controller.py` & `oobabot_plugin-0.2.1/src/oobabot_plugin/controller.py`

 * *Files 15% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
         t_view = transcript_view.TranscriptView(
             self.worker.get_transcript,
             self.worker.get_fancy_author,
         )
 
         self.layout.layout_ui(
-            get_logs=self.worker.get_logs,
+            get_log_etag=self.worker.get_log_etag,
             has_plausible_token=plausible_token,
             stable_diffusion_keywords=stable_diffusion_keywords,
             api_extension_loaded=self.api_extension_loaded,
             is_using_character=is_using_character,
             get_transcript_html=t_view.get_html,
             is_voice_enabled=self.worker.is_voice_enabled(),
         )
@@ -79,10 +79,19 @@
         )
 
         # sets up what happens when each button is pressed
         button_handlers.ButtonHandlers(
             is_using_character, self.layout, self.worker, enablers
         )
 
+        # when the log etag changes, update the log html
+        self.layout.log_etag_textbox.change(
+            lambda _etag: self.layout.log_output_html.update(
+                value=self.worker.get_logs(),
+            ),
+            inputs=[self.layout.log_etag_textbox],
+            outputs=[self.layout.log_output_html],
+        )
+
         # start the bot if the setting is enabled
         if self.worker.bot.settings.oobabooga_settings.get("plugin_auto_start"):
             self.worker.start()
```

### Comparing `oobabot_plugin-0.2.0/src/oobabot_plugin/input_handlers.py` & `oobabot_plugin-0.2.1/src/oobabot_plugin/input_handlers.py`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.2.0/src/oobabot_plugin/install.py` & `oobabot_plugin-0.2.1/src/oobabot_plugin/install.py`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.2.0/src/oobabot_plugin/instructions.md` & `oobabot_plugin-0.2.1/src/oobabot_plugin/instructions.md`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.2.0/src/oobabot_plugin/layout.py` & `oobabot_plugin-0.2.1/src/oobabot_plugin/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,23 +79,25 @@
         self.transcript_html: typing.Optional[gr.HTML]
 
         #############################################
         # Runtime section
         #############################################
 
         # runtime widgets
+        self.status_html: gr.HTML
         self.start_button: gr.Button
         self.plugin_auto_start_checkbox: gr.Checkbox
         self.stop_button: gr.Button
+        self.log_etag_textbox: gr.Textbox
         self.log_output_html: gr.HTML
         self.running_state_textbox: gr.Textbox
 
     def layout_ui(
         self,
-        get_logs: typing.Callable[[], str],
+        get_log_etag: typing.Callable[[], int],
         has_plausible_token: bool,
         stable_diffusion_keywords: typing.List[str],
         api_extension_loaded: bool,
         is_using_character: bool,
         get_transcript_html: typing.Callable[[], str],
         is_voice_enabled: bool,
     ) -> None:
@@ -122,15 +124,15 @@
                         self._init_config_ui(
                             has_plausible_token,
                             stable_diffusion_keywords,
                             is_using_character,
                         )
                     with gr.Column(scale=2):
                         self._init_runtime_ui(
-                            get_logs,
+                            get_log_etag,
                             api_extension_loaded,
                         )
 
             with self.tab_advanced:
                 self._init_advanced_ui()
 
             if self.tab_audio is None:
@@ -378,47 +380,57 @@
 
     #############################################
     # Runtime tab
     #############################################
 
     def _init_runtime_ui(
         self,
-        get_logs: typing.Callable[[], str],
+        get_log_etag: typing.Callable[[], int],
         api_extension_loaded: bool,
     ) -> None:
         with gr.Row():
             self.start_button = gr.Button(
                 value="Start Oobabot",
                 interactive=False,
             )
             self.plugin_auto_start_checkbox = gr.Checkbox(
-                label="Start automatically when Oobabooga starts",
+                label="Start automatically",
                 value=False,
                 interactive=True,
                 elem_id="oobabot-plugin-auto-start",
             )
             self.stop_button = gr.Button(
                 value="Stop Oobabot",
                 interactive=False,
             )
             self.running_state_textbox = gr.Textbox(
                 "",
                 interactive=False,
                 visible=False,
                 elem_id="oobabot-is-running",
             )
-            # visible=False,  TODO: HIDE
 
-        gr.Markdown("### Oobabot Status", elem_id="oobabot-status-heading")
+        self.status_html = gr.HTML(
+            strings.status_heading(""),
+            elem_id="oobabot-status-heading",
+        )
         if not api_extension_loaded:
             gr.Markdown(
                 "**Warning**: The API extension is not loaded.  "
                 + "`Oobabot` will not work unless it is enabled.",
                 elem_id="oobabot-api-not-loaded",
             )
         with gr.Row():
+            # this value changes every time the log is updated
+            # it is used to trigger a full HTML update
+            self.log_etag_textbox = gr.Textbox(
+                value=get_log_etag,
+                every=strings.QUICK_UPDATE_INTERVAL_SECONDS,
+                interactive=False,
+                visible=False,
+                elem_id="oobabot-log-etag",
+            )
             self.log_output_html = gr.HTML(
+                value="",
                 label="Oobabot Log",
-                value=get_logs,
-                every=strings.QUICK_UPDATE_INTERVAL_SECONDS,
                 elem_classes=["oobabot-output"],
             )
```

### Comparing `oobabot_plugin-0.2.0/src/oobabot_plugin/script.py` & `oobabot_plugin-0.2.1/src/oobabot_plugin/script.py`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.2.0/src/oobabot_plugin/server.py` & `oobabot_plugin-0.2.1/src/oobabot_plugin/server.py`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.2.0/src/oobabot_plugin/strings.py` & `oobabot_plugin-0.2.1/src/oobabot_plugin/strings.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,267 +12,411 @@
 000000b0: 7274 2069 6d70 6f72 746c 6962 0a69 6d70  rt importlib.imp
 000000c0: 6f72 7420 6c6f 6767 696e 670a 696d 706f  ort logging.impo
 000000d0: 7274 206f 730a 696d 706f 7274 2070 6174  rt os.import pat
 000000e0: 686c 6962 0a69 6d70 6f72 7420 7379 730a  hlib.import sys.
 000000f0: 696d 706f 7274 2074 7970 6573 0a69 6d70  import types.imp
 00000100: 6f72 7420 7479 7069 6e67 0a0a 696d 706f  ort typing..impo
 00000110: 7274 206f 6f62 6162 6f74 2e66 616e 6379  rt oobabot.fancy
-00000120: 5f6c 6f67 6765 720a 0a54 4f4b 454e 5f4c  _logger..TOKEN_L
-00000130: 454e 5f43 4841 5253 203d 2037 320a 0a51  EN_CHARS = 72..Q
-00000140: 5549 434b 5f55 5044 4154 455f 494e 5445  UICK_UPDATE_INTE
-00000150: 5256 414c 5f53 4543 4f4e 4453 3a20 666c  RVAL_SECONDS: fl
-00000160: 6f61 7420 3d20 302e 350a 0a0a 6465 6620  oat = 0.5...def 
-00000170: 7265 736f 7572 6365 286e 616d 653a 2073  resource(name: s
-00000180: 7472 2920 2d3e 2073 7472 3a0a 2020 2020  tr) -> str:.    
-00000190: 2320 7265 7475 726e 2069 6d70 6f72 746c  # return importl
-000001a0: 6962 2e72 6573 6f75 7263 6573 2e72 6561  ib.resources.rea
-000001b0: 645f 7465 7874 2822 6f6f 6261 626f 745f  d_text("oobabot_
-000001c0: 706c 7567 696e 222c 206e 616d 6529 0a20  plugin", name). 
-000001d0: 2020 2072 6574 7572 6e20 7061 7468 6c69     return pathli
-000001e0: 622e 5061 7468 286f 732e 7061 7468 2e6a  b.Path(os.path.j
-000001f0: 6f69 6e28 6f73 2e70 6174 682e 6469 726e  oin(os.path.dirn
-00000200: 616d 6528 5f5f 6669 6c65 5f5f 292c 206e  ame(__file__), n
-00000210: 616d 6529 292e 7265 6164 5f74 6578 7428  ame)).read_text(
-00000220: 0a20 2020 2020 2020 2065 6e63 6f64 696e  .        encodin
-00000230: 673d 2275 7466 2d38 220a 2020 2020 290a  g="utf-8".    ).
-00000240: 0a0a 6465 6620 6765 745f 696e 7374 7275  ..def get_instru
-00000250: 6374 696f 6e73 5f6d 6172 6b64 6f77 6e28  ctions_markdown(
-00000260: 2920 2d3e 2074 7970 696e 672e 5475 706c  ) -> typing.Tupl
-00000270: 655b 7374 722c 2073 7472 5d3a 0a20 2020  e[str, str]:.   
-00000280: 2022 2222 0a20 2020 2052 6574 7572 6e73   """.    Returns
-00000290: 206d 6172 6b64 6f77 6e20 696e 2074 776f   markdown in two
-000002a0: 2070 6172 7473 2c20 6265 666f 7265 2061   parts, before a
-000002b0: 6e64 2061 6674 6572 2074 6865 0a20 2020  nd after the.   
-000002c0: 2074 6f6b 656e 2069 6e70 7574 2062 6f78   token input box
-000002d0: 2e0a 2020 2020 2222 220a 2020 2020 6d64  ..    """.    md
-000002e0: 5f74 6578 7420 3d20 7265 736f 7572 6365  _text = resource
-000002f0: 2822 696e 7374 7275 6374 696f 6e73 2e6d  ("instructions.m
-00000300: 6422 290a 2020 2020 7265 7475 726e 2074  d").    return t
-00000310: 7570 6c65 286d 645f 7465 7874 2e73 706c  uple(md_text.spl
-00000320: 6974 2822 7b7b 544f 4b45 4e5f 494e 5055  it("{{TOKEN_INPU
-00000330: 545f 424f 587d 7d22 2c20 3129 290a 0a0a  T_BOX}}", 1))...
-00000340: 6465 6620 6765 745f 7472 616e 7363 7269  def get_transcri
-00000350: 7074 5f6d 6172 6b64 6f77 6e28 2920 2d3e  pt_markdown() ->
-00000360: 2073 7472 3a0a 2020 2020 7265 7475 726e   str:.    return
-00000370: 2072 6573 6f75 7263 6528 2274 7261 6e73   resource("trans
-00000380: 6372 6970 742e 6d64 2229 0a0a 0a64 6566  cript.md")...def
-00000390: 2067 6574 5f63 7373 2829 202d 3e20 7374   get_css() -> st
-000003a0: 723a 0a20 2020 2072 6574 7572 6e20 7265  r:.    return re
-000003b0: 736f 7572 6365 2822 6f6f 6261 626f 745f  source("oobabot_
-000003c0: 6c6f 672e 6373 7322 290a 0a0a 6465 6620  log.css")...def 
-000003d0: 6765 745f 6a73 2829 202d 3e20 7374 723a  get_js() -> str:
-000003e0: 0a20 2020 2072 6574 7572 6e20 7265 736f  .    return reso
-000003f0: 7572 6365 2822 6f6f 6261 626f 745f 6c6f  urce("oobabot_lo
-00000400: 672e 6a73 2229 0a0a 0a64 6566 2074 6f6b  g.js")...def tok
-00000410: 656e 5f69 735f 706c 6175 7369 626c 6528  en_is_plausible(
-00000420: 746f 6b65 6e3a 2073 7472 2920 2d3e 2062  token: str) -> b
-00000430: 6f6f 6c3a 0a20 2020 2072 6574 7572 6e20  ool:.    return 
-00000440: 6c65 6e28 746f 6b65 6e2e 7374 7269 7028  len(token.strip(
-00000450: 2929 203e 3d20 544f 4b45 4e5f 4c45 4e5f  )) >= TOKEN_LEN_
-00000460: 4348 4152 530a 0a0a 6465 6620 666f 726d  CHARS...def form
-00000470: 6174 5f73 6176 655f 7265 7375 6c74 2879  at_save_result(y
-00000480: 616d 6c5f 6572 726f 723a 2074 7970 696e  aml_error: typin
-00000490: 672e 4f70 7469 6f6e 616c 5b73 7472 5d29  g.Optional[str])
-000004a0: 202d 3e20 7374 723a 0a20 2020 2069 6620   -> str:.    if 
-000004b0: 7961 6d6c 5f65 7272 6f72 3a0a 2020 2020  yaml_error:.    
-000004c0: 2020 2020 7265 7475 726e 2022 e29d 8c20      return "... 
-000004d0: 2a2a 4572 726f 722a 2a3a 2022 202b 2079  **Error**: " + y
-000004e0: 616d 6c5f 6572 726f 720a 2020 2020 7265  aml_error.    re
-000004f0: 7475 726e 2022 e29c 94ef b88f 202a 2a53  turn "...... **S
-00000500: 6176 6564 2a2a 220a 0a0a 6465 6620 6d61  aved**"...def ma
-00000510: 6b65 5f6c 696e 6b5f 6672 6f6d 5f74 6f6b  ke_link_from_tok
-00000520: 656e 280a 2020 2020 746f 6b65 6e3a 2073  en(.    token: s
-00000530: 7472 2c0a 2020 2020 666e 5f63 616c 635f  tr,.    fn_calc_
-00000540: 696e 7669 7465 5f75 726c 3a20 7479 7069  invite_url: typi
-00000550: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
-00000560: 6e67 2e43 616c 6c61 626c 655b 5b73 7472  ng.Callable[[str
-00000570: 5d2c 2073 7472 5d5d 2c0a 2920 2d3e 2073  ], str]],.) -> s
-00000580: 7472 3a0a 2020 2020 6966 206e 6f74 2074  tr:.    if not t
-00000590: 6f6b 656e 206f 7220 6e6f 7420 666e 5f63  oken or not fn_c
-000005a0: 616c 635f 696e 7669 7465 5f75 726c 3a0a  alc_invite_url:.
-000005b0: 2020 2020 2020 2020 7265 7475 726e 2022          return "
-000005c0: 4120 6c69 6e6b 2077 696c 6c20 6170 7065  A link will appe
-000005d0: 6172 2068 6572 6520 6f6e 6365 2079 6f75  ar here once you
-000005e0: 2068 6176 6520 7365 7420 796f 7572 2044   have set your D
-000005f0: 6973 636f 7264 2074 6f6b 656e 2e22 0a20  iscord token.". 
-00000600: 2020 206c 696e 6b20 3d20 666e 5f63 616c     link = fn_cal
-00000610: 635f 696e 7669 7465 5f75 726c 2874 6f6b  c_invite_url(tok
-00000620: 656e 290a 2020 2020 7265 7475 726e 2028  en).    return (
-00000630: 0a20 2020 2020 2020 2066 273c 6120 6872  .        f'<a hr
-00000640: 6566 3d22 7b6c 696e 6b7d 2220 6964 3d22  ef="{link}" id="
-00000650: 6f6f 6261 626f 742d 696e 7669 7465 2d6c  oobabot-invite-l
-00000660: 696e 6b22 2074 6172 6765 743d 225f 626c  ink" target="_bl
-00000670: 616e 6b22 3e43 6c69 636b 2068 6572 6520  ank">Click here 
-00000680: 746f 203c 7072 653e 270a 2020 2020 2020  to <pre>'.      
-00000690: 2020 2b20 2269 6e76 6974 6520 796f 7572    + "invite your
-000006a0: 2062 6f74 3c2f 7072 653e 2074 6f20 6120   bot</pre> to a 
-000006b0: 4469 7363 6f72 6420 7365 7276 6572 3c2f  Discord server</
-000006c0: 613e 2e22 0a20 2020 2029 0a0a 0a64 6566  a>.".    )...def
-000006d0: 2075 7064 6174 655f 6469 7363 6f72 645f   update_discord_
-000006e0: 696e 7669 7465 5f6c 696e 6b28 0a20 2020  invite_link(.   
-000006f0: 206e 6577 5f74 6f6b 656e 3a20 7374 722c   new_token: str,
-00000700: 0a20 2020 2069 735f 746f 6b65 6e5f 7661  .    is_token_va
-00000710: 6c69 643a 2062 6f6f 6c2c 0a20 2020 2069  lid: bool,.    i
-00000720: 735f 7465 7374 6564 3a20 626f 6f6c 2c0a  s_tested: bool,.
-00000730: 2020 2020 666e 5f67 656e 6572 6174 655f      fn_generate_
-00000740: 696e 7669 7465 5f75 726c 3a20 7479 7069  invite_url: typi
-00000750: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
-00000760: 6e67 2e43 616c 6c61 626c 655b 5b73 7472  ng.Callable[[str
-00000770: 5d2c 2073 7472 5d5d 2c0a 293a 0a20 2020  ], str]],.):.   
-00000780: 206e 6577 5f74 6f6b 656e 203d 206e 6577   new_token = new
-00000790: 5f74 6f6b 656e 2e73 7472 6970 2829 0a20  _token.strip(). 
-000007a0: 2020 2070 7265 6669 7820 3d20 2222 0a20     prefix = "". 
-000007b0: 2020 2069 6620 6973 5f74 6573 7465 643a     if is_tested:
-000007c0: 0a20 2020 2020 2020 2069 6620 6973 5f74  .        if is_t
-000007d0: 6f6b 656e 5f76 616c 6964 3a0a 2020 2020  oken_valid:.    
-000007e0: 2020 2020 2020 2020 7072 6566 6978 203d          prefix =
-000007f0: 2022 e29c 94ef b88f 2059 6f75 7220 746f   "...... Your to
-00000800: 6b65 6e20 6973 2076 616c 6964 2e3c 6272  ken is valid.<br
-00000810: 3e3c 6272 3e22 0a20 2020 2020 2020 2065  ><br>".        e
-00000820: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00000830: 2070 7265 6669 7820 3d20 22e2 9d8c 2059   prefix = "... Y
-00000840: 6f75 7220 746f 6b65 6e20 6973 2069 6e76  our token is inv
-00000850: 616c 6964 2e22 0a20 2020 2069 6620 6973  alid.".    if is
-00000860: 5f74 6f6b 656e 5f76 616c 6964 3a0a 2020  _token_valid:.  
-00000870: 2020 2020 2020 7265 7475 726e 2070 7265        return pre
-00000880: 6669 7820 2b20 6d61 6b65 5f6c 696e 6b5f  fix + make_link_
-00000890: 6672 6f6d 5f74 6f6b 656e 280a 2020 2020  from_token(.    
-000008a0: 2020 2020 2020 2020 6e65 775f 746f 6b65          new_toke
-000008b0: 6e2c 0a20 2020 2020 2020 2020 2020 2066  n,.            f
-000008c0: 6e5f 6765 6e65 7261 7465 5f69 6e76 6974  n_generate_invit
-000008d0: 655f 7572 6c2c 0a20 2020 2020 2020 2029  e_url,.        )
-000008e0: 0a20 2020 2069 6620 6e65 775f 746f 6b65  .    if new_toke
-000008f0: 6e3a 0a20 2020 2020 2020 2072 6574 7572  n:.        retur
-00000900: 6e20 7072 6566 6978 0a20 2020 2072 6574  n prefix.    ret
-00000910: 7572 6e20 2241 206c 696e 6b20 7769 6c6c  urn "A link will
-00000920: 2061 7070 6561 7220 6865 7265 206f 6e63   appear here onc
-00000930: 6520 796f 7520 6861 7665 2073 6574 2079  e you have set y
-00000940: 6f75 7220 4469 7363 6f72 6420 746f 6b65  our Discord toke
-00000950: 6e2e 220a 0a0a 4348 4152 4143 5445 525f  n."...CHARACTER_
-00000960: 4e4f 4e45 203d 2022 4e6f 6e65 220a 0a0a  NONE = "None"...
-00000970: 6465 6620 6765 745f 6176 6169 6c61 626c  def get_availabl
-00000980: 655f 6368 6172 6163 7465 7273 2829 202d  e_characters() -
-00000990: 3e20 7479 7069 6e67 2e4c 6973 745b 7374  > typing.List[st
-000009a0: 725d 3a0a 2020 2020 2222 220a 2020 2020  r]:.    """.    
-000009b0: 5468 6973 2069 7320 6120 6c69 7374 206f  This is a list o
-000009c0: 6620 616c 6c20 6669 6c65 7320 696e 2074  f all files in t
-000009d0: 6865 202e 2f63 6861 7261 6374 6572 7320  he ./characters 
-000009e0: 666f 6c64 6572 2077 686f 7365 0a20 2020  folder whose.   
-000009f0: 2065 7874 656e 7369 6f6e 2069 7320 2e6a   extension is .j
-00000a00: 736f 6e2c 202e 7961 6d6c 2c20 6f72 202e  son, .yaml, or .
-00000a10: 796d 6c0a 0a20 2020 2054 6865 206c 6973  yml..    The lis
-00000a20: 7420 6973 2074 6865 6e20 736f 7274 6564  t is then sorted
-00000a30: 2061 6c70 6861 6265 7469 6361 6c6c 792c   alphabetically,
-00000a40: 2061 6e64 2027 4e6f 6e65 2720 6973 2061   and 'None' is a
-00000a50: 6464 6564 2074 6f0a 2020 2020 7468 6520  dded to.    the 
-00000a60: 7374 6172 742e 0a20 2020 2022 2222 0a20  start..    """. 
-00000a70: 2020 2063 6861 7261 6374 6572 7320 3d20     characters = 
-00000a80: 5b5d 0a20 2020 2066 6f72 2065 7874 656e  [].    for exten
-00000a90: 7369 6f6e 2069 6e20 5b22 796d 6c22 2c20  sion in ["yml", 
-00000aa0: 2279 616d 6c22 2c20 226a 736f 6e22 5d3a  "yaml", "json"]:
-00000ab0: 0a20 2020 2020 2020 2066 6f72 2066 696c  .        for fil
-00000ac0: 6570 6174 6820 696e 2070 6174 686c 6962  epath in pathlib
-00000ad0: 2e50 6174 6828 2263 6861 7261 6374 6572  .Path("character
-00000ae0: 7322 292e 676c 6f62 2866 222a 2e7b 6578  s").glob(f"*.{ex
-00000af0: 7465 6e73 696f 6e7d 2229 3a0a 2020 2020  tension}"):.    
-00000b00: 2020 2020 2020 2020 6368 6172 6163 7465          characte
-00000b10: 7273 2e61 7070 656e 6428 6669 6c65 7061  rs.append(filepa
-00000b20: 7468 2e73 7465 6d29 0a20 2020 2063 6861  th.stem).    cha
-00000b30: 7261 6374 6572 732e 736f 7274 2829 0a20  racters.sort(). 
-00000b40: 2020 2063 6861 7261 6374 6572 732e 696e     characters.in
-00000b50: 7365 7274 2830 2c20 4348 4152 4143 5445  sert(0, CHARACTE
-00000b60: 525f 4e4f 4e45 290a 2020 2020 7265 7475  R_NONE).    retu
-00000b70: 726e 2063 6861 7261 6374 6572 730a 0a0a  rn characters...
-00000b80: 6465 6620 7265 7061 6972 5f6c 6f67 6769  def repair_loggi
-00000b90: 6e67 2829 202d 3e20 7479 7069 6e67 2e4f  ng() -> typing.O
-00000ba0: 7074 696f 6e61 6c5b 6c6f 6767 696e 672e  ptional[logging.
-00000bb0: 4c6f 6767 6572 5d3a 0a20 2020 2023 2323  Logger]:.    ###
-00000bc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000bd0: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
-00000be0: 2020 2020 2320 736f 2c20 6c6f 6767 696e      # so, loggin
-00000bf0: 675f 636f 6c6f 7273 2e70 792c 2072 6174  g_colors.py, rat
-00000c00: 6865 7220 7468 616e 2075 7369 6e67 2074  her than using t
-00000c10: 6865 206c 6f67 6769 6e67 206d 6f64 756c  he logging modul
-00000c20: 6527 7320 6275 696c 742d 696e 0a20 2020  e's built-in.   
-00000c30: 2023 2066 6f72 6d61 7474 6572 2c20 6973   # formatter, is
-00000c40: 206d 6f6e 6b65 792d 7061 7463 6869 6e67   monkey-patching
-00000c50: 2074 6865 206c 6f67 6769 6e67 206d 6f64   the logging mod
-00000c60: 756c 6527 7320 5374 7265 616d 4861 6e64  ule's StreamHand
-00000c70: 6c65 722e 656d 6974 2e0a 2020 2020 2320  ler.emit..    # 
-00000c80: 5468 6973 2069 7320 6120 7072 6f62 6c65  This is a proble
-00000c90: 6d20 666f 7220 7573 2c20 6265 6361 7573  m for us, becaus
-00000ca0: 6520 7765 2061 6c73 6f20 7573 6520 7468  e we also use th
-00000cb0: 6520 6c6f 6767 696e 6720 6d6f 6475 6c65  e logging module
-00000cc0: 2c20 6275 740a 2020 2020 2320 646f 6e27  , but.    # don'
-00000cd0: 7420 7761 6e74 2041 4e53 4920 636f 6c6f  t want ANSI colo
-00000ce0: 7220 636f 6465 7320 7368 6f77 696e 6720  r codes showing 
-00000cf0: 7570 2069 6e20 4854 4d4c 2e20 2057 6520  up in HTML.  We 
-00000d00: 616c 736f 2064 6f6e 2774 2077 616e 740a  also don't want.
-00000d10: 2020 2020 2320 746f 2062 7265 616b 2074      # to break t
-00000d20: 6865 6972 206c 6f67 6769 6e67 2e0a 2020  heir logging..  
-00000d30: 2020 230a 2020 2020 2320 536f 2c20 7765    #.    # So, we
-00000d40: 2772 6520 676f 696e 6720 746f 2073 6176  're going to sav
-00000d50: 6520 7468 6569 7220 6d6f 6e6b 6579 2d70  e their monkey-p
-00000d60: 6174 6368 6564 2065 6d69 742c 2072 656c  atched emit, rel
-00000d70: 6f61 6420 7468 6520 6c6f 6767 696e 670a  oad the logging.
-00000d80: 2020 2020 2320 6d6f 6475 6c65 2c20 7361      # module, sa
-00000d90: 7665 206f 6666 2074 6865 2022 7265 616c  ve off the "real
-00000da0: 2220 656d 6974 2c20 7468 656e 2072 652d  " emit, then re-
-00000db0: 6170 706c 7920 7468 6569 7220 6d6f 6e6b  apply their monk
-00000dc0: 6579 2d70 6174 6368 2e0a 2020 2020 230a  ey-patch..    #.
-00000dd0: 2020 2020 2320 5765 206e 6565 6420 746f      # We need to
-00000de0: 2064 6f20 616c 6c20 7468 6973 2062 6566   do all this bef
-00000df0: 6f72 6520 7765 2063 7265 6174 6520 7468  ore we create th
-00000e00: 6520 6f6f 6261 626f 745f 776f 726b 6572  e oobabot_worker
-00000e10: 2c20 736f 2074 6861 740a 2020 2020 2320  , so that.    # 
-00000e20: 7468 6520 6c6f 6773 2063 7265 6174 6564  the logs created
-00000e30: 2064 7572 696e 6720 7374 6172 7475 7020   during startup 
-00000e40: 6172 6520 7072 6f70 6572 6c79 2066 6f72  are properly for
-00000e50: 6d61 7474 6564 2e0a 0a20 2020 2023 2073  matted...    # s
-00000e60: 6176 6520 7468 6520 6d6f 6e6b 6579 2d70  ave the monkey-p
-00000e70: 6174 6368 6564 2065 6d69 740a 2020 2020  atched emit.    
-00000e80: 6861 636b 6564 5f65 6d69 7420 3d20 6c6f  hacked_emit = lo
-00000e90: 6767 696e 672e 5374 7265 616d 4861 6e64  gging.StreamHand
-00000ea0: 6c65 722e 656d 6974 0a0a 2020 2020 2320  ler.emit..    # 
-00000eb0: 7265 6c6f 6164 2074 6865 206c 6f67 6769  reload the loggi
-00000ec0: 6e67 206d 6f64 756c 650a 2020 2020 7472  ng module.    tr
-00000ed0: 793a 0a20 2020 2020 2020 2069 6d70 6f72  y:.        impor
-00000ee0: 746c 6962 2e72 656c 6f61 6428 6c6f 6767  tlib.reload(logg
-00000ef0: 696e 6729 0a20 2020 2065 7863 6570 7420  ing).    except 
-00000f00: 496d 706f 7274 4572 726f 7220 6173 2065  ImportError as e
-00000f10: 7272 3a0a 2020 2020 2020 2020 7072 696e  rr:.        prin
-00000f20: 7428 6622 4f6f 6261 626f 743a 2045 7272  t(f"Oobabot: Err
-00000f30: 6f72 2072 656c 6f61 6469 6e67 206c 6f67  or reloading log
-00000f40: 6769 6e67 206d 6f64 756c 653a 207b 6572  ging module: {er
-00000f50: 727d 222c 2066 696c 653d 7379 732e 7374  r}", file=sys.st
-00000f60: 6465 7272 290a 2020 2020 2020 2020 7265  derr).        re
-00000f70: 7475 726e 204e 6f6e 650a 0a20 2020 2023  turn None..    #
-00000f80: 2063 7265 6174 6520 6f75 7220 6c6f 6767   create our logg
-00000f90: 6572 2065 6172 6c79 0a20 2020 206f 6f62  er early.    oob
-00000fa0: 6162 6f74 2e66 616e 6379 5f6c 6f67 6765  abot.fancy_logge
-00000fb0: 722e 696e 6974 5f6c 6f67 6769 6e67 286c  r.init_logging(l
-00000fc0: 6f67 6769 6e67 2e44 4542 5547 2c20 5472  ogging.DEBUG, Tr
-00000fd0: 7565 290a 2020 2020 6f6f 6261 5f6c 6f67  ue).    ooba_log
-00000fe0: 6765 7220 3d20 6f6f 6261 626f 742e 6661  ger = oobabot.fa
-00000ff0: 6e63 795f 6c6f 6767 6572 2e67 6574 2829  ncy_logger.get()
-00001000: 0a0a 2020 2020 2320 6d61 6e75 616c 6c79  ..    # manually
-00001010: 2061 7070 6c79 2074 6865 2022 636f 7272   apply the "corr
-00001020: 6563 7422 2065 6d69 7420 746f 2065 6163  ect" emit to eac
-00001030: 6820 6f66 2074 6865 2053 7472 6561 6d48  h of the StreamH
-00001040: 616e 646c 6572 730a 2020 2020 2320 7468  andlers.    # th
-00001050: 6174 2066 616e 6379 5f6c 6f67 6765 7220  at fancy_logger 
-00001060: 6372 6561 7465 640a 2020 2020 666f 7220  created.    for 
-00001070: 6861 6e64 6c65 7220 696e 206f 6f62 615f  handler in ooba_
-00001080: 6c6f 6767 6572 2e68 616e 646c 6572 733a  logger.handlers:
-00001090: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-000010a0: 7374 616e 6365 2868 616e 646c 6572 2c20  stance(handler, 
-000010b0: 6c6f 6767 696e 672e 5374 7265 616d 4861  logging.StreamHa
-000010c0: 6e64 6c65 7229 3a0a 2020 2020 2020 2020  ndler):.        
-000010d0: 2020 2020 6861 6e64 6c65 722e 656d 6974      handler.emit
-000010e0: 203d 2074 7970 6573 2e4d 6574 686f 6454   = types.MethodT
-000010f0: 7970 6528 6c6f 6767 696e 672e 5374 7265  ype(logging.Stre
-00001100: 616d 4861 6e64 6c65 722e 656d 6974 2c20  amHandler.emit, 
-00001110: 6861 6e64 6c65 7229 0a0a 2020 2020 6c6f  handler)..    lo
-00001120: 6767 696e 672e 5374 7265 616d 4861 6e64  gging.StreamHand
-00001130: 6c65 722e 656d 6974 203d 2068 6163 6b65  ler.emit = hacke
-00001140: 645f 656d 6974 0a20 2020 2072 6574 7572  d_emit.    retur
-00001150: 6e20 6f6f 6261 5f6c 6f67 6765 720a       n ooba_logger.
+00000120: 5f6c 6f67 6765 720a 0a23 2074 6865 2064  _logger..# the d
+00000130: 6973 636f 7264 2074 6f6b 656e 2068 6173  iscord token has
+00000140: 2074 6869 7320 666f 726d 6174 3a0a 2320   this format:.# 
+00000150: 4141 4141 4141 4141 4141 4141 4141 4141  AAAAAAAAAAAAAAAA
+00000160: 4141 4141 4141 4141 4141 2e42 4242 4242  AAAAAAAAAA.BBBBB
+00000170: 422e 4343 4343 4343 4343 4343 4343 4343  B.CCCCCCCCCCCCCC
+00000180: 4343 4343 4343 4343 4343 4343 4343 4343  CCCCCCCCCCCCCCCC
+00000190: 4343 4343 4343 4343 0a23 0a23 2077 6865  CCCCCCCC.#.# whe
+000001a0: 7265 2065 6163 6820 7365 6374 696f 6e2c  re each section,
+000001b0: 2041 2c20 422c 2061 6e64 2043 2c20 6973   A, B, and C, is
+000001c0: 2069 6e64 6570 656e 6465 6e74 6c79 2061   independently a
+000001d0: 2062 6173 6536 342d 656e 636f 6465 6420   base64-encoded 
+000001e0: 7374 7269 6e67 2e0a 230a 2320 5365 6374  string..#.# Sect
+000001f0: 696f 6e20 4120 656e 636f 6465 7320 7468  ion A encodes th
+00000200: 6520 436c 6965 6e74 2049 442e 0a23 0a23  e Client ID..#.#
+00000210: 2054 6865 2063 6c69 656e 7420 4944 2069   The client ID i
+00000220: 7320 6120 2273 6e6f 7766 6c61 6b65 222c  s a "snowflake",
+00000230: 2077 6869 6368 2069 7320 696e 6865 7265   which is inhere
+00000240: 6e74 6c79 2061 2036 342d 6269 7420 696e  ntly a 64-bit in
+00000250: 7465 6765 7220 7661 6c75 652e 0a23 2042  teger value..# B
+00000260: 6566 6f72 6520 6265 696e 6720 7374 6f72  efore being stor
+00000270: 6564 2c20 7468 6973 2076 616c 7565 2069  ed, this value i
+00000280: 7320 636f 6e76 6572 7465 6420 746f 2061  s converted to a
+00000290: 2064 6563 696d 616c 2073 7472 696e 6720   decimal string 
+000002a0: 7265 7072 6573 656e 7461 7469 6f6e 2c0a  representation,.
+000002b0: 2320 7468 656e 2074 6861 7420 7374 7269  # then that stri
+000002c0: 6e67 2069 7320 656e 636f 6465 6420 7769  ng is encoded wi
+000002d0: 7468 2062 6173 6536 342e 0a23 0a23 2020  th base64..#.#  
+000002e0: 2049 7473 2073 7472 7563 7475 7265 3a0a   Its structure:.
+000002f0: 230a 2320 2062 6974 7320 2020 2020 2020  #.#  bits       
+00000300: 2020 2020 2028 3432 2920 2020 2020 2020       (42)       
+00000310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000320: 2028 3529 2020 2028 3529 2020 2020 2028   (5)   (5)     (
+00000330: 3132 290a 2320 2064 6464 6464 6464 6464  12).#  ddddddddd
+00000340: 6464 6464 6464 6464 6464 6464 6464 6464  dddddddddddddddd
+00000350: 6464 6464 6464 6464 6464 6464 6464 6464  dddddddddddddddd
+00000360: 2063 6363 6363 2062 6262 6262 2061 6161   ccccc bbbbb aaa
+00000370: 6161 6161 6161 6161 6161 0a23 2020 2020  aaaaaaaaaa.#    
+00000380: 2020 2020 2020 3130 3031 3031 3130 3031        1001011001
+00000390: 3030 3131 3131 3131 3130 3030 3030 3030  0011111110000000
+000003a0: 3031 3030 3130 3120 3030 3030 3020 3030  0100101 00000 00
+000003b0: 3030 3020 3030 3030 3030 3030 3030 3030  000 000000000000
+000003c0: 0a23 2077 6865 7265 3a0a 2320 2020 6420  .# where:.#   d 
+000003d0: 2d20 6e75 6d62 6572 206f 6620 6d69 6c6c  - number of mill
+000003e0: 6973 6563 6f6e 6473 2073 696e 6365 2074  iseconds since t
+000003f0: 6865 2044 6973 636f 7264 2065 706f 6368  he Discord epoch
+00000400: 2028 3230 3135 2d30 312d 3031 5430 303a   (2015-01-01T00:
+00000410: 3030 3a30 302e 3030 305a 290a 2320 2020  00:00.000Z).#   
+00000420: 6320 2d20 636c 6965 6e74 2049 440a 2320  c - client ID.# 
+00000430: 2020 6220 2d20 7072 6f63 6573 7320 4944    b - process ID
+00000440: 0a23 2020 2061 202d 2069 6e63 7265 6d65  .#   a - increme
+00000450: 6e74 696e 6720 636f 756e 7465 7220 2870  nting counter (p
+00000460: 6572 2070 726f 6365 7373 290a 230a 2320  er process).#.# 
+00000470: 4469 7363 6f72 6420 7761 7320 6f6e 6c79  Discord was only
+00000480: 2063 7265 6174 6564 2069 6e20 4d61 7920   created in May 
+00000490: 3230 3135 2c20 616e 6420 7468 6520 6c6f  2015, and the lo
+000004a0: 7765 7374 206b 6e6f 776e 2073 6e6f 7766  west known snowf
+000004b0: 6c61 6b65 2028 6265 6c6f 6e67 696e 670a  lake (belonging.
+000004c0: 2320 746f 2074 6865 2044 6973 636f 7264  # to the Discord
+000004d0: 2043 544f 2920 6973 2027 3231 3135 3435   CTO) is '211545
+000004e0: 3335 3135 3431 3232 3735 3227 2c20 6974  35154122752', it
+000004f0: 2068 6176 696e 6720 6265 656e 2067 656e   having been gen
+00000500: 6572 6174 6564 206f 6e20 4672 6964 6179  erated on Friday
+00000510: 0a23 2046 6562 7275 6172 7920 3237 2c20  .# February 27, 
+00000520: 3230 3135 2061 7420 3039 3a31 333a 3431  2015 at 09:13:41
+00000530: 2e31 3132 2055 5443 2e0a 230a 2320 5768  .112 UTC..#.# Wh
+00000540: 656e 2070 7574 2069 6e74 6f20 616e 2065  en put into an e
+00000550: 6e74 6972 6520 736e 6f77 666c 616b 652c  ntire snowflake,
+00000560: 2074 6869 7320 6861 7320 616e 2065 6e63   this has an enc
+00000570: 6f64 6564 206c 656e 6774 6820 6f66 2032  oded length of 2
+00000580: 3420 6368 6172 6163 7465 7273 2e0a 230a  4 characters..#.
+00000590: 2320 5468 6520 7665 7279 206c 6173 7420  # The very last 
+000005a0: 746f 6b65 6e20 6576 6572 2c20 6765 6e65  token ever, gene
+000005b0: 7261 7465 6420 736f 6d65 7469 6d65 2069  rated sometime i
+000005c0: 6e20 7468 6520 5554 4320 6166 7465 726e  n the UTC aftern
+000005d0: 6f6f 6e20 6f66 204d 6179 2031 332c 2032  oon of May 13, 2
+000005e0: 3135 342c 0a23 2063 6f75 6c64 2068 6176  154,.# could hav
+000005f0: 6520 616e 2065 6e63 6f64 6564 206c 656e  e an encoded len
+00000600: 6774 6820 6f66 2032 3820 6368 6172 6163  gth of 28 charac
+00000610: 7465 7273 2e0a 230a 2320 4475 6520 746f  ters..#.# Due to
+00000620: 2074 6865 2077 6179 2074 6861 7420 6261   the way that ba
+00000630: 7365 3634 2065 6e63 6f64 696e 6720 776f  se64 encoding wo
+00000640: 726b 732c 2074 6865 206c 656e 6774 6820  rks, the length 
+00000650: 6f66 2074 6865 2065 6e63 6f64 6564 2073  of the encoded s
+00000660: 7472 696e 6720 776f 756c 640a 2320 6e6f  tring would.# no
+00000670: 726d 616c 6c79 2061 6c77 6179 7320 6265  rmally always be
+00000680: 2061 206d 756c 7469 706c 6520 6f66 2034   a multiple of 4
+00000690: 2e20 2048 6f77 6576 6572 2c20 6166 7465  .  However, afte
+000006a0: 7220 7468 6520 656e 636f 6469 6e67 2069  r the encoding i
+000006b0: 7320 646f 6e65 2c20 4469 7363 6f72 640a  s done, Discord.
+000006c0: 2320 6472 6f70 7320 7468 6520 7472 6169  # drops the trai
+000006d0: 6c69 6e67 2027 3d27 2063 6861 7261 6374  ling '=' charact
+000006e0: 6572 732c 2077 6869 6368 206d 6561 6e73  ers, which means
+000006f0: 2074 6861 7420 7468 6520 6c65 6e67 7468   that the length
+00000700: 206f 6620 7468 6520 656e 636f 6465 640a   of the encoded.
+00000710: 2320 7374 7269 6e67 2069 7320 6e6f 7420  # string is not 
+00000720: 616c 7761 7973 2061 206d 756c 7469 706c  always a multipl
+00000730: 6520 6f66 2034 2e0a 230a 2320 536f 2c20  e of 4..#.# So, 
+00000740: 7661 6c69 6420 6c65 6e67 7468 7320 666f  valid lengths fo
+00000750: 7220 7365 6374 696f 6e20 4120 6172 653a  r section A are:
+00000760: 2032 342c 2032 352c 2032 362c 2032 372c   24, 25, 26, 27,
+00000770: 2061 6e64 2032 382e 0a23 0a23 2041 6464   and 28..#.# Add
+00000780: 696e 6720 696e 2074 6865 206f 7468 6572  ing in the other
+00000790: 2034 3620 6368 6172 6163 7465 7273 2028   46 characters (
+000007a0: 6672 6f6d 2074 6865 2074 776f 2070 6572  from the two per
+000007b0: 696f 6420 7365 7061 7261 746f 7273 2c20  iod separators, 
+000007c0: 6669 7865 642d 6c65 6e67 7468 0a23 2073  fixed-length.# s
+000007d0: 6563 7469 6f6e 7320 4220 616e 6420 4320  ections B and C 
+000007e0: 6f66 2036 2061 6e64 2033 3820 6368 6172  of 6 and 38 char
+000007f0: 6163 7465 7273 2c20 7265 7370 6563 7469  acters, respecti
+00000800: 7665 6c79 292c 2077 6520 6765 7420 7468  vely), we get th
+00000810: 6520 7661 6c69 6420 6c65 6e67 7468 730a  e valid lengths.
+00000820: 2320 666f 7220 7468 6520 656e 7469 7265  # for the entire
+00000830: 2074 6f6b 656e 3a0a 2320 2020 3730 2c20   token:.#   70, 
+00000840: 3731 2c20 3732 2c20 3733 2c20 3734 0a23  71, 72, 73, 74.#
+00000850: 0a54 4f4b 454e 5f4c 454e 5f56 414c 4944  .TOKEN_LEN_VALID
+00000860: 5f52 414e 4745 203d 2072 616e 6765 2837  _RANGE = range(7
+00000870: 302c 2037 3420 2b20 3129 0a0a 5155 4943  0, 74 + 1)..QUIC
+00000880: 4b5f 5550 4441 5445 5f49 4e54 4552 5641  K_UPDATE_INTERVA
+00000890: 4c5f 5345 434f 4e44 533a 2066 6c6f 6174  L_SECONDS: float
+000008a0: 203d 2030 2e35 0a0a 0a64 6566 2072 6573   = 0.5...def res
+000008b0: 6f75 7263 6528 6e61 6d65 3a20 7374 7229  ource(name: str)
+000008c0: 202d 3e20 7374 723a 0a20 2020 2023 2072   -> str:.    # r
+000008d0: 6574 7572 6e20 696d 706f 7274 6c69 622e  eturn importlib.
+000008e0: 7265 736f 7572 6365 732e 7265 6164 5f74  resources.read_t
+000008f0: 6578 7428 226f 6f62 6162 6f74 5f70 6c75  ext("oobabot_plu
+00000900: 6769 6e22 2c20 6e61 6d65 290a 2020 2020  gin", name).    
+00000910: 7265 7475 726e 2070 6174 686c 6962 2e50  return pathlib.P
+00000920: 6174 6828 6f73 2e70 6174 682e 6a6f 696e  ath(os.path.join
+00000930: 286f 732e 7061 7468 2e64 6972 6e61 6d65  (os.path.dirname
+00000940: 285f 5f66 696c 655f 5f29 2c20 6e61 6d65  (__file__), name
+00000950: 2929 2e72 6561 645f 7465 7874 280a 2020  )).read_text(.  
+00000960: 2020 2020 2020 656e 636f 6469 6e67 3d22        encoding="
+00000970: 7574 662d 3822 0a20 2020 2029 0a0a 0a64  utf-8".    )...d
+00000980: 6566 2067 6574 5f69 6e73 7472 7563 7469  ef get_instructi
+00000990: 6f6e 735f 6d61 726b 646f 776e 2829 202d  ons_markdown() -
+000009a0: 3e20 7479 7069 6e67 2e54 7570 6c65 5b73  > typing.Tuple[s
+000009b0: 7472 2c20 7374 725d 3a0a 2020 2020 2222  tr, str]:.    ""
+000009c0: 220a 2020 2020 5265 7475 726e 7320 6d61  ".    Returns ma
+000009d0: 726b 646f 776e 2069 6e20 7477 6f20 7061  rkdown in two pa
+000009e0: 7274 732c 2062 6566 6f72 6520 616e 6420  rts, before and 
+000009f0: 6166 7465 7220 7468 650a 2020 2020 746f  after the.    to
+00000a00: 6b65 6e20 696e 7075 7420 626f 782e 0a20  ken input box.. 
+00000a10: 2020 2022 2222 0a20 2020 206d 645f 7465     """.    md_te
+00000a20: 7874 203d 2072 6573 6f75 7263 6528 2269  xt = resource("i
+00000a30: 6e73 7472 7563 7469 6f6e 732e 6d64 2229  nstructions.md")
+00000a40: 0a20 2020 2072 6574 7572 6e20 7475 706c  .    return tupl
+00000a50: 6528 6d64 5f74 6578 742e 7370 6c69 7428  e(md_text.split(
+00000a60: 227b 7b54 4f4b 454e 5f49 4e50 5554 5f42  "{{TOKEN_INPUT_B
+00000a70: 4f58 7d7d 222c 2031 2929 0a0a 0a64 6566  OX}}", 1))...def
+00000a80: 2067 6574 5f74 7261 6e73 6372 6970 745f   get_transcript_
+00000a90: 6d61 726b 646f 776e 2829 202d 3e20 7374  markdown() -> st
+00000aa0: 723a 0a20 2020 2072 6574 7572 6e20 7265  r:.    return re
+00000ab0: 736f 7572 6365 2822 7472 616e 7363 7269  source("transcri
+00000ac0: 7074 2e6d 6422 290a 0a0a 6465 6620 6765  pt.md")...def ge
+00000ad0: 745f 6373 7328 2920 2d3e 2073 7472 3a0a  t_css() -> str:.
+00000ae0: 2020 2020 7265 7475 726e 2072 6573 6f75      return resou
+00000af0: 7263 6528 226f 6f62 6162 6f74 5f6c 6f67  rce("oobabot_log
+00000b00: 2e63 7373 2229 0a0a 0a64 6566 2067 6574  .css")...def get
+00000b10: 5f6a 7328 2920 2d3e 2073 7472 3a0a 2020  _js() -> str:.  
+00000b20: 2020 7265 7475 726e 2072 6573 6f75 7263    return resourc
+00000b30: 6528 226f 6f62 6162 6f74 5f6c 6f67 2e6a  e("oobabot_log.j
+00000b40: 7322 290a 0a0a 6465 6620 746f 6b65 6e5f  s")...def token_
+00000b50: 6973 5f70 6c61 7573 6962 6c65 2874 6f6b  is_plausible(tok
+00000b60: 656e 3a20 7374 7229 202d 3e20 626f 6f6c  en: str) -> bool
+00000b70: 3a0a 2020 2020 7265 7475 726e 206c 656e  :.    return len
+00000b80: 2874 6f6b 656e 2e73 7472 6970 2829 2920  (token.strip()) 
+00000b90: 696e 2054 4f4b 454e 5f4c 454e 5f56 414c  in TOKEN_LEN_VAL
+00000ba0: 4944 5f52 414e 4745 0a0a 0a64 6566 2066  ID_RANGE...def f
+00000bb0: 6f72 6d61 745f 7361 7665 5f72 6573 756c  ormat_save_resul
+00000bc0: 7428 7961 6d6c 5f65 7272 6f72 3a20 7479  t(yaml_error: ty
+00000bd0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
+00000be0: 725d 2920 2d3e 2073 7472 3a0a 2020 2020  r]) -> str:.    
+00000bf0: 6966 2079 616d 6c5f 6572 726f 723a 0a20  if yaml_error:. 
+00000c00: 2020 2020 2020 2072 6574 7572 6e20 22e2         return ".
+00000c10: 9d8c 202a 2a45 7272 6f72 2a2a 3a20 2220  .. **Error**: " 
+00000c20: 2b20 7961 6d6c 5f65 7272 6f72 0a20 2020  + yaml_error.   
+00000c30: 2072 6574 7572 6e20 22e2 9c94 efb8 8f20   return "...... 
+00000c40: 2a2a 5361 7665 642a 2a22 0a0a 0a64 6566  **Saved**"...def
+00000c50: 206d 616b 655f 6c69 6e6b 5f66 726f 6d5f   make_link_from_
+00000c60: 746f 6b65 6e28 0a20 2020 2074 6f6b 656e  token(.    token
+00000c70: 3a20 7374 722c 0a20 2020 2066 6e5f 6361  : str,.    fn_ca
+00000c80: 6c63 5f69 6e76 6974 655f 7572 6c3a 2074  lc_invite_url: t
+00000c90: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
+00000ca0: 7970 696e 672e 4361 6c6c 6162 6c65 5b5b  yping.Callable[[
+00000cb0: 7374 725d 2c20 7374 725d 5d2c 0a29 202d  str], str]],.) -
+00000cc0: 3e20 7374 723a 0a20 2020 2069 6620 6e6f  > str:.    if no
+00000cd0: 7420 746f 6b65 6e20 6f72 206e 6f74 2066  t token or not f
+00000ce0: 6e5f 6361 6c63 5f69 6e76 6974 655f 7572  n_calc_invite_ur
+00000cf0: 6c3a 0a20 2020 2020 2020 2072 6574 7572  l:.        retur
+00000d00: 6e20 2241 206c 696e 6b20 7769 6c6c 2061  n "A link will a
+00000d10: 7070 6561 7220 6865 7265 206f 6e63 6520  ppear here once 
+00000d20: 796f 7520 6861 7665 2073 6574 2079 6f75  you have set you
+00000d30: 7220 4469 7363 6f72 6420 746f 6b65 6e2e  r Discord token.
+00000d40: 220a 2020 2020 6c69 6e6b 203d 2066 6e5f  ".    link = fn_
+00000d50: 6361 6c63 5f69 6e76 6974 655f 7572 6c28  calc_invite_url(
+00000d60: 746f 6b65 6e29 0a20 2020 2072 6574 7572  token).    retur
+00000d70: 6e20 280a 2020 2020 2020 2020 6627 3c61  n (.        f'<a
+00000d80: 2068 7265 663d 227b 6c69 6e6b 7d22 2069   href="{link}" i
+00000d90: 643d 226f 6f62 6162 6f74 2d69 6e76 6974  d="oobabot-invit
+00000da0: 652d 6c69 6e6b 2220 7461 7267 6574 3d22  e-link" target="
+00000db0: 5f62 6c61 6e6b 223e 436c 6963 6b20 6865  _blank">Click he
+00000dc0: 7265 2074 6f20 3c70 7265 3e27 0a20 2020  re to <pre>'.   
+00000dd0: 2020 2020 202b 2022 696e 7669 7465 2079       + "invite y
+00000de0: 6f75 7220 626f 743c 2f70 7265 3e20 746f  our bot</pre> to
+00000df0: 2061 2044 6973 636f 7264 2073 6572 7665   a Discord serve
+00000e00: 723c 2f61 3e2e 220a 2020 2020 290a 0a0a  r</a>.".    )...
+00000e10: 6465 6620 7570 6461 7465 5f64 6973 636f  def update_disco
+00000e20: 7264 5f69 6e76 6974 655f 6c69 6e6b 280a  rd_invite_link(.
+00000e30: 2020 2020 6e65 775f 746f 6b65 6e3a 2073      new_token: s
+00000e40: 7472 2c0a 2020 2020 6973 5f74 6f6b 656e  tr,.    is_token
+00000e50: 5f76 616c 6964 3a20 626f 6f6c 2c0a 2020  _valid: bool,.  
+00000e60: 2020 6973 5f74 6573 7465 643a 2062 6f6f    is_tested: boo
+00000e70: 6c2c 0a20 2020 2066 6e5f 6765 6e65 7261  l,.    fn_genera
+00000e80: 7465 5f69 6e76 6974 655f 7572 6c3a 2074  te_invite_url: t
+00000e90: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
+00000ea0: 7970 696e 672e 4361 6c6c 6162 6c65 5b5b  yping.Callable[[
+00000eb0: 7374 725d 2c20 7374 725d 5d2c 0a29 3a0a  str], str]],.):.
+00000ec0: 2020 2020 6e65 775f 746f 6b65 6e20 3d20      new_token = 
+00000ed0: 6e65 775f 746f 6b65 6e2e 7374 7269 7028  new_token.strip(
+00000ee0: 290a 2020 2020 7072 6566 6978 203d 2022  ).    prefix = "
+00000ef0: 220a 2020 2020 6966 2069 735f 7465 7374  ".    if is_test
+00000f00: 6564 3a0a 2020 2020 2020 2020 6966 2069  ed:.        if i
+00000f10: 735f 746f 6b65 6e5f 7661 6c69 643a 0a20  s_token_valid:. 
+00000f20: 2020 2020 2020 2020 2020 2070 7265 6669             prefi
+00000f30: 7820 3d20 22e2 9c94 efb8 8f20 596f 7572  x = "...... Your
+00000f40: 2074 6f6b 656e 2069 7320 7661 6c69 642e   token is valid.
+00000f50: 3c62 723e 3c62 723e 220a 2020 2020 2020  <br><br>".      
+00000f60: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00000f70: 2020 2020 7072 6566 6978 203d 2022 e29d      prefix = "..
+00000f80: 8c20 596f 7572 2074 6f6b 656e 2069 7320  . Your token is 
+00000f90: 696e 7661 6c69 642e 220a 2020 2020 6966  invalid.".    if
+00000fa0: 2069 735f 746f 6b65 6e5f 7661 6c69 643a   is_token_valid:
+00000fb0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000fc0: 7072 6566 6978 202b 206d 616b 655f 6c69  prefix + make_li
+00000fd0: 6e6b 5f66 726f 6d5f 746f 6b65 6e28 0a20  nk_from_token(. 
+00000fe0: 2020 2020 2020 2020 2020 206e 6577 5f74             new_t
+00000ff0: 6f6b 656e 2c0a 2020 2020 2020 2020 2020  oken,.          
+00001000: 2020 666e 5f67 656e 6572 6174 655f 696e    fn_generate_in
+00001010: 7669 7465 5f75 726c 2c0a 2020 2020 2020  vite_url,.      
+00001020: 2020 290a 2020 2020 6966 206e 6577 5f74    ).    if new_t
+00001030: 6f6b 656e 3a0a 2020 2020 2020 2020 7265  oken:.        re
+00001040: 7475 726e 2070 7265 6669 780a 2020 2020  turn prefix.    
+00001050: 7265 7475 726e 2022 4120 6c69 6e6b 2077  return "A link w
+00001060: 696c 6c20 6170 7065 6172 2068 6572 6520  ill appear here 
+00001070: 6f6e 6365 2079 6f75 2068 6176 6520 7365  once you have se
+00001080: 7420 796f 7572 2044 6973 636f 7264 2074  t your Discord t
+00001090: 6f6b 656e 2e22 0a0a 0a43 4841 5241 4354  oken."...CHARACT
+000010a0: 4552 5f4e 4f4e 4520 3d20 224e 6f6e 6522  ER_NONE = "None"
+000010b0: 0a0a 0a64 6566 2067 6574 5f61 7661 696c  ...def get_avail
+000010c0: 6162 6c65 5f63 6861 7261 6374 6572 7328  able_characters(
+000010d0: 2920 2d3e 2074 7970 696e 672e 4c69 7374  ) -> typing.List
+000010e0: 5b73 7472 5d3a 0a20 2020 2022 2222 0a20  [str]:.    """. 
+000010f0: 2020 2054 6869 7320 6973 2061 206c 6973     This is a lis
+00001100: 7420 6f66 2061 6c6c 2066 696c 6573 2069  t of all files i
+00001110: 6e20 7468 6520 2e2f 6368 6172 6163 7465  n the ./characte
+00001120: 7273 2066 6f6c 6465 7220 7768 6f73 650a  rs folder whose.
+00001130: 2020 2020 6578 7465 6e73 696f 6e20 6973      extension is
+00001140: 202e 6a73 6f6e 2c20 2e79 616d 6c2c 206f   .json, .yaml, o
+00001150: 7220 2e79 6d6c 0a0a 2020 2020 5468 6520  r .yml..    The 
+00001160: 6c69 7374 2069 7320 7468 656e 2073 6f72  list is then sor
+00001170: 7465 6420 616c 7068 6162 6574 6963 616c  ted alphabetical
+00001180: 6c79 2c20 616e 6420 274e 6f6e 6527 2069  ly, and 'None' i
+00001190: 7320 6164 6465 6420 746f 0a20 2020 2074  s added to.    t
+000011a0: 6865 2073 7461 7274 2e0a 2020 2020 2222  he start..    ""
+000011b0: 220a 2020 2020 6368 6172 6163 7465 7273  ".    characters
+000011c0: 203d 205b 5d0a 2020 2020 666f 7220 6578   = [].    for ex
+000011d0: 7465 6e73 696f 6e20 696e 205b 2279 6d6c  tension in ["yml
+000011e0: 222c 2022 7961 6d6c 222c 2022 6a73 6f6e  ", "yaml", "json
+000011f0: 225d 3a0a 2020 2020 2020 2020 666f 7220  "]:.        for 
+00001200: 6669 6c65 7061 7468 2069 6e20 7061 7468  filepath in path
+00001210: 6c69 622e 5061 7468 2822 6368 6172 6163  lib.Path("charac
+00001220: 7465 7273 2229 2e67 6c6f 6228 6622 2a2e  ters").glob(f"*.
+00001230: 7b65 7874 656e 7369 6f6e 7d22 293a 0a20  {extension}"):. 
+00001240: 2020 2020 2020 2020 2020 2063 6861 7261             chara
+00001250: 6374 6572 732e 6170 7065 6e64 2866 696c  cters.append(fil
+00001260: 6570 6174 682e 7374 656d 290a 2020 2020  epath.stem).    
+00001270: 6368 6172 6163 7465 7273 2e73 6f72 7428  characters.sort(
+00001280: 290a 2020 2020 6368 6172 6163 7465 7273  ).    characters
+00001290: 2e69 6e73 6572 7428 302c 2043 4841 5241  .insert(0, CHARA
+000012a0: 4354 4552 5f4e 4f4e 4529 0a20 2020 2072  CTER_NONE).    r
+000012b0: 6574 7572 6e20 6368 6172 6163 7465 7273  eturn characters
+000012c0: 0a0a 0a64 6566 2072 6570 6169 725f 6c6f  ...def repair_lo
+000012d0: 6767 696e 6728 2920 2d3e 2074 7970 696e  gging() -> typin
+000012e0: 672e 4f70 7469 6f6e 616c 5b6c 6f67 6769  g.Optional[loggi
+000012f0: 6e67 2e4c 6f67 6765 725d 3a0a 2020 2020  ng.Logger]:.    
+00001300: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001310: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001320: 2323 0a20 2020 2023 2073 6f2c 206c 6f67  ##.    # so, log
+00001330: 6769 6e67 5f63 6f6c 6f72 732e 7079 2c20  ging_colors.py, 
+00001340: 7261 7468 6572 2074 6861 6e20 7573 696e  rather than usin
+00001350: 6720 7468 6520 6c6f 6767 696e 6720 6d6f  g the logging mo
+00001360: 6475 6c65 2773 2062 7569 6c74 2d69 6e0a  dule's built-in.
+00001370: 2020 2020 2320 666f 726d 6174 7465 722c      # formatter,
+00001380: 2069 7320 6d6f 6e6b 6579 2d70 6174 6368   is monkey-patch
+00001390: 696e 6720 7468 6520 6c6f 6767 696e 6720  ing the logging 
+000013a0: 6d6f 6475 6c65 2773 2053 7472 6561 6d48  module's StreamH
+000013b0: 616e 646c 6572 2e65 6d69 742e 0a20 2020  andler.emit..   
+000013c0: 2023 2054 6869 7320 6973 2061 2070 726f   # This is a pro
+000013d0: 626c 656d 2066 6f72 2075 732c 2062 6563  blem for us, bec
+000013e0: 6175 7365 2077 6520 616c 736f 2075 7365  ause we also use
+000013f0: 2074 6865 206c 6f67 6769 6e67 206d 6f64   the logging mod
+00001400: 756c 652c 2062 7574 0a20 2020 2023 2064  ule, but.    # d
+00001410: 6f6e 2774 2077 616e 7420 414e 5349 2063  on't want ANSI c
+00001420: 6f6c 6f72 2063 6f64 6573 2073 686f 7769  olor codes showi
+00001430: 6e67 2075 7020 696e 2048 544d 4c2e 2020  ng up in HTML.  
+00001440: 5765 2061 6c73 6f20 646f 6e27 7420 7761  We also don't wa
+00001450: 6e74 0a20 2020 2023 2074 6f20 6272 6561  nt.    # to brea
+00001460: 6b20 7468 6569 7220 6c6f 6767 696e 672e  k their logging.
+00001470: 0a20 2020 2023 0a20 2020 2023 2053 6f2c  .    #.    # So,
+00001480: 2077 6527 7265 2067 6f69 6e67 2074 6f20   we're going to 
+00001490: 7361 7665 2074 6865 6972 206d 6f6e 6b65  save their monke
+000014a0: 792d 7061 7463 6865 6420 656d 6974 2c20  y-patched emit, 
+000014b0: 7265 6c6f 6164 2074 6865 206c 6f67 6769  reload the loggi
+000014c0: 6e67 0a20 2020 2023 206d 6f64 756c 652c  ng.    # module,
+000014d0: 2073 6176 6520 6f66 6620 7468 6520 2272   save off the "r
+000014e0: 6561 6c22 2065 6d69 742c 2074 6865 6e20  eal" emit, then 
+000014f0: 7265 2d61 7070 6c79 2074 6865 6972 206d  re-apply their m
+00001500: 6f6e 6b65 792d 7061 7463 682e 0a20 2020  onkey-patch..   
+00001510: 2023 0a20 2020 2023 2057 6520 6e65 6564   #.    # We need
+00001520: 2074 6f20 646f 2061 6c6c 2074 6869 7320   to do all this 
+00001530: 6265 666f 7265 2077 6520 6372 6561 7465  before we create
+00001540: 2074 6865 206f 6f62 6162 6f74 5f77 6f72   the oobabot_wor
+00001550: 6b65 722c 2073 6f20 7468 6174 0a20 2020  ker, so that.   
+00001560: 2023 2074 6865 206c 6f67 7320 6372 6561   # the logs crea
+00001570: 7465 6420 6475 7269 6e67 2073 7461 7274  ted during start
+00001580: 7570 2061 7265 2070 726f 7065 726c 7920  up are properly 
+00001590: 666f 726d 6174 7465 642e 0a0a 2020 2020  formatted...    
+000015a0: 2320 7361 7665 2074 6865 206d 6f6e 6b65  # save the monke
+000015b0: 792d 7061 7463 6865 6420 656d 6974 0a20  y-patched emit. 
+000015c0: 2020 2068 6163 6b65 645f 656d 6974 203d     hacked_emit =
+000015d0: 206c 6f67 6769 6e67 2e53 7472 6561 6d48   logging.StreamH
+000015e0: 616e 646c 6572 2e65 6d69 740a 0a20 2020  andler.emit..   
+000015f0: 2023 2072 656c 6f61 6420 7468 6520 6c6f   # reload the lo
+00001600: 6767 696e 6720 6d6f 6475 6c65 0a20 2020  gging module.   
+00001610: 2074 7279 3a0a 2020 2020 2020 2020 696d   try:.        im
+00001620: 706f 7274 6c69 622e 7265 6c6f 6164 286c  portlib.reload(l
+00001630: 6f67 6769 6e67 290a 2020 2020 6578 6365  ogging).    exce
+00001640: 7074 2049 6d70 6f72 7445 7272 6f72 2061  pt ImportError a
+00001650: 7320 6572 723a 0a20 2020 2020 2020 2070  s err:.        p
+00001660: 7269 6e74 2866 224f 6f62 6162 6f74 3a20  rint(f"Oobabot: 
+00001670: 4572 726f 7220 7265 6c6f 6164 696e 6720  Error reloading 
+00001680: 6c6f 6767 696e 6720 6d6f 6475 6c65 3a20  logging module: 
+00001690: 7b65 7272 7d22 2c20 6669 6c65 3d73 7973  {err}", file=sys
+000016a0: 2e73 7464 6572 7229 0a20 2020 2020 2020  .stderr).       
+000016b0: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
+000016c0: 2020 2320 6372 6561 7465 206f 7572 206c    # create our l
+000016d0: 6f67 6765 7220 6561 726c 790a 2020 2020  ogger early.    
+000016e0: 6f6f 6261 626f 742e 6661 6e63 795f 6c6f  oobabot.fancy_lo
+000016f0: 6767 6572 2e69 6e69 745f 6c6f 6767 696e  gger.init_loggin
+00001700: 6728 6c6f 6767 696e 672e 4445 4255 472c  g(logging.DEBUG,
+00001710: 2054 7275 6529 0a20 2020 206f 6f62 615f   True).    ooba_
+00001720: 6c6f 6767 6572 203d 206f 6f62 6162 6f74  logger = oobabot
+00001730: 2e66 616e 6379 5f6c 6f67 6765 722e 6765  .fancy_logger.ge
+00001740: 7428 290a 0a20 2020 2023 206d 616e 7561  t()..    # manua
+00001750: 6c6c 7920 6170 706c 7920 7468 6520 2263  lly apply the "c
+00001760: 6f72 7265 6374 2220 656d 6974 2074 6f20  orrect" emit to 
+00001770: 6561 6368 206f 6620 7468 6520 5374 7265  each of the Stre
+00001780: 616d 4861 6e64 6c65 7273 0a20 2020 2023  amHandlers.    #
+00001790: 2074 6861 7420 6661 6e63 795f 6c6f 6767   that fancy_logg
+000017a0: 6572 2063 7265 6174 6564 0a20 2020 2066  er created.    f
+000017b0: 6f72 2068 616e 646c 6572 2069 6e20 6f6f  or handler in oo
+000017c0: 6261 5f6c 6f67 6765 722e 6861 6e64 6c65  ba_logger.handle
+000017d0: 7273 3a0a 2020 2020 2020 2020 6966 2069  rs:.        if i
+000017e0: 7369 6e73 7461 6e63 6528 6861 6e64 6c65  sinstance(handle
+000017f0: 722c 206c 6f67 6769 6e67 2e53 7472 6561  r, logging.Strea
+00001800: 6d48 616e 646c 6572 293a 0a20 2020 2020  mHandler):.     
+00001810: 2020 2020 2020 2068 616e 646c 6572 2e65         handler.e
+00001820: 6d69 7420 3d20 7479 7065 732e 4d65 7468  mit = types.Meth
+00001830: 6f64 5479 7065 286c 6f67 6769 6e67 2e53  odType(logging.S
+00001840: 7472 6561 6d48 616e 646c 6572 2e65 6d69  treamHandler.emi
+00001850: 742c 2068 616e 646c 6572 290a 0a20 2020  t, handler)..   
+00001860: 206c 6f67 6769 6e67 2e53 7472 6561 6d48   logging.StreamH
+00001870: 616e 646c 6572 2e65 6d69 7420 3d20 6861  andler.emit = ha
+00001880: 636b 6564 5f65 6d69 740a 2020 2020 7265  cked_emit.    re
+00001890: 7475 726e 206f 6f62 615f 6c6f 6767 6572  turn ooba_logger
+000018a0: 0a0a 0a53 5441 5455 535f 5052 4546 4958  ...STATUS_PREFIX
+000018b0: 203d 2022 3c68 333e 4f6f 6261 626f 7420   = "<h3>Oobabot 
+000018c0: 5374 6174 7573 3c2f 6833 3e22 0a0a 0a64  Status</h3>"...d
+000018d0: 6566 2073 7461 7475 735f 6865 6164 696e  ef status_headin
+000018e0: 6728 7374 6174 7573 3a20 7374 7229 202d  g(status: str) -
+000018f0: 3e20 7374 723a 0a20 2020 2069 6620 7374  > str:.    if st
+00001900: 6174 7573 203d 3d20 2272 756e 6e69 6e67  atus == "running
+00001910: 223a 0a20 2020 2020 2020 2072 6574 7572  ":.        retur
+00001920: 6e20 280a 2020 2020 2020 2020 2020 2020  n (.            
+00001930: 5354 4154 5553 5f50 5245 4649 580a 2020  STATUS_PREFIX.  
+00001940: 2020 2020 2020 2020 2020 2b20 273c 6469            + '<di
+00001950: 7620 636c 6173 733d 226f 6f62 6162 6f74  v class="oobabot
+00001960: 5f73 7461 7475 7320 6f6f 6261 626f 745f  _status oobabot_
+00001970: 7374 6174 7573 5f72 756e 6e69 6e67 223e  status_running">
+00001980: 5275 6e6e 696e 673c 2f64 6976 3e27 0a20  Running</div>'. 
+00001990: 2020 2020 2020 2029 0a20 2020 2069 6620         ).    if 
+000019a0: 7374 6174 7573 203d 3d20 2273 746f 7070  status == "stopp
+000019b0: 6564 223a 0a20 2020 2020 2020 2072 6574  ed":.        ret
+000019c0: 7572 6e20 280a 2020 2020 2020 2020 2020  urn (.          
+000019d0: 2020 5354 4154 5553 5f50 5245 4649 580a    STATUS_PREFIX.
+000019e0: 2020 2020 2020 2020 2020 2020 2b20 273c              + '<
+000019f0: 6469 7620 636c 6173 733d 226f 6f62 6162  div class="oobab
+00001a00: 6f74 5f73 7461 7475 7320 6f6f 6261 626f  ot_status oobabo
+00001a10: 745f 7374 6174 7573 5f73 746f 7070 6564  t_status_stopped
+00001a20: 223e 5374 6f70 7065 643c 2f64 6976 3e27  ">Stopped</div>'
+00001a30: 0a20 2020 2020 2020 2029 0a20 2020 2072  .        ).    r
+00001a40: 6574 7572 6e20 5354 4154 5553 5f50 5245  eturn STATUS_PRE
+00001a50: 4649 580a                                FIX.
```

### Comparing `oobabot_plugin-0.2.0/src/oobabot_plugin/transcript_view.py` & `oobabot_plugin-0.2.1/src/oobabot_plugin/transcript_view.py`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.2.0/src/oobabot_plugin/worker.py` & `oobabot_plugin-0.2.1/src/oobabot_plugin/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,22 +86,30 @@
         """
         Returns True if the user has entered a discord token.
         """
         if self.bot.settings.discord_settings.get_str("discord_token"):
             return True
         return False
 
+    def get_log_etag(self) -> int:
+        """
+        Returns an etag for the oobabot's log.
+        """
+        if self.bot is None:
+            return -1
+        return self.bot.log_count()
+
     def get_logs(self) -> str:
         """
         Returns the logs from the oobabot.
         """
         if self.bot is None:
             return ""
 
-        lines = oobabot.fancy_logger.recent_logs.get_all()
+        lines = self.bot.logs()
         return (
             '<div class="oobabot-log">' + "\n<br>".join(lines) + "</div></body></html>"
         )
 
     def save_settings(self):
         if self.bot is None:
             return
```

### Comparing `oobabot_plugin-0.2.0/PKG-INFO` & `oobabot_plugin-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: oobabot-plugin
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Discord bot plugin to oobabooga's text-generation-webui, based on oobabot.
 Home-page: https://github.com/chrisrude/oobabot-plugin
 License: MIT
 Author: Christopher Rude
 Author-email: chris@rudesoftware.net
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi (>=0.99.1,<0.100.0)
 Requires-Dist: gradio (>=3.34.0,<3.35.0)
-Requires-Dist: oobabot (>=0.2.0,<0.3.0)
+Requires-Dist: oobabot (>=0.2.1,<0.3.0)
 Project-URL: Repository, https://github.com/chrisrude/oobabot-plugin
 Description-Content-Type: text/markdown
 
 # Oobabot-plugin
 
 [**`oobabot`**](https://github.com/chrisrude/oobabot) is a Discord bot which talks to a Large Language Model AIs (like LLaMA, llama.cpp, etc...), running on [oobabooga's text-generation-webui](https://github.com/oobabooga/text-generation-webui).
```

