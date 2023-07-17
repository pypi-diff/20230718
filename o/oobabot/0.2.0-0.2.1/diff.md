# Comparing `tmp/oobabot-0.2.0.tar.gz` & `tmp/oobabot-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oobabot-0.2.0.tar", max compression
+gzip compressed data, was "oobabot-0.2.1.tar", max compression
```

## Comparing `oobabot-0.2.0.tar` & `oobabot-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1067 2023-06-04 16:32:46.838921 oobabot-0.2.0/LICENSE
--rw-r--r--   0        0        0    14771 2023-07-07 09:39:36.542311 oobabot-0.2.0/README.md
--rw-r--r--   0        0        0     1242 2023-06-28 06:17:56.191776 oobabot-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      109 2023-06-22 17:46:43.191778 oobabot-0.2.0/src/oobabot/__init__.py
--rw-r--r--   0        0        0      121 2023-06-04 16:34:13.130150 oobabot-0.2.0/src/oobabot/__main__.py
--rw-r--r--   0        0        0     5701 2023-06-25 07:35:53.143740 oobabot-0.2.0/src/oobabot/audio_commands.py
--rw-r--r--   0        0        0     4255 2023-06-28 03:58:01.057680 oobabot-0.2.0/src/oobabot/audio_responder.py
--rw-r--r--   0        0        0     6715 2023-06-24 10:16:43.418003 oobabot-0.2.0/src/oobabot/bot_commands.py
--rw-r--r--   0        0        0     7616 2023-06-04 16:34:13.130476 oobabot-0.2.0/src/oobabot/decide_to_respond.py
--rw-r--r--   0        0        0    30180 2023-06-27 18:17:06.105806 oobabot-0.2.0/src/oobabot/discord_bot.py
--rw-r--r--   0        0        0    13538 2023-06-28 06:17:56.192524 oobabot-0.2.0/src/oobabot/discord_utils.py
--rw-r--r--   0        0        0     7398 2023-06-28 06:17:56.193881 oobabot-0.2.0/src/oobabot/discrivener.py
--rw-r--r--   0        0        0     7696 2023-06-28 06:17:56.195692 oobabot-0.2.0/src/oobabot/discrivener_message.py
--rw-r--r--   0        0        0     9954 2023-06-30 16:20:06.306446 oobabot-0.2.0/src/oobabot/fancy_logger.py
--rw-r--r--   0        0        0     3106 2023-06-25 08:04:52.621295 oobabot-0.2.0/src/oobabot/http_client.py
--rw-r--r--   0        0        0    13441 2023-06-28 02:27:36.169389 oobabot-0.2.0/src/oobabot/image_generator.py
--rw-r--r--   0        0        0    10232 2023-06-27 19:34:35.425514 oobabot-0.2.0/src/oobabot/ooba_client.py
--rwxr-xr-x   0        0        0     8344 2023-06-30 16:20:06.306774 oobabot-0.2.0/src/oobabot/oobabot.py
--rw-r--r--   0        0        0    13657 2023-07-05 22:59:35.084527 oobabot-0.2.0/src/oobabot/overengineered_settings_parser.py
--rw-r--r--   0        0        0     4145 2023-07-05 22:59:35.086048 oobabot-0.2.0/src/oobabot/persona.py
--rw-r--r--   0        0        0     7774 2023-06-04 16:34:13.132066 oobabot-0.2.0/src/oobabot/prompt_generator.py
--rw-r--r--   0        0        0     3243 2023-06-04 16:34:13.132218 oobabot-0.2.0/src/oobabot/repetition_tracker.py
--rw-r--r--   0        0        0     6736 2023-06-04 16:34:13.132382 oobabot-0.2.0/src/oobabot/response_stats.py
--rw-r--r--   0        0        0     9963 2023-06-27 16:19:38.608247 oobabot-0.2.0/src/oobabot/runtime.py
--rw-r--r--   0        0        0    11466 2023-06-27 18:16:30.917288 oobabot-0.2.0/src/oobabot/sd_client.py
--rw-r--r--   0        0        0    30574 2023-07-07 09:39:36.544798 oobabot-0.2.0/src/oobabot/settings.py
--rw-r--r--   0        0        0    10905 2023-07-02 22:19:21.886909 oobabot-0.2.0/src/oobabot/templates.py
--rw-r--r--   0        0        0     3744 2023-06-28 03:58:01.058041 oobabot-0.2.0/src/oobabot/transcript.py
--rw-r--r--   0        0        0     5191 2023-06-28 06:17:56.198342 oobabot-0.2.0/src/oobabot/types.py
--rw-r--r--   0        0        0    12730 2023-06-28 06:17:56.198871 oobabot-0.2.0/src/oobabot/voice_client.py
--rw-r--r--   0        0        0    15608 1970-01-01 00:00:00.000000 oobabot-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-04 16:32:46.838921 oobabot-0.2.1/LICENSE
+-rw-r--r--   0        0        0    14771 2023-07-17 23:06:16.143080 oobabot-0.2.1/README.md
+-rw-r--r--   0        0        0     1243 2023-07-17 23:06:16.147063 oobabot-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-07-17 23:06:16.148762 oobabot-0.2.1/src/oobabot/__init__.py
+-rw-r--r--   0        0        0      121 2023-06-04 16:34:13.130150 oobabot-0.2.1/src/oobabot/__main__.py
+-rw-r--r--   0        0        0     5701 2023-06-25 07:35:53.143740 oobabot-0.2.1/src/oobabot/audio_commands.py
+-rw-r--r--   0        0        0     4255 2023-06-28 03:58:01.057680 oobabot-0.2.1/src/oobabot/audio_responder.py
+-rw-r--r--   0        0        0     7630 2023-07-09 16:08:40.821308 oobabot-0.2.1/src/oobabot/bot_commands.py
+-rw-r--r--   0        0        0     7616 2023-06-04 16:34:13.130476 oobabot-0.2.1/src/oobabot/decide_to_respond.py
+-rw-r--r--   0        0        0    30784 2023-07-09 16:08:40.822212 oobabot-0.2.1/src/oobabot/discord_bot.py
+-rw-r--r--   0        0        0    13885 2023-07-09 16:08:40.822598 oobabot-0.2.1/src/oobabot/discord_utils.py
+-rw-r--r--   0        0        0     7224 2023-07-09 16:08:40.822910 oobabot-0.2.1/src/oobabot/discrivener.py
+-rw-r--r--   0        0        0     7696 2023-06-28 06:17:56.195692 oobabot-0.2.1/src/oobabot/discrivener_message.py
+-rw-r--r--   0        0        0    10189 2023-07-12 10:32:53.174573 oobabot-0.2.1/src/oobabot/fancy_logger.py
+-rw-r--r--   0        0        0     3106 2023-06-25 08:04:52.621295 oobabot-0.2.1/src/oobabot/http_client.py
+-rw-r--r--   0        0        0    11727 2023-07-09 16:08:40.823923 oobabot-0.2.1/src/oobabot/image_generator.py
+-rw-r--r--   0        0        0    10285 2023-07-17 23:06:16.149834 oobabot-0.2.1/src/oobabot/ooba_client.py
+-rwxr-xr-x   0        0        0     8803 2023-07-12 10:43:42.912452 oobabot-0.2.1/src/oobabot/oobabot.py
+-rw-r--r--   0        0        0    13657 2023-07-05 22:59:35.084527 oobabot-0.2.1/src/oobabot/overengineered_settings_parser.py
+-rw-r--r--   0        0        0     4145 2023-07-05 22:59:35.086048 oobabot-0.2.1/src/oobabot/persona.py
+-rw-r--r--   0        0        0     7167 2023-07-09 16:08:40.826615 oobabot-0.2.1/src/oobabot/prompt_generator.py
+-rw-r--r--   0        0        0     3243 2023-06-04 16:34:13.132218 oobabot-0.2.1/src/oobabot/repetition_tracker.py
+-rw-r--r--   0        0        0     6736 2023-06-04 16:34:13.132382 oobabot-0.2.1/src/oobabot/response_stats.py
+-rw-r--r--   0        0        0    10031 2023-07-09 16:08:40.827913 oobabot-0.2.1/src/oobabot/runtime.py
+-rw-r--r--   0        0        0    18019 2023-07-09 16:08:40.828872 oobabot-0.2.1/src/oobabot/sd_client.py
+-rw-r--r--   0        0        0    31578 2023-07-09 16:08:40.829319 oobabot-0.2.1/src/oobabot/settings.py
+-rw-r--r--   0        0        0     9837 2023-07-09 16:08:40.830085 oobabot-0.2.1/src/oobabot/templates.py
+-rw-r--r--   0        0        0     3744 2023-06-28 03:58:01.058041 oobabot-0.2.1/src/oobabot/transcript.py
+-rw-r--r--   0        0        0     5191 2023-06-28 06:17:56.198342 oobabot-0.2.1/src/oobabot/types.py
+-rw-r--r--   0        0        0    12730 2023-06-28 06:17:56.198871 oobabot-0.2.1/src/oobabot/voice_client.py
+-rw-r--r--   0        0        0    15608 1970-01-01 00:00:00.000000 oobabot-0.2.1/PKG-INFO
```

### Comparing `oobabot-0.2.0/LICENSE` & `oobabot-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oobabot-0.2.0/README.md` & `oobabot-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
                [--discord-token DISCORD_TOKEN] [--dont-split-responses]
                [--history-lines HISTORY_LINES] [--ignore-dms] [--reply-in-thread]
                [--stream-responses] [--base-url BASE_URL] [--log-all-the-things]
                [--message-regex MESSAGE_REGEX] [--image-words [IMAGE_WORDS ...]]
                [--stable-diffusion-url STABLE_DIFFUSION_URL]
                [--extra-prompt-text EXTRA_PROMPT_TEXT]
 
