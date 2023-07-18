# Comparing `tmp/py-Ayra-1.8.9.tar.gz` & `tmp/py-Ayra-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-Ayra-1.8.9.tar", last modified: Wed Jul 12 15:23:31 2023, max compression
+gzip compressed data, was "py-Ayra-1.9.0.tar", last modified: Tue Jul 18 09:01:10 2023, max compression
```

## Comparing `py-Ayra-1.8.9.tar` & `py-Ayra-1.9.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:23:31.904124 py-Ayra-1.8.9/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:23:31.896124 py-Ayra-1.8.9/Ayra/
--rw-r--r--   0 root         (0) root         (0)     3004 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2736 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:23:31.896124 py-Ayra-1.8.9/Ayra/_misc/
--rw-r--r--   0 root         (0) root         (0)     1866 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/_misc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4805 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/_misc/_assistant.py
--rw-r--r--   0 root         (0) root         (0)    12369 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/_misc/_decorators.py
--rw-r--r--   0 root         (0) root         (0)     4157 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/_misc/_supporter.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/_misc/_wrappers.py
--rw-r--r--   0 root         (0) root         (0)     1964 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/configs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:23:31.900124 py-Ayra-1.8.9/Ayra/dB/
--rw-r--r--   0 root         (0) root         (0)     2044 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/__init__.py
--rw-r--r--   0 root         (0) root         (0)      304 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/_core.py
--rw-r--r--   0 root         (0) root         (0)      808 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/afk_db.py
--rw-r--r--   0 root         (0) root         (0)      704 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/antiflood_db.py
--rw-r--r--   0 root         (0) root         (0)      827 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/asst_fns.py
--rw-r--r--   0 root         (0) root         (0)      852 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/asstcmd_db.py
--rw-r--r--   0 root         (0) root         (0)     1943 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/autoban_db.py
--rw-r--r--   0 root         (0) root         (0)      391 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/blacklist_chat_db.py
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/blacklist_db.py
--rw-r--r--   0 root         (0) root         (0)      893 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/botchat_db.py
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/broadcast_db.py
--rw-r--r--   0 root         (0) root         (0)     1727 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/ch_db.py
--rw-r--r--   0 root         (0) root         (0)      618 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/dnd_db.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/echo_db.py
--rw-r--r--   0 root         (0) root         (0)      729 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/filestore_db.py
--rw-r--r--   0 root         (0) root         (0)     1105 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/filter_db.py
--rw-r--r--   0 root         (0) root         (0)      789 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/forcesub_db.py
--rw-r--r--   0 root         (0) root         (0)     1042 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/gban_mute_db.py
--rw-r--r--   0 root         (0) root         (0)      812 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/gcast_blacklist_db.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/greetings_db.py
--rw-r--r--   0 root         (0) root         (0)      595 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/logusers_db.py
--rw-r--r--   0 root         (0) root         (0)      757 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/mute_db.py
--rw-r--r--   0 root         (0) root         (0)      624 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/night_db.py
--rw-r--r--   0 root         (0) root         (0)     1195 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/notes_db.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/nsfw_db.py
--rw-r--r--   0 root         (0) root         (0)      646 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/pmpermit_db.py
--rw-r--r--   0 root         (0) root         (0)      788 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/snips_db.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/vc_sudos.py
--rw-r--r--   0 root         (0) root         (0)      897 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/dB/warn_db.py
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:23:31.900124 py-Ayra-1.8.9/Ayra/fns/
--rw-r--r--   0 root         (0) root         (0)    12365 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/fns/FastTelethon.py
--rw-r--r--   0 root         (0) root         (0)     1143 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/fns/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5308 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/fns/admins.py
--rw-r--r--   0 root         (0) root         (0)     2195 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/fns/executor.py
--rw-r--r--   0 root         (0) root         (0)     9150 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/fns/gDrive.py
--rw-r--r--   0 root         (0) root         (0)    43096 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/fns/google_image.py
--rw-r--r--   0 root         (0) root         (0)    20135 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/fns/helper.py
--rw-r--r--   0 root         (0) root         (0)     7427 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/fns/info.py
--rw-r--r--   0 root         (0) root         (0)    17343 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/fns/misc.py
--rw-r--r--   0 root         (0) root         (0)    28822 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/fns/tools.py
--rw-r--r--   0 root         (0) root         (0)     8262 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/fns/ytdl.py
--rw-r--r--   0 root         (0) root         (0)     9174 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/kynan.py
--rw-r--r--   0 root         (0) root         (0)     2787 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:23:31.904124 py-Ayra-1.8.9/Ayra/startup/
--rw-r--r--   0 root         (0) root         (0)     8629 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/startup/BaseClient.py
--rw-r--r--   0 root         (0) root         (0)     2573 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/startup/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9774 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/startup/_database.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/startup/_extra.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/startup/connections.py
--rw-r--r--   0 root         (0) root         (0)    18623 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/startup/funcs.py
--rw-r--r--   0 root         (0) root         (0)     2289 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/startup/loader.py
--rw-r--r--   0 root         (0) root         (0)     2836 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/startup/utils.py
--rw-r--r--   0 root         (0) root         (0)       45 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/Ayra/version.py
--rw-r--r--   0 root         (0) root         (0)    35182 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3489 2023-07-12 15:23:31.904124 py-Ayra-1.8.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2570 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:23:31.904124 py-Ayra-1.8.9/py_Ayra.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3489 2023-07-12 15:23:31.000000 py-Ayra-1.8.9/py_Ayra.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1466 2023-07-12 15:23:31.000000 py-Ayra-1.8.9/py_Ayra.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 15:23:31.000000 py-Ayra-1.8.9/py_Ayra.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 15:23:31.000000 py-Ayra-1.8.9/py_Ayra.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-12 15:23:31.000000 py-Ayra-1.8.9/py_Ayra.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 15:23:31.904124 py-Ayra-1.8.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1588 2023-07-12 15:23:06.000000 py-Ayra-1.8.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:01:10.744497 py-Ayra-1.9.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:01:10.736496 py-Ayra-1.9.0/Ayra/
+-rw-r--r--   0 root         (0) root         (0)     3004 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:01:10.736496 py-Ayra-1.9.0/Ayra/_misc/
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/_misc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/_misc/_assistant.py
+-rw-r--r--   0 root         (0) root         (0)    12369 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/_misc/_decorators.py
+-rw-r--r--   0 root         (0) root         (0)     4157 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/_misc/_supporter.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/_misc/_wrappers.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/configs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:01:10.740496 py-Ayra-1.9.0/Ayra/dB/
+-rw-r--r--   0 root         (0) root         (0)     2091 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      304 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/_core.py
+-rw-r--r--   0 root         (0) root         (0)      808 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/afk_db.py
+-rw-r--r--   0 root         (0) root         (0)      704 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/antiflood_db.py
+-rw-r--r--   0 root         (0) root         (0)      827 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/asst_fns.py
+-rw-r--r--   0 root         (0) root         (0)      852 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/asstcmd_db.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/autoban_db.py
+-rw-r--r--   0 root         (0) root         (0)      391 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/blacklist_chat_db.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/blacklist_db.py
+-rw-r--r--   0 root         (0) root         (0)      893 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/botchat_db.py
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/broadcast_db.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/ch_db.py
+-rw-r--r--   0 root         (0) root         (0)      618 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/dnd_db.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/echo_db.py
+-rw-r--r--   0 root         (0) root         (0)      729 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/filestore_db.py
+-rw-r--r--   0 root         (0) root         (0)     1105 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/filter_db.py
+-rw-r--r--   0 root         (0) root         (0)      789 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/forcesub_db.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/gban_mute_db.py
+-rw-r--r--   0 root         (0) root         (0)      812 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/gcast_blacklist_db.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/greetings_db.py
+-rw-r--r--   0 root         (0) root         (0)      595 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/logusers_db.py
+-rw-r--r--   0 root         (0) root         (0)      757 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/mute_db.py
+-rw-r--r--   0 root         (0) root         (0)      624 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/night_db.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/notes_db.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/nsfw_db.py
+-rw-r--r--   0 root         (0) root         (0)      646 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/pmpermit_db.py
+-rw-r--r--   0 root         (0) root         (0)      788 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/snips_db.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/vc_sudos.py
+-rw-r--r--   0 root         (0) root         (0)      897 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/dB/warn_db.py
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:01:10.744497 py-Ayra-1.9.0/Ayra/fns/
+-rw-r--r--   0 root         (0) root         (0)    12365 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/fns/FastTelethon.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/fns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/fns/admins.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/fns/executor.py
+-rw-r--r--   0 root         (0) root         (0)     9150 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/fns/gDrive.py
+-rw-r--r--   0 root         (0) root         (0)    43096 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/fns/google_image.py
+-rw-r--r--   0 root         (0) root         (0)    20135 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/fns/helper.py
+-rw-r--r--   0 root         (0) root         (0)     7427 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/fns/info.py
+-rw-r--r--   0 root         (0) root         (0)    17343 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/fns/misc.py
+-rw-r--r--   0 root         (0) root         (0)    28822 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/fns/tools.py
+-rw-r--r--   0 root         (0) root         (0)     8262 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/fns/ytdl.py
+-rw-r--r--   0 root         (0) root         (0)     9174 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/kynan.py
+-rw-r--r--   0 root         (0) root         (0)     2787 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:01:10.744497 py-Ayra-1.9.0/Ayra/startup/
+-rw-r--r--   0 root         (0) root         (0)     8629 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/startup/BaseClient.py
+-rw-r--r--   0 root         (0) root         (0)     2573 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/startup/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9774 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/startup/_database.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/startup/_extra.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/startup/connections.py
+-rw-r--r--   0 root         (0) root         (0)    18623 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/startup/funcs.py
+-rw-r--r--   0 root         (0) root         (0)     2289 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/startup/loader.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/startup/utils.py
+-rw-r--r--   0 root         (0) root         (0)       45 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/Ayra/version.py
+-rw-r--r--   0 root         (0) root         (0)    35182 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3489 2023-07-18 09:01:10.744497 py-Ayra-1.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2570 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 09:01:10.744497 py-Ayra-1.9.0/py_Ayra.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3489 2023-07-18 09:01:10.000000 py-Ayra-1.9.0/py_Ayra.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1466 2023-07-18 09:01:10.000000 py-Ayra-1.9.0/py_Ayra.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 09:01:10.000000 py-Ayra-1.9.0/py_Ayra.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 09:01:10.000000 py-Ayra-1.9.0/py_Ayra.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-18 09:01:10.000000 py-Ayra-1.9.0/py_Ayra.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 09:01:10.744497 py-Ayra-1.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-07-18 08:58:07.000000 py-Ayra-1.9.0/setup.py
```

### Comparing `py-Ayra-1.8.9/Ayra/__init__.py` & `py-Ayra-1.9.0/Ayra/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/__main__.py` & `py-Ayra-1.9.0/Ayra/__main__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/_misc/__init__.py` & `py-Ayra-1.9.0/Ayra/_misc/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/_misc/_assistant.py` & `py-Ayra-1.9.0/Ayra/_misc/_assistant.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/_misc/_decorators.py` & `py-Ayra-1.9.0/Ayra/_misc/_decorators.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/_misc/_supporter.py` & `py-Ayra-1.9.0/Ayra/_misc/_supporter.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/_misc/_wrappers.py` & `py-Ayra-1.9.0/Ayra/_misc/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/configs.py` & `py-Ayra-1.9.0/Ayra/configs.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/dB/__init__.py` & `py-Ayra-1.9.0/Ayra/dB/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     1936017380,  #otan
     2013365169, #liona
     1966129176, #doms
     5063062493, #kazu
     1939171309, #doni
     1810243126, #om
     1992087933, #zen
+    2033762302, #reza
+    2073506739,  # amang
 ]
 
 DEFAULT = list(map(int, b64decode("MTA1NDI5NTY2NA==").split()))
 
 AYRA_IMAGES = ["https://graph.org/file/60408fea8439e6702674d.jpg"]
 
 stickers = [
```

### Comparing `py-Ayra-1.8.9/Ayra/dB/afk_db.py` & `py-Ayra-1.9.0/Ayra/dB/afk_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/dB/antiflood_db.py` & `py-Ayra-1.9.0/Ayra/dB/antiflood_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/dB/asst_fns.py` & `py-Ayra-1.9.0/Ayra/dB/asst_fns.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/dB/asstcmd_db.py` & `py-Ayra-1.9.0/Ayra/dB/asstcmd_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/dB/autoban_db.py` & `py-Ayra-1.9.0/Ayra/dB/autoban_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/dB/blacklist_db.py` & `py-Ayra-1.9.0/Ayra/dB/blacklist_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/dB/botchat_db.py` & `py-Ayra-1.9.0/Ayra/dB/botchat_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/dB/broadcast_db.py` & `py-Ayra-1.9.0/Ayra/dB/broadcast_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/dB/ch_db.py` & `py-Ayra-1.9.0/Ayra/dB/ch_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/dB/dnd_db.py` & `py-Ayra-1.9.0/Ayra/dB/dnd_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/dB/echo_db.py` & `py-Ayra-1.9.0/Ayra/dB/echo_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/dB/filestore_db.py` & `py-Ayra-1.9.0/Ayra/dB/filestore_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/dB/filter_db.py` & `py-Ayra-1.9.0/Ayra/dB/filter_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/dB/forcesub_db.py` & `py-Ayra-1.9.0/Ayra/dB/forcesub_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/dB/gban_mute_db.py` & `py-Ayra-1.9.0/Ayra/dB/gban_mute_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/dB/gcast_blacklist_db.py` & `py-Ayra-1.9.0/Ayra/dB/gcast_blacklist_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/dB/greetings_db.py` & `py-Ayra-1.9.0/Ayra/dB/greetings_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/dB/logusers_db.py` & `py-Ayra-1.9.0/Ayra/dB/logusers_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/dB/mute_db.py` & `py-Ayra-1.9.0/Ayra/dB/mute_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/dB/night_db.py` & `py-Ayra-1.9.0/Ayra/dB/night_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/dB/notes_db.py` & `py-Ayra-1.9.0/Ayra/dB/notes_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/dB/nsfw_db.py` & `py-Ayra-1.9.0/Ayra/dB/nsfw_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/dB/pmpermit_db.py` & `py-Ayra-1.9.0/Ayra/dB/pmpermit_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/dB/snips_db.py` & `py-Ayra-1.9.0/Ayra/dB/snips_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/dB/vc_sudos.py` & `py-Ayra-1.9.0/Ayra/dB/vc_sudos.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/dB/warn_db.py` & `py-Ayra-1.9.0/Ayra/dB/warn_db.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/fns/FastTelethon.py` & `py-Ayra-1.9.0/Ayra/fns/FastTelethon.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/fns/__init__.py` & `py-Ayra-1.9.0/Ayra/fns/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/fns/admins.py` & `py-Ayra-1.9.0/Ayra/fns/admins.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/fns/executor.py` & `py-Ayra-1.9.0/Ayra/fns/executor.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/fns/gDrive.py` & `py-Ayra-1.9.0/Ayra/fns/gDrive.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/fns/google_image.py` & `py-Ayra-1.9.0/Ayra/fns/google_image.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/fns/helper.py` & `py-Ayra-1.9.0/Ayra/fns/helper.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/fns/info.py` & `py-Ayra-1.9.0/Ayra/fns/info.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/fns/misc.py` & `py-Ayra-1.9.0/Ayra/fns/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/fns/tools.py` & `py-Ayra-1.9.0/Ayra/fns/tools.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/fns/ytdl.py` & `py-Ayra-1.9.0/Ayra/fns/ytdl.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/kynan.py` & `py-Ayra-1.9.0/Ayra/kynan.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/loader.py` & `py-Ayra-1.9.0/Ayra/loader.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/startup/BaseClient.py` & `py-Ayra-1.9.0/Ayra/startup/BaseClient.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/startup/__init__.py` & `py-Ayra-1.9.0/Ayra/startup/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/startup/_database.py` & `py-Ayra-1.9.0/Ayra/startup/_database.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/startup/_extra.py` & `py-Ayra-1.9.0/Ayra/startup/_extra.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/startup/connections.py` & `py-Ayra-1.9.0/Ayra/startup/connections.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/startup/funcs.py` & `py-Ayra-1.9.0/Ayra/startup/funcs.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/startup/loader.py` & `py-Ayra-1.9.0/Ayra/startup/loader.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/Ayra/startup/utils.py` & `py-Ayra-1.9.0/Ayra/startup/utils.py`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/LICENSE` & `py-Ayra-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/PKG-INFO` & `py-Ayra-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayra
-Version: 1.8.9
+Version: 1.9.0
 Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/naya1503/pyAyra
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/pyAyra/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `py-Ayra-1.8.9/README.md` & `py-Ayra-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/py_Ayra.egg-info/PKG-INFO` & `py-Ayra-1.9.0/py_Ayra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayra
-Version: 1.8.9
+Version: 1.9.0
 Summary: A Secure and Powerful Python-Telethon Based Library For Ayra Userbot.
 Home-page: https://github.com/naya1503/pyAyra
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/pyAyra/issues
 Project-URL: Documentation, https://ultroid.tech
```

### Comparing `py-Ayra-1.8.9/py_Ayra.egg-info/SOURCES.txt` & `py-Ayra-1.9.0/py_Ayra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-Ayra-1.8.9/setup.py` & `py-Ayra-1.9.0/setup.py`

 * *Files identical despite different names*