-oobabot v0.2.0: Discord bot for oobabooga's text-generation-webui
+oobabot v0.2.1: Discord bot for oobabooga's text-generation-webui
 
 General Settings:
 
   -h, --help
   -c CONFIG, --config CONFIG
                         Path to a config file to read settings from. Command line settings
                         will override settings in this file. (default: config.yml)
```

### Comparing `oobabot-0.2.0/pyproject.toml` & `oobabot-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oobabot"
-version = "0.2.0"
+version = "0.2.1"
 description = "A Discord bot which talks to Large Language Model AIs running on oobabooga's text-generation-webui"
 authors = ["Christopher Rude <chris@rudesoftware.net>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/chrisrude/oobabot"
 
 [tool.poetry.dependencies]
@@ -30,15 +30,15 @@
 pycodestyle = ["-E203", "-W503", "-W504"]
 
 [tool.poetry.group.test.dependencies]
 black = "^23.3.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 pre-commit = "^3.2.0"
-pyright = "1.1.315"
+pyright = "^1.1.316"
 pytest = "^7.1"
 pylint = "^2.17.4"
 
 [tool.isort]
 profile = "black"
 force_single_line = true
 force_sort_within_sections = true
```

### Comparing `oobabot-0.2.0/src/oobabot/audio_commands.py` & `oobabot-0.2.1/src/oobabot/audio_commands.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.2.0/src/oobabot/audio_responder.py` & `oobabot-0.2.1/src/oobabot/audio_responder.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.2.0/src/oobabot/bot_commands.py` & `oobabot-0.2.1/src/oobabot/bot_commands.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,24 +33,54 @@
         prompt_generator: prompt_generator.PromptGenerator,
     ):
         self.decide_to_respond = decide_to_respond
         self.repetition_tracker = repetition_tracker
         self.persona = persona
         self.reply_in_thread = discord_settings["reply_in_thread"]
         self.template_store = template_store
-        self.discrivener_location = discord_settings["discrivener_location"]
-        self.discrivener_model_location = discord_settings["discrivener_model_location"]
-        self.audio_commands = audio_commands.AudioCommands(
-            persona,
-            ooba_client,
-            prompt_generator,
+
+        (
             self.discrivener_location,
             self.discrivener_model_location,
+        ) = discord_utils.validate_discrivener_locations(
+            discord_settings["discrivener_location"],
+            discord_settings["discrivener_model_location"],
         )
 
+        if (
+            discord_settings["discrivener_location"]
+            and self.discrivener_location is None
+        ):
+            fancy_logger.get().warning(
+                "Audio disabled because executable at discrivener_location "
+                + "could not be found: %s",
+                discord_settings["discrivener_location"],
+            )
+
+        if (
+            discord_settings["discrivener_model_location"]
+            and self.discrivener_model_location is None
+        ):
+            fancy_logger.get().warning(
+                "Audio disable because the discrivener_model_location "
+                + "could not be found: %s",
+                discord_settings["discrivener_model_location"],
+            )
+
+        if self.discrivener_location is None or self.discrivener_model_location is None:
+            self.audio_commands = None
+        else:
+            self.audio_commands = audio_commands.AudioCommands(
+                persona,
+                ooba_client,
+                prompt_generator,
+                self.discrivener_location,
+                self.discrivener_model_location,
+            )
+
     async def on_ready(self, client: discord.Client):
         """
         Register commands with Discord.
         """
 
         async def get_messageable(
             interaction: discord.Interaction,
@@ -162,18 +192,15 @@
             "Registering commands, sometimes this takes a while..."
         )
 
         tree = discord.app_commands.CommandTree(client)
         tree.add_command(lobotomize)
         tree.add_command(say)
 
-        if discord_utils.is_discrivener_installed(
-            self.discrivener_location,
-            self.discrivener_model_location,
-        ):
+        if self.audio_commands is not None:
             self.audio_commands.add_commands(tree)
 
         commands = await tree.sync(guild=None)
         for command in commands:
             fancy_logger.get().info(
                 "Registered command: %s: %s", command.name, command.description
             )
```

### Comparing `oobabot-0.2.0/src/oobabot/decide_to_respond.py` & `oobabot-0.2.1/src/oobabot/decide_to_respond.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.2.0/src/oobabot/discord_bot.py` & `oobabot-0.2.1/src/oobabot/discord_bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -513,38 +513,47 @@
         last_message = None
         async for token in response_iterator:
             if "" == token:
                 continue
 
             response += token
             (response, abort_response) = self._filter_immersion_breaking_lines(response)
-            if abort_response:
-                break
-            if not response:
-                # we can't send an empty message
-                continue
+
+            # if we are aborting a response, we want to at least post
+            # the valid parts, so don't abort quite yet.
 
             if last_message is None:
+                if not response:
+                    # we don't want to send an empty message
+                    continue
+
                 # when we send the first message, we don't want to send a notification,
                 # as it will only include the first token of the response.  This will
                 # not be very useful to anyone.
                 last_message = await response_channel.send(
                     response,
                     allowed_mentions=allowed_mentions,
                     silent=True,
                     suppress_embeds=True,
                     reference=reference,  # type: ignore
                 )
             else:
                 await last_message.edit(
                     content=response,
                     allowed_mentions=allowed_mentions,
+                    suppress=True,
                 )
                 last_message.content = response
 
+            # we want to abort the response only after we've sent any valid
+            # messages, and potentially removed any partial immersion-breaking
+            # lines that we posted when they were in the process of being received.
+            if abort_response:
+                break
+
             this_response_stat.log_response_part()
 
         if last_message is not None:
             self.repetition_tracker.log_message(
                 response_channel_id,
                 discord_utils.discord_message_to_generic_message(last_message),
             )
@@ -557,14 +566,18 @@
         """
         Given a string that represents an individual response message,
         filter out any lines that would break immersion.
 
         These include lines that include a termination symbol, lines
         that attempt to carry on the conversation as a different user,
         and lines that include text which is part of the AI prompt.
+
+        Returns the subset of the input string that should be sent,
+        and a boolean indicating if we should abort the response entirely,
+        ignoring any further lines.
         """
         lines = sentence.split("\n")
         good_lines = []
         previous_line = ""
         abort_response = False
         for line in lines:
             # if the AI gives itself a second line, just ignore
```

### Comparing `oobabot-0.2.0/src/oobabot/discord_utils.py` & `oobabot-0.2.1/src/oobabot/discord_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 in the future, and to make it easier to test the AI without having to mock the
 Discord library.
 """
 
 
 import base64
 import functools
+import os
 import pathlib
 import re
 import typing
 
 import discord
 
 from oobabot import fancy_logger
@@ -192,16 +193,19 @@
     # extract it from there.
     #
     # the discord token has this format:
     # AAAAAAAAAAAAAAAAAAAAAAAAAA.BBBBBB.CCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCCC
     #
     # where each section, A, B, and C, is independently a base64-encoded string.
     #
-    # Section A encodes the bot's client ID, which is a 16-digit number.
-    # the other sections aren't important here.
+    # Section A encodes the bot's client ID, which is the decimal encoding of
+    # a 64-bit number in the range [21154535154122752, 18446744073709551615]
+    # (17 to 20 digits long).
+    #
+    # The other sections aren't important here.
     token_parts = discord_token.split(".")
     token_part_a = token_parts[0]
 
     # the base64 decoder requires the string to be a multiple of 4 characters
     # long, so we need to add padding
     if len(token_part_a) % 4 != 0:
         token_part_a += "=" * (4 - len(token_part_a) % 4)
@@ -255,52 +259,56 @@
         interaction.channel,
         reason,
     )
 
     await interaction.response.send_message(reason, ephemeral=True, silent=True)
 
 
-def is_discrivener_installed(
-    discrivener_location: str, discrivener_model_location: str
-):
+def _file_exists_and_is_file(filepath: typing.Optional[str]) -> typing.Optional[str]:
+    if filepath is None:
+        return None
+
+    path = pathlib.Path(filepath).expanduser()
+    if not path.is_file():
+        return None
+
+    if not os.access(path, os.R_OK):
+        return None
+
+    return str(path.resolve())
+
+
+def validate_discrivener_locations(
+    discrivener_location: str,
+    discrivener_model_location: str,
+) -> typing.Tuple[typing.Optional[str], typing.Optional[str]]:
     """
     Verify that the file discrivener_location exists
     and is a file.
 
     If that passes, also checks that discrivener_model_location
     exists and is a file.
-    """
-    if not discrivener_location:
-        return False
 
-    discrivener_location_path = pathlib.Path(discrivener_location).expanduser()
-    if not discrivener_location_path.is_file():
-        fancy_logger.get().warning(
-            "Discrivener not found at %s.  Audio integration not enabled.",
-            discrivener_location_path,
-        )
-        return False
-
-    fancy_logger.get().info("Discrivener found at %s", discrivener_location_path)
+    Returns the expanded paths to each files if it exists,
+    or None if it doesn't.
 
-    discrivener_model_location_path = pathlib.Path(
-        discrivener_model_location
-    ).expanduser()
-    if not discrivener_model_location_path.is_file():
-        fancy_logger.get().warning(
-            "Discrivener model not found at %s.  Audio integration not enabled.",
-            discrivener_model_location_path,
-        )
-        return False
-
-    fancy_logger.get().info(
-        "Discrivener model found at %s", discrivener_model_location_path
-    )
+    Returns the tuple of these checks for the two passed files.
+    """
+    actual_discrivener_location = _file_exists_and_is_file(discrivener_location)
+    # check that the discrivener binary is executable as well
+    if actual_discrivener_location is not None:
+        if not os.access(actual_discrivener_location, os.X_OK):
+            fancy_logger.get().warning(
+                "discrivener binary is not executable: %s",
+                actual_discrivener_location,
+            )
+            actual_discrivener_location = None
 
-    return True
+    actual_model_location = _file_exists_and_is_file(discrivener_model_location)
+    return (actual_discrivener_location, actual_model_location)
 
 
 # the following class was modified from O'Reilly's Python Cookbook,
 # chapter 5, section 19.  Its use is allowed under this license:
 # Copyright (c) 2001, Sébastien Keim
 # All rights reserved.
 # Redistribution and use in source and binary forms, with or without
```

### Comparing `oobabot-0.2.0/src/oobabot/discrivener.py` & `oobabot-0.2.1/src/oobabot/discrivener.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,26 +9,23 @@
 import json
 import pathlib
 import signal
 import typing
 
 from oobabot import discrivener_message
 from oobabot import fancy_logger
-from oobabot import settings
 from oobabot import types
 
 
 class Discrivener:
     """
     Launches and handles the Discrivener process.
     """
 
-    # we want this shorter than STOP_LOCK_TIMEOUT so that
-    # we can log output from the process before we exit
-    KILL_TIMEOUT = settings.Settings.STOP_LOCK_TIMEOUT - 0.5
+    KILL_TIMEOUT: float = 2.0
 
     # pylint: disable=R1732
     def __init__(
         self,
         discrivener_location: str,
         discrivener_model_location: str,
         handler: typing.Callable[["types.DiscrivenerMessage"], None],
```

### Comparing `oobabot-0.2.0/src/oobabot/discrivener_message.py` & `oobabot-0.2.1/src/oobabot/discrivener_message.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.2.0/src/oobabot/fancy_logger.py` & `oobabot-0.2.1/src/oobabot/fancy_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,19 +275,29 @@
 class RingBufferedHandler(logging.Handler):
     """
     A singleton logging handler that stores the last N log messages in a ring buffer.
     """
 
     def __init__(self, buffer_size: int = 45) -> None:
         super().__init__()
+        self.change_count = 0
         self.buffer = RingBuffer(buffer_size)
 
     def emit(self, record: logging.LogRecord) -> None:
+        self.change_count += 1
         self.buffer.append(self.format(record))
 
+    @property
+    def changes(self) -> int:
+        """
+        Return the number of times the buffer has been
+        updated.
+        """
+        return self.change_count
+
     def get_all(self) -> typing.List[str]:
         return self.buffer.get()
 
 
 recent_logs = RingBufferedHandler()
```

### Comparing `oobabot-0.2.0/src/oobabot/http_client.py` & `oobabot-0.2.1/src/oobabot/http_client.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.2.0/src/oobabot/image_generator.py` & `oobabot-0.2.1/src/oobabot/image_generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import asyncio
 import io
 import re
 import typing
 
 import discord
 
-from oobabot import discord_utils
 from oobabot import fancy_logger
 from oobabot import http_client
 from oobabot import ooba_client
 from oobabot import prompt_generator
 from oobabot import sd_client
 from oobabot import templates
 
@@ -236,37 +235,27 @@
     ):
         self.ai_name = persona_settings.get("ai_name", "")
         self.ooba_client = ooba_client
         self.image_words = sd_settings.get("image_words", [])
         self.prompt_generator = prompt_generator
         self.stable_diffusion_client = stable_diffusion_client
         self.template_store = template_store
-        self.use_ai_generated_keywords = sd_settings.get("use_ai_generated_keywords")
 
         self.image_patterns = [
             re.compile(
                 r"^.*\b" + image_word + r"\b[\s]*(of|with)?[\s]*[:]?(.*)$",
                 re.IGNORECASE,
             )
             for image_word in self.image_words
         ]
 
     def on_ready(self):
         """
         Called when the bot is connected to Discord.
         """
-        if self.use_ai_generated_keywords:
-            fancy_logger.get().debug(
-                "Stable Diffusion: image prompts generated with AI preprocessing"
-            )
-        else:
-            fancy_logger.get().debug(
-                "Stable Diffusion: image prompts extracted with regex"
-            )
-
         fancy_logger.get().debug(
             "Stable Diffusion: image keywords: %s",
             ", ".join(self.image_words),
         )
 
     # @fancy_logger.log_async_task
     async def _generate_image(
@@ -341,41 +330,10 @@
         raw_message: discord.Message,
         response_channel: discord.abc.Messageable,
     ) -> "asyncio.Task[discord.Message]":
         """
         Kick off a task to generate an image, post it to the channel,
         and return message the image is posted in.
         """
-
-        if self.use_ai_generated_keywords:
-            # ignore the prompt extracted above, and instead pass
-            # the raw message back to Oobabooga and ask it to
-            # generate keywords.  Then pass those keywords to
-            # the image generator.
-            return asyncio.create_task(
-                self._generate_keywords_then_image(
-                    raw_message,
-                    response_channel,
-                )
-            )
-
         return asyncio.create_task(
             self._generate_image(user_image_keywords, raw_message, response_channel)
         )
-
-    async def _generate_keywords_then_image(
-        self,
-        raw_message: discord.Message,
-        response_channel: discord.abc.Messageable,
-    ) -> "discord.Message":
-        message = discord_utils.discord_message_to_generic_message(raw_message)
-        # remove the bot's name from the body text, so it doesn't
-        # pollute the keywords
-        message.body_text = message.body_text.replace(self.ai_name, "")
-        keyword_generation_prompt = self.prompt_generator.keyword_generation_prompt(
-            message
-        )
-        ai_keywords = await self.ooba_client.request_as_string(
-            keyword_generation_prompt
-        )
-        fancy_logger.get().debug("AI-generated keywords: %s", ai_keywords)
-        return await self._generate_image(ai_keywords, raw_message, response_channel)
```

### Comparing `oobabot-0.2.0/src/oobabot/ooba_client.py` & `oobabot-0.2.1/src/oobabot/ooba_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,16 +235,16 @@
         request.update(self.request_params)
 
         async with self._get_session().ws_connect(
             self.OOBABOOGA_STREAMING_URI_PATH
         ) as websocket:
             await websocket.send_json(request)
             if self.log_all_the_things:
-                print(f"Sent request:\n{json.dumps(request, indent=1)}")
-                print(f"Prompt:\n{request['prompt']}")
+                print(f"Sent request:\n{json.dumps(request, indent=1).encode('utf-8')}")
+                print(f"Prompt:\n{str(request['prompt']).encode('utf-8')}")
 
             async for msg in websocket:
                 # we expect a series of text messages in JSON encoding,
                 # like this:
                 #
                 # {"event": "text_stream", "message_num": 0, "text": ""}
                 # {"event": "text_stream", "message_num": 1, "text": "Oh"}
@@ -258,15 +258,15 @@
 
                     incoming_data = msg.json()
                     if "text_stream" == incoming_data["event"]:
                         self.total_response_tokens += 1
                         text = incoming_data["text"]
                         if text != SentenceSplitter.END_OF_INPUT:
                             if self.log_all_the_things:
-                                print(text, end="", flush=True)
+                                print(text.encode("utf-8"), end="", flush=True)
 
                             yield text
 
                     elif "stream_end" == incoming_data["event"]:
                         # Make sure any unprinted text is flushed.
                         if self.log_all_the_things:
                             print("", flush=True)
```

### Comparing `oobabot-0.2.0/src/oobabot/oobabot.py` & `oobabot-0.2.1/src/oobabot/oobabot.py`

 * *Files 6% similar despite different names*

```diff
@@ -145,18 +145,19 @@
         """
         Returns True if the bot is configured to participate in voice channels.
 
         This checks that both:
          a. discrivener is configured
          b. discrivener is installed
         """
-        return discord_utils.is_discrivener_installed(
+        exe_location, model_location = discord_utils.validate_discrivener_locations(
             self.settings.discord_settings.get_str("discrivener_location"),
             self.settings.discord_settings.get_str("discrivener_model_location"),
         )
+        return exe_location is not None and model_location is not None
 
     @property
     def current_voice_transcript(
         self,
     ) -> typing.List["types.VoiceMessage"]:
         """
         If the bot is currently in a voice channel, returns the transcript
@@ -183,14 +184,27 @@
         the server-specific nickname, color, and icon.
         """
         client = voice_client.VoiceClient.current_instance
         if client is None:
             return None
         return discord_utils.author_from_user_id(user_id, client.guild)
 
+    def log_count(self) -> int:
+        """
+        Returns the current number of times the log has been
+        appended to.
+        """
+        return fancy_logger.recent_logs.changes
+
+    def logs(self) -> typing.List[str]:
+        """
+        Returns a list of the most recent log messages.
+        """
+        return fancy_logger.recent_logs.get_all()
+
 
 def run_cli():
     """
     Run the bot from the command line.  Blocks until the bot exits.
 
     This is the main entrypoint for the CLI.
```

### Comparing `oobabot-0.2.0/src/oobabot/overengineered_settings_parser.py` & `oobabot-0.2.1/src/oobabot/overengineered_settings_parser.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.2.0/src/oobabot/persona.py` & `oobabot-0.2.1/src/oobabot/persona.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.2.0/src/oobabot/prompt_generator.py` & `oobabot-0.2.1/src/oobabot/prompt_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -189,24 +189,7 @@
         message_history_txt = ""
         if message_history is not None:
             message_history_txt = await self._render_history(
                 message_history,
             )
         image_coming = self.image_request_made if image_requested else ""
         return self._generate(message_history_txt, image_coming)
-
-    def keyword_generation_prompt(
-        self,
-        image_request_message: types.GenericMessage,
-    ) -> str:
-        """
-        given a message that requests an image, generate a prompt
-        to the AI to take that message text and generate a set of
-        keywords describing that image
-        """
-        return self.template_store.format(
-            templates.Templates.PROMPT_IMAGE_KEYWORDS,
-            {
-                templates.TemplateToken.AI_NAME: self.persona.ai_name,
-                templates.TemplateToken.USER_MESSAGE: image_request_message.body_text,
-            },
-        )
```

### Comparing `oobabot-0.2.0/src/oobabot/repetition_tracker.py` & `oobabot-0.2.1/src/oobabot/repetition_tracker.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.2.0/src/oobabot/response_stats.py` & `oobabot-0.2.1/src/oobabot/response_stats.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.2.0/src/oobabot/runtime.py` & `oobabot-0.2.1/src/oobabot/runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
         self.stable_diffusion_client: typing.Optional[
             sd_client.StableDiffusionClient
         ] = None
         sd_settings = settings.stable_diffusion_settings.get_all()
         if sd_settings["stable_diffusion_url"]:
             self.stable_diffusion_client = sd_client.StableDiffusionClient(
                 settings=sd_settings,
+                magic_model_key=settings.SD_CLIENT_MAGIC_MODEL_KEY,
             )
 
         ########################################################
         # Bot logic
 
         self.persona = persona.Persona(
             persona_settings=settings.persona_settings.get_all()
```

### Comparing `oobabot-0.2.0/src/oobabot/sd_client.py` & `oobabot-0.2.1/src/oobabot/sd_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,34 +2,48 @@
 """
 Client for generating images using the AUTOMATIC1111
 API.  Takes a prompt and returns image binary data in PNG format.
 """
 
 import asyncio
 import base64
+import re
 import time
 import typing
 
 import aiohttp
 
 from oobabot import fancy_logger
 from oobabot import http_client
 
 # todo: response stats for SD client
 
 
+def _find_substring_in_dict(
+    desired_val: str, search_list: typing.List
+) -> typing.Optional[str]:
+    desired_val = desired_val.lower()
+    for value in search_list:
+        if value.lower() in desired_val:
+            return value
+    return None
+
+
 class StableDiffusionClient(http_client.SerializedHttpClient):
     """
     Purpose: Client for generating images using the AUTOMATIC1111
     API.  Takes a prompt and returns image binary data in PNG format.
     """
 
     SERVICE_NAME = "Stable Diffusion"
     STABLE_DIFFUSION_API_URI_PATH: str = "/sdapi/v1/"
 
+    SAMPLER_KEY = "sampler_name"
+    SAMPLER_KEY_ALIAS = "sampler"
+
     API_COMMAND_URLS = {
         "get_samplers": STABLE_DIFFUSION_API_URI_PATH + "samplers",
         # get_samplers: GET only
         #   returns a list of samplers which we can use
         #   in text2img
         "options": STABLE_DIFFUSION_API_URI_PATH + "options",
         # options: GET and POST
@@ -56,20 +70,41 @@
         # ...
         # ]
     }
 
     def __init__(
         self,
         settings: typing.Dict[str, typing.Any],
+        magic_model_key: str,
     ):
         super().__init__(self.SERVICE_NAME, settings["stable_diffusion_url"])
 
         self.extra_prompt_text = settings["extra_prompt_text"]
         self.request_params = settings["request_params"]
+
+        # lower-case all keys in request_params
+        self.request_params = {k.lower(): v for k, v in self.request_params.items()}
         self.sd_models = []
+        self.sd_samplers = []
+
+        self.user_override_params = {}
+        # ensure that each customizable param is in the request_params
+        for param in settings["user_override_params"]:
+            param = param.lower()
+            if param not in self.request_params:
+                fancy_logger.get().warning(
+                    "Stable Diffusion:  customizable param '%s' not in request_params."
+                    + "  Ignoring setting.",
+                    param,
+                )
+                continue
+            # store the type of the param, so we can validate user input later
+            self.user_override_params[param] = type(self.request_params[param])
+
+        self.magic_model_key = magic_model_key.lower()
 
         # when we're in a "age restricted" channel, we'll swap
         # the "negative_prompt" in the request_params with this
         # value.  Otherwise we'll use the one already in
         # request_params["negative_prompt"]
         self.negative_prompt_nsfw = self.request_params.pop("negative_prompt_nsfw", "")
 
@@ -157,14 +192,148 @@
 
     async def get_samplers(self) -> typing.List[str]:
         return await self._call_and_extract_field("get_samplers", "name")
 
     async def get_models(self) -> typing.List[str]:
         return await self._call_and_extract_field("sd-models", "model_name")
 
+    SD_DELIMITER = "="
+
+    def _find_model(self, desired_model: str) -> typing.Optional[str]:
+        return _find_substring_in_dict(desired_model, self.sd_models)
+
+    def _find_sampler(self, desired_sampler: str) -> typing.Optional[str]:
+        return _find_substring_in_dict(desired_sampler, self.sd_samplers)
+
+    def _to_key_value_pair(
+        self, word: str
+    ) -> typing.Optional[typing.Tuple[str, typing.Any]]:
+        if self.SD_DELIMITER not in word:
+            return None
+
+        keyword_pair = word.split(self.SD_DELIMITER, 1)
+        if len(keyword_pair) < 2:
+            return None
+        key, val = keyword_pair
+
+        # lowercase the key, so we can match it against the
+        # user_override_params dict
+        key = key.lower()
+
+        # magical alias for "negative_prompt"
+        if key == "np":
+            key = "negative_prompt"
+
+        if key == self.SAMPLER_KEY_ALIAS:
+            key = self.SAMPLER_KEY
+
+        if key not in self.user_override_params:
+            return None
+
+        # try to remove any quotes around the value
+        if val.startswith('"') and val.endswith('"'):
+            val = val[1:-1]
+
+        try:
+            val_type = self.user_override_params[key]
+            if val_type == bool:
+                if val.lower in ("true", "yes", "y"):
+                    val = True
+                elif val.lower in ("false", "no", "n"):
+                    val = False
+            elif val_type == int:
+                val = int(val)
+            elif val_type == float:
+                val = float(val)
+        except ValueError:
+            return None
+
+        return (key, val)
+
+    def update_model_and_sampler(self, params: typing.Dict[str, typing.Any]):
+        """
+        Model and Sampler are special since we have a list of known acceptable
+        values.  If the user specifies a value that is not in the list, we
+        ignore it.  If the user specifies a value that is in the list, we
+        override the default.
+
+        Also, "sampler" is an alias for "sampler_name", and "model" is an
+        alias for what should appear in "override_settings.sd_model_checkpoint".
+
+        Finally, we allow the user to specify a substring of the model or
+        sampler name, and we will match the first one we find.  This is
+        useful for when the user doesn't know the exact name of the model
+        or sampler, but knows a substring of it.
+        """
+        desired_model = params.pop(self.magic_model_key, None)
+        if desired_model is not None:
+            model = self._find_model(desired_model)
+            if model is not None:
+                if "override_settings" not in params:
+                    params["override_settings"] = {}
+                params["override_settings"]["sd_model_checkpoint"] = model
+                fancy_logger.get().debug(
+                    "Stable Diffusion: per user request, setting model to '%s'", model
+                )
+            else:
+                fancy_logger.get().debug(
+                    "Stable Diffusion: unavailable model requested.  "
+                    + "If newly added, restart oobabot: '%s'",
+                    desired_model,
+                )
+
+        # the proper key is "sampler_name", but we also allow
+        # "sampler" for convenience.  Move the value, if any, over now.
+        desired_sampler = params.pop(self.SAMPLER_KEY_ALIAS, None)
+        if desired_sampler is not None:
+            params[self.SAMPLER_KEY] = desired_sampler
+
+        desired_sampler = params.pop(self.SAMPLER_KEY, None)
+        if desired_sampler is not None:
+            sampler = self._find_sampler(desired_sampler)
+            if sampler is not None:
+                params[self.SAMPLER_KEY] = sampler
+            else:
+                fancy_logger.get().debug(
+                    "Stable Diffusion: unavailable sampler requested.  "
+                    + "If newly added, restart oobabot: '%s'",
+                    desired_sampler,
+                )
+
+    # this is intended to split the prompt into words, but
+    # also to handle quoted strings.  For instance, if the
+    # prompt is:
+    #   "zombie taylor swift" pinup movie poster
+    # then we want to split it into:
+    #   ["zombie taylor swift", "pinup", "movie", "poster"]
+    #
+    SD_PARAM_SPLIT_REGEX = re.compile(r'(?:".*?"|\S)+')
+
+    def update_params(self, prompt: str, params: typing.Dict[str, typing.Any]) -> str:
+        """
+        Updates the request parameters included in the given prompt,
+        and then returns the remaining prompt.
+        """
+        remaining_prompt = ""
+        for word in self.SD_PARAM_SPLIT_REGEX.findall(prompt):
+            key_val_pair = self._to_key_value_pair(word)
+            if key_val_pair is None:
+                remaining_prompt += word + " "
+                continue
+            key, val = key_val_pair
+
+            fancy_logger.get().debug(
+                "Stable Diffusion: per user request, setting '%s' to '%s'", key, val
+            )
+            params[key] = val
+
+        self.update_model_and_sampler(params)
+
+        return remaining_prompt.strip()
+
     def generate_image(
         self,
         prompt: str,
         is_channel_nsfw: bool = False,
     ) -> "asyncio.Task[bytes]":
         """
         Generate an image from a prompt.
@@ -174,42 +343,31 @@
             this will change the negative prompt.
         Returns:
             The image as bytes.
         Raises:
             OobaHttpClientError, if the request fails.
         """
         request = self.request_params.copy()
-        request["prompt"] = prompt
+
         if is_channel_nsfw:
             request["negative_prompt"] = self.negative_prompt_nsfw
 
-        # try to extract a model name from the prompt.  If we do,
-        # set it via ['override_settings']['sd_model_checkpoint']
-        lower_prompt = prompt.lower()
-        for model in self.sd_models:
-            if model.lower() in lower_prompt:
-                if "override_settings" not in request:
-                    request["override_settings"] = {}
-                request["override_settings"]["sd_model_checkpoint"] = model
-
-                fancy_logger.get().debug(
-                    "Stable Diffusion:  setting model to '%s'", model
-                )
-                # remove the model name from the prompt itself
-                request["prompt"] = request["prompt"].replace(model, "")
-                break
+        # extract any allowed user overrides from the prompt
+        # and add them to the request dict.  The remaining
+        # prompt is returned.
+        request["prompt"] = self.update_params(prompt, request)
 
         if self.extra_prompt_text:
             request["prompt"] += ", " + self.extra_prompt_text
 
         async def do_post() -> bytes:
             fancy_logger.get().debug(
                 "Stable Diffusion: Image request (nsfw: %r): %s",
                 is_channel_nsfw,
-                request["prompt"],
+                request,
             )
             start_time = time.time()
 
             async with self._get_session().post(
                 self.API_COMMAND_URLS["txt2img"],
                 json=request,
             ) as response:
@@ -248,52 +406,65 @@
                         err,
                     )
                     await asyncio.sleep(1)
                     tries += 1
 
         return asyncio.create_task(do_post_with_retry())
 
-    async def verify_sampler_available(self):
-        """
-        Checks that the requested sampler is available on the server.
-        If it isn't, logs a warning and sets the sampler to the default.
-        """
-        samplers = await self.get_samplers()
-
-        desired_sampler = self.request_params.get("sampler")
-        if not desired_sampler:
-            fancy_logger.get().debug(
-                "Stable Diffusion: Using default sampler on SD server"
-            )
-            return
-
-        if desired_sampler in samplers:
-            fancy_logger.get().debug(
-                "Stable Diffusion: Using desired sampler '%s'", desired_sampler
-            )
-            return
-
-        fancy_logger.get().warning(
-            "Stable Diffusion: Desired sampler '%s' not available",
-            desired_sampler,
-        )
-        fancy_logger.get().info(
-            "Stable Diffusion: Available samplers: %s", ", ".join(samplers)
-        )
-        self.request_params["sampler"] = ""
-
     async def _setup(self):
-        await self.verify_sampler_available()
         await self.set_options()
         self.sd_models = await self.get_models()
+        self.sd_samplers = await self.get_samplers()
         fancy_logger.get().info(
             "Stable Diffusion: Available models: %s", ", ".join(self.sd_models)
         )
+        # log a warning if the default model is not available
+        desired_model = self.request_params.get(self.magic_model_key, None)
+        if desired_model:
+            model = self._find_model(desired_model)
+            if model is None:
+                fancy_logger.get().warning(
+                    "Stable Diffusion: Desired default model '%s' not available.",
+                    desired_model,
+                )
+            else:
+                fancy_logger.get().debug(
+                    "Stable Diffusion: Using default model '%s'", desired_model
+                )
+
+        fancy_logger.get().info(
+            "Stable Diffusion: Available samplers: %s", ", ".join(self.sd_samplers)
+        )
+        # log a warning if the default sampler is not available
+        desired_sampler = self.request_params.get(
+            self.SAMPLER_KEY_ALIAS, self.request_params.get(self.SAMPLER_KEY, None)
+        )
+        if desired_sampler:
+            sampler = self._find_sampler(desired_sampler)
+            if sampler is None:
+                fancy_logger.get().warning(
+                    "Stable Diffusion: Desired default sampler '%s' not available.",
+                    desired_sampler,
+                )
+            else:
+                fancy_logger.get().debug(
+                    "Stable Diffusion: Using default sampler '%s'", desired_sampler
+                )
+
         fancy_logger.get().debug(
             "Stable Diffusion: Using negative prompt: %s...",
             str(self.request_params.get("negative_prompt", ""))[:20],
         )
         if self.extra_prompt_text:
             fancy_logger.get().debug(
-                "Stable Diffusion: will append to every prompt: '%s'",
+                "Stable Diffusion: Bot will append to every prompt: '%s'",
                 self.extra_prompt_text,
             )
+        if 0 == len(self.user_override_params):
+            fancy_logger.get().debug(
+                "Stable Diffusion: Users cannot override any SD params"
+            )
+        else:
+            fancy_logger.get().debug(
+                "Stable Diffusion: Users may override: %s",
+                ", ".join(self.user_override_params.keys()),
+            )
```

### Comparing `oobabot-0.2.0/src/oobabot/settings.py` & `oobabot-0.2.1/src/oobabot/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,18 +70,14 @@
     environment variables and command line arguments.
     """
 
     ############################################################
     # This section is for constants which are not yet
     # customizable by the user.
 
-    # when trying to stop the bot, wait this long before
-    # giving up and just exiting
-    STOP_LOCK_TIMEOUT: float = 5.0
-
     # This is a table of the probability that the bot will respond
     # in an unsolicited manner (i.e. it isn't specifically pinged)
     # to a message, based on how long ago it was pinged in that
     # same channel.
     TIME_VS_RESPONSE_CHANCE: typing.List[typing.Tuple[float, float]] = [
         # (seconds, base % chance of an unsolicited response)
         (60.0, 0.90),
@@ -133,34 +129,49 @@
     # use this prompt for "age_restricted" Discord channels
     #  i.e. channel.nsfw is true
     DEFAULT_SD_NEGATIVE_PROMPT_NSFW: str = "animal harm, suicide, loli"
 
     # use this prompt for non-age-restricted channels
     DEFAULT_SD_NEGATIVE_PROMPT: str = DEFAULT_SD_NEGATIVE_PROMPT_NSFW + ", nsfw"
 
+    SD_CLIENT_MAGIC_MODEL_KEY = "model"
+
     DEFAULT_SD_REQUEST_PARAMS: typing.Dict[str, typing.Union[bool, int, str]] = {
-        # default values are commented out
-        #
-        # "do_not_save_samples": False,
+        "cfg_scale": 7,
         #    This is a privacy concern for the users of the service.
         #    We don't want to save the generated images anyway, since they
         #    are going to be on Discord.  Also, we don't want to use the
         #    disk space.
         "do_not_save_samples": True,
-        #
-        # "do_not_save_grid": False,
-        #    Sames as above.
         "do_not_save_grid": True,
+        "enable_hr": False,
+        # this is a fake setting, SD calls it "sd_model_checkpoint",
+        # and it needs to appear under "override_params".  But put it here
+        # for convenience, the SD client will do the right thing with it.
+        SD_CLIENT_MAGIC_MODEL_KEY: "",
         "negative_prompt": DEFAULT_SD_NEGATIVE_PROMPT,
         "negative_prompt_nsfw": DEFAULT_SD_NEGATIVE_PROMPT_NSFW,
+        "sampler_name": "",
+        "seed": -1,
         "steps": 30,
         "width": 512,
         "height": 512,
-        "sampler": "",
     }
+
+    DEFAULT_SD_USER_OVERRIDE_PARAMS = [
+        "cfg_scale",
+        "enable_hr",
+        SD_CLIENT_MAGIC_MODEL_KEY,
+        "negative_prompt",
+        "sampler_name",
+        "seed",
+        "height",
+        "width",
+    ]
+
     # words to look for in the prompt to indicate that the user
     # wants to generate an image
     DEFAULT_IMAGE_WORDS: typing.List[str] = [
         "draw me",
         "drawing",
         "photo",
         "pic",
@@ -469,18 +480,17 @@
         self.discord_settings.add_setting(
             oesp.ConfigSetting[int](
                 name="unsolicited_channel_cap",
                 default=3,
                 description_lines=[
                     textwrap.dedent(
                         """
-                        FEATURE PREVIEW: Adds a limit to the number of channels
-                        the bot will post unsolicited messages in at the same
-                        time.  This is to prevent the bot from being too noisy
-                        in large servers.
+                        Adds a limit to the number of channels the bot will post
+                        unsolicited messages in at the same time.  This is to
+                        prevent the bot from being too noisy in large servers.
 
                         When set, only the most recent N channels the bot has
                         been summoned in will have a chance of receiving an
                         unsolicited message.  The bot will still respond to
                         @-mentions and wake words in any channel it can access.
 
                         Set to 0 to disable this feature.
@@ -673,30 +683,45 @@
                 ],
                 include_in_argparse=False,
                 show_default_in_yaml=False,
                 place_default_in_yaml=True,
             )
         )
         self.stable_diffusion_settings.add_setting(
-            oesp.ConfigSetting[bool](
-                name="use_ai_generated_keywords",
-                default=False,
+            oesp.ConfigSetting[list](
+                name="user_override_params",
+                default=self.DEFAULT_SD_USER_OVERRIDE_PARAMS,
                 description_lines=[
                     textwrap.dedent(
                         """
-                        FEATURE PREVIEW: If set, the bot will ask Oobabooga to generate
-                        image keywords from a user's message.  It will then pass the
-                        keywords that Oobabooga produces to Stable Diffusion to finally
-                        generate an image.
-                        Otherwise, the bot will simply extract keywords directly
-                        from the user's message using a simple regex.
+                        These parameters can be overridden by the Discord user
+                        by including them in their image generation request.
+
+                        The format for this is: param_name=value
+
+                        This is a whitelist of parameters that can be overridden.
+                        They must be simple parameters (strings, numbers, booleans),
+                        and they must be in the request_params dictionary.
+
+                        The value the user inputs will be checked against the type
+                        from the request_params dictionary, and if it doesn't match,
+                        the default value will be used instead.
+
+                        Otherwise, this value will be passed through to Stable
+                        Diffusion without any changes, so be mindful of what you allow
+                        here.  It could potentially be used to inject malicious
+                        values into your SD server.
+
+                        For example, steps=1000000 could be bad for your server.
                         """
                     )
                 ],
                 include_in_argparse=False,
+                show_default_in_yaml=False,
+                place_default_in_yaml=True,
             )
         )
 
         ###########################################################
         # Template Settings
 
         self.template_settings = oesp.ConfigSettingGroup(
```

### Comparing `oobabot-0.2.0/src/oobabot/templates.py` & `oobabot-0.2.1/src/oobabot/templates.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,17 +25,14 @@
     IMAGE_UNAUTHORIZED = "image_unauthorized"
 
     # prompts to the AI to generate text responses
     PROMPT = "prompt"
     PROMPT_HISTORY_LINE = "prompt_history_line"
     PROMPT_IMAGE_COMING = "prompt_image_coming"
 
-    # prompts to the AI to generate image keywords
-    PROMPT_IMAGE_KEYWORDS = "prompt_image_keywords"
-
     def __str__(self) -> str:
         return self.value
 
     def __lt__(self, other: "Templates") -> bool:
         return str(self.value) < str(other.value)
 
 
@@ -105,26 +102,14 @@
                 TemplateToken.AI_NAME,
             ],
             "Part of the AI response-generation prompt, this is used to "
             + "inform the AI that it is in the process of generating an "
             + "image.",
             True,
         ),
-        Templates.PROMPT_IMAGE_KEYWORDS: (
-            [
-                TemplateToken.AI_NAME,
-                TemplateToken.USER_MESSAGE,
-            ],
-            """
-            Sent to Oobabooga, along with the user's image request, to generate
-            image keywords.  The AI's response to this prompt will then be sent
-            to Stable Diffusion to generate an image.
-            """,
-            True,
-        ),
         Templates.IMAGE_DETACH: (
             [
                 TemplateToken.IMAGE_PROMPT,
                 TemplateToken.USER_NAME,
             ],
             "Shown in Discord when the user selects to discard an image "
             + "that Stable Diffusion had generated.",
@@ -183,30 +168,14 @@
             """
         ),
         Templates.PROMPT_IMAGE_COMING: textwrap.dedent(
             """
             {AI_NAME}: is currently generating an image, as requested.
             """
         ),
-        Templates.PROMPT_IMAGE_KEYWORDS: textwrap.dedent(
-            """
-            Below is an instruction that describes a task, paired with an input
-            that provides further context. Write a response that appropriately
-            completes the request.
-
-            ### Instruction:
-            The input text asks for an image to be created.  Please create a list
-            of keywords to describe that image.
-
-            ### Input:
-            {USER_MESSAGE}
-
-            ### Response:
-            """
-        ),
         Templates.IMAGE_DETACH: textwrap.dedent(
             """
             {USER_NAME} asked for an image with the prompt:
                 '{IMAGE_PROMPT}'
             ...but couldn't find a suitable one.
             """
         ),
```

### Comparing `oobabot-0.2.0/src/oobabot/transcript.py` & `oobabot-0.2.1/src/oobabot/transcript.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.2.0/src/oobabot/types.py` & `oobabot-0.2.1/src/oobabot/types.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.2.0/src/oobabot/voice_client.py` & `oobabot-0.2.1/src/oobabot/voice_client.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.2.0/PKG-INFO` & `oobabot-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oobabot
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Discord bot which talks to Large Language Model AIs running on oobabooga's text-generation-webui
 Home-page: https://github.com/chrisrude/oobabot
 License: MIT
 Author: Christopher Rude
 Author-email: chris@rudesoftware.net
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -99,15 +99,15 @@
                [--discord-token DISCORD_TOKEN] [--dont-split-responses]
                [--history-lines HISTORY_LINES] [--ignore-dms] [--reply-in-thread]
                [--stream-responses] [--base-url BASE_URL] [--log-all-the-things]
                [--message-regex MESSAGE_REGEX] [--image-words [IMAGE_WORDS ...]]
                [--stable-diffusion-url STABLE_DIFFUSION_URL]
                [--extra-prompt-text EXTRA_PROMPT_TEXT]
 
-oobabot v0.2.0: Discord bot for oobabooga's text-generation-webui
+oobabot v0.2.1: Discord bot for oobabooga's text-generation-webui
 
 General Settings:
 
   -h, --help
   -c CONFIG, --config CONFIG
                         Path to a config file to read settings from. Command line settings
                         will override settings in this file. (default: config.yml)
```

